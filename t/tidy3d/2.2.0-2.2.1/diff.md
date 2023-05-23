# Comparing `tmp/tidy3d-2.2.0.tar.gz` & `tmp/tidy3d-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.2.0.tar", last modified: Mon May 22 17:05:06 2023, max compression
+gzip compressed data, was "tidy3d-2.2.1.tar", last modified: Tue May 23 18:01:04 2023, max compression
```

## Comparing `tidy3d-2.2.0.tar` & `tidy3d-2.2.1.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.777744 tidy3d-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-22 17:04:49.000000 tidy3d-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-22 17:04:49.000000 tidy3d-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-22 17:05:06.777744 tidy3d-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-22 17:04:49.000000 tidy3d-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-22 17:04:49.000000 tidy3d-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.757744 tidy3d-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:05:06.777744 tidy3d-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 17:04:49.000000 tidy3d-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.757744 tidy3d-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.761744 tidy3d-2.2.0/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.761744 tidy3d-2.2.0/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    53136 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.761744 tidy3d-2.2.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40386 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146570 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    68574 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   117741 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.777744 tidy3d-2.2.0/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.777744 tidy3d-2.2.0/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.632015 tidy3d-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-23 18:00:43.000000 tidy3d-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-23 18:00:43.000000 tidy3d-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 18:01:04.632015 tidy3d-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-23 18:00:43.000000 tidy3d-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 18:00:43.000000 tidy3d-2.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.600015 tidy3d-2.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:01:04.636015 tidy3d-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-23 18:00:43.000000 tidy3d-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.600015 tidy3d-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.604015 tidy3d-2.2.1/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.608015 tidy3d-2.2.1/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53136 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.608015 tidy3d-2.2.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.608015 tidy3d-2.2.1/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.612015 tidy3d-2.2.1/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40386 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.612015 tidy3d-2.2.1/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.612015 tidy3d-2.2.1/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146570 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68574 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117741 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.624015 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.624015 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.624015 tidy3d-2.2.1/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.632015 tidy3d-2.2.1/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.632015 tidy3d-2.2.1/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.616015 tidy3d-2.2.1/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.2.0/LICENSE` & `tidy3d-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/PKG-INFO` & `tidy3d-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.2.0
+Version: 2.2.1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.2.0/README.md` & `tidy3d-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/setup.py` & `tidy3d-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.2.1/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/_test_local/_test_data_performance.py` & `tidy3d-2.2.1/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/_test_local/_test_fit_web.py` & `tidy3d-2.2.1/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.2.1/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/_test_local/_test_web.py` & `tidy3d-2.2.1/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_IO.py` & `tidy3d-2.2.1/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_apodization.py` & `tidy3d-2.2.1/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_base.py` & `tidy3d-2.2.1/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_boundaries.py` & `tidy3d-2.2.1/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_custom.py` & `tidy3d-2.2.1/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_field_projection.py` & `tidy3d-2.2.1/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_geometry.py` & `tidy3d-2.2.1/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_grid.py` & `tidy3d-2.2.1/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_grid_spec.py` & `tidy3d-2.2.1/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_medium.py` & `tidy3d-2.2.1/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_meshgenerate.py` & `tidy3d-2.2.1/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_mode.py` & `tidy3d-2.2.1/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_monitor.py` & `tidy3d-2.2.1/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_sidewall.py` & `tidy3d-2.2.1/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_simulation.py` & `tidy3d-2.2.1/tests/test_components/test_simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_source.py` & `tidy3d-2.2.1/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_components/test_types.py` & `tidy3d-2.2.1/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_data/test_data_arrays.py` & `tidy3d-2.2.1/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_data/test_monitor_data.py` & `tidy3d-2.2.1/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_data/test_sim_data.py` & `tidy3d-2.2.1/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_package/test_config.py` & `tidy3d-2.2.1/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_package/test_log.py` & `tidy3d-2.2.1/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_package/test_make_script.py` & `tidy3d-2.2.1/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_package/test_material_library.py` & `tidy3d-2.2.1/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_package/test_parametric_variants.py` & `tidy3d-2.2.1/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_adjoint.py` & `tidy3d-2.2.1/tests/test_plugins/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.2.1/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.2.1/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.2.1/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_polyslab.py` & `tidy3d-2.2.1/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.2.1/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_plugins/test_waveguide.py` & `tidy3d-2.2.1/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_auth.py` & `tidy3d-2.2.1/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_cli.py` & `tidy3d-2.2.1/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_material_fitter.py` & `tidy3d-2.2.1/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.2.1/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.2.1/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.2.1/tests/test_web/test_tidy3d_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/test_web/test_webapi.py` & `tidy3d-2.2.1/tests/test_web/test_webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tests/utils.py` & `tidy3d-2.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/__init__.py` & `tidy3d-2.2.1/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/__main__.py` & `tidy3d-2.2.1/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/apodization.py` & `tidy3d-2.2.1/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/base.py` & `tidy3d-2.2.1/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/boundary.py` & `tidy3d-2.2.1/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/data/data_array.py` & `tidy3d-2.2.1/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/data/dataset.py` & `tidy3d-2.2.1/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/data/monitor_data.py` & `tidy3d-2.2.1/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/data/sim_data.py` & `tidy3d-2.2.1/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/field_projection.py` & `tidy3d-2.2.1/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/geometry.py` & `tidy3d-2.2.1/tidy3d/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/grid/grid.py` & `tidy3d-2.2.1/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.2.1/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/grid/mesher.py` & `tidy3d-2.2.1/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/medium.py` & `tidy3d-2.2.1/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/mode.py` & `tidy3d-2.2.1/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/monitor.py` & `tidy3d-2.2.1/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/simulation.py` & `tidy3d-2.2.1/tidy3d/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/source.py` & `tidy3d-2.2.1/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/structure.py` & `tidy3d-2.2.1/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/transformation.py` & `tidy3d-2.2.1/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/types.py` & `tidy3d-2.2.1/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/validators.py` & `tidy3d-2.2.1/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/components/viz.py` & `tidy3d-2.2.1/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/config.py` & `tidy3d-2.2.1/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/constants.py` & `tidy3d-2.2.1/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/exceptions.py` & `tidy3d-2.2.1/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/log.py` & `tidy3d-2.2.1/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/material_library/material_library.py` & `tidy3d-2.2.1/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/material_library/material_reference.py` & `tidy3d-2.2.1/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.2.1/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.2.1/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.2.1/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.2.1/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.2.1/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.2.1/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/mode/solver.py` & `tidy3d-2.2.1/tidy3d/plugins/mode/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,15 @@
         mu_zz = mu[2, 2, :]
         dxf, dxb, dyf, dyb = der_mats
 
         def any_pec(eps_vec, threshold=0.9 * np.abs(pec_val)):
             """Check if there are any PEC values in the given permittivity array."""
             return np.any(np.abs(eps_vec) >= threshold)
 
-        if np.any(any_pec(i) for i in [eps_xx, eps_yy, eps_zz]):
+        if any(any_pec(i) for i in [eps_xx, eps_yy, eps_zz]):
             enable_preconditioner = True
 
         # Compute the matrix for diagonalization
         inv_eps_zz = sp.spdiags(1 / eps_zz, [0], N, N)
         inv_mu_zz = sp.spdiags(1 / mu_zz, [0], N, N)
 
         if enable_incidence_matrices:
```

### Comparing `tidy3d-2.2.0/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.2.1/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.2.1/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.2.1/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.2.1/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.2.1/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/updater.py` & `tidy3d-2.2.1/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/__init__.py` & `tidy3d-2.2.1/tidy3d/web/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/asynchronous.py` & `tidy3d-2.2.1/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/auth.py` & `tidy3d-2.2.1/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/cacert.pem` & `tidy3d-2.2.1/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/cli/app.py` & `tidy3d-2.2.1/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/cli/migrate.py` & `tidy3d-2.2.1/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/config.py` & `tidy3d-2.2.1/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/container.py` & `tidy3d-2.2.1/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/environment.py` & `tidy3d-2.2.1/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/http_management.py` & `tidy3d-2.2.1/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/httputils.py` & `tidy3d-2.2.1/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/material_fitter.py` & `tidy3d-2.2.1/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/material_libray.py` & `tidy3d-2.2.1/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/s3utils.py` & `tidy3d-2.2.1/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/simulation_task.py` & `tidy3d-2.2.1/tidy3d/web/simulation_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/task.py` & `tidy3d-2.2.1/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/types.py` & `tidy3d-2.2.1/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d/web/webapi.py` & `tidy3d-2.2.1/tidy3d/web/webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.2.1/tidy3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.2.0
+Version: 2.2.1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.2.0/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.2.1/tidy3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.0/tidy3d.egg-info/requires.txt` & `tidy3d-2.2.1/tidy3d.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 toml
 boto3==1.23.1
 requests
 pyjwt
 click==8.0.3
 responses
 
+[:python_version <= "3.9"]
+typing-extensions<=4.5.0
+
 [dev]
 pre-commit
 black==22.3.0
 pylint
 tox
 pytest
 pytest-timeout
```

