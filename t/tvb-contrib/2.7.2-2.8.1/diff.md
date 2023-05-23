# Comparing `tmp/tvb-contrib-2.7.2.tar.gz` & `tmp/tvb-contrib-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-contrib-2.7.2.tar", last modified: Wed Jan  4 06:21:43 2023, max compression
+gzip compressed data, was "tvb-contrib-2.8.1.tar", last modified: Tue May 23 12:09:29 2023, max compression
```

## Comparing `tvb-contrib-2.7.2.tar` & `tvb-contrib-2.8.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.320489 tvb-contrib-2.7.2/
--rw-r--r--   0 root         (0) root         (0)    36777 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1741 2023-01-04 06:21:43.319489 tvb-contrib-2.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1256 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-04 06:21:43.320489 tvb-contrib-2.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2155 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.270487 tvb-contrib-2.7.2/tvb/
--rw-r--r--   0 root         (0) root         (0)     1363 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.270487 tvb-contrib-2.7.2/tvb/contrib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.271487 tvb-contrib-2.7.2/tvb/contrib/cosimulation/
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/cosimulation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3928 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/cosimulation/cosim_history.py
--rw-r--r--   0 root         (0) root         (0)    10292 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/cosimulation/cosim_monitors.py
--rw-r--r--   0 root         (0) root         (0)    17020 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/cosimulation/cosimulator.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/cosimulation/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.278487 tvb-contrib-2.7.2/tvb/contrib/from_articles/
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py
--rw-r--r--   0 root         (0) root         (0)     6259 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py
--rw-r--r--   0 root         (0) root         (0)     6068 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py
--rw-r--r--   0 root         (0) root         (0)     7195 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py
--rw-r--r--   0 root         (0) root         (0)     7440 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py
--rw-r--r--   0 root         (0) root         (0)     6542 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.279487 tvb-contrib-2.7.2/tvb/contrib/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.286487 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3489 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/base.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/connectivity.py
--rw-r--r--   0 root         (0) root         (0)    16694 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/head.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/local_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/projections.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/region_mapping.py
--rw-r--r--   0 root         (0) root         (0)     7046 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/sensors.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/structural.py
--rw-r--r--   0 root         (0) root         (0)     5774 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/surface.py
--rw-r--r--   0 root         (0) root         (0)    26326 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/time_series.py
--rw-r--r--   0 root         (0) root         (0)    57272 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/time_series_xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.289488 tvb-contrib-2.7.2/tvb/contrib/scripts/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7178 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/linear_with_stimulus.py
--rw-r--r--   0 root         (0) root         (0)    13150 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py
--rw-r--r--   0 root         (0) root         (0)    13470 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py
--rw-r--r--   0 root         (0) root         (0)    34444 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py
--rw-r--r--   0 root         (0) root         (0)     9841 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/models/wilson_cowan_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.291488 tvb-contrib-2.7.2/tvb/contrib/scripts/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/plot/plotter.py
--rw-r--r--   0 root         (0) root         (0)    19366 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/plot/time_series_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.292488 tvb-contrib-2.7.2/tvb/contrib/scripts/service/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3589 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/service/head_service.py
--rw-r--r--   0 root         (0) root         (0)    16448 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/service/time_series_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.295488 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/command_line_utils.py
--rw-r--r--   0 root         (0) root         (0)     8983 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/computations_utils.py
--rw-r--r--   0 root         (0) root         (0)    31003 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/data_structures_utils.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/log_error_utils.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/parcellation_utils.py
--rw-r--r--   0 root         (0) root         (0)    10411 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/scripts/utils/time_series_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.296488 tvb-contrib-2.7.2/tvb/contrib/simulator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.296488 tvb-contrib-2.7.2/tvb/contrib/simulator/demos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.298488 tvb-contrib-2.7.2/tvb/contrib/simulator/files/
--rw-r--r--   0 root         (0) root         (0)   240542 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/files/nerf_int.npz
--rw-r--r--   0 root         (0) root         (0)   240542 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/files/psi.npz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.303488 tvb-contrib-2.7.2/tvb/contrib/simulator/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19274 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/brunel_wang.py
--rw-r--r--   0 root         (0) root         (0)     8671 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/epileptor.py
--rw-r--r--   0 root         (0) root         (0)     7010 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/generic_2d_oscillator.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/hindmarsh_rose.py
--rw-r--r--   0 root         (0) root         (0)     7687 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/jansen_rit_david.py
--rw-r--r--   0 root         (0) root         (0)     9840 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/larter.py
--rw-r--r--   0 root         (0) root         (0)    15305 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/larter_breakspear.py
--rw-r--r--   0 root         (0) root         (0)    12813 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/liley_steynross.py
--rw-r--r--   0 root         (0) root         (0)     7883 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/morris_lecar.py
--rw-r--r--   0 root         (0) root         (0)     8444 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/simulator/models/wong_wang.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.303488 tvb-contrib-2.7.2/tvb/contrib/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.304488 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.310489 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/
--rw-r--r--   0 root         (0) root         (0)     3454 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py
--rw-r--r--   0 root         (0) root         (0)     4133 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py
--rw-r--r--   0 root         (0) root         (0)     8840 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/function_tvb.py
--rw-r--r--   0 root         (0) root         (0)     6345 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py
--rw-r--r--   0 root         (0) root         (0)     7009 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/monitors_test.py
--rw-r--r--   0 root         (0) root         (0)     5104 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py
--rw-r--r--   0 root         (0) root         (0)     3220 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py
--rw-r--r--   0 root         (0) root         (0)     3277 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py
--rw-r--r--   0 root         (0) root         (0)     3271 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/update_function_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.315489 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5485 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py
--rw-r--r--   0 root         (0) root         (0)     5356 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py
--rw-r--r--   0 root         (0) root         (0)    16622 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py
--rw-r--r--   0 root         (0) root         (0)    14850 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py
--rw-r--r--   0 root         (0) root         (0)     3570 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py
--rw-r--r--   0 root         (0) root         (0)     2550 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/update_function_test.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/synchronization_time_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.315489 tvb-contrib-2.7.2/tvb/contrib/tests/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4392 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/model/model_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.316489 tvb-contrib-2.7.2/tvb/contrib/tests/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14798 2023-01-04 05:55:05.000000 tvb-contrib-2.7.2/tvb/contrib/tests/scripts/time_series_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 06:21:43.318489 tvb-contrib-2.7.2/tvb_contrib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1741 2023-01-04 06:21:43.000000 tvb-contrib-2.7.2/tvb_contrib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5425 2023-01-04 06:21:43.000000 tvb-contrib-2.7.2/tvb_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 06:21:43.000000 tvb-contrib-2.7.2/tvb_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-01-04 06:21:43.000000 tvb-contrib-2.7.2/tvb_contrib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-04 06:21:43.000000 tvb-contrib-2.7.2/tvb_contrib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.796074 tvb-contrib-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-23 12:09:29.795073 tvb-contrib-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:29.796074 tvb-contrib-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.762072 tvb-contrib-2.8.1/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.762072 tvb-contrib-2.8.1/tvb/contrib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.763072 tvb-contrib-2.8.1/tvb/contrib/cosimulation/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/cosimulation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/cosimulation/cosim_history.py
+-rw-r--r--   0 root         (0) root         (0)    10292 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/cosimulation/cosim_monitors.py
+-rw-r--r--   0 root         (0) root         (0)    17024 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/cosimulation/cosimulator.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/cosimulation/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.768072 tvb-contrib-2.8.1/tvb/contrib/from_articles/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py
+-rw-r--r--   0 root         (0) root         (0)     7195 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py
+-rw-r--r--   0 root         (0) root         (0)     7440 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py
+-rw-r--r--   0 root         (0) root         (0)     6542 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.768072 tvb-contrib-2.8.1/tvb/contrib/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.771072 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/base.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)    16694 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/head.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/local_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/projections.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/region_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     7049 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/sensors.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/structural.py
+-rw-r--r--   0 root         (0) root         (0)     5775 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/surface.py
+-rw-r--r--   0 root         (0) root         (0)    26326 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/time_series.py
+-rw-r--r--   0 root         (0) root         (0)    57272 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/time_series_xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.772072 tvb-contrib-2.8.1/tvb/contrib/scripts/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7178 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/linear_with_stimulus.py
+-rw-r--r--   0 root         (0) root         (0)    13150 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py
+-rw-r--r--   0 root         (0) root         (0)    13470 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py
+-rw-r--r--   0 root         (0) root         (0)    34444 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/models/wilson_cowan_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.773072 tvb-contrib-2.8.1/tvb/contrib/scripts/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/plot/plotter.py
+-rw-r--r--   0 root         (0) root         (0)    19366 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/plot/time_series_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.774073 tvb-contrib-2.8.1/tvb/contrib/scripts/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/service/head_service.py
+-rw-r--r--   0 root         (0) root         (0)    16449 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/service/time_series_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.776073 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/command_line_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8983 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/computations_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30981 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/data_structures_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/log_error_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/parcellation_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10411 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/scripts/utils/time_series_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.776073 tvb-contrib-2.8.1/tvb/contrib/simulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.777073 tvb-contrib-2.8.1/tvb/contrib/simulator/demos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.778073 tvb-contrib-2.8.1/tvb/contrib/simulator/files/
+-rw-r--r--   0 root         (0) root         (0)   240542 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/files/nerf_int.npz
+-rw-r--r--   0 root         (0) root         (0)   240542 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/files/psi.npz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.781073 tvb-contrib-2.8.1/tvb/contrib/simulator/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19277 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/brunel_wang.py
+-rw-r--r--   0 root         (0) root         (0)     8671 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/epileptor.py
+-rw-r--r--   0 root         (0) root         (0)     7010 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/generic_2d_oscillator.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/hindmarsh_rose.py
+-rw-r--r--   0 root         (0) root         (0)     7687 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/jansen_rit_david.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/larter.py
+-rw-r--r--   0 root         (0) root         (0)    15305 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/larter_breakspear.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/liley_steynross.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/morris_lecar.py
+-rw-r--r--   0 root         (0) root         (0)     8444 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/simulator/models/wong_wang.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.781073 tvb-contrib-2.8.1/tvb/contrib/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.782073 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.786073 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3983 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py
+-rw-r--r--   0 root         (0) root         (0)     4134 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/function_tvb.py
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/monitors_test.py
+-rw-r--r--   0 root         (0) root         (0)     5105 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/update_function_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.791073 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py
+-rw-r--r--   0 root         (0) root         (0)    16684 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/update_function_test.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/synchronization_time_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.792073 tvb-contrib-2.8.1/tvb/contrib/tests/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4392 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/model/model_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.793073 tvb-contrib-2.8.1/tvb/contrib/tests/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14798 2023-05-23 11:37:02.000000 tvb-contrib-2.8.1/tvb/contrib/tests/scripts/time_series_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:29.795073 tvb-contrib-2.8.1/tvb_contrib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-23 12:09:29.000000 tvb-contrib-2.8.1/tvb_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5425 2023-05-23 12:09:29.000000 tvb-contrib-2.8.1/tvb_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:29.000000 tvb-contrib-2.8.1/tvb_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-23 12:09:29.000000 tvb-contrib-2.8.1/tvb_contrib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:29.000000 tvb-contrib-2.8.1/tvb_contrib.egg-info/top_level.txt
```

### Comparing `tvb-contrib-2.7.2/LICENSE` & `tvb-contrib-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/PKG-INFO` & `tvb-contrib-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-contrib
-Version: 2.7.2
+Version: 2.8.1
 Summary: A package with TVB contributed additions to the simulator, useful for scripting.
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Stuart Knock, Dionysios Perdikis, Paula Sanz Leon, Bogdan Valean, Marmaduke Woodman
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience contrib
```

### Comparing `tvb-contrib-2.7.2/README.rst` & `tvb-contrib-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/setup.py` & `tvb-contrib-2.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 #
 
 import os
 import shutil
 import setuptools
 
-CONTRIB_VERSION = "2.7.2"
+CONTRIB_VERSION = "2.8.1"
 CONTRIB_DEPENDENCIES = ["tvb-library", "xarray", "scikit-learn"]
 TEAM = "Stuart Knock, Dionysios Perdikis, Paula Sanz Leon, Bogdan Valean, Marmaduke Woodman"
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as fd:
     DESCRIPTION = fd.read()
 
 setuptools.setup(name='tvb-contrib',
```

### Comparing `tvb-contrib-2.7.2/tvb/__init__.py` & `tvb-contrib-2.8.1/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/cosimulation/cosim_history.py` & `tvb-contrib-2.8.1/tvb/contrib/cosimulation/cosim_history.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/cosimulation/cosim_monitors.py` & `tvb-contrib-2.8.1/tvb/contrib/cosimulation/cosim_monitors.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/cosimulation/cosimulator.py` & `tvb-contrib-2.8.1/tvb/contrib/cosimulation/cosimulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         doc="1, when the proxy nodes substitute TVB nodes and their mutual connections should be removed.")
 
     voi = NArray(
         dtype=int,
         label="Cosimulation model state variables' indices",
         doc=("Indices of model's variables of interest (VOI) that"
              "should be updated (i.e., overwriten) during cosimulation."),
-        default=numpy.asarray([], dtype=numpy.int),
+        default=numpy.asarray([], dtype=numpy.int_),
         required=True)
 
     proxy_inds = NArray(
-        dtype=numpy.int,
+        dtype=numpy.int_,
         label="Indices of TVB proxy nodes",
-        default=numpy.asarray([], dtype=numpy.int),
+        default=numpy.asarray([], dtype=numpy.int_),
         required=True)
 
     cosim_monitors = List(
                     of=CosimMonitor,
                     label="TVB monitor")
 
     synchronization_time = Float(
@@ -245,15 +245,15 @@
                 raise ValueError("Incorrect cosimulation updates values shape %s, \nexpected %s "
                                  "(i.e., (<=synchronization_n_step, n_voi, n_proxy_nodes, number_of_modes))" %
                                  (str(cosim_updates[1].shape), str(self.good_cosim_update_values_shape)))
             else:
                 n_steps = cosim_updates[0].shape[0]
                 # Now update cosimulation history with the cosimulation inputs:
                 self._update_cosim_history(numpy.array(numpy.around(cosim_updates[0] / self.integrator.dt),
-                                                       dtype=numpy.int),
+                                                       dtype=numpy.int_),
                                            cosim_updates[1])
 
             self.simulation_length = n_steps * self.integrator.dt
         else:
             # Normal TVB simulation - no cosimulation:
             if cosim_updates is not None:
                 raise ValueError("cosim_update is not used in normal simulation")
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/cosimulation/exception.py` & `tvb-contrib-2.8.1/tvb/contrib/cosimulation/exception.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_a.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_b.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_c.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_g2d_d.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_sj2d.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_sj3d_a.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc_a.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc_b.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py` & `tvb-contrib-2.8.1/tvb/contrib/from_articles/region_deterministic_bnm_wc_c.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/base.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/connectivity.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/head.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/head.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/local_connectivity.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/local_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/lookup_tables.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/projections.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/projections.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/region_mapping.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/sensors.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,20 +96,20 @@
     def to_tvb_instance(self, **kwargs):
         return super(SensorsMEG, self).to_tvb_instance(TVBSensorsMEG, **kwargs)
 
 
 class SensorsInternal(Sensors, TVBSensorsInternal):
     logger = get_logger(__name__)
     elec_labels = NArray(
-        dtype=np.str,
+        dtype=np.str_,
         label="Electrodes' labels", default=None, required=False,
         doc="""Labels of electrodes.""")
 
     elec_inds = NArray(
-        dtype=np.int,
+        dtype=np.int64,
         label="Electrodes' indices", default=None, required=False,
         doc="""Indices of electrodes.""")
 
     @property
     def number_of_electrodes(self):
         if self.elec_labels is None:
             return 0
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/structural.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/structural.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/surface.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/surface.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from tvb.datatypes.surfaces import SkullSkin as TVBSkullSkin
 from tvb.datatypes.surfaces import Surface as TVBSurface
 from tvb.datatypes.surfaces import WhiteMatterSurface as TVBWhiteMatterSurface
 
 
 class Surface(TVBSurface, BaseModel):
     vox2ras = NArray(
-        dtype=np.float,
+        dtype=np.float_,
         label="vox2ras", default=np.array([]), required=False,
         doc="""Voxel to RAS coordinates transformation array.""")
 
     def get_vertex_normals(self):
         # If there is at least 3 vertices and 1 triangle...
         if self.number_of_vertices > 2 and self.number_of_triangles > 0:
             if self.vertex_normals.shape[0] != self.number_of_vertices:
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/time_series.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/datatypes/time_series_xarray.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/datatypes/time_series_xarray.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/models/linear_reduced_wong_wang_exc_io.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/models/linear_with_stimulus.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/models/linear_with_stimulus.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/models/reduced_wong_wang_exc_io.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/models/reduced_wong_wang_exc_io_inh_i.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/models/spiking_wong_wang_exc_io_inh_i.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/models/wilson_cowan_constraint.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/models/wilson_cowan_constraint.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/plot/plotter.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/plot/plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/plot/power_spectra_coherence_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/plot/time_series_plotter.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/plot/time_series_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/service/head_service.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/service/head_service.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/service/time_series_service.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/service/time_series_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             decim_data, decim_time, decim_dt, decim_n_times = decimate_signals(time_series.squeezed,
                                                                                time_series.time, decim_ratio)
             return time_series.duplicate(data=decim_data, sample_period=float(decim_dt), **kwargs)
         else:
             return time_series.duplicate(**kwargs)
 
     def convolve(self, time_series, win_len=None, kernel=None, **kwargs):
-        n_kernel_points = np.int(np.round(win_len))
+        n_kernel_points = np.int_(np.round(win_len))
         if kernel is None:
             kernel = np.ones((n_kernel_points, 1, 1, 1)) / n_kernel_points
         else:
             kernel = kernel * np.ones((n_kernel_points, 1, 1, 1))
         return time_series.duplicate(data=convolve(time_series.data, kernel, mode='same'), **kwargs)
 
     def hilbert_envelope(self, time_series, **kwargs):
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/command_line_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/command_line_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/computations_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/computations_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/data_structures_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/data_structures_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,21 @@
 #
 
 """
 .. moduleauthor:: Dionysios Perdikis <Denis@tvb.invalid>
 """
 
 import re
-from collections import OrderedDict
-try:
-    from collections import Hashable
-except ImportError:
-    from collections.abc import Hashable
 import itertools
-from copy import deepcopy
 import numpy as np
-from tvb.contrib.scripts.utils.log_error_utils import warning, raise_value_error, raise_import_error
+from copy import deepcopy
+from collections.abc import Hashable
 from six import string_types
+from collections import OrderedDict
+from tvb.contrib.scripts.utils.log_error_utils import warning, raise_value_error, raise_import_error
 from tvb.basic.logger.builder import get_logger
 
 logger = get_logger(__name__)
 
 
 class CalculusConfig(object):
     # Normalization configuration
@@ -52,26 +49,26 @@
     MIN_SINGLE_VALUE = np.finfo("single").min
     MAX_SINGLE_VALUE = np.finfo("single").max
     MAX_INT_VALUE = np.iinfo(np.int64).max
     MIN_INT_VALUE = np.iinfo(np.int64).max
 
 
 def is_numeric(value):
-    return isinstance(value, (float, np.float, np.float64, np.float32, np.float16, np.float128,
-                              int, np.int, np.int0, np.int8, np.int16, np.int32, np.int64,
+    return isinstance(value, (float, np.float_, np.float64, np.float32, np.float16, np.float128,
+                              int, np.int_, np.int0, np.int8, np.int16, np.int32, np.int64,
                               complex, np.complex, np.complex64, np.complex128, np.complex256,
                               np.long, np.number))
 
 
 def is_integer(value):
-    return isinstance(value, (int, np.int, np.int0, np.int8, np.int16, np.int32, np.int64))
+    return isinstance(value, (int, np.int_, np.intp, np.int8, np.int16, np.int32, np.int64))
 
 
 def is_float(value):
-    return isinstance(value, (float, np.float, np.float64, np.float32, np.float16, np.float128))
+    return isinstance(value, (float, np.float_, np.float64, np.float32, np.float16, np.float128))
 
 
 def vector2scalar(x):
     if not (isinstance(x, np.ndarray)):
         return x
     else:
         y = np.squeeze(x)
@@ -618,15 +615,15 @@
     else:
         return False
 
 
 def shape_to_size(shape):
     shape = np.array(shape)
     shape = shape[shape > 0]
-    return np.int(np.max([shape.prod(), 1]))
+    return np.int_(np.max([shape.prod(), 1]))
 
 
 def shape_to_ndim(shape, squeeze=False):
     if squeeze:
         shape = filter(lambda x: not (np.any(np.in1d(x, [0, 1]))), list(shape))
     return len(shape)
 
@@ -651,18 +648,18 @@
     elif np.all(arr == arr[0]):
         return arr[0]
     else:
         return arr
 
 
 def assert_arrays(params, shape=None, transpose=False):
-    # type: (object, object) -> object
+    # type: (object, object, bool) -> object
     if shape is None or \
             not (isinstance(shape, tuple)
-                 and len(shape) in range(3) and np.all([isinstance(s, (int, np.int)) for s in shape])):
+                 and len(shape) in range(3) and np.all([isinstance(s, (int, np.int_)) for s in shape])):
         shape = None
         shapes = []  # list of all unique shapes
         n_shapes = []  # list of all unique shapes' frequencies
         size = 0  # initial shape
     else:
         size = shape_to_size(shape)
 
@@ -711,16 +708,16 @@
         shapes = np.array(shapes)[ind]
         n_shapes = np.array(n_shapes)[ind]
         # Find the most frequent shape
         ind = np.argmax(n_shapes)
         shape = tuple(shapes[ind])
 
     if transpose and len(shape) > 1:
-        if (transpose is "horizontal" or "row" and shape[0] > shape[1]) or \
-                (transpose is "vertical" or "column" and shape[0] < shape[1]):
+        if (transpose == "horizontal" or transpose == "row" and shape[0] > shape[1]) or \
+                (transpose == "vertical" or transpose == "column" and shape[0] < shape[1]):
             shape = list(shape)
             temp = shape[1]
             shape[1] = shape[0]
             shape[0] = temp
             shape = tuple(shape)
 
     # Now reshape or tile when necessary
@@ -744,39 +741,39 @@
 def make_float(x, precision="64"):
     if isinstance(x, np.ndarray):
         if isequal_string(precision, "64"):
             return x.astype(np.float64)
         elif isequal_string(precision, "32"):
             return x.astype(np.float32)
         else:
-            return x.astype(np.float)
+            return x.astype(np.float_)
     else:
         if isequal_string(precision, "64"):
             return np.float64(x)
         elif isequal_string(precision, "32"):
             np.float32(x)
         else:
-            return np.float(x)
+            return np.float_(x)
 
 
 def make_int(x, precision="64"):
     if isinstance(x, np.ndarray):
         if isequal_string(precision, "64"):
             return x.astype(np.int64)
         elif isequal_string(precision, "32"):
             return x.astype(np.int32)
         else:
-            return x.astype(np.int)
+            return x.astype(np.int_)
     else:
         if isequal_string(precision, "64"):
             return np.int64(x)
         elif isequal_string(precision, "32"):
             np.int32(x)
         else:
-            return np.int(x)
+            return np.int_(x)
 
 
 def copy_object_attributes(obj1, obj2, attr1, attr2=None, deep_copy=False, check_none=False):
     attr1 = ensure_list(attr1)
     if attr2 is None:
         attr2 = attr1
     else:
@@ -823,15 +820,15 @@
         else:
             keys.append(xlbl)
     if len(ys):
         sorted_events = OrderedDict()
         for key, xlbl in zip(keys, xlabels):
             sorted_events[key] = np.sort(ys[np.where((xs == xlbl).all(axis=-1))])
     else:
-        sorted_events = OrderedDict(zip(keys, [np.array([])]*len(keys)))
+        sorted_events = OrderedDict(zip(keys, [np.array([])] * len(keys)))
     return sorted_events
 
 
 def data_xarray_from_continuous_events(events, times, senders, variables=[],
                                        filter_senders=None, exclude_senders=[], name=None,
                                        dims_names=["Time", "Variable", "Neuron"]):
     unique_times = np.unique(times).tolist()
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/file_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/log_error_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/log_error_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/parcellation_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/parcellation_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/scripts/utils/time_series_utils.py` & `tvb-contrib-2.8.1/tvb/contrib/scripts/utils/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/demos/region_deterministic_contributed_model.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/files/nerf_int.npz` & `tvb-contrib-2.8.1/tvb/contrib/simulator/files/nerf_int.npz`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/files/psi.npz` & `tvb-contrib-2.8.1/tvb/contrib/simulator/files/psi.npz`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/brunel_wang.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/brunel_wang.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,22 +235,22 @@
     taurp_i = NArray(
         label=":math:`\\tau_{rp_{i}}`",
         default=numpy.array([1.0, ]),
         domain=Range(lo=0.0, hi=2.0, step=0.5),
         doc="""Inhibitory absolute refractory period (ms)""")
 
     Cext = NArray(
-        dtype=numpy.int,
+        dtype=numpy.int_,
         label=":math:`C_{ext}`",
         default=numpy.array([800, ]),
         domain=Range(lo=500, hi=1200, step=100),
         doc="""Number of external (excitatory) connections""")
 
     C = NArray(
-        dtype=numpy.int,
+        dtype=numpy.int_,
         label=":math:`C`",
         default=numpy.array([200, ]),
         domain=Range(lo=100, hi=500, step=100),
         doc="Number of neurons for each node")
 
     nuext = NArray(
         label=":math:`\\nu_{ext}`",
@@ -267,15 +267,15 @@
     wminus = NArray(
         label=":math:`w_{-}`",
         default=numpy.array([1., ]),
         domain=Range(lo=0.2, hi=2., step=0.05),
         doc="""Synaptic coupling strength [w-] (dimensionless)""")
 
     NMAX = NArray(
-        dtype=numpy.int,
+        dtype=numpy.int_,
         label=":math:`N_{MAX}`",
         default=numpy.array([8, ], dtype=numpy.int32),
         domain=Range(lo=2, hi=8, step=1),
         doc="""This is a magic number as given in the original code.
         It is used to compute the phi and psi -- computationally expensive --
         functions""")
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/epileptor.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/epileptor.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/generic_2d_oscillator.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/generic_2d_oscillator.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/hindmarsh_rose.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/hindmarsh_rose.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/jansen_rit_david.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/jansen_rit_david.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/larter.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/larter.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/larter_breakspear.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/larter_breakspear.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/liley_steynross.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/liley_steynross.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/morris_lecar.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/morris_lecar.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/simulator/models/wong_wang.py` & `tvb-contrib-2.8.1/tvb/contrib/simulator/models/wong_wang.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/ReducedWongWang.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_delay_update_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
 """
 .. moduleauthor:: Lionel Kusch <lkusch@thevirtualbrain.org>
 .. moduleauthor:: Dionysios Perdikis <dionperd@gmail.com>
 """
 
 import numpy as np
-
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.parallel.function_tvb import TvbSim
 
 
 class TestDoubleProxyPrecisionComplexDelayUpdate(BaseTestCase):
     """
     test the transmission of information between two models with proxy in most complex case and different delay
     """
+
     def test_double_precision_complex_delay_update(self):
-        weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]],dtype=np.float)
-        delay = np.array([[7, 8, 5, 1], [9, 3, 7, 9], [4, 3, 2, 8], [9, 10, 11, 5]],dtype=np.float)
-        max = np.int(np.max(delay)*10+1)
+        weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]], dtype=np.float_)
+        delay = np.array([[7, 8, 5, 1], [9, 3, 7, 9], [4, 3, 2, 8], [9, 10, 11, 5]], dtype=np.float_)
+        max = np.int_(np.max(delay) * 10 + 1)
         resolution_simulation = 0.1
         time_synchronize = np.min(delay)
         proxy_id_1 = [1]
         proxy_id_2 = [0, 2]
 
         # simulation with one proxy
         np.random.seed(42)
@@ -77,11 +77,11 @@
             # compare with raw monitor delayed of time_synchronize
             np.testing.assert_array_equal(result_ref, result_1[1])
 
             time_ref, result_ref = sim_ref(time_synchronize)
 
             # COMPARE PROXY 1
             np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_2, :], axis=2)[0],
-                              np.squeeze(result_1[0][:, proxy_id_2, :], axis=2)[0])
+                                          np.squeeze(result_1[0][:, proxy_id_2, :], axis=2)[0])
             # COMPARE PROXY 2
-            np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_1,:], axis=2)[0],
-                              np.squeeze(result_2[0][:, proxy_id_1,:], axis=2)[0])
+            np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_1, :], axis=2)[0],
+                                          np.squeeze(result_2[0][:, proxy_id_1, :], axis=2)[0])
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_complex_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     test the transmission of information between two model with proxy in most complex case
     """
 
     def test_double_precision_complex(self):
         weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]])
         delay = np.array([[7, 8, 5, 1], [10, 3, 7, 9], [4, 3, 2, 8], [9, 10, 11, 5]])
-        max = np.int(np.max(delay)*10+1)
+        max = np.int_(np.max(delay)*10+1)
         init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0], [0.9,0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
         synchronization_time = 0.1 * 10
         proxy_id_1 = [1]
         proxy_id_2 = [0, 2]
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/double_proxy_precision_simple_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     test the transmission of information between two model with proxy in simple case
     """
 
     def test_double_precision_simple(self):
         weight = np.array([[1, 1], [1, 1]])
         delay = np.array([[10.0, 10.0], [10.0, 10.0]])
-        max = np.int(np.max(delay)*10+1)
+        max = np.int_(np.max(delay)*10+1)
         init_value = np.array([[[0.1,0.0], [0.1,0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
         synchronization_time = 0.1 * 4
         proxy_id_1 = [0]
         proxy_id_2 = [1]
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/function_tvb.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/function_tvb.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         )
     else:
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = CoSimulator(
                           voi=np.array([0]),
                           synchronization_time=time_synchronize,
                           cosim_monitors=(RawCosim(),),
-                          proxy_inds=np.asarray(id_proxy, dtype=np.int),
+                          proxy_inds=np.asarray(id_proxy, dtype=np.int_),
                           model=model,
                           connectivity=connectivity,
                           coupling=coupling,
                           integrator=integrator,
                           monitors=monitors,
                           initial_conditions=initial_condition
                           )
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/modify_wongwang_precision_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         model = model_class(tau_s=np.random.rand(76))
         connectivity = lab.connectivity.Connectivity().from_file()
         connectivity.speed = np.array([4.0])
         connectivity = adjust_connectivity_delays(connectivity)
         coupling = lab.coupling.Linear(a=np.array(0.0154))
         integrator = lab.integrators.HeunDeterministic(dt=0.1, bounded_state_variable_indices=np.array([0]),
                                                        state_variable_boundaries=np.array([[0.0, 1.0]]))
-        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int))
+        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int_))
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = simulator(model=model,
                         connectivity=connectivity,
                         coupling=coupling,
                         integrator=integrator,
                         monitors=(monitors,),
                         initial_conditions=init,
@@ -93,15 +93,15 @@
         model_1 = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_1 = CoSimulator(
                             voi=np.array([0]),
                             synchronization_time=synchronization_time,
                             cosim_monitors=(RawCosim(),),
-                            proxy_inds=np.asarray([0], dtype=np.int),
+                            proxy_inds=np.asarray([0], dtype=np.int_),
                             model=model_1,
                             connectivity=connectivity,
                             coupling=coupling,
                             integrator=integrator,
                             monitors=(monitors,),
                             initial_conditions=init,
         )
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/monitors_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/monitors_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         model = lab.models.ReducedWongWang(tau_s=np.random.rand(76))
         connectivity = lab.connectivity.Connectivity().from_file()
         connectivity.speed = np.array([4.0])
         connectivity = adjust_connectivity_delays(connectivity)
         coupling = lab.coupling.Linear(a=np.array(0.0154))
         integrator = lab.integrators.HeunDeterministic(dt=0.1, bounded_state_variable_indices=np.array([0]),
                                                        state_variable_boundaries=np.array([[0.0, 1.0]]))
-        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int))
+        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int_))
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = lab.simulator.Simulator(model=model,
                                       connectivity=connectivity,
                                       coupling=coupling,
                                       integrator=integrator,
                                       monitors=(monitors,),
                                       initial_conditions=init,
@@ -84,15 +84,15 @@
         sim_1 = CoSimulator(
             voi=np.array([0]),
             synchronization_time=synchronization_time,
             cosim_monitors=(RawCosim(), RawVoiCosim(variables_of_interest=np.array([0])),
                             RawDelayed(), RawVoiDelayed(variables_of_interest=np.array([0])),
                             CosimCoupling(coupling=coupling),
                             CosimCoupling(coupling=coupling, variables_of_interest=np.array([0]))),
-            proxy_inds=np.asarray([0], dtype=np.int),
+            proxy_inds=np.asarray([0], dtype=np.int_),
             model=model_1,
             connectivity=connectivity,
             coupling=coupling,
             integrator=integrator,
             monitors=(monitors,),
             initial_conditions=init,
         )
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_bad_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Compare the result between simulation with one proxy and without proxy but whith the wrong value at the beginning
     """
 
     def test_precision_bad(self):
         weight = np.array([[2, 8], [3, 5]])
         delay = 100.0
         delays = np.array([[delay, delay], [delay, delay]])
-        max = np.int(np.max(delay)*10+1)
+        max = np.int_(np.max(delay)*10+1)
         init_value = np.array([[0.9,0.0], [0.9,0.0]]*max)
         resolution_simulation = 0.1
         synchronization_time = 0.1 * 10.0
         nb_init = (int(delay / resolution_simulation)) + 1
         initial_condition = np.array(init_value * nb_init).reshape((nb_init, 2, weight.shape[0], 1))
         proxy_id = [0]
         no_proxy = [1]
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 
 import numpy as np
 
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.parallel.function_tvb import TvbSim
 
 
-class TestPrecisionDelay(BaseTestCase):
+class TestPrecisionDelayUpdate(BaseTestCase):
     """
-    compare the result between simulation with one proxy and without proxy and different delay
+    compare the result between simulation with 1-3 proxy and without proxy and different delay
     """
 
-    def test_precision_delay(self):
+    def test_precision_delay_update(self):
         weight = np.array([[2, 8, 0], [0, 0, 0], [3, 0, 1]])
         delay = np.array([[0.6, 0.5, 1.0], [0.7, 0.8, 3.0], [1.0, 0.5, 0.7]])
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0]]] * max)
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0], [0.2, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
-        synchronization_time = 0.1 * 4
+        synchronization_time = np.min(delay)
         proxy_id = [0]
-        no_proxy = [1,2]
+        no_proxy = [1, 2]
 
         # simulation with one proxy
         np.random.seed(42)
         sim = TvbSim(weight, delay, proxy_id, resolution_simulation, synchronization_time,
                      initial_condition=initial_condition)
         time, result = sim(synchronization_time)
 
@@ -57,18 +57,19 @@
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation, synchronization_time,
                          initial_condition=initial_condition)
         time, result_ref = sim_ref(synchronization_time)
 
         # compare with TVB Raw monitor delayed by synchronization_time
         np.testing.assert_array_equal(np.squeeze(result_ref[:, no_proxy, :], axis=2)[0],
-                        np.squeeze(result[0][:, no_proxy, :], axis=2)[0])
+                                      np.squeeze(result[0][:, no_proxy, :], axis=2)[0])
 
         for i in range(0, 1000):
-            time, result = sim(synchronization_time, [time, result_ref[:, proxy_id][:, :, 0]])
+            delay_input = [time, result_ref[:, proxy_id][:, :, 0]]
+            time, result = sim(synchronization_time, delay_input)
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref, result[1])
 
             time, result_ref = sim_ref(synchronization_time)
 
             # compare with TVB Raw monitor delayed by synchronization_time
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_update_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_delay_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 
 import numpy as np
 
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.parallel.function_tvb import TvbSim
 
 
-class TestPrecisionDelayUpdate(BaseTestCase):
+class TestPrecisionDelay(BaseTestCase):
     """
-    compare the result between simulation with 1-3 proxy and without proxy and different delay
+    compare the result between simulation with one proxy and without proxy and different delay
     """
 
-    def test_precision_delay_update(self):
+    def test_precision_delay(self):
         weight = np.array([[2, 8, 0], [0, 0, 0], [3, 0, 1]])
         delay = np.array([[0.6, 0.5, 1.0], [0.7, 0.8, 3.0], [1.0, 0.5, 0.7]])
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0]]] * max)
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0], [0.2, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
-        synchronization_time = np.min(delay)
+        synchronization_time = 0.1 * 4
         proxy_id = [0]
-        no_proxy = [1,2]
+        no_proxy = [1, 2]
 
         # simulation with one proxy
         np.random.seed(42)
         sim = TvbSim(weight, delay, proxy_id, resolution_simulation, synchronization_time,
                      initial_condition=initial_condition)
         time, result = sim(synchronization_time)
 
@@ -57,19 +57,18 @@
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation, synchronization_time,
                          initial_condition=initial_condition)
         time, result_ref = sim_ref(synchronization_time)
 
         # compare with TVB Raw monitor delayed by synchronization_time
         np.testing.assert_array_equal(np.squeeze(result_ref[:, no_proxy, :], axis=2)[0],
-                        np.squeeze(result[0][:, no_proxy, :], axis=2)[0])
+                                      np.squeeze(result[0][:, no_proxy, :], axis=2)[0])
 
         for i in range(0, 1000):
-            delay_input = [time, result_ref[:, proxy_id][:, :, 0]]
-            time, result = sim(synchronization_time, delay_input)
+            time, result = sim(synchronization_time, [time, result_ref[:, proxy_id][:, :, 0]])
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref, result[1])
 
             time, result_ref = sim_ref(synchronization_time)
 
             # compare with TVB Raw monitor delayed by synchronization_time
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_delay_update_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     """
     Compare the result between simulation with 1-3 proxy and without proxy and different delay
     """
 
     def test_precision_multiple_delay_update(self):
         weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]])
         delay = np.array([[0.1, 0.2, 0.5, 0.8], [0.3, 0.5, 0.5, 0.4], [0.6, 0.7, 0.1, 0.2], [0.3, 0.4, 0.5, 1.2]]) * 10
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0], [0.2,0.0]]] * max)
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0], [0.2, 0.0], [0.2, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
         synchronization_time = 0.1 * 10
         proxy_id = [0, 1, 2]
         no_proxy = [3]
 
         # simulation with one or more proxy
@@ -57,15 +57,15 @@
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation, synchronization_time,
                          initial_condition=initial_condition)
         time, result_ref = sim_ref(synchronization_time)
 
         # compare with the CosimMonitor RawCosim
         np.testing.assert_array_equal(np.squeeze(result_ref[:, no_proxy, :], axis=1)[0],
-                        np.squeeze(result[0][:, no_proxy, :], axis=1)[0])
+                                      np.squeeze(result[0][:, no_proxy, :], axis=1)[0])
 
         for i in range(0, 1000):
             delai_input = [time, result_ref[:, proxy_id][:, :, 0]]
             time, result = sim(synchronization_time, delai_input)
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref, result[1])
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_multiple_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     """
     compare the result between simulation with one proxy and without proxy and different delay
     """
 
     def test_precision_multiple(self):
         weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]])
         delay = np.array([[0.1, 0.1, 0.1, 0.1], [0.1, 0.1, 0.1, 0.1], [0.1, 0.1, 0.1, 0.1], [0.1, 0.1, 0.1, 0.1]]) * 10
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0], [0.2,0.0]]] * max)
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0], [0.2, 0.0], [0.2, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
         synchronization_time = 0.1 * 5
         proxy_id = [0, 1, 2]
         no_proxy = [3]
 
         # simulation with one or more proxy
@@ -57,15 +57,15 @@
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation, synchronization_time,
                          initial_condition=initial_condition)
         time, result_ref = sim_ref(synchronization_time)
 
         # compare with the CosimMonitor RawCosim
         np.testing.assert_array_equal(np.squeeze(result_ref[:, no_proxy, :], axis=1)[0],
-                        np.squeeze(result[0][:, no_proxy, :], axis=1)[0])
+                                      np.squeeze(result[0][:, no_proxy, :], axis=1)[0])
 
         for i in range(0, 1000):
             time, result = sim(synchronization_time, [time, result_ref[:, proxy_id][:, :, 0]])
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref, result[1])
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/proxy_precision_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/parallel/update_function_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/parallel/update_function_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,35 +22,34 @@
 
 """
 .. moduleauthor:: Lionel Kusch <lkusch@thevirtualbrain.org>
 .. moduleauthor:: Dionysios Perdikis <dionperd@gmail.com>
 """
 
 import numpy as np
-import operator
 
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.parallel.function_tvb import TvbSim
 
 
-class TestDoubleProxyPrecisionComplex(BaseTestCase):
+class TestDoubleProxyPrecisionSimple(BaseTestCase):
     """
-    Test the transmission of information between two models with proxy in most complex cases
+    test the transmission of information between two model with proxy in simple case
     """
 
-    def test_double_proxy_precision_complex(self):
-        weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]])
-        delay = np.array([[7, 8, 5, 1], [10, 3, 7, 9], [4, 3, 2, 8], [9, 10, 11, 5]])
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.9,0.0], [0.1,0.0], [0.2,0.0], [0.3,0.0]]] * max)
+    def test_double_proxy_precision_simple(self):
+        weight = np.array([[1, 1], [1, 1]])
+        delay = np.array([[10.0, 10.0], [10.0, 10.0]])
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
-        synchronization_time =np.min(delay)
-        proxy_id_1 = [1]
-        proxy_id_2 = [0, 2]
+        synchronization_time = 0.1 * 4
+        proxy_id_1 = [0]
+        proxy_id_2 = [1]
 
         # simulation_2 with one proxy
         np.random.seed(42)
         sim_2 = TvbSim(weight, delay, proxy_id_2, resolution_simulation,
                        synchronization_time, initial_condition=initial_condition)
         time, s_2, result_2 = sim_2(synchronization_time, rate=True)
 
@@ -63,49 +62,45 @@
         # full simulation
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation,
                          synchronization_time, initial_condition=initial_condition)
         time_ref, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
 
         # COMPARE PROXY 1
-        np.testing.assert_array_equal(np.squeeze(result_ref[:,proxy_id_2,:], axis=2),
-                          np.squeeze(result_1[0][:,proxy_id_2,:], axis=2))
-        np.testing.assert_array_equal(np.squeeze(s_ref[:,proxy_id_2,:], axis=2),
-                            np.squeeze(s_1[0][:,proxy_id_2,:], axis=2))
+        np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_2, :], axis=2),
+                                      np.squeeze(result_1[0][:, proxy_id_2, :], axis=2))
+        np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_2, :], axis=2),
+                                      np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
         # COMPARE PROXY 2
-        np.testing.assert_array_equal(np.squeeze(result_ref[:,proxy_id_1,:], axis=2),
-                          np.squeeze(result_2[0][:,proxy_id_1,:], axis=2))
-        np.testing.assert_array_equal(np.squeeze(s_ref[:,proxy_id_1,:], axis=2),
-                            np.squeeze(s_2[0][:,proxy_id_1,:], axis=2))
+        np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_1, :], axis=2),
+                                      np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
+        np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_1, :], axis=2),
+                                      np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
 
         for i in range(0, 1000):
             time, s_2, result_2 = sim_2(synchronization_time,
                                         rate_data=[time, result_1[0][:, proxy_id_2][:, :, 0]], rate=True)
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref[:, proxy_id_1, :], result_2[1][:, proxy_id_1, :])
-            np.testing.assert_array_equal(result_ref[:, proxy_id_2, :]*np.NAN, result_2[1][:, proxy_id_2, :])
+            np.testing.assert_array_equal(result_ref[:, proxy_id_2, :] * np.NAN, result_2[1][:, proxy_id_2, :])
             np.testing.assert_array_equal(s_ref, s_2[1])
 
             time, s_1, result_1 = sim_1(synchronization_time,
                                         rate_data=[time_ref, result_ref[:, proxy_id_1][:, :, 0]], rate=True)
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref[:, proxy_id_2, :], result_1[1][:, proxy_id_2, :])
-            np.testing.assert_array_equal(result_ref[:, proxy_id_1, :]*np.NAN, result_1[1][:, proxy_id_1, :])
+            np.testing.assert_array_equal(result_ref[:, proxy_id_1, :] * np.NAN, result_1[1][:, proxy_id_1, :])
             np.testing.assert_array_equal(s_ref, s_1[1])
 
             time_ref, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
             # COMPARE PROXY 1
-            np.testing.assert_array_equal(
-                np.squeeze(result_ref[:, proxy_id_2, :], axis=2),
-                np.squeeze(result_1[0][:, proxy_id_2, :],  axis=2))
-            np.testing.assert_array_equal(
-                np.squeeze(s_ref[:, proxy_id_2, :], axis=2),
-                np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
+            np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_2, :], axis=2),
+                                          np.squeeze(result_1[0][:, proxy_id_2, :], axis=2))
+            np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_2, :], axis=2),
+                                          np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
             # COMPARE PROXY 2
-            np.testing.assert_array_equal(
-                np.squeeze(result_ref[:, proxy_id_1, :], axis=2),
-                np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
-            np.testing.assert_array_equal(
-                np.squeeze(s_ref[:, proxy_id_1, :], axis=2),
-                np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
+            np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_1, :], axis=2),
+                                          np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
+            np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_1, :], axis=2),
+                                          np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_simple_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/double_proxy_precision_complex_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,34 +22,35 @@
 
 """
 .. moduleauthor:: Lionel Kusch <lkusch@thevirtualbrain.org>
 .. moduleauthor:: Dionysios Perdikis <dionperd@gmail.com>
 """
 
 import numpy as np
+import operator
 
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.parallel.function_tvb import TvbSim
 
 
-class TestDoubleProxyPrecisionSimple(BaseTestCase):
+class TestDoubleProxyPrecisionComplex(BaseTestCase):
     """
-    test the transmission of information between two model with proxy in simple case
+    Test the transmission of information between two models with proxy in most complex cases
     """
 
-    def test_double_proxy_precision_simple(self):
-        weight = np.array([[1, 1], [1, 1]])
-        delay = np.array([[10.0, 10.0], [10.0, 10.0]])
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0]]] * max)
+    def test_double_proxy_precision_complex(self):
+        weight = np.array([[5, 2, 4, 0], [8, 5, 4, 1], [6, 1, 7, 9], [10, 0, 5, 6]])
+        delay = np.array([[7, 8, 5, 1], [10, 3, 7, 9], [4, 3, 2, 8], [9, 10, 11, 5]])
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.9, 0.0], [0.1, 0.0], [0.2, 0.0], [0.3, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
-        synchronization_time = 0.1 * 4
-        proxy_id_1 = [0]
-        proxy_id_2 = [1]
+        synchronization_time = np.min(delay)
+        proxy_id_1 = [1]
+        proxy_id_2 = [0, 2]
 
         # simulation_2 with one proxy
         np.random.seed(42)
         sim_2 = TvbSim(weight, delay, proxy_id_2, resolution_simulation,
                        synchronization_time, initial_condition=initial_condition)
         time, s_2, result_2 = sim_2(synchronization_time, rate=True)
 
@@ -63,44 +64,48 @@
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation,
                          synchronization_time, initial_condition=initial_condition)
         time_ref, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
 
         # COMPARE PROXY 1
         np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_2, :], axis=2),
-                          np.squeeze(result_1[0][:, proxy_id_2, :], axis=2))
+                                      np.squeeze(result_1[0][:, proxy_id_2, :], axis=2))
         np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_2, :], axis=2),
-                            np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
+                                      np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
         # COMPARE PROXY 2
         np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_1, :], axis=2),
-                          np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
+                                      np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
         np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_1, :], axis=2),
-                            np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
+                                      np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
 
         for i in range(0, 1000):
             time, s_2, result_2 = sim_2(synchronization_time,
                                         rate_data=[time, result_1[0][:, proxy_id_2][:, :, 0]], rate=True)
 
             # compare with Raw monitor delayed by synchronization_time
-            np.testing.assert_array_equal(result_ref[:,proxy_id_1,:], result_2[1][:,proxy_id_1,:])
-            np.testing.assert_array_equal(result_ref[:,proxy_id_2,:]*np.NAN, result_2[1][:,proxy_id_2,:])
+            np.testing.assert_array_equal(result_ref[:, proxy_id_1, :], result_2[1][:, proxy_id_1, :])
+            np.testing.assert_array_equal(result_ref[:, proxy_id_2, :] * np.NAN, result_2[1][:, proxy_id_2, :])
             np.testing.assert_array_equal(s_ref, s_2[1])
 
             time, s_1, result_1 = sim_1(synchronization_time,
                                         rate_data=[time_ref, result_ref[:, proxy_id_1][:, :, 0]], rate=True)
 
             # compare with Raw monitor delayed by synchronization_time
             np.testing.assert_array_equal(result_ref[:, proxy_id_2, :], result_1[1][:, proxy_id_2, :])
-            np.testing.assert_array_equal(result_ref[:, proxy_id_1, :]*np.NAN, result_1[1][:, proxy_id_1, :])
+            np.testing.assert_array_equal(result_ref[:, proxy_id_1, :] * np.NAN, result_1[1][:, proxy_id_1, :])
             np.testing.assert_array_equal(s_ref, s_1[1])
 
             time_ref, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
             # COMPARE PROXY 1
-            np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_2, :], axis=2),
-                              np.squeeze(result_1[0][:, proxy_id_2, :], axis=2))
-            np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_2, :], axis=2),
-                                np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
+            np.testing.assert_array_equal(
+                np.squeeze(result_ref[:, proxy_id_2, :], axis=2),
+                np.squeeze(result_1[0][:, proxy_id_2, :], axis=2))
+            np.testing.assert_array_equal(
+                np.squeeze(s_ref[:, proxy_id_2, :], axis=2),
+                np.squeeze(s_1[0][:, proxy_id_2, :], axis=2))
             # COMPARE PROXY 2
-            np.testing.assert_array_equal(np.squeeze(result_ref[:, proxy_id_1, :], axis=2),
-                              np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
-            np.testing.assert_array_equal(np.squeeze(s_ref[:, proxy_id_1, :], axis=2),
-                                np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
+            np.testing.assert_array_equal(
+                np.squeeze(result_ref[:, proxy_id_1, :], axis=2),
+                np.squeeze(result_2[0][:, proxy_id_1, :], axis=2))
+            np.testing.assert_array_equal(
+                np.squeeze(s_ref[:, proxy_id_1, :], axis=2),
+                np.squeeze(s_2[0][:, proxy_id_1, :], axis=2))
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/modify_wongwang_precision_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,23 +24,21 @@
 .. moduleauthor:: Lionel Kusch <lkusch@thevirtualbrain.org>
 .. moduleauthor:: Dionysios Perdikis <dionperd@gmail.com>
 """
 
 import numpy as np
 import pytest
 import operator
-
 import tvb.simulator.lab as lab
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.synchronization_time_set import SYNCHRONIZATION_TIME, adjust_connectivity_delays
 from tvb.contrib.tests.cosimulation.parallel.ReducedWongWang import ReducedWongWangProxy
 from tvb.contrib.cosimulation.cosim_monitors import RawCosim
 from tvb.contrib.cosimulation.cosimulator import CoSimulator
 
-
 SIMULATION_LENGTH = 3.0
 
 
 class TestModifyWongWang(BaseTestCase):
     """
     Initialisation of the test for the reference simulation
     """
@@ -55,15 +53,15 @@
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         connectivity = lab.connectivity.Connectivity().from_file()
         connectivity.speed = np.array([4.0])
         connectivity = adjust_connectivity_delays(connectivity)
         coupling = lab.coupling.Linear(a=np.array(0.0154))
         integrator = lab.integrators.HeunDeterministic(dt=0.1, bounded_state_variable_indices=np.array([0]),
                                                        state_variable_boundaries=np.array([[0.0, 1.0]]))
-        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int))
+        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int_))
 
         return model, connectivity, coupling, init, integrator, monitors
 
     def _reference_simulation(self, simulator=lab.simulator.Simulator):
         model, connectivity, coupling, init, integrator, monitors = self._prepare_reference_simulation()
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = simulator(model=model,
@@ -79,29 +77,30 @@
         return connectivity, coupling, integrator, monitors, sim, result, result_all
 
 
 class TestModifyWongWangRate(TestModifyWongWang):
     """
     Test to compare the version in TVB and the modified version
     """
+
     def test_with_no_cosimulation(self):
         connectivity, coupling, integrator, monitors, sim, result, result_all = self._reference_simulation()
         result_2 = self._reference_simulation(simulator=CoSimulator)[5]
         diff = result - result_2
         assert np.sum(diff) == 0.0
 
     def test_without_proxy(self):
         model, connectivity, coupling, init, integrator, monitors = self._prepare_reference_simulation()
         np.random.seed(42)
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = CoSimulator(
             voi=np.array([0]),
             synchronization_time=SYNCHRONIZATION_TIME,
             cosim_monitors=(RawCosim(),),
-            proxy_inds=np.array([], dtype=np.int),
+            proxy_inds=np.array([], dtype=np.int_),
             model=model,
             connectivity=connectivity,
             coupling=coupling,
             integrator=integrator,
             monitors=(monitors,),
             initial_conditions=init,
         )
@@ -111,18 +110,18 @@
     def test_without_voi(self):
         model, connectivity, coupling, init, integrator, monitors = self._prepare_reference_simulation()
         np.random.seed(42)
         id_proxy = range(11)
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = CoSimulator(
-            voi=np.array([], dtype=np.int),
+            voi=np.array([], dtype=np.int_),
             synchronization_time=SYNCHRONIZATION_TIME,
             cosim_monitors=(RawCosim(),),
-            proxy_inds=np.asarray(id_proxy, dtype=np.int),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
             model=model,
             connectivity=connectivity,
             coupling=coupling,
             integrator=integrator,
             monitors=(monitors,),
             initial_conditions=init,
         )
@@ -140,15 +139,15 @@
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_3 = CoSimulator(
             voi=np.array([0]),
             synchronization_time=synchronization_time,
             cosim_monitors=(RawCosim(),),
-            proxy_inds=np.asarray(id_proxy, dtype=np.int),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
             model=model,
             connectivity=connectivity,
             coupling=coupling,
             integrator=integrator,
             monitors=(monitors,),
             initial_conditions=init,
         )
@@ -164,41 +163,41 @@
             result_3_all[0] = np.concatenate((result_3_all[0], result_3_all_step[0][0]))
             result_3_all[1] = np.concatenate((result_3_all[1], result_3_all_step[0][1]))
 
         simulation_n_steps = int(SIMULATION_LENGTH / integrator.dt)
         # The beginning is good for rate
         for i in range(np.min(sim_3.connectivity.idelays[np.nonzero(sim_3.connectivity.idelays)]) + 1):
             np.testing.assert_array_equal(result_all[0][1][i][0][len(id_proxy):],
-                                          result_3_all[1][i+sync_steps, 0, len(id_proxy):])
-            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)]*np.NAN,
-                                          result_3_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                          result_3_all[1][i + sync_steps, 0, len(id_proxy):])
+            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)] * np.NAN,
+                                          result_3_all[1][i + sync_steps, 0, :len(id_proxy)])
         # After the delays impact the simulation, there is some difference for rate
         idelays = np.copy(sim_3.connectivity.idelays)
-        idelays = idelays[len(id_proxy):,:len(id_proxy)]
+        idelays = idelays[len(id_proxy):, :len(id_proxy)]
         min_delay = idelays[np.nonzero(idelays)].min()
         for i in range(min_delay + 1, simulation_n_steps):
             diff = result_all[0][1][i][0][len(id_proxy):] - result_3_all[1][i + sync_steps, 0, len(id_proxy):]
             assert np.isnan(diff.sum())
-            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)]*np.NAN,
+            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)] * np.NAN,
                                           result_3_all[1][i + sync_steps, 0, :len(id_proxy)])
 
         # The beginning is good for S
         for i in range(np.min(sim_3.connectivity.idelays[np.nonzero(sim_3.connectivity.idelays)]) + 1):
             np.testing.assert_array_equal(result_all[0][1][i][1][len(id_proxy):],
-                                          result_3_all[1][i+sync_steps, 1, len(id_proxy):])
-            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)]*np.NAN,
-                                          result_3_all[1][i+sync_steps, 1, :len(id_proxy)])
+                                          result_3_all[1][i + sync_steps, 1, len(id_proxy):])
+            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)] * np.NAN,
+                                          result_3_all[1][i + sync_steps, 1, :len(id_proxy)])
         # After the delays impact the simulation, there is some difference for S
         idelays = np.copy(sim_3.connectivity.idelays)
-        idelays = idelays[len(id_proxy):,:len(id_proxy)]
+        idelays = idelays[len(id_proxy):, :len(id_proxy)]
         min_delay = idelays[np.nonzero(idelays)].min()
         for i in range(min_delay + 1, simulation_n_steps):
             diff = result_all[0][1][i][1][len(id_proxy):] - result_3_all[1][i + sync_steps, 1, len(id_proxy):]
             assert np.isnan(diff.sum())
-            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)]*np.NAN,
+            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)] * np.NAN,
                                           result_3_all[1][i + sync_steps, 1, :len(id_proxy)])
 
     def test_with_proxy_bad_input(self):
         connectivity, coupling, integrator, monitors, sim, result, result_all = self._reference_simulation()
         # The modify model without proxy
         np.random.seed(42)
         init = np.concatenate((np.random.random_sample((385, 1, 76, 1)),
@@ -208,15 +207,15 @@
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_4 = CoSimulator(
             voi=np.array([0]),
             synchronization_time=synchronization_time,
             cosim_monitors=(RawCosim(),),
-            proxy_inds=np.asarray(id_proxy, dtype=np.int),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
             model=model,
             connectivity=connectivity,
             coupling=coupling,
             integrator=integrator,
             monitors=(monitors,),
             initial_conditions=init,
         )
@@ -233,44 +232,44 @@
                 cosim_updates=[np.array([result_all[0][0][(sync_steps * j) + i] for i in range(sync_steps)]),
                                np.ones((sync_steps, 1, len(id_proxy), 1)) * 0.7])
             result_4_all[0] = np.concatenate((result_4_all[0], result_4_all_step[0][0]))
             result_4_all[1] = np.concatenate((result_4_all[1], result_4_all_step[0][1]))
 
         simulation_n_steps = int(SIMULATION_LENGTH / integrator.dt)
         # The beginning is good for rate
-        for i in range(np.min(sim_4.connectivity.idelays[np.nonzero(sim_4.connectivity.idelays)])+1):
+        for i in range(np.min(sim_4.connectivity.idelays[np.nonzero(sim_4.connectivity.idelays)]) + 1):
             np.testing.assert_array_equal(result_all[0][1][i][0][len(id_proxy):],
-                                          result_4_all[1][i+sync_steps, 0, len(id_proxy):])
+                                          result_4_all[1][i + sync_steps, 0, len(id_proxy):])
             np.testing.assert_array_compare(operator.__ne__, result_all[0][1][i][0][:len(id_proxy)],
-                                            result_4_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                            result_4_all[1][i + sync_steps, 0, :len(id_proxy)])
         # After the delays impact the simulation, there is some difference for rate
         idelays = np.copy(sim_4.connectivity.idelays)
-        idelays = idelays[len(id_proxy):,:len(id_proxy)]
+        idelays = idelays[len(id_proxy):, :len(id_proxy)]
         min_delay = idelays[np.nonzero(idelays)].min()
         for i in range(min_delay + 1, simulation_n_steps):
-            diff = result_all[0][1][i][0][len(id_proxy):] - result_4_all[1][i+sync_steps, 0, len(id_proxy):]
+            diff = result_all[0][1][i][0][len(id_proxy):] - result_4_all[1][i + sync_steps, 0, len(id_proxy):]
             assert np.sum(diff) != 0.0
             np.testing.assert_array_compare(operator.__ne__, result_all[0][1][i][0][:len(id_proxy)],
-                                            result_4_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                            result_4_all[1][i + sync_steps, 0, :len(id_proxy)])
 
         # The beginning is good for S
-        for i in range(np.min(sim_4.connectivity.idelays[np.nonzero(sim_4.connectivity.idelays)])+1):
+        for i in range(np.min(sim_4.connectivity.idelays[np.nonzero(sim_4.connectivity.idelays)]) + 1):
             np.testing.assert_array_equal(result_all[0][1][i][1][len(id_proxy):],
-                                          result_4_all[1][i+sync_steps, 1, len(id_proxy):])
-            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)]*np.NAN,
-                                          result_4_all[1][i+sync_steps, 1, :len(id_proxy)])
+                                          result_4_all[1][i + sync_steps, 1, len(id_proxy):])
+            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)] * np.NAN,
+                                          result_4_all[1][i + sync_steps, 1, :len(id_proxy)])
         # After the delays impact the simulation, there is some difference for S
         idelays = np.copy(sim_4.connectivity.idelays)
-        idelays = idelays[len(id_proxy):,:len(id_proxy)]
+        idelays = idelays[len(id_proxy):, :len(id_proxy)]
         min_delay = idelays[np.nonzero(idelays)].min()
         for i in range(min_delay + 1, simulation_n_steps):
-            diff = result_all[0][1][i][1][len(id_proxy):] - result_4_all[1][i+sync_steps, 1, len(id_proxy):]
+            diff = result_all[0][1][i][1][len(id_proxy):] - result_4_all[1][i + sync_steps, 1, len(id_proxy):]
             assert np.sum(diff) != 0.0  # TODO: Find out why it fails for the first two iterations!
-            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)]*np.NAN,
-                                          result_4_all[1][i+sync_steps, 1, :len(id_proxy)])
+            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)] * np.NAN,
+                                          result_4_all[1][i + sync_steps, 1, :len(id_proxy)])
 
     def test_with_proxy_right_input(self):
         connectivity, coupling, integrator, monitors, sim, result, result_all = self._reference_simulation()
         # The modify model without proxy
         np.random.seed(42)
         init = np.concatenate((np.random.random_sample((385, 1, 76, 1)),
                                np.random.random_sample((385, 1, 76, 1))), axis=1)
@@ -279,15 +278,15 @@
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_5 = CoSimulator(
             voi=np.array([0]),
             synchronization_time=synchronization_time,
             cosim_monitors=(RawCosim(),),
-            proxy_inds=np.asarray(id_proxy, dtype=np.int),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
             model=model,
             connectivity=connectivity,
             coupling=coupling,
             integrator=integrator,
             monitors=(monitors,),
             initial_conditions=init,
         )
@@ -304,18 +303,18 @@
                 cosim_updates=[np.array([result_all[0][0][(sync_steps * j) + i] for i in range(sync_steps)]),
                                np.array([result_all[0][1][(sync_steps * j) + i][0][id_proxy]
                                          for i in range(sync_steps)]).reshape((sync_steps, 1, len(id_proxy), 1))])
             result_5_all[0] = np.concatenate((result_5_all[0], result_5_all_step[0][0]))
             result_5_all[1] = np.concatenate((result_5_all[1], result_5_all_step[0][1]))
 
         # test for rate and then for S
-        simulation_n_steps = int(SIMULATION_LENGTH/integrator.dt)
+        simulation_n_steps = int(SIMULATION_LENGTH / integrator.dt)
         for i in range(simulation_n_steps):
             np.testing.assert_array_equal(result_all[0][1][i][0][len(id_proxy):],
-                                          result_5_all[1][i+sync_steps, 0, len(id_proxy):])
+                                          result_5_all[1][i + sync_steps, 0, len(id_proxy):])
             np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)],
-                                          result_5_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                          result_5_all[1][i + sync_steps, 0, :len(id_proxy)])
         for i in range(simulation_n_steps):
             np.testing.assert_array_equal(result_all[0][1][i][1][len(id_proxy):],
-                                          result_5_all[1][i+sync_steps, 1, len(id_proxy):])
-            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)]*np.NAN,
-                                          result_5_all[1][i+sync_steps, 1, :len(id_proxy)])
+                                          result_5_all[1][i + sync_steps, 1, len(id_proxy):])
+            np.testing.assert_array_equal(result_all[0][1][i][1][:len(id_proxy)] * np.NAN,
+                                          result_5_all[1][i + sync_steps, 1, :len(id_proxy)])
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/modify_wongwang_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,21 @@
 .. moduleauthor:: Lionel Kusch <lkusch@thevirtualbrain.org>
 .. moduleauthor:: Dionysios Perdikis <dionperd@gmail.com>
 """
 
 import numpy as np
 import pytest
 import operator
-
 import tvb.simulator.lab as lab
 from tvb.tests.library.base_testcase import BaseTestCase
 from tvb.contrib.tests.cosimulation.synchronization_time_set import SYNCHRONIZATION_TIME, adjust_connectivity_delays
 from tvb.contrib.tests.cosimulation.parallel.ReducedWongWang import ReducedWongWangProxy
 from tvb.contrib.cosimulation.cosim_monitors import RawCosim, CosimCoupling
 from tvb.contrib.cosimulation.cosimulator import CoSimulator
 
-
 SIMULATION_LENGTH = 3.0
 
 
 class TestModifyWongWang(BaseTestCase):
     """
     Test to compare the version in tvb and the modified version
     """
@@ -55,15 +53,15 @@
         model = model_class(tau_s=np.random.rand(76))
         connectivity = lab.connectivity.Connectivity().from_file()
         connectivity.speed = np.array([4.0])
         connectivity = adjust_connectivity_delays(connectivity)
         coupling = lab.coupling.Linear(a=np.array(0.0154))
         integrator = lab.integrators.HeunDeterministic(dt=0.1, bounded_state_variable_indices=np.array([0]),
                                                        state_variable_boundaries=np.array([[0.0, 1.0]]))
-        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int))
+        monitors = lab.monitors.Raw(period=0.1, variables_of_interest=np.array(0, dtype=np.int_))
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim = simulator(model=model,
                         connectivity=connectivity,
                         coupling=coupling,
                         integrator=integrator,
                         monitors=(monitors,),
                         initial_conditions=init,
@@ -95,185 +93,186 @@
                                np.random.random_sample((385, 1, 76, 1))), axis=1)
         np.random.seed(42)
         id_proxy = range(11)
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_3 = CoSimulator(
-                            voi=np.array([0]),
-                            synchronization_time=synchronization_time,
-                            cosim_monitors=(RawCosim(),),
-                            proxy_inds=np.asarray(id_proxy, dtype=np.int),
-                            model=model,
-                            connectivity=connectivity,
-                            coupling=coupling,
-                            integrator=integrator,
-                            monitors=(monitors,),
-                            initial_conditions=init,
-                            )
+            voi=np.array([0]),
+            synchronization_time=synchronization_time,
+            cosim_monitors=(RawCosim(),),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
+            model=model,
+            connectivity=connectivity,
+            coupling=coupling,
+            integrator=integrator,
+            monitors=(monitors,),
+            initial_conditions=init,
+        )
         sim_3.configure()
-        sim_3.run() # run the first steps because the history is delayed
+        sim_3.run()  # run the first steps because the history is delayed
 
         sim_to_sync_time = int(SIMULATION_LENGTH / synchronization_time)
         sync_steps = int(synchronization_time / integrator.dt)
 
         result_3_all = [np.empty((0,)), np.empty((sync_steps, 2, 76, 1))]
 
         for j in range(0, sim_to_sync_time):
             result_3_all_step = sim_3.run()
             result_3_all[0] = np.concatenate((result_3_all[0], result_3_all_step[0][0]))
             result_3_all[1] = np.concatenate((result_3_all[1], result_3_all_step[0][1]))
 
         # The beginning is good for rate and S
         for i in range(np.min(sim_3.connectivity.idelays[np.nonzero(sim_3.connectivity.idelays)]) + 1):
             np.testing.assert_array_equal(result_all[0][1][i][0][len(id_proxy):],
-                                          result_3_all[1][i+sync_steps, 0, len(id_proxy):])
-            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)]*np.NAN,
-                                          result_3_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                          result_3_all[1][i + sync_steps, 0, len(id_proxy):])
+            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)] * np.NAN,
+                                          result_3_all[1][i + sync_steps, 0, :len(id_proxy)])
         # After the delays impact the simulation, there is some difference for S
         idelays = np.copy(sim_3.connectivity.idelays)
-        idelays = idelays[len(id_proxy):,:len(id_proxy)]
+        idelays = idelays[len(id_proxy):, :len(id_proxy)]
         min_delay = idelays[np.nonzero(idelays)].min()
-        for i in range(min_delay + 1, int(SIMULATION_LENGTH/integrator.dt)):
+        for i in range(min_delay + 1, int(SIMULATION_LENGTH / integrator.dt)):
             diff = result_all[0][1][i][0][len(id_proxy):] - result_3_all[1][i + sync_steps, 0, len(id_proxy):]
             assert np.isnan(diff.sum())
-            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)]*np.NAN,
+            np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)] * np.NAN,
                                           result_3_all[1][i + sync_steps, 0, :len(id_proxy)])
 
     def test_with_proxy_bad_input(self):
         connectivity, coupling, integrator, monitors, sim, result, result_all = self._reference_simulation()
         # The modify model without proxy
         np.random.seed(42)
         init = np.concatenate((np.random.random_sample((385, 1, 76, 1)),
                                np.random.random_sample((385, 1, 76, 1))), axis=1)
         np.random.seed(42)
         id_proxy = range(11)
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_4 = CoSimulator(
-                            voi=np.array([0]),
-                            synchronization_time=synchronization_time,
-                            cosim_monitors=(RawCosim(),),
-                            proxy_inds=np.asarray(id_proxy, dtype=np.int),
-                            model=model,
-                            connectivity=connectivity,
-                            coupling=coupling,
-                            integrator=integrator,
-                            monitors=(monitors,),
-                            initial_conditions=init,
-                            )
+            voi=np.array([0]),
+            synchronization_time=synchronization_time,
+            cosim_monitors=(RawCosim(),),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
+            model=model,
+            connectivity=connectivity,
+            coupling=coupling,
+            integrator=integrator,
+            monitors=(monitors,),
+            initial_conditions=init,
+        )
         sim_4.configure()
-        sim_4.run() # run the first steps because the history is delayed
+        sim_4.run()  # run the first steps because the history is delayed
 
         sim_to_sync_time = int(SIMULATION_LENGTH / synchronization_time)
         sync_steps = int(synchronization_time / integrator.dt)
 
         result_4_all = [np.empty((0,)), np.empty((sync_steps, 2, 76, 1))]
 
         for j in range(0, sim_to_sync_time):
             result_4_all_step = sim_4.run(
                 cosim_updates=[np.array([result_all[0][0][(sync_steps * j) + i] for i in range(sync_steps)]),
                                np.ones((sync_steps, 1, len(id_proxy), 1)) * 0.7])
             result_4_all[0] = np.concatenate((result_4_all[0], result_4_all_step[0][0]))
             result_4_all[1] = np.concatenate((result_4_all[1], result_4_all_step[0][1]))
 
         # The beginning is good for rate and S
-        for i in range(np.min(sim_4.connectivity.idelays[np.nonzero(sim_4.connectivity.idelays)])+1):
+        for i in range(np.min(sim_4.connectivity.idelays[np.nonzero(sim_4.connectivity.idelays)]) + 1):
             np.testing.assert_array_equal(result_all[0][1][i][0][len(id_proxy):],
-                                          result_4_all[1][i+sync_steps, 0, len(id_proxy):])
+                                          result_4_all[1][i + sync_steps, 0, len(id_proxy):])
             np.testing.assert_array_compare(operator.__ne__,
                                             result_all[0][1][i][0][:len(id_proxy)],
-                                            result_4_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                            result_4_all[1][i + sync_steps, 0, :len(id_proxy)])
         # After the delays impact the simulation, there is some difference for for rate and S
         idelays = np.copy(sim_4.connectivity.idelays)
-        idelays = idelays[len(id_proxy):,:len(id_proxy)]
+        idelays = idelays[len(id_proxy):, :len(id_proxy)]
         min_delay = idelays[np.nonzero(idelays)].min()
-        for i in range(min_delay + 1, int(SIMULATION_LENGTH/integrator.dt)):
-            diff = result_all[0][1][i][0][len(id_proxy):] - result_4_all[1][i+sync_steps, 0, len(id_proxy):]
+        for i in range(min_delay + 1, int(SIMULATION_LENGTH / integrator.dt)):
+            diff = result_all[0][1][i][0][len(id_proxy):] - result_4_all[1][i + sync_steps, 0, len(id_proxy):]
             assert np.sum(diff) != 0.0  # TODO: Find out why it fails for the first two iterations!
             np.testing.assert_array_compare(operator.__ne__,
                                             result_all[0][1][i][0][:len(id_proxy)],
-                                            result_4_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                            result_4_all[1][i + sync_steps, 0, :len(id_proxy)])
 
     def test_with_proxy_right_input(self):
         connectivity, coupling, integrator, monitors, sim, result, result_all = self._reference_simulation()
         # The modify model without proxy
         np.random.seed(42)
         init = np.concatenate((np.random.random_sample((385, 1, 76, 1)),
                                np.random.random_sample((385, 1, 76, 1))), axis=1)
         np.random.seed(42)
         id_proxy = range(11)
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_5 = CoSimulator(
-                            voi=np.array([0]),
-                            synchronization_time=synchronization_time,
-                            cosim_monitors=(RawCosim(),),
-                            proxy_inds=np.asarray(id_proxy, dtype=np.int),
-                            model=model,
-                            connectivity=connectivity,
-                            coupling=coupling,
-                            integrator=integrator,
-                            monitors=(monitors,),
-                            initial_conditions=init,
-                            )
+            voi=np.array([0]),
+            synchronization_time=synchronization_time,
+            cosim_monitors=(RawCosim(),),
+            proxy_inds=np.asarray(id_proxy, dtype=np.int_),
+            model=model,
+            connectivity=connectivity,
+            coupling=coupling,
+            integrator=integrator,
+            monitors=(monitors,),
+            initial_conditions=init,
+        )
         sim_5.configure()
-        sim_5.run() # run the first steps because the history is delayed
+        sim_5.run()  # run the first steps because the history is delayed
 
         sim_to_sync_time = int(SIMULATION_LENGTH / synchronization_time)
         sync_steps = int(synchronization_time / integrator.dt)
 
         result_5_all = [np.empty((0,)), np.empty((sync_steps, 2, 76, 1))]
 
         for j in range(0, sim_to_sync_time):
             result_5_all_step = sim_5.run(
                 cosim_updates=[np.array([result_all[0][0][(sync_steps * j) + i] for i in range(sync_steps)]),
                                np.array([result_all[0][1][(sync_steps * j) + i][0][id_proxy]
                                          for i in range(sync_steps)]).reshape((sync_steps, 1, len(id_proxy), 1))])
             result_5_all[0] = np.concatenate((result_5_all[0], result_5_all_step[0][0]))
             result_5_all[1] = np.concatenate((result_5_all[1], result_5_all_step[0][1]))
 
-        for i in range(int(SIMULATION_LENGTH/integrator.dt)):
+        for i in range(int(SIMULATION_LENGTH / integrator.dt)):
             np.testing.assert_array_equal(result_all[0][1][i][0][len(id_proxy):],
-                                          result_5_all[1][i+sync_steps, 0, len(id_proxy):])
+                                          result_5_all[1][i + sync_steps, 0, len(id_proxy):])
             np.testing.assert_array_equal(result_all[0][1][i][0][:len(id_proxy)],
-                                          result_5_all[1][i+sync_steps, 0, :len(id_proxy)])
+                                          result_5_all[1][i + sync_steps, 0, :len(id_proxy)])
 
     def test_without_proxy_coupling(self):
         connectivity, coupling, integrator, monitors, sim, result, result_all = self._reference_simulation()
         # The modify model without proxy
         np.random.seed(42)
         init = np.concatenate((np.random.random_sample((385, 1, 76, 1)),
                                np.random.random_sample((385, 1, 76, 1))), axis=1)
         model = ReducedWongWangProxy(tau_s=np.random.rand(76))
         synchronization_time = SYNCHRONIZATION_TIME
         # Initialise a Simulator -- Model, Connectivity, Integrator, and Monitors.
         sim_6 = CoSimulator(
-                            voi=np.array([0]),
-                            synchronization_time=synchronization_time,
-                            cosim_monitors=(CosimCoupling(coupling=coupling),),
-                            proxy_inds=np.asarray([0], dtype=np.int),
-                            model=model,
-                            connectivity=connectivity,
-                            coupling=coupling,
-                            integrator=integrator,
-                            monitors=(monitors,),
-                            initial_conditions=init,
-                            )
+            voi=np.array([0]),
+            synchronization_time=synchronization_time,
+            cosim_monitors=(CosimCoupling(coupling=coupling),),
+            proxy_inds=np.asarray([0], dtype=np.int_),
+            model=model,
+            connectivity=connectivity,
+            coupling=coupling,
+            integrator=integrator,
+            monitors=(monitors,),
+            initial_conditions=init,
+        )
         sim_6.configure()
 
         sim_to_sync_time = int(SIMULATION_LENGTH / synchronization_time)
         sync_steps = int(synchronization_time / integrator.dt)
 
         with pytest.raises(ValueError):
-           coupling_future = sim_6.loop_cosim_monitor_output(sync_steps, 1)
+            coupling_future = sim_6.loop_cosim_monitor_output(sync_steps, 1)
 
         coupling_future = sim_6.loop_cosim_monitor_output()
 
         for i in range(sim_to_sync_time):
             result_2 = sim_6.run(
-                cosim_updates=[np.arange(i * synchronization_time, (i + 1) * synchronization_time, 0.1)-synchronization_time,
-                               np.zeros((int(synchronization_time/0.1),1,1,1))])[0][1][:, 0, 0, 0]
-            np.testing.assert_array_equal(result[i*sync_steps:(i+1)*sync_steps]*0.0, result_2)
+                cosim_updates=[
+                    np.arange(i * synchronization_time, (i + 1) * synchronization_time, 0.1) - synchronization_time,
+                    np.zeros((int(synchronization_time / 0.1), 1, 1, 1))])[0][1][:, 0, 0, 0]
+            np.testing.assert_array_equal(result[i * sync_steps:(i + 1) * sync_steps] * 0.0, result_2)
             assert np.sum(np.isnan(sim_6.loop_cosim_monitor_output()[0][1])) == 9
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/proxy_precision_delay_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,47 +35,47 @@
     """
     compare the result between simulation with one proxy and without proxy and different delay
     """
 
     def test_precision_delay(self):
         weight = np.array([[2, 8, 10], [0.2, 0.5, 0.1], [3, 0.6, 1]])
         delay = np.array([[0.6, 0.5, 1.0], [0.7, 0.8, 3.0], [1.0, 0.5, 0.7]])
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0]]] * max)
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0], [0.2, 0.0]]] * max)
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
         synchronization_time = 0.1 * 4
         proxy_id = [0]
-        no_proxy = [1,2]
+        no_proxy = [1, 2]
 
         # simulation with one proxy
         np.random.seed(42)
         sim = TvbSim(weight, delay, proxy_id, resolution_simulation,
                      synchronization_time, initial_condition=initial_condition)
-        time, s , result= sim(synchronization_time, rate=True)
+        time, s, result = sim(synchronization_time, rate=True)
 
         # full simulation
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation,
                          synchronization_time, initial_condition=initial_condition)
         time, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
 
         # compare with the CosimMonitor RawCosim
-        np.testing.assert_array_equal(np.squeeze(result_ref[:,no_proxy,:], axis=2),
-                        np.squeeze(result[0][:,no_proxy,:], axis=2))
-        np.testing.assert_array_equal(np.squeeze(s_ref[:,no_proxy,:], axis=2),
-                          np.squeeze(s[0][:,no_proxy,:], axis=2))
+        np.testing.assert_array_equal(np.squeeze(result_ref[:, no_proxy, :], axis=2),
+                                      np.squeeze(result[0][:, no_proxy, :], axis=2))
+        np.testing.assert_array_equal(np.squeeze(s_ref[:, no_proxy, :], axis=2),
+                                      np.squeeze(s[0][:, no_proxy, :], axis=2))
 
         for i in range(0, 1000):
             time, s, result = sim(synchronization_time,
                                   rate_data=[time, result_ref[:, proxy_id][:, :, 0]], rate=True)
 
             # compare with RawDelayed monitor, delayed by synchronization_time
             np.testing.assert_array_equal(result_ref[:, no_proxy, :], result[1][:, no_proxy, :])
-            np.testing.assert_array_equal(result_ref[:, proxy_id, :]*np.NAN, result[1][:, proxy_id, :])
+            np.testing.assert_array_equal(result_ref[:, proxy_id, :] * np.NAN, result[1][:, proxy_id, :])
             np.testing.assert_array_equal(s_ref, s[1])
 
             time, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
 
             # compare with the CosimMonitor RawCosim
             np.testing.assert_array_equal(result_ref[:, no_proxy, :], result[0][:, no_proxy, :])
             np.testing.assert_array_equal(s_ref[:, no_proxy, :], s[0][:, no_proxy, :])
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/proxy_precision_multiple_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,47 +39,47 @@
     def test_precision_delay(self):
         weight = np.array([[5, 2, 4, 0],
                            [8, 5, 4, 1],
                            [6, 1, 7, 9],
                            [10, 0, 5, 6]])
         delay = np.array([[0.1, 0.1, 0.1, 0.1], [0.1, 0.1, 0.1, 0.1],
                           [0.1, 0.1, 0.1, 0.1], [0.1, 0.1, 0.1, 0.1]]) * 10
-        max = np.int(np.max(delay)*10+1)
-        init_value = np.array([[[0.1,0.0], [0.1,0.0], [0.2,0.0], [0.2,0.0]]* max] )
+        max = np.int_(np.max(delay) * 10 + 1)
+        init_value = np.array([[[0.1, 0.0], [0.1, 0.0], [0.2, 0.0], [0.2, 0.0]] * max])
         initial_condition = init_value.reshape((max, 2, weight.shape[0], 1))
         resolution_simulation = 0.1
         synchronization_time = np.min(delay)
-        proxy_id = [0,2,3]
+        proxy_id = [0, 2, 3]
         no_proxy = [1]
 
         # simulation with one or more proxy
         np.random.seed(42)
         sim = TvbSim(weight, delay, proxy_id, resolution_simulation,
                      synchronization_time, initial_condition=initial_condition)
-        time, s , result= sim(synchronization_time, rate=True)
+        time, s, result = sim(synchronization_time, rate=True)
 
         # full simulation
         np.random.seed(42)
         sim_ref = TvbSim(weight, delay, [], resolution_simulation,
                          synchronization_time, initial_condition=initial_condition)
         time, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
 
         # compare with the CosimMonitor RawCosim
         np.testing.assert_array_equal(np.squeeze(result_ref[:, no_proxy, :], axis=2),
-                        np.squeeze(result[0][:, no_proxy, :], axis=2))
+                                      np.squeeze(result[0][:, no_proxy, :], axis=2))
         np.testing.assert_array_equal(np.squeeze(s_ref[:, no_proxy, :], axis=2),
-                          np.squeeze(s[0][:, no_proxy, :], axis=2))
+                                      np.squeeze(s[0][:, no_proxy, :], axis=2))
 
         for i in range(0, 1000):
             time, s, result = sim(synchronization_time,
                                   rate_data=[time, result_ref[:, proxy_id][:, :, 0]], rate=True)
 
             # compare with RawDelayed monitor, delayed by synchronization_time
             np.testing.assert_array_equal(result_ref[:, no_proxy, :], result[1][:, no_proxy, :])
-            np.testing.assert_array_equal(result_ref[:, proxy_id, :]*np.NAN, result[1][:, proxy_id, :])
+            np.testing.assert_array_equal(result_ref[:, proxy_id, :] * np.NAN, result[1][:, proxy_id, :])
             np.testing.assert_array_equal(s_ref, s[1])
 
             time, s_ref, result_ref = sim_ref(synchronization_time, rate=True)
 
             # compare with the CosimMonitor RawCosim
             np.testing.assert_array_equal(result_ref[:, no_proxy, :], result[0][:, no_proxy, :])
             np.testing.assert_array_equal(s_ref[:, no_proxy, :], s[0][:, no_proxy, :])
```

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/proxy_precision_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/simple/update_function_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/simple/update_function_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/cosimulation/synchronization_time_set.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/cosimulation/synchronization_time_set.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/model/model_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/model/model_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb/contrib/tests/scripts/time_series_test.py` & `tvb-contrib-2.8.1/tvb/contrib/tests/scripts/time_series_test.py`

 * *Files identical despite different names*

### Comparing `tvb-contrib-2.7.2/tvb_contrib.egg-info/PKG-INFO` & `tvb-contrib-2.8.1/tvb_contrib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-contrib
-Version: 2.7.2
+Version: 2.8.1
 Summary: A package with TVB contributed additions to the simulator, useful for scripting.
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Stuart Knock, Dionysios Perdikis, Paula Sanz Leon, Bogdan Valean, Marmaduke Woodman
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience contrib
```

### Comparing `tvb-contrib-2.7.2/tvb_contrib.egg-info/SOURCES.txt` & `tvb-contrib-2.8.1/tvb_contrib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

