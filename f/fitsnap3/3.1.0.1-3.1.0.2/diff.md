# Comparing `tmp/fitsnap3-3.1.0.1.tar.gz` & `tmp/fitsnap3-3.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsnap3-3.1.0.1.tar", last modified: Fri May 19 23:51:21 2023, max compression
+gzip compressed data, was "fitsnap3-3.1.0.2.tar", last modified: Tue May 23 19:13:34 2023, max compression
```

## Comparing `fitsnap3-3.1.0.1.tar` & `fitsnap3-3.1.0.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/
--rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.1.0.1/LICENSE
--rw-rw-r--   0 drew      (1000) drew      (1000)    24956 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     3819 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/README.md
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2062 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3/__main__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3/fitsnap.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3.egg-info/
--rw-rw-r--   0 drew      (1000) drew      (1000)    24956 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     5206 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/SOURCES.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/dependency_links.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/requires.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/top_level.txt
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3lib/calculators/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    18640 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1240 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     9650 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_base.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11388 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    25241 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    28349 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10443 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/fitsnap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3811 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/initialize.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.851093 fitsnap3-3.1.0.1/fitsnap3lib/io/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/error.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7670 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/input.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      374 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.851093 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1645 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      905 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/output_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8636 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/outputs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7918 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14208 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      287 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/template_output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8163 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      346 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7408 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2209 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1057 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      850 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/eshift.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2301 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/extras.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4860 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/groups.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      881 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/memory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1022 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/outfile.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      745 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/path.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1249 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/reference.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1633 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/section_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6824 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/sections.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1136 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      497 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4495 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5562 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      506 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1611 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      387 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/template.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      986 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/trainshift.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.859093 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.859093 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pairwise.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pas.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12048 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/write.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.859093 fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/regressor.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.863093 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/setup.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.863093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.867093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/genlib.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.867093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.867093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/young.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      354 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/parallel_output.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    37710 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/parallel_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.871093 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4024 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/ase_funcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4513 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/json_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17005 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scrape.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      783 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scraper_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/template_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    27319 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/vasp_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19569 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/xyz_scraper.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.875093 fitsnap3-3.1.0.1/fitsnap3lib/solvers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2906 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/anl.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2984 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10116 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/bcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8379 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/lreg.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5167 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/mcmc.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4828 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/merr.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    39329 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/opt.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    43491 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2868 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    24358 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1110 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1622 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/svd.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      187 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/template_solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1733 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/tensorflowsvd.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.875093 fitsnap3-3.1.0.1/fitsnap3lib/tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/configuration.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/dataframe_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/dataloaders.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1157 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/group_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/lammps_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/nn_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/test_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.879093 fitsnap3-3.1.0.1/fitsnap3lib/units/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/conversion_finder.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/energy.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/force.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/length.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/mass.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/pressure.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/temperature.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/time.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/units.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1096 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/pyproject.toml
--rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/setup.cfg
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/tests/
--rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/tests/test_examples.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11801 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/tests/test_pytorch.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.1.0.2/LICENSE
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24931 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3795 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.2/README.md
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.750412 fitsnap3-3.1.0.2/fitsnap3/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2062 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3/__main__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3/fitsnap.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3.egg-info/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24931 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5206 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/SOURCES.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/dependency_links.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/requires.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/top_level.txt
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3lib/calculators/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    18640 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1240 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     9650 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_base.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11388 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    25241 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    28349 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10427 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.2/fitsnap3lib/fitsnap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3811 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/initialize.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3lib/io/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/error.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7650 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/input.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      374 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.758412 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1645 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      905 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/output_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8636 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/outputs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7918 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14208 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      287 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/template_output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8163 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/ace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      346 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7408 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2209 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1057 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      850 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/eshift.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2301 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/extras.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4860 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/groups.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      881 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/memory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1022 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/outfile.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      745 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/path.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1249 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/reference.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1633 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/section_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6824 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/sections.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1136 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      497 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4495 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5562 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      506 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1611 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      387 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/template.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      986 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/trainshift.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.766412 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.766412 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pairwise.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pas.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12048 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/write.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.766412 fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/regressor.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.770412 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/setup.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.770412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.770412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/gen_labels.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/genlib.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.774412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/tree_method.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.774412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/young.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      354 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/parallel_output.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    37710 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/parallel_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.778412 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4024 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/ase_funcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4513 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/json_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17005 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scrape.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      783 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scraper_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/template_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    27319 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/vasp_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19569 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/xyz_scraper.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.778412 fitsnap3-3.1.0.2/fitsnap3lib/solvers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2906 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/anl.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2984 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10116 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/bcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8379 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/lreg.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5167 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/mcmc.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4828 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/merr.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    39329 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/opt.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    43491 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2868 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24358 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1110 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1622 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/svd.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      187 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/template_solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1733 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/tensorflowsvd.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.782412 fitsnap3-3.1.0.2/fitsnap3lib/tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/configuration.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/dataframe_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/dataloaders.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1157 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/group_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/lammps_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/nn_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/test_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/fitsnap3lib/units/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/conversion_finder.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/energy.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/force.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/length.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/mass.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/pressure.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/temperature.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/time.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/units.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1096 2023-05-23 19:11:06.000000 fitsnap3-3.1.0.2/pyproject.toml
+-rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/setup.cfg
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/tests/
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/tests/test_examples.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11801 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/tests/test_pytorch.py
```

### Comparing `fitsnap3-3.1.0.1/LICENSE` & `fitsnap3-3.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/PKG-INFO` & `fitsnap3-3.1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.1.0.1
+Version: 3.1.0.2
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991 
         
@@ -356,15 +356,15 @@
         GNU Library General Public License instead of this License.
         
 Project-URL: repository, https://github.com/FitSNAP/FitSNAP
 Project-URL: documentation, https://fitsnap.github.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!----------------BEGIN-HEADER------------------------------------>
 
 <img width="300" alt="FitSNAP" src="https://github.com/FitSNAP/FitSNAP/blob/master/docs/images/FitSNAP.png">
 
@@ -378,20 +378,20 @@
 **Colab Python notebook tutorial:** [https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb](https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb)
 
 #### How to cite 
 Rohskopf et al., (2023). FitSNAP: Atomistic machine learning with LAMMPS. Journal of Open Source Software, 8(84), 5118, https://doi.org/10.21105/joss.05118
 
 #### Dependencies:
 
-* This package expects Python 3.8+ 
+* This package expects Python 3.10+ 
 * Python dependencies: See `pyproject.toml`
 * [Compile LAMMPS as a shared library with python support](https://docs.lammps.org/Python_head.html). 
 If you can run `import lammps; lmp = lammps.lammps()` without errors in your Python interpreter, 
 you're good to go!
-* [Optional] To use neural network fitting functionality, install PyTorch with `pip install torch`. 
+* [Optional] To use neural network fitting functionality, install PyTorch. 
 * [Optional] For optimal performance, also install your favorite flavor of MPI (OpenMPI, MPICH) and 
 the Python package `mpi4py`. If installing mpi4py with a Python package manager, we recommend using 
 pip over conda as pip will auto-configure your package to your system's defaut MPI version 
 (usually what you used to build LAMMPS).
 * [Optional] For atomic cluster expansion (ACE) capabilities, build LAMMPS with the ML-PACE package, 
 along with the `compute_pace` files from [https://github.com/jmgoff/lammps-user-pace](https://github.com/jmgoff/lammps-user-pace)
```

### Comparing `fitsnap3-3.1.0.1/README.md` & `fitsnap3-3.1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 **Colab Python notebook tutorial:** [https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb](https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb)
 
 #### How to cite 
 Rohskopf et al., (2023). FitSNAP: Atomistic machine learning with LAMMPS. Journal of Open Source Software, 8(84), 5118, https://doi.org/10.21105/joss.05118
 
 #### Dependencies:
 
-* This package expects Python 3.8+ 
+* This package expects Python 3.10+ 
 * Python dependencies: See `pyproject.toml`
 * [Compile LAMMPS as a shared library with python support](https://docs.lammps.org/Python_head.html). 
 If you can run `import lammps; lmp = lammps.lammps()` without errors in your Python interpreter, 
 you're good to go!
-* [Optional] To use neural network fitting functionality, install PyTorch with `pip install torch`. 
+* [Optional] To use neural network fitting functionality, install PyTorch. 
 * [Optional] For optimal performance, also install your favorite flavor of MPI (OpenMPI, MPICH) and 
 the Python package `mpi4py`. If installing mpi4py with a Python package manager, we recommend using 
 pip over conda as pip will auto-configure your package to your system's defaut MPI version 
 (usually what you used to build LAMMPS).
 * [Optional] For atomic cluster expansion (ACE) capabilities, build LAMMPS with the ML-PACE package, 
 along with the `compute_pace` files from [https://github.com/jmgoff/lammps-user-pace](https://github.com/jmgoff/lammps-user-pace)
```

### Comparing `fitsnap3-3.1.0.1/fitsnap3/__main__.py` & `fitsnap3-3.1.0.2/fitsnap3/__main__.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3.egg-info/PKG-INFO` & `fitsnap3-3.1.0.2/fitsnap3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.1.0.1
+Version: 3.1.0.2
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991 
         
@@ -356,15 +356,15 @@
         GNU Library General Public License instead of this License.
         
 Project-URL: repository, https://github.com/FitSNAP/FitSNAP
 Project-URL: documentation, https://fitsnap.github.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!----------------BEGIN-HEADER------------------------------------>
 
 <img width="300" alt="FitSNAP" src="https://github.com/FitSNAP/FitSNAP/blob/master/docs/images/FitSNAP.png">
 
@@ -378,20 +378,20 @@
 **Colab Python notebook tutorial:** [https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb](https://colab.research.google.com/github/FitSNAP/FitSNAP/blob/master/tutorial.ipynb)
 
 #### How to cite 
 Rohskopf et al., (2023). FitSNAP: Atomistic machine learning with LAMMPS. Journal of Open Source Software, 8(84), 5118, https://doi.org/10.21105/joss.05118
 
 #### Dependencies:
 
-* This package expects Python 3.8+ 
+* This package expects Python 3.10+ 
 * Python dependencies: See `pyproject.toml`
 * [Compile LAMMPS as a shared library with python support](https://docs.lammps.org/Python_head.html). 
 If you can run `import lammps; lmp = lammps.lammps()` without errors in your Python interpreter, 
 you're good to go!
-* [Optional] To use neural network fitting functionality, install PyTorch with `pip install torch`. 
+* [Optional] To use neural network fitting functionality, install PyTorch. 
 * [Optional] For optimal performance, also install your favorite flavor of MPI (OpenMPI, MPICH) and 
 the Python package `mpi4py`. If installing mpi4py with a Python package manager, we recommend using 
 pip over conda as pip will auto-configure your package to your system's defaut MPI version 
 (usually what you used to build LAMMPS).
 * [Optional] For atomic cluster expansion (ACE) capabilities, build LAMMPS with the ML-PACE package, 
 along with the `compute_pace` files from [https://github.com/jmgoff/lammps-user-pace](https://github.com/jmgoff/lammps-user-pace)
```

### Comparing `fitsnap3-3.1.0.1/fitsnap3.egg-info/SOURCES.txt` & `fitsnap3-3.1.0.2/fitsnap3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator.py` & `fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator_factory.py` & `fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_base.py` & `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_base.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_custom.py` & `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_pace.py` & `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_snap.py` & `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_snap.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/fitsnap.py` & `fitsnap3-3.1.0.2/fitsnap3lib/fitsnap.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         scraper (:obj:`class` Scraper): Instance of the Scraper class for gathering configs.
         data (:obj:`list`): List of dictionaries, where each configuration of atoms has its own 
             dictionary.
         calculator (:obj:`class` Calculator): Instance of the Calculator class for calculating 
             descriptors and fitting data.
         solver (:obj:`class` Solver): Instance of the Solver class for performing a fit.
     """
-    def __init__(self, input: (str | dict)=None, comm=None, arglist: list=None):
+    def __init__(self, input=None, comm=None, arglist: list=[]):
         self.comm = comm
         # Instantiate ParallelTools and Config instances belonging to this FitSnap instance.
         # NOTE: Each proc in `comm` creates a different `pt` object, but shared arrays still share 
         #       memory within `comm`.
         self.pt = ParallelTools(comm=comm)
         self.pt.all_barrier()
         self.config = Config(self.pt, input, arguments_lst=arglist)
```

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/initialize.py` & `fitsnap3-3.1.0.2/fitsnap3lib/initialize.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/input.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Attributes:
         infile: String for optional input filename. Defaults to None.
         indict: Dictionary for optional input dictionary of settings, to replace input file. Defaults 
             to None.
         
     """
 
-    def __init__(self, pt, input: (str | dict) = None, arguments_lst: list = None):
+    def __init__(self, pt, input=None, arguments_lst: list = []):
         self.pt = pt
         self.input = input
         # Input file (infile) and dictionary (indict) set to None by default and get set in 
         # parse_config.
         self.infile = None
         self.indict = None
         self.default_protocol = HIGHEST_PROTOCOL
@@ -41,15 +41,15 @@
 
         # Generate random 128 bit hash to identify this fit on rank 0.
         if self.pt._rank == 0:
             self.hash = f"{random.getrandbits(128):032x}"
         else:
             self.hash = None
 
-    def parse_cmdline(self, arguments_lst=None):
+    def parse_cmdline(self, arguments_lst=[]):
         """ Parse command line args. """
         parser = argparse.ArgumentParser(prog="fitsnap3")
         if (self.input is None):
             parser.add_argument("infile", action="store",
                                 help="Input file with bispectrum etc. options")
 
         # Optional args.
```

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/custom.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/output_factory.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/output_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/outputs.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/pace.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/snap.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/snap.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/ace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/eshift.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/eshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/extras.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/extras.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/groups.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/groups.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/memory.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/memory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/outfile.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/outfile.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/path.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/path.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/reference.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/reference.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/scraper.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/section_factory.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/section_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/sections.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/sections.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/ard.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/ard.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/jax.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/network.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/solver.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/solver.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/trainshift.py` & `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/trainshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/jax.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pairwise.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pairwise.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pas.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pas.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pytorch.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/write.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/write.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/regressor.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/regressor.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/setup.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/setup.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/gen_labels.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/genlib.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/genlib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/tree_method.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/young.py` & `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/young.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/parallel_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/parallel_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/ase_funcs.py` & `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/ase_funcs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/json_scraper.py` & `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/json_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scrape.py` & `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scrape.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scraper_factory.py` & `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scraper_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/vasp_scraper.py` & `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/vasp_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/xyz_scraper.py` & `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/xyz_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/anl.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/anl.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/ard.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/ard.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/bcs.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/bcs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/jax.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/lasso.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/lasso.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/lreg.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/lreg.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/mcmc.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/mcmc.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/merr.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/merr.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/network.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/opt.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/opt.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/pytorch.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/ridge.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/ridge.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/scalapack.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver_factory.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/svd.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/svd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/solvers/tensorflowsvd.py` & `fitsnap3-3.1.0.2/fitsnap3lib/solvers/tensorflowsvd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/configuration.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/dataframe_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/dataframe_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/dataloaders.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/dataloaders.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/group_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/group_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/lammps_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/lammps_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/nn_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/nn_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/tools/test_tools.py` & `fitsnap3-3.1.0.2/fitsnap3lib/tools/test_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/units/conversion_finder.py` & `fitsnap3-3.1.0.2/fitsnap3lib/units/conversion_finder.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/fitsnap3lib/units/units.py` & `fitsnap3-3.1.0.2/fitsnap3lib/units/units.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/pyproject.toml` & `fitsnap3-3.1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = [
     "setuptools>=42",
 ]
-build-backend = 'setuptools.build_meta'
+build-backend = 'setuptools.build_meta' 
 
 [project]
 name = "fitsnap3"
-version = "3.1.0.1"
+version = "3.1.0.2"
 description = "Molecular Machine Learning Interface"
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.10.0"
+requires-python = ">=3.9.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 authors = [
     { name = "Drew Rohskopf", email = "adrohsk@sandia.gov" },
```

### Comparing `fitsnap3-3.1.0.1/tests/test_examples.py` & `fitsnap3-3.1.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.1/tests/test_pytorch.py` & `fitsnap3-3.1.0.2/tests/test_pytorch.py`

 * *Files identical despite different names*

