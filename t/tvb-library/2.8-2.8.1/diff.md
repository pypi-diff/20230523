# Comparing `tmp/tvb-library-2.8.tar.gz` & `tmp/tvb-library-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-library-2.8.tar", last modified: Mon Feb 20 15:25:41 2023, max compression
+gzip compressed data, was "tvb-library-2.8.1.tar", last modified: Tue May 23 12:09:27 2023, max compression
```

## Comparing `tvb-library-2.8.tar` & `tvb-library-2.8.1.tar`

### file list

```diff
@@ -1,270 +1,264 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.828412 tvb-library-2.8/
--rw-r--r--   0 root         (0) root         (0)      946 2023-02-16 21:35:08.000000 tvb-library-2.8/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-02-16 21:35:08.000000 tvb-library-2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      168 2023-02-16 21:35:08.000000 tvb-library-2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5457 2023-02-20 15:25:41.828412 tvb-library-2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4949 2023-02-16 21:35:08.000000 tvb-library-2.8/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-20 15:25:41.828412 tvb-library-2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2854 2023-02-20 15:19:36.000000 tvb-library-2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.743413 tvb-library-2.8/tvb/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.752412 tvb-library-2.8/tvb/analyzers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4686 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/fft.py
--rw-r--r--   0 root         (0) root         (0)    14415 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/fmri_balloon.py
--rw-r--r--   0 root         (0) root         (0)    14416 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/graph.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/ica.py
--rw-r--r--   0 root         (0) root         (0)    13711 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/ica_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     4098 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/info.py
--rw-r--r--   0 root         (0) root         (0)     3499 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/metric_kuramoto_index.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/metric_proxy_metastability.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/metric_variance_global.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/metric_variance_of_node_variance.py
--rw-r--r--   0 root         (0) root         (0)     5013 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/node_coherence.py
--rw-r--r--   0 root         (0) root         (0)    12520 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/node_complex_coherence.py
--rw-r--r--   0 root         (0) root         (0)     4500 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/pca.py
--rw-r--r--   0 root         (0) root         (0)     7060 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/analyzers/wavelet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.753413 tvb-library-2.8/tvb/basic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.755412 tvb-library-2.8/tvb/basic/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6020 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/config/environment.py
--rw-r--r--   0 root         (0) root         (0)     8381 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/config/profile_settings.py
--rw-r--r--   0 root         (0) root         (0)    16344 2023-02-20 15:19:36.000000 tvb-library-2.8/tvb/basic/config/settings.py
--rw-r--r--   0 root         (0) root         (0)     6323 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/config/stored.py
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-20 15:21:28.000000 tvb-library-2.8/tvb/basic/config/tvb.version
--rw-r--r--   0 root         (0) root         (0)     1666 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/config/utils.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.756412 tvb-library-2.8/tvb/basic/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/logger/builder.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/logger/library_logger.conf
--rw-r--r--   0 root         (0) root         (0)     1728 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/logger/library_logger_test.conf
--rw-r--r--   0 root         (0) root         (0)     2027 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/logger/simple_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.758412 tvb-library-2.8/tvb/basic/neotraits/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25352 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/_attr.py
--rw-r--r--   0 root         (0) root         (0)    12075 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/_core.py
--rw-r--r--   0 root         (0) root         (0)    10753 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/_declarative_base.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/api.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/ex.py
--rw-r--r--   0 root         (0) root         (0)     6637 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/neotraits/info.py
--rw-r--r--   0 root         (0) root         (0)     5928 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/profile.py
--rw-r--r--   0 root         (0) root         (0)     8553 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/basic/readers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.775412 tvb-library-2.8/tvb/datatypes/
--rw-r--r--   0 root         (0) root         (0)     1590 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33607 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/connectivity.py
--rw-r--r--   0 root         (0) root         (0)     9158 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/cortex.py
--rw-r--r--   0 root         (0) root         (0)    20099 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/equations.py
--rw-r--r--   0 root         (0) root         (0)     3650 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/fcd.py
--rw-r--r--   0 root         (0) root         (0)     3308 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/graph.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/local_connectivity.py
--rw-r--r--   0 root         (0) root         (0)     8235 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/mode_decompositions.py
--rw-r--r--   0 root         (0) root         (0)     9306 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/patterns.py
--rw-r--r--   0 root         (0) root         (0)     5654 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/projections.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/region_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11810 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/sensors.py
--rw-r--r--   0 root         (0) root         (0)    12479 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/spectral.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/structural.py
--rw-r--r--   0 root         (0) root         (0)    29883 2023-02-20 14:28:21.000000 tvb-library-2.8/tvb/datatypes/surfaces.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/temporal_correlations.py
--rw-r--r--   0 root         (0) root         (0)    12200 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/tracts.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/datatypes/volumes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.776412 tvb-library-2.8/tvb/rateML/
--rwxr-xr-x   0 root         (0) root         (0)    22851 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/README.md
--rwxr-xr-x   0 root         (0) root         (0)    15067 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XML2model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.779412 tvb-library-2.8/tvb/rateML/XMLmodels/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/epileptor.xml
--rw-r--r--   0 root         (0) root         (0)     2107 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/kuramoto.xml
--rw-r--r--   0 root         (0) root         (0)     4396 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/model_template.xml
--rw-r--r--   0 root         (0) root         (0)     5096 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/montbrio.xml
--rw-r--r--   0 root         (0) root         (0)     3916 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/oscillator.xml
--rw-r--r--   0 root         (0) root         (0)     5966 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/rwongwang.xml
--rw-r--r--   0 root         (0) root         (0)     6318 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/rwongwang_deco.xml
--rw-r--r--   0 root         (0) root         (0)    12080 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/XMLmodels/zerlaut.xml
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.782412 tvb-library-2.8/tvb/rateML/generatedModels/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.784412 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10351 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/epileptorref.c
--rw-r--r--   0 root         (0) root         (0)     6901 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c
--rw-r--r--   0 root         (0) root         (0)     7865 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/montbrioref.c
--rw-r--r--   0 root         (0) root         (0)     7862 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c
--rw-r--r--   0 root         (0) root         (0)     8667 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c
--rw-r--r--   0 root         (0) root         (0)     9812 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/epileptor.c
--rw-r--r--   0 root         (0) root         (0)     5461 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/epileptor.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/kuramoto.c
--rw-r--r--   0 root         (0) root         (0)     1571 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/kuramoto.py
--rw-r--r--   0 root         (0) root         (0)     7745 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/montbrio.c
--rw-r--r--   0 root         (0) root         (0)     3181 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/montbrio.py
--rw-r--r--   0 root         (0) root         (0)     8939 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/montbrio_heun.c
--rw-r--r--   0 root         (0) root         (0)     7858 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/oscillator.c
--rw-r--r--   0 root         (0) root         (0)     3359 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/oscillator.py
--rw-r--r--   0 root         (0) root         (0)     8433 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/rwongwang.c
--rw-r--r--   0 root         (0) root         (0)     5577 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/rwongwang.py
--rw-r--r--   0 root         (0) root         (0)    17337 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/zerlaut.c
--rw-r--r--   0 root         (0) root         (0)     7711 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/generatedModels/zerlaut_func.h
--rw-r--r--   0 root         (0) root         (0)    25374 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/rML_v0.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.785412 tvb-library-2.8/tvb/rateML/run/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/run/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17732 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/run/model_driver.py
--rw-r--r--   0 root         (0) root         (0)    18267 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/run/model_driver_bold.py
--rw-r--r--   0 root         (0) root         (0)    17347 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/run/model_driver_heun.py
--rw-r--r--   0 root         (0) root         (0)    18301 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/run/model_driver_zerlaut.py
--rwxr-xr-x   0 root         (0) root         (0)     2972 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/run/regular_run.py
--rwxr-xr-x   0 root         (0) root         (0)    13603 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/tmpl8_cuda.py
--rw-r--r--   0 root         (0) root         (0)    17614 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/tmpl8_driver.py
--rwxr-xr-x   0 root         (0) root         (0)     5191 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/rateML/tmpl8_python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.789412 tvb-library-2.8/tvb/simulator/
--rw-r--r--   0 root         (0) root         (0)     1397 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.791412 tvb-library-2.8/tvb/simulator/_numba/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6168 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/coupling.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/gpu_bench.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/integrators.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/loops.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/models.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/_numba/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.793412 tvb-library-2.8/tvb/simulator/backend/
--rw-r--r--   0 root         (0) root         (0)     1295 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/base.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/cu.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/nb.py
--rw-r--r--   0 root         (0) root         (0)     9404 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/nb_mpr.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/np.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/ref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.797412 tvb-library-2.8/tvb/simulator/backend/templates/
--rw-r--r--   0 root         (0) root         (0)     2131 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/cu-base.cu.mako
--rw-r--r--   0 root         (0) root         (0)     2141 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/cu-coupling.cu.mako
--rw-r--r--   0 root         (0) root         (0)     3245 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/cu-defs.cu.mako
--rw-r--r--   0 root         (0) root         (0)     2027 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/cu-dfuns.cu.mako
--rw-r--r--   0 root         (0) root         (0)     2639 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/cu-sim-ode.cu.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.797412 tvb-library-2.8/tvb/simulator/backend/templates/generated/
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/generated/.gitignore
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/nb-coupling.py.mako
--rw-r--r--   0 root         (0) root         (0)     2145 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/nb-coupling2.py.mako
--rw-r--r--   0 root         (0) root         (0)     1950 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/nb-dfuns.py.mako
--rw-r--r--   0 root         (0) root         (0)     6061 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/nb-integrate.py.mako
--rw-r--r--   0 root         (0) root         (0)     5359 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/nb-montbrio.py.mako
--rw-r--r--   0 root         (0) root         (0)     3234 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/nb-sim.py.mako
--rw-r--r--   0 root         (0) root         (0)     2492 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/np-coupling.py.mako
--rw-r--r--   0 root         (0) root         (0)     1786 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/np-dfuns.py.mako
--rw-r--r--   0 root         (0) root         (0)     3739 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/np-integrate.py.mako
--rw-r--r--   0 root         (0) root         (0)     2219 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/backend/templates/np-sim.py.mako
--rw-r--r--   0 root         (0) root         (0)     6177 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/common.py
--rw-r--r--   0 root         (0) root         (0)    16501 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/coupling.py
--rw-r--r--   0 root         (0) root         (0)     6283 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/descriptors.py
--rw-r--r--   0 root         (0) root         (0)    12555 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/history.py
--rw-r--r--   0 root         (0) root         (0)    22441 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/integrators.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/lab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.802412 tvb-library-2.8/tvb/simulator/models/
--rw-r--r--   0 root         (0) root         (0)     6367 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.808412 tvb-library-2.8/tvb/simulator/models/__pycache__/
--rw-r--r--   0 root         (0) root         (0)   233001 2023-02-16 22:01:41.000000 tvb-library-2.8/tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.get_fluct_regime_vars-459.py310.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1534 2023-02-16 22:01:41.000000 tvb-library-2.8/tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.get_fluct_regime_vars-459.py310.nbi
--rw-r--r--   0 root         (0) root         (0)    77852 2023-02-16 22:01:41.000000 tvb-library-2.8/tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.threshold_func-513.py310.1.nbc
--rw-r--r--   0 root         (0) root         (0)     1308 2023-02-16 22:01:41.000000 tvb-library-2.8/tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.threshold_func-513.py310.nbi
--rw-r--r--   0 root         (0) root         (0)    11018 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/base.py
--rw-r--r--   0 root         (0) root         (0)    21582 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/epileptor.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/epileptorT.py
--rw-r--r--   0 root         (0) root         (0)    16115 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/epileptor_rs.py
--rw-r--r--   0 root         (0) root         (0)    29904 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/epileptorcodim3.py
--rw-r--r--   0 root         (0) root         (0)     7902 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/hopfield.py
--rw-r--r--   0 root         (0) root         (0)    35533 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/infinite_theta.py
--rw-r--r--   0 root         (0) root         (0)    23147 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/jansen_rit.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/kuramotoT.py
--rw-r--r--   0 root         (0) root         (0)    18473 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/larter_breakspear.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/linear.py
--rw-r--r--   0 root         (0) root         (0)    22719 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/oscillator.py
--rw-r--r--   0 root         (0) root         (0)    25605 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/stefanescu_jirsa.py
--rw-r--r--   0 root         (0) root         (0)    16734 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/wilson_cowan.py
--rw-r--r--   0 root         (0) root         (0)     6739 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/wong_wang.py
--rw-r--r--   0 root         (0) root         (0)    15293 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/wong_wang_exc_inh.py
--rw-r--r--   0 root         (0) root         (0)    37228 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/models/zerlaut.py
--rw-r--r--   0 root         (0) root         (0)    43223 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/monitors.py
--rw-r--r--   0 root         (0) root         (0)    10525 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/noise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.813412 tvb-library-2.8/tvb/simulator/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23618 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/base_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.813412 tvb-library-2.8/tvb/simulator/plot/colourmaps/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/colourmaps/BlackToBlue
--rw-r--r--   0 root         (0) root         (0)     9150 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/compare_integrators.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/config.py
--rw-r--r--   0 root         (0) root         (0)    14154 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/epileptor_plotter.py
--rw-r--r--   0 root         (0) root         (0)     8068 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/head_plotter.py
--rw-r--r--   0 root         (0) root         (0)     5840 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/head_plotter_3d.py
--rw-r--r--   0 root         (0) root         (0)    35895 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/phase_plane_interactive.py
--rw-r--r--   0 root         (0) root         (0)     3956 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/plotter.py
--rw-r--r--   0 root         (0) root         (0)    20529 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/power_spectra_interactive.py
--rw-r--r--   0 root         (0) root         (0)    32161 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/time_series_plotter.py
--rw-r--r--   0 root         (0) root         (0)    29755 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/timeseries_interactive.py
--rw-r--r--   0 root         (0) root         (0)    22861 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/tools.py
--rw-r--r--   0 root         (0) root         (0)    10714 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/plot/utils.py
--rw-r--r--   0 root         (0) root         (0)    28923 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/simulator/simulator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.814412 tvb-library-2.8/tvb/tests/
--rw-r--r--   0 root         (0) root         (0)     2099 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/bench.py
--rw-r--r--   0 root         (0) root         (0)     6437 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/bench_against_mpr_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.814412 tvb-library-2.8/tvb/tests/library/
--rw-r--r--   0 root         (0) root         (0)     1653 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/base_testcase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.815412 tvb-library-2.8/tvb/tests/library/basic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/basic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.816412 tvb-library-2.8/tvb/tests/library/basic/neotraits/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/basic/neotraits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/basic/neotraits/_attr_test.py
--rw-r--r--   0 root         (0) root         (0)    27221 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/basic/neotraits/neotraits_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.820412 tvb-library-2.8/tvb/tests/library/datatypes/
--rw-r--r--   0 root         (0) root         (0)   115069 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/Edited_Connectivity.h5
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7570 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/connectivity_test.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/equations_test.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/graph_test.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/mode_decompositions_test.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/patterns_test.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/projections_test.py
--rw-r--r--   0 root         (0) root         (0)     4209 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/sensors_test.py
--rw-r--r--   0 root         (0) root         (0)     5725 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/spectral_test.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/surfaces_test.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/temporal_correlations_test.py
--rw-r--r--   0 root         (0) root         (0)     4446 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/timeseries_test.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/datatypes/volumes_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.824412 tvb-library-2.8/tvb/tests/library/simulator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15561 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/_numba_tests.py
--rw-r--r--   0 root         (0) root         (0)    10929 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/_opencl_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.826412 tvb-library-2.8/tvb/tests/library/simulator/backend/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/backendtestbase.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/cubackend_test.py
--rw-r--r--   0 root         (0) root         (0)    14631 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py
--rw-r--r--   0 root         (0) root         (0)    11349 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/nbbackend_test.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/nbmprperf_test.py
--rw-r--r--   0 root         (0) root         (0)     9706 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/backend/npbackend_test.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/common_test.py
--rw-r--r--   0 root         (0) root         (0)     5840 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/coupling_test.py
--rw-r--r--   0 root         (0) root         (0)     5221 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/descriptors_test.py
--rw-r--r--   0 root         (0) root         (0)     3913 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/history_test.py
--rw-r--r--   0 root         (0) root         (0)     9442 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/integrators_test.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/modelir_test.py
--rw-r--r--   0 root         (0) root         (0)    12034 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/models_test.py
--rw-r--r--   0 root         (0) root         (0)    10916 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/monitors_test.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/noise_test.py
--rw-r--r--   0 root         (0) root         (0)    10229 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/rateml_test.py
--rw-r--r--   0 root         (0) root         (0)     2802 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/regionmapping_test.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/rngperf_test.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/simulator_step_test.py
--rw-r--r--   0 root         (0) root         (0)    15884 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/simulator_test.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/library/simulator/stimulation_test.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-02-16 21:35:08.000000 tvb-library-2.8/tvb/tests/validate_model_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 15:25:41.827412 tvb-library-2.8/tvb_library.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5457 2023-02-20 15:25:41.000000 tvb-library-2.8/tvb_library.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8890 2023-02-20 15:25:41.000000 tvb-library-2.8/tvb_library.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 15:25:41.000000 tvb-library-2.8/tvb_library.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      183 2023-02-20 15:25:41.000000 tvb-library-2.8/tvb_library.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-20 15:25:41.000000 tvb-library-2.8/tvb_library.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.577964 tvb-library-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)      946 2023-05-23 11:37:04.000000 tvb-library-2.8.1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-library-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-23 11:37:04.000000 tvb-library-2.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-05-23 12:09:27.576964 tvb-library-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-05-23 11:37:04.000000 tvb-library-2.8.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:27.577964 tvb-library-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-05-23 11:37:04.000000 tvb-library-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.431956 tvb-library-2.8.1/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.442957 tvb-library-2.8.1/tvb/analyzers/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/fft.py
+-rw-r--r--   0 root         (0) root         (0)    14371 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/fmri_balloon.py
+-rw-r--r--   0 root         (0) root         (0)    14416 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/ica.py
+-rw-r--r--   0 root         (0) root         (0)    13711 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/ica_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/info.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/metric_kuramoto_index.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/metric_proxy_metastability.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/metric_variance_global.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/metric_variance_of_node_variance.py
+-rw-r--r--   0 root         (0) root         (0)     5015 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/node_coherence.py
+-rw-r--r--   0 root         (0) root         (0)    12504 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/node_complex_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/pca.py
+-rw-r--r--   0 root         (0) root         (0)     7060 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/analyzers/wavelet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.444957 tvb-library-2.8.1/tvb/basic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.449957 tvb-library-2.8.1/tvb/basic/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6020 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/config/environment.py
+-rw-r--r--   0 root         (0) root         (0)     9210 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/config/profile_settings.py
+-rw-r--r--   0 root         (0) root         (0)    16346 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/config/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/config/stored.py
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-23 12:05:19.000000 tvb-library-2.8.1/tvb/basic/config/tvb.version
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/config/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.452957 tvb-library-2.8.1/tvb/basic/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/logger/builder.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/logger/library_logger.conf
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/logger/library_logger_test.conf
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/logger/simple_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.456958 tvb-library-2.8.1/tvb/basic/neotraits/
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25350 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/_attr.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/_core.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/_declarative_base.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/api.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/ex.py
+-rw-r--r--   0 root         (0) root         (0)     6755 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/neotraits/info.py
+-rw-r--r--   0 root         (0) root         (0)     5928 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/profile.py
+-rw-r--r--   0 root         (0) root         (0)     8553 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/basic/readers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.468958 tvb-library-2.8.1/tvb/datatypes/
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33607 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     9158 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/cortex.py
+-rw-r--r--   0 root         (0) root         (0)    20099 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/equations.py
+-rw-r--r--   0 root         (0) root         (0)     3650 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/fcd.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/graph.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/local_connectivity.py
+-rw-r--r--   0 root         (0) root         (0)     8235 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/mode_decompositions.py
+-rw-r--r--   0 root         (0) root         (0)     9306 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/projections.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/region_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11811 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    12479 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/spectral.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/structural.py
+-rw-r--r--   0 root         (0) root         (0)    29883 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/surfaces.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/temporal_correlations.py
+-rw-r--r--   0 root         (0) root         (0)    12200 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/tracts.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/datatypes/volumes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.472958 tvb-library-2.8.1/tvb/rateML/
+-rwxr-xr-x   0 root         (0) root         (0)    22851 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/README.md
+-rwxr-xr-x   0 root         (0) root         (0)    15067 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XML2model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.477959 tvb-library-2.8.1/tvb/rateML/XMLmodels/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/epileptor.xml
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/kuramoto.xml
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/model_template.xml
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/montbrio.xml
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/oscillator.xml
+-rw-r--r--   0 root         (0) root         (0)     5966 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/rwongwang.xml
+-rw-r--r--   0 root         (0) root         (0)     6318 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/rwongwang_deco.xml
+-rw-r--r--   0 root         (0) root         (0)    12080 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/XMLmodels/zerlaut.xml
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.486959 tvb-library-2.8.1/tvb/rateML/generatedModels/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.489959 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10351 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/epileptorref.c
+-rw-r--r--   0 root         (0) root         (0)     6901 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/montbrioref.c
+-rw-r--r--   0 root         (0) root         (0)     7862 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c
+-rw-r--r--   0 root         (0) root         (0)     9812 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/epileptor.c
+-rw-r--r--   0 root         (0) root         (0)     5461 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/epileptor.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/kuramoto.c
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/kuramoto.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/montbrio.c
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/montbrio.py
+-rw-r--r--   0 root         (0) root         (0)     8939 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/montbrio_heun.c
+-rw-r--r--   0 root         (0) root         (0)     7858 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/oscillator.c
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/oscillator.py
+-rw-r--r--   0 root         (0) root         (0)     8433 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/rwongwang.c
+-rw-r--r--   0 root         (0) root         (0)     5577 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/rwongwang.py
+-rw-r--r--   0 root         (0) root         (0)    17337 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/zerlaut.c
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/generatedModels/zerlaut_func.h
+-rw-r--r--   0 root         (0) root         (0)    25374 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/rML_v0.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.493960 tvb-library-2.8.1/tvb/rateML/run/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/run/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17732 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/run/model_driver.py
+-rw-r--r--   0 root         (0) root         (0)    18267 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/run/model_driver_bold.py
+-rw-r--r--   0 root         (0) root         (0)    17347 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/run/model_driver_heun.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/run/model_driver_zerlaut.py
+-rwxr-xr-x   0 root         (0) root         (0)     2972 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/run/regular_run.py
+-rwxr-xr-x   0 root         (0) root         (0)    13603 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/tmpl8_cuda.py
+-rw-r--r--   0 root         (0) root         (0)    17614 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/tmpl8_driver.py
+-rwxr-xr-x   0 root         (0) root         (0)     5191 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/rateML/tmpl8_python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.500960 tvb-library-2.8.1/tvb/simulator/
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.506960 tvb-library-2.8.1/tvb/simulator/_numba/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6168 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/coupling.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/gpu_bench.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/integrators.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/loops.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/models.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/_numba/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.509960 tvb-library-2.8.1/tvb/simulator/backend/
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/base.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/cu.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/nb.py
+-rw-r--r--   0 root         (0) root         (0)     9404 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/nb_mpr.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/np.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/ref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.518961 tvb-library-2.8.1/tvb/simulator/backend/templates/
+-rw-r--r--   0 root         (0) root         (0)     2131 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/cu-base.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/cu-coupling.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     3245 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/cu-defs.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/cu-dfuns.cu.mako
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/cu-sim-ode.cu.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.519961 tvb-library-2.8.1/tvb/simulator/backend/templates/generated/
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/generated/.gitignore
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/nb-coupling.py.mako
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/nb-coupling2.py.mako
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/nb-dfuns.py.mako
+-rw-r--r--   0 root         (0) root         (0)     6061 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/nb-integrate.py.mako
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/nb-montbrio.py.mako
+-rw-r--r--   0 root         (0) root         (0)     3234 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/nb-sim.py.mako
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/np-coupling.py.mako
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/np-dfuns.py.mako
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/np-integrate.py.mako
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/backend/templates/np-sim.py.mako
+-rw-r--r--   0 root         (0) root         (0)     6271 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/common.py
+-rw-r--r--   0 root         (0) root         (0)    16501 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/coupling.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/descriptors.py
+-rw-r--r--   0 root         (0) root         (0)    12555 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/history.py
+-rw-r--r--   0 root         (0) root         (0)    22441 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/integrators.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/lab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.531961 tvb-library-2.8.1/tvb/simulator/models/
+-rw-r--r--   0 root         (0) root         (0)     6448 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11018 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/base.py
+-rw-r--r--   0 root         (0) root         (0)    21582 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/epileptor.py
+-rw-r--r--   0 root         (0) root         (0)    16115 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/epileptor_rs.py
+-rw-r--r--   0 root         (0) root         (0)    29904 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/epileptorcodim3.py
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/hopfield.py
+-rw-r--r--   0 root         (0) root         (0)    35533 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/infinite_theta.py
+-rw-r--r--   0 root         (0) root         (0)    23147 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/jansen_rit.py
+-rw-r--r--   0 root         (0) root         (0)    12504 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/k_ion_exchange.py
+-rw-r--r--   0 root         (0) root         (0)    18473 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/larter_breakspear.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/linear.py
+-rw-r--r--   0 root         (0) root         (0)    22719 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/oscillator.py
+-rw-r--r--   0 root         (0) root         (0)    25605 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/stefanescu_jirsa.py
+-rw-r--r--   0 root         (0) root         (0)    16734 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/wilson_cowan.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/wong_wang.py
+-rw-r--r--   0 root         (0) root         (0)    15293 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/wong_wang_exc_inh.py
+-rw-r--r--   0 root         (0) root         (0)    40228 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/models/zerlaut.py
+-rw-r--r--   0 root         (0) root         (0)    43225 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/monitors.py
+-rw-r--r--   0 root         (0) root         (0)    10525 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/noise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.538962 tvb-library-2.8.1/tvb/simulator/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23618 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/base_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.539962 tvb-library-2.8.1/tvb/simulator/plot/colourmaps/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/colourmaps/BlackToBlue
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/compare_integrators.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/config.py
+-rw-r--r--   0 root         (0) root         (0)    14154 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/epileptor_plotter.py
+-rw-r--r--   0 root         (0) root         (0)     8068 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/head_plotter.py
+-rw-r--r--   0 root         (0) root         (0)     5840 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/head_plotter_3d.py
+-rw-r--r--   0 root         (0) root         (0)    35926 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/phase_plane_interactive.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/plotter.py
+-rw-r--r--   0 root         (0) root         (0)    20529 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/power_spectra_interactive.py
+-rw-r--r--   0 root         (0) root         (0)    32161 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/time_series_plotter.py
+-rw-r--r--   0 root         (0) root         (0)    29755 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/timeseries_interactive.py
+-rw-r--r--   0 root         (0) root         (0)    22865 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/tools.py
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/plot/utils.py
+-rw-r--r--   0 root         (0) root         (0)    28923 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/simulator/simulator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.541962 tvb-library-2.8.1/tvb/tests/
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/bench.py
+-rw-r--r--   0 root         (0) root         (0)     6437 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/bench_against_mpr_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.542962 tvb-library-2.8.1/tvb/tests/library/
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/base_testcase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.543962 tvb-library-2.8.1/tvb/tests/library/basic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/basic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.545962 tvb-library-2.8.1/tvb/tests/library/basic/neotraits/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/basic/neotraits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/basic/neotraits/_attr_test.py
+-rw-r--r--   0 root         (0) root         (0)    27593 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/basic/neotraits/neotraits_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.555963 tvb-library-2.8.1/tvb/tests/library/datatypes/
+-rw-r--r--   0 root         (0) root         (0)   115069 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/Edited_Connectivity.h5
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7570 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/connectivity_test.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/equations_test.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/graph_test.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/mode_decompositions_test.py
+-rw-r--r--   0 root         (0) root         (0)     4646 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/patterns_test.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/projections_test.py
+-rw-r--r--   0 root         (0) root         (0)     4209 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/sensors_test.py
+-rw-r--r--   0 root         (0) root         (0)     5725 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/spectral_test.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/surfaces_test.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/temporal_correlations_test.py
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/timeseries_test.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/datatypes/volumes_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.568963 tvb-library-2.8.1/tvb/tests/library/simulator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15561 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/_numba_tests.py
+-rw-r--r--   0 root         (0) root         (0)    10929 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/_opencl_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.573963 tvb-library-2.8.1/tvb/tests/library/simulator/backend/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/backendtestbase.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/cubackend_test.py
+-rw-r--r--   0 root         (0) root         (0)    14631 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py
+-rw-r--r--   0 root         (0) root         (0)    11349 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/nbbackend_test.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/nbmprperf_test.py
+-rw-r--r--   0 root         (0) root         (0)     9706 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/backend/npbackend_test.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/common_test.py
+-rw-r--r--   0 root         (0) root         (0)     5840 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/coupling_test.py
+-rw-r--r--   0 root         (0) root         (0)     5221 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/descriptors_test.py
+-rw-r--r--   0 root         (0) root         (0)     3913 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/history_test.py
+-rw-r--r--   0 root         (0) root         (0)     9442 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/integrators_test.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/modelir_test.py
+-rw-r--r--   0 root         (0) root         (0)    12034 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/models_test.py
+-rw-r--r--   0 root         (0) root         (0)    10916 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/monitors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/noise_test.py
+-rw-r--r--   0 root         (0) root         (0)    10229 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/rateml_test.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/regionmapping_test.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/rngperf_test.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/simulator_step_test.py
+-rw-r--r--   0 root         (0) root         (0)    15884 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/simulator_test.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/library/simulator/stimulation_test.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-05-23 11:37:04.000000 tvb-library-2.8.1/tvb/tests/validate_model_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:27.575964 tvb-library-2.8.1/tvb_library.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-05-23 12:09:27.000000 tvb-library-2.8.1/tvb_library.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8450 2023-05-23 12:09:27.000000 tvb-library-2.8.1/tvb_library.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:27.000000 tvb-library-2.8.1/tvb_library.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-23 12:09:27.000000 tvb-library-2.8.1/tvb_library.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:27.000000 tvb-library-2.8.1/tvb_library.egg-info/top_level.txt
```

### Comparing `tvb-library-2.8/AUTHORS` & `tvb-library-2.8.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/LICENSE` & `tvb-library-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/PKG-INFO` & `tvb-library-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tvb-library
-Version: 2.8
+Version: 2.8.1
 Summary: A package for performing whole brain simulations
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
-Author: Marmaduke Woodman, Stuart Knock, Paula Sanz Leon, Viktor Jirsa
+Author: Marmaduke Woodman,  Jan Fousek, Stuart Knock, Paula Sanz Leon, Viktor Jirsa
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience human animal neuronal dynamics models delay
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `tvb-library-2.8/README.rst` & `tvb-library-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/setup.py` & `tvb-library-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     python setup.py install/develop
 """
 
 import os
 import shutil
 import setuptools
 
-LIBRARY_VERSION = "2.8"
+LIBRARY_VERSION = "2.8.1"
 
-LIBRARY_TEAM = "Marmaduke Woodman, Stuart Knock, Paula Sanz Leon, Viktor Jirsa"
+LIBRARY_TEAM = "Marmaduke Woodman,  Jan Fousek, Stuart Knock, Paula Sanz Leon, Viktor Jirsa"
 
 LIBRARY_REQUIRED_PACKAGES = ["autopep8", "Deprecated", "docutils", "ipywidgets", "lxml", "mako>=1.1.4", "matplotlib",
                              "networkx", "numba", "numexpr", "numpy", "pylems", "scipy", "six"]
 
 LIBRARY_REQUIRED_EXTRA = ["h5py",  "pytest", "pytest-benchmark", "pytest-xdist", "tvb-gdist", "tvb-data"]
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as fd:
```

### Comparing `tvb-library-2.8/tvb/__init__.py` & `tvb-library-2.8.1/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/fft.py` & `tvb-library-2.8.1/tvb/analyzers/fft.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/fmri_balloon.py` & `tvb-library-2.8.1/tvb/analyzers/fmri_balloon.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,16 +216,15 @@
         # NOTE: hard coded initial conditions
         state = numpy.zeros((input_shape[0], balloon_nvar, input_shape[2], input_shape[3]))  # s
         state[0, 1, :] = 1.  # f
         state[0, 2, :] = 1.  # v
         state[0, 3, :] = 1.  # q
 
         # BOLD model coefficients
-        k = self.compute_derived_parameters()
-        k1, k2, k3 = k[0], k[1], k[2]
+        k1, k2, k3 = self.compute_derived_parameters()
 
         # prepare integrator
         self.integrator.dt = 1. / self.time_series.sample_rate # s
         self.integrator.configure()
         self.log.debug("Integration time step size will be: %s seconds" % str(self.integrator.dt))
 
         scheme = self.integrator.scheme
@@ -303,15 +302,15 @@
             Generalized BOLD signal model.
             Page 400 in [Stephan2007]_, Eq. (12)
             """
             k1 = 4.3 * self.nu_0 * self.E0 * self.TE
             k2 = self.epsilon * self.r_0 * self.E0 * self.TE
             k3 = 1 - self.epsilon
 
-        return numpy.array([k1, k2, k3])
+        return k1, k2, k3
 
     def input_transformation(self, time_series, mode):
         """
         Perform an operation on the input time-series.
         """
 
         self.log.debug("Computing: %s on the input time series" % str(mode))
```

### Comparing `tvb-library-2.8/tvb/analyzers/graph.py` & `tvb-library-2.8.1/tvb/analyzers/graph.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/ica.py` & `tvb-library-2.8.1/tvb/analyzers/ica.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/ica_algorithm.py` & `tvb-library-2.8.1/tvb/analyzers/ica_algorithm.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/info.py` & `tvb-library-2.8.1/tvb/analyzers/info.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/metric_kuramoto_index.py` & `tvb-library-2.8.1/tvb/analyzers/metric_kuramoto_index.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/metric_proxy_metastability.py` & `tvb-library-2.8.1/tvb/analyzers/metric_proxy_metastability.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/metric_variance_global.py` & `tvb-library-2.8.1/tvb/analyzers/metric_variance_global.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/metric_variance_of_node_variance.py` & `tvb-library-2.8.1/tvb/analyzers/metric_variance_of_node_variance.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/node_coherence.py` & `tvb-library-2.8.1/tvb/analyzers/node_coherence.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,11 +134,11 @@
     log.debug(narray_describe(coh))
     log.debug("freq")
     log.debug(narray_describe(freq))
 
     spec = spectral.CoherenceSpectrum(
         source=time_series,
         nfft=nfft,
-        array_data=coh.astype(numpy.float),
+        array_data=coh.astype(numpy.float64),
         frequency=freq)
     return spec
```

### Comparing `tvb-library-2.8/tvb/analyzers/node_complex_coherence.py` & `tvb-library-2.8.1/tvb/analyzers/node_complex_coherence.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     nfreq = int(numpy.min([max_freq, numpy.floor((seg_tpts + zeropad) / 2.0) + 1]))
 
     resulted_shape, av_result_shape = complex_coherence_result_shape(time_series.data.shape, max_freq, epoch_length,
                                                                      segment_length, segment_shift,
                                                                      time_series.sample_period, zeropad,
                                                                      average_segments)
     cs = numpy.zeros(resulted_shape, dtype=numpy.complex128)
-    av = numpy.matrix(numpy.zeros(av_result_shape, dtype=numpy.complex128))
+    av = numpy.zeros(av_result_shape, dtype=numpy.complex128)
     coh = numpy.zeros(resulted_shape, dtype=numpy.complex128)
 
     # Apply windowing function
     if window_function is not None:
         if window_function not in SUPPORTED_WINDOWING_FUNCTIONS:
             log.error("Windowing function is: %s" % window_function)
             log.error("Must be in: %s" % str(SUPPORTED_WINDOWING_FUNCTIONS))
@@ -238,21 +238,21 @@
                     for j in numpy.arange(nepochs):
                         cs[:, :, f, j] = cs[:, :, f, j] - av[:, f, j] * av[:, f, j].conj().T
 
     # Compute Complex Coherence
     ndim = len(cs.shape)
     if ndim == 3:
         for i in numpy.arange(cs.shape[2]):
-            temp = numpy.matrix(cs[:, :, i])
+            temp = numpy.array(cs[:, :, i])
             coh[:, :, i] = cs[:, :, i] / numpy.sqrt(temp.diagonal().conj().T * temp.diagonal())
 
     elif ndim == 4:
         for i in numpy.arange(cs.shape[2]):
             for j in numpy.arange(cs.shape[3]):
-                temp = numpy.matrix(numpy.squeeze(cs[:, :, i, j]))
+                temp = numpy.array(numpy.squeeze(cs[:, :, i, j]))
                 coh[:, :, i, j] = temp / numpy.sqrt(temp.diagonal().conj().T * temp.diagonal().T)
 
     log.debug("result")
     log.debug(narray_describe(cs))
     spectra = spectral.ComplexCoherenceSpectrum(source=time_series,
                                                 array_data=coh,
                                                 cross_spectrum=cs,
```

### Comparing `tvb-library-2.8/tvb/analyzers/pca.py` & `tvb-library-2.8.1/tvb/analyzers/pca.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/analyzers/wavelet.py` & `tvb-library-2.8.1/tvb/analyzers/wavelet.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/config/environment.py` & `tvb-library-2.8.1/tvb/basic/config/environment.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/config/profile_settings.py` & `tvb-library-2.8.1/tvb/basic/config/profile_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 #
 
 """
 Prepare TVB settings to be grouped under various profile classes.
 
 .. moduleauthor:: Lia Domide <lia.domide@codemart.ro>
 """
+
 import os
 import sys
-
 from tvb.basic.config import stored
 from tvb.basic.config.environment import Environment
 from tvb.basic.config.settings import ClusterSettings, DBSettings, VersionSettings, WebSettings, HPCSettings
 
 
 class BaseSettingsProfile(object):
     TVB_USER_HOME = os.environ.get('TVB_USER_HOME', '~')
@@ -81,14 +81,24 @@
         self.MAX_RANGE_NUMBER = self.manager.get_attribute(stored.KEY_MAX_RANGE_NR, 2000, int)
         # Max number of threads in the pool of ops running in parallel. TO be correlated with CPU cores
         self.MAX_THREADS_NUMBER = self.manager.get_attribute(stored.KEY_MAX_THREAD_NR, 4, int)
         self.OPERATIONS_BACKGROUND_JOB_INTERVAL = self.manager.get_attribute(stored.KEY_OP_BACKGROUND_INTERVAL, 60, int)
         # The maximum disk space that can be used by one single user, in KB.
         self.MAX_DISK_SPACE = self.manager.get_attribute(stored.KEY_MAX_DISK_SPACE_USR, 5 * 1024 * 1024, int)
 
+        # The url of the elasticsearch server
+        self.ELASTICSEARCH_URL = self.manager.get_attribute(stored.KEY_ELASTICSEARCH_URL, "", str)
+        # The security key that is used to connect to the server
+        self.ELASTICSEARCH_API_KEY = self.manager.get_attribute(stored.KEY_ELASTICSEARCH_API_KEY, "", str)
+        # The request timeout for the elasticsearch rest calls
+        self.ELASTICSEARCH_LOGGING_INDEX = self.manager.get_attribute(stored.KEY_ELASTICSEARCH_LOGGING_INDEX, "", str)
+        self.ELASTICSEARCH_REQUEST_TIMEOUT = self.manager.get_attribute(stored.KEY_ELASTICSEARCH_REQUEST_TIMEOUT, 30, int)
+        # The number of logs in a message batch that are sent to the server
+        self.ELASTICSEARCH_BUFFER_THRESHOLD = self.manager.get_attribute(stored.KEY_ELASTICSEARCH_BUFFER_THRESHOLD, 1000000, int)
+
     @property
     def BIN_FOLDER(self):
         """
         Return path towards tvb_bin location. It will be used in some environment for determining the starting point
         """
         try:
             import tvb_bin
```

### Comparing `tvb-library-2.8/tvb/basic/config/settings.py` & `tvb-library-2.8.1/tvb/basic/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
     Gather settings related to various version numbers of TVB application
     """
 
     SVN_GIT_MIGRATION_REVISION = 10000
 
     # Current release number
-    BASE_VERSION = "2.8"
+    BASE_VERSION = "2.8.1"
 
     # Current DB version. Create a new migration script from command line and copy its gid here
     DB_STRUCTURE_VERSION = '32d4bf9f8def'
 
     # This is the version of the data stored in H5 and XML files
     # and should be used by next versions to know how to import
     # data in TVB format, in case data structure changes.
```

### Comparing `tvb-library-2.8/tvb/basic/config/stored.py` & `tvb-library-2.8.1/tvb/basic/config/stored.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,21 @@
 KEY_OPENSHIFT_DEPLOY = "OPENSHIFT_DEPLOY"
 KEY_OPENSHIFT_NAMESPACE = "OPENSHIFT_NAMESPACE"
 KEY_OPENSHIFT_APPLICATION = "OPENSHIFT_APPLICATION"
 KEY_PROCESSING_OPERATIONS_APPLICATION = "PROCESSING_OPERATIONS_APPLICATION"
 KEY_DATA_ENCRYPTION_HANDLER_APPLICATION = "DATA_ENCRYPTION_HANDLER_APPLICATION"
 KEY_DEPLOY_CONTEXT = "DEPLOY_CONTEXT"
 KEY_REST_DEPLOY_CONTEXT = "REST_DEPLOY_CONTEXT"
+KEY_ELASTICSEARCH_API_KEY = "ELASTICSEARCH_API_KEY"
+KEY_ELASTICSEARCH_URL = "ELASTICSEARCH_URL"
+KEY_ELASTICSEARCH_LOGGING_INDEX = "ELASTICSEARCH_LOGGING_INDEX"
+KEY_ELASTICSEARCH_REQUEST_TIMEOUT = "ELASTICSEARCH_REQUEST_TIMEOUT"
+KEY_ELASTICSEARCH_BUFFER_THRESHOLD = "ELASTICSEARCH_BUFFER_THRESHOLD"
+
+UTF8 = "utf-8"
 
 
 class SettingsManager(object):
     def __init__(self, config_file_location):
         self.config_file_location = config_file_location
         self.stored_settings = self._read_config_file()
 
@@ -90,25 +97,25 @@
         Get data from the configurations file in the form of a dictionary.
         Return empty dictionary if file not present.
         """
         if not os.path.exists(self.config_file_location):
             return {}
 
         config_dict = {}
-        with open(self.config_file_location, 'r') as cfg_file:
+        with open(self.config_file_location, 'r', encoding= UTF8) as cfg_file:
             data = cfg_file.read()
             entries = [line for line in data.split('\n') if not line.startswith('#') and len(line.strip()) > 0]
             for one_entry in entries:
                 name, value = one_entry.split('=', 1)
-                config_dict[name] = value
+                config_dict[name] = value.strip() if value else ""
         return config_dict
 
     def _store_config_file(self, config_dict):
 
-        with open(self.config_file_location, 'w') as file_writer:
+        with open(self.config_file_location, 'w',  encoding= UTF8) as file_writer:
             for key in config_dict:
                 file_writer.write(key + '=' + str(config_dict[key]) + '\n')
 
         self.stored_settings = self._read_config_file()
 
     def add_entries_to_config_file(self, input_data):
         """
@@ -139,15 +146,15 @@
 
         self._store_config_file(config_dict)
 
     def write_config_data(self, config_dict):
         """
         Overwrite anything already existent in the config file
         """
-        with open(self.config_file_location, 'w') as file_writer:
+        with open(self.config_file_location, 'w',  encoding= UTF8) as file_writer:
             for key in config_dict:
                 file_writer.write(key + '=' + str(config_dict[key]) + '\n')
 
         self.stored_settings = self._read_config_file()
 
     def get_attribute(self, key, default=None, dtype=str):
         """
```

### Comparing `tvb-library-2.8/tvb/basic/config/utils.py` & `tvb-library-2.8.1/tvb/basic/config/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/exceptions.py` & `tvb-library-2.8.1/tvb/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/logger/builder.py` & `tvb-library-2.8.1/tvb/basic/logger/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 import importlib
 import os
 import weakref
 import logging
 import logging.config
 from tvb.basic.profile import TvbProfile
 from tvb.basic.config.profile_settings import MATLABLibraryProfile
+from logging import StreamHandler
 
 
 class LoggerBuilder(object):
     """
     Class taking care of uniform Python logger initialization. 
     It uses the Python native logging package. 
     It's purpose is just to offer a common mechanism for initializing all modules in a package.
@@ -73,14 +74,17 @@
         """
         self._loggers[parent_module] = logger = logging.getLogger(parent_module)
         return logger
 
     def set_loggers_level(self, level):
         for logger in self._loggers.values():
             logger.setLevel(level)
+            for handler in logger.handlers:
+                if isinstance(handler, StreamHandler) and handler.stream.name == 'stdout':
+                    handler.setLevel(min(level, handler.level))
 
 
 # We make sure a single instance of logger-builder is created.
 if "GLOBAL_LOGGER_BUILDER" not in globals():
 
     if TvbProfile.is_library_mode():
         GLOBAL_LOGGER_BUILDER = LoggerBuilder('tvb.basic.logger')
@@ -91,7 +95,16 @@
 def get_logger(parent_module=''):
     """
     Function to retrieve a new Python logger instance for current module.
     
     :param parent_module: module name for which to create logger.
     """
     return GLOBAL_LOGGER_BUILDER.build_logger(parent_module)
+
+
+def set_loggers_level(level):
+    """
+    Function to set the logging level for the loggers and their console handlers
+
+    :param level: the level to be set
+    """
+    GLOBAL_LOGGER_BUILDER.set_loggers_level(level)
```

### Comparing `tvb-library-2.8/tvb/basic/logger/library_logger.conf` & `tvb-library-2.8.1/tvb/basic/logger/library_logger.conf`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/logger/library_logger_test.conf` & `tvb-library-2.8.1/tvb/basic/logger/library_logger_test.conf`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/logger/simple_handler.py` & `tvb-library-2.8.1/tvb/basic/logger/simple_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/neotraits/__init__.py` & `tvb-library-2.8.1/tvb/basic/neotraits/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/neotraits/_attr.py` & `tvb-library-2.8.1/tvb/basic/neotraits/_attr.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
 
 """
 This private module implements concrete declarative attributes
 """
-import collections.abc
 import inspect
 import numpy
 import types
 import typing
+from collections.abc import Sequence
 from ._declarative_base import _Attr, MetaType
 from .ex import TraitValueError, TraitTypeError, TraitAttributeError, TraitFinalAttributeError
 from tvb.basic.logger.builder import get_logger
 
 if typing.TYPE_CHECKING:
     from ._core import HasTraits
 
@@ -231,15 +231,15 @@
     The attribute is a list of values.
     Choices and type are reinterpreted as applying not to the list but to the elements of it
     """
 
     def __init__(self, of=object, default=(), doc='', label='', final=False, choices=None):
         # type: (type, tuple, str, str, bool, typing.Optional[tuple]) -> None
         super(List, self).__init__(
-            field_type=collections.abc.Sequence,
+            field_type=Sequence,
             default=default,
             doc=doc,
             label=label,
             required=True,
             final=final,
             choices=None,
         )
```

### Comparing `tvb-library-2.8/tvb/basic/neotraits/_core.py` & `tvb-library-2.8.1/tvb/basic/neotraits/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 import uuid
 from enum import Enum
 import numpy
 import typing
 from six import add_metaclass
 from numpy.random import RandomState
 from scipy.sparse import csc_matrix, spmatrix
-
 from ._attr import Attr
 from ._declarative_base import _Property, MetaType
 from .info import trait_object_str, trait_object_repr_html, narray_summary_info
 from .ex import TraitAttributeError, TraitTypeError, TraitError, TraitFinalAttributeError
 from tvb.basic.logger.builder import get_logger
 
 
@@ -189,15 +188,15 @@
 
     # The base __init__ and __str__ rely upon metadata gathered by MetaType
     # we could have injected these in MetaType, but we don't need meta powers
     # this is simpler to grok
 
     gid = Attr(field_type=uuid.UUID)
 
-    TYPES_TO_DEEPCOPY = (RandomState, csc_matrix, spmatrix)
+    TYPES_TO_DEEPCOPY = (RandomState, csc_matrix, spmatrix, list, tuple)
 
     def __init__(self, **kwargs):
         """
         The default init accepts kwargs for all declarative attrs
         and sets them to the given values
         """
         # cls just to emphasise that the metadata is on the class not on instances
```

### Comparing `tvb-library-2.8/tvb/basic/neotraits/_declarative_base.py` & `tvb-library-2.8.1/tvb/basic/neotraits/_declarative_base.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/neotraits/api.py` & `tvb-library-2.8.1/tvb/basic/neotraits/api.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/neotraits/ex.py` & `tvb-library-2.8.1/tvb/basic/neotraits/ex.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/neotraits/info.py` & `tvb-library-2.8.1/tvb/basic/neotraits/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,29 +111,29 @@
     if ar.size == 0:
         return {f'{ar_name} {key_empty}': 'True'} if ar_name else {key_empty: 'True'}
 
     ret = {key_shape: str(ar.shape),
            key_type: str(ar.dtype)}
 
     if ar.dtype.kind in 'iufc':
-        key_nan = numpy.isnan(ar).any()
-        if key_nan:
+        has_nan = numpy.isnan(ar).any()
+        if has_nan:
             ret[key_nan] = 'True'
         ret[key_min_max] = '[{:g}, {:g}, {:g}]'.format(ar.min(), numpy.median(ar), ar.max())
 
     if condensed:
         condensed_desc = ""
         if ar.shape == (1,):
             condensed_desc += str(ar.item())
         else:
             for key in [key_min_max, key_type, key_shape, key_empty, key_nan]:
                 if key in ret:
                     condensed_desc += f' {key} = {ret[key]}'
 
-        return {ar_name: condensed_desc} if ar_name else {'': condensed_desc}
+        return {ar_name: condensed_desc} if ar_name else {'array': condensed_desc}
 
     if ar_name:
         return {ar_name + ' ' + k: v for k, v in ret.items()}
     else:
         return ret
 
 
@@ -186,32 +186,39 @@
         result.append(row_fmt.format(k, summary[k]))
 
     result += ['</tbody></table>']
 
     return '\n'.join(result)
 
 
+def convert_rst_to_html(doc):
+    """
+    Convert from rst to html that can be rendered by Mathjax
+    """
+    kwargs = {
+        'writer_name': 'html',
+        'settings_overrides': {
+            '_disable_config': True,
+            'report_level': 5,
+            'math_output': "MathJax /dummy.js",
+        },
+    }
+
+    return publish_parts(doc, **kwargs)['html_body']
+
+
 def prepare_html(doc):
     # type: (str) -> str
     """
     Create html (that can be further enhanced by MathJax) from the description received as parameter
     """
     try:
         html_id = uuid.uuid1()
 
-        kwargs = {
-            'writer_name': 'html',
-            'settings_overrides': {
-                '_disable_config': True,
-                'report_level': 5,
-                'math_output': "MathJax /dummy.js",
-            },
-        }
-
-        html = publish_parts(doc, **kwargs)['html_body']
+        html = convert_rst_to_html(doc)
 
         html = html.replace('div class="document"', f'div class="document" id="{html_id}"', 1)
         html += fr'<script>MathJax.Hub.Queue(["Typeset", MathJax.Hub, "{html_id}"]);</script>'
 
     except Exception:
         html = str(doc)
     return html
```

### Comparing `tvb-library-2.8/tvb/basic/profile.py` & `tvb-library-2.8.1/tvb/basic/profile.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/basic/readers.py` & `tvb-library-2.8.1/tvb/basic/readers.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/__init__.py` & `tvb-library-2.8.1/tvb/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/connectivity.py` & `tvb-library-2.8.1/tvb/datatypes/connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/cortex.py` & `tvb-library-2.8.1/tvb/datatypes/cortex.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/equations.py` & `tvb-library-2.8.1/tvb/datatypes/equations.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/fcd.py` & `tvb-library-2.8.1/tvb/datatypes/fcd.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/graph.py` & `tvb-library-2.8.1/tvb/datatypes/graph.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/local_connectivity.py` & `tvb-library-2.8.1/tvb/datatypes/local_connectivity.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/mode_decompositions.py` & `tvb-library-2.8.1/tvb/datatypes/mode_decompositions.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/patterns.py` & `tvb-library-2.8.1/tvb/datatypes/patterns.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/projections.py` & `tvb-library-2.8.1/tvb/datatypes/projections.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/region_mapping.py` & `tvb-library-2.8.1/tvb/datatypes/region_mapping.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/sensors.py` & `tvb-library-2.8.1/tvb/datatypes/sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         result = Sensors()
 
         if content_type == '.txt.bz2':
             decompressor = bz2.BZ2Decompressor()
             bytes_stream = decompressor.decompress(bytes_stream)
 
         content_str = StringIO(bytes_stream.decode())
-        result.labels = numpy.loadtxt(content_str, dtype=numpy.str, skiprows=0, usecols=(0,))
+        result.labels = numpy.loadtxt(content_str, dtype=numpy.str_, skiprows=0, usecols=(0,))
         content_str.seek(0)
         result.locations = numpy.loadtxt(content_str, dtype=numpy.float64, skiprows=0, usecols=(1, 2, 3))
 
         return result
 
     def configure(self):
         """
```

### Comparing `tvb-library-2.8/tvb/datatypes/spectral.py` & `tvb-library-2.8.1/tvb/datatypes/spectral.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/structural.py` & `tvb-library-2.8.1/tvb/datatypes/structural.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/surfaces.py` & `tvb-library-2.8.1/tvb/datatypes/surfaces.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/temporal_correlations.py` & `tvb-library-2.8.1/tvb/datatypes/temporal_correlations.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/time_series.py` & `tvb-library-2.8.1/tvb/datatypes/time_series.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/tracts.py` & `tvb-library-2.8.1/tvb/datatypes/tracts.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/datatypes/volumes.py` & `tvb-library-2.8.1/tvb/datatypes/volumes.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/README.md` & `tvb-library-2.8.1/tvb/rateML/README.md`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XML2model.py` & `tvb-library-2.8.1/tvb/rateML/XML2model.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/epileptor.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/epileptor.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/kuramoto.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/kuramoto.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/model_template.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/model_template.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/montbrio.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/montbrio.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/oscillator.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/oscillator.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/rwongwang.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/rwongwang.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/rwongwang_deco.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/rwongwang_deco.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/XMLmodels/zerlaut.xml` & `tvb-library-2.8.1/tvb/rateML/XMLmodels/zerlaut.xml`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/epileptorref.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/epileptorref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/kuramotoref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/montbrioref.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/montbrioref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/oscillatorref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/cuda_refs/rwongwangref.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/epileptor.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/epileptor.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/epileptor.py` & `tvb-library-2.8.1/tvb/rateML/generatedModels/epileptor.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/kuramoto.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/kuramoto.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/kuramoto.py` & `tvb-library-2.8.1/tvb/rateML/generatedModels/kuramoto.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/montbrio.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/montbrio.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/montbrio.py` & `tvb-library-2.8.1/tvb/rateML/generatedModels/montbrio.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/montbrio_heun.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/montbrio_heun.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/oscillator.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/oscillator.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/oscillator.py` & `tvb-library-2.8.1/tvb/rateML/generatedModels/oscillator.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/rwongwang.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/rwongwang.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/rwongwang.py` & `tvb-library-2.8.1/tvb/rateML/generatedModels/rwongwang.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/zerlaut.c` & `tvb-library-2.8.1/tvb/rateML/generatedModels/zerlaut.c`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/generatedModels/zerlaut_func.h` & `tvb-library-2.8.1/tvb/rateML/generatedModels/zerlaut_func.h`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/rML_v0.xsd` & `tvb-library-2.8.1/tvb/rateML/rML_v0.xsd`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/run/model_driver.py` & `tvb-library-2.8.1/tvb/rateML/run/model_driver.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/run/model_driver_bold.py` & `tvb-library-2.8.1/tvb/rateML/run/model_driver_bold.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/run/model_driver_heun.py` & `tvb-library-2.8.1/tvb/rateML/run/model_driver_heun.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/run/model_driver_zerlaut.py` & `tvb-library-2.8.1/tvb/rateML/run/model_driver_zerlaut.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/run/regular_run.py` & `tvb-library-2.8.1/tvb/rateML/run/regular_run.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/tmpl8_cuda.py` & `tvb-library-2.8.1/tvb/rateML/tmpl8_cuda.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/tmpl8_driver.py` & `tvb-library-2.8.1/tvb/rateML/tmpl8_driver.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/rateML/tmpl8_python.py` & `tvb-library-2.8.1/tvb/rateML/tmpl8_python.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/__init__.py` & `tvb-library-2.8.1/tvb/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/_numba/coupling.py` & `tvb-library-2.8.1/tvb/simulator/_numba/coupling.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/_numba/gpu_bench.py` & `tvb-library-2.8.1/tvb/simulator/_numba/gpu_bench.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/_numba/integrators.py` & `tvb-library-2.8.1/tvb/simulator/_numba/integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/_numba/loops.py` & `tvb-library-2.8.1/tvb/simulator/_numba/loops.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/_numba/models.py` & `tvb-library-2.8.1/tvb/simulator/_numba/models.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/_numba/util.py` & `tvb-library-2.8.1/tvb/simulator/_numba/util.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/__init__.py` & `tvb-library-2.8.1/tvb/simulator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/base.py` & `tvb-library-2.8.1/tvb/simulator/backend/base.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/cu.py` & `tvb-library-2.8.1/tvb/simulator/backend/cu.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/nb.py` & `tvb-library-2.8.1/tvb/simulator/backend/nb.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/nb_mpr.py` & `tvb-library-2.8.1/tvb/simulator/backend/nb_mpr.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/np.py` & `tvb-library-2.8.1/tvb/simulator/backend/np.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/ref.py` & `tvb-library-2.8.1/tvb/simulator/backend/ref.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/__init__.py` & `tvb-library-2.8.1/tvb/simulator/backend/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/cu-base.cu.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/cu-base.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/cu-coupling.cu.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/cu-coupling.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/cu-defs.cu.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/cu-defs.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/cu-dfuns.cu.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/cu-dfuns.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/cu-sim-ode.cu.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/cu-sim-ode.cu.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/nb-coupling.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/nb-coupling.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/nb-coupling2.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/nb-coupling2.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/nb-dfuns.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/nb-dfuns.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/nb-integrate.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/nb-integrate.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/nb-montbrio.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/nb-montbrio.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/nb-sim.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/nb-sim.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/np-coupling.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/np-coupling.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/np-dfuns.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/np-dfuns.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/np-integrate.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/np-integrate.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/backend/templates/np-sim.py.mako` & `tvb-library-2.8.1/tvb/simulator/backend/templates/np-sim.py.mako`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/common.py` & `tvb-library-2.8.1/tvb/simulator/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,19 @@
 import numpy
 import os
 import re
 import six
 import logging
 from tvb.basic.logger.builder import GLOBAL_LOGGER_BUILDER, get_logger
 from .backend.ref import ReferenceBackend
+from deprecated import deprecated
 
 
+
+@deprecated(reason="Use builder.set_logger_level instead")
 def log_debug(debug=False, timestamp=False, prefix=''):
     level_name = 'DEBUG' if debug else 'INFO'
     level = getattr(logging, level_name)
     GLOBAL_LOGGER_BUILDER.set_loggers_level(level)
     LOG = get_logger(__name__)
     for handler in LOG.root.handlers:
         handler.setLevel(level)
```

### Comparing `tvb-library-2.8/tvb/simulator/coupling.py` & `tvb-library-2.8.1/tvb/simulator/coupling.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/descriptors.py` & `tvb-library-2.8.1/tvb/simulator/descriptors.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/history.py` & `tvb-library-2.8.1/tvb/simulator/history.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/integrators.py` & `tvb-library-2.8.1/tvb/simulator/integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/lab.py` & `tvb-library-2.8.1/tvb/simulator/lab.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,32 +27,34 @@
 """
 tvb.simulator.lab is a umbrella module designed to make console and scripting
 work easier by importing all the simulator pieces at once.
 
 .. moduleauthor:: Marmaduke Woodman <marmaduke.woodman@univ-amu.fr>
 
 """
-
+import logging
 import os
 import sys
 
+from tvb.basic.logger.builder import set_loggers_level
+
 # avoid segfaulting in absence of X11 DISPLAY
 if sys.platform in ('linux2', ) and 'DISPLAY' not in os.environ:
     try:
         import matplotlib as mpl
         mpl.use('Agg')
     except Exception:
         pass
 
 from tvb.basic.profile import TvbProfile
 TvbProfile.set_profile(TvbProfile.LIBRARY_PROFILE)
 
 from tvb.simulator.common import get_logger, log_debug
 
-log_debug(False)
+set_loggers_level(logging.INFO)
 
 from tvb.simulator import (simulator, models, coupling, integrators, monitors, noise)
 from tvb.datatypes import (connectivity, surfaces, equations, patterns, region_mapping, sensors, cortex,
                            local_connectivity, time_series)
 
 from tvb.simulator.plot.tools import (hinton_diagram, plot_3d_centres, plot_connectivity,
                                       plot_fast_kde, plot_local_connectivity, plot_matrix,
```

### Comparing `tvb-library-2.8/tvb/simulator/models/__init__.py` & `tvb-library-2.8.1/tvb/simulator/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     MONTBRIO_PAZO_ROXIN = "MontbrioPazoRoxin"
     COOMBES_BYRNE = "CoombesByrne"
     COOMBES_BYRNE_2D = "CoombesByrne2D"
     GAST_SCHMIDT_KNOSCHE_SD = "GastSchmidtKnosche_SD"
     GAST_SCHMIDT_KNOSCHE_SF = "GastSchmidtKnosche_SF"
     DUMONT_GUTKIN = "DumontGutkin"
     DECO_BALANCED_EXC_INH = "DecoBalancedExcInh"
+    K_ION_EXCHANGE = "KIonEx"
 
     def get_class(self):
         return _get_imported_model(self.value)
 
     @staticmethod
     def get_base_model_subclasses():
         return [model.get_class() for model in list(ModelsEnum) if model != ModelsEnum.BASE_MODEL]
@@ -108,14 +109,15 @@
     'oscillator': [ModelsEnum.GENERIC_2D_OSCILLATOR, ModelsEnum.KURAMOTO, ModelsEnum.SUP_HOPF],
     'stefanescu_jirsa': [ModelsEnum.REDUCED_SET_HINDMARSH_ROSE, ModelsEnum.REDUCED_SET_FITZ_HUGH_NAGUMO],
     'wilson_cowan': [ModelsEnum.WILSON_COWAN],
     'wong_wang': [ModelsEnum.REDUCED_WONG_WANG],
     'wong_wang_exc_inh': [ModelsEnum.REDUCED_WONG_WANG_EXC_INH, ModelsEnum.DECO_BALANCED_EXC_INH],
     'zerlaut': [ModelsEnum.ZERLAUT_FIRST_ORDER, ModelsEnum.ZERLAUT_SECOND_ORDER],
     'infinite_theta': [ModelsEnum.MONTBRIO_PAZO_ROXIN, ModelsEnum.COOMBES_BYRNE, ModelsEnum.COOMBES_BYRNE_2D, ModelsEnum.GAST_SCHMIDT_KNOSCHE_SF, ModelsEnum.GAST_SCHMIDT_KNOSCHE_SD, ModelsEnum.DUMONT_GUTKIN],
+    'k_ion_exchange': [ModelsEnum.K_ION_EXCHANGE],
 }
 
 
 def _find_lems_models():
     import os, tvb.dsl
     dsl_path = os.path.dirname(os.path.abspath(tvb.dsl.__file__))
     xml_folder = os.path.join(dsl_path, 'NeuroML', 'XMLmodels')
```

### Comparing `tvb-library-2.8/tvb/simulator/models/base.py` & `tvb-library-2.8.1/tvb/simulator/models/base.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/epileptor.py` & `tvb-library-2.8.1/tvb/simulator/models/epileptor.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/epileptor_rs.py` & `tvb-library-2.8.1/tvb/simulator/models/epileptor_rs.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/epileptorcodim3.py` & `tvb-library-2.8.1/tvb/simulator/models/epileptorcodim3.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/hopfield.py` & `tvb-library-2.8.1/tvb/simulator/models/hopfield.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/infinite_theta.py` & `tvb-library-2.8.1/tvb/simulator/models/infinite_theta.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/jansen_rit.py` & `tvb-library-2.8.1/tvb/simulator/models/jansen_rit.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/kuramotoT.py` & `tvb-library-2.8.1/tvb/simulator/models/linear.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,64 +20,66 @@
 #
 #   CITATION:
 # When using The Virtual Brain for scientific publications, please cite it as explained here:
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
 
-from tvb.simulator.models.base import Model, ModelNumbaDfun
+"""
+Generic linear model.
+"""
+
 import numpy
-from numpy import *
-from numba import guvectorize, float64
+from .base import Model
 from tvb.basic.neotraits.api import NArray, Final, List, Range
 
 
-class KuramotoT(ModelNumbaDfun):
-        
-    omega = NArray(
-        label=":math:`omega`",
-        default=numpy.array([60.0 * 2.0 * 3.1415927 / 1e3]),
-        doc=""""""
-    )    
+class Linear(Model):
+    gamma = NArray(
+        label=r":math:`\gamma`",
+        default=numpy.array([-10.0]),
+        domain=Range(lo=-100.0, hi=0.0, step=1.0),
+        doc="The damping coefficient specifies how quickly the node's activity relaxes, must be larger"
+            " than the node's in-degree in order to remain stable.")
 
     state_variable_range = Final(
         label="State Variable ranges [lo, hi]",
-        default={"V": numpy.array([0.0])},
-        doc="""state variables"""
-    )
+        default={"x": numpy.array([-1, 1])},
+        doc="Range used for state variable initialization and visualization.")
 
-    state_variable_boundaries = Final(
-        label="State Variable boundaries [lo, hi]",
-        default={"V": numpy.array([-2, 1])},
-    )
     variables_of_interest = List(
         of=str,
-        label="Variables or quantities available to Monitors",
-        choices=('V', ),
-        default=('V', ),
-        doc="Variables to monitor"
+        label="Variables watched by Monitors",
+        choices=("x",),
+        default=("x",), )
+
+    coupling_terms = Final(
+        label="Coupling terms",
+        # how to unpack coupling array
+        default=["c"]
     )
 
-    state_variables = ['V']
-
-    _nvar = 1
-    cvar = numpy.array([0,], dtype = numpy.int32)
-
-    def dfun(self, vw, c, local_coupling=0.0):
-        vw_ = vw.reshape(vw.shape[:-1]).T
-        c_ = c.reshape(c.shape[:-1]).T
-        deriv = _numba_dfun_KuramotoT(vw_, c_, self.omega, local_coupling)
-
-        return deriv.T[..., numpy.newaxis]
-
-@guvectorize([(float64[:], float64[:], float64, float64, float64[:])], '(n),(m)' + ',()'*2 + '->(n)', nopython=True)
-def _numba_dfun_KuramotoT(vw, coupling, omega, local_coupling, dx):
-    "Gufunc for KuramotoT model equations."
-
-    # long-range coupling
-    c_pop0 = coupling[0]
+    state_variable_dfuns = Final(
+        label="Drift functions",
+        default={
+            "x": "gamma * x + c",
+        }
+    )
 
-    V = vw[0]
+    parameter_names = List(
+        of=str,
+        label="List of parameters for this model",
+        default=tuple('gamma'.split()))
 
+    state_variables = ('x',)
+    _nvar = 1
+    cvar = numpy.array([0], dtype=numpy.int32)
 
-    dx[0] = omega + c_pop0
-    
+    def dfun(self, state, coupling, local_coupling=0.0):
+        """
+        .. math::
+            x = a{\gamma} + b
+        """
+        x, = state
+        c, = coupling
+        dx = self.gamma * x + c + local_coupling * x
+        return numpy.array([dx])
```

### Comparing `tvb-library-2.8/tvb/simulator/models/larter_breakspear.py` & `tvb-library-2.8.1/tvb/simulator/models/larter_breakspear.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/linear.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/temporal_correlations_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,67 +19,34 @@
 #
 #
 #   CITATION:
 # When using The Virtual Brain for scientific publications, please cite it as explained here:
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
-
 """
-Generic linear model.
+Created on Mar 20, 2013
+
+.. moduleauthor:: Bogdan Neacsa <bogdan.neacsa@codemart.ro>
 """
 
 import numpy
-from .base import Model
-from tvb.basic.neotraits.api import NArray, Final, List, Range
-
-
-class Linear(Model):
-    gamma = NArray(
-        label=r":math:`\gamma`",
-        default=numpy.array([-10.0]),
-        domain=Range(lo=-100.0, hi=0.0, step=1.0),
-        doc="The damping coefficient specifies how quickly the node's activity relaxes, must be larger"
-            " than the node's in-degree in order to remain stable.")
-
-    state_variable_range = Final(
-        label="State Variable ranges [lo, hi]",
-        default={"x": numpy.array([-1, 1])},
-        doc="Range used for state variable initialization and visualization.")
-
-    variables_of_interest = List(
-        of=str,
-        label="Variables watched by Monitors",
-        choices=("x",),
-        default=("x",), )
-
-    coupling_terms = Final(
-        label="Coupling terms",
-        # how to unpack coupling array
-        default=["c"]
-    )
-
-    state_variable_dfuns = Final(
-        label="Drift functions",
-        default={
-            "x": "gamma * x + c",
-        }
-    )
-
-    parameter_names = List(
-        of=str,
-        label="List of parameters for this model",
-        default=tuple('gamma'.split()))
+from tvb.tests.library.base_testcase import BaseTestCase
+from tvb.datatypes import temporal_correlations, time_series
 
-    state_variables = ('x',)
-    _nvar = 1
-    cvar = numpy.array([0], dtype=numpy.int32)
 
-    def dfun(self, state, coupling, local_coupling=0.0):
-        """
-        .. math::
-            x = a{\gamma} + b
-        """
-        x, = state
-        c, = coupling
-        dx = self.gamma * x + c + local_coupling * x
-        return numpy.array([dx])
+class TestTemporalCorrelations(BaseTestCase):
+    """
+    Tests the defaults for `tvb.datatypes.temporal_correlations` module.
+    """
+
+    def test_crosscorrelation(self):
+        data = numpy.random.random((10, 10))
+        ts = time_series.TimeSeries(data=data, title='meh')
+        dt = temporal_correlations.CrossCorrelation(source=ts, array_data=numpy.array([0]))
+        summary_info = dt.summary_info()
+        assert summary_info['Dimensions'] == ('Offsets', 'Node', 'Node', 'State Variable', 'Mode')
+        assert summary_info['Source'] == 'meh'
+        assert summary_info['Temporal correlation type'] == 'CrossCorrelation'
+        assert dt.labels_ordering == ('Offsets', 'Node', 'Node', 'State Variable', 'Mode')
+        assert dt.source is not None
+        assert dt.time is None
```

### Comparing `tvb-library-2.8/tvb/simulator/models/oscillator.py` & `tvb-library-2.8.1/tvb/simulator/models/oscillator.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/stefanescu_jirsa.py` & `tvb-library-2.8.1/tvb/simulator/models/stefanescu_jirsa.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/wilson_cowan.py` & `tvb-library-2.8.1/tvb/simulator/models/wilson_cowan.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/wong_wang.py` & `tvb-library-2.8.1/tvb/simulator/models/wong_wang.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/wong_wang_exc_inh.py` & `tvb-library-2.8.1/tvb/simulator/models/wong_wang_exc_inh.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/models/zerlaut.py` & `tvb-library-2.8.1/tvb/simulator/models/zerlaut.py`

 * *Files 7% similar despite different names*

```diff
@@ -182,21 +182,21 @@
     a_i = NArray(
         label=":math:`a_i`",
         default=numpy.array([0.0]),
         domain=Range(lo=0.0, hi=20.0, step=0.1),
         doc="""Inhibitory adaptation conductance [nS]""")
 
     tau_w_e = NArray(
-        label=":math:`tau_{we}`",
+        label=r":math:`\tau_{we}`",
         default=numpy.array([500.0]),
         domain=Range(lo=1.0, hi=1000.0, step=1.0),
         doc="""Adaptation time constant of excitatory neurons [ms]""")
 
     tau_w_i = NArray(
-        label=":math:`tau_{wi}`",
+        label=r":math:`\tau_{wi}`",
         default=numpy.array([1.0]),
         domain=Range(lo=1.0, hi=1000.0, step=1.0),
         doc="""Adaptation time constant of inhibitory neurons [ms]""")
 
     E_e = NArray(
         label=r":math:`E_e`",
         default=numpy.array([0.0]),
@@ -236,15 +236,21 @@
     N_tot = NArray(
         dtype=numpy.int64,
         label=":math:`N_{tot}`",
         default=numpy.array([10000]),
         domain=Range(lo=1000, hi=50000, step=1000),
         doc="""cell number""")
 
-    p_connect = NArray(
+    p_connect_e = NArray(
+        label=r":math:`\epsilon`",
+        default=numpy.array([0.05]),
+        domain=Range(lo=0.001, hi=0.2, step=0.001),  # valid only for relatively sparse connectivities
+        doc="""connectivity probability""")
+
+    p_connect_i = NArray(
         label=r":math:`\epsilon`",
         default=numpy.array([0.05]),
         domain=Range(lo=0.001, hi=0.2, step=0.001),  # valid only for relatively sparse connectivities
         doc="""connectivity probability""")
 
     g = NArray(
         label=":math:`g`",
@@ -309,21 +315,41 @@
 
     external_input_in_in = NArray(
         label=r":math:`\nu_e^{drive}`",
         default=numpy.array([0.000]),
         domain=Range(lo=0.00, hi=0.1, step=0.001),
         doc="""external drive""")
 
+    tau_OU = NArray(
+        label=r":math:`\tau` noise",
+        default=numpy.array([5.0]),
+        domain=Range(lo=0.10, hi=10.0, step=0.01),
+        doc="""time constant noise""")
+
+    weight_noise = NArray(
+        label="Weight noise",
+        default=numpy.array([10.5]),
+        domain=Range(lo=0., hi=50.0, step=1.0),
+        doc="""weight noise""")
+
+    S_i = NArray(
+        label="Scaling Inh",
+        default=numpy.array([1.]),
+        domain=Range(lo=0., hi=2., step=0.01),
+        doc="""Scaling of the remote input for the inhibitory population with
+        respect to the excitatory population.""")
+
     # Used for phase-plane axis ranges and to bound random initial() conditions.
     state_variable_range = Final(
         label="State Variable ranges [lo, hi]",
         default={"E": numpy.array([1e-3, 250.e-3]),  # actually the 100Hz should be replaced by 1/T_refrac
                  "I": numpy.array([1e-3, 250.e-3]),
                  "W_e": numpy.array([0.0, 200.0]),
                  "W_i": numpy.array([0.0, 0.0]),
+                 "ou_drift": numpy.array([0.0,0.0]),
                  },
         doc="""The values for each state-variable should be set to encompass
         the expected dynamic range of that state-variable for the current
         parameters, it is used as a mechanism for bounding random initial
         conditions when the simulation isn't started from an explicit history,
         it is also provides the default range of phase-plane plots.\n
         E: firing rate of excitatory population in KHz\n
@@ -331,54 +357,58 @@
         W_e: level of adaptation of excitatory in pA\n
         W_i: level of adaptation of inhibitory in pA\n
         """)
 
     variables_of_interest = List(
         of=str,
         label="Variables watched by Monitors",
-        choices=("E", "I", "W_e", "W_i"),
+        choices=("E", "I", "W_e", "W_i", "ou_drift"),
         default=("E",),
         doc="""This represents the default state-variables of this Model to be
                monitored. It can be overridden for each Monitor if desired. The
                corresponding state-variable indices for this model are :math:`E = 0`,
                :math:`I = 1` and :math:`W = 2`.""")
 
     state_variable_boundaries = Final(
         label="Firing rate of population is always positive",
         default={"E": numpy.array([0.0, None]),
                  "I": numpy.array([0.0, None])},
         doc="""The values for each state-variable should be set to encompass
             the boundaries of the dynamic range of that state-variable. Set None for one-sided boundaries""")
 
-    state_variables = 'E I W_e W_i'.split()
-    _nvar = 4
+    state_variables = 'E I W_e W_i ou_drift'.split()
+    _nvar = 5
     cvar = numpy.array([0], dtype=numpy.int32)
 
     def dfun(self, state_variables, coupling, local_coupling=0.00):
         r"""
         .. math::
             T \dot{\nu_\mu} &= -F_\mu(\nu_e,\nu_i) + \nu_\mu ,{\forall}\mu\in\{e,i\}\\
             \dot{W}_k &= W_k/tau_w-b*E_k  \\
 
         """
         E = state_variables[0, :]
         I = state_variables[1, :]
         W_e = state_variables[2, :]
         W_i = state_variables[3, :]
+        ou_drift = state_variables[4, :]
         derivative = numpy.empty_like(state_variables)
 
         # long-range coupling
         c_0 = coupling[0, :]
 
         # short-range (local) coupling
         lc_E = local_coupling * E
         lc_I = local_coupling * I
 
         # external firing rate
-        Fe_ext = c_0 + lc_E
+        Fe_ext = c_0 + lc_E + self.weight_noise * ou_drift
+        index_bad_input = numpy.where( Fe_ext*self.K_ext_e  < 0)
+        Fe_ext[index_bad_input] = 0.0
+
         Fi_ext = lc_I
 
         # Excitatory firing rate derivation
         derivative[0] = (self.TF_excitatory(
             E, I, Fe_ext + self.external_input_ex_ex,
                   Fi_ext + self.external_input_ex_in,
             W_e) - E) / self.T
@@ -389,26 +419,27 @@
             W_i) - I) / self.T
         # Adaptation excitatory
         mu_V, sigma_V, T_V = self.get_fluct_regime_vars(
             E, I, Fe_ext + self.external_input_ex_ex,
                   Fi_ext + self.external_input_ex_in,
             W_e, self.Q_e, self.tau_e, self.E_e,
             self.Q_i, self.tau_i, self.E_i,
-            self.g_L, self.C_m, self.E_L_e, self.N_tot,
-            self.p_connect, self.g, self.K_ext_e, self.K_ext_i)
+            self.g_L, self.C_m, self.E_L_e, self.N_tot,self.p_connect_e,
+            self.p_connect_i, self.g, self.K_ext_e, self.K_ext_i)
         derivative[2] = -W_e / self.tau_w_e + self.b_e * E + self.a_e * (mu_V - self.E_L_e) / self.tau_w_e
         # Adaptation inhibitory
         mu_V, sigma_V, T_V = self.get_fluct_regime_vars(
             E, I, Fe_ext + self.external_input_in_ex,
                   Fi_ext + self.external_input_in_in,
             W_i, self.Q_e, self.tau_e, self.E_e,
             self.Q_i, self.tau_i, self.E_i,
-            self.g_L, self.C_m, self.E_L_i, self.N_tot,
-            self.p_connect, self.g, self.K_ext_e, self.K_ext_i)
+            self.g_L, self.C_m, self.E_L_i, self.N_tot,self.p_connect_e,
+            self.p_connect_i, self.g, self.K_ext_e, self.K_ext_i)
         derivative[3] = -W_i / self.tau_w_i + self.b_i * I + self.a_i * (mu_V - self.E_L_i) / self.tau_w_i
+        derivative[4] = -ou_drift/self.tau_OU
 
         return derivative
 
     def TF_excitatory(self, fe, fi, fe_ext, fi_ext, W):
         """
         transfer function for excitatory population
         :param fe: firing rate of excitatory population
@@ -445,25 +476,25 @@
         :param P: Polynome of neurons phenomenological threshold (order 9)
         :param E_L: leak reversal potential
         :return: result of transfer function
         """
         mu_V, sigma_V, T_V = self.get_fluct_regime_vars(fe, fi, fe_ext, fi_ext, W, self.Q_e, self.tau_e, self.E_e,
                                                         self.Q_i, self.tau_i, self.E_i,
                                                         self.g_L, self.C_m, E_L, self.N_tot,
-                                                        self.p_connect, self.g, self.K_ext_e, self.K_ext_i)
+                                                        self.p_connect_e, self.p_connect_i, self.g, self.K_ext_e, self.K_ext_i)
         V_thre = self.threshold_func(mu_V, sigma_V, T_V * self.g_L / self.C_m,
                                      P[0], P[1], P[2], P[3], P[4], P[5], P[6], P[7], P[8], P[9])
         V_thre *= 1e3  # the threshold need to be in mv and not in Volt
         f_out = self.estimate_firing_rate(mu_V, sigma_V, T_V, V_thre)
         return f_out
 
     @staticmethod
     @jit(nopython=True, cache=True)
     def get_fluct_regime_vars(Fe, Fi, Fe_ext, Fi_ext, W, Q_e, tau_e, E_e, Q_i, tau_i, E_i, g_L, C_m, E_L, N_tot,
-                              p_connect, g, K_ext_e, K_ext_i):
+                              p_connect_e, p_connect_i, g, K_ext_e, K_ext_i):
         """
         Compute the mean characteristic of neurons.
         Inspired from the next repository :
         https://github.com/yzerlaut/notebook_papers/tree/master/modeling_mesoscopic_dynamics
         :param Fe: firing rate of excitatory population
         :param Fi: firing rate of inhibitory population
         :param Fe_ext: external excitatory input
@@ -476,22 +507,23 @@
         :param tau_i: inhibitory decay
         :param E_i: inhibitory reversal potential
         :param E_L: leakage reversal voltage of neurons
         :param g_L: leak conductance
         :param C_m: membrane capacitance
         :param E_L: leak reversal potential
         :param N_tot: cell number
-        :param p_connect: connectivity probability
+        :param p_connect_e: connectivity probability of excitatory neurons
+        :param p_connect_i: connectivity probability of inhibitory neurons
         :param g: fraction of inhibitory cells
         :return: mean and variance of membrane voltage of neurons and autocorrelation time constant
         """
         # firing rate
         # 1e-6 represent spontaneous release of synaptic neurotransmitter or some intrinsic currents of neurons
-        fe = (Fe + 1.0e-6) * (1. - g) * p_connect * N_tot + Fe_ext * K_ext_e
-        fi = (Fi + 1.0e-6) * g * p_connect * N_tot + Fi_ext * K_ext_i
+        fe = (Fe + 1.0e-6) * (1. - g) * p_connect_e * N_tot + Fe_ext * K_ext_e
+        fi = (Fi + 1.0e-6) * g * p_connect_i * N_tot + Fi_ext * K_ext_i
 
         # conductance fluctuation and effective membrane time constant
         mu_Ge, mu_Gi = Q_e * tau_e * fe, Q_i * tau_i * fi  # Eqns 5 from [MV_2018]
         mu_G = g_L + mu_Ge + mu_Gi  # Eqns 6 from [MV_2018]
         T_m = C_m / mu_G  # Eqns 6 from [MV_2018]
 
         # membrane potential
@@ -565,50 +597,65 @@
 
     .. automethod:: Zerlaut_adaptation_second_order.__init__
 
     The general formulation for the \textit{\textbf{Zerlaut_adaptation_second_order}} model as a
     dynamical unit at a node $k$ in a BNM with $l$ nodes reads:
 
     .. math::
+        \begin{aligned}
         \forall \mu,\lambda,\eta \in \{e,i\}^3\,
-        \left\{
-        \begin{split}
-        T \, \frac{\partial \nu_\mu}{\partial t} = & (\mathcal{F}_\mu - \nu_\mu )
-        + \frac{1}{2} \, c_{\lambda \eta} \,
+        &\left\{
+        \begin{aligned}
+        T \frac{\partial \nu_\mu}{\partial t} &= (\mathcal{F}_\mu - \nu_\mu )
+        + \frac{1}{2} c_{\lambda \eta} 
         \frac{\partial^2 \mathcal{F}_\mu}{\partial \nu_\lambda \partial \nu_\eta} \\
-        T \, \frac{\partial c_{\lambda \eta} }{\partial t}  =  & A_{\lambda \eta} +
-        (\mathcal{F}_\lambda - \nu_\lambda ) \, (\mathcal{F}_\eta - \nu_\eta ) + \\
-        & c_{\lambda \mu} \frac{\partial \mathcal{F}_\mu}{\partial \nu_\lambda} +
+        T \frac{\partial c_{\lambda \eta} }{\partial t}  &= A_{\lambda \eta} +
+        (\mathcal{F}_\lambda - \nu_\lambda ) (\mathcal{F}_\eta - \nu_\eta )  \\
+        &+ c_{\lambda \mu} \frac{\partial \mathcal{F}_\mu}{\partial \nu_\lambda} +
         c_{\mu \eta} \frac{\partial \mathcal{F}_\mu}{\partial \nu_\eta}
         - 2  c_{\lambda \eta}
-        \end{split}
-        \right.
-        dot{W}_k &= W_k/tau_w-b*E_k  \\
+        \end{aligned}\\
+        \right. \\
+        &\frac{\partial W_\mu}{\partial t} = \frac{W_\mu}{\tau_{w\mu}}-b_\mu*\nu_\mu +
+        \frac{a_\mu(\mu_V-E_{L_\mu})}{\tau_{w\mu}}\\
+        \end{aligned}
 
         with:
         A_{\lambda \eta} =
         \left\{
         \begin{split}
-        \frac{\mathcal{F}_\lambda \, (1/T - \mathcal{F}_\lambda)}{N_\lambda}
+        \frac{\mathcal{F}_\lambda (1/T - \mathcal{F}_\lambda)}{N_\lambda}
         \qquad & \textrm{if  } \lambda=\eta \\
         0 \qquad & \textrm{otherwise}
         \end{split}
         \right.
+
+        where:
+        \begin{split}
+        F_\lambda &= F_\lambda(\nu_e, \nu_i, \nu^{input\lambda}_e, \nu^{input\lambda}_i, W_\lambda)\\
+        \nu^{input,e}_e &= \nu_{connectome} + \nu_{surface} + \nu^{ext}_ee + w_{noise}OU\\
+        \nu^{input,e}_i &= S_i\nu_{connectome} + \nu_{surface} + \nu^{ext}_ei + w_{noise}OU\\
+        \nu^{input,i}_e &= \nu_{surface} + \nu^{ext}_ie\\
+        \nu^{input,i}_i &= \nu_{surface} + \nu^{ext}_ii\\
+        \end{split}
+
+        \textrm{given OU is the Ornstein-Uhlenbeck process}.
     """
 
     #  Used for phase-plane axis ranges and to bound random initial() conditions.
     state_variable_range = Final(
         label="State Variable ranges [lo, hi]",
         default={"E": numpy.array([1e-3, 250.e-3]),  # actually the 100Hz should be replaced by 1/T_refrac
                  "I": numpy.array([1e-3, 250.e-3]),
-                 "C_ee": numpy.array([0.5e-3, 0.0e-3]),  # variance is positive or null
-                 "C_ei": numpy.array([0.5e-3, -0.5e-3]),  # the co-variance is in [-c_ee*c_ii,c_ee*c_ii]
-                 "C_ii": numpy.array([0.5e-3, 0.0e-3]),  # variance is positive or null
+                 "C_ee": numpy.array([0.0e-3, 0.5e-3]),  # variance is positive or null
+                 "C_ei": numpy.array([-0.5e-3, 0.5e-3]),  # the co-variance is in [-c_ee*c_ii,c_ee*c_ii]
+                 "C_ii": numpy.array([0.0e-3, 0.5e-3]),  # variance is positive or null
                  "W_e": numpy.array([0.0, 200.0]),
                  "W_i": numpy.array([0.0, 0.0]),
+                 "ou_drift":numpy.array([0.0, 0.0]),
                  },
         doc="""The values for each state-variable should be set to encompass
         the expected dynamic range of that state-variable for the current
         parameters, it is used as a mechanism for bounding random inital
         conditions when the simulation isn't started from an explicit history,
         it is also provides the default range of phase-plane plots.\n
         E: firing rate of excitatory population in KHz\n
@@ -618,76 +665,96 @@
         C_ie: the variance of the inhibitory population activity \n
         W: level of adaptation
         """)
 
     variables_of_interest = List(
         of=str,
         label="Variables watched by Monitors",
-        choices=("E", "I", "C_ee", "C_ei", "C_ii", "W_e", "W_i"),
+        choices=("E", "I", "C_ee", "C_ei", "C_ii", "W_e", "W_i", "ou_drift"),
         default=("E",),
         doc="""This represents the default state-variables of this Model to be
                monitored. It can be overridden for each Monitor if desired. The
                corresponding state-variable indices for this model are :math:`E = 0`,
                :math:`I = 1`, :math:`C_ee = 2`, :math:`C_ei = 3`, :math:`C_ii = 4` and :math:`W = 5`.""")
 
-    state_variables = 'E I C_ee C_ei C_ii W_e W_i'.split()
-    _nvar = 7
+    state_variables = 'E I C_ee C_ei C_ii W_e W_i ou_drift'.split()
+    _nvar = 8
 
     def dfun(self, state_variables, coupling, local_coupling=0.00):
         r"""
         .. math::
+            \begin{aligned}
             \forall \mu,\lambda,\eta \in \{e,i\}^3\,
-            \left\{
-            \begin{split}
-            T \, \frac{\partial \nu_\mu}{\partial t} = & (\mathcal{F}_\mu - \nu_\mu )
-            + \frac{1}{2} \, c_{\lambda \eta} \,
+            &\left\{
+            \begin{aligned}
+            T \frac{\partial \nu_\mu}{\partial t} &= (\mathcal{F}_\mu - \nu_\mu )
+            + \frac{1}{2} c_{\lambda \eta} 
             \frac{\partial^2 \mathcal{F}_\mu}{\partial \nu_\lambda \partial \nu_\eta} \\
-            T \, \frac{\partial c_{\lambda \eta} }{\partial t}  =  & A_{\lambda \eta} +
-            (\mathcal{F}_\lambda - \nu_\lambda ) \, (\mathcal{F}_\eta - \nu_\eta ) + \\
-            & c_{\lambda \mu} \frac{\partial \mathcal{F}_\mu}{\partial \nu_\lambda} +
+            T \frac{\partial c_{\lambda \eta} }{\partial t}  &= A_{\lambda \eta} +
+            (\mathcal{F}_\lambda - \nu_\lambda ) (\mathcal{F}_\eta - \nu_\eta )  \\
+            &+ c_{\lambda \mu} \frac{\partial \mathcal{F}_\mu}{\partial \nu_\lambda} +
             c_{\mu \eta} \frac{\partial \mathcal{F}_\mu}{\partial \nu_\eta}
             - 2  c_{\lambda \eta}
-            \end{split}
-            \right.
-            dot{W}_k &= W_k/tau_w-b*E_k  \\
+            \end{aligned}\\
+            \right. \\
+            &\frac{\partial W_\mu}{\partial t} = \frac{W_\mu}{\tau_{w\mu}}-b_\mu*\nu_\mu +
+            \frac{a_\mu(\mu_V-E_{L_\mu})}{\tau_{w\mu}}\\
+            \end{aligned}
 
             with:
             A_{\lambda \eta} =
             \left\{
             \begin{split}
-            \frac{\mathcal{F}_\lambda \, (1/T - \mathcal{F}_\lambda)}{N_\lambda}
+            \frac{\mathcal{F}_\lambda (1/T - \mathcal{F}_\lambda)}{N_\lambda}
             \qquad & \textrm{if  } \lambda=\eta \\
             0 \qquad & \textrm{otherwise}
             \end{split}
             \right.
 
+            where:
+            \begin{split}
+            F_\lambda &= F_\lambda(\nu_e, \nu_i, \nu^{input\lambda}_e, \nu^{input\lambda}_i, W_\lambda)\\
+            \nu^{input,e}_e &= \nu_{connectome} + \nu_{surface} + \nu^{ext}_ee + w_{noise}OU\\
+            \nu^{input,e}_i &= S_i\nu_{connectome} + \nu_{surface} + \nu^{ext}_ei + w_{noise}OU\\
+            \nu^{input,i}_e &= \nu_{surface} + \nu^{ext}_ie\\
+            \nu^{input,i}_i &= \nu_{surface} + \nu^{ext}_ii\\
+            \end{split}
+
+            \textrm{given OU is the Ornstein-Uhlenbeck process}.
         """
         # number of neurons
         N_e = self.N_tot * (1 - self.g)
         N_i = self.N_tot * self.g
         # state variable
         E = state_variables[0, :]
         I = state_variables[1, :]
         C_ee = state_variables[2, :]
         C_ei = state_variables[3, :]
         C_ii = state_variables[4, :]
         W_e = state_variables[5, :]
         W_i = state_variables[6, :]
+        ou_drift = state_variables[7,:]
         derivative = numpy.empty_like(state_variables)
 
         # long-range coupling
         c_0 = coupling[0, :]
 
         # short-range (local) coupling
         lc_E = local_coupling * E
         lc_I = local_coupling * I
 
         # external firing rate for the different population
-        E_input_excitatory = c_0 + lc_E + self.external_input_ex_ex
-        E_input_inhibitory = c_0 + lc_E + self.external_input_in_ex
+        E_input_excitatory = c_0 + lc_E + self.external_input_ex_ex + self.weight_noise * ou_drift
+        index_bad_input = numpy.where( E_input_excitatory < 0)
+        E_input_excitatory[index_bad_input] = 0.0
+
+        E_input_inhibitory = self.S_i * c_0 + lc_E + self.external_input_in_ex + self.weight_noise * ou_drift
+        index_bad_input = numpy.where( E_input_inhibitory < 0)
+        E_input_inhibitory[index_bad_input] = 0.0
+
         I_input_excitatory = lc_I + self.external_input_ex_in
         I_input_inhibitory = lc_I + self.external_input_in_in
 
         # Transfer function of excitatory and inhibitory neurons
         _TF_e = self.TF_excitatory(E, I, E_input_excitatory, I_input_excitatory, W_e)
         _TF_i = self.TF_inhibitory(E, I, E_input_inhibitory, I_input_inhibitory, W_i)
 
@@ -733,68 +800,65 @@
         _diff_fi_TF_i = _diff_fi(self.TF_inhibitory, E, I, E_input_inhibitory, I_input_inhibitory, W_i)
 
         # equation is inspired from github of Zerlaut :
         # https://github.com/yzerlaut/notebook_papers/blob/master/modeling_mesoscopic_dynamics/mean_field/master_equation.py
         # Excitatory firing rate derivation
         derivative[0] = (_TF_e - E
                          + .5 * C_ee * _diff2_fe_fe_e(E, I, E_input_excitatory, I_input_excitatory, W_e)
-                         + .5 * C_ei * _diff2_fe_fi(self.TF_excitatory, E, I, E_input_excitatory, I_input_excitatory,
-                                                    W_e)
-                         + .5 * C_ei * _diff2_fi_fe(self.TF_excitatory, E, I, E_input_excitatory, I_input_excitatory,
-                                                    W_e)
+                         + .5 * C_ei * _diff2_fe_fi(self.TF_excitatory, E, I, E_input_excitatory, I_input_excitatory, W_e)
+                         + .5 * C_ei * _diff2_fi_fe(self.TF_excitatory, E, I, E_input_excitatory, I_input_excitatory, W_e)
                          + .5 * C_ii * _diff2_fi_fi_e(E, I, E_input_excitatory, I_input_excitatory, W_e)
                          ) / self.T
         # Inhibitory firing rate derivation
         derivative[1] = (_TF_i - I
                          + .5 * C_ee * _diff2_fe_fe_i(E, I, E_input_inhibitory, I_input_inhibitory, W_i)
-                         + .5 * C_ei * _diff2_fe_fi(self.TF_inhibitory, E, I, E_input_inhibitory, I_input_inhibitory,
-                                                    W_i)
-                         + .5 * C_ei * _diff2_fi_fe(self.TF_inhibitory, E, I, E_input_inhibitory, I_input_inhibitory,
-                                                    W_i)
+                         + .5 * C_ei * _diff2_fe_fi(self.TF_inhibitory, E, I, E_input_inhibitory, I_input_inhibitory, W_i)
+                         + .5 * C_ei * _diff2_fi_fe(self.TF_inhibitory, E, I, E_input_inhibitory, I_input_inhibitory, W_i)
                          + .5 * C_ii * _diff2_fi_fi_i(E, I, E_input_inhibitory, I_input_inhibitory, W_i)
                          ) / self.T
         # Covariance excitatory-excitatory derivation
         derivative[2] = (_TF_e * (1. / self.T - _TF_e) / N_e
                          + (_TF_e - E) ** 2
                          + 2. * C_ee * _diff_fe_TF_e
-                         + 2. * C_ei * _diff_fi_TF_i
+                         + 2. * C_ei * _diff_fi_TF_e
                          - 2. * C_ee
                          ) / self.T
         # Covariance excitatory-inhibitory or inhibitory-excitatory derivation
         derivative[3] = ((_TF_e - E) * (_TF_i - I)
                          + C_ee * _diff_fe_TF_e
                          + C_ei * _diff_fe_TF_i
                          + C_ei * _diff_fi_TF_e
                          + C_ii * _diff_fi_TF_i
                          - 2. * C_ei
                          ) / self.T
         # Covariance inhibitory-inhibitory derivation
         derivative[4] = (_TF_i * (1. / self.T - _TF_i) / N_i
                          + (_TF_i - I) ** 2
                          + 2. * C_ii * _diff_fi_TF_i
-                         + 2. * C_ei * _diff_fe_TF_e
+                         + 2. * C_ei * _diff_fe_TF_i
                          - 2. * C_ii
                          ) / self.T
 
         # Adaptation excitatory
         mu_V, sigma_V, T_V = self.get_fluct_regime_vars(
             E, I,
             E_input_excitatory,
-            E_input_inhibitory,
+            I_input_excitatory,
             W_e, self.Q_e, self.tau_e, self.E_e,
             self.Q_i, self.tau_i, self.E_i,
             self.g_L, self.C_m, self.E_L_e, self.N_tot,
-            self.p_connect, self.g, self.K_ext_e, self.K_ext_i)
+            self.p_connect_e, self.p_connect_i, self.g, self.K_ext_e, self.K_ext_i)
         derivative[5] = -W_e / self.tau_w_e + self.b_e * E + self.a_e * (mu_V - self.E_L_e) / self.tau_w_e
 
         # Adaptation inhibitory
         mu_V, sigma_V, T_V = self.get_fluct_regime_vars(
             E, I,
-            I_input_excitatory,
+            E_input_inhibitory,
             I_input_inhibitory,
             W_i, self.Q_e, self.tau_e, self.E_e,
             self.Q_i, self.tau_i, self.E_i,
             self.g_L, self.C_m, self.E_L_i, self.N_tot,
-            self.p_connect, self.g, self.K_ext_e, self.K_ext_i)
+            self.p_connect_e, self.p_connect_i, self.g, self.K_ext_e, self.K_ext_i)
         derivative[6] = -W_i / self.tau_w_i + self.b_i * I + self.a_i * (mu_V - self.E_L_i) / self.tau_w_i
 
+        derivative[7] = -ou_drift/self.tau_OU
         return derivative
```

### Comparing `tvb-library-2.8/tvb/simulator/monitors.py` & `tvb-library-2.8.1/tvb/simulator/monitors.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         by transforming them all to 0.
         Otherwise, the later check not numpy.all(areas == numpy.arange(number_of_areas)) would fail for all regions
         being cortical or in one hemisphere.
         """
         spatial_mask = numpy.array([int(val) for val in mask])
         unique_mask = numpy.unique(spatial_mask)
         if len(unique_mask) == 1 and unique_mask[0] == 1:
-            return numpy.zeros(len(spatial_mask), dtype=numpy.int)
+            return numpy.zeros(len(spatial_mask), dtype=numpy.int_)
         return spatial_mask
 
     def config_for_sim(self, simulator):
 
         # initialize base attributes
         super(SpatialAverage, self).config_for_sim(simulator)
         self.is_default_special_mask = False
@@ -482,15 +482,15 @@
         "Construct analytic or default set of spatial filters for simulation."
         # this will not be implemented but kept for API uniformity
         raise NotImplementedError(
             "No general purpose analytic formula available for spatial "
             "projection matrices. Please select an appropriate projection "
             "matrix."
         )
-    
+
     _gain_configuration_done = False
 
     def config_for_sim(self, simulator):
         "Configure projection matrix monitor for given simulation."
 
         # method body is not idempotent, so if we've been here before, don't redo
         if self._gain_configuration_done:
@@ -548,19 +548,19 @@
             self.log.debug('Precomputed projection not unavailable, using analytic approximation.')
             self.gain = self.analytic(**sources)
 
         # reduce to region lead field if region sim
         # this fails when rmap doesn't have non_cortical, need to ensure "full" first
         # OR fix non_cortical_rmap_idx to be empty in that case:
         cortical_rmap = self.rmap.copy()
-        if (self.rmap.max()+1) == conn.cortical.sum():
+        if (self.rmap.max() + 1) == conn.cortical.sum():
             # there are no non_cortical indices in rmap, so cortical_rmap is already fine
             pass
         else:
-            non_cortical_rmap_idx = numpy.hstack([numpy.argwhere(self.rmap==i)[:,0] for i in non_cortical_indices])
+            non_cortical_rmap_idx = numpy.hstack([numpy.argwhere(self.rmap == i)[:, 0] for i in non_cortical_indices])
             cortical_rmap = numpy.delete(cortical_rmap, non_cortical_rmap_idx)
         if not using_cortical_surface and self.gain.shape[1] == cortical_rmap.size:
             gain = numpy.zeros((self.gain.shape[0], conn.number_of_regions))
             numpy_add_at(gain.T, cortical_rmap, self.gain.T)
             self.log.debug('Region mapping gain shape %s to %s', self.gain.shape, gain.shape)
             self.gain = gain
```

### Comparing `tvb-library-2.8/tvb/simulator/noise.py` & `tvb-library-2.8.1/tvb/simulator/noise.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/base_plotter.py` & `tvb-library-2.8.1/tvb/simulator/plot/base_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/colourmaps/BlackToBlue` & `tvb-library-2.8.1/tvb/simulator/plot/colourmaps/BlackToBlue`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/compare_integrators.py` & `tvb-library-2.8.1/tvb/simulator/plot/compare_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/config.py` & `tvb-library-2.8.1/tvb/simulator/plot/config.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/epileptor_plotter.py` & `tvb-library-2.8.1/tvb/simulator/plot/epileptor_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/head_plotter.py` & `tvb-library-2.8.1/tvb/simulator/plot/head_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/head_plotter_3d.py` & `tvb-library-2.8.1/tvb/simulator/plot/head_plotter_3d.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/phase_plane_interactive.py` & `tvb-library-2.8.1/tvb/simulator/plot/phase_plane_interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 # TODO: Add connectivity term to parameters...
 # TODO: Memory grows with usage, may be just a lazy garbage collector but, should
 #      check for leaks or look into "forcing" cleanup...
 
 import numpy
 import matplotlib.pyplot as plt
 import colorsys
+import numbers
 import matplotlib.widgets as widgets
 from deprecated import deprecated
 from tvb.simulator.common import get_logger
 import tvb.simulator.models as models_module
 import tvb.simulator.integrators as integrators_module
 from tvb.basic.neotraits.api import HasTraits, Attr, NArray, List
 
@@ -370,15 +371,15 @@
         offset = 0.0
         self.param_sliders = dict()
         # import pdb; pdb.set_trace()
         for param_name in type(self.model).declarative_attrs:
             if self.exclude_sliders is not None and param_name in self.exclude_sliders:
                 continue
             param_def = getattr(type(self.model), param_name)
-            if not isinstance(param_def, NArray) or not param_def.dtype == numpy.float:
+            if not isinstance(param_def, NArray) or not issubclass(param_def.dtype.type, numbers.Real):
                 continue
             param_range = param_def.domain
             if param_range is None:
                 continue
             offset += 0.035
             sax = self.ipp_fig.add_axes([0.825, 0.865 - offset, 0.125, 0.025],
                                         facecolor=AXCOLOUR)
```

### Comparing `tvb-library-2.8/tvb/simulator/plot/plotter.py` & `tvb-library-2.8.1/tvb/simulator/plot/plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/power_spectra_interactive.py` & `tvb-library-2.8.1/tvb/simulator/plot/power_spectra_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/time_series_plotter.py` & `tvb-library-2.8.1/tvb/simulator/plot/time_series_plotter.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/timeseries_interactive.py` & `tvb-library-2.8.1/tvb/simulator/plot/timeseries_interactive.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/plot/tools.py` & `tvb-library-2.8.1/tvb/simulator/plot/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,16 +603,16 @@
         kern_nx = numpy.round(kern_nx / dx)
         kern_ny = numpy.round(kern_ny / dy)
 
     # Determine the bandwidth to use for the gaussian kernel
     inv_cov = numpy.linalg.inv(cov * scotts_factor ** 2)
 
     # x & y (pixel) coords of the kernel grid, with <x,y> = <0,0> in center
-    xx = numpy.arange(kern_nx, dtype=numpy.float) - kern_nx / 2.0
-    yy = numpy.arange(kern_ny, dtype=numpy.float) - kern_ny / 2.0
+    xx = numpy.arange(kern_nx, dtype=numpy.float64) - kern_nx / 2.0
+    yy = numpy.arange(kern_ny, dtype=numpy.float64) - kern_ny / 2.0
     xx, yy = numpy.meshgrid(xx, yy)
 
     # Then evaluate the gaussian function on the kernel grid
     kernel = numpy.vstack((xx.flatten(), yy.flatten()))
     kernel = numpy.dot(inv_cov, kernel) * kernel
     kernel = numpy.sum(kernel, axis=0) / 2.0
     kernel = numpy.exp(-kernel)
```

### Comparing `tvb-library-2.8/tvb/simulator/plot/utils.py` & `tvb-library-2.8.1/tvb/simulator/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/simulator/simulator.py` & `tvb-library-2.8.1/tvb/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/__init__.py` & `tvb-library-2.8.1/tvb/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/bench.py` & `tvb-library-2.8.1/tvb/tests/bench.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/bench_against_mpr_backend.py` & `tvb-library-2.8.1/tvb/tests/bench_against_mpr_backend.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/__init__.py` & `tvb-library-2.8.1/tvb/tests/library/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/base_testcase.py` & `tvb-library-2.8.1/tvb/tests/library/base_testcase.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/basic/neotraits/_attr_test.py` & `tvb-library-2.8.1/tvb/tests/library/basic/neotraits/_attr_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/basic/neotraits/neotraits_test.py` & `tvb-library-2.8.1/tvb/tests/library/basic/neotraits/neotraits_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,28 @@
 #   CITATION:
 # When using The Virtual Brain for scientific publications, please cite it as explained here:
 # https://www.thevirtualbrain.org/tvb/zwei/neuroscience-publications
 #
 #
 
 import abc
-import copy
 import types
 import uuid
 import numpy
 import numpy as np
 import pytest
 from tvb.datatypes import connectivity
 from tvb.simulator import (simulator, models, coupling, integrators, monitors, noise)
 from tvb.basic.neotraits._core import TraitProperty
 from tvb.basic.neotraits.api import (
-    HasTraits, Attr, NArray, Final, List, trait_property,
+    HasTraits, Attr, NArray, Final, List, trait_property, narray_summary_info, narray_describe,
     Int, Float, Range, cached_trait_property, LinspaceRange, Dim
 )
 from tvb.basic.neotraits.ex import TraitTypeError, TraitValueError, TraitAttributeError, TraitError
 
-from tvb.basic.neotraits.info import narray_summary_info
-
 
 def test_simple_declaration():
     class A(HasTraits):
         fi = Attr(int)
 
 
 def test_simple_instantiation():
@@ -762,15 +759,15 @@
 
 def test_summary_info():
     class Z(HasTraits):
         zu = Attr(int)
 
     class A(HasTraits):
         a = Attr(str, default='ana')
-        b = NArray(dtype=int)
+        b = NArray(dtype=np.int64)
         ref = Attr(field_type=Z)
 
     ainst = A(b=np.arange(3))
     ainst.title = 'the red rose'
     ainst.gid = uuid.UUID(int=0)
     zinst = Z(zu=2)
     zinst.title = 'Z zuzu'
@@ -813,24 +810,37 @@
     assert summary['shape'] == "(3,)"
 
 
 def test_narray_summary_info_condensed_form():
     arr = np.arange(3)
     summary = narray_summary_info(arr, ar_name='attribute_name', condensed=True)
 
-    assert summary['attribute_name'] == ' [min, median, max] = [0, 1, 2] dtype = int64 shape = (3,)'
+    assert '[min, median, max] = [0, 1, 2]' in summary['attribute_name']
+    assert 'dtype = int' in summary['attribute_name']
+    assert 'shape = (3,)' in summary['attribute_name']
 
 
 def test_narray_summary_info_condensed_form_single_item():
     arr = np.array([4])
     summary = narray_summary_info(arr, ar_name='attribute_name', condensed=True)
 
     assert summary['attribute_name'] == '4'
 
 
+def test_narray_summary_info_with_nan():
+    arr = np.array([1, 2, np.inf, np.nan])
+    summary = narray_summary_info(arr)
+
+    assert summary['has NaN'] == 'True'
+    assert summary['shape'] == "(4,)"
+
+    desc = narray_describe(arr)
+    assert desc is not None
+
+
 def test_hastraits_str_does_not_crash():
     class A(HasTraits):
         a = Attr(str, default='ana')
         b = NArray(dtype=int)
         pom = 'prun'
 
         @trait_property(Attr(int))
@@ -970,14 +980,15 @@
     o_random_stream = original.integrator.noise.random_stream
     c_random_stream = clone.integrator.noise.random_stream
 
     # check that attr are not the same
     assert original.integrator.noise != clone.integrator.noise
     assert original.integrator.noise != integrators.IntegratorStochastic.noise.default
     assert original.model != clone.model
+    assert original.monitors[0] != clone.monitors[0]
     assert original.coupling != clone.coupling
     assert original.connectivity != clone.connectivity
     # even in the case of random generators
     assert o_random_stream is not c_random_stream
 
     # but values of attr are the same
     assert original.integrator.noise.ntau == clone.integrator.noise.ntau == 0
```

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/Edited_Connectivity.h5` & `tvb-library-2.8.1/tvb/tests/library/datatypes/Edited_Connectivity.h5`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/connectivity_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/connectivity_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/equations_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/equations_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/graph_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/graph_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/mode_decompositions_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/mode_decompositions_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/patterns_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/patterns_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/projections_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/projections_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/sensors_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/sensors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/spectral_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/spectral_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/surfaces_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/surfaces_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/timeseries_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/timeseries_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/datatypes/volumes_test.py` & `tvb-library-2.8.1/tvb/tests/library/datatypes/volumes_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/_numba_tests.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/_numba_tests.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/_opencl_tests.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/_opencl_tests.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/backend/backendtestbase.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/backend/backendtestbase.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/backend/cubackend_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/backend/cubackend_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/backend/nbbackend_mpr_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/backend/nbbackend_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/backend/nbbackend_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/backend/nbmprperf_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/backend/nbmprperf_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/backend/npbackend_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/backend/npbackend_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/common_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/common_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/coupling_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/coupling_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/descriptors_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/descriptors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/history_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/history_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/integrators_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/integrators_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/modelir_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/modelir_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/models_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/models_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/monitors_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/monitors_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/noise_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/noise_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/rateml_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/rateml_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/regionmapping_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/regionmapping_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/rngperf_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/rngperf_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/simulator_step_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/simulator_step_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/simulator_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/simulator_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/library/simulator/stimulation_test.py` & `tvb-library-2.8.1/tvb/tests/library/simulator/stimulation_test.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb/tests/validate_model_parameters.py` & `tvb-library-2.8.1/tvb/tests/validate_model_parameters.py`

 * *Files identical despite different names*

### Comparing `tvb-library-2.8/tvb_library.egg-info/PKG-INFO` & `tvb-library-2.8.1/tvb_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tvb-library
-Version: 2.8
+Version: 2.8.1
 Summary: A package for performing whole brain simulations
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
-Author: Marmaduke Woodman, Stuart Knock, Paula Sanz Leon, Viktor Jirsa
+Author: Marmaduke Woodman,  Jan Fousek, Stuart Knock, Paula Sanz Leon, Viktor Jirsa
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain simulator neuroscience human animal neuronal dynamics models delay
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `tvb-library-2.8/tvb_library.egg-info/SOURCES.txt` & `tvb-library-2.8.1/tvb_library.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -144,33 +144,28 @@
 tvb/simulator/backend/templates/np-integrate.py.mako
 tvb/simulator/backend/templates/np-sim.py.mako
 tvb/simulator/backend/templates/generated/.gitignore
 tvb/simulator/backend/templates/generated/__init__.py
 tvb/simulator/models/__init__.py
 tvb/simulator/models/base.py
 tvb/simulator/models/epileptor.py
-tvb/simulator/models/epileptorT.py
 tvb/simulator/models/epileptor_rs.py
 tvb/simulator/models/epileptorcodim3.py
 tvb/simulator/models/hopfield.py
 tvb/simulator/models/infinite_theta.py
 tvb/simulator/models/jansen_rit.py
-tvb/simulator/models/kuramotoT.py
+tvb/simulator/models/k_ion_exchange.py
 tvb/simulator/models/larter_breakspear.py
 tvb/simulator/models/linear.py
 tvb/simulator/models/oscillator.py
 tvb/simulator/models/stefanescu_jirsa.py
 tvb/simulator/models/wilson_cowan.py
 tvb/simulator/models/wong_wang.py
 tvb/simulator/models/wong_wang_exc_inh.py
 tvb/simulator/models/zerlaut.py
-tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.get_fluct_regime_vars-459.py310.1.nbc
-tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.get_fluct_regime_vars-459.py310.nbi
-tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.threshold_func-513.py310.1.nbc
-tvb/simulator/models/__pycache__/zerlaut.ZerlautAdaptationFirstOrder.threshold_func-513.py310.nbi
 tvb/simulator/plot/__init__.py
 tvb/simulator/plot/base_plotter.py
 tvb/simulator/plot/compare_integrators.py
 tvb/simulator/plot/config.py
 tvb/simulator/plot/epileptor_plotter.py
 tvb/simulator/plot/head_plotter.py
 tvb/simulator/plot/head_plotter_3d.py
```

