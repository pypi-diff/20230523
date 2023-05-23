# Comparing `tmp/webviz-subsurface-0.2.9.tar.gz` & `tmp/webviz-subsurface-0.2.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webviz-subsurface-0.2.9.tar", last modified: Thu Jan  6 15:14:18 2022, max compression
+gzip compressed data, was "dist/webviz-subsurface-0.2.9rc0.tar", last modified: Thu Dec 23 22:39:02 2021, max compression
```

## Comparing `webviz-subsurface-0.2.9.tar` & `webviz-subsurface-0.2.9rc0.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 15:14:17.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-06 14:47:43.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-06 15:14:17.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5064 2022-01-06 15:14:17.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-01-06 15:14:17.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-01-06 15:14:17.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21454 2022-01-06 15:14:17.000000 webviz-subsurface-0.2.9/webviz_subsurface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)    25647 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     6050 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.github/workflows/subsurface.yml
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5064 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5874 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/
--rw-r--r--   0 runner    (1001) docker     (121)     8115 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/statistics_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/unique_theming.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/vector_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)    12433 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/simulation_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/parameter_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12902 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/vector_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8630 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/fanchart_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/perf_timer.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_utils/webvizstore_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/
--rw-r--r--   0 runner    (1001) docker     (121)     9866 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/parameter_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/_tornado_table.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21494 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/tornado_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    11378 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/_tornado_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (121)    11954 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/_tornado_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     8859 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_components/color_picker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/
--rw-r--r--   0 runner    (1001) docker     (121)     4915 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider_impl_arrow.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13421 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider_impl_inmem_parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/
--rw-r--r--   0 runner    (1001) docker     (121)    13828 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_table_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12720 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3843 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_field_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     8791 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/dev_provider_perf_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/dev_resampling_perf_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_lazy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_arrow_unsmry_import.py
--rw-r--r--   0 runner    (1001) docker     (121)    10178 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/dev_compare_fmu_to_lazy_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_csv_import.py
--rw-r--r--   0 runner    (1001) docker     (121)    16578 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_presampled.py
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/history_match.py
--rw-r--r--   0 runner    (1001) docker     (121)    16064 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/units.py
--rw-r--r--   0 runner    (1001) docker     (121)    19130 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/xsection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6264 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/fmu_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     7001 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/well.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/well_completions.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/seismic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6823 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/from_timeseries_cumulatives.py
--rw-r--r--   0 runner    (1001) docker     (121)    15854 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/pvt_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/image_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/
--rw-r--r--   0 runner    (1001) docker     (121)    30617 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_common.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14114 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_water.py
--rw-r--r--   0 runner    (1001) docker     (121)    26976 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_oil.py
--rw-r--r--   0 runner    (1001) docker     (121)    19944 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_gas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/relative_permeability.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/inplace_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    28827 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_datainput/surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/smry2arrow_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_private_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_private_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12961 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_private_plugins/surface_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)    26808 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_cross_section_fmu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/
--rw-r--r--   0 runner    (1001) docker     (121)    18813 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/structural_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/realization_filter_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)    19562 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/map_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/modal_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     5275 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/uncertainty_table_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_source_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)    17499 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/figures/
--rw-r--r--   0 runner    (1001) docker     (121)     7573 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/figures/intersection.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/
--rw-r--r--   0 runner    (1001) docker     (121)    14675 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/uncertainty_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     6034 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/map_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/modal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/clientside_stores.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4914 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_and_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/realization_modal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/_tour_steps.py
--rw-r--r--   0 runner    (1001) docker     (121)    20597 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_segy_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/derived_delta_ensemble_vectors_accessor_impl.py
--rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/provider_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/derived_vectors_accessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/derived_ensemble_vectors_accessor_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5826 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/graph_figure_builder_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13950 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/ensemble_subplot_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    14936 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/vector_subplot_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/derived_ensemble_vectors_accessor_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12413 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/create_vector_traces_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/from_timeseries_cumulatives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/vector_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/provider_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/delta_ensemble_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/trace_line_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/history_vectors.py
--rw-r--r--   0 runner    (1001) docker     (121)    37621 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)    14757 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)    20248 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/models/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/models/parameters_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7643 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/models/simulation_timeseries_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6556 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/parameter_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_qc_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22546 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_response_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/figures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/figures/correlation_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/figures/color_figure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/main_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/parameter_qc_view.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11062 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/selector_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     7006 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/parameter_response_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/models/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11501 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/models/property_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    11641 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/models/simulation_timeseries_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/data_loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/utils/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/property_response_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/property_delta_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/property_qc_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/figures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/figures/correlation_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)     8580 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/property_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/
--rw-r--r--   0 runner    (1001) docker     (121)     7426 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/property_delta_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/main_view.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/selector_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/property_qc_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     6548 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/property_response_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/
--rw-r--r--   0 runner    (1001) docker     (121)    17158 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_business_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8474 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)    18668 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_surface_with_grid_cross_section.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/line_plotter_fmu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10232 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/controllers/build_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/controllers/update_figure_clientside.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/figures/
--rw-r--r--   0 runner    (1001) docker     (121)    11733 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/figures/plotly_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/data_selectors_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_traces_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_options_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    26273 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_running_time_analysis_fmu.py
--rw-r--r--   0 runner    (1001) docker     (121)    16716 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_surface_with_seismic_cross_section.py
--rw-r--r--   0 runner    (1001) docker     (121)    14986 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)    21077 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_assisted_history_matching_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     7280 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)    23612 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_parallel_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_tornado_plotter_fmu/
--rw-r--r--   0 runner    (1001) docker     (121)    10458 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_tornado_plotter_fmu/tornado_plotter_fmu.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_tornado_plotter_fmu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/
--rw-r--r--   0 runner    (1001) docker     (121)     9789 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/volumetric_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4880 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/utils/table_and_figure_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/volume_validator_and_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)    16841 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/comparison_controllers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/fipfile_qc_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12923 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/tornado_controllers.py
--rw-r--r--   0 runner    (1001) docker     (121)    16202 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/distribution_controllers.py
--rw-r--r--   0 runner    (1001) docker     (121)    22329 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/selections_controllers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4146 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/layout_controllers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/export_data_controllers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/
--rw-r--r--   0 runner    (1001) docker     (121)     5308 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/filter_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    11426 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/comparison_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/clientside_stores.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/main_view.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/fipfile_qc_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/distribution_main_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/selections_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     7527 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/tornado_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/
--rw-r--r--   0 runner    (1001) docker     (121)    20511 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_xsection.py
--rw-r--r--   0 runner    (1001) docker     (121)    41548 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/horizon_uncertainty_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_morris_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8353 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    37052 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_relative_permeability.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_history_match.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/
--rw-r--r--   0 runner    (1001) docker     (121)    20514 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/group_tree_data.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/group_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/controllers/controllers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/filters_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/main_view.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/options_view.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/selections_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    54675 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_reservoir_simulation_timeseries_regional.py
--rw-r--r--   0 runner    (1001) docker     (121)    62599 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_reservoir_simulation_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (121)    27372 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_reservoir_simulation_timeseries_onebyone.py
--rw-r--r--   0 runner    (1001) docker     (121)   145514 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_seismic_misfit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/
--rw-r--r--   0 runner    (1001) docker     (121)    11524 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_business_logic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8581 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_callbacks/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6921 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_callbacks/parameter_response_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/rft_plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18348 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_crossplot_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_misfit_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_errorplot_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)    12454 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_formation_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_map_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)    23142 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_inplace_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    28036 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_inplace_volumes_onebyone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7286 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/well_log_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/utils/xtgeo_well_log_to_json.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/utils/default_color_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/_validate_log_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/controllers/_well_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13244 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_cross_section.py
--rw-r--r--   0 runner    (1001) docker     (121)    32506 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_pvt_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7574 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_subsurface_map.py
--rw-r--r--   0 runner    (1001) docker     (121)    31078 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_surface_viewer_fmu.py
--rw-r--r--   0 runner    (1001) docker     (121)    14879 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_bhp_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)    25070 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_response_correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/inplace_volumes.css
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/block_options.css
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/container.css
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/modal.css
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/structural_uncertainty.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/js/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_assets/js/clientside_functions.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/
--rw-r--r--   0 runner    (1001) docker     (121)     4231 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/ensemble_set_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/caching_ensemble_set_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10365 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/surface_set_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/surface_leaflet_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3864 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/well_set_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    13034 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/inplace_volumes_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/observation_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6090 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_models/ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/volume_terminology.json
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/si_prefixes.json
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_unit_terminology.json
--rw-r--r--   0 runner    (1001) docker     (121)   135128 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/volume_terminology.py
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/number_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     8414 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/reservoir_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/webviz_subsurface/_figures/
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_figures/px_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_figures/barchart.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/webviz_subsurface/_figures/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/data/surface_png.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/data/parameters.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/data/surface_zarr.np.gz
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/data/colormap.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/data/volumes.csv
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/data/realizations.csv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries_regional.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_surface_viewer_fmu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_volumetric_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_tornado_plotter_fmu.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_pvt_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_relative_permeability.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_segy_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_structural_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_well_log_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_property_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries_onebyone.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_bhp_qc.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_line_plotter_fmu.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_history_match.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_rft_plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_surface_with_seismic_crossection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_surface_with_grid_crossection.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_response_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/test_surface_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/test_parameter_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/integration_tests/test_parameter_corr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/test_grouptree.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/test_well_completions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3879 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/test_tornado_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     8398 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5497 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_presampled.py
--rw-r--r--   0 runner    (1001) docker     (121)    11689 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_lazy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_table_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)    11349 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider_resampling.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_ensemble_set_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_surface_set_model.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_property_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_well_set_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/unit_tests/utils_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/utils_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/utils_tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/utils_tests/test_simulation_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-06 15:14:18.000000 webviz-subsurface-0.2.9/tests/unit_tests/data_input/
--rw-r--r--   0 runner    (1001) docker     (121)     6415 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/data_input/test_calc_from_cumulatives.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/data_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/tests/unit_tests/data_input/test_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/deploy_docker_image.sh
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-06 14:46:42.000000 webviz-subsurface-0.2.9/bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-23 22:16:54.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5067 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2597 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21454 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)    25495 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     6050 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.github/workflows/subsurface.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5067 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5874 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     8115 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/statistics_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1677 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/unique_theming.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/vector_selector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6033 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12433 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/simulation_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3778 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/parameter_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12902 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/vector_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8630 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/fanchart_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/perf_timer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/webvizstore_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/
+-rw-r--r--   0 runner    (1001) docker     (121)     9866 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/parameter_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/_tornado_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21494 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/tornado_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11378 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/_tornado_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11954 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/_tornado_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8859 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/color_picker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/
+-rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider_impl_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13421 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2364 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider_impl_inmem_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/
+-rw-r--r--   0 runner    (1001) docker     (121)    13818 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2530 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12720 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3843 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_field_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8791 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/dev_provider_perf_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3414 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/dev_resampling_perf_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13599 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3172 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_arrow_unsmry_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10178 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/dev_compare_fmu_to_lazy_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_csv_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16578 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_presampled.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4322 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/
+-rw-r--r--   0 runner    (1001) docker     (121)     2439 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/history_match.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16064 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/units.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19130 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/xsection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6264 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/fmu_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7001 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/well.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5422 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/well_completions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/seismic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6823 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/from_timeseries_cumulatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15854 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/pvt_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4393 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/image_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/
+-rw-r--r--   0 runner    (1001) docker     (121)    30617 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14114 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_water.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26976 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_oil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19944 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_gas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/relative_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/inplace_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28827 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3913 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/smry2arrow_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_private_plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_private_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12961 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_private_plugins/surface_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)    26808 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_cross_section_fmu.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (121)    18813 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/structural_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/realization_filter_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19562 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/map_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/modal_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5275 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/uncertainty_table_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_source_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17499 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/figures/
+-rw-r--r--   0 runner    (1001) docker     (121)     7573 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/figures/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/
+-rw-r--r--   0 runner    (1001) docker     (121)    14675 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3067 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/uncertainty_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6034 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/map_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/modal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/clientside_stores.py
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4914 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_and_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/realization_modal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2905 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/_tour_steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20597 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_segy_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12855 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/derived_delta_ensemble_vectors_accessor_impl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7135 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/provider_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/derived_vectors_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/derived_ensemble_vectors_accessor_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5826 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/graph_figure_builder_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13950 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/ensemble_subplot_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14936 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/vector_subplot_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     3166 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/derived_ensemble_vectors_accessor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12413 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/create_vector_traces_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6337 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/from_timeseries_cumulatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/vector_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2762 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/provider_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2551 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/delta_ensemble_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/trace_line_shape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2659 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/history_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37621 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14757 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20248 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7023 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/models/parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7643 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/models/simulation_timeseries_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6556 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/parameter_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)     3044 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_qc_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22546 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_response_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/figures/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/figures/correlation_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1867 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/figures/color_figure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/parameter_qc_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11062 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/selector_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7006 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/parameter_response_view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11501 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/models/property_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11641 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/models/simulation_timeseries_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/data_loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2474 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/utils/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10051 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/property_response_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4426 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/property_delta_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2269 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/property_qc_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/figures/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/figures/correlation_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8580 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/property_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     7426 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/property_delta_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/selector_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4015 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/property_qc_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6548 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/property_response_view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/
+-rw-r--r--   0 runner    (1001) docker     (121)    17158 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_business_logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8474 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2256 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18668 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_surface_with_grid_cross_section.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6960 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/line_plotter_fmu.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10232 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/controllers/build_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/controllers/update_figure_clientside.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/figures/
+-rw-r--r--   0 runner    (1001) docker     (121)    11733 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/figures/plotly_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     3260 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/data_selectors_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_traces_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_options_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26273 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_running_time_analysis_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16716 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_surface_with_seismic_cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14986 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21077 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_assisted_history_matching_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7280 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23612 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_parallel_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_tornado_plotter_fmu/
+-rw-r--r--   0 runner    (1001) docker     (121)    10458 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_tornado_plotter_fmu/tornado_plotter_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_tornado_plotter_fmu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)     9789 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/volumetric_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     4880 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/utils/table_and_figure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9239 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/volume_validator_and_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)    16835 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/comparison_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4068 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/fipfile_qc_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12923 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/tornado_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16202 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/distribution_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22329 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/selections_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4146 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/layout_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/export_data_controllers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/
+-rw-r--r--   0 runner    (1001) docker     (121)     5308 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/filter_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11426 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/comparison_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/clientside_stores.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6726 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2354 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/fipfile_qc_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/distribution_main_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/selections_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7527 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/tornado_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2759 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/
+-rw-r--r--   0 runner    (1001) docker     (121)    20511 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_xsection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41548 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/horizon_uncertainty_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_morris_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8353 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37052 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_relative_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5264 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_history_match.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/
+-rw-r--r--   0 runner    (1001) docker     (121)    20514 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/group_tree_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6780 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/group_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4183 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/controllers/controllers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/filters_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/options_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/selections_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54675 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_reservoir_simulation_timeseries_regional.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62599 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_reservoir_simulation_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27372 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_reservoir_simulation_timeseries_onebyone.py
+-rw-r--r--   0 runner    (1001) docker     (121)   145514 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_seismic_misfit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/
+-rw-r--r--   0 runner    (1001) docker     (121)    11524 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_business_logic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8581 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_callbacks/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6921 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_callbacks/parameter_response_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5177 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/rft_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18348 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/
+-rw-r--r--   0 runner    (1001) docker     (121)     3739 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_crossplot_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_misfit_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_errorplot_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12454 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_formation_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_map_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23142 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_inplace_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28036 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_inplace_volumes_onebyone.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7286 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/well_log_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1956 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/utils/xtgeo_well_log_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4872 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/utils/default_color_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/_validate_log_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/controllers/_well_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13244 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32506 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_pvt_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7574 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_subsurface_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31078 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_surface_viewer_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14879 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_bhp_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25070 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_response_correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/inplace_volumes.css
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/block_options.css
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/container.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/modal.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1779 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/structural_uncertainty.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/js/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/js/clientside_functions.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/
+-rw-r--r--   0 runner    (1001) docker     (121)     4231 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/ensemble_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/caching_ensemble_set_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10365 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/surface_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/surface_leaflet_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3864 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/well_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13034 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/inplace_volumes_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/observation_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6090 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/volume_terminology.json
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/si_prefixes.json
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_unit_terminology.json
+-rw-r--r--   0 runner    (1001) docker     (121)   135128 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/volume_terminology.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3483 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/number_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8414 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/reservoir_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/
+-rw-r--r--   0 runner    (1001) docker     (121)     9770 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/px_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2435 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/barchart.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/data/surface_png.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5036 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/data/parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     6357 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/data/surface_zarr.np.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/data/colormap.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/data/volumes.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/data/realizations.csv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries_regional.py
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_surface_viewer_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_volumetric_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_tornado_plotter_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_pvt_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_relative_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_segy_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8149 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_structural_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_well_log_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_property_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries_onebyone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_bhp_qc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_line_plotter_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_history_match.py
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_rft_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_surface_with_seismic_crossection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_surface_with_grid_crossection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_response_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/test_surface_selector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/test_parameter_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/integration_tests/test_parameter_corr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4548 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/test_grouptree.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5269 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/test_well_completions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3879 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/test_tornado_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     8398 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_presampled.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11689 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5600 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_table_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11349 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_ensemble_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4952 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_surface_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_property_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2081 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_well_set_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/utils_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/utils_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/utils_tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/utils_tests/test_simulation_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-23 22:39:02.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/data_input/
+-rw-r--r--   0 runner    (1001) docker     (121)     6415 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/data_input/test_calc_from_cumulatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/data_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/tests/unit_tests/data_input/test_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/deploy_docker_image.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-23 22:16:00.000000 webviz-subsurface-0.2.9rc0/bandit.yml
```

### Comparing `webviz-subsurface-0.2.9/.pylintrc` & `webviz-subsurface-0.2.9rc0/.pylintrc`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface.egg-info/PKG-INFO` & `webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-subsurface
-Version: 0.2.9
+Version: 0.2.9rc0
 Summary: Webviz config plugins for subsurface data
 Home-page: https://github.com/equinor/webviz-subsurface
 Author: R&T Equinor
 License: UNKNOWN
 Project-URL: Documentation, https://equinor.github.io/webviz-subsurface
 Project-URL: Download, https://pypi.org/project/webviz-subsurface/
 Project-URL: Source, https://github.com/equinor/webviz-subsurface
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface.egg-info/requires.txt` & `webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jsonschema>=3.2.0
 pandas>=1.1.5
 pillow>=6.1
 pyarrow>=5.0.0
 pyscal>=0.7.5
 scipy>=1.2
 statsmodels>=0.12.1
-webviz-config>=0.3.8
+webviz-config>=0.3.1
 webviz-core-components>=0.5.1
 webviz-subsurface-components>=0.4.8
 xtgeo>=2.14
 
 [:python_version < "3.7"]
 dataclasses>=0.8
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface.egg-info/entry_points.txt` & `webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface.egg-info/SOURCES.txt` & `webviz-subsurface-0.2.9rc0/webviz_subsurface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/mypy.ini` & `webviz-subsurface-0.2.9rc0/mypy.ini`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/CHANGELOG.md` & `webviz-subsurface-0.2.9rc0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [UNRELEASED] - YYYY-MM-DD
-
-## [0.2.9] - 2022-01-06
+### Added
+- [#880](https://github.com/equinor/webviz-subsurface/pull/880) - Show hover information for uncertainty envelope in `StructuralUncertainty`.
 
 ### Fixed
 
 - [#888](https://github.com/equinor/webviz-subsurface/pull/888) - Improved `SeismicMisfit` performance when using polygon files with a large number of polygons.
-- [#911](https://github.com/equinor/webviz-subsurface/pull/911) - Handle ensembles with missing surface folders in `PropertyStatistics`.
 
 ### Added
 
-- [#880](https://github.com/equinor/webviz-subsurface/pull/880) - Show hover information for uncertainty envelope in `StructuralUncertainty`.
 - [#883](https://github.com/equinor/webviz-subsurface/pull/883) - Added `Statistics + Realizations`-plot for New `SimulationTimeSeries` plugin. Includes filtering of realizations and selection to calculate statistics from all realizations or selected subset of realizations. Updated visualization mode included in user download data.
 - [#867](https://github.com/equinor/webviz-subsurface/pull/867) - Added new `SimulationTimeSeries` plugin, with code structure according to best practice plugin example `webviz-plugin-boilerplate` and usage of `EnsembleSummaryProvider`. New functionality as multiple Delta Ensembles in same plot, selectable resampling frequency and possibility to group subplots per selected ensemble or per selected vector.
 - [#884](https://github.com/equinor/webviz-subsurface/pull/884) - Added a new tab to the `RFTPlotter` plugin, with functionality to analyse RFT pressure responses to parameters.
 
 ### Changed
 
 - [#889](https://github.com/equinor/webviz-subsurface/pull/889) - Added `rel_file_pattern` argument to .arrow related factory methods in EnsembleSummaryProviderFactory.
```

### Comparing `webviz-subsurface-0.2.9/.github/workflows/subsurface.yml` & `webviz-subsurface-0.2.9rc0/.github/workflows/subsurface.yml`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md` & `webviz-subsurface-0.2.9rc0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md` & `webviz-subsurface-0.2.9rc0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/LICENSE` & `webviz-subsurface-0.2.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/PKG-INFO` & `webviz-subsurface-0.2.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-subsurface
-Version: 0.2.9
+Version: 0.2.9rc0
 Summary: Webviz config plugins for subsurface data
 Home-page: https://github.com/equinor/webviz-subsurface
 Author: R&T Equinor
 License: UNKNOWN
 Project-URL: Documentation, https://equinor.github.io/webviz-subsurface
 Project-URL: Download, https://pypi.org/project/webviz-subsurface/
 Project-URL: Source, https://github.com/equinor/webviz-subsurface
```

### Comparing `webviz-subsurface-0.2.9/setup.py` & `webviz-subsurface-0.2.9rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         "opm>=2020.10.1; sys_platform=='linux'",
         "pandas>=1.1.5",
         "pillow>=6.1",
         "pyarrow>=5.0.0",
         "pyscal>=0.7.5",
         "scipy>=1.2",
         "statsmodels>=0.12.1",  # indirect dependency through https://plotly.com/python/linear-fits/
-        "webviz-config>=0.3.8",
+        "webviz-config>=0.3.1",
         "webviz-core-components>=0.5.1",
         "webviz-subsurface-components>=0.4.8",
         "xtgeo>=2.14",
     ],
     extras_require={"tests": TESTS_REQUIRE},
     setup_requires=["setuptools_scm~=3.2"],
     python_requires="~=3.6",
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/statistics_plotting.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/statistics_plotting.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/unique_theming.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/unique_theming.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/vector_selector.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/vector_selector.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/formatting.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/colors.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/colors.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/simulation_timeseries.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/simulation_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,21 @@
 def calc_series_statistics(
     df: pd.DataFrame, vectors: list, refaxis: str = "DATE"
 ) -> pd.DataFrame:
     """Calculate statistics for given vectors over the ensembles
     refaxis is used if another column than DATE should be used to groupby.
     """
     # Invert p10 and p90 due to oil industry convention.
-    def p10(x: List[float]) -> np.floating:
+    def p10(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=90)
 
-    def p90(x: List[float]) -> np.floating:
+    def p90(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=10)
 
-    def p50(x: List[float]) -> np.floating:
+    def p50(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=50)
 
     # Calculate statistics, ignoring NaNs.
     stat_df = (
         df[["ENSEMBLE", refaxis] + vectors]
         .groupby(["ENSEMBLE", refaxis])
         .agg([np.nanmean, np.nanmin, np.nanmax, p10, p90, p50])
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/parameter_response.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/parameter_response.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/vector_calculator.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/vector_calculator.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/fanchart_plotting.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/fanchart_plotting.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_utils/perf_timer.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_utils/perf_timer.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_components/parameter_filter.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/_tornado_table.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/_tornado_table.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/tornado_widget.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/tornado_widget.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/_tornado_bar_chart.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/_tornado_bar_chart.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_components/tornado/_tornado_data.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/tornado/_tornado_data.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_components/color_picker.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_components/color_picker.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider_impl_arrow.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider_impl_arrow.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider_factory.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider_factory.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_table_provider_impl_inmem_parquet.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_table_provider_impl_inmem_parquet.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_resampling.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_resampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     Note that xp and yp must be arrays of the same length.
     It is assumed that both the x and the xp array is sorted in increasing order.
     """
 
     # Finds the leftmost valid insertion indices for the values x in xp
     indices = np.searchsorted(xp, x, side="left")
 
-    padded_y = np.concatenate((yp, np.array([yright])))
+    padded_y = np.concatenate((yp, [yright]))
 
     ret_arr = padded_y[indices]
 
     if x[0] < xp[0]:
         idx = np.searchsorted(x, xp[0])
         ret_arr[0:idx] = yleft
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_table_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_table_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider_factory.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider_factory.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_field_metadata.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_field_metadata.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/dev_provider_perf_testing.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/dev_provider_perf_testing.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/dev_resampling_perf_testing.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/dev_resampling_perf_testing.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_dataframe_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_lazy.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_lazy.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_arrow_unsmry_import.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_arrow_unsmry_import.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/dev_compare_fmu_to_lazy_provider.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/dev_compare_fmu_to_lazy_provider.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_csv_import.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_csv_import.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_presampled.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/_provider_impl_arrow_presampled.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_providers/ensemble_summary_provider/ensemble_summary_provider.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/__init__.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/history_match.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/history_match.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/units.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/units.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/xsection.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/xsection.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/fmu_input.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/fmu_input.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/well.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/well.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/well_completions.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/well_completions.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/seismic.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/seismic.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/from_timeseries_cumulatives.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/from_timeseries_cumulatives.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/pvt_data.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/pvt_data.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/image_processing.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/image_processing.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_common.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_common.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_water.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_water.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_oil.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_oil.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_init_io/pvt_gas.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_init_io/pvt_gas.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/relative_permeability.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/relative_permeability.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/inplace_volumes.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/inplace_volumes.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_datainput/eclipse_unit.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_datainput/eclipse_unit.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/smry2arrow_batch.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/smry2arrow_batch.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_private_plugins/surface_selector.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_private_plugins/surface_selector.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_cross_section_fmu.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_cross_section_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/structural_uncertainty.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/structural_uncertainty.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/realization_filter_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/realization_filter_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/map_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/map_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/modal_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/modal_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/uncertainty_table_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/uncertainty_table_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_source_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_source_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/controllers/intersection_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/figures/intersection.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/figures/intersection.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_data.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_data.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/uncertainty_table.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/uncertainty_table.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/map_data.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/map_data.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/modal.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/modal.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/clientside_stores.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/clientside_stores.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_and_map.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/intersection_and_map.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/views/realization_modal.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/views/realization_modal.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_structural_uncertainty/_tour_steps.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_structural_uncertainty/_tour_steps.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_segy_viewer.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_segy_viewer.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/derived_delta_ensemble_vectors_accessor_impl.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/derived_delta_ensemble_vectors_accessor_impl.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/provider_set.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/provider_set.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/types.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/types.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/derived_vectors_accessor.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/derived_vectors_accessor.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/types/derived_ensemble_vectors_accessor_impl.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/types/derived_ensemble_vectors_accessor_impl.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/graph_figure_builder_base.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/graph_figure_builder_base.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/ensemble_subplot_builder.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/ensemble_subplot_builder.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/vector_subplot_builder.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_property_serialization/vector_subplot_builder.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/derived_ensemble_vectors_accessor_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/derived_ensemble_vectors_accessor_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/create_vector_traces_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/create_vector_traces_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/from_timeseries_cumulatives.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/from_timeseries_cumulatives.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/vector_statistics.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/vector_statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     # Get vectors names, keep order
     columns_list = list(vectors_df.columns)
     vector_names = sorted(
         (set(columns_list) ^ set(["DATE", "REAL"])), key=columns_list.index
     )
 
     # Invert p10 and p90 due to oil industry convention.
-    def p10(x: List[float]) -> np.floating:
+    def p10(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=90)
 
-    def p90(x: List[float]) -> np.floating:
+    def p90(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=10)
 
-    def p50(x: List[float]) -> np.floating:
+    def p50(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=50)
 
     statistics_df: pd.DataFrame = (
         vectors_df[["DATE"] + vector_names]
         .groupby(["DATE"])
         .agg([np.nanmean, np.nanmin, np.nanmax, p10, p90, p50])
         .reset_index(level=["DATE"], col_level=0)
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/provider_set_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/provider_set_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/delta_ensemble_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/delta_ensemble_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/trace_line_shape.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/trace_line_shape.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/utils/history_vectors.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/utils/history_vectors.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_callbacks.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_callbacks.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_plugin.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_simulation_time_series/_layout.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_simulation_time_series/_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/models/parameters_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/models/parameters_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/models/simulation_timeseries_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/models/simulation_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/parameter_analysis.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/parameter_analysis.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_qc_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_qc_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_response_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/controllers/parameter_response_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/figures/correlation_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/figures/correlation_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/figures/color_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/figures/color_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/main_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/main_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/parameter_qc_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/parameter_qc_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/selector_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/selector_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_analysis/views/parameter_response_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_analysis/views/parameter_response_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/models/property_statistics_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/models/property_statistics_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/models/simulation_timeseries_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/models/simulation_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/utils/colors.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/utils/colors.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/utils/surface.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/utils/surface.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     for ensemble in ensembles:
         for zone in zones:
             for prop in properties:
                 for statistic in statistics:
                     zone_in_file = surface_renaming.get(zone, zone)
                     prop_in_file = surface_renaming.get(prop, prop)
                     path = (
-                        surface_folders.get(ensemble, pathlib.Path())
+                        surface_folders[ensemble]
                         / statistic
                         / f"{zone_in_file}--{prop_in_file}.gri"
                     )
                     if path.exists():
                         surface_table.append(
                             {
                                 "ensemble": ensemble,
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/property_response_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/property_response_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/property_delta_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/property_delta_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/controllers/property_qc_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/controllers/property_qc_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/figures/correlation_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/figures/correlation_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/property_statistics.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/property_statistics.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/property_delta_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/property_delta_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/main_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/main_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/selector_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/selector_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/property_qc_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/property_qc_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_property_statistics/views/property_response_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_property_statistics/views/property_response_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_business_logic.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_business_logic.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_callbacks.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_callbacks.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_plugin.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_completions/_layout.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_completions/_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_surface_with_grid_cross_section.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_surface_with_grid_cross_section.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/line_plotter_fmu.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/line_plotter_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/controllers/build_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/controllers/build_figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,18 +242,18 @@
 def calc_series_statistics(
     df: pd.DataFrame, vectors: list, refaxis: str = "DATE"
 ) -> pd.DataFrame:
     """Calculate statistics for given vectors over the ensembles
     refaxis is used if another column than DATE should be used to groupby.
     """
     # Invert p10 and p90 due to oil industry convention.
-    def p10(x: List[float]) -> np.floating:
+    def p10(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=90)
 
-    def p90(x: List[float]) -> np.floating:
+    def p90(x: List[float]) -> List[float]:
         return np.nanpercentile(x, q=10)
 
     # Calculate statistics, ignoring NaNs.
     stat_df = (
         df[["ENSEMBLE", refaxis] + vectors]
         .groupby(["ENSEMBLE", refaxis])
         .agg([np.nanmean, np.nanmin, np.nanmax, p10, p90])
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/controllers/update_figure_clientside.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/controllers/update_figure_clientside.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/figures/plotly_line_plot.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/figures/plotly_line_plot.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/data_selectors_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/data_selectors_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/__init__.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_traces_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_traces_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_options_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_line_plotter_fmu/views/plot_options_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_running_time_analysis_fmu.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_running_time_analysis_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_surface_with_seismic_cross_section.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_surface_with_seismic_cross_section.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_correlation.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_correlation.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_assisted_history_matching_analysis.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_assisted_history_matching_analysis.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_disk_usage.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_disk_usage.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_parallel_coordinates.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_tornado_plotter_fmu/tornado_plotter_fmu.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_tornado_plotter_fmu/tornado_plotter_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/volumetric_analysis.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/volumetric_analysis.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/utils/table_and_figure_utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/utils/table_and_figure_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/utils/utils.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/utils/utils.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/volume_validator_and_combinator.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/volume_validator_and_combinator.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/comparison_controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/comparison_controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         df = df.rename(columns={f"{resp} diff": "diff", f"{resp} diff (%)": "diff (%)"})
     df = add_fluid_zone_column(df, selections["filters"])
     return df.sort_values(by=[abssort_on], key=abs, ascending=False)
 
 
 def compute_highlighted_col(
     df: pd.DataFrame, response: str, value1: str, selections: dict
-) -> np.ndarray:
+) -> list:
     highlight_mask = (df[response][value1] > selections["Ignore <"]) & (
         df[response]["diff (%)"].abs() > selections["Accept value"]
     )
     return np.where(highlight_mask, "yes", "no")
 
 
 def find_higlighted_real_count(
```

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/fipfile_qc_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/fipfile_qc_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/tornado_controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/tornado_controllers.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/distribution_controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/distribution_controllers.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/selections_controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/selections_controllers.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/layout_controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/layout_controllers.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/controllers/export_data_controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/controllers/export_data_controllers.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/filter_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/filter_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/comparison_layout.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/comparison_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/clientside_stores.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/clientside_stores.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/main_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/main_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/fipfile_qc_layout.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/fipfile_qc_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/distribution_main_layout.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/distribution_main_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/selections_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/selections_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_volumetric_analysis/views/tornado_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_volumetric_analysis/views/tornado_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/__init__.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_xsection.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_xsection.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/horizon_uncertainty_viewer.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/horizon_uncertainty_viewer.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_table.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_horizon_uncertainty_viewer/_huv_table.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_morris_plot.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_morris_plot.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_distribution.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_distribution.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_relative_permeability.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_relative_permeability.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_history_match.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_history_match.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/group_tree_data.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/group_tree_data.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/group_tree.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/group_tree.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/controllers/controllers.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/filters_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/filters_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/main_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/main_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/options_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/options_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_group_tree/views/selections_view.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_group_tree/views/selections_view.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_reservoir_simulation_timeseries_regional.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_reservoir_simulation_timeseries_regional.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_reservoir_simulation_timeseries.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_reservoir_simulation_timeseries.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_reservoir_simulation_timeseries_onebyone.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_reservoir_simulation_timeseries_onebyone.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_seismic_misfit.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_seismic_misfit.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_business_logic.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_business_logic.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_callbacks/callbacks.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_callbacks/parameter_response_callbacks.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_callbacks/parameter_response_callbacks.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/rft_plotter.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/rft_plotter.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_layout.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_layout.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_crossplot_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_crossplot_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_misfit_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_misfit_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_errorplot_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_errorplot_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_formation_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_formation_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_rft_plotter/_figures/_map_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_rft_plotter/_figures/_map_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_inplace_volumes.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_inplace_volumes.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_inplace_volumes_onebyone.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_inplace_volumes_onebyone.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/well_log_viewer.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/well_log_viewer.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/utils/xtgeo_well_log_to_json.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/utils/xtgeo_well_log_to_json.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/utils/default_color_tables.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/utils/default_color_tables.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/_validate_log_templates.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/_validate_log_templates.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_log_viewer/controllers/_well_controller.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_log_viewer/controllers/_well_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_well_cross_section.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_well_cross_section.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_pvt_plot.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_pvt_plot.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_subsurface_map.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_subsurface_map.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_surface_viewer_fmu.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_surface_viewer_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_bhp_qc.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_bhp_qc.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/plugins/_parameter_response_correlation.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/plugins/_parameter_response_correlation.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/modal.css` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/modal.css`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_assets/css/structural_uncertainty.css` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/css/structural_uncertainty.css`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_assets/js/clientside_functions.js` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_assets/js/clientside_functions.js`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/ensemble_set_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/ensemble_set_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/caching_ensemble_set_model_factory.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/caching_ensemble_set_model_factory.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/surface_set_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/surface_set_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/surface_leaflet_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/surface_leaflet_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/parameter_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/parameter_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/well_set_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/well_set_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/inplace_volumes_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/inplace_volumes_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/observation_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/observation_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_models/ensemble_model.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_models/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/volume_terminology.json` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/volume_terminology.json`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_unit_terminology.json` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_unit_terminology.json`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_vectors.json` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/abbreviation_data/reservoir_simulation_vectors.json`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/volume_terminology.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/volume_terminology.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/number_formatting.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/number_formatting.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_abbreviations/reservoir_simulation.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_abbreviations/reservoir_simulation.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_figures/px_figure.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/px_figure.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_figures/barchart.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/barchart.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/webviz_subsurface/_figures/scatterplot.py` & `webviz-subsurface-0.2.9rc0/webviz_subsurface/_figures/scatterplot.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/README.md` & `webviz-subsurface-0.2.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/data/surface_png.txt` & `webviz-subsurface-0.2.9rc0/tests/data/surface_png.txt`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/data/parameters.csv` & `webviz-subsurface-0.2.9rc0/tests/data/parameters.csv`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/data/surface_zarr.np.gz` & `webviz-subsurface-0.2.9rc0/tests/data/surface_zarr.np.gz`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/data/volumes.csv` & `webviz-subsurface-0.2.9rc0/tests/data/volumes.csv`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/data/realizations.csv` & `webviz-subsurface-0.2.9rc0/tests/data/realizations.csv`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries_regional.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries_regional.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_surface_viewer_fmu.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_surface_viewer_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_volumetric_analysis.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_volumetric_analysis.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_tornado_plotter_fmu.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_tornado_plotter_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_analysis.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_analysis.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_segy_viewer.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_segy_viewer.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_structural_uncertainty.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_structural_uncertainty.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_reservoir_simulation_timeseries.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_well_log_viewer.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_well_log_viewer.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_line_plotter_fmu.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_line_plotter_fmu.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_history_match.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_history_match.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_rft_plotter.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_rft_plotter.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_surface_with_seismic_crossection.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_surface_with_seismic_crossection.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_surface_with_grid_crossection.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_surface_with_grid_crossection.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/plugin_tests/test_parameter_response_correlation.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/plugin_tests/test_parameter_response_correlation.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/test_surface_selector.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/test_surface_selector.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/test_parameter_filter.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/test_parameter_filter.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/integration_tests/test_parameter_corr.py` & `webviz-subsurface-0.2.9rc0/tests/integration_tests/test_parameter_corr.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/conftest.py` & `webviz-subsurface-0.2.9rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/test_grouptree.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/test_grouptree.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/test_well_completions.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/test_well_completions.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/plugin_tests/test_tornado_data.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/plugin_tests/test_tornado_data.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_presampled.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_presampled.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_lazy.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider_impl_arrow_lazy.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_table_provider.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_table_provider.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/provider_tests/test_ensemble_summary_provider_resampling.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/provider_tests/test_ensemble_summary_provider_resampling.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_ensemble_set_model.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_ensemble_set_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_ensemble_model.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_surface_set_model.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_surface_set_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_property_statistics_model.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_property_statistics_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/model_tests/test_well_set_model.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/model_tests/test_well_set_model.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/utils_tests/test_simulation_timeseries.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/utils_tests/test_simulation_timeseries.py`

 * *Files identical despite different names*

### Comparing `webviz-subsurface-0.2.9/tests/unit_tests/data_input/test_calc_from_cumulatives.py` & `webviz-subsurface-0.2.9rc0/tests/unit_tests/data_input/test_calc_from_cumulatives.py`

 * *Files identical despite different names*

