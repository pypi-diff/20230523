# Comparing `tmp/tvb-rest-client-2.7.2.tar.gz` & `tmp/tvb-rest-client-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-rest-client-2.7.2.tar", last modified: Wed Jan  4 06:21:47 2023, max compression
+gzip compressed data, was "tvb-rest-client-2.8.1.tar", last modified: Tue May 23 12:09:33 2023, max compression
```

## Comparing `tvb-rest-client-2.7.2.tar` & `tvb-rest-client-2.8.1.tar`

### file list

```diff
@@ -1,383 +1,385 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.772705 tvb-rest-client-2.7.2/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      300 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/MANIFEST_rest_client.in
--rw-r--r--   0 root         (0) root         (0)     4288 2023-01-04 06:21:47.771705 tvb-rest-client-2.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4235 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/README.rst
--rw-r--r--   0 root         (0) root         (0)     3716 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/README_rest_client.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-04 06:21:47.772705 tvb-rest-client-2.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3133 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.700701 tvb-rest-client-2.7.2/tvb/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.700701 tvb-rest-client-2.7.2/tvb/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.705702 tvb-rest-client-2.7.2/tvb/adapters/analyzers/
--rw-r--r--   0 root         (0) root         (0)     1811 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8953 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_adapters.py
--rw-r--r--   0 root         (0) root         (0)     9731 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_centrality_adapters.py
--rw-r--r--   0 root         (0) root         (0)     5845 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_clustering_adapters.py
--rw-r--r--   0 root         (0) root         (0)     8009 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_degree_adapters.py
--rw-r--r--   0 root         (0) root         (0)    17032 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/cross_correlation_adapter.py
--rw-r--r--   0 root         (0) root         (0)    20045 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/fcd_adapter.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/fmri_balloon_adapter.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/fourier_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/ica_adapter.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/metrics_group_timeseries.py
--rw-r--r--   0 root         (0) root         (0)     7841 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/node_coherence_adapter.py
--rw-r--r--   0 root         (0) root         (0)    11026 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/node_complex_coherence_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/node_covariance_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7446 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/pca_adapter.py
--rw-r--r--   0 root         (0) root         (0)    11610 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/analyzers/wavelet_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.707702 tvb-rest-client-2.7.2/tvb/adapters/creators/
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33529 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/allen_creator.py
--rw-r--r--   0 root         (0) root         (0)    11383 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/connectivity_creator.py
--rw-r--r--   0 root         (0) root         (0)     7621 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/local_connectivity_creator.py
--rw-r--r--   0 root         (0) root         (0)    18196 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/siibra_base.py
--rw-r--r--   0 root         (0) root         (0)     8463 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/siibra_creator.py
--rw-r--r--   0 root         (0) root         (0)    12706 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/creators/stimulus_creator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.707702 tvb-rest-client-2.7.2/tvb/adapters/datatypes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.712702 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/
--rw-r--r--   0 root         (0) root         (0)     2553 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5450 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/annotation.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/connectivity.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/fcd.py
--rw-r--r--   0 root         (0) root         (0)     5801 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/graph.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/local_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     3795 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/mapped_value.py
--rw-r--r--   0 root         (0) root         (0)     3742 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/mode_decompositions.py
--rw-r--r--   0 root         (0) root         (0)     3680 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/patterns.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/projections.py
--rw-r--r--   0 root         (0) root         (0)     5471 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/region_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.713702 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/
--rw-r--r--   0 root         (0) root         (0)     3568 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_region_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2949 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_sensor.py
--rw-r--r--   0 root         (0) root         (0)     4074 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_surface.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_timeseries.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_volume.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/sensors.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/simulation_history.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/spectral.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/structural.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/surface.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/temporal_correlations.py
--rw-r--r--   0 root         (0) root         (0)    12512 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/tracts.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.717702 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/annotation_h5.py
--rw-r--r--   0 root         (0) root         (0)     3086 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/connectivity_h5.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/fcd_h5.py
--rw-r--r--   0 root         (0) root         (0)     3365 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/graph_h5.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/local_connectivity_h5.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/mapped_value_h5.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/mode_decompositions_h5.py
--rw-r--r--   0 root         (0) root         (0)     2758 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/patterns_h5.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/projections_h5.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/region_mapping_h5.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/sensors_h5.py
--rw-r--r--   0 root         (0) root         (0)     8931 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/spectral_h5.py
--rw-r--r--   0 root         (0) root         (0)     3663 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/structural_h5.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/surface_h5.py
--rw-r--r--   0 root         (0) root         (0)     2284 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/temporal_correlations_h5.py
--rw-r--r--   0 root         (0) root         (0)    14867 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/time_series_h5.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/tracts_h5.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/volumes_h5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.719702 tvb-rest-client-2.7.2/tvb/adapters/exporters/
--rw-r--r--   0 root         (0) root         (0)     1383 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/exporters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8179 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/exporters/abcexporter.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/exporters/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8641 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/exporters/export_manager.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/exporters/tvb_export.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/exporters/tvb_linked_export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.722702 tvb-rest-client-2.7.2/tvb/adapters/forms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4713 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/coupling_forms.py
--rw-r--r--   0 root         (0) root         (0)     7218 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/equation_forms.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/equation_plot_forms.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/form_with_ranges.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/integrator_forms.py
--rw-r--r--   0 root         (0) root         (0)    42072 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/model_forms.py
--rw-r--r--   0 root         (0) root         (0)    10872 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/monitor_forms.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/noise_forms.py
--rw-r--r--   0 root         (0) root         (0)    16528 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/simulator_fragments.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/surface_model_parameters_form.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/forms/transfer_vector_form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.723703 tvb-rest-client-2.7.2/tvb/adapters/simulator/
--rw-r--r--   0 root         (0) root         (0)     1275 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/simulator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7644 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/simulator/hpc_simulator_adapter.py
--rw-r--r--   0 root         (0) root         (0)     2664 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/simulator/range_parameters.py
--rw-r--r--   0 root         (0) root         (0)    14600 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/simulator/simulator_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.728703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/
--rw-r--r--   0 root         (0) root         (0)     1877 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11661 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/bids_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.728703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/brco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/brco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5884 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/brco/parser.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/brco_importer.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/connectivity_measure_importer.py
--rw-r--r--   0 root         (0) root         (0)     8851 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/csv_connectivity_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.729703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8434 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti/parser.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti_surface_importer.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti_timeseries_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.729703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat/parser.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py
--rw-r--r--   0 root         (0) root         (0)     9047 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat_timeseries_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.729703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/networkx_connectivity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/networkx_connectivity/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6830 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/networkx_connectivity/parser.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/networkx_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.730703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/nifti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/nifti/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3247 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/nifti/parser.py
--rw-r--r--   0 root         (0) root         (0)    10868 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/nifti_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.730703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj/parser.py
--rw-r--r--   0 root         (0) root         (0)     3863 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj/surface.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj_importer.py
--rw-r--r--   0 root         (0) root         (0)     7796 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/projection_matrix_importer.py
--rw-r--r--   0 root         (0) root         (0)     7637 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/region_mapping_importer.py
--rw-r--r--   0 root         (0) root         (0)     5676 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/sensors_importer.py
--rw-r--r--   0 root         (0) root         (0)    10129 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/tract_importer.py
--rw-r--r--   0 root         (0) root         (0)    10997 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/tumor_dataset_importer.py
--rw-r--r--   0 root         (0) root         (0)     7532 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/tvb_importer.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_connectivity_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.731703 tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_surface/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_surface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6443 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_surface/parser.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_surface_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.737703 tvb-rest-client-2.7.2/tvb/adapters/visualizers/
--rw-r--r--   0 root         (0) root         (0)     1955 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12080 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/annotations_viewer.py
--rw-r--r--   0 root         (0) root         (0)    21242 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/brain.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/complex_imaginary_coherence.py
--rw-r--r--   0 root         (0) root         (0)    24356 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/connectivity.py
--rw-r--r--   0 root         (0) root         (0)     3548 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/connectivity_edge_bundle.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/cross_coherence.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/cross_correlation.py
--rw-r--r--   0 root         (0) root         (0)    17334 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/eeg_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5293 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/fourier_spectrum.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/histogram.py
--rw-r--r--   0 root         (0) root         (0)     4662 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/ica.py
--rw-r--r--   0 root         (0) root         (0)     4520 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/local_connectivity_view.py
--rw-r--r--   0 root         (0) root         (0)     8139 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/matrix_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/pca.py
--rw-r--r--   0 root         (0) root         (0)     4768 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/pearson_cross_correlation.py
--rw-r--r--   0 root         (0) root         (0)     3969 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/pearson_edge_bundle.py
--rw-r--r--   0 root         (0) root         (0)    11964 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/phase_plane_interactive.py
--rw-r--r--   0 root         (0) root         (0)    17234 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/pse.py
--rw-r--r--   0 root         (0) root         (0)     4398 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/pse_discrete.py
--rw-r--r--   0 root         (0) root         (0)     8421 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/pse_isocline.py
--rw-r--r--   0 root         (0) root         (0)    25048 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/region_volume_mapping.py
--rw-r--r--   0 root         (0) root         (0)    10855 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/sensors.py
--rw-r--r--   0 root         (0) root         (0)    25212 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/surface_view.py
--rw-r--r--   0 root         (0) root         (0)     7919 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/time_series.py
--rw-r--r--   0 root         (0) root         (0)     8697 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/time_series_volume.py
--rw-r--r--   0 root         (0) root         (0)    11662 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/topographic.py
--rw-r--r--   0 root         (0) root         (0)     4565 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/tract.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/adapters/visualizers/wavelet_spectrogram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.737703 tvb-rest-client-2.7.2/tvb/config/
--rw-r--r--   0 root         (0) root         (0)     3095 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/algorithm_categories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.738703 tvb-rest-client-2.7.2/tvb/config/init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.738703 tvb-rest-client-2.7.2/tvb/config/init/alembic/
--rw-r--r--   0 root         (0) root         (0)     2389 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.739703 tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2466 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12427 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
--rw-r--r--   0 root         (0) root         (0)     9934 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/datatypes_registry.py
--rw-r--r--   0 root         (0) root         (0)     9460 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/initializer.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/introspector_registry.py
--rw-r--r--   0 root         (0) root         (0)     5505 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/init/model_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.740703 tvb-rest-client-2.7.2/tvb/config/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/logger/cluster_handler.py
--rw-r--r--   0 root         (0) root         (0)     3131 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/logger/dev_logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     2794 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/logger/logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     5741 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/config/profile_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.741703 tvb-rest-client-2.7.2/tvb/core/
--rw-r--r--   0 root         (0) root         (0)     1571 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.744704 tvb-rest-client-2.7.2/tvb/core/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22960 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/abcadapter.py
--rw-r--r--   0 root         (0) root         (0)     8032 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/abcdisplayer.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/abcremover.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/abcuploader.py
--rw-r--r--   0 root         (0) root         (0)     5639 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/arguments_serialisation.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/constants.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/adapters/inputs_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.744704 tvb-rest-client-2.7.2/tvb/core/code_versions/
--rw-r--r--   0 root         (0) root         (0)     1468 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/base_classes.py
--rw-r--r--   0 root         (0) root         (0)     3046 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.747704 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/
--rw-r--r--   0 root         (0) root         (0)     3101 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/4455_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/4750_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/5454_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/6093_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/6600_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/6728_update_code.py
--rw-r--r--   0 root         (0) root         (0)     9996 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/7350_update_code.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/7450_update_code.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/9444_update_code.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.748704 tvb-rest-client-2.7.2/tvb/core/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/exportable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.748704 tvb-rest-client-2.7.2/tvb/core/entities/file/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.750704 tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/
--rw-r--r--   0 root         (0) root         (0)    10820 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/002_update_files.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/003_update_files.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/004_update_files.py
--rw-r--r--   0 root         (0) root         (0)    69312 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/005_update_files.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11892 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/files_update_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.751704 tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/burst_configuration_h5.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/datatype_measure_h5.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/simulation_history_h5.py
--rw-r--r--   0 root         (0) root         (0)    12551 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/view_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.752704 tvb-rest-client-2.7.2/tvb/core/entities/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14738 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/filters/chain.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/filters/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/filters/factory.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/generic_attributes.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.753704 tvb-rest-client-2.7.2/tvb/core/entities/model/
--rw-r--r--   0 root         (0) root         (0)     1473 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5744 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/model/model_burst.py
--rw-r--r--   0 root         (0) root         (0)    16256 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/model/model_datatype.py
--rw-r--r--   0 root         (0) root         (0)    20454 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/model/model_operation.py
--rw-r--r--   0 root         (0) root         (0)     9071 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/model/model_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.755704 tvb-rest-client-2.7.2/tvb/core/entities/storage/
--rw-r--r--   0 root         (0) root         (0)     2179 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5541 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/burst_dao.py
--rw-r--r--   0 root         (0) root         (0)    26762 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/datatype_dao.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    23696 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/operation_dao.py
--rw-r--r--   0 root         (0) root         (0)    15007 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/project_dao.py
--rw-r--r--   0 root         (0) root         (0)     5571 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/root_dao.py
--rw-r--r--   0 root         (0) root         (0)    14395 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/session_maker.py
--rw-r--r--   0 root         (0) root         (0)     3353 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/storage/workflow_dao.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.755704 tvb-rest-client-2.7.2/tvb/core/entities/transient/
--rw-r--r--   0 root         (0) root         (0)     1291 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/transient/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11723 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/transient/context_overlay.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/transient/range_parameter.py
--rw-r--r--   0 root         (0) root         (0)    13225 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/entities/transient/structure_entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.756704 tvb-rest-client-2.7.2/tvb/core/neocom/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neocom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17618 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neocom/_h5loader.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neocom/_registry.py
--rw-r--r--   0 root         (0) root         (0)    11003 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neocom/h5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.758704 tvb-rest-client-2.7.2/tvb/core/neotraits/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18223 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/_h5accessors.py
--rw-r--r--   0 root         (0) root         (0)    15188 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/_h5core.py
--rw-r--r--   0 root         (0) root         (0)     4604 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/db.py
--rw-r--r--   0 root         (0) root         (0)    20754 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/forms.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/h5.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/spatial_model.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/uploader_view_model.py
--rw-r--r--   0 root         (0) root         (0)     3466 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/neotraits/view_model.py
--rw-r--r--   0 root         (0) root         (0)     5224 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/operation_async_launcher.py
--rw-r--r--   0 root         (0) root         (0)     6933 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/operation_hpc_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.758704 tvb-rest-client-2.7.2/tvb/core/project_versions/
--rw-r--r--   0 root         (0) root         (0)     1407 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/project_versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.759704 tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/
--rw-r--r--   0 root         (0) root         (0)     3200 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/1_update_project.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/2_update_project.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/3_update_project.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/removers_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.763704 tvb-rest-client-2.7.2/tvb/core/services/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17253 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/algorithm_service.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/authorization.py
--rw-r--r--   0 root         (0) root         (0)     3455 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/backend_client_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.764705 tvb-rest-client-2.7.2/tvb/core/services/backend_clients/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/backend_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/backend_clients/backend_client.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/backend_clients/cluster_scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)    20257 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/backend_clients/hpc_scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)    11834 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/backend_clients/standalone_client.py
--rw-r--r--   0 root         (0) root         (0)     4063 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/burst_config_serialization.py
--rw-r--r--   0 root         (0) root         (0)    18549 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/burst_service.py
--rw-r--r--   0 root         (0) root         (0)     1855 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/email_sender.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8322 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/figure_service.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/hpc_operation_service.py
--rw-r--r--   0 root         (0) root         (0)    36771 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/import_service.py
--rw-r--r--   0 root         (0) root         (0)    19683 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/operation_service.py
--rw-r--r--   0 root         (0) root         (0)    49272 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/project_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.764705 tvb-rest-client-2.7.2/tvb/core/services/resources/
--rw-r--r--   0 root         (0) root         (0)    20092 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/resources/branding_bar.png
--rw-r--r--   0 root         (0) root         (0)    21014 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/resources/branding_bar.svg
--rw-r--r--   0 root         (0) root         (0)    13153 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/settings_service.py
--rw-r--r--   0 root         (0) root         (0)    14266 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/simulator_service.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/texture_to_json.py
--rw-r--r--   0 root         (0) root         (0)    16498 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/services/user_service.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.764705 tvb-rest-client-2.7.2/tvb/interfaces/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.698701 tvb-rest-client-2.7.2/tvb/interfaces/rest/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.765704 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10489 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
--rw-r--r--   0 root         (0) root         (0)     8764 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.765704 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10056 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.766705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/client_decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.767705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/datatype/
--rw-r--r--   0 root         (0) root         (0)     5682 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/datatype/datatype_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.767705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/
--rw-r--r--   0 root         (0) root         (0)     7767 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/fire_simulation.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/launch_operation.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/utils.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/main_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.767705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/operation/
--rw-r--r--   0 root         (0) root         (0)     4096 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/operation/operation_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.768705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/project/
--rw-r--r--   0 root         (0) root         (0)     2868 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/project/project_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.768705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/simulator/
--rw-r--r--   0 root         (0) root         (0)     2500 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/simulator/simulation_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.768705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/tests/rest_test.py
--rw-r--r--   0 root         (0) root         (0)    11305 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/tvb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.768705 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/user/
--rw-r--r--   0 root         (0) root         (0)     4989 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/client/user/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.770705 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/decoders.py
--rw-r--r--   0 root         (0) root         (0)     5717 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/dtos.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/files_helper.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-01-04 05:55:06.000000 tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:47.771705 tvb-rest-client-2.7.2/tvb_rest_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4288 2023-01-04 06:21:47.000000 tvb-rest-client-2.7.2/tvb_rest_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13622 2023-01-04 06:21:47.000000 tvb-rest-client-2.7.2/tvb_rest_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 06:21:47.000000 tvb-rest-client-2.7.2/tvb_rest_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2023-01-04 06:21:47.000000 tvb-rest-client-2.7.2/tvb_rest_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-04 06:21:47.000000 tvb-rest-client-2.7.2/tvb_rest_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.567260 tvb-rest-client-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/MANIFEST_rest_client.in
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-05-23 12:09:33.566260 tvb-rest-client-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3716 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/README_rest_client.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:33.567260 tvb-rest-client-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.404252 tvb-rest-client-2.8.1/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.404252 tvb-rest-client-2.8.1/tvb/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.410252 tvb-rest-client-2.8.1/tvb/adapters/analyzers/
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8953 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_adapters.py
+-rw-r--r--   0 root         (0) root         (0)     9731 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_centrality_adapters.py
+-rw-r--r--   0 root         (0) root         (0)     5845 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_clustering_adapters.py
+-rw-r--r--   0 root         (0) root         (0)     8009 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_degree_adapters.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/cross_correlation_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    20045 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/fcd_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/fmri_balloon_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/fourier_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/ica_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/metrics_group_timeseries.py
+-rw-r--r--   0 root         (0) root         (0)     7956 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_coherence_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    11026 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_complex_coherence_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_covariance_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7446 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/pca_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    11610 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/analyzers/wavelet_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.413253 tvb-rest-client-2.8.1/tvb/adapters/creators/
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33529 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/allen_creator.py
+-rw-r--r--   0 root         (0) root         (0)    11384 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/connectivity_creator.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/local_connectivity_creator.py
+-rw-r--r--   0 root         (0) root         (0)    21351 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_base.py
+-rw-r--r--   0 root         (0) root         (0)     9827 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_creator.py
+-rw-r--r--   0 root         (0) root         (0)    12706 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/creators/stimulus_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.413253 tvb-rest-client-2.8.1/tvb/adapters/datatypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.421253 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/annotation.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/fcd.py
+-rw-r--r--   0 root         (0) root         (0)     5801 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/local_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mapped_value.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mode_decompositions.py
+-rw-r--r--   0 root         (0) root         (0)     3680 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/projections.py
+-rw-r--r--   0 root         (0) root         (0)     5471 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/region_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.424253 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_region_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2949 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_surface.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_timeseries.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_volume.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/sensors.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/simulation_history.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/spectral.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/structural.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/surface.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/temporal_correlations.py
+-rw-r--r--   0 root         (0) root         (0)    12512 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/tracts.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.433254 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/annotation_h5.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/connectivity_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/fcd_h5.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/graph_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/local_connectivity_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mapped_value_h5.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mode_decompositions_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/patterns_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/projections_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/region_mapping_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/sensors_h5.py
+-rw-r--r--   0 root         (0) root         (0)     8931 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/spectral_h5.py
+-rw-r--r--   0 root         (0) root         (0)     3663 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/structural_h5.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/surface_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/temporal_correlations_h5.py
+-rw-r--r--   0 root         (0) root         (0)    14867 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/time_series_h5.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/tracts_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/volumes_h5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.436254 tvb-rest-client-2.8.1/tvb/adapters/exporters/
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/abcexporter.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/export_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_export.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_linked_export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.442254 tvb-rest-client-2.8.1/tvb/adapters/forms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4713 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/coupling_forms.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/equation_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/equation_plot_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/form_with_ranges.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/integrator_forms.py
+-rw-r--r--   0 root         (0) root         (0)    42482 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/model_forms.py
+-rw-r--r--   0 root         (0) root         (0)    10872 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/monitor_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/noise_forms.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/simulator_fragments.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/surface_model_parameters_form.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/forms/transfer_vector_form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.444254 tvb-rest-client-2.8.1/tvb/adapters/simulator/
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7644 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/hpc_simulator_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/range_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    14600 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/simulator/simulator_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.452255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/bids_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.453255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5884 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/parser.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco_importer.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/connectivity_measure_importer.py
+-rw-r--r--   0 root         (0) root         (0)     8851 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/csv_connectivity_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.454255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8341 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/parser.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_surface_importer.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_timeseries_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.455255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py
+-rw-r--r--   0 root         (0) root         (0)     9047 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.456255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/parser.py
+-rw-r--r--   0 root         (0) root         (0)     5062 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.457255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3244 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/parser.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.458255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/parser.py
+-rw-r--r--   0 root         (0) root         (0)     3863 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/surface.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj_importer.py
+-rw-r--r--   0 root         (0) root         (0)     7796 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/projection_matrix_importer.py
+-rw-r--r--   0 root         (0) root         (0)     7637 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/region_mapping_importer.py
+-rw-r--r--   0 root         (0) root         (0)     5676 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/sensors_importer.py
+-rw-r--r--   0 root         (0) root         (0)    10129 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/tract_importer.py
+-rw-r--r--   0 root         (0) root         (0)    10997 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/tumor_dataset_importer.py
+-rw-r--r--   0 root         (0) root         (0)     7532 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/tvb_importer.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_connectivity_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.459255 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6445 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/parser.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.477256 tvb-rest-client-2.8.1/tvb/adapters/visualizers/
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12080 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/annotations_viewer.py
+-rw-r--r--   0 root         (0) root         (0)    21242 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/brain.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/complex_imaginary_coherence.py
+-rw-r--r--   0 root         (0) root         (0)    24356 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity_edge_bundle.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_correlation.py
+-rw-r--r--   0 root         (0) root         (0)    17334 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/eeg_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5293 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/fourier_spectrum.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/histogram.py
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/ica.py
+-rw-r--r--   0 root         (0) root         (0)     4520 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/local_connectivity_view.py
+-rw-r--r--   0 root         (0) root         (0)     8139 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/matrix_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pca.py
+-rw-r--r--   0 root         (0) root         (0)     4768 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_cross_correlation.py
+-rw-r--r--   0 root         (0) root         (0)     3969 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_edge_bundle.py
+-rw-r--r--   0 root         (0) root         (0)    11964 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/phase_plane_interactive.py
+-rw-r--r--   0 root         (0) root         (0)    17234 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_discrete.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_isocline.py
+-rw-r--r--   0 root         (0) root         (0)    25048 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/region_volume_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    10855 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    25212 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/surface_view.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series_volume.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/topographic.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/tract.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/adapters/visualizers/wavelet_spectrogram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.478256 tvb-rest-client-2.8.1/tvb/config/
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/algorithm_categories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.481256 tvb-rest-client-2.8.1/tvb/config/init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.481256 tvb-rest-client-2.8.1/tvb/config/init/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.484256 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/datatypes_registry.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/initializer.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/introspector_registry.py
+-rw-r--r--   0 root         (0) root         (0)     5505 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/init/model_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.486256 tvb-rest-client-2.8.1/tvb/config/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/cluster_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/dev_logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5445 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/elasticsearch_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/logger/logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5820 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/config/profile_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.489256 tvb-rest-client-2.8.1/tvb/core/
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.493257 tvb-rest-client-2.8.1/tvb/core/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22960 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcadapter.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcdisplayer.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcremover.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/abcuploader.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/arguments_serialisation.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/adapters/inputs_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.495257 tvb-rest-client-2.8.1/tvb/core/code_versions/
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/base_classes.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.499257 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4455_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4750_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/5454_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6093_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6600_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6728_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     9996 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7350_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7450_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/9444_update_code.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.502257 tvb-rest-client-2.8.1/tvb/core/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/exportable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.503257 tvb-rest-client-2.8.1/tvb/core/entities/file/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.507257 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/
+-rw-r--r--   0 root         (0) root         (0)    10820 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/002_update_files.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/003_update_files.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/004_update_files.py
+-rw-r--r--   0 root         (0) root         (0)    69315 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/005_update_files.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/files_update_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.510257 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/burst_configuration_h5.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/datatype_measure_h5.py
+-rw-r--r--   0 root         (0) root         (0)     6508 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/simulation_history_h5.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/view_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.512257 tvb-rest-client-2.8.1/tvb/core/entities/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14738 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/chain.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/filters/factory.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/generic_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.515258 tvb-rest-client-2.8.1/tvb/core/entities/model/
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_burst.py
+-rw-r--r--   0 root         (0) root         (0)    16256 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_datatype.py
+-rw-r--r--   0 root         (0) root         (0)    20454 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_operation.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/model/model_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.520258 tvb-rest-client-2.8.1/tvb/core/entities/storage/
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/burst_dao.py
+-rw-r--r--   0 root         (0) root         (0)    26852 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/datatype_dao.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    23487 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/operation_dao.py
+-rw-r--r--   0 root         (0) root         (0)    15003 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/project_dao.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/root_dao.py
+-rw-r--r--   0 root         (0) root         (0)    14395 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/session_maker.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/storage/workflow_dao.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.523258 tvb-rest-client-2.8.1/tvb/core/entities/transient/
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11723 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/context_overlay.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/range_parameter.py
+-rw-r--r--   0 root         (0) root         (0)    13225 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/entities/transient/structure_entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.525258 tvb-rest-client-2.8.1/tvb/core/neocom/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17618 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/_h5loader.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/_registry.py
+-rw-r--r--   0 root         (0) root         (0)    11003 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neocom/h5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.531258 tvb-rest-client-2.8.1/tvb/core/neotraits/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/_h5accessors.py
+-rw-r--r--   0 root         (0) root         (0)    15188 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/_h5core.py
+-rw-r--r--   0 root         (0) root         (0)     4592 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/db.py
+-rw-r--r--   0 root         (0) root         (0)    20754 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/h5.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/spatial_model.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/uploader_view_model.py
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/neotraits/view_model.py
+-rw-r--r--   0 root         (0) root         (0)     5224 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/operation_async_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     6933 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/operation_hpc_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.532259 tvb-rest-client-2.8.1/tvb/core/project_versions/
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.534259 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/1_update_project.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/2_update_project.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/3_update_project.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/removers_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.543259 tvb-rest-client-2.8.1/tvb/core/services/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17253 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/algorithm_service.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_client_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.545259 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/backend_client.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/cluster_scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)    20257 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/hpc_scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)    11834 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/backend_clients/standalone_client.py
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/burst_config_serialization.py
+-rw-r--r--   0 root         (0) root         (0)    18549 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/burst_service.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/email_sender.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8322 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/figure_service.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/hpc_operation_service.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/import_service.py
+-rw-r--r--   0 root         (0) root         (0)    19683 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/operation_service.py
+-rw-r--r--   0 root         (0) root         (0)    49199 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/project_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.546259 tvb-rest-client-2.8.1/tvb/core/services/resources/
+-rw-r--r--   0 root         (0) root         (0)    20092 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.png
+-rw-r--r--   0 root         (0) root         (0)    21014 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.svg
+-rw-r--r--   0 root         (0) root         (0)    13153 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/settings_service.py
+-rw-r--r--   0 root         (0) root         (0)    14266 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/simulator_service.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/texture_to_json.py
+-rw-r--r--   0 root         (0) root         (0)    16498 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/services/user_service.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.547259 tvb-rest-client-2.8.1/tvb/interfaces/
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.547259 tvb-rest-client-2.8.1/tvb/interfaces/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.550259 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)     8764 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.551259 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.553259 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/client_decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.553259 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/datatype/
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/datatype/datatype_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.555260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/
+-rw-r--r--   0 root         (0) root         (0)     7767 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/fire_simulation.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/launch_operation.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/main_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.555260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/operation/
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/operation/operation_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.556260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/project/
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/project/project_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.557260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/simulator/
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/simulator/simulation_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.558260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/rest_test.py
+-rw-r--r--   0 root         (0) root         (0)    11305 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tvb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.559260 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/user/
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/client/user/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.562260 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/decoders.py
+-rw-r--r--   0 root         (0) root         (0)     5717 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/dtos.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/files_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-23 11:37:04.000000 tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:33.565260 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13697 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:33.000000 tvb-rest-client-2.8.1/tvb_rest_client.egg-info/top_level.txt
```

### Comparing `tvb-rest-client-2.7.2/AUTHORS` & `tvb-rest-client-2.8.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/LICENSE` & `tvb-rest-client-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/PKG-INFO` & `tvb-rest-client-2.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-rest-client
-Version: 2.7.2
+Version: 2.8.1
 Summary: A helper package for preparing and sending requests towards the TVB REST API
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
```

### Comparing `tvb-rest-client-2.7.2/README.rst` & `tvb-rest-client-2.8.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 |
                 |
             tvb.config.init
                 |
                 |
             tvb.interfaces
 
-**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/4263723/files/tvb_data.zip?download=1.
+**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/7574266/files/tvb_data.zip?download=1.
 After download, unzip and execute `python setup.py develop` in the correct env.
 
 Usage
 -----
 
 To use TVB code, clone from GitHub (https://github.com/the-virtual-brain/tvb-root), or get from Pypi::
```

### Comparing `tvb-rest-client-2.7.2/README_rest_client.rst` & `tvb-rest-client-2.8.1/README_rest_client.rst`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/setup.py` & `tvb-rest-client-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import shutil
 
 import setuptools
 from setuptools.command.egg_info import manifest_maker
 
 manifest_maker.template = 'MANIFEST_rest_client.in'
 
-VERSION = "2.7.2"
+VERSION = "2.8.1"
 
 TVB_TEAM = "Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze"
 
 TVB_INSTALL_REQUIREMENTS = ["alembic", "h5py", "nibabel", "numpy", "Pillow", "psutil",
                             "pyAesCrypt", "requests", "scipy", "simplejson", "sqlalchemy",
                             "tvb-data", "tvb-gdist", "tvb-library", "tvb-storage", "werkzeug"]
```

### Comparing `tvb-rest-client-2.7.2/tvb/__init__.py` & `tvb-rest-client-2.8.1/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_adapters.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_centrality_adapters.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_centrality_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_clustering_adapters.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_clustering_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/bct_degree_adapters.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/bct_degree_adapters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/cross_correlation_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/cross_correlation_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 .. moduleauthor:: Stuart A. Knock <Stuart@tvb.invalid>
 .. moduleauthor:: Lia Domide <lia.domide@codemart.ro>
 .. moduleauthor:: Paula Popa <paula.popa@codemart.ro>
 
 """
 
 import uuid
-
 import numpy
-from scipy.signal.signaltools import correlate
+from scipy.signal import correlate
 from tvb.adapters.datatypes.db.graph import CorrelationCoefficientsIndex
 from tvb.adapters.datatypes.db.temporal_correlations import CrossCorrelationIndex
 from tvb.adapters.datatypes.db.time_series import TimeSeriesIndex, TimeSeriesEEGIndex, TimeSeriesMEGIndex, \
     TimeSeriesSEEGIndex
 from tvb.adapters.datatypes.h5.temporal_correlations_h5 import CrossCorrelationH5
 from tvb.basic.neotraits.api import Float
 from tvb.basic.neotraits.info import narray_describe
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/fcd_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/fcd_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/fmri_balloon_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/fmri_balloon_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/fourier_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/fourier_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/ica_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/ica_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/metrics_group_timeseries.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/metrics_group_timeseries.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/node_coherence_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_coherence_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,18 @@
             node_slice[1] = slice(var, var + 1)
             small_ts.data = time_series_h5.read_data_slice(tuple(node_slice))
             partial_coh = calculate_cross_coherence(small_ts, view_model.nfft)
             coherence_h5.write_data_slice(partial_coh)
 
         time_series_h5.close()
 
+        if partial_coh is None:
+            self.log.warn(f"Empty TS {input_shape[1]} ?")
+            return None
+
         partial_coh.source.gid = view_model.time_series
         partial_coh.gid = uuid.UUID(coherence_spectrum_index.gid)
 
         coherence_spectrum_index.fill_from_has_traits(partial_coh)
         self.fill_index_from_h5(coherence_spectrum_index, coherence_h5)
 
         coherence_h5.store(partial_coh, scalars_only=True)
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/node_complex_coherence_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_complex_coherence_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/node_covariance_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/node_covariance_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/pca_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/pca_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/analyzers/wavelet_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/analyzers/wavelet_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/allen_creator.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/allen_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/connectivity_creator.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/connectivity_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     new_tracts = NArray(
         default=None,
         label="Tracts json array",
         required=True,
         doc="""""")
 
     interest_area_indexes = NArray(
-        dtype=numpy.int,
+        dtype=numpy.int_,
         default=None,
         label="Indices of selected nodes as json array",
         required=True,
         doc="""""")
 
     is_branch = Attr(
         field_type=bool,
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/local_connectivity_creator.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/local_connectivity_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/siibra_base.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,74 +28,107 @@
 Utility functions for using siibra to extract Structural and Functional connectivities
 
 .. moduleauthor:: Romina Baila <romina.baila@codemart.ro>
 """
 import numpy as np
 import siibra
 from enum import Enum
-from nibabel import Nifti1Image
 from tvb.basic.logger.builder import get_logger
 from tvb.datatypes import connectivity
 from tvb.datatypes.graph import ConnectivityMeasure
 
 LOGGER = get_logger(__name__)
 
 DEFAULT_ATLAS = 'Multilevel Human Atlas'
 DEFAULT_PARCELLATION = 'Julich-Brain Cytoarchitectonic Maps 2.9'
+DEFAULT_COHORT = 'HCP'
+THOUSAND_BRAINS_COHORT = '1000BRAINS'
 
 
 class Component2Modality(Enum):
-    WEIGHTS = siibra.modalities.StreamlineCounts
-    TRACTS = siibra.modalities.StreamlineLengths
-    FC = siibra.modalities.FunctionalConnectivity
+    WEIGHTS = siibra.features.connectivity.StreamlineCounts
+    TRACTS = siibra.features.connectivity.StreamlineLengths
+    FUNCTIONAL_CONNECTIVITY = siibra.features.connectivity.FunctionalConnectivity
+
+
+# ########################################## SIIBRA CREATOR INITIALIZATION #############################################
+def get_cohorts_for_sc(parcellation_name):
+    """
+    Given a parcellation name, return the name of all the cohorts related to it and containing data about
+    Structural Connectivities. We chose to return the options for Struct. Conn., as, for the moment, the same values
+    are returned for Functional Conn.
+    """
+    parcellation = siibra.parcellations[parcellation_name]
+    features = siibra.features.get(parcellation, siibra.features.connectivity.StreamlineCounts)
+    return [f.cohort.upper() for f in features]
 
 
 # ######################################## SIIBRA PARAMETERS CONFIGURATION #############################################
 def check_atlas_parcellation_compatible(atlas, parcellation):
     """ Given an atlas and a parcellation, verify that the atlas contains the parcellation, i.e. they are compatible """
     return parcellation in list(atlas.parcellations)
 
 
 def get_atlases_for_parcellation(parcelation):
     """ Given a parcelation, return all the atlases that contain it """
-    return list(parcelation.atlases)
+    atlases = siibra.atlases
+    atlases = [a for a in atlases if parcelation in list(a.parcellations)]
+    return atlases
 
 
 def get_parcellations_for_atlas(atlas):
     """ Given the name of an atlas, return all the parcellations inside it """
     return list(atlas.parcellations)
 
 
-def parse_subject_ids(subject_ids):
+def parse_subject_ids(subject_ids, cohort):
     """
     Given a string representing subject ids or a range of subject ids; return the list containing all the included ids
     """
-    parsed_ids = []
+    parsed_ids_as_str = []
     individual_splits = subject_ids.split(';')
-    for s in individual_splits:
-        # if a range was written
-        if '-' in s:
-            start, end = s.split('-')
-            start_int = int(start)
-            end_int = int(end) + 1  # so that the last element in range is also included
-            ids_list_from_range = list(range(start_int, end_int))
-            parsed_ids.extend(ids_list_from_range)
-        else:
-            s_int = int(s)
-            parsed_ids.append(s_int)
 
-    # convert the subject ids list back to strings into the required format
-    parsed_ids_strings = [str(id).zfill(3) for id in parsed_ids]
-    return parsed_ids_strings
+    if cohort == THOUSAND_BRAINS_COHORT:
+        for s in individual_splits:
+            parsed_ids_as_str.append(s)
+    elif cohort == DEFAULT_COHORT:
+        parsed_ids = []
+        for s in individual_splits:
+            # if a range was written
+            if '-' in s:
+                start, end = s.split('-')
+                start_int = int(start)
+                end_int = int(end) + 1  # so that the last element in range is also included
+                ids_list_from_range = list(range(start_int, end_int))
+                parsed_ids.extend(ids_list_from_range)
+            else:
+                s_int = int(s)
+                parsed_ids.append(s_int)
+
+        # convert the subject ids list back to strings into the required format
+        parsed_ids_as_str = [str(id).zfill(3) for id in parsed_ids]
 
+    return parsed_ids_as_str
 
-def init_siibra_params(atlas_name, parcellation_name, subject_ids):
+
+def init_siibra_params(atlas_name, parcellation_name, cohort_name, subject_ids):
+    """
+    Initialize siibra parameters (if some were not given) and check the compatibility of the provided parameters.
+    :param: atlas_name - name of atlas as str
+    :param: parcellation_name - name of parcellation as str
+    :param: cohort_name - name of cohort as str
+    :param: subject_ids - list of unparsed subject ids given as str
+    :return: (atlas, parcellation, cohort_name, subject_ids) - tuple containing a siibra atlas object,
+    a siibra parcellation object and a cohort name all compatible with each other and a list of parsed ids
+    """
+    # check that the atlas and the parcellation exist within siibra
     atlas = siibra.atlases[atlas_name] if atlas_name else None
     parcellation = siibra.parcellations[parcellation_name] if parcellation_name else None
 
+    # check compatibility of atlas and parcellation
     if atlas and parcellation:
         compatible = check_atlas_parcellation_compatible(atlas, parcellation)
         if not compatible:
             raise ValueError(f'Atlas \'{atlas.name}\' does not contain parcellation \'{parcellation.name}\'. '
                              f'Please choose a different atlas and/or parcellation.')
 
     if atlas and not parcellation:
@@ -124,322 +157,281 @@
     if not atlas and not parcellation:
         LOGGER.warning(f'No atlas and no parcellation were provided, so default ones will be selected.')
         atlas = siibra.atlases[DEFAULT_ATLAS]
         parcellation = siibra.parcellations[DEFAULT_PARCELLATION]
 
     LOGGER.info(f'Using atlas {atlas.name} and parcellation {parcellation.name}')
 
+    # check the compatibility of cohort and parcellation
+    cohort_options = get_cohorts_for_sc(parcellation.name)
+    if cohort_name is None:
+        cohort_name = DEFAULT_COHORT
+    elif cohort_name not in cohort_options:
+        raise ValueError(f'The cohort \"{cohort_name}\" is not available for parcellation \"{parcellation.name}\"!')
+
+    # check subject ids
     if not subject_ids:
         LOGGER.info(
-            f'No list of subject ids was provided, so the connectivities will be computed for all available subjects!')
-        subject_ids = 'all'
-    elif subject_ids != 'all':
-        subject_ids = parse_subject_ids(subject_ids)
-
-    return atlas, parcellation, subject_ids
-
-
-# ################################################# SIIBRA METHODS #####################################################
-def compute_centroids(region, space):
-    """
-    Compute the centroids of a region in a specified space.
-    It is the uncached and slightly modified version of siibra.core.region.spatial_props.
-    """
-    from skimage import measure
-
-    if not region.mapped_in_space(space):
-        raise RuntimeError(
-            f"Spatial properties of {region.name} cannot be computed in {space.name}. "
-            "This region is only mapped in these spaces: "
-            ", ".join(s.name for s in region.supported_spaces)
-        )
-
-    # build binary mask of the image
-    pimg = build_mask_for_centroids(region=region, space=space)
-
-    # compute properties of labelled volume
-    A = np.asarray(pimg.get_fdata(), dtype=np.int32).squeeze()
-    C = measure.label(A)
-
-    # compute centroid only for the first connected component of the region
-    nonzero = np.c_[np.nonzero(C == 1)]
-    centroid = siibra.Point(np.dot(pimg.affine, np.r_[nonzero.mean(0), 1])[:3], space=space)
-    # tuple() gives the coordinate of the centroid
-    centroid_coord = tuple(centroid)
-
-    return centroid_coord
-
-
-def build_mask_for_centroids(region, space, resolution_mm=None, maptype: siibra.MapType = siibra.MapType.LABELLED,
-                             threshold_continuous=None, consider_other_types=True):
-    """
-    Returns a mask for the specified region in the specified space.
-    It is the uncached version of siibra.core.region.build_mask
-    """
-    spaceobj = siibra.core.Space.REGISTRY[space]
-    if spaceobj.is_surface:
-        raise NotImplementedError(
-            "Region masks for surface spaces are not yet supported."
-        )
-
-    mask = None
-    if isinstance(maptype, str):
-        maptype = siibra.MapType[maptype.upper()]
-
-    if region.has_regional_map(spaceobj, maptype):
-        # the region has itself a map of that type linked
-        mask = region.get_regional_map(space, maptype).fetch(
-            resolution_mm=resolution_mm
-        )
+            f'The mean across all connectivities from cohort {cohort_name} will be computed.')
+        subject_ids = [None]
     else:
-        # retrieve  map of that type from the region's corresponding parcellation map
-        parcmap = region.parcellation.get_map(spaceobj, maptype)
-        mask = parcmap.fetch_regionmap(region, resolution_mm=resolution_mm)
-
-    if mask is None:
-        # Attempt to produce a map from the child regions.
-        # We only accept this if all child regions produce valid masks.
-        # NOTE We ignore extension regions here, since this is a complex case currently (e.g. iam regions in BigBrain)
-        LOGGER.debug(f"Merging child regions to build mask for their parent {region.name}:")
-        maskdata = None
-        affine = None
-        for c in region.children:
-            if c.extended_from is not None:
-                continue
-            childmask = build_mask_for_centroids(c, space, resolution_mm, maptype, threshold_continuous)
-            if childmask is None:
-                LOGGER.warning(f"No success getting mask for child {c.name}")
-                break
-            if maskdata is None:
-                affine = childmask.affine
-                maskdata = np.asanyarray(childmask.dataobj)
-            else:
-                assert (childmask.affine == affine).all()
-                maskdata = np.maximum(maskdata, np.asanyarray(childmask.dataobj))
-        else:
-            # we get here only if the for loop was not interrupted by 'break'
-            if maskdata is not None:
-                return Nifti1Image(maskdata, affine)
-
-    if mask is None:
-        # No map of the requested type found for the region.
-        LOGGER.warn(
-            f"Could not compute {maptype.name.lower()} mask for {region.name} in {spaceobj.name}."
-        )
-        if consider_other_types:
-            for other_maptype in (set(siibra.MapType) - {maptype}):
-                mask = region.build_mask(
-                    space, resolution_mm, other_maptype, threshold_continuous, consider_other_types=False
-                )
-                if mask is not None:
-                    LOGGER.info(
-                        f"A mask was generated from map type {other_maptype.name.lower()} instead."
-                    )
-                    return mask
-        return None
-
-    if (threshold_continuous is not None) and (maptype == siibra.MapType.CONTINUOUS):
-        data = np.asanyarray(mask.dataobj) > threshold_continuous
-        LOGGER.info(f"Mask built using a continuous map thresholded at {threshold_continuous}.")
-        assert np.any(data > 0)
-        mask = Nifti1Image(data.astype("uint8").squeeze(), mask.affine)
-
-    return mask
-
-
-# ######################################## COMMON CONNECTIVITY METHODS #################################################
-def get_connectivity_component(parcellation, component):
-    # type: (str, Component2Modality) -> []
-    """
-        :return: a list of all available connectivity components (weights/tract lengths)
-    """
-    modality = component.value
-    all_conns = siibra.get_features(parcellation, modality)
+        subject_ids = parse_subject_ids(subject_ids, cohort_name)
 
-    if len(all_conns) == 0:
-        raise AttributeError(f'No connectivity component \'{Component2Modality(component).name}\' was found '
-                             f'in parcellation \'{parcellation}\'!')
-    return all_conns
+    return atlas, parcellation, cohort_name, subject_ids
 
 
+# ############################################# CONNECTIVITY METHODS ###################################################
 def get_hemispheres_for_regions(region_names):
-    """ Given a list of region names, compute the hemispheres to which they belon to """
+    """
+    Given a list of region names, compute the hemispheres to which they belon to. 0 means the region belongs to the left
+    hemisphere, 1 means it belongs to the right hemisphere (according to TVB convention).
+    :param: region_names - list of str containing the names of the regions
+    :return: hemi - list of ints indicating the hemisphere for each region in `region_names`
+    """
     LOGGER.info(f'Computing hemispheres for regions')
     hemi = []
     for name in region_names:
         if 'right' in name:
             hemi.append(1)
         # TODO: regions referring to both hemispheres are put in the left hemisphere; change this?
         else:
             hemi.append(0)
 
     return hemi
 
 
 def get_regions_positions(regions):
-    """ Given a list of regions, compute the positions of their centroids """
+    """
+    Given a list of siibra regions, compute the positions of their centroids.
+    :param: regions - list of siibra region objects
+    :return: positions - list of tuples; each tuple represents the position of a region in `regions` and contains
+    3 floating point coordinates
+    """
     LOGGER.info(f'Computing positions for regions')
     positions = []
-    space = siibra.spaces.MNI152_2009C_NONL_ASYM  # commonly used space in the documentation
+    space = siibra.spaces.MNI_152_ICBM_2009C_NONLINEAR_ASYMMETRIC  # commonly used space in the documentation
 
     for r in regions:
-        centroid = compute_centroids(r, space)
+        centroid = r.spatial_props(space)['components'][0]['centroid'].coordinate
         positions.append(centroid)
 
     return positions
 
 
 # ###################################### STRUCTURAL CONNECTIVITY METHODS ###############################################
-def filter_structural_connectivity_by_id(weights, tracts, subj_ids):
+def get_connectivity_matrix(parcellation, cohort, subjects, component):
+    # type: (siibra.core.parcellation.Parcellation, str, list, Component2Modality) -> {}
     """
-    Given two lists of connectivity weights and tract lengths and a list of subject ids, keep only the weights and
-    tracts for those subjects
+    Retrieve the structural connectivity components (weights/tracts) for all the subjects provided, for the specified
+    parcellation and cohort. The matrices are returned inside a dictionary, where the keys are the subject ids and the
+    values represent the connectivity matrix.
+    :param: parcellation - siibra Parcellation object for which we compute the connectivity matrices
+    :param: cohort - name of cohort for which we compute the connectivity matrices
+    :param: subjects - list containing the subject ids as strings
+    :param: component - enum value specifying the connectivity component we want, weights or tracts
+    return: conn_matrices - dict containing the conn. matrices (values) for the specified subject ids (keys)
     """
-    filtered_weights = []
-    filtered_tracts = []
-
-    for subj in subj_ids:
-        weight = [w for w in weights if w.subject == subj]
-        tract = [t for t in tracts if t.subject == subj]
-
-        filtered_weights += weight
-        filtered_tracts += tract
+    modality = component.value
+    features = siibra.features.get(parcellation, modality)
+    conn_for_cohort = None  # conn. obj. (StreamlineCounts/StreamlineLengths) for specified cohort
+    conn_matrices = {}  # dict containing connectivity matrices for the specified users
+    # select the connectivities for the specific cohort
+    for f in features:
+        if f.cohort == cohort:
+            conn_for_cohort = f
+            break
+
+    if conn_for_cohort is None:
+        LOGGER.info("NO conn_for_cohort was found")
+        return conn_matrices
+
+    # for 1000BRAINS cohort, if the user did not specify a suffix (_1, _2), get all the possible ids for that subject
+    if cohort == THOUSAND_BRAINS_COHORT and subjects is not None:
+        subjects = [s for s in sorted(conn_for_cohort.subjects) if any(x in s for x in subjects)]
+
+    # get the conn. matrices for each specified subject
+    for s in subjects:
+        if s is None:
+            s = 'mean'
+        matrix = conn_for_cohort.get_matrix(s)
+        conn_matrices[s] = matrix
+        LOGGER.info(f'{component.name} for subject {s} retrieved successfully.')
 
-    return filtered_weights, filtered_tracts
+    return conn_matrices
 
 
 def create_tvb_structural_connectivity(weights_matrix, tracts_matrix, region_names, hemispheres, positions):
-    """ Compute a TVB Connectivity based on its components obtained from siibra """
-
+    # type: (pandas.DataFrame, pandas.DataFrame, list, list, list) -> tvb.datatypes.connectivity.Connectivity
+    """
+    Create and configure a TVB Connectivity, based on its components obtained from siibra.
+    :param: weights_matrix - pandas.DataFrame matrix for weights; obtained from siibra
+    :param: tracts_matrix - pandas.DataFrame matrix for tracts; obtained from siibra
+    :param: region_names - list of str containing the names of the regions for which the connectivity is computed
+    :param: hemispheres - list of ints, corresponding to the hemisphere that each region from `region_names belongs to
+    :param: positions - list of tuples, corresponding to region coordinates for each region from `region_names`
+    :return: conn - a tvb.datatypes.connectivity.Connectivity object
+    """
     conn = connectivity.Connectivity()
     conn.weights = weights_matrix.to_numpy()
     conn.tract_lengths = tracts_matrix.to_numpy()
     conn.region_labels = np.array(region_names)
     conn.hemispheres = np.array(hemispheres, dtype=np.bool_)
     conn.centres = np.array(positions)
 
     conn.configure()
     return conn
 
 
-def get_tvb_connectivities_from_kg(atlas=None, parcellation=None, subject_ids=None):
+def get_structural_connectivities_from_kg(atlas=None, parcellation=None, cohort=None, subject_ids=None):
     """
-    Return a list of TVB Structural Connectivities, based on the specified atlas and parcellation,
-    for the subjects mentioned in 'subject_ids'
+    Return a dictionary of TVB Structural Connectivities using data from siibra and the KG, based on the specified
+    atlas, parcelation and cohort, and for the specified subjects
+    :param: atlas - str specifying the atlas name
+    :param: parcellation - str specifying the parcellation name
+    :param: cohort - str specifying the cohort name
+    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be computed
+    :return: connectivities - dict containing tvb structural Connectivities as values and the subject ids as keys
     """
-    atlas, parcellation, subject_ids = init_siibra_params(atlas, parcellation, subject_ids)
+    atlas, parcellation, cohort, subject_ids = init_siibra_params(atlas, parcellation, cohort, subject_ids)
     connectivities = {}
-    weights = get_connectivity_component(parcellation, Component2Modality.WEIGHTS)
-    tracts = get_connectivity_component(parcellation, Component2Modality.TRACTS)
-
-    if not weights or not tracts:
-        raise AttributeError(f'Could not find both weights and tract lengths from parcellation \'{parcellation.name}\', '
-                             f'so a connectivity cannot be computed')
-
-    if subject_ids != 'all':
-        weights, tracts = filter_structural_connectivity_by_id(weights, tracts, subject_ids)
+    weights = get_connectivity_matrix(parcellation, cohort, subject_ids, Component2Modality.WEIGHTS)
+    tracts = get_connectivity_matrix(parcellation, cohort, subject_ids, Component2Modality.TRACTS)
 
     # regions are the same for all weights and tract lengths matrices, so they can be computed only once
-    regions = weights[0].matrix.index.values
+    regions = list(weights.values())[0].index.values
+    # because siibra sometimes returns tuples instead of actual regions, change list to contain only regions
+    regions = [r[1] if type(r) == tuple else r for r in regions]
     region_names = [r.name for r in regions]
     hemi = get_hemispheres_for_regions(region_names)
     positions = get_regions_positions(regions)
 
     LOGGER.info(f'Computing TVB Connectivities')
-    no_conns = min(len(weights), len(tracts))  # in siibra v0.3a24 weights have additional subjects
-    for i in range(no_conns):
-        weights_matrix = weights[i].matrix
-        tracts_matrix = tracts[i].matrix
-        conn = create_tvb_structural_connectivity(weights_matrix, tracts_matrix, region_names, hemi, positions)
-        subj = weights[i].subject
+    for subject, matrix in weights.items():
+        weights_matrix = matrix
+        tracts_matrix = tracts[subject]
+        tvb_conn = create_tvb_structural_connectivity(weights_matrix, tracts_matrix, region_names, hemi, positions)
 
         # structural connectivities stored as dict, to link a functional connectivity with the correct
         # structural connectivity when creating connectivity measures
-        connectivities[subj] = conn
+        connectivities[subject] = tvb_conn
 
     return connectivities
 
 
 # #################################### FUNCTIONAL CONNECTIVITY METHODS #################################################
-
-def filter_functional_connectivity_by_id(fcs, subj_ids):
-    """
-    Given a list of functional connectivities and a list of subject ids, keep only the functional connectivities
-    for those subjects
+def get_functional_connectivity_matrix(parcellation, cohort, subject):
     """
-    filtered_fcs = []
-
-    for subj in subj_ids:
-        fc = [f for f in fcs if f.subject == subj]
-        filtered_fcs += fc
+    Get all the functional connectivities for the specified parcellation, cohort and just ONE specific subject;
+    In v0.4a35 of siibra, functional connectivities belonging to the same cohort can be split into multiple (5)
+    siibra FunctionalConnectivity objects
+    :param: parcellation - siibra Parcellation object
+    :param: cohort - str specifying the cohort name
+    :param: subject - str specifying exactly one subject id
+    :return: (fcs_list, fcs_names_list) - tuple containing 2 lists; `fcs_list` contains pandas.Dataframe matrices and
+    `fcs_names_list` contains the name for each matrix from the previous list, obtained from the file they are stored
+    in in the KG
+    """
+    modality = Component2Modality.FUNCTIONAL_CONNECTIVITY.value
+    features = siibra.features.get(parcellation, modality)
+    fcs_list = []  # the FC matrices
+    fcs_names_list = []  # the name of the files containing the FC matrices in fcs_list
+
+    for f in features:
+        if f.cohort == cohort:
+            fc_matrix = f.get_matrix(subject)
+            fcs_names_list.append(f._files[subject])
+            fcs_list.append(fc_matrix)
 
-    return filtered_fcs
+    return fcs_list, fcs_names_list
 
 
 def get_fc_name_from_file_path(path_to_file):
     """
     Given the entire path to a file containing a siibra FunctionalConnectivity, return just the filename
-    Note: highly dependent on EBRAINS/siibra storage conventions
+    Note: highly dependent on KG/siibra storage conventions
+    :param: path_to_file - str representing the path to a Functional Connectivity from the KG
+    :return: filename - just the filename (without the extension)
     """
     file_with_extension = path_to_file.rsplit('/', 1)[1]
     filename = file_with_extension.rsplit('.', 1)[0]
 
     return filename
 
 
-def create_tvb_connectivity_measure(siibra_fc, structural_connectivity):
+def create_tvb_connectivity_measure(siibra_fc, structural_connectivity, siibra_fc_filename):
     """
-    Given a FunctionalConnectivity from  siibra for a subject and its corresponding TVB Structural Connectivity
-    (for the same subject), return a TVB ConnectivityMeasure having as data the siibra FC
+    Given a FunctionalConnectivity from siibra TVB Structural Connectivity (both for the same subject),
+    return a TVB ConnectivityMeasure containing those 2 connectivities
+    :param: siibra_fc - pandas.Dataframe matrix from siibra containing a functional connectivity
+    :param: structural_connectivity - a TVB structural connectivity
+    :param: siibra_fc_filename - the name of the file containing the functional connectivity from siibra
+    :return: conn_measure - tvb.datatypes.graph.ConnectivityMeasure representing a functional connectivity
     """
-    fc_matrix = siibra_fc.matrix.to_numpy()
+    fc_matrix = siibra_fc.to_numpy()
     conn_measure = ConnectivityMeasure(array_data=fc_matrix, connectivity=structural_connectivity)
-    fc_name = get_fc_name_from_file_path(siibra_fc.filename)
-    conn_measure.title = fc_name
+    conn_measure.title = get_fc_name_from_file_path(siibra_fc_filename)
 
     return conn_measure
 
 
-def get_connectivity_measures_from_kg(atlas=None, parcellation=None, subject_ids=None, structural_connectivities=None):
-    atlas, parcellation, subject_ids = init_siibra_params(atlas, parcellation, subject_ids)
+def get_connectivity_measures_from_kg(atlas=None, parcellation=None, cohort=None, subject_ids=None,
+                                      structural_connectivities=None):
+    """
+    Return a dictionary of TVB Connectivity Measures using data from siibra and the KG, based on the specified
+    atlas, parcelation and cohort, and for the specified subjects
+    :param: atlas - str specifying the atlas name
+    :param: parcellation - str specifying the parcellation name
+    :param: cohort - str specifying the cohort name
+    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be computed
+    :param: structural_connectivities - dict of TVB Structural Connectivities computed for the subjects from
+    `subject_ids`, where subject ids are keys and the structural connectivities are values
+    :return: conn_measures - dict containing TVB Connectivity Measures as values and the subject ids as keys
+    """
+    atlas, parcellation, cohort, subject_ids = init_siibra_params(atlas, parcellation, cohort, subject_ids)
     conn_measures = {}
 
-    fcs = get_connectivity_component(parcellation, Component2Modality.FC)
-
-    if not fcs:
-        LOGGER.error(
-            f'Could not find any functional connectivity in parcellation {parcellation.name}, so a TVB Functional '
-            f'Connectivity cannot be computed')
-        return
-
-    if subject_ids != 'all':
-        fcs = filter_functional_connectivity_by_id(fcs, subject_ids)
-
-    for fc in fcs:
-        subject = fc.subject
-
-        # the conn measures are kept in a list, as there are multiple conn measures for the same subject
-        if subject not in conn_measures.keys():
-            conn_measures[subject] = []
-        sc = structural_connectivities[subject]
-        conn_measure = create_tvb_connectivity_measure(fc, sc)
-
-        # conn. measures kept as dict to be able to set the subject on GenericAttributes in SiibraCreator
-        conn_measures[subject].append(conn_measure)
+    # for 1000BRAINS cohort, if the user did not specify a suffix (_1, _2), get all the possible ids for that subject
+    if cohort == THOUSAND_BRAINS_COHORT and any('_' not in s for s in subject_ids):
+        f = [f for f in siibra.features.get(parcellation, siibra.features.connectivity.FunctionalConnectivity)
+             if f.cohort == THOUSAND_BRAINS_COHORT]
+        f = f[0]  # get the first feature from the feature list, we just want to know the subject names
+        subjects_for_cohort = f.subjects
+        subject_ids = [s for s in sorted(subjects_for_cohort) if any(x in s for x in subject_ids)]
+
+    for s in subject_ids:
+        if s is None:
+            s = 'mean'
+        conn_measures[s] = []
+        sc = structural_connectivities[s]
+
+        fcs, fcs_names = get_functional_connectivity_matrix(parcellation, cohort, s)
+
+        # create a tvb conn measure from a siibra fc and append it in the final dict for the specified subject
+        for i in range(len(fcs)):
+            conn_measure = create_tvb_connectivity_measure(fcs[i], sc, fcs_names[i])
+            conn_measures[s].append(conn_measure)
 
     return conn_measures
 
 
 # ################################################# FINAL API ##########################################################
-
-
-def get_connectivities_from_kg(atlas=None, parcellation=None, subject_ids=None, compute_fc=False):
+def get_connectivities_from_kg(atlas=None, parcellation=None, cohort=DEFAULT_COHORT,
+                               subject_ids=None, compute_fc=False):
     """
     Compute the TVB Structural Connectivities and optionally Functional Connectivities for the selected subjects
+    :param: atlas - str specifying the atlas name
+    :param: parcellation - str specifying the parcellation name
+    :param: cohort - str specifying the cohort name
+    :param: subject_ids - unparsed str specifying the subject ids for which the connectivities will be computed
+    :param: compute_fc - boolean value indicating if for the specified subjects the functional connectivities should
+    also be retrieved
+    :return: (sc_dict, conn_measures_dict) - tuple containing 2 dictionaries: one with structural connectivities and
+    one for functional connectivities; for each dictionary, the keys are the subject ids and the values are the
+    connectivities
     """
     conn_measures_dict = {}
-    sc_dict = get_tvb_connectivities_from_kg(atlas, parcellation, subject_ids)
+    sc_dict = get_structural_connectivities_from_kg(atlas, parcellation, cohort, subject_ids)
 
     if compute_fc:
-        conn_measures_dict = get_connectivity_measures_from_kg(atlas, parcellation, subject_ids, sc_dict)
+        conn_measures_dict = get_connectivity_measures_from_kg(atlas, parcellation, cohort, subject_ids, sc_dict)
 
     return sc_dict, conn_measures_dict
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/siibra_creator.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/siibra_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,31 +53,30 @@
     """
     # should use `atlases = [a.name for a in list(siibra.atlases)]`, but only the default one has data
     atlases = [siibra_base.DEFAULT_ATLAS]  # list with atlases names
     # should get only valid parcellations for default atlas, but only newest version of Julich parcellation
     # has data and corresponds with the current API of siibra
     parcellations = [siibra_base.DEFAULT_PARCELLATION]
 
-    atlas_dict = {}
-    parcellation_dict = {}
+    # get available cohorts
+    cohorts = siibra_base.get_cohorts_for_sc(parcellations[0])
 
-    for a_name in atlases:
-        atlas_dict[a_name] = a_name
-
-    for p_name in parcellations:
-        parcellation_dict[p_name] = p_name
+    atlas_dict = {a_name: a_name for a_name in atlases}
+    parcellation_dict = {p_name: p_name for p_name in parcellations}
+    cohort_dict = {(y := c_name.upper()): y for c_name in cohorts}
 
     atlas_options = TVBEnum('AtlasOptions', atlas_dict)
     parcellation_options = TVBEnum('ParcellationOptions', parcellation_dict)
+    cohort_options = TVBEnum('CohortOptions', cohort_dict)
 
-    return atlas_options, parcellation_options
+    return atlas_options, parcellation_options, cohort_options
 
 
 if 'SIIBRA_INIT_DONE' not in globals():
-    ATLAS_OPTS, PARCELLATION_OPTS = init_siibra_options()
+    ATLAS_OPTS, PARCELLATION_OPTS, COHORT_OPTS = init_siibra_options()
     SIIBRA_INIT_DONE = True
 
 
 class SiibraModel(ViewModel):
     ebrains_token = Str(
         label='EBRAINS token',
         required=True,
@@ -96,26 +95,43 @@
         field_type=PARCELLATION_OPTS,
         default=PARCELLATION_OPTS[siibra_base.DEFAULT_PARCELLATION],
         label='Parcellation',
         required=True,
         doc='Parcellation to be used (only TVB compatible ones listed here)'
     )
 
+    cohort = EnumAttr(
+        field_type=COHORT_OPTS,
+        default=COHORT_OPTS[siibra_base.DEFAULT_COHORT],
+        label='Cohort',
+        required=True,
+        doc='Cohort to be used'
+    )
+
     subject_ids = Str(
         label='Subjects',
         required=True,
         default='000',
-        doc="""The list of all subject IDs for which the structural and optionally functional connectivities
-        The IDs can be specified in 3 ways: <br/>
-        1. individually, delimited by a semicolon symbol: 000;001;002<br/>
+        doc="""The list of all subject IDs for which the structural and optionally functional connectivities are 
+        computed. Depending on the selected cohort, you can specify the IDs in the following ways: <br/>
+        a) For the "HCP" cohort, the subject IDs are: 000,001,002, etc. Each subject has exactly one 
+        subject ID associated to them. Thus, there are 3 ways to specify the IDs:<br/>
+        1. individually, delimited by a semicolon symbol: 000;001;002. <br/>
         2. As a range, specifying the first and last IDs: 000-050 will retrieve all the subjects starting with 
-        subject 000 until subject 050 (51 subjects)<br/>
+        subject 000 until subject 050 (51 subjects). <br/>
         A combination of the 2 methods is also supported: 000-005;010 will retrieve all the subjects starting with 
-        subject 000 until subject 005 (6 subjects) AND subject 010 (so 7 subjects in total)<br/>
-        3. Using the keyword 'all' (without apostrophes) to get the connectivities for all the available subjects """)
+        subject 000 until subject 005 (6 subjects) AND subject 010 (so 7 subjects in total)<br/> <br/>
+        b) For "1000BRAINS" cohort, the subject IDs are: 0001_1, 0001_2, 0002_1, 0002_2, etc. Each subject can have 
+        multiple subjects IDs associated to them, indicated by the "_1", "_2" suffix, but most of subjects have 
+        just one ID, ending in "_1". Thus, there are 2 ways to specify the IDs: <br/>
+        1. individually and specifying the exact ID, so including "_1" or "_2". Multiple IDs can be mentioned 
+        by using a semicolon symbol to delimitate them: 0001_1;0017_1;0017_2. <br/>
+        2. individually, and specifying just the prefix for a subject. Multiple IDs can be mentioned by using a 
+        semicolon symbol to delimitate them: 0001;0017 will be converted to 4 IDs: 0001_1, 0001_2, 0017_1, 0017_2.
+        """)
 
     fc = Attr(
         field_type=bool,
         label="Compute Functional Connectivities",
         default=True,
         required=True,
         doc="Set if the functional connectivities for the specified subjects should also be computed"
@@ -124,14 +140,15 @@
 
 class SiibraCreatorForm(ABCAdapterForm):
     def __init__(self):
         super(SiibraCreatorForm, self).__init__()
         self.ebrains_token = UserSessionStrField(SiibraModel.ebrains_token, name="ebrains_token", key=KEY_AUTH_TOKEN)
         self.atlas = SelectField(SiibraModel.atlas, name='atlas')
         self.parcellation = SelectField(SiibraModel.parcellation, name='parcellation')
+        self.cohort = SelectField(SiibraModel.cohort, name='cohort')
         self.subject_ids = StrField(SiibraModel.subject_ids, name='subject_ids')
         self.fc = BoolField(SiibraModel.fc, name='fc')
 
     @staticmethod
     def get_view_model():
         return SiibraModel
 
@@ -160,34 +177,34 @@
     def get_output(self):
         return [ConnectivityIndex, ConnectivityMeasureIndex]
 
     def launch(self, view_model):
         ebrains_token = view_model.ebrains_token
         atlas = view_model.atlas.value
         parcellation = view_model.parcellation.value
+        cohort = view_model.cohort.value
         subject_ids = view_model.subject_ids
         compute_fc = view_model.fc
 
         os.environ[CLB_AUTH_TOKEN_KEY] = ebrains_token
 
         # list of all resulting indices for connectivities and possibly connectivity measures
         results = []
 
         try:
-            conn_dict, conn_measures_dict = siibra_base.get_connectivities_from_kg(atlas, parcellation, subject_ids,
-                                                                                    compute_fc)
+            conn_dict, conn_measures_dict = siibra_base.get_connectivities_from_kg(atlas, parcellation, cohort,
+                                                                                   subject_ids, compute_fc)
         except SiibraHttpRequestError as e:
             if e.response.status_code in [401, 403]:
                 raise ConnectionError('Invalid EBRAINS authentication token. Please provide a new one.')
             else:
                 raise ConnectionError('We could not complete the operation. '
                                       'Please check the logs and contact the development team from TVB, siibra or EBRAINS KG.')
 
-
-        # list of indexes after store_complete() is called on each struct. conn. and conn. measures
+        # list of indexes for stored the Struct. Conn. and Conn. Measures
         conn_indices = []
         conn_measures_indices = []
 
         for subject_id, conn in conn_dict.items():
             generic_attrs = view_model.generic_attributes
             generic_attrs.subject = subject_id
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/creators/stimulus_creator.py` & `tvb-rest-client-2.8.1/tvb/adapters/creators/stimulus_creator.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/annotation.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/annotation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/connectivity.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/fcd.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/fcd.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/graph.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/graph.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/local_connectivity.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/local_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/mapped_value.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mapped_value.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/mode_decompositions.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/mode_decompositions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/patterns.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/patterns.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/projections.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/projections.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/region_mapping.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_connectivity.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_region_mapping.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_sensor.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_sensor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_surface.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_surface.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_timeseries.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_timeseries.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/removers/remover_volume.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/removers/remover_volume.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/sensors.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/sensors.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/simulation_history.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/simulation_history.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/spectral.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/spectral.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/structural.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/structural.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/surface.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/surface.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/temporal_correlations.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/temporal_correlations.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/time_series.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/tracts.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/tracts.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/db/volume.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/db/volume.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/annotation_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/annotation_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/connectivity_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/connectivity_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/fcd_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/fcd_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/graph_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/graph_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/local_connectivity_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/local_connectivity_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/mapped_value_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mapped_value_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/mode_decompositions_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/mode_decompositions_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/patterns_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/patterns_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/projections_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/projections_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/region_mapping_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/region_mapping_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/sensors_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/sensors_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/spectral_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/spectral_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/structural_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/structural_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/surface_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/surface_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/temporal_correlations_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/temporal_correlations_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/time_series_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/time_series_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/tracts_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/tracts_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/datatypes/h5/volumes_h5.py` & `tvb-rest-client-2.8.1/tvb/adapters/datatypes/h5/volumes_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/exporters/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/exporters/abcexporter.py` & `tvb-rest-client-2.8.1/tvb/adapters/exporters/abcexporter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/exporters/exceptions.py` & `tvb-rest-client-2.8.1/tvb/adapters/exporters/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/exporters/export_manager.py` & `tvb-rest-client-2.8.1/tvb/adapters/exporters/export_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/exporters/tvb_export.py` & `tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_export.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/exporters/tvb_linked_export.py` & `tvb-rest-client-2.8.1/tvb/adapters/exporters/tvb_linked_export.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/coupling_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/coupling_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/equation_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/equation_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/equation_plot_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/equation_plot_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/form_with_ranges.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/form_with_ranges.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/integrator_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/integrator_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/model_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/model_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,32 +496,37 @@
         self.E_e = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.E_e)
         self.E_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.E_i)
         self.Q_e = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.Q_e)
         self.Q_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.Q_i)
         self.tau_e = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.tau_e)
         self.tau_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.tau_i)
         self.N_tot = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.N_tot)
-        self.p_connect = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.p_connect)
+        self.p_connect_e = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.p_connect_e)
+        self.p_connect_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.p_connect_i)
         self.g = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.g)
         self.K_ext_e = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.K_ext_e)
         self.K_ext_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.K_ext_i)
         self.T = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.T)
         self.P_e = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.P_e)
         self.P_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.P_i)
         self.external_input_ex_ex = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.external_input_ex_ex)
         self.external_input_ex_in = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.external_input_ex_in)
         self.external_input_in_ex = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.external_input_in_ex)
         self.external_input_in_in = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.external_input_in_in)
+        self.tau_OU = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.tau_OU)
+        self.weight_noise = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.weight_noise)
+        self.S_i = ArrayField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.S_i)
         self.variables_of_interest = MultiSelectField(ModelsEnum.ZERLAUT_FIRST_ORDER.value.variables_of_interest)
 
     def get_params_configurable_in_phase_plane(self):
         return [self.g_L, self.E_L_e, self.E_L_i, self.C_m, self.b_e, self.b_i, self.a_e, self.a_i, self.tau_w_e,
                 self.tau_w_i, self.E_e, self.E_i, self.Q_e, self.Q_i, self.tau_e, self.tau_i, self.N_tot,
-                self.p_connect, self.g, self.K_ext_e, self.K_ext_i, self.T, self.external_input_ex_ex,
-                self.external_input_ex_in, self.external_input_in_ex, self.external_input_in_in]
+                self.p_connect_e, self.p_connect_i, self.g, self.K_ext_e, self.K_ext_i, self.T,
+                self.external_input_ex_ex, self.external_input_ex_in, self.external_input_in_ex,
+                self.external_input_in_in, self.tau_OU, self.weight_noise, self.S_i]
 
 
 class ZerlautAdaptationSecondOrderModelForm(ZerlautAdaptationFirstOrderModelForm):
 
     def __init__(self, are_voi_disabled=False):
         super(ZerlautAdaptationSecondOrderModelForm, self).__init__(are_voi_disabled)
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/monitor_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/monitor_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/noise_forms.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/noise_forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/simulator_fragments.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/simulator_fragments.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/surface_model_parameters_form.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/surface_model_parameters_form.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/forms/transfer_vector_form.py` & `tvb-rest-client-2.8.1/tvb/adapters/forms/transfer_vector_form.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/simulator/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/simulator/hpc_simulator_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/simulator/hpc_simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/simulator/range_parameters.py` & `tvb-rest-client-2.8.1/tvb/adapters/simulator/range_parameters.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/simulator/simulator_adapter.py` & `tvb-rest-client-2.8.1/tvb/adapters/simulator/simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/bids_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/bids_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                     centres_path = json_dict[self.COORDS_ROWS_KEY][1]
 
                     dir_path = os.path.dirname(net_file_path)
                     labels_path = os.path.join(dir_path, labels_path).replace(self.JSON_EXTENSION, self.TSV_EXTENSION)
                     centres_path = os.path.join(dir_path, centres_path).replace(self.JSON_EXTENSION, self.TSV_EXTENSION)
 
                     centres = self.read_list_data(centres_path)
-                    labels_vector = self.read_list_data(labels_path, dtype=numpy.str, usecols=[0])
+                    labels_vector = self.read_list_data(labels_path, dtype=numpy.str_, usecols=[0])
 
         connectivity = Connectivity()
 
         expected_number_of_nodes = len(centres)
         connectivity.set_centres(centres, expected_number_of_nodes)
         connectivity.set_region_labels(labels_vector)
         connectivity.set_weights(weights_matrix, expected_number_of_nodes)
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/brco/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/brco_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/brco_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/connectivity_measure_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/connectivity_measure_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/csv_connectivity_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/csv_connectivity_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     def __init__(self, operation_id):
         self.logger = get_logger(__name__)
         self.operation_id = operation_id
 
     @staticmethod
     def _get_meta_dict(data_array):
         data_array_meta = data_array.meta
-        if data_array_meta is None or data_array_meta.data is None:
+        if data_array_meta is None:
             return {}
-        return dict((meta_pair.name, meta_pair.value) for meta_pair in data_array_meta.data)
+        return data_array_meta
 
     @staticmethod
     def _is_surface_gifti(data_arrays):
         return (len(data_arrays) == 2
                 and intent_codes.code["NIFTI_INTENT_POINTSET"] == data_arrays[0].intent
                 and data_type_codes.code["NIFTI_TYPE_FLOAT32"] == data_arrays[0].datatype
                 and intent_codes.code["NIFTI_INTENT_TRIANGLE"] == data_arrays[1].intent
@@ -119,15 +119,15 @@
 
         if should_center:
             vertices = center_vertices(vertices)
 
         # set hemisphere mask if cortex
         if isinstance(surface, CorticalSurface):
             # if there was a 2nd file then len(vertices) != vertices_in_lh
-            surface.hemisphere_mask = numpy.zeros(len(vertices), dtype=numpy.bool)
+            surface.hemisphere_mask = numpy.zeros(len(vertices), dtype=numpy.bool_)
             surface.hemisphere_mask[vertices_in_lh:] = 1
 
         surface.vertices = vertices
         surface.number_of_vertices = surface.vertices.shape[0]
         surface.triangles = triangles
         surface.number_of_triangles = surface.triangles.shape[0]
         return surface
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti_surface_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_surface_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/gifti_timeseries_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/gifti_timeseries_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_eeg_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/mat_timeseries_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/mat_timeseries_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/networkx_connectivity/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_connectivity/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/networkx_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/networkx_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/nifti/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,9 +77,9 @@
         Parse NIFTI file and write in result_dt a 4D or 3D array [time*, x, y, z].
         """
 
         # Copy data from NIFTI file to our TVB storage
         # In NIFTI format time is the 4th dimension, while our TimeSeries has
         # it as first dimension, so we have to adapt imported data
 
-        nifti_data = self.nifti_image.get_data()
+        nifti_data = self.nifti_image.dataobj
         return numpy.array(nifti_data, dtype=numpy.int32)
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/nifti_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/nifti_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     def _apply_corrections_and_mapping(self, data, conn_nr_regions, view_model):
 
         self.log.info("Writing RegionVolumeMapping with min=%d, mix=%d" % (data.min(), data.max()))
 
         if view_model.mappings_file:
             try:
-                mapping_data = numpy.loadtxt(view_model.mappings_file, dtype=numpy.str, usecols=(0, 2))
+                mapping_data = numpy.loadtxt(view_model.mappings_file, dtype=numpy.str_, usecols=(0, 2))
                 mapping_data = {int(row[0]): int(row[1]) for row in mapping_data}
             except Exception:
                 raise ValidationException("Invalid Mapping File. Expected 3 columns (int, string, int)")
 
             if len(data.shape) != 3:
                 raise ValidationException('Invalid RVM data. Expected 3D.')
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/parser.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj/surface.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj/surface.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/obj_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/obj_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/projection_matrix_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/projection_matrix_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/region_mapping_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/region_mapping_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/sensors_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/sensors_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/tract_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/tract_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/tumor_dataset_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/tumor_dataset_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/tvb_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/tvb_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_connectivity_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_connectivity_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,25 +122,25 @@
 
         for file_name in files:
             file_name_low = file_name.lower()
             if self.WEIGHT_TOKEN in file_name_low:
                 weights_matrix = self.read_list_data(file_name)
             elif self.CENTRES_TOKEN in file_name_low or self.CENTRES_TOKEN2 in file_name_low:
                 centres = self.read_list_data(file_name, usecols=[1, 2, 3])
-                labels_vector = self.read_list_data(file_name, dtype=numpy.str, usecols=[0])
+                labels_vector = self.read_list_data(file_name, dtype=numpy.str_, usecols=[0])
             elif self.TRACT_TOKEN in file_name_low:
                 tract_matrix = self.read_list_data(file_name)
             elif self.ORIENTATION_TOKEN in file_name_low:
                 orientation = self.read_list_data(file_name)
             elif self.AREA_TOKEN in file_name_low:
                 areas = self.read_list_data(file_name)
             elif self.CORTICAL_INFO in file_name_low:
-                cortical_vector = self.read_list_data(file_name, dtype=numpy.bool)
+                cortical_vector = self.read_list_data(file_name, dtype=numpy.bool_)
             elif self.HEMISPHERE_INFO in file_name_low:
-                hemisphere_vector = self.read_list_data(file_name, dtype=numpy.bool)
+                hemisphere_vector = self.read_list_data(file_name, dtype=numpy.bool_)
 
         # Clean remaining text-files.
         self.storage_interface.remove_files(files, True)
 
         result = Connectivity()
 
         # Set attributes
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_surface/parser.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,20 @@
 
         if self.bi_hemispheric:
             self._read_files(vertices_lh, normals_lh, triangles_lh, path)
             vertices_in_lh = self._read_vertices
             self._read_files(vertices_rh, normals_rh, triangles_rh, path)
             self._stack_arrays()
 
-            self.hemisphere_mask = numpy.ones(len(self.vertices), dtype=numpy.bool)
+            self.hemisphere_mask = numpy.ones(len(self.vertices), dtype=numpy.bool_)
             self.hemisphere_mask[0:vertices_in_lh] = 0
         else:
             self._read_files(vertices, normals, triangles, path)
             self._stack_arrays()
-            self.hemisphere_mask = numpy.zeros(len(self.vertices), dtype=numpy.bool)
+            self.hemisphere_mask = numpy.zeros(len(self.vertices), dtype=numpy.bool_)
 
     def _stack_arrays(self):
         self.vertices = numpy.vstack(self.vertices)
         self.triangles = numpy.vstack(self.triangles)
         if self.normals:
             self.normals = numpy.vstack(self.normals)
```

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/uploaders/zip_surface_importer.py` & `tvb-rest-client-2.8.1/tvb/adapters/uploaders/zip_surface_importer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/__init__.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/annotations_viewer.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/annotations_viewer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/brain.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/brain.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/complex_imaginary_coherence.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/complex_imaginary_coherence.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/connectivity.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/connectivity_edge_bundle.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/connectivity_edge_bundle.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/cross_coherence.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_coherence.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/cross_correlation.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/eeg_monitor.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/eeg_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/fourier_spectrum.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/fourier_spectrum.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/histogram.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/histogram.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/ica.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/ica.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/local_connectivity_view.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/local_connectivity_view.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/matrix_viewer.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/matrix_viewer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/pca.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pca.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/pearson_cross_correlation.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/pearson_edge_bundle.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pearson_edge_bundle.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/phase_plane_interactive.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/phase_plane_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/pse.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/pse_discrete.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_discrete.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/pse_isocline.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/pse_isocline.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/region_volume_mapping.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/region_volume_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/sensors.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/sensors.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/surface_view.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/surface_view.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/time_series.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/time_series_volume.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/time_series_volume.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/topographic.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/topographic.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/tract.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/tract.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/adapters/visualizers/wavelet_spectrogram.py` & `tvb-rest-client-2.8.1/tvb/adapters/visualizers/wavelet_spectrogram.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/__init__.py` & `tvb-rest-client-2.8.1/tvb/config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,26 +29,17 @@
 
 E.g. Scientific libraries modules are plugged, to avoid close dependencies.
 E.g. A list with all the modules where adapters are implemented.
 """
 # There are kept here for being used inside tvb.core
 # We can not move all these in IntrospectovRegistry, due to circular dependencies
 
-from collections import OrderedDict
-# Import metrics here, so that Traits will find them and return them as known subclasses
-from tvb.analyzers.metric_kuramoto_index import compute_kuramoto_index_metric
-from tvb.analyzers.metric_proxy_metastability import compute_proxy_metastability_metric
-from tvb.analyzers.metric_variance_global import compute_variance_global_metric
-from tvb.analyzers.metric_variance_of_node_variance import compute_variance_of_node_variance_metric
-
-ALGORITHMS = {'GlobalVariance': compute_variance_global_metric,
-              'KuramotoIndex': compute_kuramoto_index_metric,
-              'ProxyMetastabilitySynchrony': compute_proxy_metastability_metric,
-              'VarianceNodeVariance': compute_variance_of_node_variance_metric}
+from tvb.analyzers import METRICS
 
+ALGORITHMS = METRICS
 
 SIMULATION_DATATYPE_CLASS = "SimulationState"
 
 TVB_IMPORTER_MODULE = "tvb.adapters.uploaders.tvb_importer"
 TVB_IMPORTER_CLASS = "TVBImporter"
 
 SIMULATOR_MODULE = "tvb.adapters.simulator.simulator_adapter"
```

### Comparing `tvb-rest-client-2.7.2/tvb/config/algorithm_categories.py` & `tvb-rest-client-2.8.1/tvb/config/algorithm_categories.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/alembic/env.py` & `tvb-rest-client-2.8.1/tvb/config/init/alembic/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,33 @@
 from sqlalchemy import pool
 from alembic import context
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
+# Interpret the config file for Python logging.
+# This line sets up loggers basically.
+if config.config_file_name is not None:
+    fileConfig(config.config_file_name)
+
 # add your model's MetaData object here
 # for 'autogenerate' support
 # from myapp import mymodel
 # target_metadata = mymodel.Base.metadata
 from tvb.core.neotraits.db import Base
 target_metadata = Base.metadata
 
 # other values from the config, defined by the needs of env.py,
 # can be acquired:
 # my_important_option = config.get_main_option("my_important_option")
 # ... etc.
 
 
-def run_migrations_offline():
+def run_migrations_offline() -> None:
     """Run migrations in 'offline' mode.
 
     This configures the context with just a URL
     and not an Engine, though an Engine is acceptable
     here as well.  By skipping the Engine creation
     we don't even need a DBAPI to be available.
 
@@ -44,38 +49,30 @@
         dialect_opts={"paramstyle": "named"},
     )
 
     with context.begin_transaction():
         context.run_migrations()
 
 
-def run_migrations_online():
+def run_migrations_online() -> None:
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
-    connectable = config.attributes.get('connection', None)
-
-    if connectable is None:
-        # only create Engine if we don't have a Connection
-        # from the outside
-        connectable = engine_from_config(
-            config.get_section(config.config_ini_section),
-            prefix="sqlalchemy.",
-            poolclass=pool.NullPool,
-        )
-
-        # when connectable is already a Connection object, calling
-        # connect() gives us a *branched connection*.
+    connectable = engine_from_config(
+        config.get_section(config.config_ini_section, {}),
+        prefix="sqlalchemy.",
+        poolclass=pool.NullPool,
+    )
 
     with connectable.connect() as connection:
         context.configure(
-            connection=connection, target_metadata=target_metadata, render_as_batch=True
+            connection=connection, target_metadata=target_metadata
         )
 
         with context.begin_transaction():
             context.run_migrations()
 
 
 if context.is_offline_mode():
```

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py` & `tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py` & `tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py` & `tvb-rest-client-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/datatypes_registry.py` & `tvb-rest-client-2.8.1/tvb/config/init/datatypes_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/initializer.py` & `tvb-rest-client-2.8.1/tvb/config/init/initializer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/introspector_registry.py` & `tvb-rest-client-2.8.1/tvb/config/init/introspector_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/init/model_manager.py` & `tvb-rest-client-2.8.1/tvb/config/init/model_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/logger/cluster_handler.py` & `tvb-rest-client-2.8.1/tvb/config/logger/cluster_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/config/logger/dev_logger_config.conf` & `tvb-rest-client-2.8.1/tvb/config/logger/dev_logger_config.conf`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ############################################
 ## TVB - logging configuration. ##
 ############################################
 [loggers]
-keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, cherrypy, sqlalchemy, sqlalchemyEcho, rst2pdf, numba, matplotlib
+keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, cherrypy, sqlalchemy, sqlalchemyEcho, rst2pdf, numba, matplotlib, elastic_transport
 
 [handlers]
-keys=consoleHandler,fileHandler,cherrypyFileHandler,sqlalchemyFileHandler, traceUserFileHandler
+keys=consoleHandler,fileHandler,cherrypyFileHandler,sqlalchemyFileHandler, traceUserFileHandler, elasticSearchHandler
 
 [formatters]
 keys=simpleFormatter
 
 [logger_root]
 level=DEBUG
 handlers=consoleHandler, fileHandler
@@ -22,15 +22,15 @@
 level=DEBUG
 handlers=consoleHandler, fileHandler
 qualname=tvb
 propagate=0
 
 [logger_tvb_trace_user]
 level=NOTSET
-handlers=traceUserFileHandler
+handlers=traceUserFileHandler, elasticSearchHandler
 qualname=tvb_user_actions
 propagate=0
 
 [logger_tvb_core_entities_file]
 level=INFO
 handlers=consoleHandler, fileHandler
 qualname=tvb.core.entities.file
@@ -78,14 +78,20 @@
 
 [logger_matplotlib]
 level=ERROR
 handlers=consoleHandler, fileHandler
 qualname=matplotlib
 propagate=0
 
+[logger_elastic_transport]
+level=ERROR
+handlers=consoleHandler, fileHandler
+qualname=elastic_transport
+propagate=0
+
 ############################################
 ## Handlers                               ##
 ############################################
 
 [handler_consoleHandler]
 class=StreamHandler
 level=INFO
@@ -115,14 +121,20 @@
 [handler_sqlalchemyFileHandler]
 class=tvb.basic.logger.simple_handler.SimpleTimedRotatingFileHandler
 level=INFO
 formatter=simpleFormatter
 # Generate a new file every midnight and keep logs for 1 day
 args=('sqlalchemy.log', 'midnight', 1, 1)
 
+
+[handler_elasticSearchHandler]
+class=tvb.config.logger.elasticsearch_handler.ElasticQueueHandler
+level=NOTSET
+formatter=simpleFormatter
+
 ############################################
 ## Formatters                             ##
 ############################################
 
 [formatter_simpleFormatter]
 format=%(asctime)s - %(levelname)s - %(name)s - %(message)s
-datefmt=
+datefmt=%Y-%m-%dT%H:%M:%S
```

### Comparing `tvb-rest-client-2.7.2/tvb/config/logger/logger_config.conf` & `tvb-rest-client-2.8.1/tvb/config/logger/logger_config.conf`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ############################################
 ## TVB - logging configuration. ##
 ############################################
 [loggers]
-keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, tvb_traits, cherrypy, sqlalchemy, rst2pdf, numba, matplotlib
+keys=root, tvb, tvb_trace_user, tvb_core_entities_file, tvb_simulator, tvb_traits, cherrypy, sqlalchemy, rst2pdf, numba, matplotlib, elastic_transport
 
 [handlers]
-keys=consoleHandler,fileHandler,cherrypyFileHandler, traceUserFileHandler
+keys=consoleHandler,fileHandler,cherrypyFileHandler, traceUserFileHandler, elasticSearchHandler
 
 [formatters]
 keys=simpleFormatter
 
 [logger_root]
 level=WARNING
 handlers=fileHandler
@@ -22,15 +22,15 @@
 level=INFO
 handlers=fileHandler
 qualname=tvb
 propagate=0
 
 [logger_tvb_trace_user]
 level=NOTSET
-handlers=traceUserFileHandler
+handlers=traceUserFileHandler, elasticSearchHandler
 qualname=tvb_user_actions
 propagate=0
 
 [logger_tvb_core_entities_file]
 level=WARNING
 handlers=fileHandler
 qualname=tvb.core.entities.file
@@ -79,14 +79,20 @@
 
 [logger_matplotlib]
 level=ERROR
 handlers=consoleHandler, fileHandler
 qualname=matplotlib
 propagate=0
 
+[logger_elastic_transport]
+level=ERROR
+handlers=consoleHandler, fileHandler
+qualname=elastic_transport
+propagate=0
+
 ############################################
 ## Handlers                               ##
 ############################################
 
 [handler_consoleHandler]
 class=StreamHandler
 level=ERROR
@@ -108,14 +114,22 @@
 
 [handler_traceUserFileHandler]
 class=tvb.basic.logger.simple_handler.SimpleTimedRotatingFileHandler
 level=NOTSET
 formatter=simpleFormatter
 # Generate a new file every midnight and keep logs for 30 days
 args=('trace_user.log', 'midnight', 1, 30)
+
+
+[handler_elasticSearchHandler]
+class=tvb.config.logger.elasticsearch_handler.ElasticQueueHandler
+level=NOTSET
+formatter=simpleFormatter
+
+
 ############################################
 ## Formatters                             ##
 ############################################
 
 [formatter_simpleFormatter]
 format=%(asctime)s - %(levelname)s - %(name)s - %(message)s
-datefmt=
+datefmt=%Y-%m-%dT%H:%M:%S
```

### Comparing `tvb-rest-client-2.7.2/tvb/config/profile_settings.py` & `tvb-rest-client-2.8.1/tvb/config/profile_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 TVB global configurations are predefined/read from here, for working with Framework.
 
 .. moduleauthor:: Lia Domide <lia.domide@codemart.ro>
 """
 
 import os
 import sys
+import tvb.config.init
 from tvb.basic.config import stored
 from tvb.basic.config.profile_settings import BaseSettingsProfile
 from tvb.basic.config.settings import DBSettings
 from tvb.basic.logger import builder
 from tvb.basic.logger.builder import LoggerBuilder
 from tvb.config.init.datatypes_registry import populate_datatypes_registry
 
@@ -60,15 +61,16 @@
 
     def initialize_for_deployment(self):
         """
         Specific initialization for deployment and framework settings
         """
         super(WebSettingsProfile, self).initialize_for_deployment()
 
-        inside_static_folder = os.path.join(self.EXTERNALS_FOLDER_PARENT, 'tvb')
+        inside_static_folder = os.path.dirname(os.path.dirname(os.path.dirname(
+            os.path.abspath(tvb.config.init.__file__))))
         self.web.CHERRYPY_CONFIGURATION['/statichelp']['tools.staticdir.root'] = inside_static_folder
 
         # We want to disable warnings we get from sqlalchemy for traited attributes when we are in deployment mode.
         import warnings
         from sqlalchemy import exc as sa_exc
 
         warnings.simplefilter("ignore", category=sa_exc.SAWarning)
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/abcadapter.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/abcadapter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/abcdisplayer.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/abcdisplayer.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/abcremover.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/abcremover.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/abcuploader.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/abcuploader.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/arguments_serialisation.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/arguments_serialisation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/constants.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/constants.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/exceptions.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/adapters/inputs_processor.py` & `tvb-rest-client-2.8.1/tvb/core/adapters/inputs_processor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/base_classes.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/base_classes.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_manager.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/4455_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4455_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/4750_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/4750_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/5454_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/5454_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/6093_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6093_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/6600_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6600_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/6728_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/6728_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/7350_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7350_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/7450_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/7450_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/9444_update_code.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/9444_update_code.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/code_versions/code_update_scripts/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/code_versions/code_update_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/decorators.py` & `tvb-rest-client-2.8.1/tvb/core/decorators.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/exportable.py` & `tvb-rest-client-2.8.1/tvb/core/entities/exportable.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/002_update_files.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/002_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/003_update_files.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/003_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/004_update_files.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/004_update_files.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/005_update_files.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/005_update_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,15 +649,15 @@
                                                                                         kwargs['storage_manager'])
     else:
         operation_xml_parameters, additional_params = _migrate_time_series(operation_xml_parameters)
 
     root_metadata['nr_dimensions'] = int(root_metadata['nr_dimensions'])
     root_metadata['sample_rate'] = float(root_metadata['sample_rate'])
     root_metadata['volume'] = _parse_gid(root_metadata['volume'])
-    root_metadata['volume'] = root_metadata['volume']
+    # root_metadata['volume'] = root_metadata['volume']
     root_metadata.pop('nr_dimensions')
     root_metadata.pop('sample_rate')
     return {'operation_xml_parameters': operation_xml_parameters, 'additional_params': additional_params}
 
 
 def _migrate_volume(**kwargs):
     root_metadata = kwargs['root_metadata']
@@ -932,15 +932,15 @@
 
 
 def _migrate_stimuli_surface(**kwargs):
     root_metadata = kwargs['root_metadata']
     root_metadata['surface'] = _parse_gid(root_metadata['surface'])
     operation_xml_parameters = kwargs['operation_xml_parameters']
     operation_xml_parameters['focal_points_triangles'] = numpy.asarray(
-        json.loads(root_metadata['focal_points_triangles']), dtype=numpy.int)
+        json.loads(root_metadata['focal_points_triangles']), dtype=numpy.int_)
     _migrate_stimuli(['focal_points_surface', 'focal_points_triangles'], root_metadata, kwargs['storage_manager'],
                      kwargs['input_file'])
     additional_params = [_migrate_stimuli_equation_params(operation_xml_parameters, 'temporal'),
                          _migrate_stimuli_equation_params(operation_xml_parameters, 'spatial')]
 
     return {'operation_xml_parameters': operation_xml_parameters, 'additional_params': additional_params}
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/file_update_scripts/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/file_update_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/files_update_manager.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/files_update_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/burst_configuration_h5.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/burst_configuration_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/datatype_measure_h5.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/datatype_measure_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/simulation_history_h5.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/simulation_history_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/file/simulator/view_model.py` & `tvb-rest-client-2.8.1/tvb/core/entities/file/simulator/view_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/filters/chain.py` & `tvb-rest-client-2.8.1/tvb/core/entities/filters/chain.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/filters/exceptions.py` & `tvb-rest-client-2.8.1/tvb/core/entities/filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/filters/factory.py` & `tvb-rest-client-2.8.1/tvb/core/entities/filters/factory.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/generic_attributes.py` & `tvb-rest-client-2.8.1/tvb/core/entities/generic_attributes.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/load.py` & `tvb-rest-client-2.8.1/tvb/core/entities/load.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/model/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/entities/model/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/model/model_burst.py` & `tvb-rest-client-2.8.1/tvb/core/entities/model/model_burst.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/model/model_datatype.py` & `tvb-rest-client-2.8.1/tvb/core/entities/model/model_datatype.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/model/model_operation.py` & `tvb-rest-client-2.8.1/tvb/core/entities/model/model_operation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/model/model_project.py` & `tvb-rest-client-2.8.1/tvb/core/entities/model/model_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/burst_dao.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/burst_dao.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # When using The Virtual Brain for scientific publications, please cite it as explained here:
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
 
 from sqlalchemy import desc, func, or_
 from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy.orm import aliased
 from sqlalchemy.orm.exc import NoResultFound
 from tvb.core.entities.model.model_burst import BurstConfiguration
 from tvb.core.entities.model.model_datatype import DataType
 from tvb.core.entities.storage.root_dao import RootDAO, DEFAULT_PAGE_SIZE
 
 
 class BurstDAO(RootDAO):
@@ -96,16 +97,17 @@
         return None
 
     def get_burst_for_operation_id(self, operation_id, is_group=False):
         burst = None
         try:
             burst = self.get_burst_for_direct_operation_id(operation_id, is_group)
             if not burst:
-                burst = self.session.query(BurstConfiguration
-                                           ).join(DataType, DataType.fk_parent_burst == BurstConfiguration.gid
+                burst_alias = aliased(BurstConfiguration, flat=True)
+                burst = self.session.query(burst_alias
+                                           ).join(DataType, DataType.fk_parent_burst == burst_alias.gid
                                                   ).filter(DataType.fk_from_operation == operation_id).first()
         except NoResultFound:
             self.logger.debug("No burst found for operation id = %s" % (operation_id,))
         except SQLAlchemyError as excep:
             self.logger.exception(excep)
         return burst
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/datatype_dao.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/datatype_dao.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def get_datatypegroup_for_project(self, project_id):
         """
         Returns all DataTypeGroup entities from a project.
         """
         query = self.session.query(DataTypeGroup
-                                   ).join((OperationGroup, OperationGroup.id == DataTypeGroup.fk_operation_group)
+                                   ).join(OperationGroup, OperationGroup.id == DataTypeGroup.fk_operation_group
                                           ).filter(OperationGroup.fk_launched_in == project_id).order_by(DataTypeGroup.id)
         return query.all()
 
     def get_datatypegroup_by_op_group_id(self, operation_group_id):
         """
         Returns the DataTypeGroup corresponding to a certain OperationGroup.
         """
@@ -266,70 +266,70 @@
 
 
     def get_datatypes_in_project(self, project_id, only_visible=False):
         """
         Get all the DataTypes for a given project with no other filter apart from the projectId
         """
         query = self.session.query(DataType
-                    ).join((Operation, Operation.id == DataType.fk_from_operation)
+                    ).join(Operation, Operation.id == DataType.fk_from_operation
                     ).filter(Operation.fk_launched_in == project_id).order_by(DataType.id)
 
         if only_visible:
             query = query.filter(DataType.visible == True)
 
         return query.all()
 
 
     def get_data_in_project(self, project_id, visibility_filter=None, filter_value=None):
         """
         Get all the DataTypes for a given project, including Linked Entities and DataType Groups.
 
+        :param project_id: ID for the current project to filter for
         :param visibility_filter: when not None, will filter by DataTye fields
         :param filter_value: when not None, will filter with ilike multiple DataType string attributes
         """
         resulted_data = []
         try:
             # First Query DT, DT_gr, Lk_DT and Lk_DT_gr
-            query = self.session.query(DataType
-                        ).join((Operation, Operation.id == DataType.fk_from_operation)
+            datatype_alias = aliased(DataType, flat=True)
+            query = self.session.query(datatype_alias
+                        ).join(Operation, Operation.id == datatype_alias.fk_from_operation
                         ).join(Algorithm).join(AlgorithmCategory
-                        ).outerjoin((Links, and_(Links.fk_from_datatype == DataType.id,
-                                                       Links.fk_to_project == project_id))
-                        ).outerjoin(BurstConfiguration,
-                                    DataType.fk_parent_burst == BurstConfiguration.gid
-                                    ).filter(DataType.fk_datatype_group == None
+                        ).outerjoin(Links, and_(Links.fk_from_datatype == datatype_alias.id,
+                                                Links.fk_to_project == project_id)
+                        ).outerjoin(BurstConfiguration, datatype_alias.fk_parent_burst == BurstConfiguration.gid
+                                    ).filter(datatype_alias.fk_datatype_group == None
                         ).filter(or_(Operation.fk_launched_in == project_id,
                                      Links.fk_to_project == project_id))
 
             if visibility_filter:
-                filter_str = visibility_filter.get_sql_filter_equivalent()
+                filter_str = visibility_filter.get_sql_filter_equivalent('datatype_alias')
                 if filter_str is not None:
                     query = query.filter(eval(filter_str))
             if filter_value is not None:
                 query = query.filter(self._compose_filter_datatype_ilike(filter_value))
 
             resulted_data = query.all()
 
             # Now query what it was not covered before:
             # Links of DT which are part of a group, but the entire group is not linked
             links = aliased(Links)
-            query2 = self.session.query(DataType
-                        ).join((Operation, Operation.id == DataType.fk_from_operation)
+            query2 = self.session.query(datatype_alias
+                        ).join(Operation, Operation.id == datatype_alias.fk_from_operation
                         ).join(Algorithm).join(AlgorithmCategory
-                        ).join((Links, and_(Links.fk_from_datatype == DataType.id,
-                                                  Links.fk_to_project == project_id))
-                        ).outerjoin(links, and_(links.fk_from_datatype == DataType.fk_datatype_group,
+                        ).join(Links, and_(Links.fk_from_datatype == datatype_alias.id,
+                                           Links.fk_to_project == project_id)
+                        ).outerjoin(links, and_(links.fk_from_datatype == datatype_alias.fk_datatype_group,
                                                 links.fk_to_project == project_id)
-                        ).outerjoin(BurstConfiguration,
-                                    DataType.fk_parent_burst == BurstConfiguration.gid
-                                    ).filter(DataType.fk_datatype_group != None
+                        ).outerjoin(BurstConfiguration, datatype_alias.fk_parent_burst == BurstConfiguration.gid
+                                    ).filter(datatype_alias.fk_datatype_group != None
                         ).filter(links.id == None)
 
             if visibility_filter:
-                filter_str = visibility_filter.get_sql_filter_equivalent()
+                filter_str = visibility_filter.get_sql_filter_equivalent('datatype_alias')
                 if filter_str is not None:
                     query2 = query2.filter(eval(filter_str))
             if filter_value is not None:
                 query2 = query2.filter(self._compose_filter_datatype_ilike(filter_value))
 
             resulted_data.extend(query2.all())
 
@@ -465,25 +465,25 @@
             self.logger.exception(excep)
             return None
 
 
     def count_datatypes(self, project_id, datatype_class):
 
         query = self.session.query(datatype_class
-                    ).join((Operation, datatype_class.fk_from_operation == Operation.id)
+                    ).join(Operation, datatype_class.fk_from_operation == Operation.id
                     ).outerjoin(Links
                     ).filter(or_(Operation.fk_launched_in == project_id,
                                  Links.fk_to_project == project_id))
         return query.count()
 
 
     def try_load_last_entity_of_type(self, project_id, datatype_class):
 
         query = self.session.query(datatype_class
-                    ).join((Operation, datatype_class.fk_from_operation == Operation.id)
+                    ).join(Operation, datatype_class.fk_from_operation == Operation.id
                     ).outerjoin(Links
                     ).filter(or_(Operation.fk_launched_in == project_id,
                                  Links.fk_to_project == project_id))
         query = query.order_by(desc(datatype_class.id)).limit(1)
         result = query.all()
 
         if result is not None and len(result):
@@ -500,39 +500,38 @@
 
         if not issubclass(datatype_class, Base):
             self.logger.warning("Trying to filter not DB class:" + str(datatype_class))
             return result, count
 
         try:
             # Prepare generic query:
-            query = self.session.query(datatype_class.id,
-                                       func.max(datatype_class.type),
-                                       func.max(datatype_class.gid),
-                                       func.max(datatype_class.subject),
+            datatype_alias = aliased(datatype_class, flat=True)
+            query = self.session.query(datatype_alias.id,
+                                       func.max(datatype_alias.type),
+                                       func.max(datatype_alias.gid),
+                                       func.max(datatype_alias.subject),
                                        func.max(Operation.completion_date),
                                        func.max(Operation.user_group),
-                                       func.max(text('"OPERATION_GROUPS_1".name')),
-                                       func.max(DataType.user_tag_1)
-                        ).join((Operation, datatype_class.fk_from_operation == Operation.id)
-                        ).outerjoin((BurstConfiguration, datatype_class.fk_parent_burst ==
-                                     BurstConfiguration.gid)
+                                       func.max(OperationGroup.name),
+                                       func.max(datatype_alias.user_tag_1)
+                        ).join(Operation, datatype_alias.fk_from_operation == Operation.id
+                        ).outerjoin(BurstConfiguration, datatype_alias.fk_parent_burst == BurstConfiguration.gid
                         ).outerjoin(Links
-                        ).outerjoin((OperationGroup, Operation.fk_operation_group ==
-                                     OperationGroup.id), aliased=True
-                        ).filter(DataType.invalid == False
+                        ).outerjoin(OperationGroup, Operation.fk_operation_group == OperationGroup.id
+                        ).filter(datatype_alias.invalid == False
                         ).filter(or_(Operation.fk_launched_in == project_id,
                                      Links.fk_to_project == project_id))
 
             if filters:
-                filter_str = filters.get_sql_filter_equivalent(datatype_to_check='datatype_class')
+                filter_str = filters.get_sql_filter_equivalent(datatype_to_check='datatype_alias')
                 if filter_str is not None:
                     query = query.filter(eval(filter_str))
 
             # Retrieve the results
-            query = query.group_by(datatype_class.id).order_by(desc(datatype_class.id))
+            query = query.group_by(datatype_alias.id).order_by(desc(datatype_alias.id))
 
             result = query.limit(max(page_size, 0)).all()
             count = query.count()
         except Exception as excep:
             self.logger.exception(excep)
 
         return result, count
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/exceptions.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/operation_dao.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/operation_dao.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,50 +246,46 @@
                                                    func.min(Operation.fk_from_algo),
                                                    func.max(Operation.fk_launched_by),
                                                    func.min(Operation.create_date),
                                                    func.min(Operation.start_date),
                                                    func.max(Operation.completion_date),
                                                    func.min(Operation.status),
                                                    func.max(Operation.additional_info),
-                                                   func.min(case_([(Operation.visible, 1)], else_=0)),
+                                                   func.min(case_((Operation.visible, 1), else_=0)),
                                                    func.min(Operation.user_group),
                                                    func.min(Operation.gid))
 
             query = select_clause.join(Algorithm).join(
                 AlgorithmCategory).filter(Operation.fk_launched_in == project_id)
 
             if filter_chain is not None:
                 filter_string = filter_chain.get_sql_filter_equivalent()
                 query = query.filter(eval(filter_string))
-            query = query.group_by(case_([(Operation.fk_operation_group > 0,
-                                           - Operation.fk_operation_group)], else_=Operation.id))
+            query = query.group_by(case_((Operation.fk_operation_group > 0,
+                                           - Operation.fk_operation_group), else_=Operation.id))
 
             if is_count:
                 return query.count()
 
             return query.order_by(desc(func.max(Operation.id))).offset(page_start).limit(page_size).all()
 
         except SQLAlchemyError as excep:
             self.logger.exception(excep)
             return 0 if is_count else None
 
 
-    def get_results_for_operation(self, operation_id, filters=None):
+    def get_results_for_operation(self, operation_id):
         """
         Retrieve DataTypes entities, resulted after executing an operation.
         """
         try:
             query = self.session.query(DataType
                                        ).filter_by(fk_from_operation=operation_id
                                        ).filter(and_(DataType.type != self.EXCEPTION_DATATYPE_GROUP,
                                                      DataType.type != self.EXCEPTION_DATATYPE_SIMULATION))
-            if filters:
-                filter_str = filters.get_sql_filter_equivalent()
-                if filter_str is not None:
-                    query = query.filter(eval(filter_str))
             query = query.order_by(DataType.id)
             result = query.all()
             for dt in result:
                 dt.display_name
 
             return result
         except SQLAlchemyError as excep:
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/project_dao.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/project_dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,18 +246,18 @@
         return result
 
     def get_projects_for_user(self, user_id, page_start=0, page_size=DEFAULT_PAGE_SIZE, is_count=False):
         """
         Return all projects a given user can access (administrator or not).
         """
         # First load projects that current user is administrator for.
-        query = self.session.query(Project).join((User, Project.fk_admin == User.id)
-                                                 ).outerjoin((User_to_Project,
+        query = self.session.query(Project).join(User, Project.fk_admin == User.id
+                                                 ).outerjoin(User_to_Project,
                                                               and_(Project.id == User_to_Project.fk_project,
-                                                                   User_to_Project.fk_user == user_id))
+                                                                   User_to_Project.fk_user == user_id)
                                                              ).filter(
             or_(User.id == user_id, User_to_Project.fk_user == user_id)
         ).order_by(desc(Project.id))
         if is_count:
             result = query.count()
         else:
             result = query.offset(max(page_start, 0)).limit(max(page_size, 0)).all()
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/root_dao.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/root_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/session_maker.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/session_maker.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/storage/workflow_dao.py` & `tvb-rest-client-2.8.1/tvb/core/entities/storage/workflow_dao.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/transient/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/entities/transient/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/transient/context_overlay.py` & `tvb-rest-client-2.8.1/tvb/core/entities/transient/context_overlay.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/transient/range_parameter.py` & `tvb-rest-client-2.8.1/tvb/core/entities/transient/range_parameter.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/entities/transient/structure_entities.py` & `tvb-rest-client-2.8.1/tvb/core/entities/transient/structure_entities.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neocom/_h5loader.py` & `tvb-rest-client-2.8.1/tvb/core/neocom/_h5loader.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neocom/_registry.py` & `tvb-rest-client-2.8.1/tvb/core/neocom/_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neocom/h5.py` & `tvb-rest-client-2.8.1/tvb/core/neocom/h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/_h5accessors.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/_h5accessors.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/_h5core.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/_h5core.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/db.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 #
 
 import uuid
 import numpy
 from datetime import datetime
 from sqlalchemy import Column, Integer, Text, DateTime, String, Boolean
-from sqlalchemy.ext.declarative import declarative_base, declared_attr
+from sqlalchemy.orm import declarative_base, declared_attr
 
 SCALAR_MAPPING = {
     bool: Boolean,
     int: Integer,
     str: String
 }
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/forms.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/forms.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/h5.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/h5.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/spatial_model.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/spatial_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/uploader_view_model.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/uploader_view_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/neotraits/view_model.py` & `tvb-rest-client-2.8.1/tvb/core/neotraits/view_model.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/operation_async_launcher.py` & `tvb-rest-client-2.8.1/tvb/core/operation_async_launcher.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/operation_hpc_launcher.py` & `tvb-rest-client-2.8.1/tvb/core/operation_hpc_launcher.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/project_versions/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/project_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_manager.py` & `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/1_update_project.py` & `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/1_update_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/2_update_project.py` & `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/2_update_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/3_update_project.py` & `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/3_update_project.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/project_versions/project_update_scripts/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/project_versions/project_update_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/removers_factory.py` & `tvb-rest-client-2.8.1/tvb/core/removers_factory.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/__init__.py` & `tvb-rest-client-2.8.1/tvb/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/algorithm_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/algorithm_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/authorization.py` & `tvb-rest-client-2.8.1/tvb/core/services/authorization.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/backend_client_factory.py` & `tvb-rest-client-2.8.1/tvb/core/services/backend_client_factory.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/backend_clients/backend_client.py` & `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/backend_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/backend_clients/cluster_scheduler_client.py` & `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/cluster_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/backend_clients/hpc_scheduler_client.py` & `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/hpc_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/backend_clients/standalone_client.py` & `tvb-rest-client-2.8.1/tvb/core/services/backend_clients/standalone_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/burst_config_serialization.py` & `tvb-rest-client-2.8.1/tvb/core/services/burst_config_serialization.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/burst_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/burst_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/email_sender.py` & `tvb-rest-client-2.8.1/tvb/core/services/email_sender.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/exceptions.py` & `tvb-rest-client-2.8.1/tvb/core/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/figure_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/figure_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/hpc_operation_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/hpc_operation_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/import_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/import_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/operation_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/operation_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/project_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/project_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -906,19 +906,19 @@
             if operation.view_model_gid:
                 changed_parameters = dict(Warning="Algorithm changed dramatically. We can not offer more details")
             else:
                 changed_parameters = dict(Warning="GID parameter is missing. Old implementation of the operation.")
             return [], changed_parameters
 
     @staticmethod
-    def get_results_for_operation(operation_id, selected_filter=None):
+    def get_results_for_operation(operation_id):
         """
         Retrieve the DataTypes entities resulted after the execution of the given operation.
         """
-        return dao.get_results_for_operation(operation_id, selected_filter)
+        return dao.get_results_for_operation(operation_id)
 
     @staticmethod
     def get_datatype_by_id(datatype_id):
         """Retrieve a DataType DB reference by its id."""
         return dao.get_datatype_by_id(datatype_id)
 
     @staticmethod
@@ -928,16 +928,16 @@
 
     @staticmethod
     def get_datatypegroup_by_op_group_id(operation_group_id):
         """ Returns the DataTypeGroup with the specified id. """
         return dao.get_datatypegroup_by_op_group_id(operation_group_id)
 
     @staticmethod
-    def get_datatypes_in_project(project_id, only_visible=False):
-        return dao.get_data_in_project(project_id, only_visible)
+    def get_datatypes_in_project(project_id):
+        return dao.get_data_in_project(project_id)
 
     @staticmethod
     def set_datatype_visibility(datatype_gid, is_visible):
         """
         Sets the dataType visibility. If the given dataType is a dataType group or it is part of a
         dataType group than this method will set the visibility for each dataType from this group.
         """
```

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/resources/branding_bar.png` & `tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.png`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/resources/branding_bar.svg` & `tvb-rest-client-2.8.1/tvb/core/services/resources/branding_bar.svg`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/settings_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/settings_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/simulator_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/simulator_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/texture_to_json.py` & `tvb-rest-client-2.8.1/tvb/core/services/texture_to_json.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/services/user_service.py` & `tvb-rest-client-2.8.1/tvb/core/services/user_service.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/core/utils.py` & `tvb-rest-client-2.8.1/tvb/core/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/__init__.py` & `tvb-rest-client-2.8.1/tvb/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/bids_data_builder.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/client_decorators.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/client_decorators.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/datatype/datatype_api.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/datatype/datatype_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/fire_simulation.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/fire_simulation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/launch_operation.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/launch_operation.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/examples/utils.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/examples/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/main_api.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/main_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/operation/operation_api.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/operation/operation_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/project/project_api.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/project/project_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/simulator/simulation_api.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/simulator/simulation_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/tests/rest_test.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tests/rest_test.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/tvb_client.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/tvb_client.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/client/user/user_api.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/client/user/user_api.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/decoders.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/decoders.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/dtos.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/dtos.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/exceptions.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/files_helper.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/files_helper.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/status_codes.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/status_codes.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb/interfaces/rest/commons/strings.py` & `tvb-rest-client-2.8.1/tvb/interfaces/rest/commons/strings.py`

 * *Files identical despite different names*

### Comparing `tvb-rest-client-2.7.2/tvb_rest_client.egg-info/PKG-INFO` & `tvb-rest-client-2.8.1/tvb_rest_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-rest-client
-Version: 2.7.2
+Version: 2.8.1
 Summary: A helper package for preparing and sending requests towards the TVB REST API
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
```

### Comparing `tvb-rest-client-2.7.2/tvb_rest_client.egg-info/SOURCES.txt` & `tvb-rest-client-2.8.1/tvb_rest_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
 tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
 tvb/config/init/alembic/versions/__init__.py
 tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
 tvb/config/logger/__init__.py
 tvb/config/logger/cluster_handler.py
 tvb/config/logger/dev_logger_config.conf
+tvb/config/logger/elasticsearch_handler.py
 tvb/config/logger/logger_config.conf
 tvb/core/__init__.py
 tvb/core/decorators.py
 tvb/core/operation_async_launcher.py
 tvb/core/operation_hpc_launcher.py
 tvb/core/removers_factory.py
 tvb/core/utils.py
@@ -284,14 +285,15 @@
 tvb/core/services/backend_clients/backend_client.py
 tvb/core/services/backend_clients/cluster_scheduler_client.py
 tvb/core/services/backend_clients/hpc_scheduler_client.py
 tvb/core/services/backend_clients/standalone_client.py
 tvb/core/services/resources/branding_bar.png
 tvb/core/services/resources/branding_bar.svg
 tvb/interfaces/__init__.py
+tvb/interfaces/rest/__init__.py
 tvb/interfaces/rest/bids_monitor/__init__.py
 tvb/interfaces/rest/bids_monitor/bids_data_builder.py
 tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
 tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
 tvb/interfaces/rest/bids_monitor/tests/__init__.py
 tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
 tvb/interfaces/rest/client/__init__.py
```

