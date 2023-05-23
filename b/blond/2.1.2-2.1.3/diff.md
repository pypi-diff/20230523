# Comparing `tmp/blond-2.1.2.tar.gz` & `tmp/blond-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.2.tar", last modified: Tue May  9 15:49:52 2023, max compression
+gzip compressed data, was "blond-2.1.3.tar", last modified: Tue May 23 10:07:10 2023, max compression
```

## Comparing `blond-2.1.2.tar` & `blond-2.1.3.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-09 15:49:23.000000 blond-2.1.2/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6235 2023-05-09 15:49:23.000000 blond-2.1.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3345 2023-05-09 15:49:23.000000 blond-2.1.2/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-09 15:49:23.000000 blond-2.1.2/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-05-09 15:49:23.000000 blond-2.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-09 15:49:23.000000 blond-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13940 2023-05-09 15:49:52.656000 blond-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13164 2023-05-09 15:49:23.000000 blond-2.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-09 15:49:23.000000 blond-2.1.2/WARNINGS.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.616000 blond-2.1.2/__BENCHMARKS/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/.gitignore
--rw-r--r--   0 root         (0) root         (0)    16964 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
--rw-r--r--   0 root         (0) root         (0)     4291 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM2_OTFB_no_beam.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM3_OTFB_moving_average.py
--rw-r--r--   0 root         (0) root         (0)     7415 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM4_OTFB_with_beam.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-05-09 15:49:23.000000 blond-2.1.2/__BENCHMARKS/BM5_OTFB_feedforward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.612000 blond-2.1.2/__EXAMPLES/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.620000 blond-2.1.2/__EXAMPLES/gpu_main_files/
--rw-r--r--   0 root         (0) root         (0)     5807 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     6581 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     7056 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    14174 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     9212 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.620000 blond-2.1.2/__EXAMPLES/input_files/
--rw-r--r--   0 root         (0) root         (0)    11866 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
--rw-r--r--   0 root         (0) root         (0)    16868 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_02_Finemet.txt
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
--rw-r--r--   0 root         (0) root         (0)    11976 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.624000 blond-2.1.2/__EXAMPLES/main_files/
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7353 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5605 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_06_Preprocess.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4651 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
--rw-r--r--   0 root         (0) root         (0)    11630 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
--rw-r--r--   0 root         (0) root         (0)    10276 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_14_sparse_slicing.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_18_robinson_instability.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_19_bunch_generation.py
--rw-r--r--   0 root         (0) root         (0)     6646 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
--rw-r--r--   0 root         (0) root         (0)     3132 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_21_bunch_distribution.py
--rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.624000 blond-2.1.2/__EXAMPLES/mpi_main_files/
--rw-r--r--   0 root         (0) root         (0)     5008 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
--rw-r--r--   0 root         (0) root         (0)     7618 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
--rw-r--r--   0 root         (0) root         (0)     5932 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
--rw-r--r--   0 root         (0) root         (0)    12098 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
--rw-r--r--   0 root         (0) root         (0)     6688 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_07_Ions.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
--rw-r--r--   0 root         (0) root         (0)     5255 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-05-09 15:49:23.000000 blond-2.1.2/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.624000 blond-2.1.2/__doc/
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/Makefile
--rw-r--r--   0 root         (0) root         (0)     5797 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      809 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.628000 blond-2.1.2/__doc/modules/
--rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ACS_cavity_loop.png
--rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ACS_cavity_loop.svg
--rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/RF_noise.gle
--rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/RF_noise.png
--rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/SPS_OTFB.png
--rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/SPS_OTFB.svg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/beam.rst
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/compile.rst
--rw-r--r--   0 root         (0) root         (0)    51317 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/csr_impedance_real.png
--rw-r--r--   0 root         (0) root         (0)    19684 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/equations_of_motion.rst
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/impedances.rst
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/input_parameters.rst
--rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/lhc_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)    20259 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/llrf.rst
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/monitors.rst
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/plots.rst
--rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ring_and_RFstation.gle
--rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/ring_and_RFstation.png
--rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sample.dat
--rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sample2.dat
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sanity_check.rst
--rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/sps_cavity_loop.rst
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/synchrotron_radiation.rst
--rw-r--r--   0 root         (0) root         (0)     1166 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/toolbox.rst
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/trackers.rst
--rw-r--r--   0 root         (0) root         (0)     1096 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/modules/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.612000 blond-2.1.2/__doc/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.632000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/footer.html
--rw-r--r--   0 root         (0) root         (0)     7063 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     7526 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout_old.html
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.612000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.632000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
--rw-r--r--   0 root         (0) root         (0)     3153 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
--rw-r--r--   0 root         (0) root         (0)   114281 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)    67610 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   124988 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   109948 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)    96964 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   656544 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   656568 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)   170616 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 root         (0) root         (0)   169064 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 root         (0) root         (0)    76518 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   391622 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   152796 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    90412 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    71896 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     2457 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
--rw-r--r--   0 root         (0) root         (0)    15414 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
--rw-r--r--   0 root         (0) root         (0)     6477 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-09 15:49:23.000000 blond-2.1.2/__doc/themes/sphinx_rtd_theme/versions.html
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-09 15:49:23.000000 blond-2.1.2/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/blond/
--rw-r--r--   0 root         (0) root         (0)     1199 2023-05-09 15:49:23.000000 blond-2.1.2/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-09 15:49:48.000000 blond-2.1.2/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20374 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    41527 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    39107 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    24385 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4804 2023-05-09 15:49:23.000000 blond-2.1.2/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    11654 2023-05-09 15:49:23.000000 blond-2.1.2/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10031 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/kick.cpp
--rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-09 15:49:52.000000 blond-2.1.2/blond/cpp_routines/libblond.so
--rw-r--r--   0 root         (0) root         (0)     6406 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-05-09 15:49:23.000000 blond-2.1.2/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.640000 blond-2.1.2/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/cuda_kernels/kernels_single.cu
--rw-r--r--   0 root         (0) root         (0)    10769 2023-05-09 15:49:23.000000 blond-2.1.2/blond/gpu/cupy_butils_wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39560 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    45896 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12228 2023-05-09 15:49:23.000000 blond-2.1.2/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24903 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    20249 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17272 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22443 2023-05-09 15:49:23.000000 blond-2.1.2/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    36313 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14383 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7257 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4394 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15759 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18814 2023-05-09 15:49:23.000000 blond-2.1.2/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20936 2023-05-09 15:49:23.000000 blond-2.1.2/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11025 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10004 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14165 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1210 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-05-09 15:49:23.000000 blond-2.1.2/blond/plots/plot_slices.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-09 15:49:23.000000 blond-2.1.2/blond/sanity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.644000 blond-2.1.2/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-05-09 15:49:23.000000 blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8111 2023-05-09 15:49:23.000000 blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5221 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7570 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7479 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    21008 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4877 2023-05-09 15:49:23.000000 blond-2.1.2/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26351 2023-05-09 15:49:23.000000 blond-2.1.2/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    31248 2023-05-09 15:49:23.000000 blond-2.1.2/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/blond/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    48243 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/butils_wrap.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/input_parser.py
--rw-r--r--   0 root         (0) root         (0)    14206 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/profile_mock.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-05-09 15:49:23.000000 blond-2.1.2/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.636000 blond-2.1.2/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13940 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9913 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:49:48.000000 blond-2.1.2/blond.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      400 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-09 15:49:52.000000 blond-2.1.2/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-09 15:49:23.000000 blond-2.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-09 15:49:23.000000 blond-2.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 15:49:52.656000 blond-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4808 2023-05-09 15:49:23.000000 blond-2.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.616000 blond-2.1.2/unittests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.648000 blond-2.1.2/unittests/beam_profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)   800196 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/dt_coordinates.npz
--rw-r--r--   0 root         (0) root         (0)    12422 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/test_beam_profile_object.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beam_profile/test_sparse_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/beams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beams/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14105 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beams/test_beam_object.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/beams/test_coasting_beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/general/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/general/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16184 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/general/test_separatrix_bigaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/gpu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)    16996 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/test_impedance.py
--rw-r--r--   0 root         (0) root         (0)    22133 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/gpu/test_physics_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/impedances/test_impedance.py
--rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/impedances/test_impedance_sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/test_preprocess.py
--rw-r--r--   0 root         (0) root         (0)    10862 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/test_rf_params_object.py
--rw-r--r--   0 root         (0) root         (0)     7576 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/input_parameters/test_ring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.652000 blond-2.1.2/unittests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_gpu_examples.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_mpi_examples.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_validate_gpu.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/integration/test_validate_mpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/ref_DV_MOD_FR.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/ref_DV_MOD_FRF.npy
--rw-r--r--   0 root         (0) root         (0)    74048 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/ref_V_IND_COARSE_GEN.npy
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    31675 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    40554 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    31838 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/llrf/test_signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32615 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/synchrotron_radiation/test_synch_rad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17866 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/comparison_drift.py
--rw-r--r--   0 root         (0) root         (0)    19415 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/test_drift.py
--rw-r--r--   0 root         (0) root         (0)    10188 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/trackers/test_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:49:52.656000 blond-2.1.2/unittests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21108 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_blondmath.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_ffts.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-05-09 15:49:23.000000 blond-2.1.2/unittests/utils/test_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.280000 blond-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-23 10:06:32.000000 blond-2.1.3/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-05-23 10:06:32.000000 blond-2.1.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-05-23 10:06:32.000000 blond-2.1.3/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-23 10:06:32.000000 blond-2.1.3/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-05-23 10:06:32.000000 blond-2.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-23 10:06:32.000000 blond-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13971 2023-05-23 10:07:10.280000 blond-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13195 2023-05-23 10:06:32.000000 blond-2.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-23 10:06:32.000000 blond-2.1.3/WARNINGS.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.224000 blond-2.1.3/__BENCHMARKS/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    16964 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM2_OTFB_no_beam.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM3_OTFB_moving_average.py
+-rw-r--r--   0 root         (0) root         (0)     7415 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM4_OTFB_with_beam.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-05-23 10:06:32.000000 blond-2.1.3/__BENCHMARKS/BM5_OTFB_feedforward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.216000 blond-2.1.3/__EXAMPLES/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.228000 blond-2.1.3/__EXAMPLES/gpu_main_files/
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    14174 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5582 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     9212 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.228000 blond-2.1.3/__EXAMPLES/input_files/
+-rw-r--r--   0 root         (0) root         (0)    11866 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
+-rw-r--r--   0 root         (0) root         (0)    16868 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_02_Finemet.txt
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
+-rw-r--r--   0 root         (0) root         (0)    11976 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.232000 blond-2.1.3/__EXAMPLES/main_files/
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     7353 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     5605 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_06_Preprocess.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    11630 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_14_sparse_slicing.py
+-rw-r--r--   0 root         (0) root         (0)     4665 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_18_robinson_instability.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_19_bunch_generation.py
+-rw-r--r--   0 root         (0) root         (0)     6646 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_21_bunch_distribution.py
+-rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.232000 blond-2.1.3/__EXAMPLES/mpi_main_files/
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
+-rw-r--r--   0 root         (0) root         (0)     5932 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
+-rw-r--r--   0 root         (0) root         (0)    12098 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
+-rw-r--r--   0 root         (0) root         (0)     6688 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_07_Ions.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-05-23 10:06:32.000000 blond-2.1.3/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.236000 blond-2.1.3/__doc/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5797 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      809 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.240000 blond-2.1.3/__doc/modules/
+-rwxr-xr-x   0 root         (0) root         (0)   135010 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ACS_cavity_loop.png
+-rwxr-xr-x   0 root         (0) root         (0)   185223 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ACS_cavity_loop.svg
+-rwxr-xr-x   0 root         (0) root         (0)     1144 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/RF_noise.gle
+-rwxr-xr-x   0 root         (0) root         (0)    81234 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/RF_noise.png
+-rwxr-xr-x   0 root         (0) root         (0)   176302 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/SPS_OTFB.png
+-rwxr-xr-x   0 root         (0) root         (0)   655573 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/SPS_OTFB.svg
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/beam.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/compile.rst
+-rw-r--r--   0 root         (0) root         (0)    51317 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/csr_impedance_real.png
+-rw-r--r--   0 root         (0) root         (0)    19684 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/equations_of_motion.rst
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/impedances.rst
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/input_parameters.rst
+-rwxr-xr-x   0 root         (0) root         (0)     7100 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/lhc_cavity_loop.rst
+-rw-r--r--   0 root         (0) root         (0)    20259 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/llrf.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/monitors.rst
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/plots.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1050 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ring_and_RFstation.gle
+-rwxr-xr-x   0 root         (0) root         (0)    84423 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/ring_and_RFstation.png
+-rwxr-xr-x   0 root         (0) root         (0)       39 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sample.dat
+-rwxr-xr-x   0 root         (0) root         (0)       77 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sample2.dat
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sanity_check.rst
+-rwxr-xr-x   0 root         (0) root         (0)    14087 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/sps_cavity_loop.rst
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/synchrotron_radiation.rst
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/toolbox.rst
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/trackers.rst
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/modules/utils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.216000 blond-2.1.3/__doc/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.244000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/layout.html
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/layout_old.html
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/search.html
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.216000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.244000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
+-rw-r--r--   0 root         (0) root         (0)   114281 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)    67610 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)   124988 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   109948 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)    96964 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   656544 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)   656568 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)   170616 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 root         (0) root         (0)   169064 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 root         (0) root         (0)    76518 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   391622 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   152796 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    90412 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    71896 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
+-rw-r--r--   0 root         (0) root         (0)    15414 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
+-rw-r--r--   0 root         (0) root         (0)     6477 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-23 10:06:32.000000 blond-2.1.3/__doc/themes/sphinx_rtd_theme/versions.html
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-23 10:06:32.000000 blond-2.1.3/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/blond/
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-23 10:06:32.000000 blond-2.1.3/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-23 10:07:04.000000 blond-2.1.3/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.256000 blond-2.1.3/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20374 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    41527 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    39107 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    24385 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4804 2023-05-23 10:06:32.000000 blond-2.1.3/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    12315 2023-05-23 10:06:32.000000 blond-2.1.3/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/kick.cpp
+-rwxr-xr-x   0 root         (0) root         (0)   126096 2023-05-23 10:07:10.000000 blond-2.1.3/blond/cpp_routines/libblond.so
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-05-23 10:06:32.000000 blond-2.1.3/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10554 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/butils_wrap_cupy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-05-23 10:06:32.000000 blond-2.1.3/blond/gpu/cuda_kernels/kernels_single.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39560 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    45965 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12228 2023-05-23 10:06:32.000000 blond-2.1.3/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.260000 blond-2.1.3/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24903 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    20249 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17272 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22443 2023-05-23 10:06:32.000000 blond-2.1.3/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    36313 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7257 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15759 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18814 2023-05-23 10:06:32.000000 blond-2.1.3/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20936 2023-05-23 10:06:32.000000 blond-2.1.3/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10004 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14165 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-05-23 10:06:32.000000 blond-2.1.3/blond/plots/plot_slices.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-05-23 10:06:32.000000 blond-2.1.3/blond/sanity_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.264000 blond-2.1.3/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-05-23 10:06:32.000000 blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-05-23 10:06:32.000000 blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.268000 blond-2.1.3/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5221 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7570 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    21008 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-23 10:06:32.000000 blond-2.1.3/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.268000 blond-2.1.3/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26351 2023-05-23 10:06:32.000000 blond-2.1.3/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    31248 2023-05-23 10:06:32.000000 blond-2.1.3/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.268000 blond-2.1.3/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8321 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    47022 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/butils_wrap_cpp.py
+-rw-r--r--   0 root         (0) root         (0)    15016 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/butils_wrap_python.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14206 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-05-23 10:06:32.000000 blond-2.1.3/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.252000 blond-2.1.3/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13971 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 10:07:04.000000 blond-2.1.3/blond.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      400 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 10:07:10.000000 blond-2.1.3/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-23 10:06:32.000000 blond-2.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-23 10:06:32.000000 blond-2.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 10:07:10.280000 blond-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-05-23 10:06:32.000000 blond-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.220000 blond-2.1.3/unittests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/beam_profile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   800196 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/dt_coordinates.npz
+-rw-r--r--   0 root         (0) root         (0)    12422 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/test_beam_profile_object.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beam_profile/test_sparse_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/beams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14105 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beams/test_beam_object.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/beams/test_coasting_beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/general/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/general/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16184 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/general/test_separatrix_bigaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/test_ffts.py
+-rw-r--r--   0 root         (0) root         (0)    16996 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/test_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    22133 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/gpu/test_physics_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.272000 blond-2.1.3/unittests/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/impedances/test_impedance.py
+-rwxr-xr-x   0 root         (0) root         (0)     4940 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/impedances/test_impedance_sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/test_preprocess.py
+-rw-r--r--   0 root         (0) root         (0)    10862 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/test_rf_params_object.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/input_parameters/test_ring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_gpu_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_mpi_examples.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_validate_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/integration/test_validate_mpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/ref_DV_MOD_FR.npy
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/ref_DV_MOD_FRF.npy
+-rw-r--r--   0 root         (0) root         (0)    74048 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/ref_V_IND_COARSE_GEN.npy
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    31675 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    40554 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    31838 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/llrf/test_signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.276000 blond-2.1.3/unittests/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32615 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/synchrotron_radiation/test_synch_rad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.280000 blond-2.1.3/unittests/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17866 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/comparison_drift.py
+-rw-r--r--   0 root         (0) root         (0)    19415 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/test_drift.py
+-rw-r--r--   0 root         (0) root         (0)    10188 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/trackers/test_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:07:10.280000 blond-2.1.3/unittests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23172 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_blondmath.py
+-rw-r--r--   0 root         (0) root         (0)    21382 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_butils_wrap_python.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_ffts.py
+-rw-r--r--   0 root         (0) root         (0)     5103 2023-05-23 10:06:32.000000 blond-2.1.3/unittests/utils/test_iteration.py
```

### Comparing `blond-2.1.2/.gitignore` & `blond-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/.gitlab-ci.yml` & `blond-2.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/CHANGELOG` & `blond-2.1.3/CHANGELOG`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/LICENSE.txt` & `blond-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/PKG-INFO` & `blond-2.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.2
+Version: 2.1.3
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko et al.
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -42,134 +42,115 @@
 
 Repository: <https://gitlab.cern.ch/blond/BLonD>
 
 Documentation: <https://blond-code.docs.cern.ch/>
 
 Project website: <http://blond.web.cern.ch>
 
-# Install
+# Installation
 
-## Requirements
+## Dependencies
 
-1.  A gcc compiler with C++11 support (version greater than 4.8.4).
-2.  An Anaconda distribution (Python 3 recommended).
-3.  That's all!
+1. Python 3.6 or above (Anaconda is recommended).  
+2. (Optional) For better performance, a C++ (e.g. `gcc`, `icc`, `clang`, etc) compiler with `C++11` support.
 
-## Windows GCC Installation Instructions
+### (Optional) C++ compiler installation instructions
+
+#### Windows
 
 1.  Download the latest mingw-w64 using this link:
     <https://winlibs.com/#download-release>
 2.  Extract the downloaded zip/7-zip under e.g. `C:\`. You should now
     see a directory `C:\mingw64`.
 3.  Add `C:\mingw64\bin` in the PATH Environment Variable. [Here you can
     see how to do this in Windows
     XP/Vista/7/8/10/11](https://www.computerhope.com/issues/ch000549.htm).
 4.  To validate the correct setup of gcc, open a command prompt and
     type: `gcc --version`. The first output line should contain the gcc
     version you just installed.
 
-## Install Steps
+#### Linux
+Use your distribution's package manager to install the compiler of your choice. BLonD has been tested with: `gcc` (recommended), `icc`, and `clang`.
 
-### Installing BLonD as a python package.
+## Installation Steps
 
--   Using the pip package manager:
+### Installing BLonD as a python package.
 
-    ``` bash
-    $ pip install blond
+-   Using the `pip` package manager:
+    ```bash
+    pip install blond
     ```
 
--   If this fails try to:
-
-    1.  Clone the repository from gitlab or download and extract the zip
-        from <https://gitlab.cern.ch/blond/BLonD/-/archive/master/BLonD-master.zip>
-    2.  Go to the downloaded BLonD directory and run:
-
-        ``` bash
-        $ python setup.py install
-        ```
-
--   If it still fails, go to the BLonD directory and run:
-
-    1.  
-        ``` bash
-        $ python setup.py compile
-        ```
-
-    2.  Then you have to set the PYTHONPATH variable to point to the
-        BLonD installation path.
-
--   In the occasion that it continues to fail, please open a new gitlab issue.
+### Installing BLonD manually (advanced users/ developers).
 
-### For advanced users or developers.
-
-1.  You are advised to install git in your system.
-2.  Clone the repository or download and extract it.
-3.  From within the BLonD directory run:
-    ``` bash
-    $ python blond/compile.py
+1.  Clone the repository (with `git`) or download and extract it.
+2.  (Optional) From within the BLonD directory run:
+    ```bash
+    python blond/compile.py
     ```
-4.  Adjust the PYTHONPATH to contain the path to the cloned repository.
+3. (Optional) See the complete list of the command line arguments with:
+    ```bash
+    python blond/compile.py --help
+    ```
+4.  Adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory.
 
 ## Confirm proper installation
 
--   Run the unittests with pytest (may need to be installed first with
-    pip install pytest):
-
+-   Run the unittests with `pytest` (the `pytest` package may need to be installed first):
     ``` bash
-    $ pytest -v unittests
+    pytest -v unittests
     ```
 
--   Try to run some of the main files found in the examples:
-
+-   Run some of the main files found in the `__EXAMPLES` directory:
     ``` bash
-    $ python __EXAMPLES/main_files/EX_01_Acceleration.py
-    $ python __EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
-    $ etc..
+    python __EXAMPLES/main_files/EX_01_Acceleration.py
+    python __EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+    etc..
     ```
 
-## Performace Optimizations
+# Performance Optimizations
+By default, if the C++ blond library has not been compiled, the python-only backend will be used to run the most time-consuming operations. 
 
-There are some easy ways to reduce the execution time of your
-simulation:
+To use the C++ backend and accelerate the execution of the time-consuming operations, follow the instructions provided in the section *Installing BLonD manually*.
 
-1.  Use the multi-threaded C library. To use it you have to add the -p
-    flag when compiling the C library:
+In addition you may want to:
+* Use the multi-threaded blond C++ backend:
     ``` bash
-    $ python blond/compile.py --parallel
+    python blond/compile.py --parallel
     ```
 
-2.  Enable processor specific compiler optimizations:
+* Enable processor specific compiler optimizations:
     ``` bash
-    $ python blond/compile.py --flags='-march=native'
+    python blond/compile.py --parallel --optimize
     ```
 
-3.  If you are test-case is calling the synchrotron radiation tracking method, you can accelerate it by using the Boost library. To do so you have to:  
+* If you are test-case is calling the synchrotron radiation tracking method, you can accelerate it by using the Boost library. To do so you have to:  
     1.  Download Boost: <https://www.boost.org/>. Let's say the version
         you downloaded is boost_1\_70.
     2.  Extract it, let's say in `/user/path/to/boost_1_70`.
     3.  Pass the boost installation path when compiling BLonD:
         ``` bash
-        $ python blond/compile.py --boost=/user/path/to/boost_1_7_70
+        python blond/compile.py --boost=/user/path/to/boost_1_7_70
         ```
 
-4.  Check the following section about the FFTW3 library.
+* Check the following section about the FFTW3 library.
 
-5.  *All the above can be combined.*
+* All the above can be combined, i.e.:
+    ```bash
+    python blond/compile.py --parallel --optimize --boost=...
+    ```
 
-## Changing the floating point precision (32 bit floats or 64 bit floats)
+## Changing the floating point number datatype
 
--   By default BLonD uses double precision calculations (float64). To
-    change to single precision, for faster calculations, in the
-    beginning of your mainfile you will have to add the code lines:
-    ``` python
-    from blond.utils import bmath as bm
-    bm.use_precision('single') 
-    ```
+By default BLonD uses double precision calculations (float64). To change to single precision for faster calculations, in the beginning of your mainfile you will have to add the following code lines:
+```python
+from blond.utils import bmath as bm
+bm.use_precision('single') 
+```
 
--   No other modifications are needed.
 
 ## Use the FFTW3 library for the FFTs
 
 So far only the `rfft()`, `irfft()` and `fftfreq()` routines are
 supported. `fft_convolve()` to be added soon.
 
 -   Windows:
@@ -330,21 +311,21 @@
     worker.finalize()
     ```
 
 6.  To run your script, you need to pass it to **mpirun** or
     **mpiexec**. To spawn P MPI processes run:
 
     ``` bash
-    $ mpirun -n P python main_file.py
+    mpirun -n P python main_file.py
     ```
 
 7.  For more examples have a look at the \_\_EXAMPLES/mpi_main_files/
     directory.
 
-# Using the GPU Implementation
+# Using the GPU backend
 
 ## Setup Instructions
 
 1.  Install **CUDA**: <https://developer.nvidia.com/cuda-downloads>
 2.  Install the **CuPy** library:
     <https://docs.cupy.dev/en/stable/install.html>
 3.  To verify your installation open a python terminal and execute the
@@ -352,68 +333,68 @@
 
     ``` python
     import cupy as cp 
     import numpy as np 
     a = cp.array(np.zeros(1000,np.float64)) 
     ```
 
-    To compile the Cuda files execute blond/compile.py and add the flag
+    To compile the CUDA files execute blond/compile.py and add the flag
     --gpu. The Compute Capability of your GPU will be automatically
     detected:
 
-``` bash
-$ python blond/compile.py --gpu 
-```
+    ``` bash
+    python blond/compile.py --gpu 
+    ```
 
 ## Changes required in the main file for GPU
 
 1.  Right before your main loop you need to add:
 
     ``` python
     from blond.utils import bmath as bm
     # change some of the basic functions to their GPU equivalent
     bm.use_gpu()
     ```
 
 2.  Also for every object you are using in your main loop that is in the
     following list:
 
-| GPU objects             |
-|-------------------------|
-| Beam                    |
-| Profile                 |
-| RingAndRFTracker        |
-| TotalInducedVoltage     |
-| InducedVoltageTime      |
-| InducedVoltageFreq      |
-| InductiveImpedance      |
-| InducedVoltageResonator |
-| RFStation               |
-| BeamFeedback            |
-
-you need to call their `to_gpu()` method. The following is a typical
-example from the \_\_EXAMPLES/gpu_main_files/EX_01_Acceleration.py
-mainfile.
-
-``` python
-# Define Objects
-beam = Beam(ring, N_p, N_b)
-profile = Profile(beam, CutOptions(n_slices=100), 
-             FitOptions(fit_option='gaussian'))
-# Initialize gpu
-beam.to_gpu()
-profile.to_gpu()
-```
+    | GPU objects             |
+    |-------------------------|
+    | Beam                    |
+    | Profile                 |
+    | RingAndRFTracker        |
+    | TotalInducedVoltage     |
+    | InducedVoltageTime      |
+    | InducedVoltageFreq      |
+    | InductiveImpedance      |
+    | InducedVoltageResonator |
+    | RFStation               |
+    | BeamFeedback            |
+
+    you need to call their `to_gpu()` method. The following is a typical
+    example from the \_\_EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+    mainfile.
+
+    ``` python
+    # Define Objects
+    beam = Beam(ring, N_p, N_b)
+    profile = Profile(beam, CutOptions(n_slices=100), 
+                FitOptions(fit_option='gaussian'))
+    # Initialize gpu
+    beam.to_gpu()
+    profile.to_gpu()
+    ```
 
-If an object of this list has a reference inside a different one you
-don't need to use the `to_gpu()` for the referenced object. In the
-previous example, we don't need to call `beam.to_gpu()` since `beam` is
-referenced inside the `profile`. The same would apply in a
-`TotalInducedVoltage` object and the objects in its
-`induced_voltage_list`.
+    If an object of this list has a reference inside a different one you
+    don't need to use the `to_gpu()` for the referenced object. In the
+    previous example, we don't need to call `beam.to_gpu()` since `beam` is
+    referenced inside the `profile`. The same would apply in a
+    `TotalInducedVoltage` object and the objects in its
+    `induced_voltage_list`.
 
 # Developers
 
 -   Simon Albright (simon.albright (at) cern.ch)
 -   Theodoros Argyropoulos (theodoros.argyropoulos (at) cern.ch)
 -   Konstantinos Iliakis (konstantinos.iliakis (at) cern.ch)
 -   Ivan Karpov (ivan.karpov (at) cern.ch)
```

### Comparing `blond-2.1.2/README.md` & `blond-2.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,134 +19,115 @@
 
 Repository: <https://gitlab.cern.ch/blond/BLonD>
 
 Documentation: <https://blond-code.docs.cern.ch/>
 
 Project website: <http://blond.web.cern.ch>
 
-# Install
+# Installation
 
-## Requirements
+## Dependencies
 
-1.  A gcc compiler with C++11 support (version greater than 4.8.4).
-2.  An Anaconda distribution (Python 3 recommended).
-3.  That's all!
+1. Python 3.6 or above (Anaconda is recommended).  
+2. (Optional) For better performance, a C++ (e.g. `gcc`, `icc`, `clang`, etc) compiler with `C++11` support.
 
-## Windows GCC Installation Instructions
+### (Optional) C++ compiler installation instructions
+
+#### Windows
 
 1.  Download the latest mingw-w64 using this link:
     <https://winlibs.com/#download-release>
 2.  Extract the downloaded zip/7-zip under e.g. `C:\`. You should now
     see a directory `C:\mingw64`.
 3.  Add `C:\mingw64\bin` in the PATH Environment Variable. [Here you can
     see how to do this in Windows
     XP/Vista/7/8/10/11](https://www.computerhope.com/issues/ch000549.htm).
 4.  To validate the correct setup of gcc, open a command prompt and
     type: `gcc --version`. The first output line should contain the gcc
     version you just installed.
 
-## Install Steps
+#### Linux
+Use your distribution's package manager to install the compiler of your choice. BLonD has been tested with: `gcc` (recommended), `icc`, and `clang`.
 
-### Installing BLonD as a python package.
+## Installation Steps
 
--   Using the pip package manager:
+### Installing BLonD as a python package.
 
-    ``` bash
-    $ pip install blond
+-   Using the `pip` package manager:
+    ```bash
+    pip install blond
     ```
 
--   If this fails try to:
-
-    1.  Clone the repository from gitlab or download and extract the zip
-        from <https://gitlab.cern.ch/blond/BLonD/-/archive/master/BLonD-master.zip>
-    2.  Go to the downloaded BLonD directory and run:
-
-        ``` bash
-        $ python setup.py install
-        ```
-
--   If it still fails, go to the BLonD directory and run:
-
-    1.  
-        ``` bash
-        $ python setup.py compile
-        ```
-
-    2.  Then you have to set the PYTHONPATH variable to point to the
-        BLonD installation path.
-
--   In the occasion that it continues to fail, please open a new gitlab issue.
+### Installing BLonD manually (advanced users/ developers).
 
-### For advanced users or developers.
-
-1.  You are advised to install git in your system.
-2.  Clone the repository or download and extract it.
-3.  From within the BLonD directory run:
-    ``` bash
-    $ python blond/compile.py
+1.  Clone the repository (with `git`) or download and extract it.
+2.  (Optional) From within the BLonD directory run:
+    ```bash
+    python blond/compile.py
     ```
-4.  Adjust the PYTHONPATH to contain the path to the cloned repository.
+3. (Optional) See the complete list of the command line arguments with:
+    ```bash
+    python blond/compile.py --help
+    ```
+4.  Adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory.
 
 ## Confirm proper installation
 
--   Run the unittests with pytest (may need to be installed first with
-    pip install pytest):
-
+-   Run the unittests with `pytest` (the `pytest` package may need to be installed first):
     ``` bash
-    $ pytest -v unittests
+    pytest -v unittests
     ```
 
--   Try to run some of the main files found in the examples:
-
+-   Run some of the main files found in the `__EXAMPLES` directory:
     ``` bash
-    $ python __EXAMPLES/main_files/EX_01_Acceleration.py
-    $ python __EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
-    $ etc..
+    python __EXAMPLES/main_files/EX_01_Acceleration.py
+    python __EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+    etc..
     ```
 
-## Performace Optimizations
+# Performance Optimizations
+By default, if the C++ blond library has not been compiled, the python-only backend will be used to run the most time-consuming operations. 
 
-There are some easy ways to reduce the execution time of your
-simulation:
+To use the C++ backend and accelerate the execution of the time-consuming operations, follow the instructions provided in the section *Installing BLonD manually*.
 
-1.  Use the multi-threaded C library. To use it you have to add the -p
-    flag when compiling the C library:
+In addition you may want to:
+* Use the multi-threaded blond C++ backend:
     ``` bash
-    $ python blond/compile.py --parallel
+    python blond/compile.py --parallel
     ```
 
-2.  Enable processor specific compiler optimizations:
+* Enable processor specific compiler optimizations:
     ``` bash
-    $ python blond/compile.py --flags='-march=native'
+    python blond/compile.py --parallel --optimize
     ```
 
-3.  If you are test-case is calling the synchrotron radiation tracking method, you can accelerate it by using the Boost library. To do so you have to:  
+* If you are test-case is calling the synchrotron radiation tracking method, you can accelerate it by using the Boost library. To do so you have to:  
     1.  Download Boost: <https://www.boost.org/>. Let's say the version
         you downloaded is boost_1\_70.
     2.  Extract it, let's say in `/user/path/to/boost_1_70`.
     3.  Pass the boost installation path when compiling BLonD:
         ``` bash
-        $ python blond/compile.py --boost=/user/path/to/boost_1_7_70
+        python blond/compile.py --boost=/user/path/to/boost_1_7_70
         ```
 
-4.  Check the following section about the FFTW3 library.
+* Check the following section about the FFTW3 library.
 
-5.  *All the above can be combined.*
+* All the above can be combined, i.e.:
+    ```bash
+    python blond/compile.py --parallel --optimize --boost=...
+    ```
 
-## Changing the floating point precision (32 bit floats or 64 bit floats)
+## Changing the floating point number datatype
 
--   By default BLonD uses double precision calculations (float64). To
-    change to single precision, for faster calculations, in the
-    beginning of your mainfile you will have to add the code lines:
-    ``` python
-    from blond.utils import bmath as bm
-    bm.use_precision('single') 
-    ```
+By default BLonD uses double precision calculations (float64). To change to single precision for faster calculations, in the beginning of your mainfile you will have to add the following code lines:
+```python
+from blond.utils import bmath as bm
+bm.use_precision('single') 
+```
 
--   No other modifications are needed.
 
 ## Use the FFTW3 library for the FFTs
 
 So far only the `rfft()`, `irfft()` and `fftfreq()` routines are
 supported. `fft_convolve()` to be added soon.
 
 -   Windows:
@@ -307,21 +288,21 @@
     worker.finalize()
     ```
 
 6.  To run your script, you need to pass it to **mpirun** or
     **mpiexec**. To spawn P MPI processes run:
 
     ``` bash
-    $ mpirun -n P python main_file.py
+    mpirun -n P python main_file.py
     ```
 
 7.  For more examples have a look at the \_\_EXAMPLES/mpi_main_files/
     directory.
 
-# Using the GPU Implementation
+# Using the GPU backend
 
 ## Setup Instructions
 
 1.  Install **CUDA**: <https://developer.nvidia.com/cuda-downloads>
 2.  Install the **CuPy** library:
     <https://docs.cupy.dev/en/stable/install.html>
 3.  To verify your installation open a python terminal and execute the
@@ -329,68 +310,68 @@
 
     ``` python
     import cupy as cp 
     import numpy as np 
     a = cp.array(np.zeros(1000,np.float64)) 
     ```
 
-    To compile the Cuda files execute blond/compile.py and add the flag
+    To compile the CUDA files execute blond/compile.py and add the flag
     --gpu. The Compute Capability of your GPU will be automatically
     detected:
 
-``` bash
-$ python blond/compile.py --gpu 
-```
+    ``` bash
+    python blond/compile.py --gpu 
+    ```
 
 ## Changes required in the main file for GPU
 
 1.  Right before your main loop you need to add:
 
     ``` python
     from blond.utils import bmath as bm
     # change some of the basic functions to their GPU equivalent
     bm.use_gpu()
     ```
 
 2.  Also for every object you are using in your main loop that is in the
     following list:
 
-| GPU objects             |
-|-------------------------|
-| Beam                    |
-| Profile                 |
-| RingAndRFTracker        |
-| TotalInducedVoltage     |
-| InducedVoltageTime      |
-| InducedVoltageFreq      |
-| InductiveImpedance      |
-| InducedVoltageResonator |
-| RFStation               |
-| BeamFeedback            |
-
-you need to call their `to_gpu()` method. The following is a typical
-example from the \_\_EXAMPLES/gpu_main_files/EX_01_Acceleration.py
-mainfile.
-
-``` python
-# Define Objects
-beam = Beam(ring, N_p, N_b)
-profile = Profile(beam, CutOptions(n_slices=100), 
-             FitOptions(fit_option='gaussian'))
-# Initialize gpu
-beam.to_gpu()
-profile.to_gpu()
-```
+    | GPU objects             |
+    |-------------------------|
+    | Beam                    |
+    | Profile                 |
+    | RingAndRFTracker        |
+    | TotalInducedVoltage     |
+    | InducedVoltageTime      |
+    | InducedVoltageFreq      |
+    | InductiveImpedance      |
+    | InducedVoltageResonator |
+    | RFStation               |
+    | BeamFeedback            |
+
+    you need to call their `to_gpu()` method. The following is a typical
+    example from the \_\_EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+    mainfile.
+
+    ``` python
+    # Define Objects
+    beam = Beam(ring, N_p, N_b)
+    profile = Profile(beam, CutOptions(n_slices=100), 
+                FitOptions(fit_option='gaussian'))
+    # Initialize gpu
+    beam.to_gpu()
+    profile.to_gpu()
+    ```
 
-If an object of this list has a reference inside a different one you
-don't need to use the `to_gpu()` for the referenced object. In the
-previous example, we don't need to call `beam.to_gpu()` since `beam` is
-referenced inside the `profile`. The same would apply in a
-`TotalInducedVoltage` object and the objects in its
-`induced_voltage_list`.
+    If an object of this list has a reference inside a different one you
+    don't need to use the `to_gpu()` for the referenced object. In the
+    previous example, we don't need to call `beam.to_gpu()` since `beam` is
+    referenced inside the `profile`. The same would apply in a
+    `TotalInducedVoltage` object and the objects in its
+    `induced_voltage_list`.
 
 # Developers
 
 -   Simon Albright (simon.albright (at) cern.ch)
 -   Theodoros Argyropoulos (theodoros.argyropoulos (at) cern.ch)
 -   Konstantinos Iliakis (konstantinos.iliakis (at) cern.ch)
 -   Ivan Karpov (ivan.karpov (at) cern.ch)
```

### Comparing `blond-2.1.2/WARNINGS.txt` & `blond-2.1.3/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py` & `blond-2.1.3/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__BENCHMARKS/BM2_OTFB_no_beam.py` & `blond-2.1.3/__BENCHMARKS/BM2_OTFB_no_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__BENCHMARKS/BM3_OTFB_moving_average.py` & `blond-2.1.3/__BENCHMARKS/BM3_OTFB_moving_average.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__BENCHMARKS/BM4_OTFB_with_beam.py` & `blond-2.1.3/__BENCHMARKS/BM4_OTFB_with_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__BENCHMARKS/BM5_OTFB_feedforward.py` & `blond-2.1.3/__BENCHMARKS/BM5_OTFB_feedforward.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 No intensity effects
 
 :Authors: **Helga Timko**
 '''
 
 from __future__ import division, print_function
 import blond.utils.bmath as bm
-from blond.utils import input_parser
 from blond.plots.plot import Plot
 from blond.monitors.monitors import BunchMonitor
 from blond.beam.profile import CutOptions, Profile, FitOptions
 from blond.beam.distributions import bigaussian
 from blond.beam.beam import Beam, Proton
 from blond.trackers.utilities import total_voltage
 from blond.trackers.tracker import RingAndRFTracker
```

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_07_Ions.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py` & `blond-2.1.3/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt` & `blond-2.1.3/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/input_files/EX_02_Finemet.txt` & `blond-2.1.3/__EXAMPLES/input_files/EX_02_Finemet.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/input_files/EX_05_new_HQ_table.dat` & `blond-2.1.3/__EXAMPLES/input_files/EX_05_new_HQ_table.dat`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv` & `blond-2.1.3/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_01_Acceleration.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_03_RFnoise.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_04_Stationary_multistation.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_05_Wake_impedance.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_06_Preprocess.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_06_Preprocess.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_07_Ions.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_08_Phase_Loop.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_09_Radial_Loop.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_10_Fixed_frequency.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_14_sparse_slicing.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_14_sparse_slicing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_16_impedance_test.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_17_multi_turn_wake.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_17_multi_turn_wake.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_18_robinson_instability.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_19_bunch_generation.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_19_bunch_generation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_21_bunch_distribution.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_21_bunch_distribution.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py` & `blond-2.1.3/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_07_Ions.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_07_Ions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py` & `blond-2.1.3/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/Makefile` & `blond-2.1.3/__doc/Makefile`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/conf.py` & `blond-2.1.3/__doc/conf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/index.rst` & `blond-2.1.3/__doc/index.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/make.bat` & `blond-2.1.3/__doc/make.bat`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/ACS_cavity_loop.png` & `blond-2.1.3/__doc/modules/ACS_cavity_loop.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/ACS_cavity_loop.svg` & `blond-2.1.3/__doc/modules/ACS_cavity_loop.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/RF_noise.gle` & `blond-2.1.3/__doc/modules/RF_noise.gle`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/RF_noise.png` & `blond-2.1.3/__doc/modules/RF_noise.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/SPS_OTFB.png` & `blond-2.1.3/__doc/modules/SPS_OTFB.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/SPS_OTFB.svg` & `blond-2.1.3/__doc/modules/SPS_OTFB.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/beam.rst` & `blond-2.1.3/__doc/modules/beam.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/csr_impedance_real.png` & `blond-2.1.3/__doc/modules/csr_impedance_real.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/equations_of_motion.rst` & `blond-2.1.3/__doc/modules/equations_of_motion.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/impedances.rst` & `blond-2.1.3/__doc/modules/impedances.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/input_parameters.rst` & `blond-2.1.3/__doc/modules/input_parameters.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/lhc_cavity_loop.rst` & `blond-2.1.3/__doc/modules/lhc_cavity_loop.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/llrf.rst` & `blond-2.1.3/__doc/modules/llrf.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/plots.rst` & `blond-2.1.3/__doc/modules/plots.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/ring_and_RFstation.gle` & `blond-2.1.3/__doc/modules/ring_and_RFstation.gle`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/ring_and_RFstation.png` & `blond-2.1.3/__doc/modules/ring_and_RFstation.png`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/sps_cavity_loop.rst` & `blond-2.1.3/__doc/modules/sps_cavity_loop.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/toolbox.rst` & `blond-2.1.3/__doc/modules/toolbox.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/modules/utils.rst` & `blond-2.1.3/__doc/modules/utils.rst`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/breadcrumbs.html` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/footer.html` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout.html` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/layout_old.html` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/layout_old.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/search.html` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/static/js/theme.js` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/__doc/themes/sphinx_rtd_theme/versions.html` & `blond-2.1.3/__doc/themes/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/appveyor.yml` & `blond-2.1.3/appveyor.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/__init__.py` & `blond-2.1.3/blond/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             libblond_path = os.path.join(basepath, 'cpp_routines/libblond.dll')
         if hasattr(os, 'add_dll_directory'):
             os.add_dll_directory(os.path.dirname(libblond_path))
             libblond = ctypes.CDLL(libblond_path, winmode=0)
         else:
             libblond = ctypes.CDLL(libblond_path)
     else:
-        print('YOU DO NOT HAVE A WINDOWS OR LINUX OPERATING SYSTEM. ABORTING...')
+        print('YOU DO NOT HAVE A WINDOWS OR UNIX OPERATING SYSTEM. ABORTING...')
         sys.exit()
 except OSError as e:
     print("""
         Warning: The compiled blond library was not found.
-        You can safely ignore this warning if you are in 
-        the process of compiling the library.""")
+        The python routines will be used instead.
+        """)
```

### Comparing `blond-2.1.2/blond/beam/beam.py` & `blond-2.1.3/blond/beam/beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/beam/coasting_beam.py` & `blond-2.1.3/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/beam/distributions.py` & `blond-2.1.3/blond/beam/distributions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/beam/distributions_multibunch.py` & `blond-2.1.3/blond/beam/distributions_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/beam/profile.py` & `blond-2.1.3/blond/beam/profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/beam/sparse_histogram.cpp` & `blond-2.1.3/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/beam/sparse_slices.py` & `blond-2.1.3/blond/beam/sparse_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/compile.py` & `blond-2.1.3/blond/compile.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import subprocess
 import ctypes
 import argparse
 
 path = os.path.realpath(__file__)
 basepath = os.sep.join(path.split(os.sep)[:-1])
 
-parser = argparse.ArgumentParser(description='Run python setup_cpp.py to'
-                                             ' compile the cpp routines needed from BLonD')
+parser = argparse.ArgumentParser(description='Script used to compile the C++ (and CUDA) libraries needed by BLonD.',
+                                 epilog='All arguments can be controlled with the environment variable BLOND_COMPILE_OPTS. E.g.: BLOND_COMPILE_OPTS=\'-p,--flags=-O0 -g\'')
 
 parser.add_argument('-p', '--parallel',
                     default=False, action='store_true',
                     help='Produce Multi-threaded code. Use the environment'
                          ' variable OMP_NUM_THREADS=xx to control the number of'
                          ' threads that will be used.'
                          ' Default: Serial code')
@@ -111,55 +111,65 @@
 else:
     nvcc = 'nvcc'
 
 nvccflags = [nvcc, '--cubin', '-O3', '--use_fast_math', '-maxrregcount', '32']
 # nvccflags = ['nvcc', '--cubin', '-arch', 'sm_xx', '-O3', '--use_fast_math']
 
 if __name__ == "__main__":
-    args = parser.parse_args()
+    # Parse command line options
+    args = vars(parser.parse_args())
+
+    # Parse environment variable (BLOND_COMPILE_OPTS) options
+    env_args = {}
+    if 'BLOND_COMPILE_OPTS' in os.environ:
+        env_args_lst = os.environ['BLOND_COMPILE_OPTS'].split(',')
+        env_args = vars(parser.parse_args(env_args_lst))
+
+    args.update(env_args)
+
     boost_path = None
-    with_fftw = args.with_fftw or args.with_fftw_threads or args.with_fftw_omp or \
-        (args.with_fftw_lib is not None) or (args.with_fftw_header is not None)
-    if args.boost is not None:
-        if args.boost:
-            boost_path = os.path.abspath(args.boost)
+    with_fftw = args['with_fftw'] or args['with_fftw_threads'] or args['with_fftw_omp'] or \
+        (args['with_fftw_lib'] is not None) or (args['with_fftw_header'] is not None)
+    if args['boost'] is not None:
+        if args['boost']:
+            boost_path = os.path.abspath(args['boost'])
         else:
             boost_path = ''
         cflags += ['-I', boost_path, '-DBOOST']
-    compiler = args.compiler
+    compiler = args['compiler']
 
-    if args.libs:
-        libs = args.libs.split()
+    if args['libs']:
+        libs = args['libs'].split()
 
-    if args.parallel:
+    if args['parallel']:
         cflags += ['-fopenmp', '-DPARALLEL', '-D_GLIBCXX_PARALLEL']
 
-    if args.flags:
-        cflags += args.flags.split()
+    if args['flags']:
+        cflags += args['flags'].split()
 
     if with_fftw:
         cflags += ['-DUSEFFTW3']
-        if args.with_fftw_lib is not None:
-            libs += ['-L', args.with_fftw_lib]
-        if args.with_fftw_header is not None:
-            cflags += ['-I', args.with_fftw_header]
+        if args['with_fftw_lib'] is not None:
+            libs += ['-L', args['with_fftw_lib']]
+        if args['with_fftw_header'] is not None:
+            cflags += ['-I', args['with_fftw_header']]
         if 'win' in sys.platform:
             libs += ['-lfftw3-3']
         else:
             libs += ['-lfftw3', '-lfftw3f']
-            if args.with_fftw_omp:
+            if args['with_fftw_omp']:
                 cflags += ['-DFFTW3PARALLEL']
                 libs += ['-lfftw3_omp', '-lfftw3f_omp']
-            elif args.with_fftw_threads:
+            elif args['with_fftw_threads']:
                 cflags += ['-DFFTW3PARALLEL']
                 libs += ['-lfftw3_threads', '-lfftw3f_threads']
 
     if 'posix' in os.name:
         cflags += ['-fPIC']
-        if args.optimize:
+        if args['optimize']:
             # Check compiler defined directives
             # This is compatible with python3.6 - python 3.9
             # The universal_newlines argument transforms output to text (from binary)
             ret = subprocess.run([compiler + ' -march=native -dM -E - < /dev/null | egrep "SSE|AVX|FMA"'],
                                  shell=True, stdout=subprocess.PIPE, universal_newlines=True)
 
             # If we have an error
@@ -181,51 +191,53 @@
                 else:
                     cflags += ['-msse']
 
                 # Add FMA if supported
                 if 'FMA' in stdout:
                     cflags += ['-mfma']
 
-        root, ext = os.path.splitext(args.libname)
+        root, ext = os.path.splitext(args['libname'])
         if not ext:
             ext = '.so'
         libname = os.path.abspath(root + ext)
 
     elif 'win' in sys.platform:
-        root, ext = os.path.splitext(args.libname)
+        root, ext = os.path.splitext(args['libname'])
         if not ext:
             ext = '.dll'
         libname = os.path.abspath(root + ext)
 
         if hasattr(os, 'add_dll_directory'):
             directory, filename = os.path.split(libname)
             os.add_dll_directory(directory)
 
     else:
         print(
             'YOU ARE NOT USING A WINDOWS OR LINUX OPERATING SYSTEM. ABORTING...')
         sys.exit(-1)
     command = [compiler] + cflags + ['-o', libname] + cpp_files + libs
 
-    print('Enable Multi-threaded code: ', args.parallel)
-    print('Using boost: ', args.boost is not None)
-    if args.boost is not None:
+    print('Enable Multi-threaded code: ', args['parallel'])
+    print('Use boost: ', args['boost'] is not None)
+    if args['boost'] is not None:
         print('Boost installation path: ', boost_path)
-    print('With FFTW3: ', with_fftw)
+    print('Link with FFTW3: ', with_fftw)
     if with_fftw:
-        print('Parallel FFTW3:', args.with_fftw_threads or args.with_fftw_omp)
-    if args.with_fftw_lib or args.with_fftw_header:
-        print('FFTW3 Library path: ', args.with_fftw_lib)
-        print('FFTW3 Headers path: ', args.with_fftw_header)
+        print('Parallel FFTW3:', args['with_fftw_threads'] or args['with_fftw_omp'])
+    if args['with_fftw_lib'] or args['with_fftw_header']:
+        print('FFTW3 Library path: ', args['with_fftw_lib'])
+        print('FFTW3 Headers path: ', args['with_fftw_header'])
     print('C++ Compiler: ', compiler)
-    print('Compiler version: ')
-    subprocess.run([compiler, '--version'])
+    compiler_version = subprocess.run(
+        [compiler, '--version'], capture_output=True).stdout.decode().split('\n')[0]
+    print('Compiler version: ', compiler_version)
+    
     print('Compiler flags: ', ' '.join(cflags))
     print('Extra libraries: ', ' '.join(libs))
-    print('Library name: ', libname)
+    print('Compiled library name: ', libname)
 
     # If it exists already, remove the library before re-compiling
     if os.path.isfile(libname):
         try:
             os.remove(libname)
         except OSError as e:
             pass
@@ -242,27 +254,27 @@
                 libblond = ctypes.CDLL(libname)
             print('\nThe blond library has been successfully compiled.')
         except Exception as e:
             print('\nCompilation failed.')
             print(e)
 
     # Compile the GPU library
-    if args.gpu:
+    if args['gpu']:
         print('\n'+''.join(['=']*80))
         print('\nCompiling the CUDA library')
-        if args.gpu == 'discover':
+        if args['gpu'] == 'discover':
             print('Discovering the device compute capability..')
             import cupy as cp
 
             dev = cp.cuda.Device(0)
             dev_name = cp.cuda.runtime.getDeviceProperties(dev)['name']
             comp_capability = dev.compute_capability
             print('Device name {}'.format(dev_name))
-        elif args.gpu is not None:
-            comp_capability = args.gpu
+        elif args['gpu'] is not None:
+            comp_capability = args['gpu']
 
         print('Compiling the CUDA library for architecture {}.'.format(comp_capability))
         # Add the -arch required argument
         nvccflags += ['-arch', 'sm_{}'.format(comp_capability)]
         libname_double = os.path.join(basepath,
                                       'gpu/cuda_kernels/kernels_double_sm_{}.cubin'.format(comp_capability))
         libname_single = os.path.join(basepath,
```

### Comparing `blond-2.1.2/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.3/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/blondmath.cpp` & `blond-2.1.3/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/blondmath.h` & `blond-2.1.3/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/cos.h` & `blond-2.1.3/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/drift.cpp` & `blond-2.1.3/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/exp.h` & `blond-2.1.3/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.3/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/fft.cpp` & `blond-2.1.3/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/fft.h` & `blond-2.1.3/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/histogram.cpp` & `blond-2.1.3/blond/cpp_routines/histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/kick.cpp` & `blond-2.1.3/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/libblond.so` & `blond-2.1.3/blond/cpp_routines/libblond.so`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.3/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/music_track.cpp` & `blond-2.1.3/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/sin.h` & `blond-2.1.3/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/sincos.h` & `blond-2.1.3/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.3/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.3/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.3/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/gpu/cupy_butils_wrap.py` & `blond-2.1.3/blond/gpu/butils_wrap_cupy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import cupy as cp
-from ..utils import bmath as bm
+from ..utils import precision, gpu_dev
 
-grid_size, block_size = bm.gpuDev().grid_size, bm.gpuDev().block_size
-kernels = bm.gpuDev().mod
+grid_size, block_size = gpu_dev.grid_size, gpu_dev.block_size
+kernels = gpu_dev.mod
 
 # Load all required CUDA kernels
 rf_volt_comp_kernel = kernels.get_function("rf_volt_comp")
 kick_kernel = kernels.get_function("simple_kick")
 drift_kernel = kernels.get_function("drift")
 gm_linear_interp_kick_help = kernels.get_function("lik_only_gm_copy")
 gm_linear_interp_kick_comp = kernels.get_function("lik_only_gm_comp")
@@ -15,44 +15,44 @@
 hybrid_histogram = kernels.get_function("hybrid_histogram")
 sm_histogram = kernels.get_function("sm_histogram")
 synch_rad = kernels.get_function("synchrotron_radiation")
 synch_rad_full = kernels.get_function("synchrotron_radiation_full")
 
 
 def rf_volt_comp(voltage, omega_rf, phi_rf, bin_centers):
-    assert voltage.dtype == bm.precision.real_t
-    assert omega_rf.dtype == bm.precision.real_t
-    assert phi_rf.dtype == bm.precision.real_t
-    assert bin_centers.dtype == bm.precision.real_t
+    assert voltage.dtype == precision.real_t
+    assert omega_rf.dtype == precision.real_t
+    assert phi_rf.dtype == precision.real_t
+    assert bin_centers.dtype == precision.real_t
 
-    rf_voltage = cp.zeros(bin_centers.size, bm.precision.real_t)
+    rf_voltage = cp.zeros(bin_centers.size, precision.real_t)
 
     rf_volt_comp_kernel(args=(voltage, omega_rf, phi_rf, bin_centers,
               np.int32(voltage.size), np.int32(bin_centers.size), rf_voltage),
         block=block_size, grid=grid_size)
     return rf_voltage
 
 
 def kick(dt, dE, voltage, omega_rf, phi_rf, charge, n_rf, acceleration_kick):
-    assert dt.dtype == bm.precision.real_t
-    assert dE.dtype == bm.precision.real_t
-    assert omega_rf.dtype == bm.precision.real_t
-    assert phi_rf.dtype == bm.precision.real_t
+    assert dt.dtype == precision.real_t
+    assert dE.dtype == precision.real_t
+    assert omega_rf.dtype == precision.real_t
+    assert phi_rf.dtype == precision.real_t
 
-    voltage_kick = cp.empty(voltage.size, bm.precision.real_t)
+    voltage_kick = cp.empty(voltage.size, precision.real_t)
     voltage_kick = charge * voltage
 
     kick_kernel(args=(dt,
                       dE,
                       np.int32(n_rf),
                       voltage_kick,
                       omega_rf,
                       phi_rf,
                       np.int32(dt.size),
-                      bm.precision.real_t(acceleration_kick)),
+                      precision.real_t(acceleration_kick)),
                 block=block_size, grid=grid_size)  
 
 
 def drift(dt, dE, solver, t_rev, length_ratio, alpha_order, eta_0,
               eta_1, eta_2, alpha_0, alpha_1, alpha_2, beta, energy):
 
     solver = solver.decode('utf-8')
@@ -66,155 +66,155 @@
 
     if not isinstance(t_rev, float):
         t_rev = float(t_rev)
 
     drift_kernel(args=(dt,
                 dE,
                 solver,
-                bm.precision.real_t(t_rev), bm.precision.real_t(length_ratio),
-                bm.precision.real_t(alpha_order), bm.precision.real_t(eta_0),
-                bm.precision.real_t(eta_1), bm.precision.real_t(eta_2),
-                bm.precision.real_t(alpha_0), bm.precision.real_t(alpha_1),
-                bm.precision.real_t(alpha_2),
-                bm.precision.real_t(beta), bm.precision.real_t(energy),
+                precision.real_t(t_rev), precision.real_t(length_ratio),
+                precision.real_t(alpha_order), precision.real_t(eta_0),
+                precision.real_t(eta_1), precision.real_t(eta_2),
+                precision.real_t(alpha_0), precision.real_t(alpha_1),
+                precision.real_t(alpha_2),
+                precision.real_t(beta), precision.real_t(energy),
                 np.int32(dt.size)),
           block=block_size, grid=grid_size)
 
 
 def linear_interp_kick(dt, dE, voltage,
                            bin_centers, charge,
                            acceleration_kick):
-    assert dt.dtype == bm.precision.real_t
-    assert dE.dtype == bm.precision.real_t
-    assert voltage.dtype == bm.precision.real_t
-    assert bin_centers.dtype == bm.precision.real_t
+    assert dt.dtype == precision.real_t
+    assert dE.dtype == precision.real_t
+    assert voltage.dtype == precision.real_t
+    assert bin_centers.dtype == precision.real_t
 
     macros = dt.size
     slices = bin_centers.size
 
     
-    glob_vkick_factor = cp.empty(2*(slices - 1), bm.precision.real_t)
+    glob_vkick_factor = cp.empty(2*(slices - 1), precision.real_t)
     gm_linear_interp_kick_help(args=(dt,
                                      dE,
                                      voltage,
                                      bin_centers,
-                                     bm.precision.real_t(charge),
+                                     precision.real_t(charge),
                                      np.int32(slices),
                                      np.int32(macros),
-                                     bm.precision.real_t(acceleration_kick),
+                                     precision.real_t(acceleration_kick),
                                      glob_vkick_factor),
                                grid=grid_size, block=block_size)
 
     gm_linear_interp_kick_comp(args=(dt,
                                      dE,
                                      voltage,
                                      bin_centers,
-                                     bm.precision.real_t(charge),
+                                     precision.real_t(charge),
                                      np.int32(slices),
                                      np.int32(macros),
-                                     bm.precision.real_t(acceleration_kick),
+                                     precision.real_t(acceleration_kick),
                                      glob_vkick_factor),
                                grid=grid_size, block=block_size)
 
 
 def linear_interp_kick_drift(dt, dE, total_voltage, bin_centers, charge, acc_kick,
                                 t_rev, length_ratio, alpha_order, eta_0, beta, energy):
-    assert dt.dtype == bm.precision.real_t
-    assert dE.dtype == bm.precision.real_t
-    assert total_voltage.dtype == bm.precision.real_t
-    assert bin_centers.dtype == bm.precision.real_t
+    assert dt.dtype == precision.real_t
+    assert dE.dtype == precision.real_t
+    assert total_voltage.dtype == precision.real_t
+    assert bin_centers.dtype == precision.real_t
     
 
     macros = dt.size
     slices = bin_centers.size
 
-    glob_vkick_factor = cp.empty(2*(slices - 1), bm.precision.real_t)
+    glob_vkick_factor = cp.empty(2*(slices - 1), precision.real_t)
 
     gm_linear_interp_kick_help(args=(dt,
                                      dE,
                                      total_voltage,
                                      bin_centers,
-                                     bm.precision.real_t(charge),
+                                     precision.real_t(charge),
                                      np.int32(slices),
                                      np.int32(macros),
-                                     bm.precision.real_t(acc_kick),
+                                     precision.real_t(acc_kick),
                                      glob_vkick_factor),
                                grid=grid_size, block=block_size)
     gm_linear_interp_kick_drift_comp(args=(dt,
                                            dE,
                                            total_voltage,
                                            bin_centers,
-                                           bm.precision.real_t(charge),
+                                           precision.real_t(charge),
                                            np.int32(slices),
                                            np.int32(macros),
-                                           bm.precision.real_t(acc_kick),
+                                           precision.real_t(acc_kick),
                                            glob_vkick_factor,
-                                           bm.precision.real_t(t_rev),
-                                           bm.precision.real_t(length_ratio),
-                                           bm.precision.real_t(eta_0),
-                                           bm.precision.real_t(beta),
-                                           bm.precision.real_t(energy)),
+                                           precision.real_t(t_rev),
+                                           precision.real_t(length_ratio),
+                                           precision.real_t(eta_0),
+                                           precision.real_t(beta),
+                                           precision.real_t(energy)),
                                      grid=grid_size, block=block_size)
 
 
 def slice(dt, profile, cut_left, cut_right):
 
-    assert dt.dtype == bm.precision.real_t
+    assert dt.dtype == precision.real_t
     
     n_slices = profile.size
     profile.fill(0)
 
     if not isinstance(cut_left, float):
         cut_left = float(cut_left)
     if not isinstance(cut_right, float):
         cut_right = float(cut_right)
 
-    if 4*n_slices < bm.gpuDev().attributes['MaxSharedMemoryPerBlock']:
-        sm_histogram(args=(dt, profile, bm.precision.real_t(cut_left),
-                           bm.precision.real_t(cut_right), np.uint32(n_slices),
+    if 4*n_slices < gpu_dev.attributes['MaxSharedMemoryPerBlock']:
+        sm_histogram(args=(dt, profile, precision.real_t(cut_left),
+                           precision.real_t(cut_right), np.uint32(n_slices),
                            np.uint32(dt.size)),
                      grid=grid_size, block=block_size, shared_mem=4*n_slices)
     else:
-        hybrid_histogram(args=(dt, profile, bm.precision.real_t(cut_left),
-                               bm.precision.real_t(cut_right), np.uint32(n_slices),
+        hybrid_histogram(args=(dt, profile, precision.real_t(cut_left),
+                               precision.real_t(cut_right), np.uint32(n_slices),
                                np.uint32(dt.size), np.int32(
-            bm.gpuDev().attributes['MaxSharedMemoryPerBlock']/4)),
+            gpu_dev.attributes['MaxSharedMemoryPerBlock']/4)),
             grid=grid_size, block=block_size,
-            shared_mem=bm.gpuDev().attributes['MaxSharedMemoryPerBlock'])
+            shared_mem=gpu_dev.attributes['MaxSharedMemoryPerBlock'])
 
 
 def synchrotron_radiation(dE, U0, n_kicks, tau_z):
-    assert dE.dtype == bm.precision.real_t
+    assert dE.dtype == precision.real_t
    
-    synch_rad(args=(dE, bm.precision.real_t(U0/n_kicks), np.int32(dE.size),
-                    bm.precision.real_t(tau_z * n_kicks),
+    synch_rad(args=(dE, precision.real_t(U0/n_kicks), np.int32(dE.size),
+                    precision.real_t(tau_z * n_kicks),
                     np.int32(n_kicks)),
               block=block_size, grid=grid_size)
 
 
 def synchrotron_radiation_full(dE, U0, n_kicks, tau_z, sigma_dE, energy):
-    assert dE.dtype == bm.precision.real_t
+    assert dE.dtype == precision.real_t
     
-    synch_rad_full(args=(dE, bm.precision.real_t(U0/n_kicks), np.int32(dE.size),
-                         bm.precision.real_t(sigma_dE),
-                         bm.precision.real_t(tau_z * n_kicks),
-                         bm.precision.real_t(energy), np.int32(n_kicks)),
+    synch_rad_full(args=(dE, precision.real_t(U0/n_kicks), np.int32(dE.size),
+                         precision.real_t(sigma_dE),
+                         precision.real_t(tau_z * n_kicks),
+                         precision.real_t(energy), np.int32(n_kicks)),
                    block=block_size, grid=grid_size)
 
 
 @cp.fuse(kernel_name='beam_phase_helper')
 def __beam_phase_helper(bin_centers, profile, alpha, omega_rf, phi_rf):
     base = cp.exp(alpha * bin_centers) * profile
     a = omega_rf * bin_centers + phi_rf
     return base * cp.sin(a), base * cp.cos(a)
 
 
 def beam_phase(bin_centers, profile, alpha, omega_rf, phi_rf, bin_size):
-    assert bin_centers.dtype == bm.precision.real_t
-    assert profile.dtype == bm.precision.real_t
+    assert bin_centers.dtype == precision.real_t
+    assert profile.dtype == precision.real_t
 
     array1, array2 = __beam_phase_helper(
         bin_centers, profile, alpha, omega_rf, phi_rf)
     # due to the division, the bin_size is not needed
     scoeff = cp.trapz(array1, dx=1)
     ccoeff = cp.trapz(array2, dx=1)
 
@@ -224,16 +224,16 @@
 @cp.fuse(kernel_name='beam_phase_fast_helper')
 def __beam_phase_fast_helper(bin_centers, profile, omega_rf, phi_rf):
     a = omega_rf * bin_centers + phi_rf
     return profile * cp.sin(a), profile * cp.cos(a)
 
 
 def beam_phase_fast(bin_centers, profile, omega_rf, phi_rf, bin_size):
-    assert bin_centers.dtype == bm.precision.real_t
-    assert profile.dtype == bm.precision.real_t
+    assert bin_centers.dtype == precision.real_t
+    assert profile.dtype == precision.real_t
 
     array1, array2 = __beam_phase_fast_helper(
         bin_centers, profile, omega_rf, phi_rf)
     # due to the division, the bin_size is not needed
     scoeff = cp.trapz(array1, dx=1)
     ccoeff = cp.trapz(array2, dx=1)
 
@@ -244,28 +244,28 @@
 
 # def convolve(signal, kernel, mode='full', result=None):
 #     if mode != 'full':
 #         # ConvolutionError
 #         raise RuntimeError('[convolve] Only full mode is supported')
 #     if result is None:
 #         result = cp.empty(len(signal) + len(kernel) - 1,
-#                           dtype=bm.precision.real_t)
+#                           dtype=precision.real_t)
 #     result = bm.irfft(bm.rfft(signal) * bm.rfft(kernel))
 #     return result
 
 
 # def interp(x, xp, yp, left=None, right=None, result=None):
 #     cuinterp = kernels.get_function("cuinterp")
 
 #     if not left:
 #         left = yp[0]
 #     if not right:
 #         right = yp[-1]
 #     if result is None:
-#         result = cp.empty(x.size, bm.precision.real_t)
+#         result = cp.empty(x.size, precision.real_t)
 
 #     cuinterp(args=(x, np.int32(x.size),
 #                    xp, np.int32(xp.size),
 #                    yp, result,
-#                    bm.precision.real_t(left), bm.precision.real_t(right)),
+#                    precision.real_t(left), precision.real_t(right)),
 #              block=block_size, grid=grid_size)
 #     return result
```

### Comparing `blond-2.1.2/blond/impedances/impedance.py` & `blond-2.1.3/blond/impedances/impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/impedances/impedance_sources.py` & `blond-2.1.3/blond/impedances/impedance_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,15 +481,15 @@
 
         self.time_array = time_array
         self.wake = np.zeros(self.time_array.shape, dtype=bm.precision.real_t, order='C')
         self.wake = np.zeros(self.time_array.shape)
 
         for i in range(0, self.n_twc):
             a_tilde = self.a_factor[i] / (2 * np.pi)
-            indexes = np.where(self.time_array <= a_tilde)
+            indexes = self.time_array <= a_tilde
             self.wake[indexes] += ((np.sign(self.time_array[indexes]) + 1) * 2
                                    * self.R_S[i] / a_tilde
                                    * (1 - self.time_array[indexes] / a_tilde)
                                    * bm.cos(2 * np.pi * self.frequency_R[i] *
                                           self.time_array[indexes]))
 
     def imped_calc(self, frequency_array):
@@ -861,15 +861,15 @@
 
         self.impedance = np.zeros_like(n_array, dtype=complex)
 
         # parallel plates cut-off frequency in units of f_0
         n_cut = np.sqrt(2/3) * (np.pi / self.Delta)**1.5
 
         # use approximate equation for frequencies above high_frequency_transition * n_cut
-        approx_indexes = bm.where_cpp(n_array, more_than=high_frequency_transition * n_cut)
+        approx_indexes = n_array > (high_frequency_transition * n_cut)
         if np.count_nonzero(approx_indexes) > 0:
             self.impedance[approx_indexes] = self._fs_low_frequency(frequency_array[approx_indexes])
 
         # use exact result for all other frequencies (and ignore f=0)
         exact_indexes = np.invert(approx_indexes) * n_array!=0
 
         # if there is nothing to calculate, we are done ...
@@ -1089,20 +1089,22 @@
             raise ValueError('epsilon must be a small positive value')
 
         self.impedance = np.zeros_like(frequency_array, dtype=complex)
 
         l_array = frequency_array / self.f_crit
 
         # use the low frequency approximation where f < LFT * f_c
-        low_indexes = bm.where_cpp(l_array, less_than=low_frequency_transition)
+        # low_indexes = np.where(l_array < low_frequency_transition)[0]
+        low_indexes = l_array < low_frequency_transition
         if np.count_nonzero(low_indexes) > 0:
             self.impedance[low_indexes] = self._fs_low_frequency(frequency_array[low_indexes])
 
         # use the high frequency approximation where f > HFT * f_c
-        high_indexes = bm.where_cpp(l_array, more_than=high_frequency_transition)
+        # high_indexes = np.where(l_array > high_frequency_transition)[0]
+        high_indexes = l_array > high_frequency_transition
         if np.count_nonzero(high_indexes) > 0:
             self.impedance[high_indexes] = self._fs_high_frequency(frequency_array[high_indexes])
 
         # use full integration for frequencies inbetween
         exact_indexes = np.invert(low_indexes + high_indexes)
         if np.count_nonzero(exact_indexes) == 0:
             return
```

### Comparing `blond-2.1.2/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.3/blond/impedances/induced_voltage_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/impedances/music.py` & `blond-2.1.3/blond/impedances/music.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/input_parameters/rf_parameters.py` & `blond-2.1.3/blond/input_parameters/rf_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.3/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/input_parameters/ring.py` & `blond-2.1.3/blond/input_parameters/ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/input_parameters/ring_options.py` & `blond-2.1.3/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/beam_feedback.py` & `blond-2.1.3/blond/llrf/beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/cavity_feedback.py` & `blond-2.1.3/blond/llrf/cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/impulse_response.py` & `blond-2.1.3/blond/llrf/impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/notch_filter.py` & `blond-2.1.3/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/offset_frequency.py` & `blond-2.1.3/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/rf_modulation.py` & `blond-2.1.3/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/rf_noise.py` & `blond-2.1.3/blond/llrf/rf_noise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/llrf/signal_processing.py` & `blond-2.1.3/blond/llrf/signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/monitors/monitors.py` & `blond-2.1.3/blond/monitors/monitors.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/plots/plot.py` & `blond-2.1.3/blond/plots/plot.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/plots/plot_beams.py` & `blond-2.1.3/blond/plots/plot_beams.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/plots/plot_impedance.py` & `blond-2.1.3/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/plots/plot_llrf.py` & `blond-2.1.3/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/plots/plot_parameters.py` & `blond-2.1.3/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/plots/plot_slices.py` & `blond-2.1.3/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/sanity_check.py` & `blond-2.1.3/blond/sanity_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.3/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/action.py` & `blond-2.1.3/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/diffusion.py` & `blond-2.1.3/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/filters_and_fitting.py` & `blond-2.1.3/blond/toolbox/filters_and_fitting.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/logger.py` & `blond-2.1.3/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/next_regular.py` & `blond-2.1.3/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/parameter_scaling.py` & `blond-2.1.3/blond/toolbox/parameter_scaling.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/tomoscope.cpp` & `blond-2.1.3/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/toolbox/tomoscope.py` & `blond-2.1.3/blond/toolbox/tomoscope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2016 CERN. This software is distributed under the
-# terms of the GNU General Public License version 3 (GPL Version 3), 
+# terms of the GNU General Public License version 3 (GPL Version 3),
 # copied verbatim in the file LICENSE.md.
-# In applying this license, CERN does not waive the privileges and immunities 
+# In applying this license, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 ** CERN Tomoscope-related functions to generate particle distribution or 
 probability density.**
@@ -15,103 +15,106 @@
 
 
 from __future__ import division
 from __future__ import print_function
 from builtins import str
 import numpy as np
 import h5py as hp
-import os, linecache, ctypes
+import os
+import linecache
+import ctypes
 from matplotlib import pyplot as plt
 import matplotlib.cm as cm
-# from ..setup_cpp import libblond
-from .. import libblond
+from ..utils import bmath as bm
 
 
-
-def distribution_from_tomoscope_data(dataDir, nPart, cutoff = 1000, seed = 1234,
-                                     plotFig = True, saveDistr = False):
-     
+def distribution_from_tomoscope_data(dataDir, nPart, cutoff=1000, seed=1234,
+                                     plotFig=True, saveDistr=False):
     '''
     'dataDir' is the directory of *directories* of offline-processed tomoscope 
     data containing 'plotinfo.data' and 'image001.data'
     Use 'cutoff' to eliminate measurement noise (use values around 50-100).
     Use 'seed' to change the random number seed.
     Use 'plotFig = True' to plot and save figures.
     Use 'saveDistr = True' to save particle coordinates.    
     '''
-    
+
     # Directory in which plots will be stored
-    distrDir = dataDir + '\\Distributions_' + str(nPart) + 'particles_cutoff' + str(cutoff)
+    distrDir = dataDir + '\\Distributions_' + \
+        str(nPart) + 'particles_cutoff' + str(cutoff)
     # Try to create directory
     try:
         os.makedirs(distrDir)
     # Check whether already exists/creation failed
     except OSError:
         if os.path.exists(distrDir):
             pass
         else:
             raise
-        
+
     # Loop over directories to be analysed
     for directory in os.listdir(dataDir):
-        
+
         if 'Distributions' not in directory:
-        
-            print("Analysing data of directory %s" %directory)
-            
+
+            print("Analysing data of directory %s" % directory)
+
             # Read tomoscope settings
-            plotInfo = dataDir+'\\'+directory+'\plotinfo.data'       
+            plotInfo = dataDir+'\\'+directory+'\plotinfo.data'
             profLen = np.uint(linecache.getline(plotInfo, 4)[17:-1])
             dtBin = np.double(linecache.getline(plotInfo, 6)[9:-1])
             dEBin = np.double(linecache.getline(plotInfo, 8)[9:-1])
             x0 = np.double(linecache.getline(plotInfo, 12)[8:-1])
             y0 = np.double(linecache.getline(plotInfo, 13)[8:-1])
-            
+
             # Read probability density from file
-            probDistr = np.loadtxt(dataDir+'\\'+directory+'\image001.data', 
+            probDistr = np.loadtxt(dataDir+'\\'+directory+'\image001.data',
                                    dtype=np.double, unpack=True)
             probDistr = np.ascontiguousarray(probDistr)
-            
+
             # Reconstruct particle distribution from probability distribution
             dt = np.empty(nPart)
             dE = np.empty(nPart)
-            
-            libblond.generate_distribution(dt.ctypes.data_as(ctypes.c_void_p), 
-                                         dE.ctypes.data_as(ctypes.c_void_p), 
-                                         probDistr.ctypes.data_as(ctypes.c_void_p), 
-                                         ctypes.c_uint(seed), ctypes.c_uint(profLen), 
-                                         ctypes.c_double(cutoff), ctypes.c_double(x0), 
-                                         ctypes.c_double(y0), ctypes.c_double(dtBin), 
-                                         ctypes.c_double(dEBin), ctypes.c_uint(nPart))
-        
+
+            bm.distribution_from_tomoscope(dt, dE, probDistr, seed, profLen,
+                                           cutoff, x0, y0, dtBin, dEBin)
+
+            # libblond.generate_distribution(dt.ctypes.data_as(ctypes.c_void_p),
+            #                              dE.ctypes.data_as(ctypes.c_void_p),
+            #                              probDistr.ctypes.data_as(ctypes.c_void_p),
+            #                              ctypes.c_uint(seed), ctypes.c_uint(profLen),
+            #                              ctypes.c_double(cutoff), ctypes.c_double(x0),
+            #                              ctypes.c_double(y0), ctypes.c_double(dtBin),
+            #                              ctypes.c_double(dEBin), ctypes.c_uint(nPart))
+
             if plotFig == True:
-                
-                # Settings for plots 
+
+                # Settings for plots
                 plt.rc('axes', labelsize=14, labelweight='normal')
                 plt.rc('lines', linewidth=1.5, markersize=6)
-                plt.rc('font', family='sans-serif')  
-                plt.rc('legend', fontsize=12)  
-            
+                plt.rc('font', family='sans-serif')
+                plt.rc('legend', fontsize=12)
+
                 # Plot distribution
                 plt.hist2d(dt, dE, (profLen, profLen), cmap=cm.jet)
                 plt.colorbar()
                 plt.xlabel('Time offset [s]')
                 plt.ylabel('Energy offset [eV]')
                 plt.savefig(distrDir + '\\' + directory + '.png')
                 plt.clf()
-            
+
             if saveDistr == True:
-                
+
                 h5File = hp.File(distrDir + '\\' + directory + '.h5', 'w')
-                
-                # Create group  
+
+                # Create group
                 h5File.require_group('Beam')
                 h5Group = h5File['Beam']
-                
+
                 # Create & write datasets
-                h5Group.create_dataset("dt", shape = (nPart,), dtype = 'f', 
-                                       compression = "gzip", compression_opts = 9)
+                h5Group.create_dataset("dt", shape=(nPart,), dtype='f',
+                                       compression="gzip", compression_opts=9)
                 h5Group["dt"][:] = dt
-                h5Group.create_dataset("dE", shape = (nPart,), dtype = 'f', 
-                                       compression = "gzip", compression_opts = 9)
+                h5Group.create_dataset("dE", shape=(nPart,), dtype='f',
+                                       compression="gzip", compression_opts=9)
                 h5Group["dE"][:] = dE
                 h5File.close()
```

### Comparing `blond-2.1.2/blond/trackers/tracker.py` & `blond-2.1.3/blond/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/trackers/utilities.py` & `blond-2.1.3/blond/trackers/utilities.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/utils/bmath.py` & `blond-2.1.3/blond/utils/bmath.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,266 @@
 '''
 BLonD math and physics core functions
 
-@author Stefan Hegglin, Konstantinos Iliakis, Panagiotis Tsapatsaris
+@author Stefan Hegglin, Konstantinos Iliakis, Panagiotis Tsapatsaris, Georgios Typaldos
 @date 20.10.2017
 '''
+
 # from functools import wraps
 import os
 
 import numpy as np
-from ..utils import butils_wrap
-# from ..utils import bphysics_wrap
+from ..utils import butils_wrap_cpp as _cpp
+from ..utils import butils_wrap_python as _py
+from . import precision
+from . import gpu_dev
 
-precision = butils_wrap.precision
+# Global variables
 __exec_mode = 'single_node'
 # Other modes: multi_node
 
-__gpu_dev = None
+def use_cpp():
+    '''
+    Replace all python functions by there equivalent in cpp
+    '''
+
+    # dictionary storing the CPP versions of the most compute intensive functions #
+    CPP_func_dict = {
+        'rfft': np.fft.rfft,
+        'irfft': np.fft.irfft,
+        'rfftfreq': np.fft.rfftfreq,
+
+        'kick': _cpp.kick,
+        'rf_volt_comp': _cpp.rf_volt_comp,
+        'drift': _cpp.drift,
+        'slice': _cpp.slice,
+        'slice_smooth': _cpp.slice_smooth,
+        'linear_interp_kick': _cpp.linear_interp_kick,
+        'synchrotron_radiation': _cpp.synchrotron_radiation,
+        'synchrotron_radiation_full': _cpp.synchrotron_radiation_full,
+        'music_track': _cpp.music_track,
+        'music_track_multiturn': _cpp.music_track_multiturn,
+        'fast_resonator': _cpp.fast_resonator,
+        'beam_phase': _cpp.beam_phase,
+        'beam_phase_fast': _cpp.beam_phase_fast,
+        'sparse_histogram': _cpp.sparse_histogram,
+        'distribution_from_tomoscope': _cpp.distribution_from_tomoscope,
+        'set_random_seed': _cpp.set_random_seed,
+
+        'sin_cpp': _cpp.sin_cpp,
+        'cos_cpp': _cpp.cos_cpp,
+        'exp_cpp': _cpp.exp_cpp,
+        'mean_cpp': _cpp.mean_cpp,
+        'std_cpp': _cpp.std_cpp,
+        'where_cpp': _cpp.where_cpp,
+        'interp_cpp': np.interp,
+        # 'interp_cpp': _cpp.interp_cpp,
+        # 'interp_const_space': _cpp.interp_const_space,
+        'interp_const_space': np.interp,
+        'cumtrapz': _cpp.cumtrapz,
+        'trapz_cpp': _cpp.trapz_cpp,
+        'linspace_cpp': _cpp.linspace_cpp,
+        'argmin_cpp': _cpp.argmin_cpp,
+        'argmax_cpp': _cpp.argmax_cpp,
+        'convolve': _cpp.convolve,
+        'arange_cpp': _cpp.arange_cpp,
+        'sum_cpp': _cpp.sum_cpp,
+        'sort_cpp': _cpp.sort_cpp,
+        'add_cpp': _cpp.add_cpp,
+        'mul_cpp': _cpp.mul_cpp,
+
+        'device': 'CPU_CPP'
+    }
+
+    # add numpy functions in the dictionary
+    for fname in dir(np):
+        if callable(getattr(np, fname)) and (fname not in CPP_func_dict) \
+                and (fname[0] != '_'):
+            CPP_func_dict[fname] = getattr(np, fname)
+
+    # add basic numpy modules to dictionary as they are not callable
+    CPP_func_dict['random'] = getattr(np, 'random')
+    CPP_func_dict['fft'] = getattr(np, 'fft')
+
+    __update_active_dict(CPP_func_dict)
 
-# dictionary storing the CPU versions of the desired functions #
-_CPU_func_dict = {
-    'rfft': np.fft.rfft,
-    'irfft': np.fft.irfft,
-    'rfftfreq': np.fft.rfftfreq,
-    'irfft_packed': butils_wrap.irfft_packed,
-    'sin_cpp': butils_wrap.sin_cpp,
-    'cos_cpp': butils_wrap.cos_cpp,
-    'exp_cpp': butils_wrap.exp_cpp,
-    'mean_cpp': butils_wrap.mean_cpp,
-    'std_cpp': butils_wrap.std_cpp,
-    'where_cpp': butils_wrap.where_cpp,
-    'interp_cpp': np.interp,
-    # 'interp_cpp': butils_wrap.interp_cpp,
-    # 'interp_const_space': butils_wrap.interp_const_space,
-    'interp_const_space': np.interp,
-    'cumtrapz': butils_wrap.cumtrapz,
-    'trapz_cpp': butils_wrap.trapz_cpp,
-    'linspace_cpp': butils_wrap.linspace_cpp,
-    'argmin_cpp': butils_wrap.argmin_cpp,
-    'argmax_cpp': butils_wrap.argmax_cpp,
-    'convolve': butils_wrap.convolve,
-    'arange_cpp': butils_wrap.arange_cpp,
-    'sum_cpp': butils_wrap.sum_cpp,
-    'sort_cpp': butils_wrap.sort_cpp,
-    'add_cpp': butils_wrap.add_cpp,
-    'mul_cpp': butils_wrap.mul_cpp,
-    'beam_phase': butils_wrap.beam_phase,
-    'beam_phase_fast': butils_wrap.beam_phase_fast,
-    'fast_resonator': butils_wrap.fast_resonator,
-    'kick': butils_wrap.kick,
-    'rf_volt_comp': butils_wrap.rf_volt_comp,
-    'drift': butils_wrap.drift,
-    'linear_interp_kick': butils_wrap.linear_interp_kick,
-    'LIKick_n_drift': butils_wrap.linear_interp_kick_n_drift,
-    'synchrotron_radiation': butils_wrap.synchrotron_radiation,
-    'synchrotron_radiation_full': butils_wrap.synchrotron_radiation_full,
-    'set_random_seed': butils_wrap.set_random_seed,
-    'sparse_histogram': butils_wrap.sparse_histogram,
-    # 'linear_interp_time_translation': butils_wrap.linear_interp_time_translation,
-    'slice': butils_wrap.slice,
-    'slice_smooth': butils_wrap.slice_smooth,
-    'music_track': butils_wrap.music_track,
-    'music_track_multiturn': butils_wrap.music_track_multiturn,
-    'device': 'CPU'
-}
-
-# add numpy functions in the dictionary
-for fname in dir(np):
-    if callable(getattr(np, fname)) and (fname not in _CPU_func_dict):
-        _CPU_func_dict[fname] = getattr(np, fname)
-
-# add basic numpy modules to dictionary as they are not callable
-_CPU_func_dict['random'] = getattr(np, 'random')
-_CPU_func_dict['fft'] = getattr(np, 'fft')
-
-_FFTW_func_dict = {
-    'rfft': butils_wrap.rfft,
-    'irfft': butils_wrap.irfft,
-    'rfftfreq': butils_wrap.rfftfreq
-}
 
-_MPI_func_dict = {
+def use_py():
+    '''
+    Replace all python functions by there equivalent in python
+    '''
+    # dictionary storing the Python-only versions of the most compute intensive functions #
+    PY_func_dict = {
+        'rfft': np.fft.rfft,
+        'irfft': np.fft.irfft,
+        'rfftfreq': np.fft.rfftfreq,
+
+        'kick': _py.kick,
+        'rf_volt_comp': _py.rf_volt_comp,
+        'drift': _py.drift,
+        'slice': _py.slice,
+        'slice_smooth': _py.slice_smooth,
+        'linear_interp_kick': _py.linear_interp_kick,
+        'synchrotron_radiation': _py.synchrotron_radiation,
+        'synchrotron_radiation_full': _py.synchrotron_radiation_full,
+        'music_track': _py.music_track,
+        'music_track_multiturn': _py.music_track_multiturn,
+        'fast_resonator': _py.fast_resonator,
+        'beam_phase': _py.beam_phase,
+        'beam_phase_fast': _py.beam_phase_fast,
+        'sparse_histogram': _py.sparse_histogram,
+        'distribution_from_tomoscope': _py.distribution_from_tomoscope,
+        'set_random_seed': _py.set_random_seed,
+
+        'device': 'CPU_PY'
+    }
+
+    # add numpy functions in the dictionary
+    for fname in dir(np):
+        if callable(getattr(np, fname)) and (fname not in PY_func_dict) \
+                and (fname[0] != '_'):
+
+            PY_func_dict[fname] = getattr(np, fname)
+
+    # add basic numpy modules to dictionary as they are not callable
+    PY_func_dict['random'] = getattr(np, 'random')
+    PY_func_dict['fft'] = getattr(np, 'fft')
 
-}
+    # Update the global functions
+    __update_active_dict(PY_func_dict)
+
+
+def use_cpu():
+    '''
+    If not library is found, use the python implementations
+    '''
+    from .. import libblond as __lib
+    if __lib is None:
+        use_py()
+    else:
+        use_cpp()
 
 
 def use_mpi():
     '''
     Replace some bm functions with MPI implementations
     '''
     global __exec_mode
-    globals().update(_MPI_func_dict)
+
+    MPI_func_dict = {}
+    globals().update(MPI_func_dict)
     __exec_mode = 'multi_node'
 
 
 def mpiMode():
     global __exec_mode
     return __exec_mode == 'multi_node'
 
 
 def use_fftw():
     '''
     Replace the existing rfft and irfft implementations
-    with the ones coming from butils_wrap.
+    with the ones coming from _cpp.
     '''
-    globals().update(_FFTW_func_dict)
+
+    FFTW_func_dict = {
+        'rfft': _cpp.rfft,
+        'irfft': _cpp.irfft,
+        'rfftfreq': _cpp.rfftfreq
+    }
+    globals().update(FFTW_func_dict)
 
 
 # precision can be single or double
 def use_precision(_precision='double'):
     global precision
-    butils_wrap.precision = butils_wrap.Precision(_precision)
-    precision = butils_wrap.precision
+    precision.set(_precision)
+    # utils.precision = utils.PrecisionClass(_precision)
+    # precision = PrecisionClass(_precision)
+    # Make sure that the precision object in __init__.py is also updated
+    # from . import precision as _precision
+    # _precision = precision
+    # utils.precision = PrecisionClass(_precision)
+    # precision = _cpp.precision
 
 
-def update_active_dict(new_dict):
+def __update_active_dict(new_dict):
     '''
     Update the currently active dictionary. Removes the keys of the currently
     active dictionary from globals() and spills the keys
     from new_dict to globals()
     Args:
         new_dict A dictionary which contents will be spilled to globals()
     '''
-    if not hasattr(update_active_dict, 'active_dict'):
-        update_active_dict.active_dict = new_dict
+    if not hasattr(__update_active_dict, 'active_dict'):
+        __update_active_dict.active_dict = new_dict
 
     # delete all old implementations/references from globals()
-    for key in update_active_dict.active_dict.keys():
+    for key in __update_active_dict.active_dict.keys():
         if key in globals():
             del globals()[key]
     # for key in globals().keys():
-    #     if key in update_active_dict.active_dict.keys():
+    #     if key in __update_active_dict.active_dict.keys():
     #         del globals()[key]
     # add the new active dict to the globals()
     globals().update(new_dict)
-    update_active_dict.active_dict = new_dict
-
-
-###############################################################################
-update_active_dict(_CPU_func_dict)
-###############################################################################
+    __update_active_dict.active_dict = new_dict
 
 
 # GPU Related Utilities
-
 def gpuDev():
-    return __gpu_dev
-
-
-class GPUDev:
-    __instance = None
-
-    def __init__(self, _gpu_num=0):
-        if GPUDev.__instance is not None:
-            return
-            # raise Exception("The GPUDev class is a singleton!")
-        else:
-            GPUDev.__instance = self
-
-        import cupy as cp
-        self.id = _gpu_num
-        self.dev = cp.cuda.Device(self.id)
-        self.dev.use()
-
-        self.name = cp.cuda.runtime.getDeviceProperties(self.dev)['name']
-        self.attributes = self.dev.attributes
-        self.properties = cp.cuda.runtime.getDeviceProperties(self.dev)
-
-        # set the default grid and block sizes
-        default_blocks = 2 * self.attributes['MultiProcessorCount']
-        default_threads = self.attributes['MaxThreadsPerBlock']
-        blocks = int(os.environ.get('GPU_BLOCKS', default_blocks))
-        threads = int(os.environ.get('GPU_THREADS', default_threads))
-        self.grid_size = (blocks, 1, 1)
-        self.block_size = (threads, 1, 1)
-
-        this_dir = os.path.dirname(os.path.realpath(__file__)) + "/"
-        comp_capability = self.dev.compute_capability
-
-        if precision.num == 1:
-            self.mod = cp.RawModule(path=os.path.join(
-                this_dir, f'../gpu/cuda_kernels/kernels_single_sm_{comp_capability}.cubin'))
-        else:
-            self.mod = cp.RawModule(path=os.path.join(
-                this_dir, f'../gpu/cuda_kernels/kernels_double_sm_{comp_capability}.cubin'))
-
-    def report_attributes(self):
-        # Saves into a file all the device attributes
-        with open(f'{self.name}-attributes.txt', 'w') as f:
-            for k, v in self.attributes.items():
-                f.write(f"{k}:{v}\n")
-
-    def func(self, name):
-        return self.mod.get_function(name)
-
-    def __del__(self):
-        update_active_dict(_CPU_func_dict)
+    return gpu_dev
 
 
 def use_gpu(gpu_id=0):
 
     if gpu_id < 0:
         return
 
-    global __gpu_dev
-    if __gpu_dev is None:
-        __gpu_dev = GPUDev(gpu_id)
+    global gpu_dev
+    from . import GPUDev
+    if gpu_dev is None:
+        gpu_dev = GPUDev(gpu_id)
 
         print(''.join(['#']*10) +
               ' Using GPU: id {}, name {}, Compute Capability {} '.format(
-            __gpu_dev.id, __gpu_dev.name, __gpu_dev.dev.compute_capability)
+            gpu_dev.id, gpu_dev.name, gpu_dev.dev.compute_capability)
             + ''.join(['#']*10) + '\n', flush=True)
 
-    from ..gpu import cupy_butils_wrap
+    from ..gpu import butils_wrap_cupy as _cupy
     import cupy as cp
 
-    _GPU_func_dict = {
-        # 'rfft': cupy_butils_wrap.rfft,
-        # 'irfft': cupy_butils_wrap.irfft,
+    GPU_func_dict = {
         'rfft': cp.fft.rfft,
         'irfft': cp.fft.irfft,
         'rfftfreq': cp.fft.rfftfreq,
         'convolve': cp.convolve,
-        # 'convolve': cupy_butils_wrap.convolve,
-        'beam_phase': cupy_butils_wrap.beam_phase,
-        'beam_phase_fast': cupy_butils_wrap.beam_phase_fast,
-        'kick': cupy_butils_wrap.kick,
-        'rf_volt_comp': cupy_butils_wrap.rf_volt_comp,
-        'drift': cupy_butils_wrap.drift,
-        'linear_interp_kick': cupy_butils_wrap.linear_interp_kick,
-        'LIKick_n_drift': cupy_butils_wrap.linear_interp_kick_drift,
-        'synchrotron_radiation': cupy_butils_wrap.synchrotron_radiation,
-        'synchrotron_radiation_full': cupy_butils_wrap.synchrotron_radiation_full,
-        'slice': cupy_butils_wrap.slice,
-        # 'interp_const_space': cupy_butils_wrap.interp,
+        # 'convolve': _cupy.convolve,
+        'beam_phase': _cupy.beam_phase,
+        'beam_phase_fast': _cupy.beam_phase_fast,
+        'kick': _cupy.kick,
+        'rf_volt_comp': _cupy.rf_volt_comp,
+        'drift': _cupy.drift,
+        'linear_interp_kick': _cupy.linear_interp_kick,
+        'LIKick_n_drift': _cupy.linear_interp_kick_drift,
+        'synchrotron_radiation': _cupy.synchrotron_radiation,
+        'synchrotron_radiation_full': _cupy.synchrotron_radiation_full,
+        'slice': _cupy.slice,
+        # 'interp_const_space': _cupy.interp,
         'interp_const_space': cp.interp,
         'device': 'GPU'
     }
     # add cupy functions in the dictionary
     for fname in dir(cp):
-        if callable(getattr(cp, fname)) and (fname not in _GPU_func_dict):
-            _GPU_func_dict[fname] = getattr(cp, fname)
-    update_active_dict(_GPU_func_dict)
+        if callable(getattr(cp, fname)) and (fname not in GPU_func_dict):
+            GPU_func_dict[fname] = getattr(cp, fname)
+    __update_active_dict(GPU_func_dict)
 
     # add basic cupy modules to dictionary as they are not callable
-    _GPU_func_dict['random'] = getattr(cp, 'random')
-    _GPU_func_dict['fft'] = getattr(cp, 'fft')
+    GPU_func_dict['random'] = getattr(cp, 'random')
+    GPU_func_dict['fft'] = getattr(cp, 'fft')
 
 
-def use_cpu():
-    update_active_dict(_CPU_func_dict)
+###############################################################################
+# By default use the CPU backend (python-only or C++)
+use_cpu()
+###############################################################################
```

### Comparing `blond-2.1.2/blond/utils/butils_wrap.py` & `blond-2.1.3/blond/utils/butils_wrap_cpp.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,83 +5,28 @@
 @date 20.10.2017
 '''
 
 import ctypes as ct
 import numpy as np
 import os
 from .. import libblond as __lib
-
-
-class Precision:
-    def __init__(self, precision='double'):
-        if precision in ['single', 's', '32', 'float32', 'float', 'f']:
-            self.str = 'float32'
-            self.real_t = np.float32
-            self.c_real_t = ct.c_float
-            self.complex_t = np.complex64
-            self.num = 1
-        elif precision in ['double', 'd', '64', 'float64']:
-            self.str = 'float64'
-            self.real_t = np.float64
-            self.c_real_t = ct.c_double
-            self.complex_t = np.complex128
-            self.num = 2
-
-
-precision = Precision('double')
-
+from . import precision, c_real, c_complex, c_complex64, c_complex128
 
 def __getPointer(x):
     return x.ctypes.data_as(ct.c_void_p)
 
 
 def __getLen(x):
     return ct.c_int(len(x))
 
 
-def __c_real(x):
-    if precision.num == 1:
-        return ct.c_float(x)
-    else:
-        return ct.c_double(x)
-
-
-class c_complex128(ct.Structure):
-    # Complex number, compatible with std::complex layout
-    _fields_ = [("real", ct.c_double), ("imag", ct.c_double)]
-
-    def __init__(self, pycomplex):
-        # Init from Python complex
-        self.real = pycomplex.real.astype(np.float64, order='C')
-        self.imag = pycomplex.imag.astype(np.float64, order='C')
-
-    def to_complex(self):
-        # Convert to Python complex
-        return self.real + (1.j) * self.imag
-
-
-class c_complex64(ct.Structure):
-    # Complex number, compatible with std::complex layout
-    _fields_ = [("real", ct.c_float), ("imag", ct.c_float)]
-
-    def __init__(self, pycomplex):
-        # Init from Python complex
-        self.real = pycomplex.real.astype(np.float32, order='C')
-        self.imag = pycomplex.imag.astype(np.float32, order='C')
-
-    def to_complex(self):
-        # Convert to Python complex
-        return self.real + (1.j) * self.imag
-
 # Similar to np.where with a condition of more_than < x < less_than
 # You need to define at least one of more_than, less_than
 # @return: a bool array, size equal to the input,
 #           True: element satisfied the cond, False: otherwise
-
-
 def where_cpp(x, more_than=None, less_than=None, result=None):
     if result is None:
         result = np.empty_like(x, dtype=bool)
     if more_than is None and less_than is not None:
         __lib.where_less_than(__getPointer(x), x.size,
                               ct.c_double(less_than),
                               __getPointer(result))
@@ -232,29 +177,29 @@
     __lib.max_idx.restype = ct.c_int
     return __lib.max_idx(__getPointer(x), __getLen(x))
 
 
 def linspace_cpp(start, stop, num=50, retstep=False, result=None):
     if result is None:
         result = np.empty(num, dtype=float)
-    __lib.linspace(__c_real(start), __c_real(stop),
+    __lib.linspace(c_real(start), c_real(stop),
                    ct.c_int(num), __getPointer(result))
     if retstep:
         return result, 1. * (stop-start) / (num-1)
     else:
         return result
 
 
 def arange_cpp(start, stop, step, dtype=float, result=None):
     size = int(np.ceil((stop-start)/step))
     if result is None:
         result = np.empty(size, dtype=dtype)
     if dtype == float:
-        __lib.arange_double(__c_real(start), __c_real(stop),
-                            __c_real(step), __getPointer(result))
+        __lib.arange_double(c_real(start), c_real(stop),
+                            c_real(step), __getPointer(result))
     elif dtype == int:
         __lib.arange_int(ct.c_int(start), ct.c_int(stop),
                          ct.c_int(step), __getPointer(result))
 
     return result
 
 
@@ -375,23 +320,23 @@
     if result is None:
         result = np.empty(len(x), dtype=precision.real_t, order='C')
 
     if precision.num == 1:
         __lib.interpf(__getPointer(x), __getLen(x),
                       __getPointer(xp), __getLen(xp),
                       __getPointer(yp),
-                      __c_real(left),
-                      __c_real(right),
+                      c_real(left),
+                      c_real(right),
                       __getPointer(result))
     else:
         __lib.interp(__getPointer(x), __getLen(x),
                      __getPointer(xp), __getLen(xp),
                      __getPointer(yp),
-                     __c_real(left),
-                     __c_real(right),
+                     c_real(left),
+                     c_real(right),
                      __getPointer(result))
 
     return result
 
 
 def interp_const_space(x, xp, yp, left=None, right=None, result=None):
     x = x.astype(dtype=precision.real_t, order='C', copy=False)
@@ -405,23 +350,23 @@
     if result is None:
         result = np.empty(len(x), dtype=precision.real_t, order='C')
 
     if precision.num == 1:
         __lib.interp_const_spacef(__getPointer(x), __getLen(x),
                                   __getPointer(xp), __getLen(xp),
                                   __getPointer(yp),
-                                  __c_real(left),
-                                  __c_real(right),
+                                  c_real(left),
+                                  c_real(right),
                                   __getPointer(result))
     else:
         __lib.interp_const_space(__getPointer(x), __getLen(x),
                                  __getPointer(xp), __getLen(xp),
                                  __getPointer(yp),
-                                 __c_real(left),
-                                 __c_real(right),
+                                 c_real(left),
+                                 c_real(right),
                                  __getPointer(result))
 
     return result
 
 
 def rfft(a, n=0, result=None):
     a = a.astype(dtype=precision.real_t, order='C', copy=False)
@@ -475,19 +420,19 @@
         raise ZeroDivisionError('d must be non-zero')
     if result is None:
         result = np.empty(n//2 + 1, dtype=precision.real_t)
 
     if precision.num == 1:
         __lib.rfftfreqf(ct.c_int(n),
                         __getPointer(result),
-                        __c_real(d))
+                        c_real(d))
     else:
         __lib.rfftfreq(ct.c_int(n),
                        __getPointer(result),
-                       __c_real(d))
+                       c_real(d))
 
     return result
 
 
 def irfft_packed(signal, fftsize=0, result=None):
 
     n0 = len(signal[0])
@@ -525,28 +470,28 @@
     if x is not None:
         # IntegrationError
         raise RuntimeError('[cumtrapz] x attribute is not yet supported')
     if initial:
         if result is None:
             result = np.empty(len(y), dtype=float)
         __lib.cumtrapz_w_initial(__getPointer(y),
-                                 __c_real(dx), __c_real(initial),
+                                 c_real(dx), c_real(initial),
                                  __getLen(y), __getPointer(result))
     else:
         if result is None:
             result = np.empty(len(y)-1, dtype=float)
-        __lib.cumtrapz_wo_initial(__getPointer(y), __c_real(dx),
+        __lib.cumtrapz_wo_initial(__getPointer(y), c_real(dx),
                                   __getLen(y), __getPointer(result))
     return result
 
 
 def trapz_cpp(y, x=None, dx=1.0):
     if x is None:
         __lib.trapz_const_delta.restype = ct.c_double
-        return __lib.trapz_const_delta(__getPointer(y), __c_real(dx),
+        return __lib.trapz_const_delta(__getPointer(y), c_real(dx),
                                        __getLen(y))
     else:
         __lib.trapz_var_delta.restype = ct.c_double
         return __lib.trapz_var_delta(__getPointer(y), __getPointer(x),
                                      __getLen(y))
 
 
@@ -555,44 +500,44 @@
                                      copy=False)
     profile = profile.astype(dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
         __lib.beam_phasef.restype = ct.c_float
         coeff = __lib.beam_phasef(__getPointer(bin_centers),
                                   __getPointer(profile),
-                                  __c_real(alpha),
-                                  __c_real(omegarf),
-                                  __c_real(phirf),
-                                  __c_real(bin_size),
+                                  c_real(alpha),
+                                  c_real(omegarf),
+                                  c_real(phirf),
+                                  c_real(bin_size),
                                   __getLen(profile))
 
     else:
         __lib.beam_phase.restype = ct.c_double
         coeff = __lib.beam_phase(__getPointer(bin_centers),
                                  __getPointer(profile),
-                                 __c_real(alpha),
-                                 __c_real(omegarf),
-                                 __c_real(phirf),
-                                 __c_real(bin_size),
+                                 c_real(alpha),
+                                 c_real(omegarf),
+                                 c_real(phirf),
+                                 c_real(bin_size),
                                  __getLen(profile))
     return coeff
 
 
 def beam_phase_fast(bin_centers, profile, omegarf, phirf, bin_size):
     bin_centers = bin_centers.astype(dtype=precision.real_t, order='C',
                                      copy=False)
     profile = profile.astype(dtype=precision.real_t, order='C', copy=False)
 
     __lib.beam_phase_fast.restype = ct.c_double
     coeff = __lib.beam_phase_fast(__getPointer(bin_centers),
-                             __getPointer(profile),
-                             __c_real(omegarf),
-                             __c_real(phirf),
-                             __c_real(bin_size),
-                             __getLen(profile))
+                                  __getPointer(profile),
+                                  c_real(omegarf),
+                                  c_real(phirf),
+                                  c_real(bin_size),
+                                  __getLen(profile))
     return coeff
 
 
 def rf_volt_comp(voltages, omega_rf, phi_rf, bin_centers):
 
     bin_centers = bin_centers.astype(
         dtype=precision.real_t, order='C', copy=False)
@@ -637,64 +582,64 @@
         __lib.kickf(__getPointer(dt),
                     __getPointer(dE),
                     ct.c_int(n_rf),
                     __getPointer(voltage_kick),
                     __getPointer(omegarf_kick),
                     __getPointer(phirf_kick),
                     __getLen(dt),
-                    __c_real(acceleration_kick))
+                    c_real(acceleration_kick))
     else:
         __lib.kick(__getPointer(dt),
                    __getPointer(dE),
                    ct.c_int(n_rf),
                    __getPointer(voltage_kick),
                    __getPointer(omegarf_kick),
                    __getPointer(phirf_kick),
                    __getLen(dt),
-                   __c_real(acceleration_kick))
+                   c_real(acceleration_kick))
 
 
 def drift(dt, dE, solver, t_rev, length_ratio, alpha_order, eta_0,
           eta_1, eta_2, alpha_0, alpha_1, alpha_2, beta, energy):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(dE[0], precision.real_t)
 
     # dt = dt.astype(dtype=precision.real_t, order='C', copy=False)
     # dE = dE.astype(dtype=precision.real_t, order='C', copy=False)
     if precision.num == 1:
         __lib.driftf(__getPointer(dt),
                      __getPointer(dE),
                      ct.c_char_p(solver),
-                     __c_real(t_rev),
-                     __c_real(length_ratio),
-                     __c_real(alpha_order),
-                     __c_real(eta_0),
-                     __c_real(eta_1),
-                     __c_real(eta_2),
-                     __c_real(alpha_0),
-                     __c_real(alpha_1),
-                     __c_real(alpha_2),
-                     __c_real(beta),
-                     __c_real(energy),
+                     c_real(t_rev),
+                     c_real(length_ratio),
+                     c_real(alpha_order),
+                     c_real(eta_0),
+                     c_real(eta_1),
+                     c_real(eta_2),
+                     c_real(alpha_0),
+                     c_real(alpha_1),
+                     c_real(alpha_2),
+                     c_real(beta),
+                     c_real(energy),
                      __getLen(dt))
     else:
         __lib.drift(__getPointer(dt),
                     __getPointer(dE),
                     ct.c_char_p(solver),
-                    __c_real(t_rev),
-                    __c_real(length_ratio),
-                    __c_real(alpha_order),
-                    __c_real(eta_0),
-                    __c_real(eta_1),
-                    __c_real(eta_2),
-                    __c_real(alpha_0),
-                    __c_real(alpha_1),
-                    __c_real(alpha_2),
-                    __c_real(beta),
-                    __c_real(energy),
+                    c_real(t_rev),
+                    c_real(length_ratio),
+                    c_real(alpha_order),
+                    c_real(eta_0),
+                    c_real(eta_1),
+                    c_real(eta_2),
+                    c_real(alpha_0),
+                    c_real(alpha_1),
+                    c_real(alpha_2),
+                    c_real(beta),
+                    c_real(energy),
                     __getLen(dt))
 
 
 def linear_interp_kick(dt, dE, voltage,
                        bin_centers, charge,
                        acceleration_kick):
 
@@ -710,27 +655,27 @@
     # dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
         __lib.linear_interp_kickf(__getPointer(dt),
                                   __getPointer(dE),
                                   __getPointer(voltage),
                                   __getPointer(bin_centers),
-                                  __c_real(charge),
+                                  c_real(charge),
                                   __getLen(bin_centers),
                                   __getLen(dt),
-                                  __c_real(acceleration_kick))
+                                  c_real(acceleration_kick))
     else:
         __lib.linear_interp_kick(__getPointer(dt),
                                  __getPointer(dE),
                                  __getPointer(voltage),
                                  __getPointer(bin_centers),
-                                 __c_real(charge),
+                                 c_real(charge),
                                  __getLen(bin_centers),
                                  __getLen(dt),
-                                 __c_real(acceleration_kick))
+                                 c_real(acceleration_kick))
 
 
 def linear_interp_kick_n_drift(dt, dE, total_voltage, bin_centers, charge, acc_kick,
                                solver, t_rev, length_ratio, alpha_order, eta_0, eta_1,
                                eta_2, beta, energy):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(dE[0], precision.real_t)
@@ -746,87 +691,87 @@
     if precision.num == 1:
         __lib.linear_interp_kick_n_driftf(__getPointer(dt),
                                           __getPointer(dE),
                                           __getPointer(total_voltage),
                                           __getPointer(bin_centers),
                                           __getLen(bin_centers),
                                           __getLen(dt),
-                                          __c_real(acc_kick),
+                                          c_real(acc_kick),
                                           ct.c_char_p(solver),
-                                          __c_real(t_rev),
-                                          __c_real(length_ratio),
-                                          __c_real(alpha_order),
-                                          __c_real(eta_0),
-                                          __c_real(eta_1),
-                                          __c_real(eta_2),
-                                          __c_real(beta),
-                                          __c_real(energy),
-                                          __c_real(charge))
+                                          c_real(t_rev),
+                                          c_real(length_ratio),
+                                          c_real(alpha_order),
+                                          c_real(eta_0),
+                                          c_real(eta_1),
+                                          c_real(eta_2),
+                                          c_real(beta),
+                                          c_real(energy),
+                                          c_real(charge))
     else:
         __lib.linear_interp_kick_n_drift(__getPointer(dt),
                                          __getPointer(dE),
                                          __getPointer(total_voltage),
                                          __getPointer(bin_centers),
                                          __getLen(bin_centers),
                                          __getLen(dt),
-                                         __c_real(acc_kick),
+                                         c_real(acc_kick),
                                          ct.c_char_p(solver),
-                                         __c_real(t_rev),
-                                         __c_real(length_ratio),
-                                         __c_real(alpha_order),
-                                         __c_real(eta_0),
-                                         __c_real(eta_1),
-                                         __c_real(eta_2),
-                                         __c_real(beta),
-                                         __c_real(energy),
-                                         __c_real(charge))
+                                         c_real(t_rev),
+                                         c_real(length_ratio),
+                                         c_real(alpha_order),
+                                         c_real(eta_0),
+                                         c_real(eta_1),
+                                         c_real(eta_2),
+                                         c_real(beta),
+                                         c_real(energy),
+                                         c_real(charge))
 
 
 def slice(dt, profile, cut_left, cut_right):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(profile[0], precision.real_t)
 
     # dt = dt.astype(dtype=precision.real_t, order='C', copy=False)
     # profile = profile.astype(dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
         __lib.histogramf(__getPointer(dt),
                          __getPointer(profile),
-                         __c_real(cut_left),
-                         __c_real(cut_right),
+                         c_real(cut_left),
+                         c_real(cut_right),
                          __getLen(profile),
                          __getLen(dt))
     else:
         __lib.histogram(__getPointer(dt),
                         __getPointer(profile),
-                        __c_real(cut_left),
-                        __c_real(cut_right),
+                        c_real(cut_left),
+                        c_real(cut_right),
                         __getLen(profile),
                         __getLen(dt))
 
 
 def slice_smooth(dt, profile, cut_left, cut_right):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(profile[0], precision.real_t)
 
     # dt = dt.astype(dtype=precision.real_t, order='C', copy=False)
     # profile = profile.astype(dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
         __lib.smooth_histogramf(__getPointer(dt),
                                 __getPointer(profile),
-                                __c_real(cut_left),
-                                __c_real(cut_right),
+                                c_real(cut_left),
+                                c_real(cut_right),
                                 __getLen(profile),
                                 __getLen(dt))
     else:
         __lib.smooth_histogram(__getPointer(dt),
                                __getPointer(profile),
-                               __c_real(cut_left),
-                               __c_real(cut_right),
+                               c_real(cut_left),
+                               c_real(cut_right),
                                __getLen(profile),
                                __getLen(dt))
 
 
 def sparse_histogram(dt, profile, cut_left, cut_right, bunch_indexes, n_slices_bucket):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(profile[0][0], precision.real_t)
@@ -870,34 +815,34 @@
 
     if precision.num == 1:
         __lib.music_trackf(__getPointer(dt),
                            __getPointer(dE),
                            __getPointer(induced_voltage),
                            __getPointer(array_parameters),
                            __getLen(dt),
-                           __c_real(alpha),
-                           __c_real(omega_bar),
-                           __c_real(const),
-                           __c_real(coeff1),
-                           __c_real(coeff2),
-                           __c_real(coeff3),
-                           __c_real(coeff4))
+                           c_real(alpha),
+                           c_real(omega_bar),
+                           c_real(const),
+                           c_real(coeff1),
+                           c_real(coeff2),
+                           c_real(coeff3),
+                           c_real(coeff4))
     else:
         __lib.music_track(__getPointer(dt),
                           __getPointer(dE),
                           __getPointer(induced_voltage),
                           __getPointer(array_parameters),
                           __getLen(dt),
-                          __c_real(alpha),
-                          __c_real(omega_bar),
-                          __c_real(const),
-                          __c_real(coeff1),
-                          __c_real(coeff2),
-                          __c_real(coeff3),
-                          __c_real(coeff4))
+                          c_real(alpha),
+                          c_real(omega_bar),
+                          c_real(const),
+                          c_real(coeff1),
+                          c_real(coeff2),
+                          c_real(coeff3),
+                          c_real(coeff4))
 
 
 def music_track_multiturn(dt, dE, induced_voltage, array_parameters,
                           alpha, omega_bar,
                           const, coeff1, coeff2, coeff3, coeff4):
     assert isinstance(dt[0], precision.real_t)
     assert isinstance(dE[0], precision.real_t)
@@ -915,78 +860,78 @@
 
     if precision.num == 1:
         __lib.music_track_multiturnf(__getPointer(dt),
                                      __getPointer(dE),
                                      __getPointer(induced_voltage),
                                      __getPointer(array_parameters),
                                      __getLen(dt),
-                                     __c_real(alpha),
-                                     __c_real(omega_bar),
-                                     __c_real(const),
-                                     __c_real(coeff1),
-                                     __c_real(coeff2),
-                                     __c_real(coeff3),
-                                     __c_real(coeff4))
+                                     c_real(alpha),
+                                     c_real(omega_bar),
+                                     c_real(const),
+                                     c_real(coeff1),
+                                     c_real(coeff2),
+                                     c_real(coeff3),
+                                     c_real(coeff4))
     else:
         __lib.music_track_multiturn(__getPointer(dt),
                                     __getPointer(dE),
                                     __getPointer(induced_voltage),
                                     __getPointer(array_parameters),
                                     __getLen(dt),
-                                    __c_real(alpha),
-                                    __c_real(omega_bar),
-                                    __c_real(const),
-                                    __c_real(coeff1),
-                                    __c_real(coeff2),
-                                    __c_real(coeff3),
-                                    __c_real(coeff4))
+                                    c_real(alpha),
+                                    c_real(omega_bar),
+                                    c_real(const),
+                                    c_real(coeff1),
+                                    c_real(coeff2),
+                                    c_real(coeff3),
+                                    c_real(coeff4))
 
 
 def synchrotron_radiation(dE, U0, n_kicks, tau_z):
     assert isinstance(dE[0], precision.real_t)
     # dE = dE.astype(dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
         __lib.synchrotron_radiationf(
             __getPointer(dE),
-            __c_real(U0 / n_kicks),
+            c_real(U0 / n_kicks),
             __getLen(dE),
-            __c_real(tau_z * n_kicks),
+            c_real(tau_z * n_kicks),
             ct.c_int(n_kicks))
     else:
         __lib.synchrotron_radiation(
             __getPointer(dE),
-            __c_real(U0 / n_kicks),
+            c_real(U0 / n_kicks),
             __getLen(dE),
-            __c_real(tau_z * n_kicks),
+            c_real(tau_z * n_kicks),
             ct.c_int(n_kicks))
 
 
 def synchrotron_radiation_full(dE, U0, n_kicks, tau_z, sigma_dE, energy):
     assert isinstance(dE[0], precision.real_t)
 
     # dE = dE.astype(dtype=precision.real_t, order='C', copy=False)
 
     if precision.num == 1:
         __lib.synchrotron_radiation_fullf(
             __getPointer(dE),
-            __c_real(U0 / n_kicks),
+            c_real(U0 / n_kicks),
             __getLen(dE),
-            __c_real(sigma_dE),
-            __c_real(tau_z * n_kicks),
-            __c_real(energy),
+            c_real(sigma_dE),
+            c_real(tau_z * n_kicks),
+            c_real(energy),
             ct.c_int(n_kicks))
     else:
         __lib.synchrotron_radiation_full(
             __getPointer(dE),
-            __c_real(U0 / n_kicks),
+            c_real(U0 / n_kicks),
             __getLen(dE),
-            __c_real(sigma_dE),
-            __c_real(tau_z * n_kicks),
-            __c_real(energy),
+            c_real(sigma_dE),
+            c_real(tau_z * n_kicks),
+            c_real(energy),
             ct.c_int(n_kicks))
 
 
 def set_random_seed(seed):
     __lib.set_random_seed(ct.c_int(seed))
 
 
@@ -1022,14 +967,26 @@
             __getLen(R_S),
             __getLen(frequency_array))
 
     impedance = realImp + 1j * imagImp
     return impedance
 
 
+def distribution_from_tomoscope(dt, dE, probDistr, seed, profLen,
+                                cutoff, x0, y0, dtBin, dEBin):
+
+    __lib.generate_distribution(__getPointer(dt),
+                                __getPointer(dE),
+                                __getPointer(probDistr),
+                                ct.c_uint(seed), ct.c_uint(profLen),
+                                ct.c_double(cutoff), ct.c_double(x0),
+                                ct.c_double(y0), ct.c_double(dtBin),
+                                ct.c_double(dEBin), __getLen(dt))
+
+
 # def mean(x):
 #     __lib.mean.restype = ct.c_double
 #     return __lib.mean(__getPointer(x), __getLen(x))
 
 
 # def std(x):
 #     __lib.stdev.restype = ct.c_double
```

### Comparing `blond-2.1.2/blond/utils/data_check.py` & `blond-2.1.3/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/utils/exceptions.py` & `blond-2.1.3/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/utils/mpi_config.py` & `blond-2.1.3/blond/utils/mpi_config.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond/utils/track_iteration.py` & `blond-2.1.3/blond/utils/track_iteration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/blond.egg-info/PKG-INFO` & `blond-2.1.3/blond.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.2
+Version: 2.1.3
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko et al.
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -42,134 +42,115 @@
 
 Repository: <https://gitlab.cern.ch/blond/BLonD>
 
 Documentation: <https://blond-code.docs.cern.ch/>
 
 Project website: <http://blond.web.cern.ch>
 
-# Install
+# Installation
 
-## Requirements
+## Dependencies
 
-1.  A gcc compiler with C++11 support (version greater than 4.8.4).
-2.  An Anaconda distribution (Python 3 recommended).
-3.  That's all!
+1. Python 3.6 or above (Anaconda is recommended).  
+2. (Optional) For better performance, a C++ (e.g. `gcc`, `icc`, `clang`, etc) compiler with `C++11` support.
 
-## Windows GCC Installation Instructions
+### (Optional) C++ compiler installation instructions
+
+#### Windows
 
 1.  Download the latest mingw-w64 using this link:
     <https://winlibs.com/#download-release>
 2.  Extract the downloaded zip/7-zip under e.g. `C:\`. You should now
     see a directory `C:\mingw64`.
 3.  Add `C:\mingw64\bin` in the PATH Environment Variable. [Here you can
     see how to do this in Windows
     XP/Vista/7/8/10/11](https://www.computerhope.com/issues/ch000549.htm).
 4.  To validate the correct setup of gcc, open a command prompt and
     type: `gcc --version`. The first output line should contain the gcc
     version you just installed.
 
-## Install Steps
+#### Linux
+Use your distribution's package manager to install the compiler of your choice. BLonD has been tested with: `gcc` (recommended), `icc`, and `clang`.
 
-### Installing BLonD as a python package.
+## Installation Steps
 
--   Using the pip package manager:
+### Installing BLonD as a python package.
 
-    ``` bash
-    $ pip install blond
+-   Using the `pip` package manager:
+    ```bash
+    pip install blond
     ```
 
--   If this fails try to:
-
-    1.  Clone the repository from gitlab or download and extract the zip
-        from <https://gitlab.cern.ch/blond/BLonD/-/archive/master/BLonD-master.zip>
-    2.  Go to the downloaded BLonD directory and run:
-
-        ``` bash
-        $ python setup.py install
-        ```
-
--   If it still fails, go to the BLonD directory and run:
-
-    1.  
-        ``` bash
-        $ python setup.py compile
-        ```
-
-    2.  Then you have to set the PYTHONPATH variable to point to the
-        BLonD installation path.
-
--   In the occasion that it continues to fail, please open a new gitlab issue.
+### Installing BLonD manually (advanced users/ developers).
 
-### For advanced users or developers.
-
-1.  You are advised to install git in your system.
-2.  Clone the repository or download and extract it.
-3.  From within the BLonD directory run:
-    ``` bash
-    $ python blond/compile.py
+1.  Clone the repository (with `git`) or download and extract it.
+2.  (Optional) From within the BLonD directory run:
+    ```bash
+    python blond/compile.py
     ```
-4.  Adjust the PYTHONPATH to contain the path to the cloned repository.
+3. (Optional) See the complete list of the command line arguments with:
+    ```bash
+    python blond/compile.py --help
+    ```
+4.  Adjust the `PYTHONPATH` environment variable to contain the path to the BLonD directory.
 
 ## Confirm proper installation
 
--   Run the unittests with pytest (may need to be installed first with
-    pip install pytest):
-
+-   Run the unittests with `pytest` (the `pytest` package may need to be installed first):
     ``` bash
-    $ pytest -v unittests
+    pytest -v unittests
     ```
 
--   Try to run some of the main files found in the examples:
-
+-   Run some of the main files found in the `__EXAMPLES` directory:
     ``` bash
-    $ python __EXAMPLES/main_files/EX_01_Acceleration.py
-    $ python __EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
-    $ etc..
+    python __EXAMPLES/main_files/EX_01_Acceleration.py
+    python __EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+    etc..
     ```
 
-## Performace Optimizations
+# Performance Optimizations
+By default, if the C++ blond library has not been compiled, the python-only backend will be used to run the most time-consuming operations. 
 
-There are some easy ways to reduce the execution time of your
-simulation:
+To use the C++ backend and accelerate the execution of the time-consuming operations, follow the instructions provided in the section *Installing BLonD manually*.
 
-1.  Use the multi-threaded C library. To use it you have to add the -p
-    flag when compiling the C library:
+In addition you may want to:
+* Use the multi-threaded blond C++ backend:
     ``` bash
-    $ python blond/compile.py --parallel
+    python blond/compile.py --parallel
     ```
 
-2.  Enable processor specific compiler optimizations:
+* Enable processor specific compiler optimizations:
     ``` bash
-    $ python blond/compile.py --flags='-march=native'
+    python blond/compile.py --parallel --optimize
     ```
 
-3.  If you are test-case is calling the synchrotron radiation tracking method, you can accelerate it by using the Boost library. To do so you have to:  
+* If you are test-case is calling the synchrotron radiation tracking method, you can accelerate it by using the Boost library. To do so you have to:  
     1.  Download Boost: <https://www.boost.org/>. Let's say the version
         you downloaded is boost_1\_70.
     2.  Extract it, let's say in `/user/path/to/boost_1_70`.
     3.  Pass the boost installation path when compiling BLonD:
         ``` bash
-        $ python blond/compile.py --boost=/user/path/to/boost_1_7_70
+        python blond/compile.py --boost=/user/path/to/boost_1_7_70
         ```
 
-4.  Check the following section about the FFTW3 library.
+* Check the following section about the FFTW3 library.
 
-5.  *All the above can be combined.*
+* All the above can be combined, i.e.:
+    ```bash
+    python blond/compile.py --parallel --optimize --boost=...
+    ```
 
-## Changing the floating point precision (32 bit floats or 64 bit floats)
+## Changing the floating point number datatype
 
--   By default BLonD uses double precision calculations (float64). To
-    change to single precision, for faster calculations, in the
-    beginning of your mainfile you will have to add the code lines:
-    ``` python
-    from blond.utils import bmath as bm
-    bm.use_precision('single') 
-    ```
+By default BLonD uses double precision calculations (float64). To change to single precision for faster calculations, in the beginning of your mainfile you will have to add the following code lines:
+```python
+from blond.utils import bmath as bm
+bm.use_precision('single') 
+```
 
--   No other modifications are needed.
 
 ## Use the FFTW3 library for the FFTs
 
 So far only the `rfft()`, `irfft()` and `fftfreq()` routines are
 supported. `fft_convolve()` to be added soon.
 
 -   Windows:
@@ -330,21 +311,21 @@
     worker.finalize()
     ```
 
 6.  To run your script, you need to pass it to **mpirun** or
     **mpiexec**. To spawn P MPI processes run:
 
     ``` bash
-    $ mpirun -n P python main_file.py
+    mpirun -n P python main_file.py
     ```
 
 7.  For more examples have a look at the \_\_EXAMPLES/mpi_main_files/
     directory.
 
-# Using the GPU Implementation
+# Using the GPU backend
 
 ## Setup Instructions
 
 1.  Install **CUDA**: <https://developer.nvidia.com/cuda-downloads>
 2.  Install the **CuPy** library:
     <https://docs.cupy.dev/en/stable/install.html>
 3.  To verify your installation open a python terminal and execute the
@@ -352,68 +333,68 @@
 
     ``` python
     import cupy as cp 
     import numpy as np 
     a = cp.array(np.zeros(1000,np.float64)) 
     ```
 
-    To compile the Cuda files execute blond/compile.py and add the flag
+    To compile the CUDA files execute blond/compile.py and add the flag
     --gpu. The Compute Capability of your GPU will be automatically
     detected:
 
-``` bash
-$ python blond/compile.py --gpu 
-```
+    ``` bash
+    python blond/compile.py --gpu 
+    ```
 
 ## Changes required in the main file for GPU
 
 1.  Right before your main loop you need to add:
 
     ``` python
     from blond.utils import bmath as bm
     # change some of the basic functions to their GPU equivalent
     bm.use_gpu()
     ```
 
 2.  Also for every object you are using in your main loop that is in the
     following list:
 
-| GPU objects             |
-|-------------------------|
-| Beam                    |
-| Profile                 |
-| RingAndRFTracker        |
-| TotalInducedVoltage     |
-| InducedVoltageTime      |
-| InducedVoltageFreq      |
-| InductiveImpedance      |
-| InducedVoltageResonator |
-| RFStation               |
-| BeamFeedback            |
-
-you need to call their `to_gpu()` method. The following is a typical
-example from the \_\_EXAMPLES/gpu_main_files/EX_01_Acceleration.py
-mainfile.
-
-``` python
-# Define Objects
-beam = Beam(ring, N_p, N_b)
-profile = Profile(beam, CutOptions(n_slices=100), 
-             FitOptions(fit_option='gaussian'))
-# Initialize gpu
-beam.to_gpu()
-profile.to_gpu()
-```
+    | GPU objects             |
+    |-------------------------|
+    | Beam                    |
+    | Profile                 |
+    | RingAndRFTracker        |
+    | TotalInducedVoltage     |
+    | InducedVoltageTime      |
+    | InducedVoltageFreq      |
+    | InductiveImpedance      |
+    | InducedVoltageResonator |
+    | RFStation               |
+    | BeamFeedback            |
+
+    you need to call their `to_gpu()` method. The following is a typical
+    example from the \_\_EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+    mainfile.
+
+    ``` python
+    # Define Objects
+    beam = Beam(ring, N_p, N_b)
+    profile = Profile(beam, CutOptions(n_slices=100), 
+                FitOptions(fit_option='gaussian'))
+    # Initialize gpu
+    beam.to_gpu()
+    profile.to_gpu()
+    ```
 
-If an object of this list has a reference inside a different one you
-don't need to use the `to_gpu()` for the referenced object. In the
-previous example, we don't need to call `beam.to_gpu()` since `beam` is
-referenced inside the `profile`. The same would apply in a
-`TotalInducedVoltage` object and the objects in its
-`induced_voltage_list`.
+    If an object of this list has a reference inside a different one you
+    don't need to use the `to_gpu()` for the referenced object. In the
+    previous example, we don't need to call `beam.to_gpu()` since `beam` is
+    referenced inside the `profile`. The same would apply in a
+    `TotalInducedVoltage` object and the objects in its
+    `induced_voltage_list`.
 
 # Developers
 
 -   Simon Albright (simon.albright (at) cern.ch)
 -   Theodoros Argyropoulos (theodoros.argyropoulos (at) cern.ch)
 -   Konstantinos Iliakis (konstantinos.iliakis (at) cern.ch)
 -   Ivan Karpov (ivan.karpov (at) cern.ch)
```

### Comparing `blond-2.1.2/blond.egg-info/SOURCES.txt` & `blond-2.1.3/blond.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 blond/cpp_routines/music_track.cpp
 blond/cpp_routines/openmp.cpp
 blond/cpp_routines/openmp.h
 blond/cpp_routines/sin.h
 blond/cpp_routines/sincos.h
 blond/cpp_routines/vdtcore_common.h
 blond/gpu/__init__.py
-blond/gpu/cupy_butils_wrap.py
+blond/gpu/butils_wrap_cupy.py
 blond/gpu/cuda_kernels/kernels_double.cu
 blond/gpu/cuda_kernels/kernels_single.cu
 blond/impedances/__init__.py
 blond/impedances/impedance.py
 blond/impedances/impedance_sources.py
 blond/impedances/induced_voltage_analytical.py
 blond/impedances/music.py
@@ -209,20 +209,19 @@
 blond/toolbox/tomoscope.cpp
 blond/toolbox/tomoscope.py
 blond/trackers/__init__.py
 blond/trackers/tracker.py
 blond/trackers/utilities.py
 blond/utils/__init__.py
 blond/utils/bmath.py
-blond/utils/butils_wrap.py
+blond/utils/butils_wrap_cpp.py
+blond/utils/butils_wrap_python.py
 blond/utils/data_check.py
 blond/utils/exceptions.py
-blond/utils/input_parser.py
 blond/utils/mpi_config.py
-blond/utils/profile_mock.py
 blond/utils/track_iteration.py
 unittests/beam_profile/__init__.py
 unittests/beam_profile/dt_coordinates.npz
 unittests/beam_profile/test_beam_profile_object.py
 unittests/beam_profile/test_sparse_profile.py
 unittests/beams/__init__.py
 unittests/beams/test_beam_object.py
@@ -260,10 +259,11 @@
 unittests/synchrotron_radiation/test_synch_rad.py
 unittests/trackers/__init__.py
 unittests/trackers/comparison_drift.py
 unittests/trackers/test_drift.py
 unittests/trackers/test_tracker.py
 unittests/utils/__init__.py
 unittests/utils/test_blondmath.py
+unittests/utils/test_butils_wrap_python.py
 unittests/utils/test_data_check.py
 unittests/utils/test_ffts.py
 unittests/utils/test_iteration.py
```

### Comparing `blond-2.1.2/unittests/beam_profile/dt_coordinates.npz` & `blond-2.1.3/unittests/beam_profile/dt_coordinates.npz`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/beam_profile/test_beam_profile_object.py` & `blond-2.1.3/unittests/beam_profile/test_beam_profile_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/beam_profile/test_sparse_profile.py` & `blond-2.1.3/unittests/beam_profile/test_sparse_profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/beams/test_beam_object.py` & `blond-2.1.3/unittests/beams/test_beam_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/beams/test_coasting_beam.py` & `blond-2.1.3/unittests/beams/test_coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/general/test_separatrix_bigaussian.py` & `blond-2.1.3/unittests/general/test_separatrix_bigaussian.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/gpu/test_ffts.py` & `blond-2.1.3/unittests/gpu/test_ffts.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/gpu/test_impedance.py` & `blond-2.1.3/unittests/gpu/test_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/gpu/test_physics_kernels.py` & `blond-2.1.3/unittests/gpu/test_physics_kernels.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/impedances/test_impedance.py` & `blond-2.1.3/unittests/impedances/test_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/impedances/test_impedance_sources.py` & `blond-2.1.3/unittests/impedances/test_impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/input_parameters/test_preprocess.py` & `blond-2.1.3/unittests/input_parameters/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/input_parameters/test_rf_params_object.py` & `blond-2.1.3/unittests/input_parameters/test_rf_params_object.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/input_parameters/test_ring.py` & `blond-2.1.3/unittests/input_parameters/test_ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/integration/test_examples.py` & `blond-2.1.3/unittests/integration/test_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 Integration tests, execute all __EXAMPLES main files. 
 :Authors: **Konstantinos Iliakis**
 """
 
 import unittest
 import os
 import subprocess
+import sys
 
 this_directory = os.path.dirname(os.path.realpath(__file__)) + '/'
 main_files_dir = os.path.join(this_directory, '../../__EXAMPLES/main_files')
-exec_args = ['python']
+exec_args = [sys.executable]
 timeout = 60    # Timeout in seconds
 
 class TestExamples(unittest.TestCase):
 
     def _runExample(self, example, timeout=timeout):
         file = os.path.join(main_files_dir, example)
         try:
+            ret = subprocess.run(exec_args +['-m', 'pip', 'show', 'blond'])
             ret = subprocess.run(exec_args + [file], timeout=timeout)
             self.assertEqual(ret.returncode, 0)
         except subprocess.TimeoutExpired as e:
             raise unittest.SkipTest(
                 '[{}] Timed out (timeout={}s)'.format(example, e.timeout))
 
     # Run before every test
```

### Comparing `blond-2.1.2/unittests/integration/test_gpu_examples.py` & `blond-2.1.3/unittests/integration/test_gpu_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 :Authors: **Konstantinos Iliakis**
 """
 
 import unittest
 import pytest
 import os
 import subprocess
+import sys
 
 this_directory = os.path.dirname(os.path.realpath(__file__)) + '/'
 main_files_dir = os.path.join(this_directory, '../../__EXAMPLES/gpu_main_files')
-exec_args = ['python']
+exec_args = [sys.executable]
 timeout = 90    # Timeout in seconds
 
 
 class TestGPUExamples(unittest.TestCase):
 
     def _runExample(self, example, timeout=timeout):
         file = os.path.join(main_files_dir, example)
```

### Comparing `blond-2.1.2/unittests/integration/test_mpi_examples.py` & `blond-2.1.3/unittests/integration/test_mpi_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 :Authors: **Konstantinos Iliakis**
 """
 
 import unittest
 import pytest
 import os
 import subprocess
+import sys
 
 this_directory = os.path.dirname(os.path.realpath(__file__)) + '/'
 main_files_dir = os.path.join(this_directory + '../../__EXAMPLES/mpi_main_files')
-exec_args = ['mpirun', '-n', '2', 'python']
+exec_args = ['mpirun', '-n', '2', sys.executable]
 timeout = 60    # Timeout in seconds
 
 
 class TestMpiExamples(unittest.TestCase):
 
     def _runMPIExample(self, example, timeout=timeout):
         file = os.path.join(main_files_dir, example)
@@ -37,15 +38,15 @@
 
     # Run before every test
     def setUp(self):
         pytest.importorskip('mpi4py')
         try:
             subprocess.call(['mpirun', '--version'])
         except FileNotFoundError:
-            unittest.skipTest('mpirun not found, skipping tests')
+            unittest.SkipTest('mpirun not found, skipping tests')
 
     # Run after every test
     def tearDown(self):
         pass
 
     def test_EX_01_Acceleration(self):
         example = 'EX_01_Acceleration.py'
```

### Comparing `blond-2.1.2/unittests/integration/test_validate_gpu.py` & `blond-2.1.3/unittests/integration/test_validate_gpu.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/integration/test_validate_mpi.py` & `blond-2.1.3/unittests/integration/test_validate_mpi.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/ref_DV_MOD_FR.npy` & `blond-2.1.3/unittests/llrf/ref_DV_MOD_FR.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/ref_DV_MOD_FRF.npy` & `blond-2.1.3/unittests/llrf/ref_DV_MOD_FRF.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/ref_V_IND_COARSE_GEN.npy` & `blond-2.1.3/unittests/llrf/ref_V_IND_COARSE_GEN.npy`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/test_beam_feedback.py` & `blond-2.1.3/unittests/llrf/test_beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/test_cavity_feedback.py` & `blond-2.1.3/unittests/llrf/test_cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/test_impulse_response.py` & `blond-2.1.3/unittests/llrf/test_impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/test_offset_frequency.py` & `blond-2.1.3/unittests/llrf/test_offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/test_rf_modulation.py` & `blond-2.1.3/unittests/llrf/test_rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/llrf/test_signal_processing.py` & `blond-2.1.3/unittests/llrf/test_signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/synchrotron_radiation/test_synch_rad.py` & `blond-2.1.3/unittests/synchrotron_radiation/test_synch_rad.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/trackers/comparison_drift.py` & `blond-2.1.3/unittests/trackers/comparison_drift.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/trackers/test_drift.py` & `blond-2.1.3/unittests/trackers/test_drift.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/trackers/test_tracker.py` & `blond-2.1.3/unittests/trackers/test_tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/utils/test_blondmath.py` & `blond-2.1.3/unittests/utils/test_blondmath.py`

 * *Files 12% similar despite different names*

```diff
@@ -170,14 +170,16 @@
             impedance_py1, impedance_py2, decimal=decimal)
 
 
 class TestWhere(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest('Compiled blond library not found, skipping test.')
         np.random.seed(0)
         pass
     # Run after every test
 
     def tearDown(self):
         pass
 
@@ -231,15 +233,18 @@
         testing = bm.where_cpp(a, less_than=threshold)
         np.testing.assert_equal(real, testing)
 
 class TestSin(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
+
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_sin_scalar_1(self):
         a = np.random.rand()
@@ -254,15 +259,18 @@
         np.testing.assert_almost_equal(bm.sin_cpp(a), np.sin(a), decimal=8)
 
 
 class TestCos(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
+
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_cos_scalar_1(self):
         a = np.random.rand()
@@ -277,15 +285,17 @@
         np.testing.assert_almost_equal(bm.cos_cpp(a), np.cos(a), decimal=8)
 
 
 class TestExp(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_exp_scalar_1(self):
         a = np.random.rand()
@@ -296,15 +306,17 @@
         np.testing.assert_almost_equal(bm.exp_cpp(a), np.exp(a), decimal=8)
 
 
 class TestMean(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_mean_1(self):
         a = np.random.randn(100)
@@ -315,15 +327,17 @@
         np.testing.assert_almost_equal(bm.mean_cpp(a), np.mean(a), decimal=8)
 
 
 class TestStd(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_std_1(self):
         a = np.random.randn(100)
@@ -334,15 +348,17 @@
         np.testing.assert_almost_equal(bm.std_cpp(a), np.std(a), decimal=8)
 
 
 class TestSum(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_sum_1(self):
         a = np.random.randn(100)
@@ -353,15 +369,17 @@
         np.testing.assert_almost_equal(bm.sum_cpp(a), np.sum(a), decimal=8)
 
 
 class TestLinspace(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_linspace_1(self):
         start = 0.
@@ -391,15 +409,17 @@
                                        np.linspace(start, stop, num), decimal=8)
 
 
 class TestArange(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_arange_1(self):
         start = 0.
@@ -431,15 +451,17 @@
                                        np.arange(start, stop, step), decimal=8)
 
 
 class TestArgMin(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_min_idx_1(self):
         a = np.random.randn(100)
@@ -450,15 +472,17 @@
         np.testing.assert_equal(bm.argmin_cpp(a), np.argmin(a))
 
 
 class TestArgMax(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_max_idx_1(self):
         a = np.random.randn(100)
@@ -469,15 +493,17 @@
         np.testing.assert_equal(bm.argmax_cpp(a), np.argmax(a))
 
 
 class TestConvolve(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_convolve_1(self):
         s = np.random.randn(100)
@@ -495,15 +521,17 @@
             bm.convolve(s, k, mode='valid')
 
 
 class TestInterp(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_interp_1(self):
         x = np.random.randn(100)
@@ -539,15 +567,17 @@
                                        np.interp(x, xp, yp, 0., 1.), decimal=8)
 
 
 class TestTrapz(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_trapz_1(self):
         y = np.random.randn(100)
@@ -565,15 +595,17 @@
                                        np.trapz(y, dx=0.1), decimal=8)
 
 
 class TestCumTrapz(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_cumtrapz_1(self):
         import scipy.integrate
@@ -610,15 +642,17 @@
                                        decimal=8)
 
 
 class TestSort(unittest.TestCase):
 
     # Run before every test
     def setUp(self):
-        pass
+        if bm.device != 'CPU_CPP':
+            raise unittest.SkipTest(
+                'Compiled blond library not found, skipping test.')
     # Run after every test
 
     def tearDown(self):
         pass
 
     def test_sort_1(self):
         y = np.random.randn(100)
```

### Comparing `blond-2.1.2/unittests/utils/test_data_check.py` & `blond-2.1.3/unittests/utils/test_data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/utils/test_ffts.py` & `blond-2.1.3/unittests/utils/test_ffts.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.2/unittests/utils/test_iteration.py` & `blond-2.1.3/unittests/utils/test_iteration.py`

 * *Files identical despite different names*

