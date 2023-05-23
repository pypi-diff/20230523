# Comparing `tmp/tmlt_analytics-0.7.0rc1.tar.gz` & `tmp/tmlt_analytics-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.7.0rc1.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.7.1.tar", max compression
```

## Comparing `tmlt_analytics-0.7.0rc1.tar` & `tmlt_analytics-0.7.1.tar`

### file list

```diff
@@ -1,159 +1,167 @@
--rw-r--r--   0        0        0    13178 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/LICENSE
--rw-r--r--   0        0        0    20138 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/LICENSE.docs
--rw-r--r--   0        0        0      121 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/NOTICE
--rw-r--r--   0        0        0     2597 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/README.md
--rw-r--r--   0        0        0      951 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/package-name.html
--rw-r--r--   0        0        0     1108 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/citing.rst
--rw-r--r--   0        0        0      201 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/index.rst
--rw-r--r--   0        0        0      670 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/license.rst
--rw-r--r--   0        0        0     3159 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/privacy_policy.rst
--rw-r--r--   0        0        0     6764 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/conf.py
--rw-r--r--   0        0        0   118378 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0    34101 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_books_by_unique_members.png
--rw-r--r--   0        0        0   104926 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    59042 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    30330 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_genres_by_age.png
--rw-r--r--   0        0        0    14782 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    20226 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    23590 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/flow_chart_truncation.svg
--rw-r--r--   0        0        0    14685 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_api.svg
--rw-r--r--   0        0        0     1196 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    30903 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/logo.png
--rw-r--r--   0        0        0     3971 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/index.rst
--rw-r--r--   0        0        0     4960 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/installation.rst
--rw-r--r--   0        0        0      662 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     2024 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3440 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/templates/python/module.rst
--rw-r--r--   0        0        0     1602 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/bigquery-setup.rst
--rw-r--r--   0        0        0     3022 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/docker-image.rst
--rw-r--r--   0        0        0     1237 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/index.rst
--rw-r--r--   0        0        0     6303 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/inputs-outputs.rst
--rw-r--r--   0        0        0     5770 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/parameters.rst
--rw-r--r--   0        0        0     4763 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/running-the-program.rst
--rw-r--r--   0        0        0     1716 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/setup.rst
--rw-r--r--   0        0        0      405 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11697 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8608 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     6595 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     7726 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0     2735 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/troubleshooting.rst
--rw-r--r--   0        0        0     8462 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9124 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7246 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18802 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0      430 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/index.rst
--rw-r--r--   0        0        0    11634 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/more-with-privacy-ids.rst
--rw-r--r--   0        0        0     7732 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    11302 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-id-basics.rst
--rw-r--r--   0        0        0    16226 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0     4789 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/interactive_evaluation.ipynb
--rw-r--r--   0        0        0     5459 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/private_join.ipynb
--rw-r--r--   0        0        0     6570 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/zcdp_puredp_switching.ipynb
--rw-r--r--   0        0        0     4469 2023-04-17 23:55:55.706036 tmlt_analytics-0.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/__init__.py
--rw-r--r--   0        0        0     6976 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/conftest.py
--rw-r--r--   0        0        0      115 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/__init__.py
--rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/__init__.py
--rw-r--r--   0        0        0     4265 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/conftest.py
--rw-r--r--   0        0        0      151 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/__init__.py
--rw-r--r--   0        0        0    15227 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_constraint_propagation.py
--rw-r--r--   0        0        0    21707 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l0_linf_truncation.py
--rw-r--r--   0        0        0    14517 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l1_truncation.py
--rw-r--r--   0        0        0     4011 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_partition.py
--rw-r--r--   0        0        0      143 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/mixed/__init__.py
--rw-r--r--   0        0        0     5087 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/mixed/test_mixed_session.py
--rw-r--r--   0        0        0      152 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/__init__.py
--rw-r--r--   0        0        0    25557 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/conftest.py
--rw-r--r--   0        0        0    38557 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows.py
--rw-r--r--   0        0        0     6134 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_in_max_groups.py
--rw-r--r--   0        0        0    13790 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_infs_nulls.py
--rw-r--r--   0        0        0     7754 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_invalid.py
--rw-r--r--   0        0        0     2212 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/test_invalid_constraints.py
--rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/__init__.py
--rw-r--r--   0        0        0      298 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    75163 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    54429 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0      107 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/__init__.py
--rw-r--r--   0        0        0    17843 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/conftest.py
--rw-r--r--   0        0        0    24159 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
--rw-r--r--   0        0        0    36757 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
--rw-r--r--   0        0        0     7610 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
--rw-r--r--   0        0        0    14086 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     2301 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_catalog.py
--rw-r--r--   0        0        0      657 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_cleanup.py
--rw-r--r--   0        0        0     5285 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_constraints.py
--rw-r--r--   0        0        0    21191 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_keyset.py
--rw-r--r--   0        0        0    13993 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3058 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     5865 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5420 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     3011 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    40864 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    63485 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16715 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     4904 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    84468 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_session.py
--rw-r--r--   0        0        0     1604 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_table_identifiers.py
--rw-r--r--   0        0        0     5371 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_transformation_utils.py
--rw-r--r--   0        0        0      792 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_utils.py
--rw-r--r--   0        0        0       37 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test_requirements.txt
--rw-r--r--   0        0        0      222 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     3666 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0    16188 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation.py
--rw-r--r--   0        0        0     6110 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0     5428 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     2289 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0     9786 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0     7694 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
--rw-r--r--   0        0        0    34784 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    46272 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0    59768 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    12656 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0     1250 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_identifier.py
--rw-r--r--   0        0        0     3979 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_reference.py
--rw-r--r--   0        0        0    10147 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_transformation_utils.py
--rw-r--r--   0        0        0    11663 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      306 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0      288 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_base.py
--rw-r--r--   0        0        0      735 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_simplify.py
--rw-r--r--   0        0        0    12819 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_truncation.py
--rw-r--r--   0        0        0    11850 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0     7155 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     5471 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   126388 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    41097 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    72500 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3031 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     4772 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0rc1/setup.py
--rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    16001 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/LICENSE
+-rw-r--r--   0        0        0    20138 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/LICENSE.docs
+-rw-r--r--   0        0        0      121 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/NOTICE
+-rw-r--r--   0        0        0     2597 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/README.md
+-rw-r--r--   0        0        0      951 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/_templates/package-name.html
+-rw-r--r--   0        0        0     6786 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/conf.py
+-rw-r--r--   0        0        0     1602 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3022 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1237 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6303 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5770 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4763 2023-05-23 19:26:33.524537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1716 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0      314 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/index.rst
+-rw-r--r--   0        0        0     4783 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/installation.rst
+-rw-r--r--   0        0        0     2735 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/howto-guides/troubleshooting.rst
+-rw-r--r--   0        0        0   118378 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0    34101 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2023-05-23 19:26:33.528537 tmlt_analytics-0.7.1/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    20226 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    18639 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/flat_map_row_example.svg
+-rw-r--r--   0        0        0    23590 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0    14685 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_api.svg
+-rw-r--r--   0        0        0      609 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_howto_guides.svg
+-rw-r--r--   0        0        0     1196 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    23369 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/intuitive_noise_visualization.png
+-rw-r--r--   0        0        0    30903 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/logo.png
+-rw-r--r--   0        0        0    59239 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/private_join_example.svg
+-rw-r--r--   0        0        0    35838 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/private_join_tables.svg
+-rw-r--r--   0        0        0    32227 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/images/public_join_example_zips.svg
+-rw-r--r--   0        0        0     5748 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/index.rst
+-rw-r--r--   0        0        0      662 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     3169 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/privacy-policy.rst
+-rw-r--r--   0        0        0     2024 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3440 2023-05-23 19:26:33.532537 tmlt_analytics-0.7.1/doc/templates/python/module.rst
+-rw-r--r--   0        0        0      396 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11697 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8608 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6595 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7726 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0    12414 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/understanding-sensitivity.rst
+-rw-r--r--   0        0        0     8462 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9124 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7246 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18802 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0      430 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    12394 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     8475 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    14008 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16252 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     4789 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/examples/interactive_evaluation.ipynb
+-rw-r--r--   0        0        0     5459 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/examples/private_join.ipynb
+-rw-r--r--   0        0        0     6570 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/examples/zcdp_puredp_switching.ipynb
+-rw-r--r--   0        0        0     4645 2023-05-23 19:27:07.805302 tmlt_analytics-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/__init__.py
+-rw-r--r--   0        0        0     6965 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/conftest.py
+-rw-r--r--   0        0        0      115 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/system/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-23 19:26:33.536537 tmlt_analytics-0.7.1/test/system/session/__init__.py
+-rw-r--r--   0        0        0     4265 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0     6531 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_count_distinct_optimization.py
+-rw-r--r--   0        0        0    21707 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    13996 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     3965 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    26463 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    41576 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6122 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    13702 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0     7708 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     4465 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/test_budgets.py
+-rw-r--r--   0        0        0     2212 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/__init__.py
+-rw-r--r--   0        0        0      298 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    75173 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    54858 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24152 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36750 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    14834 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      657 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21123 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    14053 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3058 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2023-05-23 19:26:33.540537 tmlt_analytics-0.7.1/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5480 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     3011 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40754 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    64146 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16787 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     4874 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    84283 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5372 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      747 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test/unit/test_utils.py
+-rw-r--r--   0        0        0       37 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/test_requirements.txt
+-rw-r--r--   0        0        0      222 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     3666 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16162 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     6137 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     5341 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     4021 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0     9810 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7694 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0    38980 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    46275 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0    60186 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12795 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3980 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10148 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0      420 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/_type_checking.py
+-rw-r--r--   0        0        0    11748 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      306 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      458 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      735 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12758 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11850 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0    10390 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5482 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   126828 2023-05-23 19:26:33.544537 tmlt_analytics-0.7.1/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41097 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    77763 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3965 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     5397 2023-05-23 19:26:33.548538 tmlt_analytics-0.7.1/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.1/setup.py
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.1/PKG-INFO
```

### Comparing `tmlt_analytics-0.7.0rc1/CHANGELOG.rst` & `tmlt_analytics-0.7.1/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,70 @@
 .. _analytics-changelog:
 
 Changelog
 =========
 
-Unreleased
-----------
+0.7.1 - 2023-05-23
+------------------
+
+This is a maintenance release that mainly contains documentation updates.
+It also fixes a bug where installing Tumult Analytics using pip 23 and above could fail due to a dependency mismatch.
+
+0.7.0 - 2023-04-27
+------------------
+
+This release adds support for *privacy identifiers*:
+Tumult Analytics can now protect input tables in which the differential privacy guarantee needs to hide the presence of arbitrarily many rows sharing the same value in a particular column.
+For example, this may be used to protect each user of a service when every row in a table is associated with a user ID.
+
+Privacy identifiers are set up using the new :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change.
+A number of features have been added to the API to support this, including alternative behaviors for various query transformations when working with IDs and the new concept of :mod:`~tmlt.analytics.constraints`.
+To get started with these features, take a look at the new :ref:`Working with privacy IDs <Working with privacy IDs>` and :ref:`Doing more with privacy IDs <Advanced IDs features>` tutorials.
 
 Added
 ~~~~~
-- Added MaxRowsPerGroupPerID contraint, which limits the number of rows each unique (ID, grouping column value) pair may appear in.
-- Added MaxGroupsPerID constraint, which limits the number of unique grouping column values associated with each unique ID.
-- Added a new :class:`tmlt.analytics.protected_change.AddRowsWithID` class, which protects the addition or removal of all rows with the same value in a specified column.
-  When creating a session with AddRowsWithID for multiple tables, you must use the new :meth:`Session.Builder.with_id_space <tmlt.analytics.session.Session.Builder.with_id_space>` method to specify the identifier space(s) of the tables.
-  See the documentation for :class:`tmlt.analytics.protected_change.AddRowsWithID` for more information.
-- Added a new method, :meth:`tmlt.analytics.session.Session.describe`, which describes a session, query, or table.
+- A new :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change has been added, which protects the addition or removal of all rows with the same value in a specified column.
+  See the documentation for :class:`~tmlt.analytics.protected_change.AddRowsWithID` and the :ref:`Doing more with privacy IDs <Advanced IDs features>` tutorial for more information.
 
+  - When creating a Session with :class:`~tmlt.analytics.protected_change.AddRowsWithID` using a :class:`Session.Builder<tmlt.analytics.session.Session.Builder>`, you must use the new :meth:`~tmlt.analytics.session.Session.Builder.with_id_space` method to specify the identifier space(s) of tables using this protected change.
+  - When creating a Session with :meth:`Session.from_dataframe()<tmlt.analytics.session.Session.from_dataframe>`, specifying an ID space is not necessary.
+
+- :class:`~tmlt.analytics.query_builder.QueryBuilder` has a new method, :meth:`~tmlt.analytics.query_builder.QueryBuilder.enforce`, for enforcing constraints on a table.
+  Types for representing these constraints are located in the new :mod:`tmlt.analytics.constraints` module.
+- A new method, :meth:`Session.describe()<tmlt.analytics.session.Session.describe>`, has been added to provide a summary of the tables in a :class:`~tmlt.analytics.session.Session`, or of a single table or the output of a query.
 
 Changed
 ~~~~~~~
-- Argument ``max_num_rows`` of ``QueryBuilder.flat_map`` is now optional for tables with a :class:`tmlt.analytics.protected_change.AddRowsWithID` protected change.
-- *Backwards-incompatible*: Argument ``max_num_rows`` is now the last parameter specified for ``QueryBuilder.flat_map``.
-- *Backwards-incompatible*: Analytics no longer allows users to set lower bounds equal to upper bounds for quantile, sum, average, variance, and standard deviation queries. Now, the lower bound must be strictly less than the upper bound.
-- *Backwards-incompatible*: Renamed ``QueryBuilder.filter`` argument from "predicate" to "condition".
-- *Backwards-incompatible*: Renamed ``query_expr.Filter`` property from "predicate" to "condition".
-- *Backwards-incompatible*: Renamed ``KeySet.filter`` argument from "expr" to "condition".
-- ``QueryBuilder.join_private`` now accepts a string as a ``right_operand``. ``QueryBuilder("table").join_private("foo")`` is equivalent to ``QueryBuilder("table").join_private(QueryBuilder("foo"))``.
-- *Backwards-incompatible*: Removed the ``attr_name`` argument from ``Session.partition_and_create``.
+- :meth:`QueryBuilder.join_private()<tmlt.analytics.query_builder.QueryBuilder.join_private>` now accepts the name of a private table as ``right_operand``.
+  For example, ``QueryBuilder("table").join_private("foo")`` is equivalent to ``QueryBuilder("table").join_private(QueryBuilder("foo"))``.
+- The ``max_num_rows`` parameter to :meth:`QueryBuilder.flat_map()<tmlt.analytics.query_builder.QueryBuilder.flat_map>` is now optional when applied to tables with an :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change.
+- *Backwards-incompatible*: The parameters to :meth:`QueryBuilder.flat_map()<tmlt.analytics.query_builder.QueryBuilder.flat_map>` have been reordered, moving ``max_num_rows`` to be the last parameter.
+- *Backwards-incompatible*: The lower and upper bounds for quantile, sum, average, variance, and standard deviation queries can no longer be equal to one another.
+  The lower bound must now be strictly less than the upper bound.
+- *Backwards-incompatible*: Renamed :meth:`QueryBuilder.filter()<tmlt.analytics.query_builder.QueryBuilder.filter>` ``predicate`` argument to ``condition``.
+- *Backwards-incompatible*: Renamed :class:`~tmlt.analytics.query_expr.Filter` query expression ``predicate`` property to ``condition``.
+- *Backwards-incompatible*: Renamed :meth:`KeySet.filter()<tmlt.analytics.keyset.KeySet.filter>` ``expr`` argument to ``condition``.
+
+Deprecated
+~~~~~~~~~~
+- The ``stability`` and ``grouping_column`` parameters to :class:`Session.from_dataframe()<tmlt.analytics.session.Session.from_dataframe>` and :class:`Session.Builder.with_private_dataframe()<tmlt.analytics.session.Session.Builder.with_private_dataframe>` are deprecated, and will be removed in a future release.
+  The ``protected_change`` parameter should be used instead, and will become required.
+
+Removed
+~~~~~~~
+- The ``attr_name`` parameter to :class:`Session.partition_and_create()<tmlt.analytics.session.Session.partition_and_create>`, which was deprecated in version 0.5.0, has been removed.
 
 Fixed
 ~~~~~
-
-- ``Session.add_public_datafame`` used to allow creation of a public table with the same name as an existing private table, even though doing so is disallowed elsewhere and is not fully supported by some ``Session`` methods.
-  It now raises a ``ValueError`` when this happens, like it already did when there was a name conflict with an existing public table.
+- :meth:`Session.add_public_datafame()<tmlt.analytics.session.Session.add_public_dataframe>` used to allow creation of a public table with the same name as an existing public table, which was neither intended nor fully supported by some :class:`~tmlt.analytics.session.Session` methods.
+  It now raises a ``ValueError`` in this case.
+- Some query patterns on tables containing nulls could cause grouped aggregations to produce the wrong set of group keys in their output.
+  This no longer happens.
+- In certain unusual cases, join transformations could erroneously drop rows containing nulls in columns that were not being joined on.
+  These rows are no longer dropped.
 
 0.6.1 - 2022-12-07
 ------------------
 
 This is a maintenance release which introduces a number of documentation improvements, but has no publicly-visible API changes.
 
 0.6.0 - 2022-12-06
```

### Comparing `tmlt_analytics-0.7.0rc1/LICENSE` & `tmlt_analytics-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/LICENSE.docs` & `tmlt_analytics-0.7.1/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/README.md` & `tmlt_analytics-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/_static/css/custom.css` & `tmlt_analytics-0.7.1/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/_static/favicon.ico` & `tmlt_analytics-0.7.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/_static/js/version-banner.js` & `tmlt_analytics-0.7.1/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/_static/logo.png` & `tmlt_analytics-0.7.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/additional-resources/privacy_policy.rst` & `tmlt_analytics-0.7.1/doc/privacy-policy.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-.. _privacy_policy:
+:orphan:
+
+.. _privacy-policy:
 
 Privacy Policy
 ==============
 
 Effective Date: Aug 26th, 2022
 
 Welcome
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/conf.py` & `tmlt_analytics-0.7.1/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 ci_tag = os.getenv("CI_COMMIT_TAG")
 ci_branch = os.getenv("CI_COMMIT_BRANCH")
 
 version = ci_tag or ci_branch or "HEAD"
 commit_hash = os.getenv("CI_COMMIT_SHORT_SHA") or "unknown version"
 build_time = datetime.datetime.utcnow().isoformat(sep=" ", timespec="minutes")
 
-linkcheck_mode_url_prefix = os.getenv("BASE_URL_OVERRIDE")
 # Linkcheck will complain that these anchors don't exist,
 # even though the link works.
 linkcheck_ignore = [
     "https://colab.research.google.com/drive/18J_UrHAKJf52RMRxi4OOpk59dV9tvKxO#offline=true&sandboxMode=true"
 ]
 
 # Sphinx configuration
@@ -140,14 +139,17 @@
     ("py:class", "Row"),
     ("py:class", "BinT"),
     ("py:class", "tmlt.analytics.binning_spec.BinT"),
     ("py:class", "BinNameT"),
     ("py:class", "Generic[BinT, BinNameT]"),
     ("py:class", "tmlt.core.domains.spark_domains.SparkColumnsDescriptor"),
     ("py:class", "sympy.core.expr.Expr"),
+    ("py:class", "Epsilon"),
+    ("py:class", "Delta"),
+    ("py:class", "Rho"),
 ]
 
 # Remove this after intersphinx can use core
 nitpick_ignore_regex = [(r"py:.*", r"tmlt.core.*")]
 
 # Theme settings
 templates_path = ["_templates"]
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/api_diagram.svg` & `tmlt_analytics-0.7.1/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.7.1/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.7.1/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.7.1/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_books_by_unique_members.png` & `tmlt_analytics-0.7.1/doc/images/chart_books_by_unique_members.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.7.1/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.7.1/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.7.1/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_education.png` & `tmlt_analytics-0.7.1/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.7.1/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_favorite_genres.png` & `tmlt_analytics-0.7.1/doc/images/chart_favorite_genres.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_filters_education.png` & `tmlt_analytics-0.7.1/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_genres_by_age.png` & `tmlt_analytics-0.7.1/doc/images/chart_genres_by_age.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.7.1/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.7.1/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.7.1/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.7.1/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.7.1/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.7.1/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.7.1/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/flow_chart_truncation.svg` & `tmlt_analytics-0.7.1/doc/images/flow_chart_truncation.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.7.1/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/index_api.svg` & `tmlt_analytics-0.7.1/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/index_more.svg` & `tmlt_analytics-0.7.1/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/index_topic_guides.svg` & `tmlt_analytics-0.7.1/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/index_tutorials.svg` & `tmlt_analytics-0.7.1/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/images/logo.png` & `tmlt_analytics-0.7.1/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/installation.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 It is compatible with Python 3.7, 3.8, and 3.9.
 Because Tumult Analytics uses PySpark for computation, it also `requires Java 8 or 11 <https://spark.apache.org/docs/3.0.0/index.html#downloading>`__.
 
 Only the x86_64 processor architecture is officially supported at present.
 Apple silicon is supported through binary translation with `Rosetta 2 <https://support.apple.com/en-us/HT211861>`__.
 
 Below are instructions for installing these prerequisites on several common platforms.
-If none of these apply to you, install Python 3 and Java from your OS package manager, or use the "Manual Installation" section to obtain installers or source distributions and build instructions for your platform.
+If none of these apply to you, install Python 3 and Java from your OS package manager or manually, then proceed with the `pip` installation.
 If you encounter any issues during the installation process, please `let us know <https://gitlab.com/tumult-labs/analytics/-/issues>`__!
 
 .. tabbed:: Linux (Debian-based)
 
     Python and ``pip``, Python's package manager, are likely already installed.
     If they are not, install them with:
 
@@ -54,16 +54,14 @@
 
     Note that despite the package name, this will install Java 8.
 
 
 .. tabbed:: macOS (Intel)
 
     The below instructions assume the use of `Homebrew <https://brew.sh/>`__ for managing packages.
-    If you do not wish to use Homebrew for this, use the "Manual Installation" instructions instead.
-
     If you do not already have Homebrew, it can be installed with:
 
     .. code-block:: bash
 
         /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 
     Python may be installed with:
@@ -81,15 +79,14 @@
     You may need to explicitly add this OpenJDK installation to your ``PATH`` for it to be detected and usable by Spark.
     This can be done by, for example, adding ``export PATH="/usr/local/opt/openjdk/bin:$PATH"`` to ``.bashrc`` and then restarting your shell.
 
 
 .. tabbed:: macOS (Apple silicon)
 
     Since Python 3.7 is not supported on the Apple silicon processor architecture, you will need to first install `Rosetta 2 <https://support.apple.com/en-us/HT211861>`__ and the x86_64 version of Homebrew.
-
     If you do not already have Rosetta 2, it can be installed with:
 
     .. code-block:: bash
 
         softwareupdate --install-rosetta
 
     The x86_64 version of Homebrew can be installed with:
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/intersphinx_mapping.json` & `tmlt_analytics-0.7.1/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/templates/python/class.rst` & `tmlt_analytics-0.7.1/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/templates/python/module.rst` & `tmlt_analytics-0.7.1/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/bigquery-setup.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/bigquery-setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/docker-image.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/docker-image.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/index.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/inputs-outputs.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/inputs-outputs.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/parameters.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/parameters.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/running-the-program.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/running-the-program.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/setup.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/bigquery/setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.7.1/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.7.1/doc/topic-guides/privacy-budgets.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.7.1/doc/topic-guides/privacy-promise.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 A :class:`~tmlt.analytics.session.Session` is initialized with:
 
 * one or more private tables (containing data you wish to query in a differentially
   private way), each associated to a :mod:`protected change<tmlt.analytics.protected_change>`;
 * zero or more public tables (containing data that does not require privacy
   protection, but may be used as auxiliary input to your computation);
 * a privacy definition along with its associated privacy parameters (e.g.
-  tutorials use `PureDBBudget`, corresponding to pure differential privacy, and
+  tutorials use `PureDPBudget`, corresponding to pure differential privacy, and
   Tumult Analytics also supports zero-concentrated differential privacy).
 
 After initialization, the Session guarantees that the answers returned by
 calling :meth:`~tmlt.analytics.session.Session.evaluate` to evaluate queries
 satisfy the corresponding privacy definition with respect to the private data,
 using the specified parameters. For example, a Session initialized with
 :code:`PureDPBudget(1)` provides :math:`{\varepsilon}`-differential privacy with
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/spark.rst` & `tmlt_analytics-0.7.1/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/troubleshooting.rst` & `tmlt_analytics-0.7.1/doc/howto-guides/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.7.1/doc/topic-guides/working-with-sessions.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.7.1/doc/tutorials/clamping-bounds.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.7.1/doc/tutorials/first-steps.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.7.1/doc/tutorials/groupby-queries.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/more-with-privacy-ids.rst` & `tmlt_analytics-0.7.1/doc/tutorials/more-with-privacy-ids.rst`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Initializing a Session with multiple IDs tables
 -----------------------------------------------
 
 Notice that both of the dataframes we’ve loaded share a common
 identifier: the ID associated with each library member. Our goal is to
 construct a :class:`Session<tmlt.analytics.session.Session>` that
 protects the addition or removal of arbitrarily many rows that share the
-same ID, *in both tables*. To do so, we have to use the 
+same ID, *in both tables*. To do so, we have to use the
 :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change
 again, but we also have to indicate that both tables share the same *ID space*.
 This is done as follows.
 
 .. testcode::
 
     budget = PureDPBudget(float("inf")) # infinite budget for the session
@@ -94,15 +94,15 @@
     Private dataframes: ['members', 'checkouts']
 
 The
 :meth:`Session.Builder.with_id_space<tmlt.analytics.session.Session.Builder.with_id_space>`
 method and the :class:`AddRowsWithID<tmlt.analytics.protected_change.AddRowsWithID>`
 protected change work together to accomplish our desired notion of privacy.
 
-- The ``with_primary_id`` function defines our ID space, ``member_id_space``. This is
+- The ``with_id_space`` function defines our ID space, ``member_id_space``. This is
   how we indicate that the same person is associated with the same ID in both tables.
 
 - This ID space is then specified to ``AddRowsWithID``’s ``identifier``
   parameter, while the ``id_column`` parameter indicates
   which column in the dataframe contains the IDs.
 
 With this information, the resulting Session now protects each library member
@@ -121,15 +121,15 @@
 - First, since each book in the checkouts table can be
   associated with more than one genre, we will expand this
   table to break out each genre for a book into a separate row.
 
 - Second, we will join the expanded checkouts data with the library
   members data, using the members ID as a join key.
 
-- Finally, we will group the joined table by age group and genres, and obtain 
+- Finally, we will group the joined table by age group and genres, and obtain
   counts by genres.
 
 Flat maps
 ~~~~~~~~~
 
 First, let's expand the checkout dataframe to
 associate each book to its genres, with each genre on its own separate row. To do this,
@@ -205,14 +205,42 @@
     print(f"Private dataframes: {session.private_sources}")
 
 .. testoutput::
     :options: +NORMALIZE_WHITESPACE
 
     Private dataframes: ['checkouts_joined', 'checkouts_single_genre', 'members', 'checkouts']
 
+Let's inspect the result of the join to make sure it looks right:
+
+.. testcode::
+
+    session.describe("checkouts_joined")
+
+.. testoutput::
+    :options: +NORMALIZE_WHITESPACE
+
+    Columns:
+	- 'member_id'         INTEGER, ID column (in ID space member_id_space)
+	- 'checkout_date'     TIMESTAMP
+	- 'title'             VARCHAR
+	- 'author'            VARCHAR
+	- 'isbn'              VARCHAR
+	- 'publication_date'  INTEGER
+	- 'publisher'         VARCHAR
+	- 'genres'            VARCHAR
+	- 'genre'             VARCHAR
+	- 'name'              VARCHAR
+	- 'age'               INTEGER
+	- 'gender'            VARCHAR
+	- 'education_level'   VARCHAR
+	- 'zip_code'          VARCHAR
+	- 'books_borrowed'    INTEGER
+	- 'favorite_genres'   VARCHAR
+	- 'date_joined'       TIMESTAMP
+
 Using :meth:`~tmlt.analytics.query_builder.QueryBuilder.join_private` on two private tables in the same ID space works seamlessly as long as the ID
 columns are part of the join and have the same name in both tables. Like with
 :meth:`~tmlt.analytics.query_builder.QueryBuilder.flat_map`, no truncation is necessary.
 
 Computing the statistic
 ~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -305,8 +333,8 @@
 
 - Data preparation is generally more convenient when using privacy IDs, because you
   don't need to worry about truncating your data (when performing e.g. flat maps or
   joins) until immediately before aggregation.
 
 - Truncation as a last step before aggregation can lead to better utility. Plus,
   if you want to compute multiple aggregations, you might also want to use different
-  truncation parameters for each.
+  truncation parameters for each.
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.7.1/doc/tutorials/privacy-budget-basics.rst`

 * *Files 9% similar despite different names*

```diff
@@ -78,14 +78,38 @@
    session = Session.from_dataframe(
        privacy_budget=budget,
        source_id="members",
        dataframe=members_df,
        protected_change=AddOneRow(),
    )
 
+Let's check that we initialized the Session as intended using the
+:meth:`describe<tmlt.analytics.session.Session.describe>` method:
+
+.. testcode::
+
+   session.describe()
+
+.. testoutput::
+   :options: +NORMALIZE_WHITESPACE
+
+   The session has a remaining privacy budget of PureDPBudget(epsilon=2.5).
+   The following private tables are available:
+   Table 'members' (no constraints):
+      Columns:
+         - 'id'               INTEGER
+         - 'name'             VARCHAR
+         - 'age'              INTEGER
+         - 'gender'           VARCHAR
+         - 'education_level'  VARCHAR
+         - 'zip_code'         VARCHAR
+         - 'books_borrowed'   INTEGER
+         - 'favorite_genres'  VARCHAR
+         - 'date_joined'      TIMESTAMP
+
 Initializing a Session with a finite privacy budget gives a simple interface
 promise: all queries evaluated on this Session, *taken together*, will provide
 differentially private results with at most ``epsilon=2.5``. This parameter
 measures the potential privacy *loss*: a lower epsilon gives a stricter limit on
 the privacy loss, and therefore a higher level of protection. Here, the
 corresponding interface promise is a *privacy guarantee*: it enforces a minimum
 level of protection on the private data. For more information about this promise
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-id-basics.rst` & `tmlt_analytics-0.7.1/doc/tutorials/privacy-id-basics.rst`

 * *Files 19% similar despite different names*

```diff
@@ -82,15 +82,38 @@
         budget,
         "checkouts",
         checkouts_df,
         protected_change=AddRowsWithID(id_column="member_id"),
     )
 
 Initializing our Session like this protects members of our library,
-regardless of how many books they've checked out.
+regardless of how many books they've checked out. Let's take a look at our Session:
+
+.. testcode::
+
+    session.describe()
+
+.. testoutput::
+    :options: +NORMALIZE_WHITESPACE
+
+    The session has a remaining privacy budget of PureDPBudget(epsilon=inf).
+    The following private tables are available:
+    Table 'checkouts' (no constraints):
+        Columns:
+            - 'checkout_date'     TIMESTAMP
+            - 'member_id'         INTEGER, ID column (in ID space default_id_space)
+            - 'title'             VARCHAR
+            - 'author'            VARCHAR
+            - 'isbn'              VARCHAR
+            - 'publication_date'  INTEGER
+            - 'publisher'         VARCHAR
+            - 'genres'            VARCHAR
+
+We can see that our Session has a single table, ``checkouts``, with 7 columns, and that
+the 'member_id' column is marked as our ID column.
 
 A simple query with privacy IDs
 -------------------------------
 
 Let's find out what the most popular books in our library are! We can do this
 by counting how many times each book has been checked out.
 
@@ -108,15 +131,16 @@
         .groupby(keyset)
         .count()
     )
     result = session.evaluate(count_query, PureDPBudget(1))
 
 .. code-block::
 
-    RuntimeError: A constraint on the number of rows contributed by each ID is needed to perform this query.
+    RuntimeError: A constraint on the number of rows contributed by each ID
+    is needed to perform this query (e.g. MaxRowsPerID).
 
 This error occurs because there is no limit to how many rows a single person
 could contribute to the data: a single library member could borrow 10000 books
 or even more! But differential privacy needs to hide the impact of a single
 person behind statistical noise… and as we saw with
 :ref:`clamping bounds<Clamping bounds>`, this is impossible if this impact
 can be arbitrarily large!
@@ -155,15 +179,14 @@
     |...|...|...|...|
     |...|...|...|...|
     |...|...|...|...|
     |...|...|...|...|
     |...|...|...|...|
     +--------------------+--------------------+----------+-----+
 
-
 .. code-block::
 
     +--------------------+--------------------+----------+-----+
     |               title|              author|      isbn|count|
     +--------------------+--------------------+----------+-----+
     |Comfort Me with A...|         Ruth Reichl|0375758739| 3787|
     |       The Alchemist|Paulo Coelho/Alan...|0061122416| 2441|
@@ -171,43 +194,45 @@
     |     Eat  Pray  Love|   Elizabeth Gilbert|0143038419| 2071|
     |The Tipping Point...|    Malcolm Gladwell|0316346624| 1884|
     +--------------------+--------------------+----------+-----+
 
 With this additional step limiting the maximum contribution of each privacy ID,
 we are now able to run the query and find the five most popular books. This
 step is also called *truncation*: we dropped (or *truncated*) some of the data
-to enforce the desired constraint. 
+to enforce the desired constraint.
 
 More constraints
 ----------------
 
 Limiting the number of rows per privacy ID is not the only way to truncate the
 data and perform queries with privacy IDs. Another option is to limit the
 number of *groups* that each ID can appear in, and limit the number of
 *rows per group* that a single privacy ID can contribute. Let's see an example
 by computing how many patrons have checked out each of our top five books.
 
 For this query, we will combine two constraints to truncate our data:
 
-* :class:`~tmlt.analytics.constraints.MaxGroupsPerID`: limiting
-  the number of groups (here, distinct books) that any library patron can contribute to
-* :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID`:
-  limiting the number of rows that any library patron can provide for each group.
-
-We will limit each patron to 5 groups (we only consider the 5 most popular books) and have
-patrons only appear once per group (we don't want to count the same patron twice for the same book).
+* :class:`~tmlt.analytics.constraints.MaxGroupsPerID`: limiting the number of
+  groups (here, distinct books) that any library patron can contribute to; and
+* :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID`: limiting the number
+  of rows that any library patron can provide for each group.
+
+We will limit each patron to 5 groups (we only consider the 5 most popular
+books) and have patrons only appear once per group (we don't want to count the
+same patron twice for the same book).
 
 Then, we will create a keyset from our top 5 books and perform a count query:
 
 .. testcode::
 
     top_five_keyset = KeySet.from_dataframe(
         top_five.select("title", "author", "isbn"),
     )
-    count_distinct_query = (QueryBuilder("checkouts")
+    count_distinct_query = (
+        QueryBuilder("checkouts")
         .enforce(MaxGroupsPerID("isbn", 5))
         .enforce(MaxRowsPerGroupPerID("isbn", 1))
         .groupby(top_five_keyset)
         .count()
     )
     result = session.evaluate(count_distinct_query, PureDPBudget(1.5))
     result.show()
@@ -234,15 +259,60 @@
     |Comfort Me with A...|         Ruth Reichl|0375758739|  481|
     |     Eat  Pray  Love|   Elizabeth Gilbert|0143038419|  658|
     |       The Alchemist|Paulo Coelho/Alan...|0061122416|  777|
     |The Devil in the ...|Erik Larson/Tony ...|0739303406|  657|
     |The Tipping Point...|    Malcolm Gladwell|0316346624|  549|
     +--------------------+--------------------+----------+-----+
 
-We can display this data as a graph:
+We could also express this query using
+:meth:`~tmlt.analytics.query_builder.QueryBuilder.count_distinct`: limiting each
+ID to a single row per library member (per ISBN) is the same as counting
+distinct IDs.
+
+.. testcode::
+
+    top_five_keyset = KeySet.from_dataframe(top_five.select("isbn"))
+    count_distinct_query = (
+        QueryBuilder("checkouts")
+        .enforce(MaxGroupsPerID("isbn", 5))
+        .groupby(top_five_keyset)
+        .count_distinct(["member_id"], name="count")
+    )
+    result = session.evaluate(
+        count_distinct_query, PureDPBudget(1.5)
+    ).join(  # Add title/author back to result
+        top_five.select("title", "author", "isbn"), on=["isbn"], how="left"
+    ).select(  # Reorder dataframe columns
+        "title", "author", "isbn", "count"
+    )
+
+.. testcode::
+    :hide:
+
+    result.show()
+
+.. testoutput::
+    :hide:
+    :options: +NORMALIZE_WHITESPACE
+
+    +--------------------+--------------------+----------+-----+
+    |               title|              author|      isbn|count|
+    +--------------------+--------------------+----------+-----+
+    |...|...|...|...|
+    |...|...|...|...|
+    |...|...|...|...|
+    |...|...|...|...|
+    |...|...|...|...|
+    +--------------------+--------------------+----------+-----+
+
+When using `count_distinct` on the ID column, we no longer need to specify the
+`MaxRowsPerGroupPerID` constraint: Tumult Analytics understands that each ID can
+contribute at most once per group.
+
+We can then display the results as a graph:
 
 .. code-block::
 
     import matplotlib.pyplot as plt
     import seaborn as sns
 
     sns.set_theme(style="whitegrid")
@@ -253,32 +323,40 @@
             return row["title"]
         return row["title"][:12] + "..."
 
     data_to_plot["short_title"] = data_to_plot.apply(
         lambda row: shorten_title(row), axis=1
     )
 
-    g = sns.barplot(x="short_title", y="count", data=data_to_plot, color="#1f77b4")
-    g.set_xticklabels(g.get_xticklabels(), rotation=45, horizontalalignment="right")
+    g = sns.barplot(x="title", y="count", data=data_to_plot, color="#1f77b4")
+    g.set_xticklabels(
+        data_to_plot["short_title"], rotation=45, horizontalalignment="right"
+    )
     plt.title("How many members have checked out popular books")
     plt.xlabel("Book Title")
     plt.ylabel("Members")
     plt.tight_layout()
     plt.show()
 
 .. image:: ../images/chart_books_by_unique_members.png
    :alt: A bar chart plotting the number of unique library members who have checked out each book. The most popular book (The Alchemist) has been checked out by about 750 people; each book after that has been checked out by fewer people, with the last book (Comfort Me With...) having been checked out by just under 500 people.
    :align: center
 
+.. _flow-chart-truncation:
 
 Summary
 -------
 
 We've seen that when using privacy IDs, we need to truncate the data to limit
 how much each privacy ID can contribute to the final statistic. There are two
 ways of doing so: using :class:`~tmlt.analytics.constraints.MaxRowsPerID`,
 or using :class:`~tmlt.analytics.constraints.MaxGroupsPerID` and
 :class:`~tmlt.analytics.constraints.MaxRowsPerGroupPerID`.
 
 .. image:: ../images/flow_chart_truncation.svg
    :alt: A flow chart showing three paths from "data with privacy IDs" to "compute statistic". The first path is "data with privacy IDs" to "truncate using MaxRowsPerID" to "compute statistic". The second and third paths are paired together. The second path is "data with privacy IDs" to "truncate using MaxGroupsPerID" to "truncate using MaxRowsPerGroupPerID" to "compute statistic". The third path is "data with privacy IDs" to "truncate using MaxRowsPerGroupPerID" to "truncate using MaxGroupsPerID" to "compute statistic".
    :align: center
+
+To understand more the impact of choosing one kind of constraint vs. another,
+you can consult our :ref:`topic guide about sensitivity<Understanding sensitivity>`.
+To learn more about how to perform more complex queries on tables initialized with
+privacy IDs, you can proceed to the :ref:`next tutorial<Advanced IDs features>`.
```

### Comparing `tmlt_analytics-0.7.0rc1/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.7.1/doc/tutorials/simple-transformations.rst`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,16 @@
     plt.tick_params(axis='both', which='major', labelsize=10)
     plt.show()
 
 .. image:: ../images/chart_age_at_joining.png
     :alt: A bar chart plotting the count of members by each age bin and gender. The chart is bimodal with peaks at 10-19 and 50-59 with no significant interaction between age and gender.
     :align: center
 
+.. _flat-map-tutorial-5:
+
 Flat maps
 ---------
 
 Similar to a map, we can also apply a "flat map" to our data. A flat map is similar to a
 map, but instead of mapping each input row to a single new row, it maps each
 input row to zero or more new rows.
```

### Comparing `tmlt_analytics-0.7.0rc1/examples/interactive_evaluation.ipynb` & `tmlt_analytics-0.7.1/examples/interactive_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/examples/private_join.ipynb` & `tmlt_analytics-0.7.1/examples/private_join.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/examples/zcdp_puredp_switching.ipynb` & `tmlt_analytics-0.7.1/examples/zcdp_puredp_switching.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/pyproject.toml` & `tmlt_analytics-0.7.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.7.0-rc.1"
+version = "0.7.1"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
@@ -40,31 +40,31 @@
 
 # When updating Core, PySpark, Pandas or SymPy, remember to update
 # test_multi_deps in the Noxfile.
 
 "tmlt.core" = "^0.9.0"
 
 pandas = "^1.2.0"
-pyspark = { version = "^3.0.0,<3.4.0", extras = ["sql"] }
+pyspark = { version = "^3.0.0,<=3.3.1", extras = ["sql"] }
 sympy = "^1.8,<1.10"
 typeguard = "^2.12.1,<2.13.0"
 typing-extensions = "^3.10.0"
 
 
 [tool.poetry.dev-dependencies]
 # Build scripting
 nox = "2022.8.7"
 nox_poetry = "1.0.1"
 
 # Linters, formatters
-black = "21.9b0"
-isort = { version = "4.3.21", extras = ["pyproject"] }
-mypy = "0.940"
-pydocstyle = { version = "6.1.1", extras = ["toml"] }
-pylint = "2.5.3"
+black = "^23.3"
+isort = { version = "^5.11", extras = ["pyproject"] }
+mypy = "^1.2"
+pydocstyle = { version = "^6.3", extras = ["toml"] }
+pylint = "^2.13"
 
 # CI, testing, docs
 pytest = "^7.1.2"
 coverage = "^6.5"
 pydata-sphinx-theme = "0.9.0"
 scanpydoc = "0.7.3" # 0.7.4 doesn't work
 sphinx = "^4.3.0"
@@ -104,29 +104,29 @@
 line_length = 88
 
 [tool.mypy]
 explicit_package_bases = true
 follow_imports = "silent"
 ignore_missing_imports = true
 namespace_packages = true
-
 check_untyped_defs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 
 [tool.pylint.master]
 # See https://github.com/PyCQA/pylint/issues/1975#issuecomment-387924981
 extension-pkg-whitelist = ['numpy']
 load-plugins = ['pylint.extensions.docparams']
 # Only check param docs in docstrings that contain an Args: section.
 # Set to "no" to show docstrings missing argument documentation.
 accept-no-param-doc = true
 
 [tool.pylint.'MESSAGES CONTROL']
+enable = ['useless-suppression']
 disable = [
   'arguments-differ',
   'bad-continuation',
   'duplicate-code',
   'fixme',
   'invalid-name',
   'logging-format-interpolation',
@@ -142,14 +142,17 @@
   'too-many-instance-attributes',
   'too-many-lines',
   'too-many-locals',
   'too-many-public-methods',
   'too-many-return-statements',
   'too-many-statements',
   'unbalanced-tuple-unpacking',
+  # black and isort group tmlt.core separately from tmlt.analytics,
+  # but pylint thinks they should both be grouped as 'tmlt'.
+  'ungrouped-imports',
   'wrong-import-order',
 ]
 
 [tool.pylint.FORMAT]
 max-line-length = 88
 
 [tool.pydocstyle]
```

### Comparing `tmlt_analytics-0.7.0rc1/test/conftest.py` & `tmlt_analytics-0.7.1/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Creates a Spark Context to use for each testing session."""
 
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
+
 # TODO(#2206): Import these fixtures from core once it is rewritten
-# pylint: disable=unused-import
+
 import logging
-from typing import Any, Sequence
+from typing import Any, Optional, Sequence
 from unittest.mock import Mock, create_autospec
 
 import numpy as np
 import pandas as pd
 import pytest
 from pyspark.sql import SparkSession
-
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measures import Measure, PureDP
 from tmlt.core.metrics import AbsoluteDifference, Metric
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber
@@ -57,15 +57,15 @@
     spark.sparkContext.setLogLevel("OFF")
     return spark
 
 
 def assert_frame_equal_with_sort(
     first_df: pd.DataFrame,
     second_df: pd.DataFrame,
-    sort_columns: Sequence[str] = None,
+    sort_columns: Optional[Sequence[str]] = None,
     **kwargs: Any,
 ):
     """Asserts that the two data frames are equal.
 
     Wrapper around pandas test function. Both dataframes are sorted
     since the ordering in Spark is not guaranteed.
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/conftest.py` & `tmlt_analytics-0.7.1/test/system/session/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_constraint_propagation.py` & `tmlt_analytics-0.7.1/test/system/session/ids/test_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l0_linf_truncation.py` & `tmlt_analytics-0.7.1/test/system/session/ids/test_l0_linf_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l1_truncation.py` & `tmlt_analytics-0.7.1/test/system/session/ids/test_l1_truncation.py`

 * *Files 6% similar despite different names*

```diff
@@ -290,17 +290,14 @@
 @pytest.mark.parametrize("session", [INF_BUDGET], indirect=True, ids=["puredp"])
 @pytest.mark.parametrize(
     "query,expected_noise",
     [
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count(), [1]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count(), [2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count(), [5]),
-        (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count_distinct(["id"]), [1]),
-        (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count_distinct(["id"]), [2]),
-        (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count_distinct(["id"]), [5]),
         # Two aggregations, a sum and a count, each with half the budget
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 10), [10, 2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 10), [50, 10]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 20), [20, 2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 20), [100, 10]),
     ],
 )
@@ -316,17 +313,14 @@
 @pytest.mark.parametrize("session", [INF_BUDGET_ZCDP], indirect=True, ids=["zcdp"])
 @pytest.mark.parametrize(
     "query,expected_noise",
     [
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count(), [0.5]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count(), [2]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count(), [12.5]),
-        (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).count_distinct(["id"]), [0.5]),
-        (QueryBuilder("id_a1").enforce(MaxRowsPerID(2)).count_distinct(["id"]), [2]),
-        (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).count_distinct(["id"]), [12.5]),
         # Two aggregations, a sum and a count, each with half the budget
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 10), [25, 1]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 10), [625, 25]),
         (QueryBuilder("id_a1").enforce(MaxRowsPerID(1)).average("n", 0, 20), [100, 1]),
         (
             QueryBuilder("id_a1").enforce(MaxRowsPerID(5)).average("n", 0, 20),
             [2500, 25],
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/ids/test_partition.py` & `tmlt_analytics-0.7.1/test/system/session/ids/test_partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 
 import pandas as pd
 import pytest
 import sympy as sp
+from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
+from tmlt.core.metrics import DictMetric
 
 from tmlt.analytics._table_identifier import NamedTable, TableCollection
 from tmlt.analytics.constraints import MaxGroupsPerID, MaxRowsPerID
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget
 from tmlt.analytics.query_builder import QueryBuilder
-from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
-from tmlt.core.metrics import DictMetric
 
-from ....conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
-)
+from ....conftest import assert_frame_equal_with_sort
 from ..conftest import INF_BUDGET, INF_BUDGET_ZCDP
 
 _KEYSET = KeySet.from_dict({"group": ["A", "B"]})
 _KEYSET2 = KeySet.from_dict({"group2": ["X", "Y"]})
 
 
 @pytest.mark.parametrize("session", [INF_BUDGET], indirect=True, ids=["puredp"])
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/mixed/test_mixed_session.py` & `tmlt_analytics-0.7.1/test/system/session/mixed/test_mixed_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/rows/conftest.py` & `tmlt_analytics-0.7.1/test/system/session/rows/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Common fixtures for non-IDs Session tests."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-member, no-self-use
-
 import datetime
 from typing import Any, List
 
 import pandas as pd
 import pytest
 from pyspark.sql import SparkSession
 from pyspark.sql.types import LongType, StringType, StructField, StructType
+from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
     analytics_to_spark_schema,
@@ -34,15 +33,14 @@
     JoinPublic,
     Map,
     PrivateSource,
     ReplaceNullAndNan,
     Select,
     SumMechanism,
 )
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 
 # Shorthands for some values used in tests
 _DATE1 = datetime.date.fromisoformat("2022-01-01")
 _DATE2 = datetime.date.fromisoformat("2022-01-02")
 
 # Dataframes for public data,
 # placed here so that test case KeySets can use them
@@ -140,39 +138,36 @@
     ),
     (  # Incomplete two-column marginal with a dataframe
         QueryBuilder("private")
         .groupby(KeySet(dataframe=GET_GROUPBY_TWO_COLUMNS))
         .count(),
         GroupByCount(
             child=PrivateSource("private"),
-            # pylint: disable=protected-access
             groupby_keys=KeySet(dataframe=GET_GROUPBY_TWO_COLUMNS),
         ),
         pd.DataFrame({"A": ["0", "0", "1"], "B": [0, 1, 1], "count": [2, 1, 0]}),
     ),
     (  # Incomplete two-column marginal with a dataframe
         QueryBuilder("private")
         .groupby(KeySet(dataframe=GET_GROUPBY_TWO_COLUMNS))
         .count_distinct(),
         GroupByCountDistinct(
             child=PrivateSource("private"),
-            # pylint: disable=protected-access
             groupby_keys=KeySet(dataframe=GET_GROUPBY_TWO_COLUMNS),
         ),
         pd.DataFrame(
             {"A": ["0", "0", "1"], "B": [0, 1, 1], "count_distinct": [2, 1, 0]}
         ),
     ),
     (  # One-column marginal with additional value
         QueryBuilder("private")
         .groupby(KeySet(dataframe=GET_GROUPBY_ONE_COLUMN))
         .count(),
         GroupByCount(
             child=PrivateSource("private"),
-            # pylint: disable=protected-access
             groupby_keys=KeySet(dataframe=GET_GROUPBY_ONE_COLUMN),
         ),
         pd.DataFrame({"A": ["0", "1", "2"], "count": [3, 1, 0]}),
     ),
     (  # One-column marginal with additional value
         QueryBuilder("private")
         .groupby(KeySet(dataframe=GET_GROUPBY_ONE_COLUMN))
@@ -407,14 +402,45 @@
     (  # Histogram Syntax
         QueryBuilder("private").histogram(
             "X", BinningSpec([0, 2, 4], names=["0,1", "2,3"], right=False)
         ),
         None,
         pd.DataFrame({"X_binned": ["0,1", "2,3"], "count": [2, 2]}),
     ),
+    (  # Binning Nulls
+        QueryBuilder("private")
+        .map(
+            lambda row: {"X": row["X"] if row["X"] != 3 else None},
+            new_column_types={"X": ColumnDescriptor(ColumnType.INTEGER)},
+        )
+        .bin_column(
+            "X", BinningSpec([10, 12, 14], names=["10,12", "12,14"], right=False)
+        )
+        .groupby(KeySet.from_dict({"X_binned": ["10,12", "12,14", None]}))
+        .count(),
+        None,
+        pd.DataFrame({"X_binned": ["10,12", "12,14", None], "count": [0, 0, 4]}),
+    ),
+    (  # Binning NaN bin names
+        QueryBuilder("private")
+        .bin_column(
+            "X",
+            BinningSpec(
+                [0, 2, 4], names=[0.1, float("nan")], nan_bin=float("nan"), right=False
+            ),
+        )
+        .map(
+            f=lambda row: {"X_binned": 0 if row["X_binned"] == 0.1 else 1},
+            new_column_types={"X_binned": ColumnType.INTEGER},
+        )
+        .groupby(KeySet.from_dict({"X_binned": [0, 1]}))
+        .count(),
+        None,
+        pd.DataFrame({"X_binned": [0, 1], "count": [2, 2]}),
+    ),
     (  # GroupByCount Filter
         QueryBuilder("private").filter("A == '0'").count(),
         GroupByCount(
             child=Filter(child=PrivateSource("private"), condition="A == '0'"),
             groupby_keys=KeySet.from_dict({}),
         ),
         pd.DataFrame({"count": [3]}),
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows.py` & `tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Tests for Session with the AddMaxRows ProtectedChange."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-member, no-self-use
+# pylint: disable=no-self-use
 
 import math
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
+from tmlt.core.measurements.interactive_measurements import PrivacyAccountantState
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.utils.exact_number import ExactNumber
+from tmlt.core.utils.parameters import calculate_noise_scale
 
 from tmlt.analytics._noise_info import _NoiseMechanism
 from tmlt.analytics._schema import ColumnType, Schema
 from tmlt.analytics._table_identifier import NamedTable
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
@@ -38,22 +42,16 @@
     ReplaceNullAndNan,
     Select,
     StdevMechanism,
     SumMechanism,
 )
 from tmlt.analytics.session import Session
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.measurements.interactive_measurements import PrivacyAccountantState
-from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
-from tmlt.core.utils.exact_number import ExactNumber
-from tmlt.core.utils.parameters import calculate_noise_scale
 
-from ....conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
-)
+from ....conftest import assert_frame_equal_with_sort
 from .conftest import EVALUATE_TESTS
 
 
 @pytest.mark.usefixtures("session_data")
 class TestSession:
     """Tests for Valid Sessions."""
 
@@ -427,15 +425,15 @@
         actual = session.evaluate(sum_query, privacy_budget)
         assert_frame_equal_with_sort(actual.toPandas(), expected, rtol=1)
 
     @pytest.mark.parametrize(
         "starting_budget,partition_budget",
         [
             (PureDPBudget(20), PureDPBudget(10)),
-            (ApproxDPBudget(20, 0.5), PureDPBudget(10)),
+            (ApproxDPBudget(20, 0.5), ApproxDPBudget(10, 0)),
             (RhoZCDPBudget(20), RhoZCDPBudget(10)),
         ],
     )
     def test_partition_and_create(
         self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
     ):
         """Tests using :func:`partition_and_create` to create a new session."""
@@ -466,15 +464,15 @@
             {"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER, "X": ColumnType.INTEGER}
         )
 
     @pytest.mark.parametrize(
         "starting_budget,partition_budget",
         [
             (PureDPBudget(20), PureDPBudget(10)),
-            (ApproxDPBudget(20, 0.5), PureDPBudget(10)),
+            (ApproxDPBudget(20, 0.5), ApproxDPBudget(10, 0)),
             (RhoZCDPBudget(20), RhoZCDPBudget(10)),
         ],
     )
     def test_partition_and_create_query(
         self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
     ):
         """Querying on a partitioned session with stability>1 works."""
@@ -515,14 +513,30 @@
         )
         query = GroupByCount(
             child=PrivateSource("private0"), groupby_keys=KeySet.from_dict({})
         )
         session2.evaluate(query, partition_budget)
 
     @pytest.mark.parametrize(
+        "starting_budget,partition_budget",
+        [(ApproxDPBudget(20, 0.5), PureDPBudget(10))],
+    )
+    def test_partition_and_create_approxDP_session_pureDP_partition(
+        self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
+    ):
+        """Tests using :func:`partition_and_create` to create a new ApproxDP session
+        that supports PureDP partitions."""
+
+        is_approxDP_starting_budget = isinstance(starting_budget, ApproxDPBudget)
+        if is_approxDP_starting_budget and isinstance(partition_budget, PureDPBudget):
+            partition_budget = ApproxDPBudget(partition_budget.epsilon, 0)
+
+        self.test_partition_and_create_query(starting_budget, partition_budget)
+
+    @pytest.mark.parametrize(
         "inf_budget,mechanism",
         [
             (PureDPBudget(float("inf")), CountMechanism.LAPLACE),
             (ApproxDPBudget(float("inf"), 0.5), CountMechanism.LAPLACE),
             (RhoZCDPBudget(float("inf")), CountMechanism.LAPLACE),
             (RhoZCDPBudget(float("inf")), CountMechanism.GAUSSIAN),
         ],
@@ -561,28 +575,33 @@
             ),
             inf_budget,
         )
         assert_frame_equal_with_sort(
             answer_session3.toPandas(), pd.DataFrame({"count": [1]})
         )
 
-    @pytest.mark.parametrize("output_measure", [(PureDP()), (RhoZCDP())])
+    @pytest.mark.parametrize("output_measure", [(PureDP()), (ApproxDP()), (RhoZCDP())])
     def test_partitions_composed(
         self, output_measure: Union[PureDP, ApproxDP, RhoZCDP]
     ):
         """Smoke test for composing :func:`partition_and_create`."""
         starting_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
         partition_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
         second_partition_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
         final_evaluate_budget: Union[PureDPBudget, ApproxDPBudget, RhoZCDPBudget]
         if output_measure == PureDP():
             starting_budget = PureDPBudget(20)
             partition_budget = PureDPBudget(10)
             second_partition_budget = PureDPBudget(5)
             final_evaluate_budget = PureDPBudget(2)
+        elif output_measure == ApproxDP():
+            starting_budget = ApproxDPBudget(20, 0)
+            partition_budget = ApproxDPBudget(10, 0)
+            second_partition_budget = ApproxDPBudget(5, 0)
+            final_evaluate_budget = ApproxDPBudget(2, 0)
         elif output_measure == RhoZCDP():
             starting_budget = RhoZCDPBudget(20)
             partition_budget = RhoZCDPBudget(10)
             second_partition_budget = RhoZCDPBudget(5)
             final_evaluate_budget = RhoZCDPBudget(2)
         else:
             pytest.fail(
@@ -665,15 +684,15 @@
         )
         session4.evaluate(query_expr=query, privacy_budget=final_evaluate_budget)
 
     @pytest.mark.parametrize(
         "starting_budget,partition_budget",
         [
             (PureDPBudget(20), PureDPBudget(10)),
-            (ApproxDPBudget(20, 0.5), PureDPBudget(10)),
+            (ApproxDPBudget(20, 0.5), ApproxDPBudget(10, 0)),
             (RhoZCDPBudget(20), RhoZCDPBudget(10)),
         ],
     )
     def test_partition_execution_order(
         self, starting_budget: PrivacyBudget, partition_budget: PrivacyBudget
     ):
         """Tests behavior using :func:`partition_and_create` sessions out of order."""
@@ -953,14 +972,66 @@
         assert len(list(spark.sparkContext._jsc.sc().getRDDStorageInfo())) == 2
         # Delete views
         session.delete_view("view1")
         assert len(list(spark.sparkContext._jsc.sc().getRDDStorageInfo())) == 1
         session.delete_view("view2")
         assert len(list(spark.sparkContext._jsc.sc().getRDDStorageInfo())) == 0
 
+    # regression test for #2491
+    def test_filter_regression(self, spark) -> None:
+        """Regression tests for issue 2491.
+
+        This issue caused incorrect results when joining a dataframe with
+        another dataframe derived from the first (in this case, a KeySet
+        derived from the private data).
+        """
+        sdf = spark.createDataFrame(
+            pd.DataFrame(
+                [["0", 1, 100000], ["1", 0, 20000], ["1", 2, 20000]],
+                columns=["A", "B", "X"],
+            )
+        )
+        total_budget = 10
+        session = Session.from_dataframe(
+            privacy_budget=PureDPBudget(total_budget),
+            source_id="private",
+            dataframe=sdf,
+            protected_change=AddOneRow(),
+        )
+
+        all_keys = KeySet.from_dataframe(sdf)
+        keyset = all_keys["A", "B"]
+        budget_per_query = PureDPBudget(total_budget / 3)
+        expected_a_b = pd.DataFrame([["0", 1], ["1", 0], ["1", 2]], columns=["A", "B"])
+
+        count_query = QueryBuilder("private").filter("B == 2").groupby(keyset).count()
+        count_result = session.evaluate(count_query, budget_per_query)
+        count_a_b = count_result.select("A", "B")
+        assert_frame_equal_with_sort(count_a_b.toPandas(), expected_a_b)
+
+        median_query = (
+            QueryBuilder("private")
+            .filter("B == 2")
+            .groupby(keyset)
+            .median("X", 0, 10**6, "dp_median")
+        )
+        median_result = session.evaluate(median_query, budget_per_query)
+        median_a_b = median_result.select("A", "B")
+        assert_frame_equal_with_sort(median_a_b.toPandas(), expected_a_b)
+
+        average_query = (
+            QueryBuilder("private")
+            .filter("B == 2")
+            .groupby(keyset)
+            .average("X", 0, 10**6, "dp_average")
+        )
+        average_result = session.evaluate(average_query, budget_per_query)
+        average_a_b = average_result.select("A", "B")
+        assert_frame_equal_with_sort(average_a_b.toPandas(), expected_a_b)
+
     def test_grouping_noninteger_stability(self, spark) -> None:
         """Test that zCDP grouping_column and non-integer stabilities work."""
         grouped_df = spark.createDataFrame(
             pd.DataFrame({"id": [7, 7, 8, 9], "group": [0, 1, 0, 1]})
         )
         ks = KeySet.from_dict({"group": [0, 1]})
         query = QueryBuilder("id").groupby(ks).count()
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_in_max_groups.py` & `tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_in_max_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 sanity check that the Session is working correctly with AddMaxRowsInMaxGroups. More
 thorough tests for Session are in
 test/system/session/rows/test_add_max_rows.py."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-member, no-self-use
-
+# pylint: disable=no-self-use
 
 from typing import Any, Dict, List
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
+from tmlt.core.measures import RhoZCDP
+from tmlt.core.utils.exact_number import ExactNumber
+from tmlt.core.utils.parameters import calculate_noise_scale
 
 from tmlt.analytics._noise_info import _NoiseMechanism
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PrivacyBudget, PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.protected_change import AddMaxRowsInMaxGroups
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import (
@@ -28,17 +30,14 @@
     CountMechanism,
     GroupByBoundedAverage,
     GroupByCount,
     PrivateSource,
     QueryExpr,
 )
 from tmlt.analytics.session import Session
-from tmlt.core.measures import RhoZCDP
-from tmlt.core.utils.exact_number import ExactNumber
-from tmlt.core.utils.parameters import calculate_noise_scale
 
 
 @pytest.mark.usefixtures("session_data")
 class TestSession:
     """Tests for Valid Sessions."""
 
     sdf: DataFrame
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_infs_nulls.py` & `tmlt_analytics-0.7.1/test/system/session/rows/test_add_max_rows_infs_nulls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """System tests for Sessions with Nulls and Infs."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-member, no-self-use
-
 import datetime
 from typing import Any, Dict, List, Mapping, Tuple, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
+from tmlt.core.measurements.interactive_measurements import SequentialQueryable
 
 from tmlt.analytics._table_identifier import NamedTable
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget
 from tmlt.analytics.protected_change import AddOneRow
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import AnalyticsDefault
 from tmlt.analytics.session import Session
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.measurements.interactive_measurements import SequentialQueryable
 
-from ....conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
-)
+from ....conftest import assert_frame_equal_with_sort
 
 
 @pytest.mark.usefixtures("null_session_data")
 class TestSessionWithNulls:
     """Tests for sessions with Nulls."""
 
     pdf: pd.DataFrame
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/rows/test_invalid.py` & `tmlt_analytics-0.7.1/test/system/session/rows/test_invalid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Tests for invalid session configurations."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-member, no-self-use
-
 from typing import Dict, Type, Union
 from unittest.mock import Mock
 
 import pytest
 from pyspark.sql import DataFrame
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.metrics import DictMetric, SymmetricDifference
+from tmlt.core.utils.exact_number import ExactNumber
 
 from tmlt.analytics._schema import Schema
 from tmlt.analytics._table_identifier import NamedTable
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import ApproxDPBudget, PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.protected_change import AddOneRow
 from tmlt.analytics.query_expr import (
@@ -22,19 +25,14 @@
     GroupByCount,
     PrivateSource,
     QueryExpr,
     Rename,
     ReplaceNullAndNan,
 )
 from tmlt.analytics.session import Session
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
-from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
-from tmlt.core.metrics import DictMetric, SymmetricDifference
-from tmlt.core.utils.exact_number import ExactNumber
 
 
 @pytest.mark.usefixtures("session_data")
 class TestInvalidSession:
     """Tests for Invalid Sessions."""
 
     sdf: DataFrame
@@ -68,15 +66,15 @@
         )
         mock_accountant.input_domain = DictDomain(
             {NamedTable("private"): self.sdf_input_domain}
         )
         mock_accountant.d_in = {NamedTable("private"): ExactNumber(1)}
         mock_accountant.privacy_budget = ExactNumber(float("inf"))
 
-        session = Session(accountant=mock_accountant, public_sources=dict())
+        session = Session(accountant=mock_accountant, public_sources={})
         session.create_view(PrivateSource("private"), "view", cache=False)
         with pytest.raises(error_type, match=expected_error_msg):
             session.evaluate(query_expr, privacy_budget=PureDPBudget(float("inf")))
 
     @pytest.mark.parametrize("output_measure", [(PureDP()), (ApproxDP()), (RhoZCDP())])
     def test_invalid_privacy_budget_evaluate_and_create(
         self, output_measure: Union[PureDP, RhoZCDP]
```

### Comparing `tmlt_analytics-0.7.0rc1/test/system/session/test_invalid_constraints.py` & `tmlt_analytics-0.7.1/test/system/session/test_invalid_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,62 @@
 """Tests for MeasurementVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=protected-access, no-member, no-self-use
+# pylint: disable=no-self-use
 
 from typing import List, Optional, Union
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
 import sympy as sp
 from pyspark.sql import DataFrame
 from pyspark.sql.types import LongType, StringType, StructField, StructType
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import (
+    SparkColumnDescriptor,
+    SparkDataFrameDomain,
+    SparkFloatColumnDescriptor,
+    SparkGroupedDataFrameDomain,
+    SparkIntegerColumnDescriptor,
+    SparkStringColumnDescriptor,
+)
+from tmlt.core.measurements.aggregations import NoiseMechanism
+from tmlt.core.measurements.base import Measurement
+from tmlt.core.measurements.chaining import ChainTM
+from tmlt.core.measures import PureDP, RhoZCDP
+from tmlt.core.metrics import (
+    DictMetric,
+    HammingDistance,
+    IfGroupedBy,
+    RootSumOfSquared,
+    SumOf,
+    SymmetricDifference,
+)
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.chaining import ChainTT
+from tmlt.core.transformations.spark_transformations.groupby import GroupBy
+from tmlt.core.transformations.spark_transformations.select import (
+    Select as SelectTransformation,
+)
+from tmlt.core.utils.exact_number import ExactNumber
+from tmlt.core.utils.type_utils import assert_never
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._measurement_visitor import (
     MeasurementVisitor,
     _get_query_bounds,
 )
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
 from tmlt.analytics._table_identifier import NamedTable
 from tmlt.analytics._table_reference import lookup_domain, lookup_metric
 from tmlt.analytics.keyset import KeySet
+from tmlt.analytics.privacy_budget import PureDPBudget
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
 )
 from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
 from tmlt.analytics.query_expr import (
@@ -48,47 +78,16 @@
     Rename,
 )
 from tmlt.analytics.query_expr import ReplaceInfinity as ReplaceInfExpr
 from tmlt.analytics.query_expr import ReplaceNullAndNan
 from tmlt.analytics.query_expr import Select as SelectExpr
 from tmlt.analytics.query_expr import StdevMechanism, SumMechanism, VarianceMechanism
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import (
-    SparkColumnDescriptor,
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-    SparkGroupedDataFrameDomain,
-    SparkIntegerColumnDescriptor,
-    SparkStringColumnDescriptor,
-)
-from tmlt.core.measurements.aggregations import NoiseMechanism
-from tmlt.core.measurements.base import Measurement
-from tmlt.core.measurements.chaining import ChainTM
-from tmlt.core.measures import PureDP, RhoZCDP
-from tmlt.core.metrics import (
-    DictMetric,
-    HammingDistance,
-    IfGroupedBy,
-    RootSumOfSquared,
-    SumOf,
-    SymmetricDifference,
-)
-from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.spark_transformations.groupby import GroupBy
-from tmlt.core.transformations.spark_transformations.select import (
-    Select as SelectTransformation,
-)
-from tmlt.core.utils.exact_number import ExactNumber
-from tmlt.core.utils.type_utils import assert_never
 
-from ...conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
-)
+from ...conftest import assert_frame_equal_with_sort
 
 
 def chain_to_list(t: ChainTT) -> List[Transformation]:
     """Turns a ChainTT's tree into a list."""
     left: List[Transformation]
     if not isinstance(t.transformation1, ChainTT):
         left = [t.transformation1]
@@ -276,33 +275,33 @@
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
         },
     )
     request.cls.catalog = catalog
 
-    budget = ExactNumber(10).expr
+    budget = PureDPBudget(10)
     stability = {
         NamedTable("private"): ExactNumber(3).expr,
         NamedTable("private_2"): ExactNumber(3).expr,
     }
     request.cls.visitor = MeasurementVisitor(
-        per_query_privacy_budget=budget,
+        privacy_budget=budget,
         stability=stability,
         input_domain=input_domain,
         input_metric=input_metric,
         output_measure=PureDP(),
         default_mechanism=NoiseMechanism.LAPLACE,
         public_sources=public_sources,
         catalog=catalog,
         table_constraints={t: [] for t in stability},
     )
     # for the methods which alter the output measure of a visitor.
     request.cls.pick_noise_visitor = MeasurementVisitor(
-        per_query_privacy_budget=budget,
+        privacy_budget=budget,
         stability=stability,
         input_domain=input_domain,
         input_metric=input_metric,
         output_measure=PureDP(),
         default_mechanism=NoiseMechanism.LAPLACE,
         public_sources=public_sources,
         catalog=catalog,
@@ -1054,15 +1053,15 @@
 
     def test_validate_measurement(self):
         """Test _validate_measurement."""
         with patch(
             "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
             autospec=True,
         ) as mock_measurement:
-            mock_measurement.privacy_function.return_value = self.visitor.budget
+            mock_measurement.privacy_function.return_value = self.visitor.budget.value
             mid_stability = ExactNumber(2).expr
             # This should finish without raising an error
             # pylint: disable=protected-access
             self.visitor._validate_measurement(mock_measurement, mid_stability)
 
             # Change it so that the privacy function returns something else
             mock_measurement.privacy_function.return_value = ExactNumber(-10).expr
@@ -1130,15 +1129,15 @@
         # pylint: enable=protected-access
         mock_measurement.input_domain = lookup_domain(
             transformation.output_domain, reference
         )
         mock_measurement.input_metric = lookup_metric(
             transformation.output_metric, reference
         )
-        mock_measurement.privacy_function.return_value = self.visitor.budget
+        mock_measurement.privacy_function.return_value = self.visitor.budget.value
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
         [
             (
                 GroupByCount(
                     child=PrivateSource("private"),
@@ -1227,15 +1226,15 @@
                 self.visitor.stability
             )
             mock_create_count.assert_called_with(
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 noise_mechanism=expected_mechanism,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 count_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
@@ -1365,15 +1364,15 @@
             )
 
             mock_create_count_distinct.assert_called_with(
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 noise_mechanism=expected_mechanism,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 count_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_new_child",
@@ -1524,15 +1523,15 @@
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 measure_column=query.measure_column,
                 quantile=query.quantile,
                 lower=query.low,
                 upper=query.high,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 quantile_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
@@ -1635,15 +1634,15 @@
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 measure_column=query.measure_column,
                 lower=lower,
                 upper=upper,
                 noise_mechanism=expected_mechanism,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 sum_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
@@ -1746,15 +1745,15 @@
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 measure_column=query.measure_column,
                 lower=lower,
                 upper=upper,
                 noise_mechanism=expected_mechanism,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 average_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
@@ -1857,15 +1856,15 @@
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 measure_column=query.measure_column,
                 lower=lower,
                 upper=upper,
                 noise_mechanism=expected_mechanism,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 variance_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
@@ -1969,15 +1968,15 @@
                 input_domain=measurement.transformation.output_domain,
                 input_metric=measurement.transformation.output_metric,
                 measure_column=query.measure_column,
                 lower=lower,
                 upper=upper,
                 noise_mechanism=expected_mechanism,
                 d_in=mid_stability,
-                d_out=self.visitor.budget,
+                d_out=self.visitor.budget.value,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 standard_deviation_column=query.output_column,
             )
 
     @pytest.mark.parametrize(
         "query",
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Tests for OutputSchemaVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-self-use, protected-access, no-member
-
 import datetime
 from typing import Dict, List, Type
 
 import pytest
 from pyspark.sql import SparkSession
 from pyspark.sql.types import LongType, StringType, StructField, StructType
 
@@ -117,27 +115,31 @@
         ),
         "Tables have no common columns to join on",
     ),
     (  # JoinPublic on column with mismatched types
         JoinPublic(
             child=PrivateSource("private"), public_table="public", join_columns=["A"]
         ),
-        "Join columns must have identical types on both tables, "
-        "but column 'A' does not",
+        (
+            "Join columns must have identical types on both tables, "
+            "but column 'A' does not"
+        ),
     ),
     (  # JoinPrivate on column with mismatched types
         JoinPrivate(
             PrivateSource("private"),
             Rename(Rename(PrivateSource("private"), {"A": "Q"}), {"B": "A"}),
             TruncationStrategy.DropExcess(1),
             TruncationStrategy.DropExcess(1),
             join_columns=["A"],
         ),
-        "Join columns must have identical types on both tables, "
-        "but column 'A' does not",
+        (
+            "Join columns must have identical types on both tables, "
+            "but column 'A' does not"
+        ),
     ),
     (  # Filter on invalid column
         Filter(child=PrivateSource("private"), condition="NONEXISTENT>1"),
         "Invalid filter condition 'NONEXISTENT>1'.*",
     ),
     (  # Rename on non-existent column
         Rename(child=PrivateSource("private"), column_mapper={"NONEXISTENT": "Z"}),
@@ -161,16 +163,18 @@
                 max_num_rows=2,
             ),
             f=lambda row: [{"j": row["X"]} for i in range(row["Repeat"])],
             schema_new_columns=Schema({"j": "INTEGER"}, grouping_column="j"),
             augment=True,
             max_num_rows=2,
         ),
-        "Multiple grouping transformations are used in this query. "
-        "Only one grouping transformation is allowed.",
+        (
+            "Multiple grouping transformations are used in this query. "
+            "Only one grouping transformation is allowed."
+        ),
     ),
     (  # FlatMap with inner grouping FlatMap but outer augment=False
         FlatMap(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
@@ -241,27 +245,31 @@
             groupby_keys=KeySet.from_dict({"B": [0, 1, 2]}),
             measure_column="A",
             quantile=0.5,
             low=10,
             high=20,
             output_column="out",
         ),
-        "Quantile query's measure column 'A' has invalid type "
-        "'VARCHAR'. Expected types: 'INTEGER' or 'DECIMAL'.",
+        (
+            "Quantile query's measure column 'A' has invalid type "
+            "'VARCHAR'. Expected types: 'INTEGER' or 'DECIMAL'."
+        ),
     ),
     (  # Type mismatch for the measure column of GroupByBoundedAverage
         GroupByBoundedAverage(
             child=PrivateSource("private"),
             groupby_keys=KeySet.from_dict({}),
             measure_column="A",
             low=0.0,
             high=1.0,
         ),
-        "measure column 'A' has invalid type 'VARCHAR'. "
-        "Expected types: 'INTEGER' or 'DECIMAL'",
+        (
+            "measure column 'A' has invalid type 'VARCHAR'. "
+            "Expected types: 'INTEGER' or 'DECIMAL'"
+        ),
     ),
     (  # Grouping column is set in a FlatMap but not used in a later GroupBy
         GroupByCount(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["B"]} for i in range(row["Repeat"])],
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
@@ -277,15 +285,14 @@
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["B"]} for i in range(row["Repeat"])],
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
                 augment=True,
                 max_num_rows=2,
             ),
-            # pylint: disable=protected-access
             groupby_keys=KeySet(dataframe=GET_GROUPBY_COLUMN_A),
         ),
         "Column 'i' produced by grouping transformation is not in groupby columns",
     ),
 ]
 
 ###TESTS FOR QUERY VALIDATION###
@@ -349,38 +356,44 @@
 
     @pytest.mark.parametrize(
         "groupby_keys,exception_type,expected_error_msg",
         [
             (
                 KeySet.from_dict({"A": [0, 1]}),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
             (
                 KeySet.from_dict({"X": [0, 1]}),
                 ValueError,
-                "Groupby column 'X' has type 'INTEGER', but the column with the"
-                " same name in the input data has type 'DECIMAL' instead.",
+                (
+                    "Groupby column 'X' has type 'INTEGER', but the column with the"
+                    " same name in the input data has type 'DECIMAL' instead."
+                ),
             ),
             (
                 KeySet.from_dict({"Y": ["0"]}),
                 KeyError,
                 "Groupby column 'Y' is not in the input schema.",
             ),
             (
                 KeySet(dataframe=GET_GROUPBY_NON_EXISTING_COLUMN),
                 KeyError,
                 "Groupby column 'yay' is not in the input schema.",
             ),
             (
                 KeySet(dataframe=GET_GROUPBY_COLUMN_WRONG_TYPE),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
         ],
     )
     def test_invalid_group_by_count(
         self,
         groupby_keys: KeySet,
         exception_type: Type[Exception],
@@ -397,16 +410,18 @@
                 KeySet.from_dict({"B": [0, 1]}),
                 ValueError,
                 "Column to aggregate must be a non-grouped column, not 'B'",
             ),
             (
                 KeySet.from_dict({"A": [0, 1]}),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
             (
                 KeySet.from_dict({"Y": ["0"]}),
                 KeyError,
                 "Groupby column 'Y' is not in the input schema.",
             ),
             (
@@ -418,16 +433,18 @@
                 KeySet(dataframe=GET_GROUPBY_NON_EXISTING_COLUMN),
                 KeyError,
                 "Groupby column 'yay' is not in the input schema.",
             ),
             (
                 KeySet(dataframe=GET_GROUPBY_COLUMN_WRONG_TYPE),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
         ],
     )
     def test_invalid_group_by_aggregations(
         self,
         groupby_keys: KeySet,
         exception_type: Type[Exception],
@@ -513,32 +530,36 @@
 
     @pytest.mark.parametrize(
         "groupby_keys,exception_type,expected_error_msg",
         [
             (
                 KeySet.from_dict({"A": [0, 1]}),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
             (
                 KeySet.from_dict({"Y": ["0"]}),
                 KeyError,
                 "Groupby column 'Y' is not in the input schema.",
             ),
             (
                 KeySet(dataframe=GET_GROUPBY_NON_EXISTING_COLUMN),
                 KeyError,
                 "Groupby column 'yay' is not in the input schema.",
             ),
             (
                 KeySet(dataframe=GET_GROUPBY_COLUMN_WRONG_TYPE),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
         ],
     )
     def test_invalid_group_by_count_null(
         self,
         groupby_keys: KeySet,
         exception_type: Type[Exception],
@@ -555,16 +576,18 @@
                 KeySet.from_dict({"B": [0, 1]}),
                 ValueError,
                 "Column to aggregate must be a non-grouped column, not 'B'",
             ),
             (
                 KeySet.from_dict({"A": [0, 1]}),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
             (
                 KeySet.from_dict({"Y": ["0"]}),
                 KeyError,
                 "Groupby column 'Y' is not in the input schema.",
             ),
             (
@@ -576,16 +599,18 @@
                 KeySet(dataframe=GET_GROUPBY_NON_EXISTING_COLUMN),
                 KeyError,
                 "Groupby column 'yay' is not in the input schema.",
             ),
             (
                 KeySet(dataframe=GET_GROUPBY_COLUMN_WRONG_TYPE),
                 ValueError,
-                "Groupby column 'A' has type 'INTEGER', but the column "
-                "with the same name in the input data has type 'VARCHAR' instead.",
+                (
+                    "Groupby column 'A' has type 'INTEGER', but the column "
+                    "with the same name in the input data has type 'VARCHAR' instead."
+                ),
             ),
         ],
     )
     def test_invalid_group_by_aggregations_null(
         self,
         groupby_keys: KeySet,
         exception_type: Type[Exception],
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/conftest.py` & `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/conftest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,23 +15,14 @@
     FloatType,
     LongType,
     StringType,
     StructField,
     StructType,
     TimestampType,
 )
-
-from tmlt.analytics._catalog import Catalog
-from tmlt.analytics._query_expr_compiler._transformation_visitor import (
-    TransformationVisitor,
-)
-from tmlt.analytics._schema import ColumnDescriptor, ColumnType
-from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
-from tmlt.analytics._table_reference import TableReference
-from tmlt.analytics._transformation_utils import get_table_from_ref
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkColumnDescriptor,
     SparkDataFrameDomain,
     SparkDateColumnDescriptor,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
@@ -39,14 +30,23 @@
     SparkTimestampColumnDescriptor,
 )
 from tmlt.core.measurements.aggregations import NoiseMechanism
 from tmlt.core.metrics import AddRemoveKeys, DictMetric, SymmetricDifference
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.chaining import ChainTT
 
+from tmlt.analytics._catalog import Catalog
+from tmlt.analytics._query_expr_compiler._transformation_visitor import (
+    TransformationVisitor,
+)
+from tmlt.analytics._schema import ColumnDescriptor, ColumnType
+from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
+from tmlt.analytics._table_reference import TableReference
+from tmlt.analytics._transformation_utils import get_table_from_ref
+
 from ....conftest import assert_frame_equal_with_sort
 
 # Example date and timestamp
 DATE1 = datetime.date.fromisoformat("2022-01-01")
 TIMESTAMP1 = datetime.datetime.fromisoformat("2022-01-01T12:30:00")
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py` & `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 import datetime
 from typing import Dict, List, Mapping, Tuple, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
+from tmlt.core.domains.spark_domains import (
+    SparkDataFrameDomain,
+    SparkFloatColumnDescriptor,
+)
+from tmlt.core.metrics import IfGroupedBy, SymmetricDifference
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.chaining import ChainTT
+from tmlt.core.transformations.identity import Identity as IdentityTransformation
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
@@ -33,22 +41,14 @@
     QueryExpr,
     Rename,
     ReplaceInfinity,
     ReplaceNullAndNan,
     Select,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.domains.spark_domains import (
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-)
-from tmlt.core.metrics import IfGroupedBy, SymmetricDifference
-from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.identity import Identity as IdentityTransformation
 
 from .conftest import (
     DATE1,
     TIMESTAMP1,
     TestTransformationVisitor,
     TestTransformationVisitorNulls,
     chain_to_list,
@@ -459,15 +459,15 @@
                 ),
             ),
         ],
     )
     def test_visit_replace_null_and_nan(
         self,
         replace_with: Mapping[
-            str, Union[int, float, str, datetime.date, datetime.datetime, float]
+            str, Union[int, float, str, datetime.date, datetime.datetime]
         ],
         expected_df: DataFrame,
     ):
         """Test generating transformations from a ReplaceNullAndNan."""
         query = ReplaceNullAndNan(PrivateSource("ids_infs_nans"), replace_with)
         transformation, reference, constraints = query.accept(self.visitor)
         self._validate_transform_basics(transformation, reference, query)
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py` & `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 import datetime
 from typing import Dict, List, Mapping, Optional, Tuple, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
 from pyspark.sql.types import LongType, StringType, StructField, StructType
+from tmlt.core.domains.spark_domains import (
+    SparkDataFrameDomain,
+    SparkFloatColumnDescriptor,
+)
+from tmlt.core.metrics import IfGroupedBy, SymmetricDifference
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.chaining import ChainTT
+from tmlt.core.transformations.dictionary import AugmentDictTransformation
+from tmlt.core.transformations.identity import Identity as IdentityTransformation
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
@@ -46,23 +55,14 @@
     QueryExpr,
     Rename,
     ReplaceInfinity,
     ReplaceNullAndNan,
     Select,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.domains.spark_domains import (
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-)
-from tmlt.core.metrics import IfGroupedBy, SymmetricDifference
-from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.dictionary import AugmentDictTransformation
-from tmlt.core.transformations.identity import Identity as IdentityTransformation
 
 from .conftest import (
     DATE1,
     TIMESTAMP1,
     TestTransformationVisitor,
     TestTransformationVisitorNulls,
     chain_to_list,
@@ -565,15 +565,15 @@
                 ),
             ),
         ],
     )
     def test_visit_replace_null_and_nan(
         self,
         replace_with: Mapping[
-            str, Union[int, float, str, datetime.date, datetime.datetime, float]
+            str, Union[int, float, str, datetime.date, datetime.datetime]
         ],
         expected_df: DataFrame,
     ):
         """Test visit_replace_null_and_nan."""
         query = ReplaceNullAndNan(
             child=PrivateSource(source_id="rows_infs_nans"), replace_with=replace_with
         )
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py` & `tmlt_analytics-0.7.1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 # Copyright Tumult Labs 2023
 
 from typing import Dict, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import DataFrame
+from tmlt.core.metrics import SymmetricDifference
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
 )
 from tmlt.analytics._table_identifier import Identifier
 from tmlt.analytics._transformation_utils import get_table_from_ref
 from tmlt.analytics.constraints import (
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
 )
 from tmlt.analytics.query_expr import EnforceConstraint, PrivateSource
-from tmlt.core.metrics import SymmetricDifference
 
 from .conftest import TestTransformationVisitor
 
 
 class TestConstraints(TestTransformationVisitor):
     """Tests for constraint handling in the transformation visitor."""
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_binning_spec.py` & `tmlt_analytics-0.7.1/test/unit/test_binning_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # pylint: disable=pointless-string-statement
 
 import datetime
 from typing import Any, List
 
 import pytest
 
+from tmlt.analytics._schema import ColumnDescriptor
 from tmlt.analytics.binning_spec import BinningSpec, _default_bin_names, _edges_as_str
 from tmlt.analytics.query_builder import ColumnType
 
 """Tests for helper functions releated to default bin names."""
 
 
 @pytest.mark.parametrize(
@@ -83,15 +84,17 @@
     assert spec.bins(include_null=True) == [
         "[0, 5]",
         "(5, 10]",
         "(10, 15]",
         "(15, 20]",
         None,
     ]
-    assert spec.column_descriptor.column_type == ColumnType.VARCHAR
+    assert spec.column_descriptor == ColumnDescriptor(
+        ColumnType.VARCHAR, allow_null=True, allow_nan=False, allow_inf=False
+    )
     bin_tests = {
         2: "[0, 5]",
         7: "(5, 10]",
         12: "(10, 15]",
         17: "(15, 20]",
         -1: None,
         0: "[0, 5]",
@@ -165,38 +168,48 @@
     edges = [0, 5, 10]
     spec = BinningSpec(edges, names=[float("NaN"), float("0")])
     assert spec.column_descriptor.allow_nan
     spec = BinningSpec(edges, names=[float("-NaN"), float("0")])
     assert spec.column_descriptor.allow_nan
     spec = BinningSpec(edges, names=[float("0"), float("5")])
     assert not spec.column_descriptor.allow_nan
+    spec = BinningSpec(edges, names=[float("0"), float(5)], nan_bin=float("nan"))
+    assert spec.column_descriptor.allow_nan
+    spec = BinningSpec(edges, names=[float("0"), float(5)], nan_bin=3.3)
+    assert not spec.column_descriptor.allow_nan
 
 
 def test_binning_allow_null() -> None:
     """BinningSpec sets allow_null as expected."""
     edges = [0, 5, 10]
     spec = BinningSpec(edges, names=["null", "5"])
     assert spec.column_descriptor.allow_null
     spec = BinningSpec(edges, names=["NULL", "5"])
     assert spec.column_descriptor.allow_null
     spec = BinningSpec(edges, names=["Null", "5"])
     assert spec.column_descriptor.allow_null
     spec = BinningSpec(edges, names=["0", "5"])
-    assert not spec.column_descriptor.allow_null
+    assert spec.column_descriptor.allow_null
 
 
 def test_binning_allow_inf() -> None:
     """BinningSpec sets allow_inf as expected."""
     edges = [float("0"), float("5"), float("10")]
     spec = BinningSpec(edges, names=[float("0"), float("inf")])
     assert spec.column_descriptor.allow_inf
     spec = BinningSpec(edges, names=[float("0"), float("-inf")])
     assert spec.column_descriptor.allow_inf
     spec = BinningSpec(edges, names=[float("0"), float("5")])
     assert not spec.column_descriptor.allow_inf
+    spec = BinningSpec(edges, names=[float("0"), float("nan")], nan_bin=float("inf"))
+    assert spec.column_descriptor.allow_inf
+    spec = BinningSpec(edges, names=[float("0"), float("nan")], nan_bin=float("-inf"))
+    assert spec.column_descriptor.allow_inf
+    spec = BinningSpec(edges, names=[float("0"), float(5)], nan_bin=3.3)
+    assert not spec.column_descriptor.allow_inf
 
 
 def test_binning_noninclusive() -> None:
     """BinningSpec with include_both_endpoints=False works as expected."""
     spec = BinningSpec([0, 5, 10, 15, 20], include_both_endpoints=False)
     assert spec.bins() == ["(0, 5]", "(5, 10]", "(10, 15]", "(15, 20]"]
     assert spec(0) is None
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_catalog.py` & `tmlt_analytics-0.7.1/test/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_cleanup.py` & `tmlt_analytics-0.7.1/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_constraints.py` & `tmlt_analytics-0.7.1/test/unit/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_keyset.py` & `tmlt_analytics-0.7.1/test/unit/test_keyset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Unit tests for KeySet."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
-# pylint: disable=no-self-use
-
 
 import datetime
 from typing import Dict, List, Mapping, Optional, Union
 
 import pandas as pd
 import pytest
 from pyspark.sql import Column
@@ -22,15 +20,15 @@
     StructType,
     TimestampType,
 )
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
 from tmlt.analytics.keyset import KeySet, _check_df_schema, _check_dict_schema
 
-from ..conftest import assert_frame_equal_with_sort  # pylint: disable=no-name-in-module
+from ..conftest import assert_frame_equal_with_sort
 
 
 @pytest.mark.parametrize(
     "types",
     [
         (StructType([StructField("A", LongType(), False)])),
         (
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_neighboring_relations.py` & `tmlt_analytics-0.7.1/test/unit/test_neighboring_relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-"""Tests for Neighboring Relations"""
-# pylint: disable=no-self-use, no-member
+"""Tests for neighboring relations."""
+
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2023
+
+# pylint: disable=no-self-use
+
 from cmath import inf, pi
 from typing import Dict
 
 import pandas as pd
 import pytest
 import sympy as sp
 from pyspark.sql import DataFrame
-
-from tmlt.analytics._neighboring_relation import (
-    AddRemoveKeys,
-    AddRemoveRows,
-    AddRemoveRowsAcrossGroups,
-    Conjunction,
-)
-from tmlt.analytics._neighboring_relation_visitor import NeighboringRelationCoreVisitor
-from tmlt.analytics._table_identifier import NamedTable, TableCollection
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.measures import PureDP, RhoZCDP
 from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
 from tmlt.core.metrics import (
     DictMetric,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.utils.exact_number import ExactNumber
 
+from tmlt.analytics._neighboring_relation import (
+    AddRemoveKeys,
+    AddRemoveRows,
+    AddRemoveRowsAcrossGroups,
+    Conjunction,
+)
+from tmlt.analytics._neighboring_relation_visitor import NeighboringRelationCoreVisitor
+from tmlt.analytics._table_identifier import NamedTable, TableCollection
+
 
 @pytest.fixture(name="test_data", scope="class")
 def setup_test_data(request, spark) -> None:
     """Set up test data."""
     table1 = spark.createDataFrame(
         pd.DataFrame(
             [["0", 1, 0], ["1", 0, 1], ["1", 2, 1], ["1", 2, 0]],
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_noise_info.py` & `tmlt_analytics-0.7.1/test/unit/test_noise_info.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 from typing import Dict
 
 import pytest
 import sympy as sp
-
-from tmlt.analytics._noise_info import (
-    _inverse_cdf,
-    _noise_from_measurement,
-    _NoiseMechanism,
-)
 from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
 from tmlt.core.domains.pandas_domains import PandasSeriesDomain
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.noise_mechanisms import (
     AddDiscreteGaussianNoise,
     AddGeometricNoise,
     AddLaplaceNoise,
 )
 from tmlt.core.measurements.pandas_measurements.series import NoisyQuantile
 from tmlt.core.measures import PureDP
 
+from tmlt.analytics._noise_info import (
+    _inverse_cdf,
+    _noise_from_measurement,
+    _NoiseMechanism,
+)
+
 
 @pytest.mark.parametrize(
     "measurement,expected",
     [
         (
             AddLaplaceNoise(NumpyIntegerDomain(), scale=sp.Rational(2.5)),
             [{"noise_mechanism": _NoiseMechanism.LAPLACE, "noise_parameter": 2.5}],
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget.py` & `tmlt_analytics-0.7.1/test/unit/test_privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.1/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 """Tests for :mod:`tmlt.analytics._privacy_budget_rounding_helper`."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 # pylint: disable=pointless-string-statement
 
 
+from tmlt.core.utils.exact_number import ExactNumber
 from typeguard import typechecked
 
 from tmlt.analytics._privacy_budget_rounding_helper import (
     BUDGET_RELATIVE_TOLERANCE,
     get_adjusted_budget,
     requested_budget_is_slightly_higher_than_remaining,
 )
-from tmlt.core.utils.exact_number import ExactNumber
+from tmlt.analytics.privacy_budget import PureDPBudget
 
 """Tests for converting a numeric budget into symbolic representation."""
-REMAINING_INT = 100
-REMAINING_EXACT = ExactNumber(100)
+FUDGE_FACTOR = 1 / 1e9
+INT_100 = 100
+PURE_DP_99 = PureDPBudget(99)
+PURE_DP_100 = PureDPBudget(100)
+PURE_DP_101 = PureDPBudget(101)
 
 
 def test_int_request():
     """Make sure int requests are handled properly.
 
     If the requested and remaining budgets are both reasonable integral values
     (i.e., nowhere near 10^9, which would be ridiculous for privacy parameters),
     we should never run into the tolerance threshold issue. This means the
     requested budget should be returned in all cases.
     """
-    adjusted = get_adjusted_budget(99, REMAINING_EXACT)
-    assert adjusted == 99
-    adjusted = get_adjusted_budget(101, REMAINING_EXACT)
-    assert adjusted == 101
+
+    adjusted = get_adjusted_budget(PURE_DP_99, PURE_DP_100)
+    assert adjusted == PURE_DP_99
+    adjusted = get_adjusted_budget(PURE_DP_101, PURE_DP_100)
+    assert adjusted == PURE_DP_101
 
 
 def test_float_request():
     """Make sure float requests are handled properly.
 
     The only time the remaining budget should be returned is if the
     requested budget is slightly less than the remaining.
     """
     # We should never round up.
-    adjusted = get_adjusted_budget(99.1, REMAINING_EXACT)
-    assert adjusted == ExactNumber.from_float(99.1, False)
-    fudge_factor = 1 / 1e9
+    adjusted = get_adjusted_budget(PureDPBudget(99.1), PURE_DP_100)
+    assert adjusted == PureDPBudget(99.1)
+
     # Even if request is only slightly less, we still should not round up.
-    requested = REMAINING_INT - fudge_factor
-    adjusted = get_adjusted_budget(requested, REMAINING_EXACT)
-    assert adjusted == ExactNumber.from_float(requested, False)
+    requested = PureDPBudget(INT_100 - FUDGE_FACTOR)
+    adjusted = get_adjusted_budget(requested, PURE_DP_100)
+    assert adjusted == requested
+
     # Slightly greater than the remaining budget means we should round down.
-    requested = REMAINING_INT + fudge_factor
-    adjusted = get_adjusted_budget(requested, REMAINING_EXACT)
-    assert adjusted == REMAINING_EXACT
+    requested = PureDPBudget(INT_100 + FUDGE_FACTOR)
+    adjusted = get_adjusted_budget(requested, PURE_DP_100)
+    assert adjusted == PURE_DP_100
+
     # Up to the threshold, we should still round down.
-    requested = REMAINING_INT + (REMAINING_INT * fudge_factor)
-    adjusted = get_adjusted_budget(requested, REMAINING_EXACT)
-    assert adjusted == REMAINING_EXACT
+    requested = PureDPBudget(INT_100 + (INT_100 * FUDGE_FACTOR))
+    adjusted = get_adjusted_budget(requested, PURE_DP_100)
+    assert adjusted == PURE_DP_100
+
     # But past the threshold, we assume this is not a rounding error, and we let
     # the requested budget proceed deeper into the system (to ultimately be caught
     # and inform the user they requested too much).
-    requested = REMAINING_INT + (REMAINING_INT * fudge_factor * 2)
-    adjusted = get_adjusted_budget(requested, REMAINING_EXACT)
-    assert adjusted == ExactNumber.from_float(requested, False)
+    requested = PureDPBudget(INT_100 + (INT_100 * FUDGE_FACTOR * 2))
+    adjusted = get_adjusted_budget(requested, PURE_DP_100)
+    assert adjusted == requested
 
 
 """Tests that our 'slightly higher' check works as intended."""
 
 
 def test_requested_budget_much_higher():
     """Make sure a requested budget that is much higher than remaining fails.
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_protected_change.py` & `tmlt_analytics-0.7.1/test/unit/test_protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_query_builder.py` & `tmlt_analytics-0.7.1/test/unit/test_query_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,33 @@
     Rename,
     ReplaceInfinity,
     ReplaceNullAndNan,
     Select,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
-from ..conftest import assert_frame_equal_with_sort  # pylint: disable=no-name-in-module
+from ..conftest import assert_frame_equal_with_sort
 
 PRIVATE_ID = "private"
 
 Row = Dict[str, Any]
 
 
 ###DEFINE ROOT BUILDER###
 def root_builder():
     """Set up QueryBuilder."""
     root_built = QueryBuilder(PRIVATE_ID)
     return root_built
 
 
+# pylint throws a lot of spurious no-member errors in this file,
+# because QueryBuilders return a QueryExpr, which doesn't have a .child and so on
+# pylint: disable=no-member
+
+
 @pytest.mark.parametrize("join_columns", [(None), (["B"])])
 def test_join_public(join_columns: Optional[List[str]]):
     """QueryBuilder.join_public works as expected with a public source ID."""
 
     join_table = "public"
     query = (
         root_builder()
@@ -257,19 +262,15 @@
         )
 
 
 def test_map_augment_is_false():
     """QueryBuilder map works as expected with augment=False."""
 
     def double_row(_: Row) -> Row:
-        """Return row with doubled value
-
-        Args:
-            _: Row to apply function to.
-        """
+        """Return row with doubled value."""
         return {"C": 2 * "B"}
 
     query = (
         root_builder()
         .map(double_row, new_column_types={"C": "VARCHAR"}, augment=False)
         .groupby(KeySet.from_dict({"C": ["0", "1"]}))
         .count()
@@ -289,19 +290,15 @@
     assert root_expr.source_id == PRIVATE_ID
 
 
 def test_map_augment_is_true():
     """QueryBuilder map works as expected with augment=True."""
 
     def double_row(_: Row) -> Row:
-        """Return row with doubled value
-
-        Args:
-            _: Row to apply function to.
-        """
+        """Return row with doubled value."""
         return {"C": 2 * "B"}
 
     query = (
         root_builder()
         .map(double_row, new_column_types={"C": "VARCHAR"}, augment=True)
         .groupby(KeySet.from_dict({"A": ["0", "1"], "C": ["0", "1"]}))
         .count()
@@ -374,19 +371,15 @@
         )
 
 
 def test_flat_map_augment_is_false():
     """QueryBuilder flat_map works as expected with augment=False."""
 
     def duplicate_rows(_: Row) -> List[Row]:
-        """Duplicate each row, with one copy having C=0, and the other C=1.
-
-        Args:
-            _: Row to apply function to.
-        """
+        """Duplicate each row, with one copy having C=0, and the other C=1."""
         return [{"C": "0"}, {"C": "1"}]
 
     query = (
         root_builder()
         .flat_map(
             duplicate_rows,
             new_column_types={"C": "VARCHAR"},
@@ -418,19 +411,15 @@
     assert root_expr.source_id == PRIVATE_ID
 
 
 def test_flat_map_augment_is_true():
     """QueryBuilder flat_map works as expected with augment=True."""
 
     def duplicate_rows(_: Row) -> List[Row]:
-        """Duplicate each row, with one copy having C=0, and the other C=1.
-
-        Args:
-            _: Row to apply function to.
-        """
+        """Duplicate each row, with one copy having C=0, and the other C=1."""
         return [{"C": "0"}, {"C": "1"}]
 
     query = (
         root_builder()
         .flat_map(
             duplicate_rows,
             new_column_types={"C": "VARCHAR"},
@@ -505,15 +494,15 @@
     query = root_builder().bin_column("A", spec).count()
     assert isinstance(query, GroupByCount)
     map_expr = query.child
     assert isinstance(map_expr, Map)
     assert map_expr.schema_new_columns == Schema(
         {
             "A_binned": ColumnDescriptor(
-                ColumnType.VARCHAR, allow_null=True, allow_nan=True, allow_inf=True
+                ColumnType.VARCHAR, allow_null=True, allow_nan=False, allow_inf=False
             )
         }
     )
     assert map_expr.augment
     root_expr = map_expr.child
     assert isinstance(root_expr, PrivateSource)
     assert root_expr.source_id == PRIVATE_ID
@@ -530,15 +519,15 @@
     query = root_builder().bin_column("A", spec, name="rounded").count()
     assert isinstance(query, GroupByCount)
     map_expr = query.child
     assert isinstance(map_expr, Map)
     assert map_expr.schema_new_columns == Schema(
         {
             "rounded": ColumnDescriptor(
-                ColumnType.INTEGER, allow_null=True, allow_nan=True, allow_inf=True
+                ColumnType.INTEGER, allow_null=True, allow_nan=False, allow_inf=False
             )
         }
     )
     assert map_expr.augment
     root_expr = map_expr.child
     assert isinstance(root_expr, PrivateSource)
     assert root_expr.source_id == PRIVATE_ID
@@ -556,15 +545,15 @@
     assert isinstance(query, GroupByCount)
     map_expr = query.child
     assert isinstance(map_expr, Map)
 
     assert map_expr.schema_new_columns == Schema(
         {
             "A_binned": ColumnDescriptor(
-                ColumnType.VARCHAR, allow_null=True, allow_nan=True, allow_inf=True
+                ColumnType.VARCHAR, allow_null=True, allow_nan=False, allow_inf=False
             )
         }
     )
 
     assert map_expr.augment
     root_expr = map_expr.child
     assert isinstance(root_expr, PrivateSource)
@@ -582,15 +571,15 @@
     assert isinstance(query, GroupByCount)
     map_expr = query.child
     assert isinstance(map_expr, Map)
 
     assert map_expr.schema_new_columns == Schema(
         {
             "New": ColumnDescriptor(
-                ColumnType.VARCHAR, allow_null=True, allow_nan=True, allow_inf=True
+                ColumnType.VARCHAR, allow_null=True, allow_nan=False, allow_inf=False
             )
         }
     )
 
     assert map_expr.augment
     root_expr = map_expr.child
     assert isinstance(root_expr, PrivateSource)
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.7.1/test/unit/test_query_expr_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests for QueryExprCompiler."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-member, protected-access, no-self-use
+# pylint: disable=protected-access, no-self-use
 
 import datetime
 from typing import Dict, List, Union
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
@@ -19,26 +19,37 @@
     DoubleType,
     LongType,
     StringType,
     StructField,
     StructType,
     TimestampType,
 )
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import (
+    SparkDataFrameDomain,
+    SparkFloatColumnDescriptor,
+    SparkIntegerColumnDescriptor,
+    SparkStringColumnDescriptor,
+)
+from tmlt.core.measurements.aggregations import NoiseMechanism
+from tmlt.core.measures import PureDP, RhoZCDP
+from tmlt.core.metrics import DictMetric, SymmetricDifference
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler import QueryExprCompiler
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
 )
 from tmlt.analytics._table_identifier import Identifier, NamedTable
 from tmlt.analytics._transformation_utils import get_table_from_ref
 from tmlt.analytics.keyset import KeySet
+from tmlt.analytics.privacy_budget import PureDPBudget, RhoZCDPBudget
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountMechanism,
     Filter,
     FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
@@ -56,24 +67,14 @@
     ReplaceNullAndNan,
     Select,
     StdevMechanism,
     SumMechanism,
     VarianceMechanism,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import (
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-    SparkIntegerColumnDescriptor,
-    SparkStringColumnDescriptor,
-)
-from tmlt.core.measurements.aggregations import NoiseMechanism
-from tmlt.core.measures import PureDP, RhoZCDP
-from tmlt.core.metrics import DictMetric, SymmetricDifference
 
 from ..conftest import assert_frame_equal_with_sort, create_mock_measurement
 
 GROUPBY_TWO_COLUMNS = pd.DataFrame([["0", 0], ["0", 1], ["1", 1]], columns=["A", "B"])
 GROUPBY_TWO_SCHEMA = StructType(
     [StructField("A", StringType(), False), StructField("B", LongType(), False)]
 )
@@ -121,25 +122,23 @@
             )
         ],
     ),
     (  # Incomplete two-column marginal with a dataframe
         [
             GroupByCount(
                 child=PrivateSource("private"),
-                # pylint: disable=protected-access
                 groupby_keys=KeySet(dataframe=GET_GROUPBY_TWO),
             )
         ],
         [pd.DataFrame({"A": ["0", "0", "1"], "B": [0, 1, 1], "count": [2, 1, 0]})],
     ),
     (  # One-column marginal with additional value
         [
             GroupByCount(
                 child=PrivateSource("private"),
-                # pylint: disable=protected-access
                 groupby_keys=KeySet(dataframe=GET_GROUPBY_ONE),
             )
         ],
         [pd.DataFrame({"A": ["0", "1", "2"], "count": [3, 1, 0]})],
     ),
     (  # BoundedAverage
         [
@@ -187,29 +186,31 @@
                 low=0.0,
                 high=1.0,
                 output_column="sum",
             )
         ],
         [pd.DataFrame({"A": ["0", "1"], "sum": [2.0, 1.0]})],
     ),
-    (  # Marginal over A, Marginal over B
+    (  # Marginal over A
         [
             GroupByCount(
                 child=PrivateSource("private"),
                 groupby_keys=KeySet.from_dict({"A": ["0", "1"]}),
-            ),
+            )
+        ],
+        [pd.DataFrame({"A": ["0", "1"], "count": [3, 1]})],
+    ),
+    (  # Marginal over B
+        [
             GroupByCount(
                 child=PrivateSource("private"),
                 groupby_keys=KeySet.from_dict({"B": [0, 1]}),
-            ),
-        ],
-        [
-            pd.DataFrame({"A": ["0", "1"], "count": [3, 1]}),
-            pd.DataFrame({"B": [0, 1], "count": [3, 1]}),
+            )
         ],
+        [pd.DataFrame({"B": [0, 1], "count": [3, 1]})],
     ),
     (  # FlatMap
         [
             GroupByBoundedSum(
                 child=ReplaceNullAndNan(
                     replace_with={},
                     child=FlatMap(
@@ -664,23 +665,21 @@
                     columns_to_count=["B"],
                 ),
                 pd.DataFrame([["0", 2], ["1", 1]], columns=["A", "count_distinct"]),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
-                    # pylint: disable=protected-access
                     groupby_keys=KeySet(dataframe=GET_GROUPBY_ONE),
                 ),
                 pd.DataFrame({"A": ["0", "1", "2"], "count_distinct": [3, 1, 0]}),
             ),
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
-                    # pylint: disable=protected-access
                     groupby_keys=KeySet(dataframe=GET_GROUPBY_ONE),
                     columns_to_count=["B"],
                 ),
                 pd.DataFrame({"A": ["0", "1", "2"], "count_distinct": [2, 1, 0]}),
             ),
         ],
     )
@@ -696,15 +695,15 @@
                     ["1", 0, 3.0],
                 ],
                 columns=["A", "B", "X"],
             )
         )
         measurement = self.compiler(
             [query_expr],
-            privacy_budget=sp.oo,
+            privacy_budget=PureDPBudget(float("inf")),
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={
                 "public": self.join_df,
                 "groupby_two_columns": self.groupby_two_columns_df,
                 "groupby_one_column": self.groupby_one_column_df,
@@ -722,15 +721,15 @@
 
         Args:
             query_exprs: The queries to evaluate.
             expected: The expected answers.
         """
         measurement = self.compiler(
             query_exprs,
-            privacy_budget=sp.oo,
+            privacy_budget=PureDPBudget(float("inf")),
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={
                 "public": self.join_df,
                 "dtypes": self.dtypes_df,
                 "groupby_two_columns": self.groupby_two_columns_df,
@@ -954,17 +953,22 @@
         self,
         query: QueryExpr,
         output_measure: Union[PureDP, RhoZCDP],
         expected: List[pd.DataFrame],
     ):
         """Tests aggregation with various privacy definition and mechanism."""
         compiler = QueryExprCompiler(output_measure=output_measure)
+        privacy_budget = (
+            PureDPBudget(float("inf"))
+            if isinstance(output_measure, PureDP)
+            else RhoZCDPBudget(float("inf"))
+        )
         measurement = compiler(
             [query],
-            privacy_budget=sp.oo,
+            privacy_budget=privacy_budget,
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={"public": self.join_df},
             catalog=self.catalog,
             table_constraints={t: [] for t in self.stability.keys()},
         )
@@ -1069,15 +1073,15 @@
             match=(
                 "(GAUSSIAN)|(Discrete gaussian) noise is not yet compatible with"
                 " floating-point values."
             ),
         ):
             compiler(
                 query_exprs,
-                privacy_budget=sp.oo,
+                privacy_budget=RhoZCDPBudget(float("inf")),
                 stability=self.stability,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={"public": self.join_df},
                 catalog=self.catalog,
                 table_constraints={t: [] for t in self.stability.keys()},
             )
@@ -1115,15 +1119,15 @@
                 ],
                 columns=["A", "B", "X", "Y"],
             ),
         )
 
     def test_join_private(self, spark):
         """Tests that join private works."""
-        sdf_2 = spark.createDataFrame(  # pylint: disable=no-member
+        sdf_2 = spark.createDataFrame(
             pd.DataFrame(
                 [["0", 0], ["0", 2], ["1", 2], ["0", 0], ["1", 4]], columns=["A", "C"]
             )
         )
         transformation, reference, _constraints = self.compiler.build_transformation(
             JoinPrivate(
                 child=PrivateSource("private"),
@@ -1315,15 +1319,15 @@
                 high=1.0,
                 output_column="sum",
                 mechanism=SumMechanism.LAPLACE,
             )
         ]
         measurement = QueryExprCompiler()(
             query_exprs,
-            privacy_budget=sp.oo,
+            privacy_budget=PureDPBudget(float("inf")),
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
             table_constraints={t: [] for t in self.stability.keys()},
         )
@@ -1366,41 +1370,55 @@
         ],
     )
     def test_invalid_queries(self, query_exprs: List[QueryExpr]):
         """QueryExprCompiler raises error on unsupported queries."""
         with pytest.raises(NotImplementedError):
             self.compiler(
                 query_exprs,
-                privacy_budget=sp.oo,
+                privacy_budget=PureDPBudget(float("inf")),
                 stability=self.stability,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={"public": self.join_df},
                 catalog=self.catalog,
                 table_constraints={t: [] for t in self.stability.keys()},
             )
 
-    def test_different_source_id(self):
-        """Tests that different source ids are allowed."""
-        self.catalog.add_private_table(
-            source_id="doubled",
-            col_types={
-                "A": ColumnType.VARCHAR,
-                "B": ColumnType.INTEGER,
-                "X": ColumnType.DECIMAL,
-            },
-        )
-        query_exprs = [
-            GroupByCount(
-                child=PrivateSource("private"), groupby_keys=KeySet.from_dict({})
+    @pytest.mark.parametrize(
+        "query_exprs",
+        [
+            (
+                [
+                    GroupByCount(
+                        child=PrivateSource("private"),
+                        groupby_keys=KeySet.from_dict({}),
+                    )
+                ]
             ),
-            GroupByCount(
-                child=PrivateSource("doubled"), groupby_keys=KeySet.from_dict({})
+            (
+                [
+                    GroupByCount(
+                        child=PrivateSource("doubled"),
+                        groupby_keys=KeySet.from_dict({}),
+                    )
+                ]
             ),
-        ]
+        ],
+    )
+    def test_different_source_id(self, query_exprs: List[QueryExpr]):
+        """Tests that different source ids are allowed."""
+        if not self.catalog.tables.get("doubled"):
+            self.catalog.add_private_table(
+                source_id="doubled",
+                col_types={
+                    "A": ColumnType.VARCHAR,
+                    "B": ColumnType.INTEGER,
+                    "X": ColumnType.DECIMAL,
+                },
+            )
         stability = {
             NamedTable("doubled"): self.stability[NamedTable("private")] * 2,
             **self.stability,
         }
         input_domain = DictDomain(
             {
                 NamedTable("doubled"): self.input_domain[NamedTable("private")],
@@ -1412,15 +1430,15 @@
                 NamedTable("doubled"): self.input_metric[NamedTable("private")],
                 **self.input_metric.key_to_metric,
             }
         )
 
         measurement = self.compiler(
             query_exprs,
-            privacy_budget=sp.Integer(10),
+            privacy_budget=PureDPBudget(10),
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             public_sources={"public": self.join_df},
             catalog=self.catalog,
             table_constraints={t: [] for t in stability.keys()},
         )
@@ -1429,15 +1447,15 @@
     def test_call_no_queries(self):
         """``__call__`` raises error if the sequence of queries has length 0."""
         with pytest.raises(
             ValueError, match=r"At least one query needs to be provided"
         ):
             self.compiler(
                 queries=[],
-                privacy_budget=sp.Integer(10),
+                privacy_budget=PureDPBudget(10),
                 stability=self.stability,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={"public": self.join_df},
                 catalog=self.catalog,
                 table_constraints={t: [] for t in self.stability.keys()},
             )
@@ -1488,50 +1506,55 @@
                         "Age": SparkIntegerColumnDescriptor(),
                     }
                 )
             }
         )
         input_metric = DictMetric({NamedTable("private"): SymmetricDifference()})
         compiler = QueryExprCompiler(output_measure=output_measure)
+        privacy_budget = (
+            PureDPBudget(1000)
+            if isinstance(output_measure, PureDP)
+            else RhoZCDPBudget(1000)
+        )
 
         query_expr = GroupByQuantile(
             child=PrivateSource("private"),
             groupby_keys=KeySet.from_dict({"Gender": ["M", "F"]}),
             measure_column="Age",
             quantile=0.5,
             low=22,
             high=29,
             output_column="out",
         )
         measurement = compiler(
             [query_expr],
-            privacy_budget=sp.Integer(1000),
+            privacy_budget=privacy_budget,
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             public_sources={},
             catalog=catalog,
             table_constraints={t: [] for t in stability},
         )
         assert measurement.input_domain == input_domain
         assert measurement.input_metric == input_metric
         assert measurement.output_measure == output_measure
-        assert measurement.privacy_function(stability) == sp.Integer(1000)
+        assert measurement.privacy_function(stability) == privacy_budget.value
 
         [actual] = measurement({NamedTable("private"): sdf})
 
         assert 26 < actual.filter(col("Gender") == "F").collect()[0]["out"] <= 28
         assert 22 < actual.filter(col("Gender") == "M").collect()[0]["out"] <= 24
 
 
 @pytest.fixture(name="test_component_data", scope="class")
 def setup_components(request):
     """Set up test."""
     request.cls._stability = {NamedTable("test"): sp.Integer(3)}
-    request.cls._privacy_budget = sp.Integer(5)
+    request.cls._privacy_budget = PureDPBudget(5)
     request.cls._input_domain = DictDomain(
         {
             NamedTable("test"): SparkDataFrameDomain(
                 analytics_to_spark_columns_descriptor(
                     Schema({"A": "VARCHAR", "X": "INTEGER"})
                 )
             )
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_query_expression.py` & `tmlt_analytics-0.7.1/test/unit/test_query_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,18 @@
             1.0,
             "type of augment must be bool; got float instead",
         ),
         (  # Invalid Schema
             lambda row: {"C": 2 * str(row["B"])},
             {"C": "VARCHAR"},
             True,
-            "type of schema_new_columns must be "
-            "tmlt.analytics._schema.Schema; got dict instead",
+            (
+                "type of schema_new_columns must be "
+                "tmlt.analytics._schema.Schema; got dict instead"
+            ),
         ),
         (  # Grouping column in schema
             lambda row: {"C": 2 * str(row["B"])},
             Schema({"C": "VARCHAR"}, grouping_column="C"),
             True,
             "Map cannot be be used to create grouping columns",
         ),
@@ -169,16 +171,18 @@
         ),
         (  # Invalid grouping result
             PrivateSource("private"),
             lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
             2,
             Schema({"i": "INTEGER", "j": "INTEGER"}, grouping_column="i"),
             False,
-            "schema_new_columns contains 2 columns, "
-            "grouping flat map can only result in 1 new column",
+            (
+                "schema_new_columns contains 2 columns, "
+                "grouping flat map can only result in 1 new column"
+            ),
         ),
     ],
 )
 def test_invalid_flatmap(
     child: QueryExpr,
     func: Callable,
     max_num_rows: int,
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.7.1/test/unit/test_query_expression_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Tests for QueryExprVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
-# pylint: disable=no-self-use
 
 import pytest
 
 from tmlt.analytics._schema import Schema
 from tmlt.analytics.constraints import MaxRowsPerID
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_schema.py` & `tmlt_analytics-0.7.1/test/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.7.1/test/unit/test_schema_conversion.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 # pylint: disable=no-self-use
 import datetime
 
 import pytest
 from pyspark.sql import types as spark_types
+from tmlt.core.domains.spark_domains import (
+    SparkColumnsDescriptor,
+    SparkDataFrameDomain,
+    SparkDateColumnDescriptor,
+    SparkFloatColumnDescriptor,
+    SparkIntegerColumnDescriptor,
+    SparkStringColumnDescriptor,
+    SparkTimestampColumnDescriptor,
+)
 
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_py_types,
     analytics_to_spark_columns_descriptor,
     analytics_to_spark_schema,
     spark_dataframe_domain_to_analytics_columns,
     spark_schema_to_analytics_columns,
 )
-from tmlt.core.domains.spark_domains import (
-    SparkColumnsDescriptor,
-    SparkDataFrameDomain,
-    SparkDateColumnDescriptor,
-    SparkFloatColumnDescriptor,
-    SparkIntegerColumnDescriptor,
-    SparkStringColumnDescriptor,
-    SparkTimestampColumnDescriptor,
-)
 
 
 class TestSchemaConversions:
     """Unit tests for schema conversions."""
 
     def test_analytics_to_py_types(self) -> None:
         """Make sure SQL92 types are mapped to the right python types."""
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_session.py` & `tmlt_analytics-0.7.1/test/unit/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Unit tests for Session."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-# pylint: disable=no-self-use, unidiomatic-typecheck, no-member
+# pylint: disable=no-self-use, unidiomatic-typecheck
 
 import re
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 from unittest.mock import ANY, Mock, patch
 
 import pandas as pd
 import pytest
@@ -19,14 +19,41 @@
     FloatType,
     IntegerType,
     LongType,
     StringType,
     StructField,
     StructType,
 )
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import (
+    SparkDataFrameDomain,
+    SparkIntegerColumnDescriptor,
+    SparkStringColumnDescriptor,
+)
+from tmlt.core.measurements.base import Measurement
+from tmlt.core.measurements.interactive_measurements import (
+    PrivacyAccountant,
+    PrivacyAccountantState,
+    SequentialComposition,
+    SequentialQueryable,
+)
+from tmlt.core.measures import ApproxDP, Measure, PureDP, RhoZCDP
+from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
+from tmlt.core.metrics import (
+    DictMetric,
+    IfGroupedBy,
+    Metric,
+    RootSumOfSquared,
+    SumOf,
+    SymmetricDifference,
+)
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.chaining import ChainTT
+from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
+from tmlt.core.utils.exact_number import ExactNumber
 from typeguard import check_type
 
 from tmlt.analytics._neighboring_relation import (
     AddRemoveKeys,
     AddRemoveRows,
     AddRemoveRowsAcrossGroups,
     Conjunction,
@@ -54,56 +81,24 @@
     AddMaxRowsInMaxGroups,
     AddOneRow,
     AddRowsWithID,
 )
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import PrivateSource, QueryExpr
 from tmlt.analytics.session import Session
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import (
-    SparkDataFrameDomain,
-    SparkIntegerColumnDescriptor,
-    SparkStringColumnDescriptor,
-)
-from tmlt.core.measurements.base import Measurement
-from tmlt.core.measurements.interactive_measurements import (
-    PrivacyAccountant,
-    PrivacyAccountantState,
-    SequentialComposition,
-    SequentialQueryable,
-)
-from tmlt.core.measures import Measure, PureDP, RhoZCDP
-from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
-from tmlt.core.metrics import (
-    DictMetric,
-    IfGroupedBy,
-    Metric,
-    RootSumOfSquared,
-    SumOf,
-    SymmetricDifference,
-)
-from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
-from tmlt.core.utils.exact_number import ExactNumber
 
-from ..conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
-    create_mock_transformation,
-)
+from ..conftest import assert_frame_equal_with_sort, create_mock_transformation
 
 
 def _privacy_budget_to_exact_number(
     budget: Union[PureDPBudget, RhoZCDPBudget]
 ) -> ExactNumber:
     """Turn a privacy budget into an Exact Number."""
-    if isinstance(budget, PureDPBudget):
-        return ExactNumber(budget.epsilon)
-    if isinstance(budget, RhoZCDPBudget):
-        return ExactNumber(budget.rho)
+    if isinstance(budget, (PureDPBudget, RhoZCDPBudget)):
+        return budget.value
     raise AssertionError("This should be unreachable")
 
 
 @pytest.fixture(name="test_data", scope="class")
 def setup_test_data(spark, request) -> None:
     """Set up test data."""
     sdf = spark.createDataFrame(
@@ -330,15 +325,15 @@
             assert_frame_equal_with_sort(
                 mock_composition_init.return_value.mock_calls[0][1][0][
                     NamedTable("private")
                 ].toPandas(),
                 self.sdf.toPandas(),
             )
             mock_session_init.assert_called_with(
-                self=ANY, accountant=ANY, public_sources=dict(), compiler=ANY
+                self=ANY, accountant=ANY, public_sources={}, compiler=ANY
             )
 
     @pytest.mark.parametrize(
         "budget,expected_output_measure,expected_metric,from_dataframe_args",
         [
             pytest.param(
                 PureDPBudget(float("inf")),
@@ -408,15 +403,15 @@
             assert_frame_equal_with_sort(
                 mock_composition_init.return_value.mock_calls[0][1][0][
                     TableCollection("default_id_space")
                 ][NamedTable("private")].toPandas(),
                 self.sdf.toPandas(),
             )
             mock_session_init.assert_called_with(
-                self=ANY, accountant=ANY, public_sources=dict(), compiler=ANY
+                self=ANY, accountant=ANY, public_sources={}, compiler=ANY
             )
 
     @pytest.mark.parametrize(
         "budget,relation,expected_metric,expected_output_measure",
         [
             pytest.param(
                 PureDPBudget(float("inf")),
@@ -593,17 +588,15 @@
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = self.sdf_input_domain
             mock_accountant.d_in = {NamedTable("private"): ExactNumber(1)}
             mock_compiler.output_measure = PureDP()
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
             session.add_public_dataframe(source_id="public", dataframe=self.join_df)
             assert "public" in session.public_source_dataframes
             assert_frame_equal_with_sort(
                 session.public_source_dataframes["public"].toPandas(),
                 self.join_df.toPandas(),
             )
@@ -655,15 +648,15 @@
                 stability_function_return_value=ExactNumber(13),
             )
             mock_compiler_transform.return_value = (
                 view_transformation,
                 TableReference(path=[NamedTable("private")]),
                 [],
             )
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             session.create_view(
                 query_expr=PrivateSource("private"),
                 source_id="identity_transformation",
                 cache=False,
             )
 
             mock_compiler_transform.assert_called_with(
@@ -684,58 +677,62 @@
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant_and_compiler(
                 spark, d_in, mock_accountant, mock_compiler
             )
             mock_accountant.privacy_budget = ExactNumber(10)
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             answer = session.evaluate(
                 query_expr=PrivateSource("private"), privacy_budget=PureDPBudget(10)
             )
             self._assert_test_evaluate_correctness(
-                session, mock_accountant, mock_compiler, 10
+                session, mock_accountant, mock_compiler, PureDPBudget(10)
             )
             check_type("answer", answer, DataFrame)
 
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_puredp_session_approxdp_query(self, spark, d_in):
-        """Tests that :func:`evaluate` calls the right things given a puredp session."""
+        """Confirm that using an approxdp query on a puredp accountant raises an
+        error."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant_and_compiler(
                 spark, d_in, mock_accountant, mock_compiler
             )
             mock_accountant.privacy_budget = ExactNumber(10)
-            session = Session(accountant=mock_accountant, public_sources=dict())
-            answer = session.evaluate(
-                query_expr=PrivateSource("private"),
-                privacy_budget=ApproxDPBudget(10, 0.5),
-            )
-            self._assert_test_evaluate_correctness(
-                session, mock_accountant, mock_compiler, 10
-            )
-            check_type("answer", answer, DataFrame)
+            session = Session(accountant=mock_accountant, public_sources={})
+            with pytest.raises(
+                ValueError,
+                match=(
+                    "Your requested privacy budget type must match the type of the"
+                    " privacy budget your Session was created with."
+                ),
+            ):
+                session.evaluate(
+                    query_expr=PrivateSource("private"),
+                    privacy_budget=ApproxDPBudget(10, 0.5),
+                )
 
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_with_zero_budget(self, spark, d_in):
         """Confirm that calling evaluate with a 'budget' of 0 fails."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant_and_compiler(
                 spark, d_in, mock_accountant, mock_compiler
             )
             mock_accountant.privacy_budget = ExactNumber(10)
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(
                 ValueError,
                 match="You need a non-zero privacy budget to evaluate a query.",
             ):
                 session.evaluate(
                     query_expr=PrivateSource("private"), privacy_budget=PureDPBudget(0)
                 )
@@ -762,15 +759,15 @@
             self._setup_accountant_and_compiler(
                 spark, d_in, mock_accountant, mock_compiler
             )
             mock_accountant.privacy_budget = ExactNumber(10)
             # Set the output measures manually
             mock_accountant.output_measure = RhoZCDP()
             mock_compiler.output_measure = RhoZCDP()
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(
                 ValueError,
                 match=(
                     "Your requested privacy budget type must match the type of the"
                     " privacy budget your Session was created with."
                 ),
             ):
@@ -786,15 +783,15 @@
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant_and_compiler(
                 spark, d_in, mock_accountant, mock_compiler
             )
             mock_accountant.privacy_budget = ExactNumber(10)
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(
                 ValueError,
                 match=(
                     "Your requested privacy budget type must match the type of the"
                     " privacy budget your Session was created with."
                 ),
             ):
@@ -814,20 +811,20 @@
             self._setup_accountant_and_compiler(
                 spark, d_in, mock_accountant, mock_compiler
             )
             mock_accountant.privacy_budget = ExactNumber(5)
             # Set the output measures manually
             mock_accountant.output_measure = RhoZCDP()
             mock_compiler.output_measure = RhoZCDP()
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             answer = session.evaluate(
                 query_expr=PrivateSource("private"), privacy_budget=RhoZCDPBudget(5)
             )
             self._assert_test_evaluate_correctness(
-                session, mock_accountant, mock_compiler, 5
+                session, mock_accountant, mock_compiler, RhoZCDPBudget(5)
             )
             check_type("answer", answer, DataFrame)
 
     def _setup_accountant(
         self, mock_accountant, d_in=None, privacy_budget=None
     ) -> None:
         """Initialize only a mock accountant."""
@@ -901,34 +898,34 @@
         mock_accountant.measure.return_value = [
             spark.createDataFrame(spark.sparkContext.emptyRDD(), StructType([]))
         ]
         mock_compiler.output_measure = PureDP()
         mock_compiler.return_value = Mock(spec_set=Measurement)
 
     def _assert_test_evaluate_correctness(
-        self, session, mock_accountant, mock_compiler, budget
+        self, session, mock_accountant, mock_compiler, privacy_budget
     ):
         """Confirm that :func:`evaluate` worked correctly."""
         assert "private" in session.private_sources
         assert session.get_schema("private") == self.sdf_col_types
 
         mock_compiler.assert_called_with(
             self=ANY,
             queries=[PrivateSource("private")],
             stability=mock_accountant.d_in,
             input_domain=mock_accountant.input_domain,
             input_metric=mock_accountant.input_metric,
-            privacy_budget=sp.Integer(budget),
+            privacy_budget=privacy_budget,
             public_sources={},
             catalog=ANY,
             table_constraints={t: [] for t in mock_accountant.d_in.keys()},
         )
 
         mock_accountant.measure.assert_called_with(
-            mock_compiler.return_value, d_out=ExactNumber(budget)
+            mock_compiler.return_value, d_out=privacy_budget.value
         )
 
     def test_partition_and_create(self):
         """Tests that :func:`partition_and_create` calls the right things."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
@@ -944,15 +941,15 @@
                     spec_set=PrivacyAccountant,
                     input_metric=DictMetric({"part1": SymmetricDifference()}),
                     input_domain=self.sdf_input_domain,
                     output_measure=PureDP(),
                 ),
             ]
 
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
 
         # Test that you need to provide splits
         with pytest.raises(
             ValueError,
             match=re.escape(
                 "You must provide a dictionary mapping split names (new source_ids) to"
                 " values on which to partition"
@@ -1229,15 +1226,15 @@
         ) as mock_accountant:
             self._setup_accountant(mock_accountant)
 
             def retire_side_effect():
                 mock_accountant.state = PrivacyAccountantState.RETIRED
 
             mock_accountant.retire.side_effect = retire_side_effect
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
 
             session.stop()
 
             with pytest.raises(
                 RuntimeError,
                 match=(
                     "This session is no longer active, and no new queries can be"
@@ -1342,17 +1339,15 @@
         ) as mock_accountant:
             with pytest.raises(
                 TypeError,
                 match=r"type of compiler must be one of "
                 r"\(QueryExprCompiler, NoneType\); got list instead",
             ):
                 self._setup_accountant(mock_accountant)
-                Session(
-                    mock_accountant, public_sources=dict(), compiler=[]  # type: ignore
-                )
+                Session(mock_accountant, public_sources={}, compiler=[])  # type: ignore
 
     def test_invalid_dataframe_initialization(self):
         """session raises error on invalid dataframe type"""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             # Private
@@ -1369,15 +1364,15 @@
                     source_id="private",
                     dataframe=self.pdf,
                     protected_change=AddOneRow(),
                 )
             # Public
             self._setup_accountant(mock_accountant)
 
-            session = Session(accountant=mock_accountant, public_sources=dict())
+            session = Session(accountant=mock_accountant, public_sources={})
             with pytest.raises(
                 TypeError,
                 match=(
                     'type of argument "dataframe" must be'
                     " pyspark.sql.dataframe.DataFrame; got pandas.core.frame.DataFrame"
                     " instead"
                 ),
@@ -1500,15 +1495,15 @@
                 "^Grouping column 'F' is not of a type on which grouping is supported.*"
             ),
         ):
             Session.from_dataframe(
                 PureDPBudget(1), "private", float_df, grouping_column="F"
             )
 
-    def test_invalid_key_column(self) -> None:  # pylint: disable=unused-argument
+    def test_invalid_key_column(self) -> None:
         """Builder raises an error if table's key column is not in dataframe."""
         with pytest.raises(
             ValueError,
             match=(
                 "^Key column 'not_a_column' does not exist in the input. Available"
                 " columns: A, B, X$"
             ),
@@ -1553,17 +1548,15 @@
                     privacy_budget=PureDPBudget(1),
                     source_id=source_id,
                     dataframe=self.sdf,
                     protected_change=AddOneRow(),
                 )
             # Public
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
             with pytest.raises(exception_type, match=expected_error_msg):
                 session.add_public_dataframe(source_id, dataframe=self.sdf)
             # create_view
             with pytest.raises(exception_type, match=expected_error_msg):
                 session.create_view(PrivateSource("private"), source_id, cache=False)
 
@@ -1581,17 +1574,15 @@
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             session = Session(
-                accountant=mock_accountant,
-                compiler=mock_compiler,
-                public_sources=dict(),
+                accountant=mock_accountant, compiler=mock_compiler, public_sources={}
             )
 
             # This should work
             session.add_public_dataframe("public_df", dataframe=self.sdf)
 
             # But this should not
             with pytest.raises(
@@ -1612,21 +1603,20 @@
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
+            mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
             with pytest.raises(
                 TypeError,
                 match=(
                     "type of query_expr must be tmlt.analytics.query_expr.QueryExpr;"
                     " got list instead"
                 ),
@@ -1659,21 +1649,20 @@
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
+            mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
             with pytest.raises(exception_type, match=expected_error_msg):
                 session.create_view(query_expr, source_id="view", cache=True)
 
     def test_invalid_column(self):
         """Tests that invalid column name for column errors."""
         with patch(
@@ -1684,30 +1673,29 @@
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
+            mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             mock_compiler.build_transformation.return_value = (
                 Mock(
                     spec_set=Transformation,
                     output_domain=self.sdf_input_domain,
                     output_metric=SymmetricDifference(),
                 ),
                 sp.Integer(1),
             )
 
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
 
             expected_schema = spark_schema_to_analytics_columns(self.sdf.schema)
             # We expect a transformation that will disallow NaNs on floats and infs
             expected_schema["X"].allow_nan = False
             expected_schema["X"].allow_inf = False
 
@@ -1736,30 +1724,29 @@
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
+            mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             mock_compiler.build_transformation.return_value = (
                 Mock(
                     spec_set=Transformation,
                     output_domain=self.sdf_input_domain,
                     output_metric=SymmetricDifference(),
                 ),
                 sp.Integer(1),
             )
 
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
 
             with pytest.raises(
                 ValueError,
                 match=(
                     "The string passed as split name must be a valid Python identifier"
                 ),
@@ -1781,30 +1768,29 @@
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
                 {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
                 {NamedTable("private"): self.sdf_input_domain}
             )
+            mock_accountant.privacy_budget = ExactNumber(1)
             mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             mock_compiler.build_transformation.return_value = (
                 Mock(
                     spec_set=Transformation,
                     output_domain=self.sdf_input_domain,
                     output_metric=SymmetricDifference(),
                 ),
                 sp.Integer(1),
             )
 
             session = Session(
-                accountant=mock_accountant,
-                public_sources=dict(),
-                compiler=mock_compiler,
+                accountant=mock_accountant, public_sources={}, compiler=mock_compiler
             )
 
             with pytest.raises(
                 TypeError,
                 match=(
                     r"'A' column is of type 'StringType\(?\)?'; 'StringType\(?\)?' "
                     "column not compatible with splits value type 'int'"
@@ -2050,16 +2036,16 @@
                 sp.Integer(10),
                 PureDP(),
                 [("df1", 1)],
                 [],
             ),
             (
                 Session.Builder().with_privacy_budget(ApproxDPBudget(10, 0.5)),
-                sp.Integer(10),
-                PureDP(),
+                (sp.Integer(10), 0),
+                ApproxDP(),
                 [("df1", 1)],
                 [],
             ),
             (
                 Session.Builder().with_privacy_budget(PureDPBudget(1.5)),
                 sp.Rational("1.5"),
                 PureDP(),
@@ -2088,16 +2074,16 @@
         expected_sympy_budget: sp.Expr,
         expected_output_measure: Measure,
         private_dataframes: List[Tuple[str, int]],
         public_dataframes: List[str],
     ):
         """Tests that building a Session works correctly."""
         # Set up the builder.
-        expected_private_sources, expected_public_sources = dict(), dict()
-        expected_stabilities = dict()
+        expected_private_sources, expected_public_sources = {}, {}
+        expected_stabilities = {}
         for source_id, stability in private_dataframes:
             builder = builder.with_private_dataframe(
                 source_id=source_id,
                 dataframe=self.dataframes[source_id],
                 protected_change=AddMaxRows(stability),
             )
             expected_private_sources[NamedTable(source_id)] = self.dataframes[source_id]
@@ -2110,27 +2096,23 @@
             expected_public_sources[source_id] = self.dataframes[source_id]
 
         # Build the session and verify that it worked.
         session = builder.build()
         # pylint: disable=protected-access
         accountant = session._accountant
         assert isinstance(accountant, PrivacyAccountant)
-        assert (
-            accountant.privacy_budget
-            == expected_sympy_budget
-            == accountant.privacy_budget
-        )
+        assert accountant.privacy_budget == expected_sympy_budget
         assert accountant.output_measure == expected_output_measure
 
-        for table_id in expected_private_sources:
+        for table_id, private_source in expected_private_sources.items():
             assert accountant._queryable is not None
             assert isinstance(accountant._queryable, SequentialQueryable)
             assert_frame_equal_with_sort(
                 accountant._queryable._data[table_id].toPandas(),
-                expected_private_sources[table_id].toPandas(),
+                private_source.toPandas(),
             )
 
         assert accountant.d_in == expected_stabilities
 
         public_sources = session._public_sources
         assert public_sources.keys() == expected_public_sources.keys()
         for key in public_sources:
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_table_identifiers.py` & `tmlt_analytics-0.7.1/test/unit/test_table_identifiers.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_transformation_utils.py` & `tmlt_analytics-0.7.1/test/unit/test_transformation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Unit tests for transofrmation utils."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
-from tmlt.analytics._table_identifier import NamedTable
-from tmlt.analytics._table_reference import TableReference
-from tmlt.analytics._transformation_utils import (
-    delete_table,
-    persist_table,
-    rename_table,
-    unpersist_table,
-)
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.metrics import DictMetric, SymmetricDifference
 from tmlt.core.transformations.identity import Identity as IdentityTransformation
 
+from tmlt.analytics._table_identifier import NamedTable
+from tmlt.analytics._table_reference import TableReference
+from tmlt.analytics._transformation_utils import (
+    delete_table,
+    persist_table,
+    rename_table,
+    unpersist_table,
+)
+
 
 def test_rename_table():
     """Test rename table."""
     sdf_input_dict_domain = DictDomain(
         {
             NamedTable("private"): SparkDataFrameDomain(
                 {
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.7.1/test/unit/test_truncation_strategy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Tests for TruncationStrategy."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
-# pylint: disable=pointless-string-statement
 
 import pytest
 
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
 
 @pytest.mark.parametrize("threshold", [(1), (8)])
```

### Comparing `tmlt_analytics-0.7.0rc1/test/unit/test_utils.py` & `tmlt_analytics-0.7.1/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_catalog.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_coerce_spark_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module containing supported variants of neighboring relations."""
-# pylint: disable=useless-super-delegation, protected-access, no-self-use
+# pylint: disable=protected-access, no-self-use
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql.types import DateType, IntegerType, LongType, StringType
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 from typing import Any, Dict, NamedTuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
-
-from tmlt.analytics._neighboring_relation import (
-    AddRemoveKeys,
-    AddRemoveRows,
-    AddRemoveRowsAcrossGroups,
-    Conjunction,
-    NeighboringRelationVisitor,
-)
-from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
 from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
 from tmlt.core.metrics import (
     DictMetric,
@@ -27,14 +18,23 @@
     Metric,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.utils.exact_number import ExactNumber
 
+from tmlt.analytics._neighboring_relation import (
+    AddRemoveKeys,
+    AddRemoveRows,
+    AddRemoveRowsAcrossGroups,
+    Conjunction,
+    NeighboringRelationVisitor,
+)
+from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
+
 
 class _RelationIDVisitor(NeighboringRelationVisitor):
     """Generate identifiers for neighboring relations."""
 
     def visit_add_remove_rows(self, relation: AddRemoveRows) -> Identifier:
         return NamedTable(relation.table)
 
@@ -70,15 +70,17 @@
 
         domain: Domain
         metric: Metric
         distance: Any
         data: Any
 
     def __init__(
-        self, tables: Dict[str, DataFrame], output_measure: Union[PureDP, RhoZCDP]
+        self,
+        tables: Dict[str, DataFrame],
+        output_measure: Union[PureDP, ApproxDP, RhoZCDP],
     ):
         """Constructor."""
         self.tables = tables
         self.output_measure = output_measure
 
     def visit_add_remove_rows(self, relation: AddRemoveRows) -> Output:
         """Build Core state from ``AddRemoveRows`` neighboring relation."""
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_noise_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from copy import deepcopy
 from enum import Enum
 from functools import singledispatch
 from typing import Any, Dict, List, Set, Tuple, Union
 
 from pyspark.sql import DataFrame
-
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.noise_mechanisms import (
     AddDiscreteGaussianNoise,
     AddGeometricNoise,
     AddLaplaceNoise,
 )
 from tmlt.core.measurements.pandas_measurements.series import NoisyQuantile
@@ -22,28 +21,27 @@
     LAPLACE = 1
     GEOMETRIC = 2
     DISCRETE_GAUSSIAN = 3
     EXPONENTIAL = 4
 
     def to_cls(self):
         """Returns the appropriate measurement class for this enum value."""
-        # pylint: disable=comparison-with-callable
         if self.value == _NoiseMechanism.LAPLACE.value:
             return AddLaplaceNoise
         if self.value == _NoiseMechanism.GEOMETRIC.value:
             return AddGeometricNoise
         if self.value == _NoiseMechanism.DISCRETE_GAUSSIAN.value:
             return AddDiscreteGaussianNoise
         if self.value == _NoiseMechanism.EXPONENTIAL.value:
             return NoisyQuantile
         raise KeyError("Unknown measurement type.")
 
 
 @singledispatch
-def _get_info(a: Any) -> Any:  # pylint: disable=unused-argument
+def _get_info(a: Any) -> Any:
     """Get information from a measurement or transformation.
 
     Output will look a lot like input's __dict__, except that:
     - Measurements become dictionaries (via _get_info)
     - Transformations become dictionaries (via _get_info)
     - ExactNumbers become floats (via .to_float(round_up=False))
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-"""Defines :class:`QueryExprCompiler` for compiling query expressions into a measurement.
-"""  # pylint: disable=line-too-long
+"""Defines :class:`QueryExprCompiler` for building transformations from query exprs."""
 # TODO(#746): Check for UnaryExpr.
 # TODO(#1044): Put the PureDPToZCDP converter directly on Vector measurements.
 # TODO(#1547): Associate metric with output measure instead of algorithm for
 #              adding noise.
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 from typing import Any, Dict, List, Sequence, Tuple, Union
 
-import sympy as sp
 from pyspark.sql import DataFrame
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.measurements.aggregations import NoiseMechanism as CoreNoiseMechanism
+from tmlt.core.measurements.base import Measurement
+from tmlt.core.measurements.composition import Composition
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.metrics import DictMetric
+from tmlt.core.transformations.base import Transformation
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._measurement_visitor import MeasurementVisitor
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
 )
 from tmlt.analytics._schema import Schema
 from tmlt.analytics._table_identifier import Identifier
 from tmlt.analytics._table_reference import TableReference
 from tmlt.analytics.constraints import Constraint
+from tmlt.analytics.privacy_budget import PrivacyBudget
 from tmlt.analytics.query_expr import QueryExpr
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.measurements.aggregations import NoiseMechanism as CoreNoiseMechanism
-from tmlt.core.measurements.base import Measurement
-from tmlt.core.measurements.composition import Composition
-from tmlt.core.measures import PureDP, RhoZCDP
-from tmlt.core.metrics import DictMetric
-from tmlt.core.transformations.base import Transformation
 
 DEFAULT_MECHANISM = "DEFAULT"
 """Constant used for DEFAULT noise mechanism"""
 
 LAPLACE_MECHANISM = "LAPLACE"
 """Constant used for LAPLACE noise mechanism"""
 
@@ -72,24 +71,24 @@
     * :class:`~tmlt.analytics.query_expr.GroupByBoundedSum`
     * :class:`~tmlt.analytics.query_expr.GroupByBoundedAverage`
     * :class:`~tmlt.analytics.query_expr.GroupByBoundedSTDEV`
     * :class:`~tmlt.analytics.query_expr.GroupByBoundedVariance`
     * :class:`~tmlt.analytics.query_expr.GroupByQuantile`
     """
 
-    def __init__(self, output_measure: Union[PureDP, RhoZCDP] = PureDP()):
+    def __init__(self, output_measure: Union[PureDP, ApproxDP, RhoZCDP] = PureDP()):
         """Constructor.
 
         Args:
             output_measure: Distance measure for measurement's output.
         """
         # TODO(#1547): Can be removed when issue is resolved.
         self._mechanism = (
             CoreNoiseMechanism.LAPLACE
-            if isinstance(output_measure, PureDP)
+            if isinstance(output_measure, (PureDP, ApproxDP))
             else CoreNoiseMechanism.DISCRETE_GAUSSIAN
         )
         self._output_measure = output_measure
 
     @property
     def mechanism(self) -> CoreNoiseMechanism:
         """Return the value of Core noise mechanism."""
@@ -97,15 +96,15 @@
 
     @mechanism.setter
     def mechanism(self, value):
         """Set the value of Core noise mechanism."""
         self._mechanism = value
 
     @property
-    def output_measure(self) -> Union[PureDP, RhoZCDP]:
+    def output_measure(self) -> Union[PureDP, ApproxDP, RhoZCDP]:
         """Return the distance measure for the measurement's output."""
         return self._output_measure
 
     @staticmethod
     def query_schema(query: QueryExpr, catalog: Catalog) -> Schema:
         """Return the schema created by a given query."""
         result = query.accept(OutputSchemaVisitor(catalog=catalog))
@@ -116,15 +115,15 @@
         return result
 
     # pylint: enable=no-self-use
 
     def __call__(
         self,
         queries: Sequence[QueryExpr],
-        privacy_budget: sp.Expr,
+        privacy_budget: PrivacyBudget,
         stability: Any,
         input_domain: DictDomain,
         input_metric: DictMetric,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
         table_constraints: Dict[Identifier, List[Constraint]],
     ) -> Measurement:
@@ -139,47 +138,45 @@
             public_sources: Public data sources for the queries.
             catalog: The catalog, used only for query validation.
             table_constraints: A mapping of tables to the existing constraints on them.
         """
         if len(queries) == 0:
             raise ValueError("At least one query needs to be provided")
 
-        measurements: List[Measurement] = []
-        per_query_privacy_budget = privacy_budget / len(queries)
+        if len(queries) != 1:
+            raise NotImplementedError("Only one query is supported at this time.")
         visitor = MeasurementVisitor(
-            per_query_privacy_budget=per_query_privacy_budget,
+            privacy_budget=privacy_budget,
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             output_measure=self._output_measure,
             default_mechanism=self._mechanism,
             public_sources=public_sources,
             catalog=catalog,
             table_constraints=table_constraints,
         )
+        measurements: List[Measurement] = []
         for query in queries:
             query_measurement = query.accept(visitor)
             if not isinstance(query_measurement, Measurement):
                 raise AssertionError(
                     "This query did not create a measurement. "
                     "This is probably a bug; please let us know so we can fix it!"
                 )
-            if (
-                query_measurement.privacy_function(stability)
-                != per_query_privacy_budget
-            ):
+            if query_measurement.privacy_function(stability) != privacy_budget.value:
                 raise AssertionError(
                     "Query measurement privacy function does not match "
-                    "per-query privacy budget. This is probably a bug; "
+                    "privacy budget value. This is probably a bug; "
                     "please let us know so we can fix it!"
                 )
             measurements.append(query_measurement)
 
         measurement = Composition(measurements)
-        if measurement.privacy_function(stability) != privacy_budget:
+        if measurement.privacy_function(stability) != privacy_budget.value:
             raise AssertionError(
                 "Measurement privacy function does not match "
                 "privacy budget. This is probably a bug; "
                 "please let us know so we can fix it!"
             )
         return measurement
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,45 @@
 
 import dataclasses
 import math
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import (
+    SparkColumnDescriptor,
+    SparkDataFrameDomain,
+    SparkFloatColumnDescriptor,
+    SparkIntegerColumnDescriptor,
+)
+from tmlt.core.measurements.aggregations import (
+    NoiseMechanism,
+    create_average_measurement,
+    create_count_distinct_measurement,
+    create_count_measurement,
+    create_quantile_measurement,
+    create_standard_deviation_measurement,
+    create_sum_measurement,
+    create_variance_measurement,
+)
+from tmlt.core.measurements.base import Measurement
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.metrics import (
+    DictMetric,
+    HammingDistance,
+    IfGroupedBy,
+    SymmetricDifference,
+)
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.spark_transformations.groupby import GroupBy
+from tmlt.core.transformations.spark_transformations.select import (
+    Select as SelectTransformation,
+)
+from tmlt.core.utils.exact_number import ExactNumber
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
@@ -28,64 +59,35 @@
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
 )
 from tmlt.analytics.keyset import KeySet
+from tmlt.analytics.privacy_budget import PrivacyBudget
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
     DropNullAndNan,
+    EnforceConstraint,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
     GroupByCountDistinct,
     GroupByQuantile,
     QueryExpr,
     QueryExprVisitor,
     ReplaceInfinity,
     StdevMechanism,
     SumMechanism,
     VarianceMechanism,
 )
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import (
-    SparkColumnDescriptor,
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-    SparkIntegerColumnDescriptor,
-)
-from tmlt.core.measurements.aggregations import (
-    NoiseMechanism,
-    create_average_measurement,
-    create_count_distinct_measurement,
-    create_count_measurement,
-    create_quantile_measurement,
-    create_standard_deviation_measurement,
-    create_sum_measurement,
-    create_variance_measurement,
-)
-from tmlt.core.measurements.base import Measurement
-from tmlt.core.measures import PureDP, RhoZCDP
-from tmlt.core.metrics import (
-    DictMetric,
-    HammingDistance,
-    IfGroupedBy,
-    SymmetricDifference,
-)
-from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.spark_transformations.groupby import GroupBy
-from tmlt.core.transformations.spark_transformations.select import (
-    Select as SelectTransformation,
-)
-from tmlt.core.utils.exact_number import ExactNumber
 
 
 def _get_query_bounds(
     query: Union[
         GroupByBoundedAverage,
         GroupByBoundedSTDEV,
         GroupByBoundedSum,
@@ -126,15 +128,15 @@
     if max_rows_per_id:
         ret.append((max_rows_per_id,))
     return ret
 
 
 def _constraint_stability(
     constraints: Tuple[Constraint, ...],
-    output_measure: Union[PureDP, RhoZCDP],
+    output_measure: Union[PureDP, ApproxDP, RhoZCDP],
     grouping_columns: List[str],
 ) -> float:
     """Compute the transformation stability of applying the given constraints.
 
     The values produced by this method are not intended for use doing actual
     stability calculations, they are just to provide an easy way to evaluate the
     relative stabilities of different possible truncations.
@@ -144,14 +146,15 @@
     elif (
         len(constraints) == 2
         and isinstance(constraints[0], MaxGroupsPerID)
         and isinstance(constraints[1], MaxRowsPerGroupPerID)
     ):
         if (
             output_measure == PureDP()
+            or output_measure == ApproxDP()
             or constraints[0].grouping_column not in grouping_columns
         ):
             return constraints[0].max * constraints[1].max
         elif output_measure == RhoZCDP():
             return math.sqrt(constraints[0].max) * constraints[1].max
         else:
             raise AssertionError(
@@ -162,31 +165,115 @@
         raise AssertionError(
             f"Constraints {constraints} are not a combination for which a stability "
             "can be computed. This is probably a bug; please let us know about it "
             "so we can fix it!"
         )
 
 
+def _generate_constrained_count_distinct(
+    query: GroupByCountDistinct, schema: Schema, constraints: List[Constraint]
+) -> Optional[GroupByCount]:
+    """Return a more optimal query for the given count-distinct, if one exists.
+
+    This method handles inferring additional constraints on a
+    GroupByCountDistinct query and using those constraints to generate more
+    optimal queries. This is possible in two cases, both on IDs tables:
+
+    - Only the ID column is being counted, and no groupby is performed. When
+      this happens, each ID can contribute at most once to the resulting count,
+      equivalent to a ``MaxRowsPerID(1)`` constraint.
+
+    - Only the ID column is being counted, and the result is grouped on exactly
+      one column which has a MaxGroupsPerID constraint on it. In this case, each
+      ID can contribute at most once to the count of each group, equivalent to a
+      ``MaxRowsPerGroupPerID(other_column, 1)`` constraint.
+
+    In both of these cases, a performance optimization is also possible: because
+    enforcing the constraints drops all but one of the rows per ID in the first
+    case or per (ID, group) value pair in the second, a normal count query will
+    produce the same result and should run faster because it doesn't need to
+    handle deduplicating the values.
+    """
+    columns_to_count = set(query.columns_to_count or schema.columns)
+    groupby_columns = query.groupby_keys.dataframe().columns
+
+    # For non-IDs cases or cases where columns other than the ID column must be
+    # distinct, there's no optimization to make.
+    if schema.id_column is None or columns_to_count != {schema.id_column}:
+        return None
+
+    mechanism = (
+        CountMechanism.DEFAULT
+        if query.mechanism == CountDistinctMechanism.DEFAULT
+        else CountMechanism.LAPLACE
+        if query.mechanism == CountDistinctMechanism.LAPLACE
+        else CountMechanism.GAUSSIAN
+        if query.mechanism == CountDistinctMechanism.GAUSSIAN
+        else None
+    )
+    if mechanism is None:
+        raise AssertionError(
+            f"Unknown mechanism {query.mechanism}. This is probably a bug; "
+            "please let us know about it so we can fix it!"
+        )
+
+    if not groupby_columns:
+        # No groupby is performed; this is equivalent to a MaxRowsPerID(1)
+        # constraint on the table.
+        return GroupByCount(
+            EnforceConstraint(query.child, MaxRowsPerID(1)),
+            groupby_keys=query.groupby_keys,
+            output_column=query.output_column,
+            mechanism=mechanism,
+        )
+    elif len(groupby_columns) == 1:
+        # A groupby on exactly one column is performed; if that column has a
+        # MaxGroupsPerID constraint, then this is equivalent to a
+        # MaxRowsPerGroupsPerID(grouping_column, 1) constraint.
+        grouping_column = groupby_columns[0]
+        constraint = next(
+            (
+                c
+                for c in constraints
+                if isinstance(c, MaxGroupsPerID)
+                and c.grouping_column == grouping_column
+            ),
+            None,
+        )
+        if constraint is not None:
+            return GroupByCount(
+                EnforceConstraint(
+                    query.child, MaxRowsPerGroupPerID(constraint.grouping_column, 1)
+                ),
+                groupby_keys=query.groupby_keys,
+                output_column=query.output_column,
+                mechanism=mechanism,
+            )
+
+    # If none of the above cases are true, no optimization is possible.
+    return None
+
+
 class MeasurementVisitor(QueryExprVisitor):
     """A visitor to create a measurement from a query expression."""
 
     def __init__(
         self,
-        per_query_privacy_budget: sp.Expr,
+        privacy_budget: PrivacyBudget,
         stability: Any,
         input_domain: DictDomain,
         input_metric: DictMetric,
-        output_measure: Union[PureDP, RhoZCDP],
+        output_measure: Union[PureDP, ApproxDP, RhoZCDP],
         default_mechanism: NoiseMechanism,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
         table_constraints: Dict[Identifier, List[Constraint]],
     ):
         """Constructor for MeasurementVisitor."""
-        self.budget = per_query_privacy_budget
+        self.budget = privacy_budget
         self.stability = stability
         self.input_domain = input_domain
         self.input_metric = input_metric
         self.default_mechanism = default_mechanism
         self.public_sources = public_sources
         self.output_measure = output_measure
         self.catalog = catalog
@@ -266,15 +353,15 @@
 
     def _pick_noise_for_count(
         self, query: Union[GroupByCount, GroupByCountDistinct]
     ) -> NoiseMechanism:
         """Pick the noise mechanism to use for a count or count-distinct query."""
         requested_mechanism: NoiseMechanism
         if query.mechanism in (CountMechanism.DEFAULT, CountDistinctMechanism.DEFAULT):
-            if isinstance(self.output_measure, PureDP):
+            if isinstance(self.output_measure, (PureDP, ApproxDP)):
                 requested_mechanism = NoiseMechanism.LAPLACE
             else:  # output measure is RhoZCDP
                 requested_mechanism = NoiseMechanism.DISCRETE_GAUSSIAN
         elif query.mechanism in (
             CountMechanism.LAPLACE,
             CountDistinctMechanism.LAPLACE,
         ):
@@ -321,15 +408,15 @@
             SumMechanism.DEFAULT,
             AverageMechanism.DEFAULT,
             VarianceMechanism.DEFAULT,
             StdevMechanism.DEFAULT,
         ):
             requested_mechanism = (
                 NoiseMechanism.LAPLACE
-                if isinstance(self.output_measure, PureDP)
+                if isinstance(self.output_measure, (PureDP, ApproxDP))
                 else NoiseMechanism.DISCRETE_GAUSSIAN
             )
         elif query.mechanism in (
             SumMechanism.LAPLACE,
             AverageMechanism.LAPLACE,
             VarianceMechanism.LAPLACE,
             StdevMechanism.LAPLACE,
@@ -440,18 +527,18 @@
 
         expected_schema = query.child.accept(OutputSchemaVisitor(self.catalog))
 
         # You can't perform these queries on nulls, NaNs, or infinite values
         # so check for those
         try:
             measure_desc = expected_schema[query.measure_column]
-        except KeyError:
+        except KeyError as e:
             raise KeyError(
                 f"Measure column {query.measure_column} is not in the input schema."
-            )
+            ) from e
 
         new_child: Optional[QueryExpr] = None
         # If null or NaN values are allowed ...
         if measure_desc.allow_null or (
             measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_nan
         ):
             # then drop those values
@@ -504,307 +591,321 @@
             groupby=groupby,
             lower_bound=lower_bound,
             upper_bound=upper_bound,
         )
 
     def _validate_measurement(self, measurement: Measurement, mid_stability: sp.Expr):
         """Validate a measurement."""
-        if measurement.privacy_function(mid_stability) != self.budget:
+        if measurement.privacy_function(mid_stability) != self.budget.value:
             raise AssertionError(
                 "Privacy function does not match per-query privacy budget. "
                 "This is probably a bug; please let us know so we can "
                 "fix it!"
             )
 
-    def visit_groupby_count(self, query: GroupByCount) -> Measurement:
+    def visit_groupby_count(self, expr: GroupByCount) -> Measurement:
         """Create a measurement from a GroupByCount query expression."""
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_count(query)
-        mechanism = self._pick_noise_for_count(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_count(expr)
+        mechanism = self._pick_noise_for_count(expr)
         child_transformation, child_ref = self._truncate_table(
-            *self._visit_child_transformation(query.child, mechanism),
-            grouping_columns=query.groupby_keys.dataframe().columns,
+            *self._visit_child_transformation(expr.child, mechanism),
+            grouping_columns=expr.groupby_keys.dataframe().columns,
         )
 
         transformation = get_table_from_ref(child_transformation, child_ref)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         mid_stability = transformation.stability_function(self.stability)
         groupby = self._build_groupby(
             transformation.output_domain,
             transformation.output_metric,
-            query.groupby_keys,
+            expr.groupby_keys,
             mechanism,
         )
 
         agg = create_count_measurement(
             input_domain=transformation.output_domain,
             input_metric=transformation.output_metric,
             noise_mechanism=mechanism,
             d_in=mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
-            count_column=query.output_column,
+            count_column=expr.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
-    def visit_groupby_count_distinct(self, query: GroupByCountDistinct) -> Measurement:
+    def visit_groupby_count_distinct(self, expr: GroupByCountDistinct) -> Measurement:
         """Create a measurement from a GroupByCountDistinct query expression."""
+        mechanism = self._pick_noise_for_count(expr)
+        (
+            child_transformation,
+            child_ref,
+            child_constraints,
+        ) = self._visit_child_transformation(expr.child, mechanism)
+        constrained_query = _generate_constrained_count_distinct(
+            expr,
+            expr.child.accept(OutputSchemaVisitor(self.catalog)),
+            child_constraints,
+        )
+        if constrained_query is not None:
+            return constrained_query.accept(self)
+
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_count_distinct(query)
-        mechanism = self._pick_noise_for_count(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_count_distinct(expr)
+
         child_transformation, child_ref = self._truncate_table(
-            *self._visit_child_transformation(query.child, mechanism),
-            grouping_columns=query.groupby_keys.dataframe().columns,
+            child_transformation,
+            child_ref,
+            child_constraints,
+            grouping_columns=expr.groupby_keys.dataframe().columns,
         )
         transformation = get_table_from_ref(child_transformation, child_ref)
 
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         # If not counting all columns, drop the ones that are neither counted
         # nor grouped on.
-        if query.columns_to_count:
-            groupby_columns = list(query.groupby_keys.schema().keys())
+        if expr.columns_to_count:
+            groupby_columns = list(expr.groupby_keys.schema().keys())
             transformation |= SelectTransformation(
                 transformation.output_domain,
                 transformation.output_metric,
-                query.columns_to_count + groupby_columns,
+                list(set(expr.columns_to_count + groupby_columns)),
             )
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
 
         mid_stability = transformation.stability_function(self.stability)
         groupby = self._build_groupby(
             transformation.output_domain,
             transformation.output_metric,
-            query.groupby_keys,
+            expr.groupby_keys,
             mechanism,
         )
 
         agg = create_count_distinct_measurement(
             input_domain=transformation.output_domain,
             input_metric=transformation.output_metric,
             noise_mechanism=mechanism,
             d_in=mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
-            count_column=query.output_column,
+            count_column=expr.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
-    def visit_groupby_quantile(self, query: GroupByQuantile) -> Measurement:
+    def visit_groupby_quantile(self, expr: GroupByQuantile) -> Measurement:
         """Create a measurement from a GroupByQuantile query expression.
 
         This method also checks to see if the schema allows invalid values
         (nulls, NaNs, and infinite values) on the measure column; if so,
         the query has DropNullAndNan and/or DropInfinity queries
         inserted immediately before it is executed.
         """
-        child_schema: Schema = query.child.accept(OutputSchemaVisitor(self.catalog))
+        child_schema: Schema = expr.child.accept(OutputSchemaVisitor(self.catalog))
         # Check the measure column for nulls/NaNs/infs (which aren't allowed)
         try:
-            measure_desc = child_schema[query.measure_column]
-        except KeyError:
+            measure_desc = child_schema[expr.measure_column]
+        except KeyError as e:
             raise KeyError(
-                f"Measure column '{query.measure_column}' is not in the input schema."
-            )
+                f"Measure column '{expr.measure_column}' is not in the input schema."
+            ) from e
         # If null or NaN values are allowed ...
         if measure_desc.allow_null or (
             measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_nan
         ):
             # Those values aren't allowed! Drop them
             # (without mutating the original QueryExpr)
             drop_null_and_nan_query = DropNullAndNan(
-                child=query.child, columns=[query.measure_column]
+                child=expr.child, columns=[expr.measure_column]
             )
-            query = dataclasses.replace(query, child=drop_null_and_nan_query)
+            expr = dataclasses.replace(expr, child=drop_null_and_nan_query)
 
         # If infinite values are allowed ...
         if measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_inf:
             # Clamp those values
             # (without mutating the original QueryExpr)
             replace_infinity_query = ReplaceInfinity(
-                child=query.child,
-                replace_with={query.measure_column: (query.low, query.high)},
+                child=expr.child,
+                replace_with={expr.measure_column: (expr.low, expr.high)},
             )
-            query = dataclasses.replace(query, child=replace_infinity_query)
+            expr = dataclasses.replace(expr, child=replace_infinity_query)
 
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_quantile(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_quantile(expr)
 
         child_transformation, child_ref = self._truncate_table(
-            *self._visit_child_transformation(query.child, self.default_mechanism),
-            grouping_columns=query.groupby_keys.dataframe().columns,
+            *self._visit_child_transformation(expr.child, self.default_mechanism),
+            grouping_columns=expr.groupby_keys.dataframe().columns,
         )
         transformation = get_table_from_ref(child_transformation, child_ref)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
         mid_stability = transformation.stability_function(self.stability)
         groupby = self._build_groupby(
             transformation.output_domain,
             transformation.output_metric,
-            query.groupby_keys,
+            expr.groupby_keys,
             self.default_mechanism,
         )
 
         agg = create_quantile_measurement(
             input_domain=transformation.output_domain,
             input_metric=transformation.output_metric,
-            measure_column=query.measure_column,
-            quantile=query.quantile,
-            lower=query.low,
-            upper=query.high,
+            measure_column=expr.measure_column,
+            quantile=expr.quantile,
+            lower=expr.low,
+            upper=expr.high,
             d_in=mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=groupby,
-            quantile_column=query.output_column,
+            quantile_column=expr.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
-    def visit_groupby_bounded_sum(self, query: GroupByBoundedSum) -> Measurement:
+    def visit_groupby_bounded_sum(self, expr: GroupByBoundedSum) -> Measurement:
         """Create a measurement from a GroupByBoundedSum query expression."""
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_sum(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_sum(expr)
 
-        info = self._build_common(query)
+        info = self._build_common(expr)
         # _build_common already checks these;
         # these asserts are just for mypy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
 
         agg = create_sum_measurement(
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
-            measure_column=query.measure_column,
+            measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
-            sum_column=query.output_column,
+            sum_column=expr.output_column,
         )
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
-    def visit_groupby_bounded_average(
-        self, query: GroupByBoundedAverage
-    ) -> Measurement:
+    def visit_groupby_bounded_average(self, expr: GroupByBoundedAverage) -> Measurement:
         """Create a measurement from a GroupByBoundedAverage query expression."""
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_average(query)
-        info = self._build_common(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_average(expr)
+        info = self._build_common(expr)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
 
         agg = create_average_measurement(
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
-            measure_column=query.measure_column,
+            measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
-            average_column=query.output_column,
+            average_column=expr.output_column,
         )
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
     def visit_groupby_bounded_variance(
-        self, query: GroupByBoundedVariance
+        self, expr: GroupByBoundedVariance
     ) -> Measurement:
         """Create a measurement from a GroupByBoundedVariance query expression."""
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_variance(query)
-        info = self._build_common(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_variance(expr)
+        info = self._build_common(expr)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
 
         agg = create_variance_measurement(
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
-            measure_column=query.measure_column,
+            measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
-            variance_column=query.output_column,
+            variance_column=expr.output_column,
         )
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
-    def visit_groupby_bounded_stdev(self, query: GroupByBoundedSTDEV) -> Measurement:
+    def visit_groupby_bounded_stdev(self, expr: GroupByBoundedSTDEV) -> Measurement:
         """Create a measurement from a GroupByBoundedStdev query expression."""
         # Peek at the schema, to see if there are errors there
-        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_stdev(query)
-        info = self._build_common(query)
+        OutputSchemaVisitor(self.catalog).visit_groupby_bounded_stdev(expr)
+        info = self._build_common(expr)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
 
         agg = create_standard_deviation_measurement(
             input_domain=info.transformation.output_domain,
             input_metric=info.transformation.output_metric,
-            measure_column=query.measure_column,
+            measure_column=expr.measure_column,
             lower=info.lower_bound,
             upper=info.upper_bound,
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
-            d_out=self.budget,
+            d_out=self.budget.value,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
-            standard_deviation_column=query.output_column,
+            standard_deviation_column=expr.output_column,
         )
 
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
     # None of these produce measurements, so they all return a NotImplementedError
     def visit_private_source(self, expr) -> Any:
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,18 +150,18 @@
         KeysView[str], query.groupby_keys.schema().keys()
     )
     schema: Schema = query.groupby_keys.schema()
 
     for column_name, column_desc in schema.items():
         try:
             input_column_desc = input_schema[column_name]
-        except KeyError:
+        except KeyError as e:
             raise KeyError(
                 f"Groupby column '{column_name}' is not in the input schema."
-            )
+            ) from e
         if column_desc.column_type != input_column_desc.column_type:
             raise ValueError(
                 f"Groupby column '{column_name}' has type"
                 f" '{column_desc.column_type.name}', but the column with the same name"
                 f" in the input data has type '{input_column_desc.column_type.name}'"
                 " instead."
             )
@@ -229,14 +229,15 @@
             **{
                 query.output_column: ColumnDescriptor(
                     output_column_type, allow_null=False
                 )
             },
         },
         grouping_column=None,
+        id_column=None,
     )
     return output_schema
 
 
 class OutputSchemaVisitor(QueryExprVisitor):
     """A visitor to get the output schema of a query expression."""
 
@@ -345,15 +346,15 @@
         spark = SparkSession.builder.getOrCreate()
         test_df = spark.createDataFrame(
             [], schema=analytics_to_spark_schema(input_schema)
         )
         try:
             test_df.filter(expr.condition)
         except Exception as e:
-            raise ValueError(f"Invalid filter condition '{expr.condition}': {e}")
+            raise ValueError(f"Invalid filter condition '{expr.condition}': {e}") from e
         return input_schema
 
     def visit_select(self, expr: Select) -> Schema:
         """Returns the resulting schema from evaluating a Select.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
@@ -458,15 +459,14 @@
             raise ValueError(
                 "Map must set augment=True to ensure that "
                 f"ID column '{input_schema.id_column}' is not lost."
             )
         return new_columns
 
     def visit_flat_map(self, expr: FlatMap) -> Schema:
-        # pylint: disable=line-too-long
         """Returns the resulting schema from evaluating a FlatMap.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType, Schema
             >>> from tmlt.analytics.query_expr import FlatMap, PrivateSource
 
         Example:
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,69 +5,14 @@
 
 import dataclasses
 import datetime
 import warnings
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, Union
 
 from pyspark.sql import DataFrame
-
-from tmlt.analytics._catalog import Catalog
-from tmlt.analytics._query_expr_compiler._constraint_propagation import (
-    propagate_flat_map,
-    propagate_join_private,
-    propagate_join_public,
-    propagate_map,
-    propagate_rename,
-    propagate_replace,
-    propagate_select,
-    propagate_unmodified,
-)
-from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
-    OutputSchemaVisitor,
-)
-from tmlt.analytics._schema import (
-    ColumnDescriptor,
-    ColumnType,
-    Schema,
-    analytics_to_spark_columns_descriptor,
-    spark_dataframe_domain_to_analytics_columns,
-    spark_schema_to_analytics_columns,
-)
-from tmlt.analytics._table_identifier import Identifier, TemporaryTable
-from tmlt.analytics._table_reference import (
-    TableReference,
-    find_named_tables,
-    find_reference,
-    lookup_domain,
-    lookup_metric,
-)
-from tmlt.analytics._transformation_utils import generate_nested_transformation
-from tmlt.analytics.constraints import Constraint, simplify_constraints
-from tmlt.analytics.query_expr import AnalyticsDefault
-from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
-from tmlt.analytics.query_expr import DropNullAndNan, EnforceConstraint
-from tmlt.analytics.query_expr import Filter as FilterExpr
-from tmlt.analytics.query_expr import FlatMap as FlatMapExpr
-from tmlt.analytics.query_expr import (
-    GroupByBoundedAverage,
-    GroupByBoundedSTDEV,
-    GroupByBoundedSum,
-    GroupByBoundedVariance,
-    GroupByCount,
-    GroupByCountDistinct,
-    GroupByQuantile,
-)
-from tmlt.analytics.query_expr import JoinPrivate as JoinPrivateExpr
-from tmlt.analytics.query_expr import JoinPublic as JoinPublicExpr
-from tmlt.analytics.query_expr import Map as MapExpr
-from tmlt.analytics.query_expr import QueryExpr, QueryExprVisitor
-from tmlt.analytics.query_expr import Rename as RenameExpr
-from tmlt.analytics.query_expr import ReplaceInfinity, ReplaceNullAndNan
-from tmlt.analytics.query_expr import Select as SelectExpr
-from tmlt.analytics.truncation_strategy import TruncationStrategy
 from tmlt.core.domains.collections import DictDomain, ListDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain, SparkRowDomain
 from tmlt.core.measurements.aggregations import NoiseMechanism
 from tmlt.core.metrics import (
     AddRemoveKeys,
     DictMetric,
     HammingDistance,
@@ -167,14 +112,69 @@
 from tmlt.core.transformations.spark_transformations.rename import (
     Rename as RenameTransformation,
 )
 from tmlt.core.transformations.spark_transformations.select import (
     Select as SelectTransformation,
 )
 
+from tmlt.analytics._catalog import Catalog
+from tmlt.analytics._query_expr_compiler._constraint_propagation import (
+    propagate_flat_map,
+    propagate_join_private,
+    propagate_join_public,
+    propagate_map,
+    propagate_rename,
+    propagate_replace,
+    propagate_select,
+    propagate_unmodified,
+)
+from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
+    OutputSchemaVisitor,
+)
+from tmlt.analytics._schema import (
+    ColumnDescriptor,
+    ColumnType,
+    Schema,
+    analytics_to_spark_columns_descriptor,
+    spark_dataframe_domain_to_analytics_columns,
+    spark_schema_to_analytics_columns,
+)
+from tmlt.analytics._table_identifier import Identifier, TemporaryTable
+from tmlt.analytics._table_reference import (
+    TableReference,
+    find_named_tables,
+    find_reference,
+    lookup_domain,
+    lookup_metric,
+)
+from tmlt.analytics._transformation_utils import generate_nested_transformation
+from tmlt.analytics.constraints import Constraint, simplify_constraints
+from tmlt.analytics.query_expr import AnalyticsDefault
+from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
+from tmlt.analytics.query_expr import DropNullAndNan, EnforceConstraint
+from tmlt.analytics.query_expr import Filter as FilterExpr
+from tmlt.analytics.query_expr import FlatMap as FlatMapExpr
+from tmlt.analytics.query_expr import (
+    GroupByBoundedAverage,
+    GroupByBoundedSTDEV,
+    GroupByBoundedSum,
+    GroupByBoundedVariance,
+    GroupByCount,
+    GroupByCountDistinct,
+    GroupByQuantile,
+)
+from tmlt.analytics.query_expr import JoinPrivate as JoinPrivateExpr
+from tmlt.analytics.query_expr import JoinPublic as JoinPublicExpr
+from tmlt.analytics.query_expr import Map as MapExpr
+from tmlt.analytics.query_expr import QueryExpr, QueryExprVisitor
+from tmlt.analytics.query_expr import Rename as RenameExpr
+from tmlt.analytics.query_expr import ReplaceInfinity, ReplaceNullAndNan
+from tmlt.analytics.query_expr import Select as SelectExpr
+from tmlt.analytics.truncation_strategy import TruncationStrategy
+
 
 class TransformationVisitor(QueryExprVisitor):
     """A visitor to create a transformation from a query expression."""
 
     class Output(NamedTuple):
         """A container for the outputs of the visitor."""
 
@@ -347,19 +347,19 @@
             raise ValueError(
                 f"Table '{expr.source_id}' does not exist. "
                 f"Available tables are: {named_tables}"
             )
         transformation = IdentityTransformation(self.input_metric, self.input_domain)
         try:
             constraints = self.table_constraints[ref.identifier]
-        except KeyError:
+        except KeyError as e:
             raise AssertionError(
                 f"Table {ref.identifier} not present in constraints dictionary. "
                 "This is probably a bug; please let us know about it so we can fix it!"
-            )
+            ) from e
         return self.Output(transformation, ref, constraints)
 
     def visit_rename(self, expr: RenameExpr) -> Output:
         """Create a transformation from a Rename query expression."""
         child_transformation, child_ref, child_constraints = expr.child.accept(self)
 
         def gen_transformation_dictmetric(parent_domain, parent_metric, target):
@@ -507,15 +507,18 @@
             raise AssertionError(
                 "Unrecognized input domain. This is probably a bug; "
                 "please let us know about it so we can fix it!"
             )
         transformer_input_domain = SparkRowDomain(input_domain.schema)
         # Any new column created by Map could contain a null value
         spark_columns_descriptor = {
-            k: dataclasses.replace(v, allow_null=True)
+            # all of the Spark<Type>ColumnDescriptor classes are dataclasses,
+            # but the SparkColumnDescriptor base class isn't;
+            # hence the "type: ignore" here
+            k: dataclasses.replace(v, allow_null=True)  # type: ignore
             for k, v in analytics_to_spark_columns_descriptor(
                 expr.schema_new_columns
             ).items()
         }
 
         if expr.augment:
             output_schema = {
@@ -591,15 +594,18 @@
             raise AssertionError(
                 "Unrecognized input domain. This is probably a bug; "
                 "please let us know about it so we can fix it!"
             )
         transformer_input_domain = SparkRowDomain(input_domain.schema)
         # Any new column created by FlatMap could contain a null value
         spark_columns_descriptor = {
-            k: dataclasses.replace(v, allow_null=True)
+            # all of the Spark<Type>ColumnDescriptor classes are dataclasses,
+            # but the SparkColumnDescriptor base class isn't;
+            # hence the "type: ignore" here
+            k: dataclasses.replace(v, allow_null=True)  # type: ignore
             for k, v in analytics_to_spark_columns_descriptor(
                 expr.schema_new_columns
             ).items()
         }
 
         if expr.augment:
             output_schema = {
@@ -827,25 +833,25 @@
             *self._visit_child(expr.child)
         )
 
         public_df: DataFrame
         if isinstance(expr.public_table, str):
             try:
                 public_df = self.public_sources[expr.public_table]
-            except KeyError:
+            except KeyError as e:
                 raise ValueError(
                     f"There is no public source with the identifier {expr.public_table}"
-                )
+                ) from e
         else:
             public_df = expr.public_table
 
         public_df_schema = Schema(spark_schema_to_analytics_columns(public_df.schema))
 
         join_null_cols = any(
-            public_df_schema[col].allow_null for col in public_df_schema.keys()
+            col_desc.allow_null for col_desc in public_df_schema.values()
         )
 
         def gen_transformation_dictmetric(parent_domain, parent_metric, target):
             input_domain = lookup_domain(child_transformation.output_domain, child_ref)
             input_metric = lookup_metric(child_transformation.output_metric, child_ref)
             if not isinstance(input_domain, SparkDataFrameDomain):
                 raise AssertionError(
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_schema.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     IntegerType,
     LongType,
     StringType,
     StructField,
     StructType,
     TimestampType,
 )
-
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.spark_domains import (
     SparkColumnDescriptor,
     SparkColumnsDescriptor,
     SparkDataFrameDomain,
     SparkDateColumnDescriptor,
     SparkFloatColumnDescriptor,
@@ -165,14 +164,19 @@
                     column_type=ColumnType[ty],
                     allow_null=default_allow_null,
                     allow_nan=default_allow_nan,
                     allow_inf=default_allow_inf,
                 )
 
     @property
+    def columns(self):
+        """Return the names of the columns in the schema."""
+        return self._column_descs.keys()
+
+    @property
     def column_descs(self) -> Dict[str, ColumnDescriptor]:
         """Returns a mapping from column name to column descriptor."""
         return dict(self._column_descs)
 
     @property
     def column_types(self) -> Dict[str, str]:
         """Returns a mapping from column name to column type."""
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_identifier.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_table_identifier.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_reference.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_table_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 from dataclasses import dataclass
 from typing import List, Optional, Union
 
-from tmlt.analytics._table_identifier import Identifier, NamedTable
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.metrics import (
     AddRemoveKeys,
     DictMetric,
     IfGroupedBy,
     Metric,
     SymmetricDifference,
 )
 
+from tmlt.analytics._table_identifier import Identifier, NamedTable
+
 
 @dataclass(frozen=True)
 class TableReference:
     """A way to reference tables via their path."""
 
     path: List[Identifier]
     """The path for the table reference, provided as a list of Identifiers."""
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/_transformation_utils.py` & `tmlt_analytics-0.7.1/tmlt/analytics/_transformation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 # pylint: disable=unused-argument
 
 from typing import Callable, Dict, Optional, Tuple, Type, cast
 
-from tmlt.analytics._table_identifier import Identifier, TemporaryTable
-from tmlt.analytics._table_reference import TableReference, lookup_domain, lookup_metric
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.metrics import AddRemoveKeys, DictMetric, Metric
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.dictionary import GetValue as GetValueTransformation
 from tmlt.core.transformations.dictionary import Subset as SubsetTransformation
@@ -33,14 +31,17 @@
 from tmlt.core.transformations.spark_transformations.persist import (
     Persist as PersistTransformation,
 )
 from tmlt.core.transformations.spark_transformations.persist import (
     Unpersist as UnpersistTransformation,
 )
 
+from tmlt.analytics._table_identifier import Identifier, TemporaryTable
+from tmlt.analytics._table_reference import TableReference, lookup_domain, lookup_metric
+
 
 def generate_nested_transformation(
     base_transformation: Transformation,
     parent_reference: TableReference,
     generator_dict: Dict[
         Type[Metric], Callable[[Domain, Metric, Identifier], Transformation]
     ],
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.7.1/tmlt/analytics/binning_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,47 +4,51 @@
 # Copyright Tumult Labs 2023
 
 import bisect
 import datetime
 import math
 from typing import Any, Generic, List, Optional, Sequence, TypeVar, cast
 
-from tmlt.analytics._schema import ColumnDescriptor, ColumnType, column_type_to_py_type
 from tmlt.core.utils.type_utils import get_element_type
 
+from tmlt.analytics._schema import ColumnDescriptor, ColumnType, column_type_to_py_type
+
 BinT = TypeVar("BinT", str, int, float, datetime.date, datetime.datetime)
 BinNameT = TypeVar("BinNameT", str, int, float, datetime.date, datetime.datetime)
 
 
 def _get_column_descriptor(
     bin_names: Sequence[Any], nan_bin: Optional[BinNameT]
 ) -> ColumnDescriptor:
     """Return the ColumnDescriptor for the non-``None`` elements of a list.
 
-    allow_nan is True if any bin_names element either matches nan_bin, or isnan.
-    allow_inf is True if any bin_names element matches float("inf") or float("-inf").
-    allow_null is True if any bin_names element when lowercased matches "null".
+    * allow_nan is True if
+       - any bin name, including nan_bin, is NaN.
+    * allow_inf is True if
+       - any bin name, including nan_bin, matches float("inf") or float("-inf").
+    * allow_null is True if (for simplicity, we always set it to be True)
+           - A value is Null.
+           - A value is out of bounds.
+           - A value is NaN, and nan_bin is not used.
     """
-    allow_null = False
-    allow_nan = False
-    allow_inf = False
-
-    for bin_name in bin_names:
-        if not allow_null and str(bin_name).lower() == "null":
-            allow_null = True
-        elif not allow_nan and (
-            bin_name == nan_bin
-            or (isinstance(bin_name, float) and math.isnan(bin_name))
-        ):
-            allow_nan = True
-        elif not allow_inf and bin_name == float("inf") or bin_name == float("-inf"):
-            allow_inf = True
+    if nan_bin is not None:
+        all_bin_names = list(bin_names) + [nan_bin]
+    else:
+        all_bin_names = list(bin_names)
+    allow_nan = any(
+        isinstance(bin_name, float) and math.isnan(bin_name)
+        for bin_name in all_bin_names
+    )
+    allow_inf = any(
+        bin_name in [float("inf"), float("-inf")] for bin_name in all_bin_names
+    )
+    allow_null = True
 
+    # nan_bin type is checked in the __init__.
     column_type = ColumnType(get_element_type(bin_names, allow_none=False))
-
     return ColumnDescriptor(column_type, allow_null, allow_nan, allow_inf)
 
 
 def _edges_as_str(bin_edges: List[BinT]) -> List[str]:
     """Format the bin edges as strings."""
     if isinstance(bin_edges[0], float):
         # 17 is roughly the maximum number of decimal digits that can be encoded
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_base.py` & `tmlt_analytics-0.7.1/tmlt/analytics/constraints/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 
 from abc import ABC, abstractmethod
 from typing import Tuple
 
-from tmlt.analytics._table_reference import TableReference
 from tmlt.core.transformations.base import Transformation
 
+from tmlt.analytics._table_reference import TableReference
+
 
 class Constraint(ABC):
     """A known, enforceable fact about a table.
 
     Constraints provide information about the contents of a table to help
     produce differentially-private results. For example, a constraint might say
     that each ID in a table corresponds to no more than two rows in that table
     (the :class:`~tmlt.analytics.constraints.MaxRowsPerID`
-    constraint). Constraints are applied via the :meth:`QueryBuilder.enforce
+    constraint). Constraints are applied via the :meth:`QueryBuilder.enforce()
     <tmlt.analytics.query_builder.QueryBuilder.enforce>` method.
 
     This class is a base class for all constraints, and cannot be used directly.
     """
 
     @abstractmethod
     def _enforce(
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_simplify.py` & `tmlt_analytics-0.7.1/tmlt/analytics/constraints/_simplify.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_truncation.py` & `tmlt_analytics-0.7.1/tmlt/analytics/constraints/_truncation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,14 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
 
 from dataclasses import dataclass
 from typing import Dict, List, Tuple, Union
 
-from typeguard import check_type
-
-from tmlt.analytics._table_identifier import TemporaryTable
-from tmlt.analytics._table_reference import TableReference, lookup_metric
-from tmlt.analytics._transformation_utils import (
-    generate_nested_transformation,
-    get_table_from_ref,
-)
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.metrics import (
     AddRemoveKeys,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
@@ -38,14 +30,22 @@
     LimitRowsPerKeyPerGroupValue,
 )
 from tmlt.core.transformations.spark_transformations.truncation import (
     LimitKeysPerGroup,
     LimitRowsPerGroup,
     LimitRowsPerKeyPerGroup,
 )
+from typeguard import check_type
+
+from tmlt.analytics._table_identifier import TemporaryTable
+from tmlt.analytics._table_reference import TableReference, lookup_metric
+from tmlt.analytics._transformation_utils import (
+    generate_nested_transformation,
+    get_table_from_ref,
+)
 
 from ._base import Constraint
 
 
 def simplify_truncation_constraints(constraints: List[Constraint]) -> List[Constraint]:
     """Remove redundant truncation constraints from a list of constraints."""
     max_rows_per_id, other_constraints = [], []
@@ -247,19 +247,19 @@
                 child_ref.parent,
                 {AddRemoveKeys: gen_tranformation_ark},
             )
 
 
 @dataclass(frozen=True)
 class MaxRowsPerGroupPerID(Constraint):
-    """A constraint limiting the number of rows associated with each unique (ID, grouping column) pair in a table.
+    """A constraint limiting rows per unique (ID, grouping column) pair in a table.
 
     For example, ``MaxRowsPerGroupPerID("group_col", 5)`` guarantees that each
-    ID appears in at most five rows for each distinct value of group_col".
-    """  # pylint: disable=line-too-long
+    ID appears in at most five rows for each distinct value in ``group_col``.
+    """
 
     grouping_column: str
     """Name of column defining the groups to truncate."""
 
     max: int
     """The maximum number of times each distinct value may appear in the column."""
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/keyset.py` & `tmlt_analytics-0.7.1/tmlt/analytics/keyset.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 from __future__ import annotations
 
 import datetime
 from typing import Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Type, Union
 
 from pyspark.sql import Column, DataFrame
 from pyspark.sql import types as spark_types
-
-from tmlt.analytics._coerce_spark_schema import coerce_spark_schema_or_fail
-from tmlt.analytics._schema import Schema, spark_schema_to_analytics_columns
 from tmlt.core.transformations.spark_transformations.groupby import (
     compute_full_domain_df,
 )
 from tmlt.core.utils.type_utils import get_element_type
 
+from tmlt.analytics._coerce_spark_schema import coerce_spark_schema_or_fail
+from tmlt.analytics._schema import Schema, spark_schema_to_analytics_columns
+
 
 def _check_df_schema(types: spark_types.StructType):
     """Raise an exception if any of the given types are not allowed in a KeySet."""
     allowed_types = {
         spark_types.LongType(),
         spark_types.StringType(),
         spark_types.DateType(),
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.7.1/tmlt/analytics/privacy_budget.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,49 @@
 
 For a full introduction to privacy budgets, see the
 :ref:`privacy budget topic guide<Privacy budget fundamentals>`.
 """
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2023
+
 import math
-from abc import ABC
-from typing import Union
+from abc import ABC, abstractmethod
+from typing import Tuple, Union
 
+import sympy as sp
+from tmlt.core.utils.exact_number import ExactNumber
 from typeguard import typechecked
 
-from tmlt.core.utils.exact_number import ExactNumber
+
+def _is_exact_number_from_integer(value: ExactNumber) -> bool:
+    """Returns True if the ExactNumber is an integer."""
+    return isinstance(value.expr, sp.Integer)
+
+
+def _to_int_or_float(value: ExactNumber) -> Union[int, float]:
+    """Converts an ExactNumber to an int or float."""
+    if _is_exact_number_from_integer(value):
+        return int(value.expr)
+    else:
+        return float(value.expr)
+
+
+def _to_exact_number(value: Union[int, float, ExactNumber]) -> ExactNumber:
+    """Converts a value to an ExactNumber."""
+    if isinstance(value, ExactNumber):
+        return value
+    elif isinstance(value, int):
+        return ExactNumber(value)
+    elif isinstance(value, float):
+        return ExactNumber.from_float(value, round_up=False)
+    else:
+        raise ValueError(
+            f"Cannot convert value of type {type(value)} to an ExactNumber."
+        )
 
 
 class PrivacyBudget(ABC):
     """Base class for specifying privacy parameters.
 
     A PrivacyBudget is a privacy definition, along with its associated parameters.
     The choice of a PrivacyBudget has an impact on the accuracy of query
@@ -27,165 +55,217 @@
         An "infinite" privacy budget means that the chosen DP algorithm will use
         parameters that do not guarantee privacy. This is not always exactly equivalent
         to evaluating the query without applying differential privacy.
         Please see the individual subclasses of PrivacyBudget for details on how to
         appropriately specify infinite budgets.
     """
 
+    @property
+    @abstractmethod
+    def value(self) -> Union[ExactNumber, Tuple[ExactNumber, ExactNumber]]:
+        """Return the value of the privacy budget."""
+
 
 class PureDPBudget(PrivacyBudget):
     """A privacy budget under pure differential privacy.
 
     This privacy definition is also known as epsilon-differential privacy, and the
     associated value is the epsilon privacy parameter. The privacy definition can
     be found `here <https://en.wikipedia.org/wiki/Differential_privacy#Definition_of_%CE%B5-differential_privacy>`__.
     """  # pylint: disable=line-too-long
 
     @typechecked
-    def __init__(self, epsilon: Union[int, float]):
+    def __init__(self, epsilon: Union[int, float, ExactNumber]):
         """Construct a new PureDPBudget.
 
         Args:
             epsilon: The epsilon privacy parameter. Must be non-negative
                 and cannot be NaN.
                 To specify an infinite budget, set epsilon equal to float('inf').
         """
-        if math.isnan(epsilon):
+        if not isinstance(epsilon, ExactNumber) and math.isnan(epsilon):
             raise ValueError("Epsilon cannot be a NaN.")
         if epsilon < 0:
             raise ValueError(
                 "Epsilon must be non-negative. "
                 f"Cannot construct a PureDPBudget with epsilon of {epsilon}."
             )
-        self._epsilon = epsilon
+        self._epsilon = _to_exact_number(epsilon)
 
     @property
-    def epsilon(self) -> Union[int, float]:
-        """Returns the value of epsilon."""
+    def value(self) -> ExactNumber:
+        """Return the value of the privacy budget as an ExactNumber.
+
+        For printing purposes, you should use the epsilon property instead, as it will
+        represent the same value, but be more human readable.
+        """
         return self._epsilon
 
+    @property
+    def epsilon(self) -> Union[int, float]:
+        """Returns the value of epsilon as an int or float.
+
+        This is helpful for human readability. If you need to use the epsilon value in
+        a computation, you should use self.value instead.
+        """
+        return _to_int_or_float(self._epsilon)
+
     def __repr__(self) -> str:
         """Returns string representation of this PureDPBudget."""
         return f"PureDPBudget(epsilon={self.epsilon})"
 
     def __eq__(self, other) -> bool:
-        """Returns whether or not two PureDPBudgets are equivalent."""
+        """Returns whether or not a PureDPBudget are equivalent to another PrivacyBudget.
+
+        PureDPBudgets are considered equal to ApproxDPBudgets that have delta of 0, and the same epsilon.
+        """
         if isinstance(other, PureDPBudget):
-            return ExactNumber.from_float(
-                self.epsilon, False
-            ) == ExactNumber.from_float(other.epsilon, False)
+            return self.value == other.value
+        if isinstance(other, ApproxDPBudget):
+            if self._epsilon == other._epsilon and other._delta == 0:
+                return True
         return False
 
 
 class ApproxDPBudget(PrivacyBudget):
     """A privacy budget under approximate differential privacy.
 
     This privacy definition is also known as (ε, δ)-differential privacy, and the
     associated privacy parameters are epsilon and delta. The formal definition can
     be found `here <https://desfontain.es/privacy/almost-differential-privacy.html#formal-definition>`__.
     """  # pylint: disable=line-too-long
 
     @typechecked
-    def __init__(self, epsilon: Union[int, float], delta: float):
+    def __init__(
+        self,
+        epsilon: Union[int, float, ExactNumber],
+        delta: Union[int, float, ExactNumber],
+    ):
         """Construct a new ApproxDPBudget.
 
         Args:
             epsilon: The epsilon privacy parameter. Must be non-negative.
                 To specify an infinite budget, set epsilon equal to float('inf').
             delta: The delta privacy parameter. Must be between 0 and 1 (inclusive).
                 If delta is 0, this is equivalent to PureDP.
         """
-        if math.isnan(epsilon):
+        if not isinstance(epsilon, ExactNumber) and math.isnan(epsilon):
             raise ValueError("Epsilon cannot be a NaN.")
-        if math.isnan(delta):
+        if not isinstance(delta, ExactNumber) and math.isnan(delta):
             raise ValueError("Delta cannot be a NaN.")
         if epsilon < 0:
             raise ValueError(
                 "Epsilon must be non-negative. "
                 f"Cannot construct an ApproxDPBudget with epsilon of {epsilon}."
             )
         if delta < 0 or delta > 1:
             raise ValueError(
                 "Delta must be between 0 and 1 (inclusive). "
                 f"Cannot construct an ApproxDPBudget with delta of {delta}."
             )
-        self._epsilon = epsilon
-        self._delta = delta
+        self._epsilon = _to_exact_number(epsilon)
+        self._delta = _to_exact_number(delta)
+
+    @property
+    def value(self) -> Tuple[ExactNumber, ExactNumber]:
+        """Returns self._epsilon and self._delta as an ExactNumber tuple.
+
+        For printing purposes, you might want to use the epsilon and delta properties
+        instead, as they will represent the same values, but be more human readable.
+        """
+        return (self._epsilon, self._delta)
 
     @property
     def epsilon(self) -> Union[int, float]:
-        """Returns the value of epsilon."""
-        return self._epsilon
+        """Returns the value of epsilon as an int or float.
+
+        This is helpful for human readability. If you need to use the epsilon value in
+        a computation, you should use self.value[0] instead.
+        """
+        return _to_int_or_float(self._epsilon)
 
     @property
-    def delta(self) -> float:
-        """Returns the value of delta."""
-        return self._delta
+    def delta(self) -> Union[int, float]:
+        """Returns the value of delta as an int or float.
+
+        This is helpful for human readability. If you need to use the delta value in
+        a computation, you should use self.value[1] instead.
+        """
+        return _to_int_or_float(self._delta)
 
     @property
     def is_infinite(self) -> bool:
         """Returns true if epsilon is float('inf') or delta is 1."""
         return self.epsilon == float("inf") or self.delta == 1
 
     def __repr__(self) -> str:
         """Returns the string representation of this ApproxDPBudget."""
         return f"ApproxDPBudget(epsilon={self.epsilon}, delta={self.delta})"
 
     def __eq__(self, other) -> bool:
-        """Returns whether two ApproxDPBudgets are equivalent.
+        """Returns whether an ApproxDPBudget is equivalent to another privacy budget.
 
+        ApproxDPBudgets that have delta of 0 are considered equal to PureDPBudgets with the same epsilon.
         ApproxDPBudgets that provide no privacy guarantee are considered equal (for example, if one has an
         epsilon of float('inf') and the other has a delta of 1).
         """
         if isinstance(other, ApproxDPBudget):
             are_both_infinite = self.is_infinite and other.is_infinite
-            is_same_epsilon = ExactNumber.from_float(
-                self.epsilon, False
-            ) == ExactNumber.from_float(other.epsilon, False)
-            is_same_delta = ExactNumber.from_float(
-                self.delta, False
-            ) == ExactNumber.from_float(other.delta, False)
-            return are_both_infinite or (is_same_epsilon and is_same_delta)
+            return are_both_infinite or self.value == other.value
+        if isinstance(other, PureDPBudget):
+            if self._epsilon == other._epsilon and self._delta == 0:
+                return True
         return False
 
 
 class RhoZCDPBudget(PrivacyBudget):
     """A privacy budget under rho-zero-concentrated differential privacy.
 
     The definition of rho-zCDP can be found in
     `this <https://arxiv.org/pdf/1605.02065.pdf>`_ paper under Definition 1.1.
     """
 
     @typechecked()
-    def __init__(self, rho: Union[int, float]):
+    def __init__(self, rho: Union[int, float, ExactNumber]):
         """Construct a new RhoZCDPBudget.
 
         Args:
             rho: The rho privacy parameter.
                 Rho must be non-negative and cannot be NaN.
                 To specify an infinite budget, set rho equal to float('inf').
         """
-        if math.isnan(rho):
+        if not isinstance(rho, ExactNumber) and math.isnan(rho):
             raise ValueError("Rho cannot be a NaN.")
         if rho < 0:
             raise ValueError(
                 "Rho must be non-negative. "
                 f"Cannot construct a RhoZCDPBudget with rho of {rho}."
             )
-        self._rho = rho
+        self._rho = _to_exact_number(rho)
 
     @property
-    def rho(self) -> Union[int, float]:
-        """Returns the value of rho."""
+    def value(self) -> ExactNumber:
+        """Return the value of the privacy budget as an ExactNumber.
+
+        For printing purposes, you should use the rho property instead, as it will
+        represent the same value, but be more human readable.
+        """
         return self._rho
 
+    @property
+    def rho(self) -> Union[int, float]:
+        """Returns the value of rho as an int or float.
+
+        This is helpful for human readability. If you need to use the rho value in
+        a computation, you should use self.value instead.
+        """
+        return _to_int_or_float(self._rho)
+
     def __repr__(self) -> str:
         """Returns string representation of this RhoZCDPBudget."""
         return f"RhoZCDPBudget(rho={self.rho})"
 
     def __eq__(self, other) -> bool:
         """Returns whether or not two RhoZCDPBudgets are equivalent."""
         if isinstance(other, RhoZCDPBudget):
-            return ExactNumber.from_float(self.rho, False) == ExactNumber.from_float(
-                other.rho, False
-            )
+            return self.value == other.value
         return False
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.7.1/tmlt/analytics/protected_change.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 class AddOneRow(AddMaxRows):
     """A shorthand for the common case of :class:`AddMaxRows` with ``max_rows = 1``."""
 
     max_rows = 1
 
     def __init__(self):
         """@nodoc."""
-        super(AddOneRow, self).__init__(max_rows=1)
+        super().__init__(max_rows=1)
 
 
 @dataclass(frozen=True)
 class AddMaxRowsInMaxGroups(ProtectedChange):
     """Protect the addition or removal of rows across a finite number of groups.
 
     :class:`AddMaxRowsInMaxGroups` provides a similar guarantee to
@@ -115,15 +115,15 @@
 
     id_column: str
     """The name of the column containing the identifier."""
 
     id_space: str = "default_id_space"
     """The identifier space of the rows that may be added or removed. If not specified,
     a default will be assigned when using this protected change with
-    :class:`tmlt.analytics.session.Session.from_dataframe`."""
+    :class:`Session.from_dataframe()<tmlt.analytics.session.Session.from_dataframe>`."""
 
     def __post_init__(self):
         """Validate attributes."""
         check_type("id_space", self.id_space, str)
         if self.id_space == "":
             raise ValueError("identifier must be non-empty")
         check_type("id_column", self.id_column, str)
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.7.1/tmlt/analytics/query_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,23 +281,24 @@
         The current query can also join with a named private table (represented
         as a string).
 
         This operation is a natural join, with the same behavior and requirements as
         :func:`join_public`.
 
         For operations on tables with a
-        :class:`tmlt.analytics.protected_change.ProtectedChange` that protects adding or
-        removing rows (e.g., :class:`~tmlt.analytics.protected_change.AddMaxRows`),
-        there is a key difference: before the join is performed, each table is
-        *truncated* based on the corresponding
+        :class:`~tmlt.analytics.protected_change.ProtectedChange` that protects
+        adding or removing rows (e.g.
+        :class:`~tmlt.analytics.protected_change.AddMaxRows`), there is a key
+        difference: before the join is performed, each table is *truncated*
+        based on the corresponding
         :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`.
 
         In contrast, operations on tables with a
-        :class:`tmlt.analytics.protected_change.AddRowsWithID`
-        :class:`tmlt.analytics.protected_change.ProtectedChange` do not require a
+        :class:`~tmlt.analytics.protected_change.AddRowsWithID`
+        :class:`~tmlt.analytics.protected_change.ProtectedChange` do not require a
         :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`, as no
         truncation is necessary while performing the join.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
@@ -994,15 +995,15 @@
                 This function should return a dictionary, which should always
                 have the same keys regardless of input, and the values in that
                 dictionary should match the column type specified in
                 ``new_column_types``. The function should not have any side effects
                 (in particular, f cannot raise exceptions).
             new_column_types: Mapping from column names to types, for new columns
                 produced by f. Using
-                :class:`tmlt.analytics.query_builder.ColumnDescriptor`
+                :class:`~tmlt.analytics.query_builder.ColumnDescriptor`
                 is preferred.
             augment: If True, add new columns to the existing dataframe (so new
                      schema = old schema + schema_new_columns).
                      If False, make the new dataframe with schema = schema_new_columns
         """
         self._query_expr = Map(
             child=self._query_expr,
@@ -1029,16 +1030,16 @@
         """Updates the current query to apply a flat map.
 
         If you provide only a ColumnType for the new column types, Analytics
         assumes that all new columns created may contain null values (and that
         DECIMAL columns may contain NaN or infinite values).
 
         Operations on tables with a
-        :class:`tmlt.analytics.protected_change.AddRowsWithID`
-        :class:`tmlt.analytics.protected_change.ProtectedChange` do not require a
+        :class:`~tmlt.analytics.protected_change.AddRowsWithID`
+        :class:`~tmlt.analytics.protected_change.ProtectedChange` do not require a
         ``max_num_rows`` argument, since it is not necessary to impose a limit on
         the number of new rows.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
@@ -1104,29 +1105,29 @@
                 The function's input is a dictionary matching a column name to
                 its value for that row.
                 This function should return a list of dictionaries.
                 Those dictionaries should always
                 have the same keys regardless of input, and the values in those
                 dictionaries should match the column type specified in
                 ``new_column_types``. The function should not have any side effects
-                (in particular, f cannot raise exceptions).
+                (in particular, ``f`` must not raise exceptions).
             new_column_types: Mapping from column names to types, for new columns
-                produced by f. Using
-                :class:`tmlt.analytics.query_builder.ColumnDescriptor`
+                produced by ``f``. Using
+                :class:`~tmlt.analytics.query_builder.ColumnDescriptor`
                 is preferred.
             augment: If True, add new columns to the existing dataframe (so new
                      schema = old schema + schema_new_columns).
                      If False, make the new dataframe with schema = schema_new_columns
             grouping: Whether this produces a new column that we want to groupby.
                 If True, this requires that any groupby aggregations following this
                 query include the new column as a groupby column. Only one new column
                 is supported, and the new column must have distinct values for each
                 input row.
-            max_num_rows: The enforced limit on the number of rows from each f(row).
-                If f produces more rows than this, only the first ``max_num_rows``
+            max_num_rows: The enforced limit on the number of rows from each ``f(row)``.
+                If ``f`` produces more rows than this, only the first ``max_num_rows``
                 rows will be in the output.
         """
         grouping_column: Optional[str]
         if grouping:
             if len(new_column_types) != 1:
                 raise ValueError(
                     "new_column_types contains "
@@ -1237,17 +1238,15 @@
             name: The name of the column that will be created. If None (the default),
                 the input column name with ``_binned`` appended to it.
         """
         if name is None:
             name = f"{column}_binned"
         binning_fn = lambda row: {name: spec(row[column])}
         return self.map(
-            binning_fn,
-            new_column_types={name: spec.column_descriptor.column_type},
-            augment=True,
+            binning_fn, new_column_types={name: spec.column_descriptor}, augment=True
         )
 
     def histogram(
         self,
         column: str,
         bin_edges: Union[Sequence[BinT], BinningSpec],
         name: Optional[str] = None,
@@ -1322,14 +1321,17 @@
 
     def enforce(self, constraint: Constraint) -> "QueryBuilder":
         """Enforce a :mod:`~tmlt.analytics.constraints.Constraint` on the current table.
 
         This method can be used to enforce constraints on the current table. See
         the :mod:`~tmlt.analytics.constraints` module for information about the
         available constraints and what they are used for.
+
+        Args:
+            constraint: The constraint to enforce.
         """
         self._query_expr = EnforceConstraint(self._query_expr, constraint, options={})
         return self
 
     def groupby(self, keys: KeySet) -> "GroupedQueryBuilder":
         """Groups the query by the given set of keys, returning a GroupedQueryBuilder.
 
@@ -1531,15 +1533,15 @@
             ... )
             >>> answer.toPandas()
                count
             0      3
 
         Args:
             name: Name for the resulting aggregation column. Defaults to "count".
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).count(name=name, mechanism=mechanism)
 
     def count_distinct(
         self,
         columns: Optional[List[str]] = None,
@@ -1614,15 +1616,15 @@
 
         Args:
             columns: Columns in which to count distinct values. If none are provided,
                 the query will count every distinct row.
             name: Name for the resulting aggregation column. Defaults to
                 "count_distinct" if no columns are provided, or
                 "count_distinct(A, B, C)" if the provided columns are A, B, and C.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
             cols: Deprecated; use ``columns`` instead.
         """
         return self.groupby(KeySet.from_dict({})).count_distinct(
             columns=columns, name=name, mechanism=mechanism, cols=cols
         )
 
@@ -1633,19 +1635,18 @@
         low: float,
         high: float,
         name: Optional[str] = None,
     ) -> QueryExpr:
         """Returns a quantile query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
-
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1705,18 +1706,18 @@
 
     def min(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a minimum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1774,18 +1775,18 @@
 
     def max(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a maximum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1843,18 +1844,18 @@
 
     def median(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a median value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1918,18 +1919,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: SumMechanism = SumMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a sum query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -1984,15 +1985,15 @@
         Args:
             column: The column to compute the sum over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_sum"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).sum(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
     def average(
@@ -2002,18 +2003,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: AverageMechanism = AverageMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns an average query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2068,15 +2069,15 @@
         Args:
             column: The column to compute the average over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_average"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).average(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
     def variance(
@@ -2086,18 +2087,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: VarianceMechanism = VarianceMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a variance query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2152,15 +2153,15 @@
         Args:
             column: The column to compute the variance over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_variance"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).variance(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
     def stdev(
@@ -2170,18 +2171,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: StdevMechanism = StdevMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a standard deviation query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~drop_null_and_nan` query will be performed first. If the
+            column being measured contains infinite values, a
+            :meth:`~drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2236,15 +2237,15 @@
         Args:
             column: The column to compute the stdev over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_stdev"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         return self.groupby(KeySet.from_dict({})).stdev(
             column=column, low=low, high=high, name=name, mechanism=mechanism
         )
 
 
@@ -2320,15 +2321,15 @@
             >>> answer.sort("A").toPandas()
                A  count
             0  0      1
             1  1      2
 
         Args:
             name: Name for the resulting aggregation column. Defaults to "count".
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = "count"
         query_expr = GroupByCount(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -2396,15 +2397,15 @@
 
         Args:
             columns: Columns in which to count distinct values. If none are provided,
                 the query will count every distinct row.
             name: Name for the resulting aggregation column. Defaults to
                 "count_distinct" if no columns are provided, or
                 "count_distinct(A, B, C)" if the provided columns are A, B, and C.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
             cols: Deprecated; use ``columns`` instead.
         """
         if cols is not None:
             warnings.warn(
                 "The `cols` argument is deprecated; use `columns` instead",
                 DeprecationWarning,
@@ -2439,18 +2440,18 @@
         low: float,
         high: float,
         name: Optional[str] = None,
     ) -> QueryExpr:
         """Returns a quantile query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2521,18 +2522,18 @@
 
     def min(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a minimum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2596,18 +2597,18 @@
 
     def max(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a maximum value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2671,18 +2672,18 @@
 
     def median(
         self, column: str, low: float, high: float, name: Optional[str] = None
     ) -> QueryExpr:
         """Returns a quantile query requesting a median value, ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -2748,18 +2749,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: SumMechanism = SumMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a sum query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a ``drop_null_and_nan`` query will be performed first. If the column being
-            measured contains infinite values, a ``drop_infinity`` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2816,15 +2817,15 @@
         Args:
             column: The column to compute the sum over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_sum"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_sum"
         query_expr = GroupByBoundedSum(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -2843,18 +2844,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: AverageMechanism = AverageMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns an average query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a `drop_null_and_nan` query will be performed first. If the column being
-            measured contains infinite values, a `drop_infinity` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -2911,15 +2912,15 @@
         Args:
             column: The column to compute the average over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_average"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_average"
         query_expr = GroupByBoundedAverage(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -2938,18 +2939,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: VarianceMechanism = VarianceMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a variance query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a `drop_null_and_nan` query will be performed first. If the column being
-            measured contains infinite values, a `drop_infinity` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -3006,15 +3007,15 @@
         Args:
             column: The column to compute the variance over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_variance"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_variance"
         query_expr = GroupByBoundedVariance(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
@@ -3033,18 +3034,18 @@
         high: float,
         name: Optional[str] = None,
         mechanism: StdevMechanism = StdevMechanism.DEFAULT,
     ) -> QueryExpr:
         """Returns a standard deviation query that is ready to be evaluated.
 
         .. note::
-            If the column being measured contains NaN or null values,
-            a `drop_null_and_nan` query will be performed first. If the column being
-            measured contains infinite values, a `drop_infinity` query will be
-            performed first.
+            If the column being measured contains NaN or null values, a
+            :meth:`~QueryBuilder.drop_null_and_nan` query will be performed
+            first. If the column being measured contains infinite values, a
+            :meth:`~QueryBuilder.drop_infinity` query will be performed first.
 
         .. note::
             Regarding the clamping bounds:
 
             #. The values for ``low`` and ``high`` are a choice the caller must make.
             #. All data will be clamped to lie within this range.
             #. The narrower the range, the less noise. Larger bounds mean more data \
@@ -3101,15 +3102,15 @@
         Args:
             column: The column to compute the stdev over.
             low: The lower bound for clamping.
             high: The upper bound for clamping. Must be such that ``low``
                 is less than ``high``.
             name: The name to give the resulting aggregation column. Defaults to
                 ``f"{column}_stdev"``.
-            mechanism: Choice of noise mechanism. By DEFAULT, the framework
+            mechanism: Choice of noise mechanism. By default, the framework
                 automatically selects an appropriate mechanism.
         """
         if name is None:
             name = f"{column}_stdev"
         query_expr = GroupByBoundedSTDEV(
             child=self._query_expr,
             groupby_keys=self._groupby_keys,
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.7.1/tmlt/analytics/query_expr.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/session.py` & `tmlt_analytics-0.7.1/tmlt/analytics/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,48 @@
 
 More details on the exact privacy promise provided by :class:`Session` can be
 found in the :ref:`Privacy promise topic guide <Privacy promise>`.
 """
 
 # Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
+from operator import xor
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union, cast
 from warnings import warn
 
 import pandas as pd  # pylint: disable=unused-import
 import sympy as sp
 from pyspark.sql import SparkSession  # pylint: disable=unused-import
 from pyspark.sql import DataFrame
+from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.measurements.base import Measurement
+from tmlt.core.measurements.interactive_measurements import (
+    InactiveAccountantError,
+    InsufficientBudgetError,
+    PrivacyAccountant,
+    PrivacyAccountantState,
+    SequentialComposition,
+)
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.metrics import AddRemoveKeys as AddRemoveKeysMetric
+from tmlt.core.metrics import (
+    DictMetric,
+    IfGroupedBy,
+    RootSumOfSquared,
+    SumOf,
+    SymmetricDifference,
+)
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.dictionary import CreateDictFromValue
+from tmlt.core.transformations.identity import Identity
+from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
+from tmlt.core.utils.configuration import SparkConfigError, check_java11
+from tmlt.core.utils.exact_number import ExactNumber
+from tmlt.core.utils.type_utils import assert_never
 from typeguard import check_type, typechecked
 
 from tmlt.analytics._catalog import Catalog, PrivateTable, PublicTable
 from tmlt.analytics._coerce_spark_schema import (
     SUPPORTED_SPARK_TYPES,
     TYPE_COERCION_MAP,
     coerce_spark_schema_or_fail,
@@ -63,14 +90,15 @@
 from tmlt.analytics._transformation_utils import (
     delete_table,
     get_table_from_ref,
     persist_table,
     rename_table,
     unpersist_table,
 )
+from tmlt.analytics._type_checking import is_exact_number_tuple
 from tmlt.analytics.constraints import Constraint, MaxGroupsPerID
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
     PrivacyBudget,
     PureDPBudget,
     RhoZCDPBudget,
 )
@@ -79,40 +107,14 @@
     AddMaxRowsInMaxGroups,
     AddOneRow,
     AddRowsWithID,
     ProtectedChange,
 )
 from tmlt.analytics.query_builder import ColumnType, QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
-from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
-from tmlt.core.measurements.base import Measurement
-from tmlt.core.measurements.interactive_measurements import (
-    InactiveAccountantError,
-    InsufficientBudgetError,
-    PrivacyAccountant,
-    PrivacyAccountantState,
-    SequentialComposition,
-)
-from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
-from tmlt.core.metrics import AddRemoveKeys as AddRemoveKeysMetric
-from tmlt.core.metrics import (
-    DictMetric,
-    IfGroupedBy,
-    RootSumOfSquared,
-    SumOf,
-    SymmetricDifference,
-)
-from tmlt.core.transformations.base import Transformation
-from tmlt.core.transformations.dictionary import CreateDictFromValue
-from tmlt.core.transformations.identity import Identity
-from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
-from tmlt.core.utils.configuration import SparkConfigError, check_java11
-from tmlt.core.utils.exact_number import ExactNumber
-from tmlt.core.utils.type_utils import assert_never
 
 __all__ = ["Session", "SUPPORTED_SPARK_TYPES", "TYPE_COERCION_MAP"]
 
 
 class _PrivateSourceTuple(NamedTuple):
     """Named tuple of private Dataframe, domain and protected change."""
 
@@ -238,17 +240,17 @@
             :data:`SUPPORTED_SPARK_TYPES` for information about which types are
             supported.
 
             Args:
                 source_id: Source id for the private source dataframe.
                 dataframe: Private source dataframe to perform queries on,
                     corresponding to the ``source_id``.
-                stability: Use ``protected_change`` instead, see
+                stability: Deprecated: use ``protected_change`` instead, see
                     :ref:`changelog<changelog#protected-change>`.
-                grouping_column: Use ``protected_change`` instead, see
+                grouping_column: Deprecated: use ``protected_change`` instead, see
                     :ref:`changelog<changelog#protected-change>`.
                 protected_change: A
                     :class:`~tmlt.analytics.protected_change.ProtectedChange`
                     specifying what changes to the input data the resulting
                     :class:`Session` should protect.
             """
             _assert_is_identifier(source_id)
@@ -269,29 +271,30 @@
                         " protected_change."
                     )
                 self._private_sources[source_id] = _PrivateSourceTuple(
                     dataframe, protected_change, domain
                 )
                 return self
 
-            # TODO(#2722): All paths through the below need deprecation
-            #     warnings, for either the use of stability/grouping_column or
-            #     the assumption of AddOneRow() if no stability is specified.
             if stability is None:
                 warn(
-                    "Using a default for protected_change is deprecated. Future"
-                    " code should explicitly specify protected_change=AddOneRow()",
+                    (
+                        "Using a default for protected_change is deprecated. Future"
+                        " code should explicitly specify protected_change=AddOneRow()"
+                    ),
                     DeprecationWarning,
                 )
                 if grouping_column is None:
                     protected_change = AddOneRow()
                 else:
                     warn(
-                        "Providing a grouping_column parameter instead of a"
-                        " protected_change parameter is deprecated",
+                        (
+                            "Providing a grouping_column parameter instead of a"
+                            " protected_change parameter is deprecated"
+                        ),
                         DeprecationWarning,
                     )
                     protected_change = AddMaxRowsInMaxGroups(grouping_column, 1, 1)
                     grouping_column = None
             else:
                 warn(
                     "Providing a stability instead of a protected_change is deprecated",
@@ -305,16 +308,18 @@
                         raise ValueError(
                             "stability must be an integer when no grouping column is"
                             " specified"
                         )
                     protected_change = AddMaxRows(stability)
                 else:
                     warn(
-                        "Providing a grouping_column parameter instead of a"
-                        " protected_change parameter is deprecated",
+                        (
+                            "Providing a grouping_column parameter instead of a"
+                            " protected_change parameter is deprecated"
+                        ),
                         DeprecationWarning,
                     )
                     if not isinstance(stability, (int, float)):
                         raise ValueError("stability must be a numeric value")
                     protected_change = AddMaxRowsInMaxGroups(
                         grouping_column, max_groups=1, max_rows_per_group=stability
                     )
@@ -342,22 +347,24 @@
             if source_id in self._private_sources or source_id in self._public_sources:
                 raise ValueError(f"Duplicate source id: '{source_id}'")
             dataframe = coerce_spark_schema_or_fail(dataframe)
             self._public_sources[source_id] = dataframe
             return self
 
         def with_id_space(self, id_space: str) -> "Session.Builder":
-            """Sets the identifier space for the session.
+            """Creates an identifier space for the session.
 
-            This defines the space of identifiers that map 1-to-1 to the identifiers
-            being protected. Any IDs table must have exactly one column containing
-            those identifiers.
+            This defines a space of identifiers that map 1-to-1 to the
+            identifiers being protected by a table with the
+            :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected
+            change. Any table with such a protected change must be a member of
+            some identifier space.
 
             Args:
-                id_space: The identifier space for the session.
+                id_space: The name of the identifier space.
             """
             _assert_is_identifier(id_space)
             if id_space in self._id_spaces:
                 raise ValueError(
                     f"This Builder already has an ID space of the name: {id_space}."
                 )
             self._id_spaces.append(id_space)
@@ -398,22 +405,17 @@
             ) from exc
 
         check_type("accountant", accountant, PrivacyAccountant)
         check_type("public_sources", public_sources, Dict[str, DataFrame])
         check_type("compiler", compiler, Optional[QueryExprCompiler])
 
         self._accountant = accountant
-        if isinstance(self._accountant.output_measure, ApproxDP):
-            raise ValueError(
-                "Accountant is using ApproxDP, which is not yet supported. This is"
-                " probably a bug, please let us know so we can fix it!"
-            )
 
-        if not isinstance(self._accountant.output_measure, (PureDP, RhoZCDP)):
-            raise ValueError("Accountant is not using PureDP or RhoZCDP.")
+        if not isinstance(self._accountant.output_measure, (PureDP, ApproxDP, RhoZCDP)):
+            raise ValueError("Accountant is not using PureDP, ApproxDP, or RhoZCDP.")
         if not isinstance(self._accountant.input_metric, DictMetric):
             raise ValueError("The input metric to a session must be a DictMetric.")
         if not isinstance(self._accountant.input_domain, DictDomain):
             raise ValueError("The input domain to a session must be a DictDomain.")
         self._public_sources = public_sources
         if compiler is None:
             compiler = QueryExprCompiler(output_measure=self._accountant.output_measure)
@@ -480,17 +482,17 @@
             {'A': 'VARCHAR', 'B': 'INTEGER', 'X': 'INTEGER'}
 
         Args:
             privacy_budget: The total privacy budget allocated to this session.
             source_id: The source id for the private source dataframe.
             dataframe: The private source dataframe to perform queries on,
                 corresponding to the `source_id`.
-            stability: Use ``protected_change`` instead, see
+            stability: Deprecated: use ``protected_change`` instead, see
                 :ref:`changelog<changelog#protected-change>`
-            grouping_column: Use ``protected_change`` instead, see
+            grouping_column: Deprecated: use ``protected_change`` instead, see
                 :ref:`changelog<changelog#protected-change>`
             protected_change: A
                 :class:`~tmlt.analytics.protected_change.ProtectedChange`
                 specifying what changes to the input data the resulting
                 :class:`Session` should protect.
         """
         # pylint: enable=line-too-long
@@ -521,45 +523,46 @@
 
         Args:
             privacy_budget: The total privacy budget allocated to this session.
             private_sources: The private data to be used in the session.
                 Provided as a dictionary {source_id: Dataframe}.
             relation: the :class:`NeighboringRelation` to be used in the session.
         """
-        output_measure: Union[ApproxDP, PureDP, RhoZCDP]
+        # pylint: disable=protected-access
+        output_measure: Union[PureDP, ApproxDP, RhoZCDP]
         sympy_budget: sp.Expr
         if isinstance(privacy_budget, PureDPBudget):
             output_measure = PureDP()
-            sympy_budget = ExactNumber.from_float(
-                privacy_budget.epsilon, round_up=False
-            ).expr
+            sympy_budget = privacy_budget._epsilon.expr
         elif isinstance(privacy_budget, ApproxDPBudget):
-            output_measure = PureDP()
+            output_measure = ApproxDP()
             if privacy_budget.is_infinite:
                 warn(
-                    "The use of ApproxDP is not yet fully supported. Because you"
-                    " selected an infinite ApproxDP budget, your session will be"
-                    " initialized with PureDP using an infinite epsilon budget.",
+                    (
+                        "The use of ApproxDP is not yet fully supported. Because you"
+                        " selected an infinite ApproxDP budget, your session will be"
+                        " initialized with PureDP using an infinite epsilon budget."
+                    ),
                     UserWarning,
                 )
-                sympy_budget = ExactNumber.from_float(float("inf"), round_up=False).expr
+                sympy_budget = (
+                    ExactNumber.from_float(float("inf"), round_up=False).expr,
+                    0,
+                )
             else:
                 warn(
                     "The use of ApproxDP is not yet fully supported. Your session"
                     " will be initialized with PureDP using the epsilon provided.",
                     UserWarning,
                 )
-                sympy_budget = ExactNumber.from_float(
-                    privacy_budget.epsilon, round_up=False
-                ).expr
+                sympy_budget = (privacy_budget._epsilon.expr, 0)
         elif isinstance(privacy_budget, RhoZCDPBudget):
             output_measure = RhoZCDP()
-            sympy_budget = ExactNumber.from_float(
-                privacy_budget.rho, round_up=False
-            ).expr
+            sympy_budget = privacy_budget._rho.expr
+        # pylint: enable=protected-access
         else:
             raise ValueError(
                 f"Unsupported PrivacyBudget variant: {type(privacy_budget)}"
             )
         # ensure we have a valid source dict for the NeighboringRelation,
         # raising exception if not.
         relation.validate_input(private_sources)
@@ -599,34 +602,31 @@
 
     @property
     def public_source_dataframes(self) -> Dict[str, DataFrame]:
         """Returns a dictionary of public source dataframes."""
         return self._public_sources
 
     @property
-    def remaining_privacy_budget(self) -> Union[PureDPBudget, RhoZCDPBudget]:
+    def remaining_privacy_budget(self) -> PrivacyBudget:
         """Returns the remaining privacy_budget left in the session.
 
         The type of the budget (e.g., PureDP or rho-zCDP) will be the same as
         the type of the budget the Session was initialized with.
         """
         output_measure = self._accountant.output_measure
-        if isinstance(output_measure, ApproxDP):
-            raise ValueError(
-                "Accountant is using ApproxDP, which is not yet supported. This is"
-                " probably a bug, please let us know so we can fix it!"
-            )
+        privacy_budget_value = self._accountant.privacy_budget
 
-        sympy_budget = self._accountant.privacy_budget
-        budget_value = ExactNumber(sympy_budget).to_float(round_up=False)
-
-        if output_measure == PureDP():
-            return PureDPBudget(budget_value)
-        if output_measure == RhoZCDP():
-            return RhoZCDPBudget(budget_value)
+        # mypy doesn't know that the ApproxDP budget is a tuple and PureDP and RhoZCDP are not
+        if output_measure == ApproxDP():
+            epsilon_budget_value, delta_budget_value = privacy_budget_value  # type: ignore
+            return ApproxDPBudget(epsilon_budget_value, delta_budget_value)
+        elif output_measure == PureDP():
+            return PureDPBudget(privacy_budget_value)  # type: ignore
+        elif output_measure == RhoZCDP():
+            return RhoZCDPBudget(privacy_budget_value)  # type: ignore
         raise RuntimeError(
             "Unexpected behavior in remaining_privacy_budget. Please file a bug report."
         )
 
     @property
     def _input_domain(self) -> DictDomain:
         """Returns the input domain of the underlying queryable."""
@@ -645,14 +645,126 @@
             raise AssertionError(
                 "Session accountant's input metric has an incorrect type. This is "
                 "probably a bug; please let us know about it so we can "
                 "fix it!"
             )
         return self._accountant.input_metric
 
+    def describe(
+        self, obj: Optional[Union[QueryExpr, QueryBuilder, str]] = None
+    ) -> None:
+        """Describe a Session, table, or query.
+
+        If ``obj`` is not specified, ``session.describe()`` will describe the
+        Session and all of the tables it contains.
+
+        If ``obj`` is a :class:`~tmlt.analytics.query_builder.QueryBuilder` or
+        :class:`~tmlt.analytics.query_expr.QueryExpr`, ``session.describe(obj)``
+        will describe the table that would result from that query if it were
+        applied to the Session.
+
+        If ``obj`` is a string, ``session.describe(obj)`` will describe the table
+        with that name. This is a shorthand for
+        ``session.describe(QueryBuilder(obj))``.
+
+        Args:
+            obj: The table or query to be described, or None to describe the
+                whole Session.
+        """
+        if obj is None:
+            self._describe_self()
+        elif isinstance(obj, QueryExpr):
+            self._describe_query(obj)
+        elif isinstance(obj, QueryBuilder):
+            self._describe_query(obj.query_expr)
+        elif isinstance(obj, str):
+            self._describe_query(QueryBuilder(obj).query_expr)
+        else:
+            assert_never(obj)
+
+    def _describe_self(self) -> None:
+        """Describe the current state of this session."""
+        out = []
+        state = self._accountant.state
+        if state == PrivacyAccountantState.ACTIVE:
+            # Don't add anything to output if the session is active
+            pass
+        elif state == PrivacyAccountantState.RETIRED:
+            out.append("This session has been stopped, and can no longer be used.")
+        elif state == PrivacyAccountantState.WAITING_FOR_CHILDREN:
+            out.append(
+                "This session is waiting for its children (created with"
+                " `partition_and_create`) to finish."
+            )
+        elif state == PrivacyAccountantState.WAITING_FOR_SIBLING:
+            out.append(
+                "This session is waiting for its sibling(s) (created with"
+                " `partition_and_create`) to finish."
+            )
+        else:
+            raise AssertionError(
+                f"Unrecognized accountant state {out}. This is probably a bug; please"
+                " let us know about it so we can fix it!"
+            )
+        budget: PrivacyBudget = self.remaining_privacy_budget
+        out.append(f"The session has a remaining privacy budget of {budget}.")
+        if len(self._catalog.tables) == 0:
+            out.append("The session has no tables available.")
+        else:
+            public_table_descs = []
+            private_table_descs = []
+            for name, table in self._catalog.tables.items():
+                column_strs = ["\t" + e for e in _describe_schema(table.schema)]
+                columns_desc = "\n".join(column_strs)
+                if isinstance(table, PublicTable):
+                    table_desc = f"Public table '{name}':\n" + columns_desc
+                    public_table_descs.append(table_desc)
+                elif isinstance(table, PrivateTable):
+                    table_desc = f"Table '{name}':\n"
+                    table_desc += columns_desc
+
+                    constraints: Optional[
+                        List[Constraint]
+                    ] = self._table_constraints.get(NamedTable(name))
+                    if not constraints:
+                        table_desc = (
+                            f"Table '{name}' (no constraints):\n" + columns_desc
+                        )
+                    else:
+                        table_desc = (
+                            f"Table '{name}':\n" + columns_desc + "\n\tConstraints:\n"
+                        )
+                        constraints_strs = [f"\t\t- {e}" for e in constraints]
+                        table_desc += "\n".join(constraints_strs)
+
+                    private_table_descs.append(table_desc)
+                else:
+                    raise AssertionError(
+                        f"Table {name} has an unrecognized type: {type(table)}. This is"
+                        " probably a bug; please let us know about it so we can"
+                        " fix it!"
+                    )
+            if len(private_table_descs) != 0:
+                out.append(
+                    "The following private tables are available:\n"
+                    + "\n".join(private_table_descs)
+                )
+            if len(public_table_descs) != 0:
+                out.append(
+                    "The following public tables are available:\n"
+                    + "\n".join(public_table_descs)
+                )
+        print("\n".join(out))
+
+    def _describe_query(self, query: QueryExpr):
+        """Describe the output schema of a query and the constraints on it."""
+        schema = self._compiler.query_schema(query, self._catalog)
+        out = _describe_schema(schema)
+        print("\n".join(out))
+
     @typechecked
     def get_schema(self, source_id: str) -> Schema:
         """Returns the schema for any data source.
 
         This includes information on whether the columns are nullable.
 
         Args:
@@ -854,28 +966,34 @@
         if source_id in self.public_sources or source_id in self.private_sources:
             raise ValueError(f"This session already has a table named '{source_id}'.")
         dataframe = coerce_spark_schema_or_fail(dataframe)
         self._public_sources[source_id] = dataframe
 
     def _compile_and_get_budget(
         self, query_expr: QueryExpr, privacy_budget: PrivacyBudget
-    ) -> Tuple[Measurement, ExactNumber]:
+    ) -> Tuple[Measurement, PrivacyBudget]:
         """Pre-processing needed for evaluate() and _noise_info()."""
         check_type("query_expr", query_expr, QueryExpr)
         check_type("privacy_budget", privacy_budget, PrivacyBudget)
 
+        is_approxDP_session = self._accountant.output_measure == ApproxDP()
+
+        # If pureDP session, and approxDP budget, let Core handle the error.
+        if is_approxDP_session and isinstance(privacy_budget, PureDPBudget):
+            privacy_budget = ApproxDPBudget(privacy_budget.epsilon, 0)
+
         self._validate_budget_type_matches_session(privacy_budget)
         if privacy_budget in [PureDPBudget(0), ApproxDPBudget(0, 0), RhoZCDPBudget(0)]:
             raise ValueError("You need a non-zero privacy budget to evaluate a query.")
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
 
         measurement = self._compiler(
             queries=[query_expr],
-            privacy_budget=adjusted_budget.expr,
+            privacy_budget=adjusted_budget,
             stability=self._accountant.d_in,
             input_domain=self._input_domain,
             input_metric=self._input_metric,
             public_sources=self._public_sources,
             catalog=self._catalog,
             table_constraints=self._table_constraints,
         )
@@ -978,66 +1096,103 @@
         """
         # pylint: enable=line-too-long
         measurement, adjusted_budget = self._compile_and_get_budget(
             query_expr, privacy_budget
         )
         self._activate_accountant()
 
+        # check if type of self._accountant.privacy_budget matches adjusted_budget value
+        if xor(
+            isinstance(self._accountant.privacy_budget, tuple),
+            isinstance(adjusted_budget.value, tuple),
+        ):
+            raise ValueError(
+                "Expected type of adjusted_budget to match type of accountant's privacy"
+                f" budget ({type(self._accountant.privacy_budget)}), but instead"
+                f" received {type(adjusted_budget.value)}. This is probably a bug;"
+                " please let us know about it so we can fix it!"
+            )
+
         try:
-            if not measurement.privacy_relation(self._accountant.d_in, adjusted_budget):
-                raise ValueError(
-                    "With these inputs and this privacy budget, "
-                    "similar inputs will *not* produce similar outputs. "
+            if not measurement.privacy_relation(
+                self._accountant.d_in, adjusted_budget.value
+            ):
+                raise AssertionError(
+                    "With these inputs and this privacy budget, similar inputs will"
+                    " *not* produce similar outputs. This is probably a bug; please let"
+                    " us know about it so we can fix it!"
                 )
             try:
-                answers = self._accountant.measure(measurement, d_out=adjusted_budget)
-            except InsufficientBudgetError:
-                if not isinstance(self._accountant.privacy_budget, ExactNumber):
-                    raise ValueError(
-                        "Expected privacy_budget to be an ExactNumber, but instead"
-                        f" received {type(self._accountant.privacy_budget)}."
-                    )
+                answers = self._accountant.measure(
+                    measurement, d_out=adjusted_budget.value
+                )
+            # TODO #2476: Parse InsufficientBudgetError based on budget type
+            except InsufficientBudgetError as e:
+                # pylint: disable=protected-access
+                if isinstance(adjusted_budget, (PureDPBudget)):
+                    approximate_budget_needed = adjusted_budget._epsilon
+                elif isinstance(adjusted_budget, (ApproxDPBudget)):
+                    approximate_budget_needed = adjusted_budget._epsilon
+                elif isinstance(adjusted_budget, RhoZCDPBudget):
+                    approximate_budget_needed = adjusted_budget._rho
+                # pylint: enable=protected-access
+                else:
+                    raise AssertionError(
+                        "Unable to convert privacy budget of"
+                        f" {adjusted_budget} to float or floats. This"
+                        " is probably a bug; please let us know about it so we can"
+                        " fix it!"
+                    ) from e
 
-                approximate_budget_needed = adjusted_budget.to_float(round_up=True)
-                if not isinstance(self._accountant.privacy_budget, ExactNumber):
+                # mypy doesn't know we just checked for Tuple[ExactNumber, ExactNumber]
+                if is_exact_number_tuple(self._accountant.privacy_budget):
+                    # pylint: disable=line-too-long
+                    approximate_budget_left = self._accountant.privacy_budget[0]  # type: ignore
+                elif isinstance(self._accountant.privacy_budget, ExactNumber):
+                    approximate_budget_left = self._accountant.privacy_budget
+                else:
                     raise AssertionError(
                         "Unable to convert privacy budget of"
-                        f" {self._accountant.privacy_budget} to float. This is probably"
-                        " a bug; please let us know about it so we can fix it!"
-                    )
-                approximate_budget_left = self._accountant.privacy_budget.to_float(
+                        f" {self._accountant.privacy_budget} to float or floats. This"
+                        " is probably a bug; please let us know about it so we can"
+                        " fix it!"
+                    ) from e
+
+                approximate_diff = abs(
+                    approximate_budget_left - approximate_budget_needed
+                ).to_float(round_up=False)
+                readable_approximate_budget_needed = approximate_budget_needed.to_float(
                     round_up=False
                 )
-                approximate_diff = abs(
-                    (self._accountant.privacy_budget - adjusted_budget).to_float(
-                        round_up=True
-                    )
+                readable_approximate_budget_left = approximate_budget_left.to_float(
+                    round_up=False
                 )
+
                 raise RuntimeError(
                     "Cannot answer query without exceeding privacy budget: it needs"
-                    f" approximately {approximate_budget_needed:.3f}, but the remaining"
-                    " budget is approximately"
-                    f" {approximate_budget_left:.3f} (difference:"
+                    f" approximately {readable_approximate_budget_needed:.3f}, but the"
+                    " remaining budget is approximately"
+                    f" {readable_approximate_budget_left:.3f} (difference:"
                     f" {approximate_diff:.3e})"
-                )
+                ) from e
             if len(answers) != 1:
                 raise AssertionError(
                     "Expected exactly one answer, but got "
                     f"{len(answers)} answers instead. This is "
                     "probably a bug; please let us know about it so "
                     "we can fix it!"
                 )
             return answers[0]
-        except InactiveAccountantError:
+        except InactiveAccountantError as e:
             raise RuntimeError(
                 "This session is no longer active. Either it was manually stopped "
                 "with session.stop(), or it was stopped indirectly by the "
                 "activity of other sessions. See partition_and_create "
                 "for more information."
-            )
+            ) from e
 
     # pylint: disable=line-too-long
     @typechecked
     def create_view(
         self, query_expr: Union[QueryExpr, QueryBuilder], source_id: str, cache: bool
     ):
         """Create a new view from a transformation and possibly cache it.
@@ -1175,17 +1330,19 @@
         source_id: str,
         privacy_budget: PrivacyBudget,
         column: Optional[str] = None,
         splits: Optional[Union[Dict[str, str], Dict[str, int]]] = None,
     ) -> Dict[str, "Session"]:
         """Returns new sessions from a partition mapped to split name/``source_id``.
 
-        The type of privacy budget that you use must match the type your Session was
-        initialized with (i.e., you cannot use a RhoZCDPBudget to partition your
-        Session if the Session was created using a PureDPBudget, and vice versa).
+        The type of privacy budget that you use must match the type your Session
+        was initialized with (i.e., you cannot use a
+        :class:`~tmlt.analytics.privacy_budget.RhoZCDPBudget` to partition your
+        Session if the Session was created using a
+        :class:`~tmlt.analytics.privacy_budget.PureDPBudget`, and vice versa).
 
         The sessions returned must be used in the order that they were created.
         Using this session again or calling stop() will stop all partition sessions.
 
         ..
             >>> # Get data
             >>> spark = SparkSession.builder.getOrCreate()
@@ -1268,14 +1425,29 @@
             )
         # If you remove this if-block, mypy will complain
         if column is None:
             raise AssertionError(
                 "column is None, even though either column or attr_name were provided."
                 " This is probably a bug; please let us know about it so we can fix it!"
             )
+
+        if not (
+            isinstance(self._accountant.privacy_budget, ExactNumber)
+            or is_exact_number_tuple(self._accountant.privacy_budget)
+        ):
+            raise AssertionError(
+                "Unable to convert privacy budget of type"
+                f" {type(self._accountant.privacy_budget)} to float or floats. This is"
+                " probably a bug; please let us know about it so we can fix it!"
+            )
+
+        is_approxDP_session = isinstance(self._accountant.output_measure, ApproxDP)
+        if is_approxDP_session and isinstance(privacy_budget, PureDPBudget):
+            privacy_budget = ApproxDPBudget(privacy_budget.epsilon, 0)
+
         self._validate_budget_type_matches_session(privacy_budget)
         self._activate_accountant()
 
         transformation: Transformation = Identity(
             domain=self._input_domain, metric=self._input_metric
         )
         table_ref = find_reference(source_id, self._input_domain)
@@ -1326,20 +1498,20 @@
                 "Transformation has an unrecognized output metric. This is "
                 "probably a bug; please let us know about it so we can fix it!"
             )
         transformation_domain = cast(SparkDataFrameDomain, transformation.output_domain)
 
         try:
             attr_type = transformation_domain.schema[column]
-        except KeyError:
+        except KeyError as e:
             raise KeyError(
                 f"'{column}' not present in transformed dataframe's columns; "
                 "schema of transformed dataframe is "
                 f"{spark_dataframe_domain_to_analytics_columns(transformation_domain)}"
-            )
+            ) from e
 
         new_sources = []
         # Actual type is Union[List[Tuple[str, ...]], List[Tuple[int, ...]]]
         # but mypy doesn't like that.
         split_vals: List[Tuple[Union[str, int], ...]] = []
         for split_name, split_val in splits.items():
             if not split_name.isidentifier():
@@ -1392,52 +1564,71 @@
         )
         chained_partition = transformation | partition_transformation
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
 
         try:
             new_accountants = self._accountant.split(
-                chained_partition, privacy_budget=adjusted_budget
+                chained_partition, privacy_budget=adjusted_budget.value
             )
-        except InactiveAccountantError:
+        except InactiveAccountantError as e:
             raise RuntimeError(
                 "This session is no longer active. Either it was manually stopped"
                 "with session.stop(), or it was stopped indirectly by the "
                 "activity of other sessions. See partition_and_create "
                 "for more information."
-            )
-        except InsufficientBudgetError:
-            if not isinstance(self._accountant.privacy_budget, ExactNumber):
-                raise ValueError(
-                    "Expected privacy_budget to be an ExactNumber, but instead"
-                    f" received {type(self._accountant.privacy_budget)}."
-                )
-
-            approximate_budget_needed = adjusted_budget.to_float(round_up=True)
-            if not isinstance(self._accountant.privacy_budget, ExactNumber):
+            ) from e
+        # TODO #2476: Parse InsufficientBudgetError based on budget type
+        except InsufficientBudgetError as e:
+            # pylint: disable=protected-access
+            if isinstance(adjusted_budget, (PureDPBudget)):
+                approximate_budget_needed = adjusted_budget._epsilon
+            elif isinstance(adjusted_budget, (ApproxDPBudget)):
+                approximate_budget_needed = adjusted_budget._epsilon
+            elif isinstance(adjusted_budget, RhoZCDPBudget):
+                approximate_budget_needed = adjusted_budget._rho
+            # pylint: enable=protected-access
+            else:
                 raise AssertionError(
                     "Unable to convert privacy budget of"
-                    f" {self._accountant.privacy_budget} to float. This is probably a"
-                    " bug; please let us know about it so we can fix it!"
-                )
+                    f" {adjusted_budget} to float or floats. This"
+                    " is probably a bug; please let us know about it so we can"
+                    " fix it!"
+                ) from e
+            # mypy doesn't know we just checked for Tuple[ExactNumber, ExactNumber]
+            if is_exact_number_tuple(self._accountant.privacy_budget):
+                # pylint: disable-next=line-too-long
+                approximate_budget_left = self._accountant.privacy_budget[0]  # type: ignore
+            elif isinstance(self._accountant.privacy_budget, ExactNumber):
+                approximate_budget_left = self._accountant.privacy_budget
+            else:
+                raise AssertionError(
+                    "Unable to convert privacy budget of"
+                    f" {self._accountant.privacy_budget} to float or floats. This"
+                    " is probably a bug; please let us know about it so we can"
+                    " fix it!"
+                ) from e
 
-            approximate_budget_left = self._accountant.privacy_budget.to_float(
+            approximate_diff = abs(
+                approximate_budget_left - approximate_budget_needed
+            ).to_float(round_up=False)
+            readable_approximate_budget_needed = approximate_budget_needed.to_float(
                 round_up=False
             )
-            approximate_diff = abs(
-                (self._accountant.privacy_budget - adjusted_budget).to_float(
-                    round_up=True
-                )
+            readable_approximate_budget_left = approximate_budget_left.to_float(
+                round_up=False
             )
+
             raise RuntimeError(
                 "Cannot perform this partition without exceeding privacy budget: it"
-                f" needs approximately {approximate_budget_needed:.3f}, but the"
-                " remaining budget is approximately"
-                f" {approximate_budget_left:.3f} (difference: {approximate_diff:.3e})"
-            )
+                f" needs approximately {readable_approximate_budget_needed:.3f}, but"
+                " the remaining budget is approximately"
+                f" {readable_approximate_budget_left:.3f} (difference:"
+                f" {approximate_diff:.3e})"
+            ) from e
 
         for i, source in enumerate(new_sources):
             if table_has_ids:
                 create_dict = CreateDictFromValue(
                     input_domain=transformation_domain,
                     input_metric=element_metric,
                     key=NamedTable(source),
@@ -1455,55 +1646,78 @@
                     key=NamedTable(source),
                 )
 
             new_accountants[i].queue_transformation(
                 transformation=dict_transformation_wrapper
             )
 
-        new_sessions = dict()
+        new_sessions = {}
         for new_accountant, source in zip(new_accountants, new_sources):
             new_sessions[source] = Session(
                 new_accountant, self._public_sources, self._compiler
             )
         return new_sessions
 
-    def _process_requested_budget(self, privacy_budget: PrivacyBudget) -> ExactNumber:
+    def _process_requested_budget(self, privacy_budget: PrivacyBudget) -> PrivacyBudget:
         """Process the requested budget to accommodate floating point imprecision.
 
         Args:
             privacy_budget: The requested budget.
         """
-        remaining_budget = self._accountant.privacy_budget
-        if not isinstance(remaining_budget, ExactNumber):
-            raise AssertionError(
-                f"Cannot understand remaining budget of {remaining_budget}. This is"
-                " probably a bug; please let us know about it so we can fix it!"
-            )
-        if isinstance(privacy_budget, PureDPBudget):
-            return get_adjusted_budget(privacy_budget.epsilon, remaining_budget)
+        remaining_budget_value = self._accountant.privacy_budget
 
-        if isinstance(privacy_budget, ApproxDPBudget):
+        if isinstance(privacy_budget, PureDPBudget):
+            if not isinstance(remaining_budget_value, ExactNumber):
+                raise AssertionError(
+                    f"Cannot understand remaining budget of {remaining_budget_value}."
+                    " This is probably a bug; please let us know about it so we can"
+                    " fix it!"
+                )
+            return get_adjusted_budget(
+                privacy_budget,
+                PureDPBudget(remaining_budget_value.to_float(round_up=False)),
+            )
+        elif isinstance(privacy_budget, ApproxDPBudget):
+            # TODO #2476: Reverse this when we support consuming delta
             if privacy_budget.is_infinite:
-                warn(
-                    "The use of ApproxDP is not yet fully supported. Because you"
-                    " selected an infinite ApproxDP budget, your budget request"
-                    " will be processed as PureDP with an infinite epsilon budget.",
-                    UserWarning,
-                )
-                return ExactNumber.from_float(float("inf"), round_up=False)
+                return ApproxDPBudget(float("inf"), 0)
             else:
                 warn(
                     "The use of ApproxDP is not yet fully supported. your budget"
                     " request will be processed as PureDP using the epsilon"
                     " provided.",
                     UserWarning,
                 )
-                return get_adjusted_budget(privacy_budget.epsilon, remaining_budget)
+                if not is_exact_number_tuple(remaining_budget_value):
+                    raise AssertionError(
+                        "Remaining budget type for ApproxDP must be Tuple[ExactNumber,"
+                        " ExactNumber], but instead received"
+                        f" {type(remaining_budget_value)}. This is probably a bug;"
+                        " please let us know about it so we can fix it!"
+                    )
+                # mypy doesn't understand that we've already checked that this is a tuple
+                remaining_epsilon, remaining_delta = remaining_budget_value  # type: ignore
+                return get_adjusted_budget(
+                    ApproxDPBudget(privacy_budget.epsilon, 0),
+                    ApproxDPBudget(
+                        remaining_epsilon.to_float(round_up=False),
+                        remaining_delta.to_float(round_up=False),
+                    ),
+                )
         elif isinstance(privacy_budget, RhoZCDPBudget):
-            return get_adjusted_budget(privacy_budget.rho, remaining_budget)
+            if not isinstance(remaining_budget_value, ExactNumber):
+                raise AssertionError(
+                    f"Cannot understand remaining budget of {remaining_budget_value}."
+                    " This is probably a bug; please let us know about it so we can"
+                    " fix it!"
+                )
+            return get_adjusted_budget(
+                privacy_budget,
+                RhoZCDPBudget(remaining_budget_value.to_float(round_up=False)),
+            )
         else:
             raise ValueError(
                 f"Unsupported variant of PrivacyBudget. Found {type(privacy_budget)}"
             )
 
     def _validate_budget_type_matches_session(
         self, privacy_budget: PrivacyBudget
@@ -1513,24 +1727,24 @@
         Args:
             privacy_budget: The requested budget.
         """
         output_measure = self._accountant.output_measure
         matches_puredp = isinstance(output_measure, PureDP) and isinstance(
             privacy_budget, PureDPBudget
         )
-        matches_approxdp = isinstance(output_measure, PureDP) and isinstance(
+        matches_approxdp = isinstance(output_measure, ApproxDP) and isinstance(
             privacy_budget, ApproxDPBudget
         )
         matches_zcdp = isinstance(output_measure, RhoZCDP) and isinstance(
             privacy_budget, RhoZCDPBudget
         )
         if not (matches_puredp or matches_approxdp or matches_zcdp):
             raise ValueError(
-                "Your requested privacy budget type must match the type of the privacy"
-                " budget your Session was created with."
+                "Your requested privacy budget type must match the type of the"
+                " privacy budget your Session was created with."
             )
 
     def _activate_accountant(self) -> None:
         if self._accountant.state == PrivacyAccountantState.ACTIVE:
             return
         if self._accountant.state == PrivacyAccountantState.RETIRED:
             raise RuntimeError(
@@ -1549,125 +1763,14 @@
             )
         self._accountant.force_activate()
 
     def stop(self) -> None:
         """Close out this session, allowing other sessions to become active."""
         self._accountant.retire()
 
-    def describe(self, x: Optional[Union[QueryExpr, QueryBuilder, str]] = None) -> None:
-        """Describe this session, or a query, or a table.
-
-        If ``x`` is ``None``, ``session._describe(x)`` will describe the session.
-
-        If ``x`` is a
-        :class:`~tmlt.analytics.query_expr.QueryExpr`,
-        ``session._describe(x)`` will describe
-        the schema resulting from that query expression.
-
-        If x is a
-        :class:`~tmlt.analytics.query_builder.QueryBuilder`,
-        ``session._describe(x) will describe the query constructed by the
-        query builder. This is equivalent to calling
-        ``session._describe(x.query_expr)``.
-
-        If x is a string, x is assumed to be a table name. In this case,
-        ``session._describe(x)`` is equivalent to
-        ``session._describe(QueryBuilder(x))``.
-        """
-        if x is None:
-            self._describe_self()
-        elif isinstance(x, QueryExpr):
-            self._describe_query(x)
-        elif isinstance(x, QueryBuilder):
-            self._describe_query(x.query_expr)
-        elif isinstance(x, str):
-            self._describe_query(QueryBuilder(x).query_expr)
-        else:
-            assert_never(x)
-
-    def _describe_self(self) -> None:
-        """Describe the current state of this session."""
-        out = []
-        state = self._accountant.state
-        if state == PrivacyAccountantState.ACTIVE:
-            # Don't add anything to output if the session is active
-            pass
-        elif state == PrivacyAccountantState.RETIRED:
-            out.append("This session has been stopped, and can no longer be used.")
-        elif state == PrivacyAccountantState.WAITING_FOR_CHILDREN:
-            out.append(
-                "This session is waiting for its children (created with"
-                " `partition_and_create`) to finish."
-            )
-        elif state == PrivacyAccountantState.WAITING_FOR_SIBLING:
-            out.append(
-                "This session is waiting for its sibling(s) (created with"
-                " `partition_and_create`) to finish."
-            )
-        else:
-            raise AssertionError(
-                f"Unrecognized accountant state {out}. This is probably a bug; please"
-                " let us know about it so we can fix it!"
-            )
-        budget: PrivacyBudget = self.remaining_privacy_budget
-        out.append(f"The session has a remaining privacy budget of {budget}.")
-        if len(self._catalog.tables) == 0:
-            out.append("The session has no tables available.")
-        else:
-            public_table_descs = []
-            private_table_descs = []
-            for name, table in self._catalog.tables.items():
-                column_strs = ["\t" + e for e in _describe_schema(table.schema)]
-                columns_desc = "\n".join(column_strs)
-                if isinstance(table, PublicTable):
-                    table_desc = f"Public table '{name}':\n" + columns_desc
-                    public_table_descs.append(table_desc)
-                elif isinstance(table, PrivateTable):
-                    table_desc = f"Table '{name}':\n"
-                    table_desc += columns_desc
-
-                    constraints: Optional[
-                        List[Constraint]
-                    ] = self._table_constraints.get(NamedTable(name))
-                    if not constraints:
-                        table_desc = (
-                            f"Table '{name}' (no constraints):\n" + columns_desc
-                        )
-                    else:
-                        table_desc = (
-                            f"Table '{name}':\n" + columns_desc + "\n\tConstraints:\n"
-                        )
-                        constraints_strs = [f"\t\t- {e}" for e in constraints]
-                        table_desc += "\n".join(constraints_strs)
-
-                    private_table_descs.append(table_desc)
-                else:
-                    raise AssertionError(
-                        f"Table {name} has an unrecognized type: {type(table)}. This is"
-                        " probably a bug; please let us know about it so we can"
-                        " fix it!"
-                    )
-            if len(private_table_descs) != 0:
-                out.append(
-                    "The following private tables are available:\n"
-                    + "\n".join(private_table_descs)
-                )
-            if len(public_table_descs) != 0:
-                out.append(
-                    "The following public tables are available:\n"
-                    + "\n".join(public_table_descs)
-                )
-        print("\n".join(out))
-
-    def _describe_query(self, query: QueryExpr):
-        """Describe the output schema of a query and the constraints on it."""
-        schema = self._compiler.query_schema(query, self._catalog)
-        out = _describe_schema(schema)
-        print("\n".join(out))
-
 
 def _assert_is_identifier(source_id: str):
     """Checks that the ``source_id`` is a valid Python identifier.
 
     Args:
         source_id: The name of the dataframe or transformation.
     """
```

### Comparing `tmlt_analytics-0.7.0rc1/tmlt/analytics/utils.py` & `tmlt_analytics-0.7.1/tmlt/analytics/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Utility functions for Analytics."""
 
+import atexit
+from textwrap import dedent
+
 import pandas as pd
 from pyspark.sql import SparkSession
+from tmlt.core.utils import cleanup as core_cleanup
+from tmlt.core.utils import configuration
 
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import PureDPBudget
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.session import Session
-from tmlt.core.utils import cleanup as core_cleanup
-from tmlt.core.utils import configuration
 
 
 def cleanup():
     """Cleanup the temporary table currently in use.
 
     If you call ``spark.stop()``, you should call this function first.
     """
@@ -41,51 +44,69 @@
 
     * create a new Spark session
     * create a Spark dataframe
     * create a :class:`~tmlt.analytics.session.Session` from that dataframe
     * perform a query on that dataframe
 
     If Analytics is correctly installed, this function should print a message
-    and finish running within a few minutes.
+    and finish running within a few seconds.
 
     If Analytics has *not* been correctly installed, this function will raise
     an error.
     """
     try:
-        print("Creating Spark session... ", end="")
-        spark = SparkSession.builder.getOrCreate()
-        print(" ok")
+        try:
+            print("Creating Spark session... ", end="")
+            spark = SparkSession.builder.getOrCreate()
+            print(" OK")
+        except RuntimeError as e:
+            # If Spark is broken, the Core cleanup atexit hook will fail, which
+            # produces some additional output the user doesn't need to see in
+            # this case.
+            atexit.unregister(
+                core_cleanup._cleanup_temp  # pylint: disable=protected-access
+            )
+            if (
+                e.args
+                and isinstance(e.args[0], str)
+                and e.args[0].startswith("Java gateway process exited before sending")
+            ):
+                raise AssertionError(
+                    "Error setting up Spark session. This likely indicates that Java is"
+                    " not installed, or is not available on your PATH."
+                ) from e
+            raise
 
         print("Creating Pandas dataframe... ", end="")
         # We use Pandas to create this dataframe,
         # just to check that Pandas is installed and we can access it
         pdf = pd.DataFrame([["a1", 1], ["a2", 2]], columns=["A", "B"])
-        print(" ok")
+        print(" OK")
 
         print("Converting to Spark dataframe... ", end="")
         sdf = spark.createDataFrame(pdf)
-        print(" ok")
+        print(" OK")
 
         print("Creating Analytics session... ", end="")
         session = Session.from_dataframe(
             privacy_budget=PureDPBudget(1), source_id="private_data", dataframe=sdf
         )
-        print(" ok")
+        print(" OK")
 
         print("Creating query...", end="")
         query = (
             QueryBuilder("private_data")
             .groupby(KeySet.from_dict({"A": ["a0", "a1", "a2"]}))
             .count(name="count")
         )
-        print(" ok")
+        print(" OK")
 
         print("Evaluating query...", end="")
         result = session.evaluate(query_expr=query, privacy_budget=PureDPBudget(1))
-        print(" ok")
+        print(" OK")
 
         print("Checking that output is as expected...", end="")
         if (
             len(result.columns) != 2
             or not "A" in result.columns
             or not "count" in result.columns
         ):
@@ -105,31 +126,27 @@
             # result.toPandas() is used here so that the error message contains the
             # whole dataframe
             raise AssertionError(
                 "Expected output to have 1 row where column A was 'a0', one row where"
                 " column A was 'a1', and one row where column A was 'a2'. Instead, got"
                 f" this result: {result.toPandas()}"
             )
-        print(" ok")
+        print(" OK")
 
         print(
             "Installation check complete. Tumult Analytics appears to be properly"
             " installed."
         )
     except Exception as e:
-        print(
-            "\n\nThere was a problem running the installation checker. You may want to"
-            " check:"
-        )
-        print("- your installed Java version (run `java -version`)")
-        print("- your installed version of Pyspark (run `pip3 show pyspark`)")
-        print("- your installed version of Pandas (run `pip3 show pandas`)")
-        print(
-            "- your installed version of Tumult Analytics "
-            "(run `pip3 show tmlt.analytics`)"
-        )
-        print(
-            "For more information, see the Tumult Analytics installation instructions\n"
-            "at https://docs.tmlt.dev/analytics/latest/installation.html"
-        )
-        print("\nRe-raising original exception...")
-        raise e
+        print(" FAILED\n")
+        raise RuntimeError(
+            dedent(
+                """
+
+            The installation test did not complete successfully. You may want to check:
+            - your Java installation (try `java -version`)
+            - your PySpark and Pandas installations (run `pip3 show pyspark pandas`)
+
+            For more information, see the Tumult Analytics installation instructions
+            at https://docs.tmlt.dev/analytics/latest/howto-guides/installation.html"""
+            )
+        ) from e
```

### Comparing `tmlt_analytics-0.7.0rc1/setup.py` & `tmlt_analytics-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
  'tmlt.analytics.constraints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.2.0,<2.0.0',
- 'pyspark[sql]>=3.0.0,<3.4.0',
+ 'pyspark[sql]>=3.0.0,<=3.3.1',
  'sympy>=1.8,<1.10',
  'tmlt.core>=0.9.0,<0.10.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.7.0rc1',
+    'version': '0.7.1',
     'description': "Tumult's differential privacy analytics API",
     'long_description': '# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nThe Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nThe Tumult Platform documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
```

### Comparing `tmlt_analytics-0.7.0rc1/PKG-INFO` & `tmlt_analytics-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-analytics
-Version: 0.7.0rc1
+Version: 0.7.1
 Summary: Tumult's differential privacy analytics API
 Home-page: https://www.tmlt.dev/
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.10.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pandas (>=1.2.0,<2.0.0)
-Requires-Dist: pyspark[sql] (>=3.0.0,<3.4.0)
+Requires-Dist: pyspark[sql] (>=3.0.0,<=3.3.1)
 Requires-Dist: sympy (>=1.8,<1.10)
 Requires-Dist: tmlt.core (>=0.9.0,<0.10.0)
 Requires-Dist: typeguard (>=2.12.1,<2.13.0)
 Requires-Dist: typing-extensions (>=3.10.0,<4.0.0)
 Project-URL: Documentation, https://docs.tmlt.dev/analytics/latest
 Project-URL: Repository, https://gitlab.com/tumult-labs/analytics
 Description-Content-Type: text/markdown
```

