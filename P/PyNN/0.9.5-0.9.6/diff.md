# Comparing `tmp/PyNN-0.9.5.tar.gz` & `tmp/PyNN-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyNN-0.9.5.tar", last modified: Thu Dec  5 09:39:33 2019, max compression
+gzip compressed data, was "dist/PyNN-0.9.6.tar", last modified: Tue Dec 22 14:19:24 2020, max compression
```

## Comparing `PyNN-0.9.5.tar` & `PyNN-0.9.6.tar`

### file list

```diff
@@ -1,489 +1,491 @@
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/
--rw-r--r--   0 andrew     (503) staff       (20)     1364 2019-09-02 15:20:52.000000 PyNN-0.9.5/.gitignore
--rw-r--r--   0 andrew     (503) staff       (20)      452 2019-11-14 14:06:45.000000 PyNN-0.9.5/.travis.yml
--rw-r--r--   0 andrew     (503) staff       (20)     2170 2019-11-14 14:06:45.000000 PyNN-0.9.5/AUTHORS
--rw-r--r--   0 andrew     (503) staff       (20)     3228 2019-09-02 15:18:12.000000 PyNN-0.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 andrew     (503) staff       (20)       69 2019-09-02 15:18:12.000000 PyNN-0.9.5/CONTRIBUTING.md
--rw-r--r--   0 andrew     (503) staff       (20)    21097 2019-01-07 20:00:27.000000 PyNN-0.9.5/LICENSE
--rw-r--r--   0 andrew     (503) staff       (20)      491 2019-09-02 15:20:52.000000 PyNN-0.9.5/MANIFEST.in
--rw-r--r--   0 andrew     (503) staff       (20)     3522 2019-12-05 09:39:33.000000 PyNN-0.9.5/PKG-INFO
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/PyNN.egg-info/
--rw-r--r--   0 andrew     (503) staff       (20)     3522 2019-12-05 09:39:33.000000 PyNN-0.9.5/PyNN.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (503) staff       (20)    13618 2019-12-05 09:39:33.000000 PyNN-0.9.5/PyNN.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (503) staff       (20)        1 2019-12-05 09:39:33.000000 PyNN-0.9.5/PyNN.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (503) staff       (20)      147 2019-12-05 09:39:33.000000 PyNN-0.9.5/PyNN.egg-info/requires.txt
--rw-r--r--   0 andrew     (503) staff       (20)        5 2019-12-05 09:39:33.000000 PyNN-0.9.5/PyNN.egg-info/top_level.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1987 2019-11-14 14:06:45.000000 PyNN-0.9.5/README.rst
--rw-r--r--   0 andrew     (503) staff       (20)    41660 2019-01-07 20:00:27.000000 PyNN-0.9.5/changelog
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/ci/
--rw-r--r--   0 andrew     (503) staff       (20)      349 2019-09-02 15:18:12.000000 PyNN-0.9.5/ci/install.sh
--rw-r--r--   0 andrew     (503) staff       (20)      233 2019-01-07 20:00:27.000000 PyNN-0.9.5/ci/install_brian.sh
--rw-r--r--   0 andrew     (503) staff       (20)     1752 2019-11-14 14:06:45.000000 PyNN-0.9.5/ci/install_nest.sh
--rw-r--r--   0 andrew     (503) staff       (20)     1240 2019-09-02 15:18:12.000000 PyNN-0.9.5/ci/install_neuron.sh
--rw-r--r--   0 andrew     (503) staff       (20)      419 2019-09-02 15:18:12.000000 PyNN-0.9.5/ci/test_script.sh
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/
--rw-r--r--   0 andrew     (503) staff       (20)     4720 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/Makefile
--rw-r--r--   0 andrew     (503) staff       (20)      378 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/README
--rw-r--r--   0 andrew     (503) staff       (20)      345 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/api_reference.txt
--rw-r--r--   0 andrew     (503) staff       (20)   188761 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/architecture_of_PyNN.svg
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/backends/
--rw-r--r--   0 andrew     (503) staff       (20)       19 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends/Brian.txt
--rw-r--r--   0 andrew     (503) staff       (20)       18 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends/MOOSE.txt
--rw-r--r--   0 andrew     (503) staff       (20)     5579 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/backends/NEST.txt
--rw-r--r--   0 andrew     (503) staff       (20)     5081 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/backends/NEURON.txt
--rw-r--r--   0 andrew     (503) staff       (20)       16 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends/NeMo.txt
--rw-r--r--   0 andrew     (503) staff       (20)      171 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends/NeuroML.txt
--rw-r--r--   0 andrew     (503) staff       (20)       74 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends/NineML.txt
--rw-r--r--   0 andrew     (503) staff       (20)       66 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends/neuromorphic.txt
--rw-r--r--   0 andrew     (503) staff       (20)      634 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/backends.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3898 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/build_examples.py
--rw-r--r--   0 andrew     (503) staff       (20)      126 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/building_networks.txt
--rw-r--r--   0 andrew     (503) staff       (20)     9454 2019-11-14 14:06:45.000000 PyNN-0.9.5/doc/conf.py
--rw-r--r--   0 andrew     (503) staff       (20)    21256 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/connections.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1290 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/contributors.txt
--rw-r--r--   0 andrew     (503) staff       (20)     5920 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/data_handling.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3885 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/descriptions.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/developers/
--rw-r--r--   0 andrew     (503) staff       (20)     6400 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/developers/adding_backend.txt
--rw-r--r--   0 andrew     (503) staff       (20)      422 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/developers/bug_reports.txt
--rw-r--r--   0 andrew     (503) staff       (20)     9704 2019-09-02 15:18:12.000000 PyNN-0.9.5/doc/developers/contributing.txt
--rw-r--r--   0 andrew     (503) staff       (20)     4722 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/developers/governance.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1078 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/developers_guide.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1795 2019-12-04 16:47:19.000000 PyNN-0.9.5/doc/download.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/examples/
--rw-r--r--   0 andrew     (503) staff       (20)      190 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/Izhikevich.txt
--rw-r--r--   0 andrew     (503) staff       (20)      230 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/VAbenchmarks.txt
--rw-r--r--   0 andrew     (503) staff       (20)      324 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/cell_type_demonstration.txt
--rw-r--r--   0 andrew     (503) staff       (20)      220 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/current_injection.txt
--rw-r--r--   0 andrew     (503) staff       (20)      315 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/random_distributions.txt
--rw-r--r--   0 andrew     (503) staff       (20)      240 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/random_numbers.txt
--rw-r--r--   0 andrew     (503) staff       (20)      194 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/simple_STDP.txt
--rw-r--r--   0 andrew     (503) staff       (20)      258 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/small_network.txt
--rw-r--r--   0 andrew     (503) staff       (20)      334 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/stochastic_deterministic_comparison.txt
--rw-r--r--   0 andrew     (503) staff       (20)      213 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/stochastic_synapses.txt
--rw-r--r--   0 andrew     (503) staff       (20)      302 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/synaptic_input.txt
--rw-r--r--   0 andrew     (503) staff       (20)      222 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/tsodyksmarkram.txt
--rw-r--r--   0 andrew     (503) staff       (20)      292 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples/varying_poisson.txt
--rw-r--r--   0 andrew     (503) staff       (20)      444 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/examples.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/images/
--rw-r--r--   0 andrew     (503) staff       (20)    33178 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/ac_source.png
--rw-r--r--   0 andrew     (503) staff       (20)    37296 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/continuous_time_spiking.png
--rw-r--r--   0 andrew     (503) staff       (20)    20389 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/dc_source.png
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/images/examples/
--rw-r--r--   0 andrew     (503) staff       (20)    41405 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/Izhikevich_nest_np1_20170505-150315.png
--rw-r--r--   0 andrew     (503) staff       (20)   781288 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/VAbenchmarks_CUBA_20170505-150538.png
--rw-r--r--   0 andrew     (503) staff       (20)   186373 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/cell_type_demonstration_nest_20170505-150320.png
--rw-r--r--   0 andrew     (503) staff       (20)    42169 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/current_injection_neuron_20170505-150317.png
--rw-r--r--   0 andrew     (503) staff       (20)   147086 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/random_distributions.png
--rw-r--r--   0 andrew     (503) staff       (20)    29149 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/random_numbers_neuron_20170505-150323.png
--rw-r--r--   0 andrew     (503) staff       (20)    87839 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/simple_stdp_neuron_20170505-150331.png
--rw-r--r--   0 andrew     (503) staff       (20)   156007 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/small_network_nest_np1_20170505-150334.png
--rw-r--r--   0 andrew     (503) staff       (20)   138718 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/stochastic_comparison_neuron_20170505-150418.png
--rw-r--r--   0 andrew     (503) staff       (20)   114780 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/stochastic_synapses__nest_20170505-150345.png
--rw-r--r--   0 andrew     (503) staff       (20)   161351 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/synaptic_input_neuron_20170505-150337.png
--rw-r--r--   0 andrew     (503) staff       (20)   274993 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/tsodyksmarkram_nest_20170505-150340.png
--rw-r--r--   0 andrew     (503) staff       (20)    52334 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/examples/varying_poisson_neuron_20170505-150343.png
--rw-r--r--   0 andrew     (503) staff       (20)    86593 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/neo_example.png
--rw-r--r--   0 andrew     (503) staff       (20)    44050 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/noise_source.png
--rw-r--r--   0 andrew     (503) staff       (20)    36721 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/ongridoffgrid.png
--rw-r--r--   0 andrew     (503) staff       (20)   213980 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/release_0.8b1_example.png
--rw-r--r--   0 andrew     (503) staff       (20)    54758 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/reset_example.png
--rw-r--r--   0 andrew     (503) staff       (20)    21713 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/step_source.png
--rw-r--r--   0 andrew     (503) staff       (20)    33178 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/images/tmp.png
--rw-r--r--   0 andrew     (503) staff       (20)     2187 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/import_export.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1090 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/index.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1731 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/injecting_current.txt
--rw-r--r--   0 andrew     (503) staff       (20)     6202 2019-11-14 14:06:45.000000 PyNN-0.9.5/doc/installation.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3334 2019-09-02 15:18:12.000000 PyNN-0.9.5/doc/introduction.txt
--rw-r--r--   0 andrew     (503) staff       (20)     2339 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/logging.txt
--rw-r--r--   0 andrew     (503) staff       (20)     4507 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/make.bat
--rw-r--r--   0 andrew     (503) staff       (20)    16146 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/neurons.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3967 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/nineml.txt
--rw-r--r--   0 andrew     (503) staff       (20)     4387 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/parallel.txt
--rw-r--r--   0 andrew     (503) staff       (20)     7794 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/parameters.txt
--rw-r--r--   0 andrew     (503) staff       (20)     7103 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/publications.txt
--rw-r--r--   0 andrew     (503) staff       (20)      318 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyNN_icon.ico
--rw-r--r--   0 andrew     (503) staff       (20)     4431 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyNN_logo.png
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/pyplots/
--rw-r--r--   0 andrew     (503) staff       (20)      695 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/ac_source.py
--rw-r--r--   0 andrew     (503) staff       (20)     1367 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/continuous_time_spiking.py
--rw-r--r--   0 andrew     (503) staff       (20)      619 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/dc_source.py
--rw-r--r--   0 andrew     (503) staff       (20)     2141 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/neo_example.py
--rw-r--r--   0 andrew     (503) staff       (20)      684 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/noise_source.py
--rw-r--r--   0 andrew     (503) staff       (20)     1327 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/plot_current_source.py
--rw-r--r--   0 andrew     (503) staff       (20)     1617 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/plot_helper.py
--rw-r--r--   0 andrew     (503) staff       (20)      795 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/reset_example.py
--rw-r--r--   0 andrew     (503) staff       (20)      734 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/pyplots/step_source.py
--rw-r--r--   0 andrew     (503) staff       (20)       46 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/quickstart.txt
--rw-r--r--   0 andrew     (503) staff       (20)     6701 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/random_numbers.txt
--rw-r--r--   0 andrew     (503) staff       (20)     2608 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/recording.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/reference/
--rw-r--r--   0 andrew     (503) staff       (20)      775 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/connectors.txt
--rw-r--r--   0 andrew     (503) staff       (20)      768 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/electrodes.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3963 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/neuronmodels.txt
--rw-r--r--   0 andrew     (503) staff       (20)     7437 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/parameters.txt
--rw-r--r--   0 andrew     (503) staff       (20)     2442 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/plasticitymodels.txt
--rw-r--r--   0 andrew     (503) staff       (20)     2305 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/populations.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1025 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/projections.txt
--rw-r--r--   0 andrew     (503) staff       (20)      671 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/random.txt
--rw-r--r--   0 andrew     (503) staff       (20)      621 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/simulationcontrol.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1140 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/space.txt
--rw-r--r--   0 andrew     (503) staff       (20)      706 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/reference/utility.txt
--rw-r--r--   0 andrew     (503) staff       (20)      471 2019-12-04 16:48:17.000000 PyNN-0.9.5/doc/release_notes.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/doc/releases/
--rw-r--r--   0 andrew     (503) staff       (20)     4620 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.6.txt
--rw-r--r--   0 andrew     (503) staff       (20)    10724 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.7.txt
--rw-r--r--   0 andrew     (503) staff       (20)    14520 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8-alpha-1.txt
--rw-r--r--   0 andrew     (503) staff       (20)      726 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8-alpha-2.txt
--rw-r--r--   0 andrew     (503) staff       (20)     5245 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8-beta-1.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3983 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8-beta-2.txt
--rw-r--r--   0 andrew     (503) staff       (20)      757 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8.0-rc-1.txt
--rw-r--r--   0 andrew     (503) staff       (20)    20121 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8.0.txt
--rw-r--r--   0 andrew     (503) staff       (20)      439 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8.1.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1354 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8.2.txt
--rw-r--r--   0 andrew     (503) staff       (20)      770 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.8.3.txt
--rw-r--r--   0 andrew     (503) staff       (20)      915 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.9.0.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1185 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/releases/0.9.1.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1481 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/releases/0.9.2.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3259 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/releases/0.9.3.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1102 2019-09-02 15:20:52.000000 PyNN-0.9.5/doc/releases/0.9.4.txt
--rw-r--r--   0 andrew     (503) staff       (20)      364 2019-12-05 09:38:14.000000 PyNN-0.9.5/doc/releases/0.9.5.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1836 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/roadmap.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3491 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/simulation_control.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3876 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/space.txt
--rw-r--r--   0 andrew     (503) staff       (20)     9354 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/standardmodels.txt
--rw-r--r--   0 andrew     (503) staff       (20)     4040 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/testdocs.py
--rw-r--r--   0 andrew     (503) staff       (20)      432 2019-01-07 20:00:27.000000 PyNN-0.9.5/doc/units.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/examples/
--rw-r--r--   0 andrew     (503) staff       (20)     1283 2019-09-21 23:57:39.000000 PyNN-0.9.5/examples/FakeStepCurrentSource.py
--rw-r--r--   0 andrew     (503) staff       (20)     2095 2019-09-02 15:20:52.000000 PyNN-0.9.5/examples/HH_cond_exp2.py
--rw-r--r--   0 andrew     (503) staff       (20)     2260 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/Izhikevich.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/examples/Potjans2014/
--rw-r--r--   0 andrew     (503) staff       (20)     3815 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/README.txt
--rw-r--r--   0 andrew     (503) staff       (20)      901 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/connectivity.py
--rw-r--r--   0 andrew     (503) staff       (20)     2520 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/microcircuit.py
--rw-r--r--   0 andrew     (503) staff       (20)     6738 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/network.py
--rw-r--r--   0 andrew     (503) staff       (20)     6009 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/network_params.py
--rw-r--r--   0 andrew     (503) staff       (20)     2659 2019-09-02 15:18:12.000000 PyNN-0.9.5/examples/Potjans2014/plotting.py
--rw-r--r--   0 andrew     (503) staff       (20)     1304 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/run_microcircuit.py
--rw-r--r--   0 andrew     (503) staff       (20)     2280 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/scaling.py
--rw-r--r--   0 andrew     (503) staff       (20)      996 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/Potjans2014/sim_params.py
--rw-r--r--   0 andrew     (503) staff       (20)     4832 2019-09-02 15:18:12.000000 PyNN-0.9.5/examples/Potjans2014/validation_microcircuit.py
--rw-r--r--   0 andrew     (503) staff       (20)      702 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/README
--rw-r--r--   0 andrew     (503) staff       (20)      662 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/StepCurrentSource.py
--rw-r--r--   0 andrew     (503) staff       (20)    10994 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/VAbenchmarks.py
--rw-r--r--   0 andrew     (503) staff       (20)     3860 2019-02-07 15:54:52.000000 PyNN-0.9.5/examples/ball_and_stick.py
--rw-r--r--   0 andrew     (503) staff       (20)     8374 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/brunel.py
--rw-r--r--   0 andrew     (503) staff       (20)     3572 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/cell_type_demonstration.py
--rw-r--r--   0 andrew     (503) staff       (20)     1402 2019-02-07 15:54:52.000000 PyNN-0.9.5/examples/connection_plot.py
--rw-r--r--   0 andrew     (503) staff       (20)    10161 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/connections.py
--rw-r--r--   0 andrew     (503) staff       (20)     2477 2019-04-29 20:34:57.000000 PyNN-0.9.5/examples/current_injection.py
--rw-r--r--   0 andrew     (503) staff       (20)     1793 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/distrib_example.py
--rw-r--r--   0 andrew     (503) staff       (20)     4868 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/gif_neuron.py
--rw-r--r--   0 andrew     (503) staff       (20)     4872 2019-02-07 15:54:52.000000 PyNN-0.9.5/examples/gif_neuron_tmp.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/examples/iaf_sfa_relref/
--rw-r--r--   0 andrew     (503) staff       (20)     1599 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/README
--rw-r--r--   0 andrew     (503) staff       (20)     3306 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/backend_comparison.py
--rw-r--r--   0 andrew     (503) staff       (20)    20432 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/iaf_sfa_network_INH_GAMMA.py
--rw-r--r--   0 andrew     (503) staff       (20)    18105 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/iaf_sfa_network_STATIC.py
--rw-r--r--   0 andrew     (503) staff       (20)     2347 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/mcb.py
--rw-r--r--   0 andrew     (503) staff       (20)    91116 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/myFigure_expected.pdf
--rw-r--r--   0 andrew     (503) staff       (20)      971 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/iaf_sfa_relref/standard_neurons.yaml
--rw-r--r--   0 andrew     (503) staff       (20)      645 2019-02-07 15:54:52.000000 PyNN-0.9.5/examples/iclamp_test.py
--rw-r--r--   0 andrew     (503) staff       (20)     2509 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/inhomogeneous_network.py
--rw-r--r--   0 andrew     (503) staff       (20)     4208 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/multiquantal_synapses.py
--rw-r--r--   0 andrew     (503) staff       (20)     3540 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/nineml_brunel.py
--rw-r--r--   0 andrew     (503) staff       (20)     4477 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/nineml_neuron.py
--rw-r--r--   0 andrew     (503) staff       (20)     3882 2019-02-07 15:54:52.000000 PyNN-0.9.5/examples/nineml_stdp.py
--rw-r--r--   0 andrew     (503) staff       (20)     2652 2019-09-02 15:20:52.000000 PyNN-0.9.5/examples/nrn_artificial_cell.py
--rw-r--r--   0 andrew     (503) staff       (20)      629 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/parameter_changes.py
--rw-r--r--   0 andrew     (503) staff       (20)     2208 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/random_distributions.py
--rw-r--r--   0 andrew     (503) staff       (20)     4210 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/random_numbers.py
--rw-r--r--   0 andrew     (503) staff       (20)     2768 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/simpleRandomNetwork.py
--rw-r--r--   0 andrew     (503) staff       (20)     2250 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/simpleRandomNetwork_csa.py
--rw-r--r--   0 andrew     (503) staff       (20)     8279 2019-11-14 10:10:41.000000 PyNN-0.9.5/examples/simple_STDP.py
--rw-r--r--   0 andrew     (503) staff       (20)     3505 2019-09-02 15:20:52.000000 PyNN-0.9.5/examples/small_network.py
--rw-r--r--   0 andrew     (503) staff       (20)     2629 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/specific_network.py
--rw-r--r--   0 andrew     (503) staff       (20)     3715 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/stdp_network.py
--rw-r--r--   0 andrew     (503) staff       (20)     4754 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/stochastic_deterministic_comparison.py
--rw-r--r--   0 andrew     (503) staff       (20)     2890 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/stochastic_synapses.py
--rw-r--r--   0 andrew     (503) staff       (20)     3907 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/stochastic_tsodyksmarkram.py
--rw-r--r--   0 andrew     (503) staff       (20)     3918 2019-02-07 15:54:52.000000 PyNN-0.9.5/examples/stochastic_tsodyksmarkram_em.py
--rw-r--r--   0 andrew     (503) staff       (20)     5177 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/synaptic_input.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/examples/tools/
--rw-r--r--   0 andrew     (503) staff       (20)     7451 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/tools/VAbenchmark_graphs.py
--rw-r--r--   0 andrew     (503) staff       (20)     2863 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/tools/comparison_plot.py
--rw-r--r--   0 andrew     (503) staff       (20)     2283 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/tools/plot_results.py
--rw-r--r--   0 andrew     (503) staff       (20)     2363 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/tools/run_all_examples.py
--rw-r--r--   0 andrew     (503) staff       (20)     3531 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/tsodyksmarkram.py
--rw-r--r--   0 andrew     (503) staff       (20)     3609 2019-09-02 15:20:52.000000 PyNN-0.9.5/examples/update_spike_source_array.py
--rw-r--r--   0 andrew     (503) staff       (20)     3030 2019-01-07 20:00:27.000000 PyNN-0.9.5/examples/varying_poisson.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/
--rw-r--r--   0 andrew     (503) staff       (20)     2696 2019-12-04 16:49:01.000000 PyNN-0.9.5/pyNN/__init__.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/brian/
--rw-r--r--   0 andrew     (503) staff       (20)     2727 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/brian/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    10281 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/brian/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     3850 2019-09-02 15:06:06.000000 PyNN-0.9.5/pyNN/brian/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)    11921 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/brian/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)     4879 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/brian/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     3331 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/brian/simulator.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/brian/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/brian/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    14104 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/brian/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)    10792 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/brian/standardmodels/electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)     7403 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/brian/standardmodels/synapses.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/common/
--rw-r--r--   0 andrew     (503) staff       (20)     1412 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/common/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     6047 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/common/control.py
--rw-r--r--   0 andrew     (503) staff       (20)    62053 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/common/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)     4173 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/common/procedural_api.py
--rw-r--r--   0 andrew     (503) staff       (20)    22202 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/common/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)    48224 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)     2474 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/core.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/descriptions/
--rw-r--r--   0 andrew     (503) staff       (20)     6367 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/descriptions/__init__.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/descriptions/templates/
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/
--rw-r--r--   0 andrew     (503) staff       (20)      136 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/assembly_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)        5 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/modeltype_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      450 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/population_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      484 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/population_old.txt
--rw-r--r--   0 andrew     (503) staff       (20)       90 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/populationview_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      370 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/projection_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)       76 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/cheetah/synapsedynamics_default.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/
--rw-r--r--   0 andrew     (503) staff       (20)      149 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/assembly_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)        8 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/modeltype_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      486 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/population_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      541 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/population_old.txt
--rw-r--r--   0 andrew     (503) staff       (20)      102 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/populationview_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)     1179 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/projection_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)       82 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/jinja2/synapsedynamics_default.txt
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/
--rw-r--r--   0 andrew     (503) staff       (20)       94 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/assembly_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)        5 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/modeltype_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      226 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/population_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)       90 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/populationview_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)      198 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/projection_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)       76 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/descriptions/templates/string/synapsedynamics_default.txt
--rw-r--r--   0 andrew     (503) staff       (20)     2578 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/errors.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/hardware/
--rw-r--r--   0 andrew     (503) staff       (20)      561 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/hardware/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     2779 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/hardware/aux.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/mock/
--rw-r--r--   0 andrew     (503) staff       (20)     2409 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/mock/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     3144 2019-04-07 14:59:32.000000 PyNN-0.9.5/pyNN/mock/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)     2193 2019-04-04 13:18:52.000000 PyNN-0.9.5/pyNN/mock/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)     1254 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/mock/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)      965 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/mock/simulator.py
--rw-r--r--   0 andrew     (503) staff       (20)     9482 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/mock/standardmodels.py
--rw-r--r--   0 andrew     (503) staff       (20)     4017 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/models.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/moose/
--rw-r--r--   0 andrew     (503) staff       (20)     9004 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/moose/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     7239 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/moose/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     3283 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/moose/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     1929 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/moose/simple_example.py
--rw-r--r--   0 andrew     (503) staff       (20)     3076 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/moose/simulator.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/moose/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/moose/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     2845 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/moose/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     3428 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/multisim.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nemo/
--rw-r--r--   0 andrew     (503) staff       (20)    19198 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     1045 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)     3259 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     6617 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/simulator.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nemo/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nemo/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     5965 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     1525 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/standardmodels/electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)     1842 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nemo/standardmodels/synapses.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nest/
--rw-r--r--   0 andrew     (503) staff       (20)     6995 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     3343 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     9217 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)     2460 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nest/conversion.py
--rw-r--r--   0 andrew     (503) staff       (20)     3759 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/nest/electrodes.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nest/extensions/
--rw-r--r--   0 andrew     (503) staff       (20)     9207 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/CMakeLists.txt
--rw-r--r--   0 andrew     (503) staff       (20)     3891 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/pynn_extensions.cpp
--rw-r--r--   0 andrew     (503) staff       (20)     1316 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/pynn_extensions.h
--rw-r--r--   0 andrew     (503) staff       (20)     5581 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/simple_stochastic_connection.h
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nest/extensions/sli/
--rw-r--r--   0 andrew     (503) staff       (20)      317 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/sli/pynn_extensions-init.sli
--rw-r--r--   0 andrew     (503) staff       (20)     5970 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/stochastic_stp_connection.h
--rw-r--r--   0 andrew     (503) staff       (20)     2109 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/extensions/stochastic_stp_connection_impl.h
--rw-r--r--   0 andrew     (503) staff       (20)     5320 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/nineml.py
--rw-r--r--   0 andrew     (503) staff       (20)     8136 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)    20120 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/nest/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)     3191 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nest/random.py
--rw-r--r--   0 andrew     (503) staff       (20)    20281 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     8648 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/nest/simulator.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nest/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nest/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    12299 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     7728 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/standardmodels/electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)     7617 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/standardmodels/synapses.py
--rw-r--r--   0 andrew     (503) staff       (20)     2774 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nest/synapses.py
--rw-r--r--   0 andrew     (503) staff       (20)     3885 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/network.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/neuroml/
--rw-r--r--   0 andrew     (503) staff       (20)     3834 2019-09-02 15:20:52.000000 PyNN-0.9.5/pyNN/neuroml/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     5538 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/neuroml/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)     6793 2019-09-02 15:20:52.000000 PyNN-0.9.5/pyNN/neuroml/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)     3775 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/neuroml/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     2658 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/neuroml/simulator.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/neuroml/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuroml/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     9551 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/neuroml/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     6398 2019-09-02 15:18:12.000000 PyNN-0.9.5/pyNN/neuroml/standardmodels/electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)     3827 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuroml/standardmodels/synapses.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/neuron/
--rw-r--r--   0 andrew     (503) staff       (20)     4938 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    24673 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     1008 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)     3566 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/nineml.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/neuron/nmodl/
--rw-r--r--   0 andrew     (503) staff       (20)     3582 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/adexp.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1530 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/alphaisyn.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1574 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/alphasyn.mod
--rwxr-xr-x   0 andrew     (503) staff       (20)      377 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/expisyn.mod
--rw-r--r--   0 andrew     (503) staff       (20)     2406 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/gammastim.mod
--rw-r--r--   0 andrew     (503) staff       (20)      322 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/gap.mod
--rw-r--r--   0 andrew     (503) staff       (20)     5180 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/gif.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1670 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/gsfa_grr.mod
--rwxr-xr-x   0 andrew     (503) staff       (20)     2353 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/hh_traub.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1390 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/izhikevich.mod
--rwxr-xr-x   0 andrew     (503) staff       (20)     5227 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/netstim2.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1300 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/poisson_stim_refractory.mod
--rw-r--r--   0 andrew     (503) staff       (20)     2838 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/quantal_stp.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1695 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/refrac.mod
--rw-r--r--   0 andrew     (503) staff       (20)      609 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/reset.mod
--rw-r--r--   0 andrew     (503) staff       (20)     2018 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_guetig.mod
--rw-r--r--   0 andrew     (503) staff       (20)     2025 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_softlimits.mod
--rw-r--r--   0 andrew     (503) staff       (20)     2283 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_songabbott.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1969 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_symm.mod
--rw-r--r--   0 andrew     (503) staff       (20)     2375 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_vogels2011.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1574 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stochastic_synapse.mod
--rw-r--r--   0 andrew     (503) staff       (20)     3290 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/stochastic_tsodyksmarkram.mod
--rw-r--r--   0 andrew     (503) staff       (20)     4840 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/tmgsyn.mod
--rw-r--r--   0 andrew     (503) staff       (20)     4825 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/tmisyn.mod
--rw-r--r--   0 andrew     (503) staff       (20)     1248 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/tsodyksmarkram.mod
--rw-r--r--   0 andrew     (503) staff       (20)     5000 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/nmodl/vecstim.mod
--rw-r--r--   0 andrew     (503) staff       (20)     5638 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)     7227 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)     3541 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/random.py
--rw-r--r--   0 andrew     (503) staff       (20)     5165 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)    23718 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/simulator.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/neuron/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/neuron/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     8797 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     9445 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/standardmodels/electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)     6313 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/neuron/standardmodels/synapses.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/nineml/
--rw-r--r--   0 andrew     (503) staff       (20)     3808 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nineml/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     4491 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nineml/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     1532 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nineml/connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)     4776 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nineml/populations.py
--rw-r--r--   0 andrew     (503) staff       (20)     2239 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nineml/projections.py
--rw-r--r--   0 andrew     (503) staff       (20)    15307 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nineml/read.py
--rw-r--r--   0 andrew     (503) staff       (20)      664 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nineml/recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     1023 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nineml/simulator.py
--rw-r--r--   0 andrew     (503) staff       (20)    15363 2019-01-07 20:00:27.000000 PyNN-0.9.5/pyNN/nineml/standardmodels.py
--rw-r--r--   0 andrew     (503) staff       (20)      267 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nineml/synapses.py
--rw-r--r--   0 andrew     (503) staff       (20)     4394 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/nineml/utility.py
--rw-r--r--   0 andrew     (503) staff       (20)    19074 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/parameters.py
--rw-r--r--   0 andrew     (503) staff       (20)    18781 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/random.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/recording/
--rw-r--r--   0 andrew     (503) staff       (20)    15692 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/recording/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     8841 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/recording/files.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/serialization/
--rw-r--r--   0 andrew     (503) staff       (20)      165 2019-09-02 15:20:52.000000 PyNN-0.9.5/pyNN/serialization/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    51176 2019-12-04 16:46:00.000000 PyNN-0.9.5/pyNN/serialization/sonata.py
--rw-r--r--   0 andrew     (503) staff       (20)    14325 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/space.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/standardmodels/
--rw-r--r--   0 andrew     (503) staff       (20)    13141 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/standardmodels/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    23371 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/standardmodels/cells.py
--rw-r--r--   0 andrew     (503) staff       (20)     3347 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/standardmodels/electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)    15134 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/standardmodels/synapses.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/pyNN/utility/
--rw-r--r--   0 andrew     (503) staff       (20)    14413 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/utility/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)    13115 2019-11-14 14:06:45.000000 PyNN-0.9.5/pyNN/utility/plotting.py
--rw-r--r--   0 andrew     (503) staff       (20)      167 2019-09-02 15:20:52.000000 PyNN-0.9.5/requirements.txt
--rw-r--r--   0 andrew     (503) staff       (20)       38 2019-12-05 09:39:33.000000 PyNN-0.9.5/setup.cfg
--rw-r--r--   0 andrew     (503) staff       (20)     5903 2019-12-04 16:47:52.000000 PyNN-0.9.5/setup.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/
--rw-r--r--   0 andrew     (503) staff       (20)      342 2019-09-02 15:18:12.000000 PyNN-0.9.5/test/README
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/benchmarks/
--rw-r--r--   0 andrew     (503) staff       (20)     9111 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/Benchmark_PyNN-0.8dev_FixedNumberPost.py
--rw-r--r--   0 andrew     (503) staff       (20)     1452 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/README.txt
--rw-r--r--   0 andrew     (503) staff       (20)      931 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/all_to_all_network.param
--rw-r--r--   0 andrew     (503) staff       (20)     6697 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/connectors_benchmark.py
--rw-r--r--   0 andrew     (503) staff       (20)      804 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/ddpc.py
--rw-r--r--   0 andrew     (503) staff       (20)       94 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/neurons_no_recording.param
--rw-r--r--   0 andrew     (503) staff       (20)      506 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/neurons_with_recording.param
--rw-r--r--   0 andrew     (503) staff       (20)     3585 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/benchmarks/plot_figure.py
--rw-r--r--   0 andrew     (503) staff       (20)     4426 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/benchmarks/simple_network.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/hardware/
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/hardware/unittests/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/hardware/unittests/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)      805 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/hardware/unittests/launch_test.py
--rw-r--r--   0 andrew     (503) staff       (20)     1603 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/mocks.py
--rw-r--r--   0 andrew     (503) staff       (20)    15606 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/test_assembly.py
--rw-r--r--   0 andrew     (503) staff       (20)    43011 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/test_connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)    20968 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/test_population.py
--rw-r--r--   0 andrew     (503) staff       (20)    17302 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/test_populationview.py
--rw-r--r--   0 andrew     (503) staff       (20)    10272 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/test_projection.py
--rw-r--r--   0 andrew     (503) staff       (20)     2143 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/hardware/unittests/test_simulation_control.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/system/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/__init__.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/system/scenarios/
--rw-r--r--   0 andrew     (503) staff       (20)      769 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)      718 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/issue231.py
--rw-r--r--   0 andrew     (503) staff       (20)      712 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/issue274.py
--rw-r--r--   0 andrew     (503) staff       (20)      350 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/registry.py
--rw-r--r--   0 andrew     (503) staff       (20)     4653 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/scenario1.py
--rw-r--r--   0 andrew     (503) staff       (20)     2234 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/scenario2.py
--rw-r--r--   0 andrew     (503) staff       (20)     3411 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/scenario3.py
--rw-r--r--   0 andrew     (503) staff       (20)     3198 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/scenario4.py
--rw-r--r--   0 andrew     (503) staff       (20)    11544 2019-09-02 15:20:52.000000 PyNN-0.9.5/test/system/scenarios/test_cell_types.py
--rw-r--r--   0 andrew     (503) staff       (20)     1699 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/test_connection_handling.py
--rw-r--r--   0 andrew     (503) staff       (20)    11359 2019-12-04 16:46:00.000000 PyNN-0.9.5/test/system/scenarios/test_connectors.py
--rw-r--r--   0 andrew     (503) staff       (20)    25901 2019-09-02 15:20:52.000000 PyNN-0.9.5/test/system/scenarios/test_electrodes.py
--rw-r--r--   0 andrew     (503) staff       (20)     9687 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/test_parameter_handling.py
--rw-r--r--   0 andrew     (503) staff       (20)     1027 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/test_procedural_api.py
--rw-r--r--   0 andrew     (503) staff       (20)    16020 2019-09-02 15:18:12.000000 PyNN-0.9.5/test/system/scenarios/test_recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     2990 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/test_simulation_control.py
--rw-r--r--   0 andrew     (503) staff       (20)     2341 2019-09-02 15:18:12.000000 PyNN-0.9.5/test/system/scenarios/test_synapse_types.py
--rw-r--r--   0 andrew     (503) staff       (20)     1860 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/scenarios/ticket166.py
--rw-r--r--   0 andrew     (503) staff       (20)     3844 2019-12-05 09:37:11.000000 PyNN-0.9.5/test/system/test_brian.py
--rw-r--r--   0 andrew     (503) staff       (20)     5037 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/test_hardware_brainscales.py
--rw-r--r--   0 andrew     (503) staff       (20)     1574 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/test_moose.py
--rw-r--r--   0 andrew     (503) staff       (20)     9450 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/system/test_nest.py
--rw-r--r--   0 andrew     (503) staff       (20)     1052 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/system/test_neuroml.py
--rw-r--r--   0 andrew     (503) staff       (20)     8761 2019-09-02 15:20:52.000000 PyNN-0.9.5/test/system/test_neuron.py
--rw-r--r--   0 andrew     (503) staff       (20)     1827 2019-09-02 15:20:52.000000 PyNN-0.9.5/test/system/test_serialization.py
-drwxr-xr-x   0 andrew     (503) staff       (20)        0 2019-12-05 09:39:33.000000 PyNN-0.9.5/test/unittests/
--rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/unittests/__init__.py
--rw-r--r--   0 andrew     (503) staff       (20)     2010 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/mocks.py
--rw-r--r--   0 andrew     (503) staff       (20)       28 2019-01-07 20:00:27.000000 PyNN-0.9.5/test/unittests/setup.cfg
--rw-r--r--   0 andrew     (503) staff       (20)    22625 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_assembly.py
--rw-r--r--   0 andrew     (503) staff       (20)     1456 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_brian.py
--rw-r--r--   0 andrew     (503) staff       (20)    51496 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_connectors_parallel.py
--rw-r--r--   0 andrew     (503) staff       (20)    52736 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_connectors_serial.py
--rw-r--r--   0 andrew     (503) staff       (20)      597 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_core.py
--rw-r--r--   0 andrew     (503) staff       (20)     2957 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_descriptions.py
--rw-r--r--   0 andrew     (503) staff       (20)     3426 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_files.py
--rw-r--r--   0 andrew     (503) staff       (20)     4254 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_idmixin.py
--rw-r--r--   0 andrew     (503) staff       (20)     2865 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_lowlevelapi.py
--rw-r--r--   0 andrew     (503) staff       (20)     8078 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_nest.py
--rw-r--r--   0 andrew     (503) staff       (20)    15465 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_neuron.py
--rw-r--r--   0 andrew     (503) staff       (20)    15008 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_parameters.py
--rw-r--r--   0 andrew     (503) staff       (20)    25452 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_population.py
--rw-r--r--   0 andrew     (503) staff       (20)    23196 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_populationview.py
--rw-r--r--   0 andrew     (503) staff       (20)    12275 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_projection.py
--rw-r--r--   0 andrew     (503) staff       (20)    10171 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_random.py
--rw-r--r--   0 andrew     (503) staff       (20)     5455 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_recording.py
--rw-r--r--   0 andrew     (503) staff       (20)     3995 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_simulation_control.py
--rw-r--r--   0 andrew     (503) staff       (20)    11282 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_space.py
--rw-r--r--   0 andrew     (503) staff       (20)     7357 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_standardmodels.py
--rw-r--r--   0 andrew     (503) staff       (20)     2390 2019-11-14 14:06:45.000000 PyNN-0.9.5/test/unittests/test_utility_functions.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/
+-rw-r--r--   0 andrew     (503) staff       (20)     1364 2020-12-09 17:54:24.000000 PyNN-0.9.6/.gitignore
+-rw-r--r--   0 andrew     (503) staff       (20)      504 2020-12-21 16:53:12.000000 PyNN-0.9.6/.travis.yml
+-rw-r--r--   0 andrew     (503) staff       (20)     2409 2020-12-21 16:53:12.000000 PyNN-0.9.6/AUTHORS
+-rw-r--r--   0 andrew     (503) staff       (20)     3228 2019-09-02 15:18:12.000000 PyNN-0.9.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 andrew     (503) staff       (20)       69 2019-09-02 15:18:12.000000 PyNN-0.9.6/CONTRIBUTING.md
+-rw-r--r--   0 andrew     (503) staff       (20)    21097 2019-01-07 20:00:27.000000 PyNN-0.9.6/LICENSE
+-rw-r--r--   0 andrew     (503) staff       (20)      491 2020-12-09 17:54:24.000000 PyNN-0.9.6/MANIFEST.in
+-rw-r--r--   0 andrew     (503) staff       (20)     3422 2020-12-22 14:19:24.000000 PyNN-0.9.6/PKG-INFO
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/PyNN.egg-info/
+-rw-r--r--   0 andrew     (503) staff       (20)     3422 2020-12-22 14:19:24.000000 PyNN-0.9.6/PyNN.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (503) staff       (20)    13566 2020-12-22 14:19:24.000000 PyNN-0.9.6/PyNN.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (503) staff       (20)        1 2020-12-22 14:19:24.000000 PyNN-0.9.6/PyNN.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      148 2020-12-22 14:19:24.000000 PyNN-0.9.6/PyNN.egg-info/requires.txt
+-rw-r--r--   0 andrew     (503) staff       (20)        5 2020-12-22 14:19:24.000000 PyNN-0.9.6/PyNN.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1987 2020-12-22 13:49:02.000000 PyNN-0.9.6/README.rst
+-rw-r--r--   0 andrew     (503) staff       (20)    41660 2019-01-07 20:00:27.000000 PyNN-0.9.6/changelog
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/ci/
+-rw-r--r--   0 andrew     (503) staff       (20)      261 2020-12-21 16:53:12.000000 PyNN-0.9.6/ci/install.sh
+-rw-r--r--   0 andrew     (503) staff       (20)      389 2020-12-21 16:53:12.000000 PyNN-0.9.6/ci/install_brian.sh
+-rw-r--r--   0 andrew     (503) staff       (20)     1752 2020-12-21 16:53:12.000000 PyNN-0.9.6/ci/install_nest.sh
+-rw-r--r--   0 andrew     (503) staff       (20)     1240 2020-12-21 16:53:12.000000 PyNN-0.9.6/ci/install_neuron.sh
+-rw-r--r--   0 andrew     (503) staff       (20)      306 2020-12-21 16:53:12.000000 PyNN-0.9.6/ci/test_script.sh
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/
+-rw-r--r--   0 andrew     (503) staff       (20)     4720 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/Makefile
+-rw-r--r--   0 andrew     (503) staff       (20)      378 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/README
+-rw-r--r--   0 andrew     (503) staff       (20)      345 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/api_reference.txt
+-rw-r--r--   0 andrew     (503) staff       (20)   188761 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/architecture_of_PyNN.svg
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/backends/
+-rw-r--r--   0 andrew     (503) staff       (20)       19 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends/Brian.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       18 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends/MOOSE.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     5579 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/backends/NEST.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     5081 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/backends/NEURON.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       16 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends/NeMo.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      171 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends/NeuroML.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       74 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends/NineML.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       66 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends/neuromorphic.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      634 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/backends.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3898 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/build_examples.py
+-rw-r--r--   0 andrew     (503) staff       (20)      126 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/building_networks.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     9454 2020-12-22 13:47:41.000000 PyNN-0.9.6/doc/conf.py
+-rw-r--r--   0 andrew     (503) staff       (20)    21645 2020-12-22 12:05:03.000000 PyNN-0.9.6/doc/connections.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1290 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/contributors.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     5920 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/data_handling.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3885 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/descriptions.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/developers/
+-rw-r--r--   0 andrew     (503) staff       (20)     6400 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/developers/adding_backend.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      422 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/developers/bug_reports.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     9694 2020-12-21 16:53:12.000000 PyNN-0.9.6/doc/developers/contributing.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     4722 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/developers/governance.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1078 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/developers_guide.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1795 2020-12-22 13:47:41.000000 PyNN-0.9.6/doc/download.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/examples/
+-rw-r--r--   0 andrew     (503) staff       (20)      190 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/Izhikevich.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      230 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/VAbenchmarks.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      324 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/cell_type_demonstration.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      220 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/current_injection.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      315 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/random_distributions.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      240 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/random_numbers.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      194 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/simple_STDP.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      258 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/small_network.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      334 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/stochastic_deterministic_comparison.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      213 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/stochastic_synapses.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      302 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/synaptic_input.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      222 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/tsodyksmarkram.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      292 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples/varying_poisson.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      444 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/examples.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/images/
+-rw-r--r--   0 andrew     (503) staff       (20)    33178 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/ac_source.png
+-rw-r--r--   0 andrew     (503) staff       (20)    37296 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/continuous_time_spiking.png
+-rw-r--r--   0 andrew     (503) staff       (20)    20389 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/dc_source.png
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/images/examples/
+-rw-r--r--   0 andrew     (503) staff       (20)    41405 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/Izhikevich_nest_np1_20170505-150315.png
+-rw-r--r--   0 andrew     (503) staff       (20)   781288 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/VAbenchmarks_CUBA_20170505-150538.png
+-rw-r--r--   0 andrew     (503) staff       (20)   186373 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/cell_type_demonstration_nest_20170505-150320.png
+-rw-r--r--   0 andrew     (503) staff       (20)    42169 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/current_injection_neuron_20170505-150317.png
+-rw-r--r--   0 andrew     (503) staff       (20)   147086 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/random_distributions.png
+-rw-r--r--   0 andrew     (503) staff       (20)    29149 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/random_numbers_neuron_20170505-150323.png
+-rw-r--r--   0 andrew     (503) staff       (20)    87839 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/simple_stdp_neuron_20170505-150331.png
+-rw-r--r--   0 andrew     (503) staff       (20)   156007 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/small_network_nest_np1_20170505-150334.png
+-rw-r--r--   0 andrew     (503) staff       (20)   138718 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/stochastic_comparison_neuron_20170505-150418.png
+-rw-r--r--   0 andrew     (503) staff       (20)   114780 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/stochastic_synapses__nest_20170505-150345.png
+-rw-r--r--   0 andrew     (503) staff       (20)   161351 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/synaptic_input_neuron_20170505-150337.png
+-rw-r--r--   0 andrew     (503) staff       (20)   274993 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/tsodyksmarkram_nest_20170505-150340.png
+-rw-r--r--   0 andrew     (503) staff       (20)    52334 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/examples/varying_poisson_neuron_20170505-150343.png
+-rw-r--r--   0 andrew     (503) staff       (20)    86593 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/neo_example.png
+-rw-r--r--   0 andrew     (503) staff       (20)    44050 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/noise_source.png
+-rw-r--r--   0 andrew     (503) staff       (20)    36721 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/ongridoffgrid.png
+-rw-r--r--   0 andrew     (503) staff       (20)   213980 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/release_0.8b1_example.png
+-rw-r--r--   0 andrew     (503) staff       (20)    54758 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/reset_example.png
+-rw-r--r--   0 andrew     (503) staff       (20)    21713 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/step_source.png
+-rw-r--r--   0 andrew     (503) staff       (20)    33178 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/images/tmp.png
+-rw-r--r--   0 andrew     (503) staff       (20)     2187 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/import_export.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1090 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/index.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1731 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/injecting_current.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     6239 2020-12-21 16:53:12.000000 PyNN-0.9.6/doc/installation.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3334 2019-09-02 15:18:12.000000 PyNN-0.9.6/doc/introduction.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     2339 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/logging.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     4507 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/make.bat
+-rw-r--r--   0 andrew     (503) staff       (20)    16146 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/neurons.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3967 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/nineml.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     4387 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/parallel.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     7794 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/parameters.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     7103 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/publications.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      318 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyNN_icon.ico
+-rw-r--r--   0 andrew     (503) staff       (20)     4431 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyNN_logo.png
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/pyplots/
+-rw-r--r--   0 andrew     (503) staff       (20)      695 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/ac_source.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1367 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/continuous_time_spiking.py
+-rw-r--r--   0 andrew     (503) staff       (20)      619 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/dc_source.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2141 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/neo_example.py
+-rw-r--r--   0 andrew     (503) staff       (20)      684 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/noise_source.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1327 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/plot_current_source.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1617 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/plot_helper.py
+-rw-r--r--   0 andrew     (503) staff       (20)      795 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/reset_example.py
+-rw-r--r--   0 andrew     (503) staff       (20)      734 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/pyplots/step_source.py
+-rw-r--r--   0 andrew     (503) staff       (20)       46 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/quickstart.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     6701 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/random_numbers.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     2608 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/recording.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/reference/
+-rw-r--r--   0 andrew     (503) staff       (20)      775 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/connectors.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      768 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/electrodes.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3963 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/neuronmodels.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     7437 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/parameters.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     2442 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/plasticitymodels.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     2305 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/populations.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1025 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/projections.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      671 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/random.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      621 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/simulationcontrol.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1140 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/space.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      706 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/reference/utility.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      493 2020-12-22 13:47:41.000000 PyNN-0.9.6/doc/release_notes.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/doc/releases/
+-rw-r--r--   0 andrew     (503) staff       (20)     4620 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.6.txt
+-rw-r--r--   0 andrew     (503) staff       (20)    10724 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.7.txt
+-rw-r--r--   0 andrew     (503) staff       (20)    14520 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8-alpha-1.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      726 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8-alpha-2.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     5245 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8-beta-1.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3983 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8-beta-2.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      757 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8.0-rc-1.txt
+-rw-r--r--   0 andrew     (503) staff       (20)    20121 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8.0.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      439 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8.1.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1354 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8.2.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      770 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.8.3.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      915 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.9.0.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1185 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/releases/0.9.1.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1481 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/releases/0.9.2.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3259 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/releases/0.9.3.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1102 2020-12-09 17:54:24.000000 PyNN-0.9.6/doc/releases/0.9.4.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      364 2020-12-21 16:53:12.000000 PyNN-0.9.6/doc/releases/0.9.5.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      809 2020-12-22 13:56:05.000000 PyNN-0.9.6/doc/releases/0.9.6.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1836 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/roadmap.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3491 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/simulation_control.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3876 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/space.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     9354 2020-12-21 16:53:12.000000 PyNN-0.9.6/doc/standardmodels.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     4040 2019-01-07 20:00:27.000000 PyNN-0.9.6/doc/testdocs.py
+-rw-r--r--   0 andrew     (503) staff       (20)      686 2020-12-21 16:53:12.000000 PyNN-0.9.6/doc/units.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/examples/
+-rw-r--r--   0 andrew     (503) staff       (20)     1283 2019-09-21 23:57:39.000000 PyNN-0.9.6/examples/FakeStepCurrentSource.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2095 2020-12-09 17:54:24.000000 PyNN-0.9.6/examples/HH_cond_exp2.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2260 2019-11-14 10:10:41.000000 PyNN-0.9.6/examples/Izhikevich.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/examples/Potjans2014/
+-rw-r--r--   0 andrew     (503) staff       (20)     3815 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/README.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      901 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/connectivity.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2520 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/microcircuit.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6738 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/network.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6009 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/network_params.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2659 2019-09-02 15:18:12.000000 PyNN-0.9.6/examples/Potjans2014/plotting.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1304 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/run_microcircuit.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2280 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/scaling.py
+-rw-r--r--   0 andrew     (503) staff       (20)      996 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/Potjans2014/sim_params.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4832 2019-09-02 15:18:12.000000 PyNN-0.9.6/examples/Potjans2014/validation_microcircuit.py
+-rw-r--r--   0 andrew     (503) staff       (20)      702 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/README
+-rw-r--r--   0 andrew     (503) staff       (20)      662 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/StepCurrentSource.py
+-rw-r--r--   0 andrew     (503) staff       (20)    10994 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/VAbenchmarks.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3860 2019-02-07 15:54:52.000000 PyNN-0.9.6/examples/ball_and_stick.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8374 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/brunel.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3570 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/cell_type_demonstration.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1402 2019-02-07 15:54:52.000000 PyNN-0.9.6/examples/connection_plot.py
+-rw-r--r--   0 andrew     (503) staff       (20)    10161 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/connections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2477 2019-04-29 20:34:57.000000 PyNN-0.9.6/examples/current_injection.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1793 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/distrib_example.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4868 2019-11-14 10:10:41.000000 PyNN-0.9.6/examples/gif_neuron.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4872 2019-02-07 15:54:52.000000 PyNN-0.9.6/examples/gif_neuron_tmp.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/examples/iaf_sfa_relref/
+-rw-r--r--   0 andrew     (503) staff       (20)     1599 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/iaf_sfa_relref/README
+-rw-r--r--   0 andrew     (503) staff       (20)     3306 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/iaf_sfa_relref/backend_comparison.py
+-rw-r--r--   0 andrew     (503) staff       (20)    20164 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/iaf_sfa_relref/iaf_sfa_network_INH_GAMMA.py
+-rw-r--r--   0 andrew     (503) staff       (20)    17837 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/iaf_sfa_relref/iaf_sfa_network_STATIC.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2347 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/iaf_sfa_relref/mcb.py
+-rw-r--r--   0 andrew     (503) staff       (20)    91116 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/iaf_sfa_relref/myFigure_expected.pdf
+-rw-r--r--   0 andrew     (503) staff       (20)      971 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/iaf_sfa_relref/standard_neurons.yaml
+-rw-r--r--   0 andrew     (503) staff       (20)      645 2019-02-07 15:54:52.000000 PyNN-0.9.6/examples/iclamp_test.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2509 2019-11-14 10:10:41.000000 PyNN-0.9.6/examples/inhomogeneous_network.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4175 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/multiquantal_synapses.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3640 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/nineml_brunel.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4477 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/nineml_neuron.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3882 2019-02-07 15:54:52.000000 PyNN-0.9.6/examples/nineml_stdp.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2658 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/nrn_artificial_cell.py
+-rw-r--r--   0 andrew     (503) staff       (20)      629 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/parameter_changes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2208 2019-11-14 10:10:41.000000 PyNN-0.9.6/examples/random_distributions.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4210 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/random_numbers.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2768 2020-12-09 17:54:24.000000 PyNN-0.9.6/examples/simpleRandomNetwork.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2250 2019-11-14 10:10:41.000000 PyNN-0.9.6/examples/simpleRandomNetwork_csa.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8279 2019-11-14 10:10:41.000000 PyNN-0.9.6/examples/simple_STDP.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3574 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/small_network.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2655 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/specific_network.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3715 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/stdp_network.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4721 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/stochastic_deterministic_comparison.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2890 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/stochastic_synapses.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3907 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/stochastic_tsodyksmarkram.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3918 2019-02-07 15:54:52.000000 PyNN-0.9.6/examples/stochastic_tsodyksmarkram_em.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5177 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/synaptic_input.py
+-rw-r--r--   0 andrew     (503) staff       (20)      964 2020-01-08 15:50:43.000000 PyNN-0.9.6/examples/tmp.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/examples/tools/
+-rw-r--r--   0 andrew     (503) staff       (20)     7451 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/tools/VAbenchmark_graphs.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2863 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/tools/comparison_plot.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2349 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/tools/plot_results.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2567 2020-12-21 16:53:12.000000 PyNN-0.9.6/examples/tools/run_all_examples.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3531 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/tsodyksmarkram.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3609 2020-12-09 17:54:24.000000 PyNN-0.9.6/examples/update_spike_source_array.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3030 2019-01-07 20:00:27.000000 PyNN-0.9.6/examples/varying_poisson.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/
+-rw-r--r--   0 andrew     (503) staff       (20)     2706 2020-12-22 14:18:15.000000 PyNN-0.9.6/pyNN/__init__.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/brian/
+-rw-r--r--   0 andrew     (503) staff       (20)     2723 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    10261 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3822 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)    11921 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4881 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3291 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/brian/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/brian/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    14262 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)    10792 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     7390 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/brian/standardmodels/synapses.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/brian2/
+-rw-r--r--   0 andrew     (503) staff       (20)     2668 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    13520 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4755 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)    13732 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4964 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3626 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/brian2/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    19182 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)    10111 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     7263 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/brian2/standardmodels/synapses.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/common/
+-rw-r--r--   0 andrew     (503) staff       (20)     1404 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/common/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6022 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/common/control.py
+-rw-r--r--   0 andrew     (503) staff       (20)    63459 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/common/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4161 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/common/procedural_api.py
+-rw-r--r--   0 andrew     (503) staff       (20)    22882 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/common/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)    48822 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/connectors.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2535 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/core.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/descriptions/
+-rw-r--r--   0 andrew     (503) staff       (20)     6214 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/descriptions/__init__.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/descriptions/templates/
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/
+-rw-r--r--   0 andrew     (503) staff       (20)      136 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/assembly_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)        5 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/modeltype_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      450 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/population_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      484 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/population_old.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       90 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/populationview_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      370 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/projection_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       76 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/cheetah/synapsedynamics_default.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/
+-rw-r--r--   0 andrew     (503) staff       (20)      149 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/assembly_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)        8 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/modeltype_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      486 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/population_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      541 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/population_old.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      102 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/populationview_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     1179 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/projection_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       82 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/jinja2/synapsedynamics_default.txt
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/
+-rw-r--r--   0 andrew     (503) staff       (20)       94 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/assembly_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)        5 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/modeltype_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      226 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/population_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       90 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/populationview_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      198 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/projection_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       76 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/descriptions/templates/string/synapsedynamics_default.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     2578 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/errors.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/hardware/
+-rw-r--r--   0 andrew     (503) staff       (20)      566 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/hardware/__init__.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/mock/
+-rw-r--r--   0 andrew     (503) staff       (20)     2409 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/mock/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3144 2019-04-07 14:59:32.000000 PyNN-0.9.6/pyNN/mock/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2193 2019-04-04 13:18:52.000000 PyNN-0.9.6/pyNN/mock/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1254 2019-09-02 15:18:12.000000 PyNN-0.9.6/pyNN/mock/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)      965 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/mock/simulator.py
+-rw-r--r--   0 andrew     (503) staff       (20)     9466 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/mock/standardmodels.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4008 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/models.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/moose/
+-rw-r--r--   0 andrew     (503) staff       (20)     8935 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/moose/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     7137 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/moose/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3224 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/moose/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1929 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/moose/simple_example.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3040 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/moose/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/moose/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/moose/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2771 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/moose/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3364 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/multisim.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nemo/
+-rw-r--r--   0 andrew     (503) staff       (20)    19198 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1045 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/connectors.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3209 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6447 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nemo/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nemo/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5879 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1508 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1825 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nemo/standardmodels/synapses.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nest/
+-rw-r--r--   0 andrew     (503) staff       (20)     6850 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3343 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8770 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/connectors.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2460 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nest/conversion.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3759 2019-09-02 15:18:12.000000 PyNN-0.9.6/pyNN/nest/electrodes.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nest/extensions/
+-rw-r--r--   0 andrew     (503) staff       (20)     9206 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/CMakeLists.txt
+-rw-r--r--   0 andrew     (503) staff       (20)     3790 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/pynn_extensions.cpp
+-rw-r--r--   0 andrew     (503) staff       (20)     1316 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/pynn_extensions.h
+-rw-r--r--   0 andrew     (503) staff       (20)     5581 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/simple_stochastic_connection.h
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nest/extensions/sli/
+-rw-r--r--   0 andrew     (503) staff       (20)      317 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/sli/pynn_extensions-init.sli
+-rw-r--r--   0 andrew     (503) staff       (20)     5970 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/stochastic_stp_connection.h
+-rw-r--r--   0 andrew     (503) staff       (20)     2109 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/extensions/stochastic_stp_connection_impl.h
+-rw-r--r--   0 andrew     (503) staff       (20)     5271 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/nineml.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8136 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)    22364 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3191 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nest/random.py
+-rw-r--r--   0 andrew     (503) staff       (20)    20264 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8877 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nest/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nest/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    12202 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     7712 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8400 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/standardmodels/synapses.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3234 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nest/synapses.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3885 2020-12-21 16:53:12.000000 PyNN-0.9.6/pyNN/network.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/neuroml/
+-rw-r--r--   0 andrew     (503) staff       (20)     3834 2020-12-09 17:54:24.000000 PyNN-0.9.6/pyNN/neuroml/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5538 2019-09-02 15:18:12.000000 PyNN-0.9.6/pyNN/neuroml/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6793 2020-12-09 17:54:24.000000 PyNN-0.9.6/pyNN/neuroml/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3775 2020-12-09 17:54:24.000000 PyNN-0.9.6/pyNN/neuroml/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2658 2019-09-02 15:18:12.000000 PyNN-0.9.6/pyNN/neuroml/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/neuroml/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuroml/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     9551 2019-09-02 15:18:12.000000 PyNN-0.9.6/pyNN/neuroml/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6398 2019-09-02 15:18:12.000000 PyNN-0.9.6/pyNN/neuroml/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3827 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuroml/standardmodels/synapses.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/neuron/
+-rw-r--r--   0 andrew     (503) staff       (20)     4938 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    24673 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1008 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/connectors.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3565 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/nineml.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/neuron/nmodl/
+-rw-r--r--   0 andrew     (503) staff       (20)     3582 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/adexp.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1530 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/alphaisyn.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1574 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/alphasyn.mod
+-rwxr-xr-x   0 andrew     (503) staff       (20)      377 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/expisyn.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     2406 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/gammastim.mod
+-rw-r--r--   0 andrew     (503) staff       (20)      322 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/gap.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     5180 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/gif.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1670 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/gsfa_grr.mod
+-rwxr-xr-x   0 andrew     (503) staff       (20)     2353 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/hh_traub.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1390 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/izhikevich.mod
+-rwxr-xr-x   0 andrew     (503) staff       (20)     5227 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/netstim2.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1300 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/poisson_stim_refractory.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     2838 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/quantal_stp.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1695 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/refrac.mod
+-rw-r--r--   0 andrew     (503) staff       (20)      609 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/reset.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     2018 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_guetig.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     2025 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_softlimits.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     2283 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_songabbott.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1969 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_symm.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     2375 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_vogels2011.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1574 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stochastic_synapse.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     3290 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/stochastic_tsodyksmarkram.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     4840 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/tmgsyn.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     4825 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/tmisyn.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     1248 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/tsodyksmarkram.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     5000 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/nmodl/vecstim.mod
+-rw-r--r--   0 andrew     (503) staff       (20)     5625 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)     7220 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3541 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/random.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5165 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)    23633 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/simulator.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/neuron/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/neuron/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8797 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     9445 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     6305 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/neuron/standardmodels/synapses.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/nineml/
+-rw-r--r--   0 andrew     (503) staff       (20)     3808 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nineml/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4490 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nineml/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1531 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nineml/connectors.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4776 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nineml/populations.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2239 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nineml/projections.py
+-rw-r--r--   0 andrew     (503) staff       (20)    15307 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nineml/read.py
+-rw-r--r--   0 andrew     (503) staff       (20)      664 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nineml/recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1023 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nineml/simulator.py
+-rw-r--r--   0 andrew     (503) staff       (20)    15363 2019-01-07 20:00:27.000000 PyNN-0.9.6/pyNN/nineml/standardmodels.py
+-rw-r--r--   0 andrew     (503) staff       (20)      267 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nineml/synapses.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4394 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/nineml/utility.py
+-rw-r--r--   0 andrew     (503) staff       (20)    19093 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/parameters.py
+-rw-r--r--   0 andrew     (503) staff       (20)    18697 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/random.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/recording/
+-rw-r--r--   0 andrew     (503) staff       (20)    16185 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/recording/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8841 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/recording/files.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/serialization/
+-rw-r--r--   0 andrew     (503) staff       (20)      165 2020-12-09 17:54:24.000000 PyNN-0.9.6/pyNN/serialization/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    51916 2020-12-22 13:35:41.000000 PyNN-0.9.6/pyNN/serialization/sonata.py
+-rw-r--r--   0 andrew     (503) staff       (20)    14325 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/space.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/standardmodels/
+-rw-r--r--   0 andrew     (503) staff       (20)    13475 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/standardmodels/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    23477 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/standardmodels/cells.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3347 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/standardmodels/electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)    15108 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/standardmodels/synapses.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/pyNN/utility/
+-rw-r--r--   0 andrew     (503) staff       (20)    14641 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/utility/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)    13115 2020-12-22 13:49:02.000000 PyNN-0.9.6/pyNN/utility/plotting.py
+-rw-r--r--   0 andrew     (503) staff       (20)      167 2020-12-21 16:53:12.000000 PyNN-0.9.6/requirements.txt
+-rw-r--r--   0 andrew     (503) staff       (20)       38 2020-12-22 14:19:24.000000 PyNN-0.9.6/setup.cfg
+-rw-r--r--   0 andrew     (503) staff       (20)     5837 2020-12-22 14:19:22.000000 PyNN-0.9.6/setup.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/test/
+-rw-r--r--   0 andrew     (503) staff       (20)      342 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/README
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/test/benchmarks/
+-rw-r--r--   0 andrew     (503) staff       (20)     9141 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/benchmarks/Benchmark_PyNN-0.8dev_FixedNumberPost.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1452 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/README.txt
+-rw-r--r--   0 andrew     (503) staff       (20)      931 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/all_to_all_network.param
+-rw-r--r--   0 andrew     (503) staff       (20)     6697 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/connectors_benchmark.py
+-rw-r--r--   0 andrew     (503) staff       (20)      804 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/ddpc.py
+-rw-r--r--   0 andrew     (503) staff       (20)       94 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/neurons_no_recording.param
+-rw-r--r--   0 andrew     (503) staff       (20)      506 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/neurons_with_recording.param
+-rw-r--r--   0 andrew     (503) staff       (20)     3585 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/benchmarks/plot_figure.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4426 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/benchmarks/simple_network.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/test/system/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/__init__.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/test/system/scenarios/
+-rw-r--r--   0 andrew     (503) staff       (20)      740 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)      718 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/issue231.py
+-rw-r--r--   0 andrew     (503) staff       (20)      712 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/issue274.py
+-rw-r--r--   0 andrew     (503) staff       (20)      350 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/registry.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4653 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/scenario1.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2234 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/scenario2.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3176 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/scenario3.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3230 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/scenario4.py
+-rw-r--r--   0 andrew     (503) staff       (20)    11749 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/test_cell_types.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5257 2020-12-22 12:05:03.000000 PyNN-0.9.6/test/system/scenarios/test_connection_handling.py
+-rw-r--r--   0 andrew     (503) staff       (20)    11440 2020-12-22 12:05:03.000000 PyNN-0.9.6/test/system/scenarios/test_connectors.py
+-rw-r--r--   0 andrew     (503) staff       (20)    25901 2020-12-16 19:00:16.000000 PyNN-0.9.6/test/system/scenarios/test_electrodes.py
+-rw-r--r--   0 andrew     (503) staff       (20)     9687 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/test_parameter_handling.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1027 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/test_procedural_api.py
+-rw-r--r--   0 andrew     (503) staff       (20)    16042 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/test_recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2999 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/test_simulation_control.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2351 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/scenarios/test_synapse_types.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1860 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/scenarios/ticket166.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3844 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/test_brian.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3106 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/test_brian2.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5037 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/test_hardware_brainscales.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1574 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/test_moose.py
+-rw-r--r--   0 andrew     (503) staff       (20)    11320 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/test_nest.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1052 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/system/test_neuroml.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8916 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/test_neuron.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1996 2020-12-21 16:53:12.000000 PyNN-0.9.6/test/system/test_serialization.py
+drwxr-xr-x   0 andrew     (503) staff       (20)        0 2020-12-22 14:19:24.000000 PyNN-0.9.6/test/unittests/
+-rw-r--r--   0 andrew     (503) staff       (20)        0 2019-01-07 20:00:27.000000 PyNN-0.9.6/test/unittests/__init__.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2006 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/mocks.py
+-rw-r--r--   0 andrew     (503) staff       (20)    22625 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_assembly.py
+-rw-r--r--   0 andrew     (503) staff       (20)     1456 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_brian.py
+-rw-r--r--   0 andrew     (503) staff       (20)    47522 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_connectors_parallel.py
+-rw-r--r--   0 andrew     (503) staff       (20)    48786 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_connectors_serial.py
+-rw-r--r--   0 andrew     (503) staff       (20)      597 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_core.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2957 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_descriptions.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3426 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_files.py
+-rw-r--r--   0 andrew     (503) staff       (20)     4254 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_idmixin.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2865 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_lowlevelapi.py
+-rw-r--r--   0 andrew     (503) staff       (20)     8078 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_nest.py
+-rw-r--r--   0 andrew     (503) staff       (20)    15463 2020-12-22 12:05:03.000000 PyNN-0.9.6/test/unittests/test_neuron.py
+-rw-r--r--   0 andrew     (503) staff       (20)    15008 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_parameters.py
+-rw-r--r--   0 andrew     (503) staff       (20)    25452 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_population.py
+-rw-r--r--   0 andrew     (503) staff       (20)    23806 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_populationview.py
+-rw-r--r--   0 andrew     (503) staff       (20)    16520 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_projection.py
+-rw-r--r--   0 andrew     (503) staff       (20)    10171 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_random.py
+-rw-r--r--   0 andrew     (503) staff       (20)     5455 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_recording.py
+-rw-r--r--   0 andrew     (503) staff       (20)     3995 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_simulation_control.py
+-rw-r--r--   0 andrew     (503) staff       (20)    11282 2020-12-22 13:49:02.000000 PyNN-0.9.6/test/unittests/test_space.py
+-rw-r--r--   0 andrew     (503) staff       (20)     7357 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_standardmodels.py
+-rw-r--r--   0 andrew     (503) staff       (20)     2390 2020-12-09 17:54:24.000000 PyNN-0.9.6/test/unittests/test_utility_functions.py
```

### Comparing `PyNN-0.9.5/.gitignore` & `PyNN-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/AUTHORS` & `PyNN-0.9.6/AUTHORS`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The following people have contributed to PyNN. Their affiliations at the time of the contributions are shown below.
 
-* Andrew Davison [1]
+* Andrew Davison [1, 20]
 * Pierre Yger [1, 9]
 * Eilif Muller [7, 13]
 * Jens Kremkow [5,6]
 * Daniel Brüderle [2]
 * Laurent Perrinet [6]
 * Jochen Eppler [3,4]
 * Dejan Pecevski [8]
@@ -18,19 +18,22 @@
 * Jan Antolik [1]
 * Alexandre Gravier
 * Thomas Close [17]
 * Oliver Breitwieser [2]
 * Jannis Schücker [16]
 * Maximilian Schmidt [16]
 * Christian Roessert [13]
-* Shailesh Appukuttan [1]
+* Shailesh Appukuttan [1, 20]
 * Elodie Legouée [1]
 * Joffrey Gonin [1]
 * Ankur Sinha [18]
 * Håkon Mørk [19]
+* Andrei Moise [20]
+* Onur Ates [20]
+* Rémy Cagnol [21]
 
 
 1.  Unité de Neuroscience, Information et Complexité, CNRS, Gif sur Yvette, France
 2.  Kirchhoff Institute for Physics, University of Heidelberg, Heidelberg, Germany
 3.  Honda Research Institute Europe GmbH, Offenbach, Germany
 4.  Bernstein Center for Computational Neuroscience, Albert-Ludwigs-University, Freiburg, Germany
 5.  Neurobiology and Biophysics, Institute of Biology III, Albert-Ludwigs-University, Freiburg, Germany
@@ -44,7 +47,9 @@
 13. Blue Brain Project, Ecole Polytechnique Fédérale de Lausanne, Lausanne, Switzerland
 14. NCBS, Bangalore, India
 15. PDC, KTH, Stockholm, Sweden
 16. Institute of Neuroscience and Medicine (INM-6), Jülich Research Center, Jülich, Germany
 17. Okinawa Institute of Science and Technology (OIST), Onna-son, Okinawa, Japan
 18. Biocomputation group, University of Hertfordshire, Hatfield, United Kingdom.
 19. Norwegian University of Life Sciences, Ås, Norway
+20. Paris-Saclay Institute of Neuroscience, CNRS/Université Paris-Saclay, Gif sur Yvette, France
+21. Faculty of Mathematics and Physics, Charles University, Prague, Czechia
```

### Comparing `PyNN-0.9.5/CODE_OF_CONDUCT.md` & `PyNN-0.9.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/LICENSE` & `PyNN-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/PKG-INFO` & `PyNN-0.9.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNN
-Version: 0.9.5
+Version: 0.9.6
 Summary: A Python package for simulator-independent specification of neuronal network models
 Home-page: http://neuralensemble.org/PyNN/
 Author: The PyNN team
 Author-email: andrew.davison@unic.cnrs-gif.fr
 License: CeCILL http://www.cecill.info
 Description: PyNN
         ====
@@ -34,15 +34,15 @@
         
         - Home page: http://neuralensemble.org/PyNN/
         - Documentation: http://neuralensemble.org/docs/PyNN/
         - Mailing list: https://groups.google.com/forum/?fromgroups#!forum/neuralensemble
         - Bug reports: https://github.com/NeuralEnsemble/PyNN/issues
         
         
-        :copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+        :copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
         :license: CeCILL, see LICENSE for details.
         
         .. image:: https://travis-ci.org/NeuralEnsemble/PyNN.png?branch=master
            :target: https://travis-ci.org/NeuralEnsemble/PyNN
            :alt: Unit Test Status
         
         .. image:: https://coveralls.io/repos/NeuralEnsemble/PyNN/badge.svg?branch=master&service=github
@@ -56,17 +56,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: plotting
 Provides-Extra: examples
-Provides-Extra: sonata
+Provides-Extra: plotting
 Provides-Extra: MPI
+Provides-Extra: sonata
```

### Comparing `PyNN-0.9.5/PyNN.egg-info/PKG-INFO` & `PyNN-0.9.6/PyNN.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNN
-Version: 0.9.5
+Version: 0.9.6
 Summary: A Python package for simulator-independent specification of neuronal network models
 Home-page: http://neuralensemble.org/PyNN/
 Author: The PyNN team
 Author-email: andrew.davison@unic.cnrs-gif.fr
 License: CeCILL http://www.cecill.info
 Description: PyNN
         ====
@@ -34,15 +34,15 @@
         
         - Home page: http://neuralensemble.org/PyNN/
         - Documentation: http://neuralensemble.org/docs/PyNN/
         - Mailing list: https://groups.google.com/forum/?fromgroups#!forum/neuralensemble
         - Bug reports: https://github.com/NeuralEnsemble/PyNN/issues
         
         
-        :copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+        :copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
         :license: CeCILL, see LICENSE for details.
         
         .. image:: https://travis-ci.org/NeuralEnsemble/PyNN.png?branch=master
            :target: https://travis-ci.org/NeuralEnsemble/PyNN
            :alt: Unit Test Status
         
         .. image:: https://coveralls.io/repos/NeuralEnsemble/PyNN/badge.svg?branch=master&service=github
@@ -56,17 +56,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: plotting
 Provides-Extra: examples
-Provides-Extra: sonata
+Provides-Extra: plotting
 Provides-Extra: MPI
+Provides-Extra: sonata
```

### Comparing `PyNN-0.9.5/PyNN.egg-info/SOURCES.txt` & `PyNN-0.9.6/PyNN.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 doc/releases/0.8.3.txt
 doc/releases/0.9.0.txt
 doc/releases/0.9.1.txt
 doc/releases/0.9.2.txt
 doc/releases/0.9.3.txt
 doc/releases/0.9.4.txt
 doc/releases/0.9.5.txt
+doc/releases/0.9.6.txt
 examples/FakeStepCurrentSource.py
 examples/HH_cond_exp2.py
 examples/Izhikevich.py
 examples/README
 examples/StepCurrentSource.py
 examples/VAbenchmarks.py
 examples/ball_and_stick.py
@@ -175,14 +176,15 @@
 examples/specific_network.py
 examples/stdp_network.py
 examples/stochastic_deterministic_comparison.py
 examples/stochastic_synapses.py
 examples/stochastic_tsodyksmarkram.py
 examples/stochastic_tsodyksmarkram_em.py
 examples/synaptic_input.py
+examples/tmp.py
 examples/tsodyksmarkram.py
 examples/update_spike_source_array.py
 examples/varying_poisson.py
 examples/Potjans2014/README.txt
 examples/Potjans2014/connectivity.py
 examples/Potjans2014/microcircuit.py
 examples/Potjans2014/network.py
@@ -219,14 +221,24 @@
 pyNN/brian/projections.py
 pyNN/brian/recording.py
 pyNN/brian/simulator.py
 pyNN/brian/standardmodels/__init__.py
 pyNN/brian/standardmodels/cells.py
 pyNN/brian/standardmodels/electrodes.py
 pyNN/brian/standardmodels/synapses.py
+pyNN/brian2/__init__.py
+pyNN/brian2/cells.py
+pyNN/brian2/populations.py
+pyNN/brian2/projections.py
+pyNN/brian2/recording.py
+pyNN/brian2/simulator.py
+pyNN/brian2/standardmodels/__init__.py
+pyNN/brian2/standardmodels/cells.py
+pyNN/brian2/standardmodels/electrodes.py
+pyNN/brian2/standardmodels/synapses.py
 pyNN/common/__init__.py
 pyNN/common/control.py
 pyNN/common/populations.py
 pyNN/common/procedural_api.py
 pyNN/common/projections.py
 pyNN/descriptions/__init__.py
 pyNN/descriptions/templates/cheetah/assembly_default.txt
@@ -246,15 +258,14 @@
 pyNN/descriptions/templates/string/assembly_default.txt
 pyNN/descriptions/templates/string/modeltype_default.txt
 pyNN/descriptions/templates/string/population_default.txt
 pyNN/descriptions/templates/string/populationview_default.txt
 pyNN/descriptions/templates/string/projection_default.txt
 pyNN/descriptions/templates/string/synapsedynamics_default.txt
 pyNN/hardware/__init__.py
-pyNN/hardware/aux.py
 pyNN/mock/__init__.py
 pyNN/mock/populations.py
 pyNN/mock/projections.py
 pyNN/mock/recording.py
 pyNN/mock/simulator.py
 pyNN/mock/standardmodels.py
 pyNN/moose/__init__.py
@@ -370,25 +381,17 @@
 test/benchmarks/all_to_all_network.param
 test/benchmarks/connectors_benchmark.py
 test/benchmarks/ddpc.py
 test/benchmarks/neurons_no_recording.param
 test/benchmarks/neurons_with_recording.param
 test/benchmarks/plot_figure.py
 test/benchmarks/simple_network.py
-test/hardware/unittests/__init__.py
-test/hardware/unittests/launch_test.py
-test/hardware/unittests/mocks.py
-test/hardware/unittests/test_assembly.py
-test/hardware/unittests/test_connectors.py
-test/hardware/unittests/test_population.py
-test/hardware/unittests/test_populationview.py
-test/hardware/unittests/test_projection.py
-test/hardware/unittests/test_simulation_control.py
 test/system/__init__.py
 test/system/test_brian.py
+test/system/test_brian2.py
 test/system/test_hardware_brainscales.py
 test/system/test_moose.py
 test/system/test_nest.py
 test/system/test_neuroml.py
 test/system/test_neuron.py
 test/system/test_serialization.py
 test/system/scenarios/__init__.py
@@ -407,15 +410,14 @@
 test/system/scenarios/test_procedural_api.py
 test/system/scenarios/test_recording.py
 test/system/scenarios/test_simulation_control.py
 test/system/scenarios/test_synapse_types.py
 test/system/scenarios/ticket166.py
 test/unittests/__init__.py
 test/unittests/mocks.py
-test/unittests/setup.cfg
 test/unittests/test_assembly.py
 test/unittests/test_brian.py
 test/unittests/test_connectors_parallel.py
 test/unittests/test_connectors_serial.py
 test/unittests/test_core.py
 test/unittests/test_descriptions.py
 test/unittests/test_files.py
```

### Comparing `PyNN-0.9.5/README.rst` & `PyNN-0.9.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 - Home page: http://neuralensemble.org/PyNN/
 - Documentation: http://neuralensemble.org/docs/PyNN/
 - Mailing list: https://groups.google.com/forum/?fromgroups#!forum/neuralensemble
 - Bug reports: https://github.com/NeuralEnsemble/PyNN/issues
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 .. image:: https://travis-ci.org/NeuralEnsemble/PyNN.png?branch=master
    :target: https://travis-ci.org/NeuralEnsemble/PyNN
    :alt: Unit Test Status
 
 .. image:: https://coveralls.io/repos/NeuralEnsemble/PyNN/badge.svg?branch=master&service=github
```

### Comparing `PyNN-0.9.5/changelog` & `PyNN-0.9.6/changelog`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/ci/install_nest.sh` & `PyNN-0.9.6/ci/install_nest.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/bin/bash
 
 set -e  # stop execution in case of errors
 
-if [ "$TRAVIS_PYTHON_VERSION" == "2.7" ] || [ "$TRAVIS_PYTHON_VERSION" == "3.6" ]; then
+if [ "$TRAVIS_PYTHON_VERSION" == "2.7" ] || [ "$TRAVIS_PYTHON_VERSION" == "3.7" ]; then
     echo -e "\n========== Installing NEST ==========\n"
     # Specify which version of NEST to install
     #export NEST_VERSION="master"
-    export NEST_VERSION="2.18.0"
+    export NEST_VERSION="2.20.0"
 
     pip install cython  #==0.28.1
 
     if [ "$NEST_VERSION" = "master" ]; then
       export NEST="nest-simulator-$NEST_VERSION"
       wget https://github.com/nest/nest-simulator/archive/$NEST_VERSION.tar.gz -O $HOME/$NEST.tar.gz;
     else
@@ -26,16 +26,16 @@
     mkdir -p $HOME/build/$NEST
     pushd $HOME/build/$NEST
     export VENV=`python -c "import sys; print(sys.prefix)"`;
     if [ "$TRAVIS_PYTHON_VERSION" == "2.7" ]; then
       ln -s /opt/python/2.7/lib/libpython2.7.so $VENV/lib/libpython2.7.so;
       export PYTHON_INCLUDE_DIR=$VENV/include/python${TRAVIS_PYTHON_VERSION}
     fi
-    if [ "$TRAVIS_PYTHON_VERSION" == "3.6" ]; then
-      ln -s /opt/python/3.6/lib/libpython3.6m.so $VENV/lib/libpython3.6.so;
+    if [ "$TRAVIS_PYTHON_VERSION" == "3.7" ]; then
+      ln -s /opt/python/3.7/lib/libpython3.7m.so $VENV/lib/libpython3.7.so;
       export PYTHON_INCLUDE_DIR=$VENV/include/python${TRAVIS_PYTHON_VERSION}m
     fi
     cython --version;
     cmake --version;
     cmake -DCMAKE_INSTALL_PREFIX=$VENV \
           -Dwith-mpi=ON  \
           -DPYTHON_EXECUTABLE=$VENV/bin/python \
```

### Comparing `PyNN-0.9.5/ci/install_neuron.sh` & `PyNN-0.9.6/ci/install_neuron.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/bin/bash
 
 set -e  # stop execution in case of errors
 
-if [ "$TRAVIS_PYTHON_VERSION" == "2.7" ]; then
+if [ "$TRAVIS_PYTHON_VERSION" == "3.7" ]; then
     echo -e "\n========== Installing NEURON ==========\n"
-    export NRN_VERSION="nrn-7.5"
+    export NRN_VERSION="nrn-7.7"
     if [ ! -f "$HOME/$NRN_VERSION/configure" ]; then
-        wget http://www.neuron.yale.edu/ftp/neuron/versions/v7.5/$NRN_VERSION.tar.gz -O $HOME/$NRN_VERSION.tar.gz;
+        wget http://www.neuron.yale.edu/ftp/neuron/versions/v7.7/$NRN_VERSION.tar.gz -O $HOME/$NRN_VERSION.tar.gz;
         pushd $HOME;
         tar xzf $NRN_VERSION.tar.gz;
         popd;
     else
         echo 'Using cached version of NEURON sources.';
     fi
     mkdir -p $HOME/build/$NRN_VERSION
```

### Comparing `PyNN-0.9.5/doc/Makefile` & `PyNN-0.9.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/architecture_of_PyNN.svg` & `PyNN-0.9.6/doc/architecture_of_PyNN.svg`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/backends/NEST.txt` & `PyNN-0.9.6/doc/backends/NEST.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/backends/NEURON.txt` & `PyNN-0.9.6/doc/backends/NEURON.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/backends.txt` & `PyNN-0.9.6/doc/backends.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/build_examples.py` & `PyNN-0.9.6/doc/build_examples.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/conf.py` & `PyNN-0.9.6/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,24 @@
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'PyNN'
 authors = u'the PyNN community'
-copyright = u'2006-2019, ' + authors
+copyright = u'2006-2020, ' + authors
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '0.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.9.5'
+release = '0.9.6'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `PyNN-0.9.5/doc/connections.txt` & `PyNN-0.9.6/doc/connections.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,22 @@
 ---------------------
 
 The simplest, and default synapse type in PyNN has constant synaptic weight:
 
 .. testcode::
 
     syn = StaticSynapse(weight=0.04, delay=0.5)
-    
+
 .. note:: weights are in microsiemens or nanoamps, depending on whether the
           post-synaptic mechanism implements a change in conductance or current,
-          and delays are in milliseconds (see :doc:`units`).
+          and delays are in milliseconds (see :doc:`units`). Weights should always
+          be positive, *except* for the case of inhibitory (see `receptor_type`
+          argument below), current-based synapses, for which they should be negative.
+          Inhibitory, conductance-based synapses have positive weights, because
+          it is the reversal potential which makes it inhibitory.
 
 It is also possible to add variability to synaptic weights and delays by
 specifying a :class:`RandomDistribution` object as the parameter value:
 
 .. testcode::
 
     w = RandomDistribution('gamma', [10, 0.004], rng=NumpyRNG(seed=4242))
@@ -106,15 +110,15 @@
 
     stdp = STDPMechanism(
               weight=0.02,  # this is the initial value of the weight
               delay="0.2 + 0.01*d",
               timing_dependence=SpikePairRule(tau_plus=20.0, tau_minus=20.0,
                                               A_plus=0.01, A_minus=0.012),
               weight_dependence=AdditiveWeightDependence(w_min=0, w_max=0.04))
-    
+
 Note that not all simulators will support all possible combinations of synaptic
 plasticity components.
 
 
 Connection algorithms
 =====================
 
@@ -308,16 +312,16 @@
 
 
 Reading connection patterns to/from a file
 ------------------------------------------
 
 Connection patterns can be read in from a text file. The file should contain
 a header specifying which parameter is in which column, e.g.::
- 
-    # columns = ["i", "j", "weight", "delay", "U", "tau_rec"]   
+
+    # columns = ["i", "j", "weight", "delay", "U", "tau_rec"]
 
 and then the connection data should be in columns separated by spaces. The
 connections are read using:
 
 .. testcode::
 
     connector = FromFileConnector("connections.txt")
@@ -369,15 +373,16 @@
     * the post-synaptic population;
     * a connection/wiring method;
     * a synapse type
 
 Optionally, we can also specify:
 
     * the name of the post-synaptic mechanism (e.g. ‘excitatory’, ‘NMDA’)
-      (by default, this is 'excitatory');
+      (if not specified, PyNN picks a default depending on the weight
+       parameter of the synapse type);
     * a label (autogenerated if not specified);
     * a :class:`Space` object, which determines how distances should be
       calculated for distance-dependent wiring schemes or parameter values.
 
 Here is a minimal example:
 
 .. testcode::
```

### Comparing `PyNN-0.9.5/doc/contributors.txt` & `PyNN-0.9.6/doc/contributors.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/data_handling.txt` & `PyNN-0.9.6/doc/data_handling.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/descriptions.txt` & `PyNN-0.9.6/doc/descriptions.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/developers/adding_backend.txt` & `PyNN-0.9.6/doc/developers/adding_backend.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/developers/contributing.txt` & `PyNN-0.9.6/doc/developers/contributing.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     - indentation of four spaces, no tabs
     - single space around most operators, but no space around the '=' sign when
       used to indicate a keyword argument or a default parameter value.
     - some function/method names in PyNN use ``mixedCase``, but these will
       gradually be deprecated and replaced with ``lower_case_with_underscores``.
       Any new functions or methods should use the latter.
-    - we currently target versions 2.7 and 3.3-3.6
+    - we currently target versions 2.7 and 3.6+
 
 
 Testing
 =======
 
 Running the PyNN test suite requires the *nose_*, *mock_* and *nose-testconfig* packages,
 and optionally the *coverage_* package. To run the entire test suite, in the
@@ -110,27 +110,27 @@
 run without a simulator installed.
 
 System tests should be written so that they can run with any of the simulators.
 The suggested way to do this is to write test functions, in a separate file,
 that take a simulator module as an argument, and then call these functions from
 ``test_neuron.py``, ``test_nest.py``, etc.
 
-System tests defined in the scenarios directory are treated as a single test 
+System tests defined in the scenarios directory are treated as a single test
 (test_scenarios()) while running nosetests. To run only the tests within a file
 named 'test_electrodes' located inside system/scenarios, use::
 
     $ nosetests -s --tc=testFile:test_electrodes test_nest.py
 
-To run a single specific test named 'test_changing_electrode' located within 
+To run a single specific test named 'test_changing_electrode' located within
 some file (and added to registry) inside system/scenarios, use::
 
     $ nosetests -s --tc=testName:test_changing_electrode test_nest.py
 
 Note that this would also run the tests specified within the simulator specific
-files such as test_brian.py, test_nest.py and test_neuron.py. To avoid 
+files such as test_brian.py, test_nest.py and test_neuron.py. To avoid
 this, specify the 'test_scenarios function' on the command line::
 
     $ nosetests -s --tc=testName:test_changing_electrode test_nest.py:test_scenarios
 
 The ``test/unsorted`` directory contains a number of old tests that are either
 no longer useful or have not yet been adapted to the nose framework. These are
 not part of the test suite, but we are gradually adapting those tests that are
@@ -216,15 +216,15 @@
 
     $ git tag x.y.z
 
 where ``x.y.z`` is the release number. You should now upload the documentation
 to http://neuralensemble.org/docs/PyNN/ by running::
 
     $ make zip
-    
+
 in the :file:`doc` directory, and then unpacking the resulting archive on the
 NeuralEnsemble server.
 
 If this is a development release (i.e. an *alpha* or *beta*), the final step is
 to upload the source package to the INCF Software Center.
 Do **not** upload development releases to PyPI.
```

### Comparing `PyNN-0.9.5/doc/developers/governance.txt` & `PyNN-0.9.6/doc/developers/governance.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/developers_guide.txt` & `PyNN-0.9.6/doc/developers_guide.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/download.txt` & `PyNN-0.9.6/doc/download.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 =========
 Downloads
 =========
 
 Source distributions
 --------------------
 
-The `latest stable version of PyNN`_ (0.9.5) may be downloaded from the
+The `latest stable version of PyNN`_ (0.9.6) may be downloaded from the
 `Python Package Index`_. This is recommended for
 anyone using PyNN for the first time.
 
 If you need support for a previous version of the API, the packages can be downloaded from
 the links below. This is recommended for anyone who needs a simulator/hardware backend that
 does not yet support the 0.8 API.
```

### Comparing `PyNN-0.9.5/doc/images/ac_source.png` & `PyNN-0.9.6/doc/images/ac_source.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/continuous_time_spiking.png` & `PyNN-0.9.6/doc/images/continuous_time_spiking.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/dc_source.png` & `PyNN-0.9.6/doc/images/dc_source.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/Izhikevich_nest_np1_20170505-150315.png` & `PyNN-0.9.6/doc/images/examples/Izhikevich_nest_np1_20170505-150315.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/VAbenchmarks_CUBA_20170505-150538.png` & `PyNN-0.9.6/doc/images/examples/VAbenchmarks_CUBA_20170505-150538.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/cell_type_demonstration_nest_20170505-150320.png` & `PyNN-0.9.6/doc/images/examples/cell_type_demonstration_nest_20170505-150320.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/current_injection_neuron_20170505-150317.png` & `PyNN-0.9.6/doc/images/examples/current_injection_neuron_20170505-150317.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/random_distributions.png` & `PyNN-0.9.6/doc/images/examples/random_distributions.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/random_numbers_neuron_20170505-150323.png` & `PyNN-0.9.6/doc/images/examples/random_numbers_neuron_20170505-150323.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/simple_stdp_neuron_20170505-150331.png` & `PyNN-0.9.6/doc/images/examples/simple_stdp_neuron_20170505-150331.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/small_network_nest_np1_20170505-150334.png` & `PyNN-0.9.6/doc/images/examples/small_network_nest_np1_20170505-150334.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/stochastic_comparison_neuron_20170505-150418.png` & `PyNN-0.9.6/doc/images/examples/stochastic_comparison_neuron_20170505-150418.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/stochastic_synapses__nest_20170505-150345.png` & `PyNN-0.9.6/doc/images/examples/stochastic_synapses__nest_20170505-150345.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/synaptic_input_neuron_20170505-150337.png` & `PyNN-0.9.6/doc/images/examples/synaptic_input_neuron_20170505-150337.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/tsodyksmarkram_nest_20170505-150340.png` & `PyNN-0.9.6/doc/images/examples/tsodyksmarkram_nest_20170505-150340.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/examples/varying_poisson_neuron_20170505-150343.png` & `PyNN-0.9.6/doc/images/examples/varying_poisson_neuron_20170505-150343.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/neo_example.png` & `PyNN-0.9.6/doc/images/neo_example.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/noise_source.png` & `PyNN-0.9.6/doc/images/noise_source.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/ongridoffgrid.png` & `PyNN-0.9.6/doc/images/ongridoffgrid.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/release_0.8b1_example.png` & `PyNN-0.9.6/doc/images/release_0.8b1_example.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/reset_example.png` & `PyNN-0.9.6/doc/images/reset_example.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/step_source.png` & `PyNN-0.9.6/doc/images/step_source.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/images/tmp.png` & `PyNN-0.9.6/doc/images/tmp.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/import_export.txt` & `PyNN-0.9.6/doc/import_export.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/index.txt` & `PyNN-0.9.6/doc/index.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/injecting_current.txt` & `PyNN-0.9.6/doc/injecting_current.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/installation.txt` & `PyNN-0.9.6/doc/installation.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 ============
 
 The following instructions are for Linux and Mac OS X. It should be possible to
 install and run PyNN on Windows, but this has not been tested.
 
 Installing PyNN requires:
 
-    * Python (version 2.7, 3.3-3.7)
+    * Python (version 2.7, 3.6+)
     * a recent version of the NumPy_ package
     * the lazyarray_ package
-    * the Neo_ package (>= 0.5.0)
+    * the Neo_ package (>= 0.8.0)
     * at least one of the supported simulators: e.g. NEURON, NEST, or Brian.
 
 Optional dependencies are:
 
     * mpi4py_ (if you wish to run distributed simulations using MPI)
     * either Jinja2_ or Cheetah_ (templating engines)
     * the CSA_ library
+    * h5py (to use the SONATA format)
 
 Installing PyNN
 ===============
 
 .. note:: if using NEURON or NEST, it is easiest if you install NEURON/NEST *before* you install PyNN (see below).
 
 The easiest way to get PyNN is to use pip_::
 
     $ pip install pyNN
 
 If you would prefer to install manually, :doc:`download the latest
 source distribution <download>`, then run the setup script, e.g.::
 
-    $ tar xzf PyNN-0.9.5.tar.gz
-    $ cd PyNN-0.9.5
+    $ tar xzf PyNN-0.9.6.tar.gz
+    $ cd PyNN-0.9.6
     $ python setup.py install
 
 This will install it to your Python :file:`site-packages` directory, and may
 require root privileges. We strongly recommend, however, that you use a
 virtualenv_ or a Conda_ environment. We assume you have already installed the
 simulator(s) you wish to use it with. If this is not the case, see below for
 installation instructions.
@@ -73,15 +74,15 @@
 
 If you installed PyNN before installing NEURON, or if you update your PyNN installation,
 you will need to manually run :command:`nrnivmodl` in the :file:`pyNN/neuron/nmodl` directory.
 
 Installing NEURON
 =================
 
-Download the sources for NEURON 7.4 or 7.5, in ``.tar.gz`` format, from `<http://www.neuron.yale.edu/neuron/download/getstd>`_.
+Download the sources for NEURON 7.4 or later, in ``.tar.gz`` format, from `<http://www.neuron.yale.edu/neuron/download/getstd>`_.
 Also download Interviews from the same location.
 
 Compile Interviews and NEURON according to the instructions given at `<http://www.neuron.yale.edu/neuron/static/download/compilestd_unix.html>`_,
 except that when you run :command:`configure`, add the options :option:`--with-nrnpython` and, optionally, :option:`--with-paranrn`, i.e.::
 
     $ ./configure --prefix=`pwd` --with-nrnpython --with-paranrn
     $ make
@@ -126,15 +127,15 @@
 
     $ cd ~
     $ python
     >>> import nest
                  -- N E S T --
       Copyright (C) 2004 The NEST Initiative
 
-    Version: v2.18.0
+    Version: v2.20.0
 
     ...
     >>> nest.Models()
     (u'ac_generator', u'aeif_cond_alpha', u'aeif_cond_alpha_RK5', u'aeif_cond_alpha_multisynapse',
     ...
 
 Check that ``'aeif_cond_alpha'`` is in the list of models. If it is not, you may need to install a newer version of the `GNU Scientific Library`_ and then recompile NEST.
```

### Comparing `PyNN-0.9.5/doc/introduction.txt` & `PyNN-0.9.6/doc/introduction.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/logging.txt` & `PyNN-0.9.6/doc/logging.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/make.bat` & `PyNN-0.9.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/neurons.txt` & `PyNN-0.9.6/doc/neurons.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/nineml.txt` & `PyNN-0.9.6/doc/nineml.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/parallel.txt` & `PyNN-0.9.6/doc/parallel.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/parameters.txt` & `PyNN-0.9.6/doc/parameters.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/publications.txt` & `PyNN-0.9.6/doc/publications.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyNN_logo.png` & `PyNN-0.9.6/doc/pyNN_logo.png`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/ac_source.py` & `PyNN-0.9.6/doc/pyplots/ac_source.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/continuous_time_spiking.py` & `PyNN-0.9.6/doc/pyplots/continuous_time_spiking.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/dc_source.py` & `PyNN-0.9.6/doc/pyplots/dc_source.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/neo_example.py` & `PyNN-0.9.6/doc/pyplots/neo_example.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/noise_source.py` & `PyNN-0.9.6/doc/pyplots/noise_source.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/plot_current_source.py` & `PyNN-0.9.6/doc/pyplots/plot_current_source.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/plot_helper.py` & `PyNN-0.9.6/doc/pyplots/plot_helper.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/reset_example.py` & `PyNN-0.9.6/doc/pyplots/reset_example.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/pyplots/step_source.py` & `PyNN-0.9.6/doc/pyplots/step_source.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/random_numbers.txt` & `PyNN-0.9.6/doc/random_numbers.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/recording.txt` & `PyNN-0.9.6/doc/recording.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/connectors.txt` & `PyNN-0.9.6/doc/reference/connectors.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/electrodes.txt` & `PyNN-0.9.6/doc/reference/electrodes.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/neuronmodels.txt` & `PyNN-0.9.6/doc/reference/neuronmodels.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/parameters.txt` & `PyNN-0.9.6/doc/reference/parameters.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/plasticitymodels.txt` & `PyNN-0.9.6/doc/reference/plasticitymodels.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/populations.txt` & `PyNN-0.9.6/doc/reference/populations.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/projections.txt` & `PyNN-0.9.6/doc/reference/projections.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/random.txt` & `PyNN-0.9.6/doc/reference/random.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/simulationcontrol.txt` & `PyNN-0.9.6/doc/reference/simulationcontrol.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/space.txt` & `PyNN-0.9.6/doc/reference/space.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/reference/utility.txt` & `PyNN-0.9.6/doc/reference/utility.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.6.txt` & `PyNN-0.9.6/doc/releases/0.6.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.7.txt` & `PyNN-0.9.6/doc/releases/0.7.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8-alpha-1.txt` & `PyNN-0.9.6/doc/releases/0.8-alpha-1.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8-alpha-2.txt` & `PyNN-0.9.6/doc/releases/0.8-alpha-2.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8-beta-1.txt` & `PyNN-0.9.6/doc/releases/0.8-beta-1.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8-beta-2.txt` & `PyNN-0.9.6/doc/releases/0.8-beta-2.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8.0-rc-1.txt` & `PyNN-0.9.6/doc/releases/0.8.0-rc-1.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8.0.txt` & `PyNN-0.9.6/doc/releases/0.8.0.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8.2.txt` & `PyNN-0.9.6/doc/releases/0.8.2.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.8.3.txt` & `PyNN-0.9.6/doc/releases/0.8.3.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.9.0.txt` & `PyNN-0.9.6/doc/releases/0.9.0.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.9.1.txt` & `PyNN-0.9.6/doc/releases/0.9.1.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.9.2.txt` & `PyNN-0.9.6/doc/releases/0.9.2.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.9.3.txt` & `PyNN-0.9.6/doc/releases/0.9.3.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/releases/0.9.4.txt` & `PyNN-0.9.6/doc/releases/0.9.4.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/roadmap.txt` & `PyNN-0.9.6/doc/roadmap.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/simulation_control.txt` & `PyNN-0.9.6/doc/simulation_control.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/space.txt` & `PyNN-0.9.6/doc/space.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/doc/standardmodels.txt` & `PyNN-0.9.6/doc/standardmodels.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 ==============  =============  =====  ========================================
 Name            Default value  Units  Description
 ==============  =============  =====  ========================================
 ``v_rest``      -65.0          mV     Resting membrane potential 
 ``cm``            1.0          nF     Capacity of the membrane
 ``tau_m``        20.0          ms     Membrane time constant
-``tau_refrac``    0.0          ms     Duration of refractory period
-``tau_syn_E``     5.0          ms     Rise time of the excitatory synaptic alpha function
-``tau_syn_I``     5.0          ms     Rise time of the inhibitory synaptic alpha function
+``tau_refrac``    0.1          ms     Duration of refractory period
+``tau_syn_E``     0.5          ms     Rise time of the excitatory synaptic alpha function
+``tau_syn_I``     0.5          ms     Rise time of the inhibitory synaptic alpha function
 ``i_offset``      0.0          nA     Offset current
 ``v_reset``     -65.0          mV     Reset potential after a spike
 ``v_thresh``    -50.0          mV     Spike threshold
 ==============  =============  =====  ========================================
 
 
 IF_curr_exp
@@ -51,15 +51,15 @@
     
 ==============  =============  =====  =========================================
 Name            Default value  Units  Description
 ==============  =============  =====  =========================================
 ``v_rest``      -65.0          mV     Resting membrane potential
 ``cm``            1.0          nF     Capacity of the membrane
 ``tau_m``        20.0          ms     Membrane time constant
-``tau_refrac``    0.0          ms     Duration of refractory period
+``tau_refrac``    0.1          ms     Duration of refractory period
 ``tau_syn_E``     5.0          ms     Decay time of excitatory synaptic current
 ``tau_syn_I``     5.0          ms     Decay time of inhibitory synaptic current
 ``i_offset``      0.0          nA     Offset current
 ``v_reset``     -65.0          mV     Reset potential after a spike
 ``v_thresh``    -50.0          mV     Spike threshold
 ==============  =============  =====  =========================================
 
@@ -73,17 +73,17 @@
 
 ==============  =============  =====  ===================================================
 Name            Default value  Units  Description
 ==============  =============  =====  ===================================================
 ``v_rest``      -65.0          mV     Resting membrane potential 
 ``cm``            1.0          nF     Capacity of the membrane
 ``tau_m``        20.0          ms     Membrane time constant
-``tau_refrac``    0.0          ms     Duration of refractory period
-``tau_syn_E``     5.0          ms     Rise time of the excitatory synaptic alpha function
-``tau_syn_I``     5.0          ms     Rise time of the inhibitory synaptic alpha function
+``tau_refrac``    0.1          ms     Duration of refractory period
+``tau_syn_E``     0.3          ms     Rise time of the excitatory synaptic alpha function
+``tau_syn_I``     0.5          ms     Rise time of the inhibitory synaptic alpha function
 ``e_rev_E``       0.0          mV     Reversal potential for excitatory input
 ``e_rev_I``     -70.0          mV     Reversal potential for inhibitory input
 ``v_thresh``    -50.0          mV     Spike threshold
 ``v_reset``     -65.0          mV     Reset potential after a spike
 ``i_offset``      0.0          nA     Offset current
 ==============  =============  =====  ===================================================
 
@@ -97,15 +97,15 @@
     
 ==============  =============  =====  ===================================================
 Name            Default value  Units  Description
 ==============  =============  =====  =================================================== 
 ``v_rest``      -65.0          mV     Resting membrane potential
 ``cm``            1.0          nF     Capacity of the membrane
 ``tau_m``        20.0          ms     Membrane time constant
-``tau_refrac``    0.0          ms     Duration of refractory period
+``tau_refrac``    0.1          ms     Duration of refractory period
 ``tau_syn_E``     5.0          ms     Decay time of the excitatory synaptic conductance
 ``tau_syn_I``     5.0          ms     Decay time of the inhibitory synaptic conductance
 ``e_rev_E``       0.0          mV     Reversal potential for excitatory input
 ``e_rev_I``     -70.0          mV     Reversal potential for inhibitory input
 ``v_thresh``    -50.0          mV     Spike threshold
 ``v_reset``     -65.0          mV     Reset potential after a spike
 ``i_offset``      0.0          nA     Offset current
@@ -147,16 +147,16 @@
 
 Availability: NEST, NEURON, Brian
 
 ==============  =============  =====  ===================================================
 Name            Default value  Units  Description
 ==============  =============  =====  =================================================== 
 ``cm``            0.281        nF     Capacity of the membrane
-``tau_refrac``    0.0          ms     Duration of refractory period
-``v_spike``       0.0          mV     Spike detection threshold
+``tau_refrac``    0.1          ms     Duration of refractory period
+``v_spike``     -40.0          mV     Spike detection threshold
 ``v_reset``     -70.6          mV     Reset value for membrane potential after a spike
 ``v_rest``      -70.6          mV     Resting membrane potential (Leak reversal potential)
 ``tau_m``         9.3667       ms     Membrane time constant
 ``i_offset``      0.0          nA     Offset current
 ``a``             4.0          nS     Subthreshold adaptation conductance
 ``b``             0.0805       nA     Spike-triggered adaptation
 ``delta_T``       2.0          mV     Slope factor
```

### Comparing `PyNN-0.9.5/doc/testdocs.py` & `PyNN-0.9.6/doc/testdocs.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/FakeStepCurrentSource.py` & `PyNN-0.9.6/examples/FakeStepCurrentSource.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/HH_cond_exp2.py` & `PyNN-0.9.6/examples/HH_cond_exp2.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Izhikevich.py` & `PyNN-0.9.6/examples/Izhikevich.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/README.txt` & `PyNN-0.9.6/examples/Potjans2014/README.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/connectivity.py` & `PyNN-0.9.6/examples/Potjans2014/connectivity.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/microcircuit.py` & `PyNN-0.9.6/examples/Potjans2014/microcircuit.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/network.py` & `PyNN-0.9.6/examples/Potjans2014/network.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/network_params.py` & `PyNN-0.9.6/examples/Potjans2014/network_params.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/plotting.py` & `PyNN-0.9.6/examples/Potjans2014/plotting.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/run_microcircuit.py` & `PyNN-0.9.6/examples/Potjans2014/run_microcircuit.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/scaling.py` & `PyNN-0.9.6/examples/Potjans2014/scaling.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/sim_params.py` & `PyNN-0.9.6/examples/Potjans2014/sim_params.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/Potjans2014/validation_microcircuit.py` & `PyNN-0.9.6/examples/Potjans2014/validation_microcircuit.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/README` & `PyNN-0.9.6/examples/README`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/StepCurrentSource.py` & `PyNN-0.9.6/examples/StepCurrentSource.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/VAbenchmarks.py` & `PyNN-0.9.6/examples/VAbenchmarks.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/ball_and_stick.py` & `PyNN-0.9.6/examples/ball_and_stick.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/brunel.py` & `PyNN-0.9.6/examples/brunel.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/cell_type_demonstration.py` & `PyNN-0.9.6/examples/cell_type_demonstration.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,28 +11,26 @@
   --plot-figure  Plot the simulation results to a file.
   --debug        Print debugging information
 
 """
 
 from pyNN.utility import get_simulator, init_logging, normalized_filename
 
-
 # === Configure the simulator ================================================
 
 sim, options = get_simulator(("--plot-figure", "Plot the simulation results to a file.", {"action": "store_true"}),
                              ("--debug", "Print debugging information"))
 
 if options.debug:
     init_logging(None, debug=True)
 
 sim.setup(timestep=0.01, min_delay=1.0)
 
 
 # === Build and instrument the network =======================================
-
 cuba_exp = sim.Population(1, sim.IF_curr_exp(i_offset=1.0), label="IF_curr_exp")
 hh = sim.Population(1, sim.HH_cond_exp(i_offset=0.2), label="HH_cond_exp")
 adexp = sim.Population(1, sim.EIF_cond_exp_isfa_ista(i_offset=1.0), label="EIF_cond_exp_isfa_ista")
 adapt = sim.Population(1, sim.IF_cond_exp_gsfa_grr(i_offset=2.0), label="IF_cond_exp_gsfa_grr")
 izh = sim.Population(1, sim.Izhikevich(i_offset=0.01), label="Izhikevich")
 
 all_neurons = cuba_exp + hh + adexp + adapt + izh
```

### Comparing `PyNN-0.9.5/examples/connection_plot.py` & `PyNN-0.9.6/examples/connection_plot.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/connections.py` & `PyNN-0.9.6/examples/connections.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/current_injection.py` & `PyNN-0.9.6/examples/current_injection.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/distrib_example.py` & `PyNN-0.9.6/examples/distrib_example.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/gif_neuron.py` & `PyNN-0.9.6/examples/gif_neuron.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/gif_neuron_tmp.py` & `PyNN-0.9.6/examples/gif_neuron_tmp.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/README` & `PyNN-0.9.6/examples/iaf_sfa_relref/README`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/backend_comparison.py` & `PyNN-0.9.6/examples/iaf_sfa_relref/backend_comparison.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/iaf_sfa_network_INH_GAMMA.py` & `PyNN-0.9.6/examples/iaf_sfa_relref/iaf_sfa_network_INH_GAMMA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 A PyNN version of the network architecture described in:
 Muller, E., Meier, K., & Schemmel, J. (2004). Methods for simulating
-high-conductance states in neural microcircuits. Proc. of BICS2004. 
+high-conductance states in neural microcircuits. Proc. of BICS2004.
 
 http://neuralensemble.org/people/eilifmuller/Publications/bics2004_mueller.pdf
 
 Script written by Lucas Sinclair & Eilif Muller.
 LCN, EPFL - October 2009
 """
 
-## Debugger ##
-#import pdb
-# pdb.set_trace()
 
 ## Import modules ##
 import numpy, pylab, time
 import pyNN.nest as sim
 import pyNN.common as common
 import pyNN.connectors as connectors
 from pyNN.utility import init_logging
@@ -29,119 +26,119 @@
     """
     Each post-synaptic neuron is connected to exactly n pre-synaptic neurons
     chosen at random.
 
     For every connection that is made the delay is set proportional to
     the distance that separates the two neurons plus some random noise
     coming from a gamma distribution.
-    
+
     N cannot be drawn from a random distribution.
-    
+
     Self connections are always enabled.
     """
-    
+
     def __init__(self, weights=0.0, dist_factor=1.0, noise_factor=0.01, n=1.0):
         """
         Create a new connector.
-        
+
         `weights`      -- The weights of all the connections made.
         `dist_factor`  -- A factor to control the delay (conversion of
                           distance to milliseconds of delay).
-        `noise_factor` -- A factor to control the noise (scale of gamma 
+        `noise_factor` -- A factor to control the noise (scale of gamma
                           distribution).
         `n`            -- Number of connections to make for each neuron.
         """
         connectors.Connector.__init__(self, weights, dt)
         self.dist_factor = dist_factor
         self.noise_factor = noise_factor
         self.n = n
-        
+
     def connect(self, projection):
         """Connect-up a Projection."""
         # Timers
         global rank
         timer0 = 0.0
         timer1 = 0.0
         timer2 = 0.0
         timer3 = 0.0
         timer4 = 0.0
-        
+
         # Recuperate variables #
         n = self.n
         dist_factor = self.dist_factor
         noise_factor = self.noise_factor
-        
+
         # Do some checking #
         assert dist_factor >= 0
         assert noise_factor >= 0
         if isinstance(n, int):
             assert n >= 0
         else:
             raise Exception("n must be an integer.")
-        
+
         # Get posts and pres #
         listPostIDs = projection.post.local_cells
         listPreIDs = projection.pre.all_cells
         countPost = len(listPostIDs)
-        countPre = len(listPreIDs)        
+        countPre = len(listPreIDs)
         listPreIndexes = numpy.arange(countPre)
         listPostIndexes = map(projection.post.id_to_index, listPostIDs)
 
         # Prepare all distances #
-        allDistances = self.space.distances(projection.post.positions, projection.pre.positions)            
-        
+        allDistances = self.space.distances(projection.post.positions, projection.pre.positions)
+
         # Get weights #
         weights = numpy.empty(n)
         weights[:] = self.weights
         is_conductance = common.is_conductance(projection.post[listPostIndexes[0]])
         weights = common.check_weight(weights, projection.synapse_type, is_conductance)
-        
+
         for i in xrange(len(listPostIDs)):
             currentPostIndex = listPostIndexes[i]
             currentPostID = listPostIDs[i]
             #currentPostIDAsList = [currentPostID]
-            
+
             # Pick n neurons at random in pre population
             myTimer = time.time()
             chosenPresIndexes = list(numpy.random.permutation(numpy.arange(countPre))[0:n])
             chosenPresIDs = list(projection.pre[chosenPresIndexes].all_cells)
             #if rank==0:
             #    print(chosenPresIDs)
             #chosenPresIDs = chosenPresIDs.tolist()
             timer0 += time.time() - myTimer
-            
+
             # Get distances
             myTimer = time.time()
             #distances = allDistances[currentPostIndex,chosenPresIndexes]
             distances = allDistances[currentPostIndex, chosenPresIndexes]
             timer1 += time.time() - myTimer
-                        
+
             # Generate gamme noise
             noise = numpy.random.gamma(1.0, noise_factor, n)
-                
+
             # Create delays with distance and noise
             myTimer = time.time()
             delays = dist_factor * distances * (1.0 + noise)
             timer2 += time.time() - myTimer
             #delays[:] = 1.0
-                        
+
             # Check for small and big delays
             myTimer = time.time()
             delaysClipped = numpy.clip(delays, common.get_min_delay(), common.get_max_delay())
             howManyClipped = len((delays != delaysClipped).nonzero()[0])
             if (howManyClipped > 1):
                 print("Warning: %d of %d delays were cliped because they were either bigger than the max delay or lower than the min delay." % (howManyClipped, n))
             delaysClipped = delaysClipped.tolist()
             timer3 += time.time() - myTimer
-                
+
             # Connect everything up
             yTimer = time.time()
             projection._convergent_connect(chosenPresIDs, currentPostID, weights, delaysClipped)
             timer4 += time.time() - myTimer
-            
+
         # Print timings
         if rank == 0:
             print("\033[2;46m" + ("Timer 0: %5.4f seconds" % timer0).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 1: %5.4f seconds" % timer1).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 2: %5.4f seconds" % timer2).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 3: %5.4f seconds" % timer3).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 4: %5.4f seconds" % timer4).ljust(60) + "\033[m")
@@ -430,48 +427,48 @@
 spikesI = popI.getSpikes()
 
 ## Process them ##
 if rank == 0:
     highestIndexE = numpy.max(spikesE[:, 0])
     listNeuronsE = list(spikesE[:, 0])
     listTimesE = list(spikesE[:, 1])
-    listNeuronsI = list(spikesI[:, 0] + highestIndexE) 
+    listNeuronsI = list(spikesI[:, 0] + highestIndexE)
     listTimesI = list(spikesI[:, 1])
 
 ## Kill the bad dir ##
 #print("Tempdir: ", sim.tempdirs)
 #theBadDir = sim.tempdirs
 #thePipe = os.popen("lsof -F f +D " + theBadDir[0])
 #theText = thePipe.read()
 #sts = thePipe.close()
 #m = re.search('\nf(\w+)\n', theText)
 #theFD = m.group(1)
 #os.close(int(theFD))
-    
+
 ## Close the simulation ##
 sim.end()
 
 
 ###################### PLOTTING ###########################
 if rank == 0:
-    
+
 ## Graph Burst ##
     pylab.figure()
     allSpikes = listTimesE + listTimesI
     allNeurons = listNeuronsE + listNeuronsI
     pylab.plot(allSpikes, allNeurons, 'r.', markersize=1, label='Action potentials')
-    
+
     pylab.xlabel("Time [milliseconds]")
     pylab.ylabel("Neuron (first E, then I)")
     pylab.title(("$C_{E\\rightarrow E}=%.2f$, $C_{E\\rightarrow I}=%.2f$," +
                "$C_{I\\rightarrow E}=%.2f$, $C_{I\\rightarrow I}=%.2f$,") %
                 (ICFactorE_E, ICFactorE_I, ICFactorI_E, ICFactorI_I))
     pylab.suptitle("Layer 4 model with Connection Factors:")
     #pylab.legend()
-    
+
     axisHeight = pylab.axis()[3]
     pylab.vlines(tinit, 0.0, axisHeight / 8, linewidth="4", color='k', linestyles='solid')
 
     pylab.plot(tbins, axisHeight / 8 / numpy.max(f) * f, linewidth="2", color='b', linestyle='steps-post')
 
     if numberOfNodes != 0:
         pylab.savefig("myFigure.pdf")
```

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/iaf_sfa_network_STATIC.py` & `PyNN-0.9.6/examples/iaf_sfa_relref/iaf_sfa_network_STATIC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 A PyNN version of the network architecture described in:
 Muller, E., Meier, K., & Schemmel, J. (2004). Methods for simulating
-high-conductance states in neural microcircuits. Proc. of BICS2004. 
+high-conductance states in neural microcircuits. Proc. of BICS2004.
 
 http://neuralensemble.org/people/eilifmuller/Publications/bics2004_mueller.pdf
 
 Script written by Lucas Sinclair & Eilif Muller.
 LCN, EPFL - October 2009
 """
 
-## Debugger ##
-#import pdb
-# pdb.set_trace()
 
 ## Import modules ##
 import numpy, pylab, math, time, os, re
 #import pyNN.nest as sim
 from mpi4py import MPI
 import pyNN.neuron as sim
 import pyNN.common as common
@@ -32,121 +29,121 @@
     """
     Each post-synaptic neuron is connected to exactly n pre-synaptic neurons
     chosen at random.
 
     For every connection that is made the delay is set proportional to
     the distance that separates the two neurons plus some random noise
     coming from a gamma distribution.
-    
+
     N cannot be drawn from a random distribution.
-    
+
     Self connections are always enabled.
     """
-    
+
     def __init__(self, weights=0.0, dist_factor=1.0, noise_factor=0.01, n=1.0):
         """
         Create a new connector.
-        
+
         `weights`      -- The weights of all the connections made.
         `dist_factor`  -- A factor to control the delay (conversion of
                           distance to milliseconds of delay).
-        `noise_factor` -- A factor to control the noise (scale of gamma 
+        `noise_factor` -- A factor to control the noise (scale of gamma
                           distribution).
         `n`            -- Number of connections to make for each neuron.
         """
         connectors.Connector.__init__(self, weights, dist_factor * 1.0)
         self.dist_factor = dist_factor
         self.noise_factor = noise_factor
         self.n = n
-        
+
     def connect(self, projection):
         """Connect-up a Projection."""
         # Timers
         global rank
         timer0 = 0.0
         timer1 = 0.0
         timer2 = 0.0
         timer3 = 0.0
         timer4 = 0.0
-        
+
         # Recuperate variables #
         n = self.n
         dist_factor = self.dist_factor
         noise_factor = self.noise_factor
-        
+
         # Do some checking #
         assert dist_factor >= 0
         assert noise_factor >= 0
         if isinstance(n, int):
             assert n >= 0
         else:
             raise Exception("n must be an integer.")
-        
+
         # Get posts and pres #
         listPostIDs = projection.post.local_cells
         listPreIDs = projection.pre.all_cells
         countPost = len(listPostIDs)
-        countPre = len(listPreIDs)        
+        countPre = len(listPreIDs)
         listPreIndexes = numpy.arange(countPre)
         listPostIndexes = map(projection.post.id_to_index, listPostIDs)
 
         # Prepare all distances #
-        allDistances = self.space.distances(projection.post.positions, projection.pre.positions)            
-        
+        allDistances = self.space.distances(projection.post.positions, projection.pre.positions)
+
         # Get weights #
         weights = numpy.empty(n)
         weights[:] = self.weights
         is_conductance = common.is_conductance(projection.post[listPostIndexes[0]])
         weights = common.check_weight(weights, projection.synapse_type, is_conductance)
 
         numpy.random.seed(12345)
-        
+
         for i in xrange(len(listPostIDs)):
             currentPostIndex = listPostIndexes[i]
             currentPostID = listPostIDs[i]
             #currentPostIDAsList = [currentPostID]
-            
+
             # Pick n neurons at random in pre population
             myTimer = time.time()
             chosenPresIndexes = list(numpy.random.permutation(numpy.arange(countPre))[0:n])
             chosenPresIDs = list(projection.pre[chosenPresIndexes].all_cells)
             #if rank==0:
             #    print(chosenPresIDs)
             #chosenPresIDs = chosenPresIDs.tolist()
             timer0 += time.time() - myTimer
-            
+
             # Get distances
             myTimer = time.time()
             #distances = allDistances[currentPostIndex,chosenPresIndexes]
             distances = allDistances[currentPostIndex, chosenPresIndexes]
             timer1 += time.time() - myTimer
-                        
+
             # Generate gamme noise
             noise = numpy.random.gamma(1.0, noise_factor, n)
-                
+
             # Create delays with distance and noise
             myTimer = time.time()
             delays = dist_factor * distances * (1.0 + noise)
             timer2 += time.time() - myTimer
             #delays[:] = 1.0
-                        
+
             # Check for small and big delays
             myTimer = time.time()
             delaysClipped = numpy.clip(delays, sim.get_min_delay(), sim.get_max_delay())
             howManyClipped = len((delays != delaysClipped).nonzero()[0])
             if (howManyClipped > 1):
                 print("Warning: %d of %d delays were cliped because they were either bigger than the max delay or lower than the min delay." % (howManyClipped, n))
             delaysClipped = delaysClipped.tolist()
             timer3 += time.time() - myTimer
-                
+
             # Connect everything up
             yTimer = time.time()
             projection._convergent_connect(chosenPresIDs, currentPostID, weights, delaysClipped)
             timer4 += time.time() - myTimer
-            
+
         # Print timings
         if rank == 0:
             print("\033[2;46m" + ("Timer 0: %5.4f seconds" % timer0).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 1: %5.4f seconds" % timer1).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 2: %5.4f seconds" % timer2).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 3: %5.4f seconds" % timer3).ljust(60) + "\033[m")
             print("\033[2;46m" + ("Timer 4: %5.4f seconds" % timer4).ljust(60) + "\033[m")
@@ -386,48 +383,48 @@
 spikesI = popI.getSpikes()
 
 ## Process them ##
 if rank == 0:
     highestIndexE = numpy.max(spikesE[:, 0])
     listNeuronsE = list(spikesE[:, 0])
     listTimesE = list(spikesE[:, 1])
-    listNeuronsI = list(spikesI[:, 0] + highestIndexE) 
+    listNeuronsI = list(spikesI[:, 0] + highestIndexE)
     listTimesI = list(spikesI[:, 1])
 
 ## Kill the bad dir ##
 #print("Tempdir: ", sim.tempdirs)
 #theBadDir = sim.tempdirs
 #thePipe = os.popen("lsof -F f +D " + theBadDir[0])
 #theText = thePipe.read()
 #sts = thePipe.close()
 #m = re.search('\nf(\w+)\n', theText)
 #theFD = m.group(1)
 #os.close(int(theFD))
-    
+
 ## Close the simulation ##
 sim.end()
 
 
 ###################### PLOTTING ###########################
 if rank == 0:
-    
+
 ## Graph Burst ##
     pylab.figure()
     allSpikes = listTimesE + listTimesI
     allNeurons = listNeuronsE + listNeuronsI
     pylab.plot(allSpikes, allNeurons, 'r.', markersize=1, label='Action potentials')
-    
+
     pylab.xlabel("Time [milliseconds]")
     pylab.ylabel("Neuron (first E, then I)")
     pylab.title(("$C_{E\\rightarrow E}=%.2f$, $C_{E\\rightarrow I}=%.2f$," +
                "$C_{I\\rightarrow E}=%.2f$, $C_{I\\rightarrow I}=%.2f$,") %
                 (ICFactorE_E, ICFactorE_I, ICFactorI_E, ICFactorI_I))
     pylab.suptitle("Layer 4 model with Connection Factors:")
     #pylab.legend()
-    
+
     axisHeight = pylab.axis()[3]
     pylab.vlines(tinit, 0.0, axisHeight / 8, linewidth="4", color='k', linestyles='solid')
 
     #pylab.plot(tbins,axisHeight/8/numpy.max(f)*f,linewidth="2",color='b',linestyle='steps-post')
 
     if numberOfNodes != 0:
         pylab.savefig("myFigure.pdf")
```

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/mcb.py` & `PyNN-0.9.6/examples/iaf_sfa_relref/mcb.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/myFigure_expected.pdf` & `PyNN-0.9.6/examples/iaf_sfa_relref/myFigure_expected.pdf`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/iaf_sfa_relref/standard_neurons.yaml` & `PyNN-0.9.6/examples/iaf_sfa_relref/standard_neurons.yaml`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/iclamp_test.py` & `PyNN-0.9.6/examples/iclamp_test.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/inhomogeneous_network.py` & `PyNN-0.9.6/examples/inhomogeneous_network.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/multiquantal_synapses.py` & `PyNN-0.9.6/examples/multiquantal_synapses.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         data[label] = populations[label].get_data().segments[0]
         gsyn = data[label].filter(name='gsyn_inh')[0]
         gsyn_mean = neo.AnalogSignal(gsyn.mean(axis=1).reshape(-1, 1),
                                      sampling_rate=gsyn.sampling_rate,
                                      channel_index=np.array([0]))
         gsyn_mean.name = 'gsyn_inh_mean'
         data[label].analogsignals.append(gsyn_mean)
-    #import pdb; pdb.set_trace()
 
     def make_panel(population, label):
         return Panel(population.get_data().segments[0].filter(name='gsyn_inh')[0],
                      data_labels=[label], yticks=True)
     labels = sorted(synapse_types)
     panels = [
         Panel(data[label].filter(name='gsyn_inh_mean')[0],
```

### Comparing `PyNN-0.9.5/examples/nineml_brunel.py` & `PyNN-0.9.6/examples/nineml_brunel.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,31 @@
 from pyNN.utility.plotting import Figure, Panel
 import argparse
 import ninemlcatalog
 
 cases = ['SR', 'SR2', 'SR3', 'SIfast', 'AI', 'SIslow']
 
 parser = argparse.ArgumentParser()
+parser.add_argument('simulator_name',
+                    help=("The simulator to use"))
 parser.add_argument('case',
                     help=("The simulation case to run, can be one of '{}'"
                           .format("', '".join(cases))))
 parser.add_argument('--plot', action='store_true',
                     help=("Plot the resulting figures"))
 parser.add_argument('--limits', nargs=2, default=(900, 1200),
                     metavar=('LOW', 'HIGH'),
                     help="The stop and start time of the plot")
 args = parser.parse_args()
 
 sim.setup()
 
 if args.case not in cases:
     raise Exception("Unrecognised case '{}', allowed cases are '{}'"
-                    .format("', '".join(cases)))
+                    .format(args.case, "', '".join(cases)))
 
 document = ninemlcatalog.load('/network/Brunel2000/' + args.case)
 xml_file = document.url
 
 print("Building network")
 net = Network(sim, xml_file)
```

### Comparing `PyNN-0.9.5/examples/nineml_neuron.py` & `PyNN-0.9.6/examples/nineml_neuron.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/nineml_stdp.py` & `PyNN-0.9.6/examples/nineml_stdp.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/nrn_artificial_cell.py` & `PyNN-0.9.6/examples/nrn_artificial_cell.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 input_conns = sim.Projection(spike_source, cells, sim.FixedProbabilityConnector(0.5), syn,
                              receptor_type="default")
 
 # === Run simulation ===========================================================
 
 sim.run(simtime)
 
-filename = normalized_filename("Results", "small_network", "pkl",
+filename = normalized_filename("Results", "nrn_artificial_cell", "pkl",
                                "neuron", sim.num_processes())
 cells.write_data(filename, annotations={'script_name': __file__})
 
 print("Mean firing rate: ", cells.mean_spike_count() * 1000.0 / simtime, "Hz")
 
 plot_figure = True
 if plot_figure:
```

### Comparing `PyNN-0.9.5/examples/parameter_changes.py` & `PyNN-0.9.6/examples/parameter_changes.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/random_distributions.py` & `PyNN-0.9.6/examples/random_distributions.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/random_numbers.py` & `PyNN-0.9.6/examples/random_numbers.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/simpleRandomNetwork.py` & `PyNN-0.9.6/examples/simpleRandomNetwork.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/simpleRandomNetwork_csa.py` & `PyNN-0.9.6/examples/simpleRandomNetwork_csa.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/simple_STDP.py` & `PyNN-0.9.6/examples/simple_STDP.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/small_network.py` & `PyNN-0.9.6/examples/small_network.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,26 @@
   --debug DEBUG  print debugging information
 
 """
 
 import numpy
 from pyNN.utility import get_simulator, init_logging, normalized_filename
 from pyNN.parameters import Sequence
-from pyNN.random import RandomDistribution as rnd
+from pyNN.random import RandomDistribution as rnd, NumpyRNG
 
 sim, options = get_simulator(("--plot-figure", "Plot the simulation results to a file.", {"action": "store_true"}),
                              ("--debug", "Print debugging information"))
 
 if options.debug:
     init_logging(None, debug=True)
 
 
 # === Define parameters ========================================================
 
-n = 20      # Number of cells
+n = 20     # Number of cells
 w = 0.002  # synaptic weight (µS)
 cell_params = {
     'tau_m'      : 20.0,   # (ms)
     'tau_syn_E'  : 2.0,    # (ms)
     'tau_syn_I'  : 4.0,    # (ms)
     'e_rev_E'    : 0.0,    # (mV)
     'e_rev_I'    : -70.0,  # (mV)
@@ -42,29 +42,32 @@
     'v_reset'    : -70.0,  # (mV)
     'v_thresh'   : -50.0,  # (mV)
     'cm'         : 0.5}    # (nF)
 dt         = 0.1           # (ms)
 syn_delay  = 1.0           # (ms)
 input_rate = 50.0          # (Hz)
 simtime    = 1000.0        # (ms)
+seed       = 945645645
 
 # === Build the network ========================================================
 
 sim.setup(timestep=dt, max_delay=syn_delay)
 
+rng = NumpyRNG(seed=seed)
+
 cells = sim.Population(n, sim.IF_cond_alpha(**cell_params),
-                       initial_values={'v': rnd('uniform', (-60.0, -50.0))},
+                       initial_values={'v': rnd('uniform', (-60.0, -50.0), rng)},
                        label="cells")
 
 number = int(2 * simtime * input_rate / 1000.0)
 numpy.random.seed(26278342)
 
 
 def generate_spike_times(i):
-    gen = lambda: Sequence(numpy.add.accumulate(numpy.random.exponential(1000.0 / input_rate, size=number)))
+    gen = lambda: Sequence(numpy.add.accumulate(dt + numpy.random.exponential(1000.0 / input_rate, size=number)))
     if hasattr(i, "__len__"):
         return [gen() for j in i]
     else:
         return gen()
 assert generate_spike_times(0).max() > simtime
 
 spike_source = sim.Population(n, sim.SpikeSourceArray(spike_times=generate_spike_times))
```

### Comparing `PyNN-0.9.5/examples/specific_network.py` & `PyNN-0.9.6/examples/specific_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 dt         = 0.1         # (ms)
 syn_delay  = 1.0         # (ms)
 input_rate = 50.0       # (Hz)
 simtime    = 1000.0      # (ms)
 
 # === Build the network ========================================================
 
-setup(timestep=dt, max_delay=syn_delay)
+setup(timestep=dt, min_delay=syn_delay, max_delay=syn_delay)
 
 cells = Population(n, IF_curr_alpha(**cell_params), initial_values={'v': 0.0}, label="cells")
 
 number = int(2 * simtime * input_rate / 1000.0)
 numpy.random.seed(26278342)
 
 
 def generate_spike_times(i):
-    gen = lambda: Sequence(numpy.add.accumulate(numpy.random.exponential(1000.0 / input_rate, size=number)))
+    gen = lambda: Sequence(numpy.add.accumulate(dt + numpy.random.exponential(1000.0 / input_rate, size=number)))
     if hasattr(i, "__len__"):
         return [gen() for j in i]
     else:
         return gen()
 assert generate_spike_times(0).max() > simtime
 
 spike_source = Population(n, SpikeSourceArray(spike_times=generate_spike_times))
```

### Comparing `PyNN-0.9.5/examples/stdp_network.py` & `PyNN-0.9.6/examples/stdp_network.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/stochastic_deterministic_comparison.py` & `PyNN-0.9.6/examples/stochastic_deterministic_comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         if 'stochastic' in label:
             gsyn = data[label].filter(name='gsyn_inh')[0]
             gsyn_mean = neo.AnalogSignal(gsyn.mean(axis=1).reshape(-1, 1),
                                          sampling_rate=gsyn.sampling_rate)
             gsyn_mean.channel_index = neo.ChannelIndex(np.array([0]))
             gsyn_mean.name = 'gsyn_inh_mean'
             data[label].analogsignals.append(gsyn_mean)
-    #import pdb; pdb.set_trace()
 
     def make_panel(population, label):
         return Panel(population.get_data().segments[0].filter(name='gsyn_inh')[0],
                      data_labels=[label], yticks=True)
     panels = [
         Panel(data['depressing, deterministic'].filter(name='gsyn_inh')[0][:, 0],
               data_labels=['depressing, deterministic'], yticks=True,
```

### Comparing `PyNN-0.9.5/examples/stochastic_synapses.py` & `PyNN-0.9.6/examples/stochastic_synapses.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/stochastic_tsodyksmarkram.py` & `PyNN-0.9.6/examples/stochastic_tsodyksmarkram.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/stochastic_tsodyksmarkram_em.py` & `PyNN-0.9.6/examples/stochastic_tsodyksmarkram_em.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/synaptic_input.py` & `PyNN-0.9.6/examples/synaptic_input.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/tools/VAbenchmark_graphs.py` & `PyNN-0.9.6/examples/tools/VAbenchmark_graphs.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/tools/comparison_plot.py` & `PyNN-0.9.6/examples/tools/comparison_plot.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/tools/plot_results.py` & `PyNN-0.9.6/examples/tools/plot_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 plt.ion()  # .rcParams['interactive'] = True
 
 example = sys.argv[1]
 
 blocks = {}
 for simulator in 'MOCK', 'NEST', 'NEURON', 'Brian', 'MOOSE', 'Nemo':
-    pattern = "Results/%s_*%s.*" % (example, simulator.lower())
+    pattern = "Results/%s_*%s*.*" % (example, simulator.lower())
     datafiles = glob.glob(pattern)
     if datafiles:
         for datafile in datafiles:
             base = os.path.basename(datafile)
             root = base[:base.find(simulator.lower()) - 1]
             if root not in blocks:
                 blocks[root] = {}
@@ -52,23 +52,25 @@
             lw -= 2
         plt.legend()
         plt.title(name)
         plt.xlabel("Time (ms)")
         plt.ylabel("Vm (mV)")
 
         plt.savefig("Results/%s.png" % name)
+        print("Results/%s.png" % name)
 
-        if blocks[name].values()[0].segments[0].filter(name="gsyn_exc"):
+        if list(blocks[name].values())[0].segments[0].filter(name="gsyn_exc"):
             plt.figure()
             lw = 2 * len(blocks[name]) - 1
             for simulator, block in blocks[name].items():
                 g_exc = block.segments[0].filter(name="gsyn_exc")[0]
-                g_inh = block.segments[0].filter(name="gsyn_inh")[0]            
+                g_inh = block.segments[0].filter(name="gsyn_inh")[0]
                 plt.plot(g_exc.times, g_exc[:, 0], label=simulator + "(exc)", linewidth=lw)
-                plt.plot(g_inh.times, g_inh[:, 0], label=simulator + "(inh)", linewidth=lw)            
+                plt.plot(g_inh.times, g_inh[:, 0], label=simulator + "(inh)", linewidth=lw)
                 lw -= 2
             plt.legend()
             plt.title(name)
             plt.xlabel("Time (ms)")
             plt.ylabel("Synaptic conductance (nS)")
-    
+
             plt.savefig("Results/%s_gsyn.png" % name)
+            print("Results/%s_gsyn.png" % name)
```

### Comparing `PyNN-0.9.5/examples/tools/run_all_examples.py` & `PyNN-0.9.6/examples/tools/run_all_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import subprocess, glob, os, sys
 
-default_simulators = ['MOCK', 'NEST', 'NEURON', 'Brian']
+default_simulators = ['MOCK', 'NEST', 'NEURON', 'Brian2']
 simulator_names = sys.argv[1:]
 if len(simulator_names) > 0:
     for name in simulator_names:
         if name not in default_simulators:
             print("Simulator must be one of: " + ", ".join(default_simulators))
             sys.exit(1)
 else:
@@ -18,47 +18,50 @@
     try:
         exec("import pyNN.%s" % sim)
         simulators.append(sim)
     except ImportError:
         pass
 
 exclude = {
-    'MOCK': ["nineml_neuron.py"],
+    'MOCK': ["nineml_neuron.py", "nineml_brunel.py"],
     'NEURON': ["nineml_neuron.py"],
-    'NEST': ["nineml_neuron.py"],
-    'Brian': ["nineml_neuron.py", "HH_cond_exp2.py", "HH_cond_exp.py", "simpleRandomNetwork_csa.py", "simpleRandomNetwork.py", "simple_STDP2.py", "simple_STDP.py"],
+    'NEST': ["nineml_neuron.py", "nineml_brunel.py"],
+    'Brian2': ["nineml_neuron.py", "nineml_brunel.py", "multiquantal_synapses.py", "random_numbers.py",
+               "gif_neuron.py", "stochastic_tsodyksmarkram.py", "stochastic_deterministic_comparison.py",
+               "stochastic_synapses.py", "varying_poisson.py"]
 }
 
 extra_args = {
     "VAbenchmarks.py": "CUBA",
     "VAbenchmarks2.py": "CUBA",
     "VAbenchmarks2-csa.py": "CUBA",
     "VAbenchmarks3.py": "CUBA",
+    "nineml_brunel.py": "SR"
 }
 
 if not os.path.exists("Results"):
     os.mkdir("Results")
 
 for simulator in simulator_names:
     if simulator.lower() in simulators:
         print("\n\n\n================== Running examples with %s =================\n" % simulator)
         for script in glob.glob("../*.py"):
             script_name = os.path.basename(script)
             if script_name not in exclude[simulator]:
-                cmd = "python %s %s" % (script, simulator.lower())
+                cmd = "%s %s %s" % (sys.executable, script, simulator.lower())
                 if script_name in extra_args:
                     cmd += " " + extra_args[script_name]
                 print(cmd, end='')
                 sys.stdout.flush()
                 logfile = open("Results/%s_%s.log" % (os.path.basename(script), simulator), 'w')
                 p = subprocess.Popen(cmd, shell=True, stdout=logfile, stderr=subprocess.PIPE, close_fds=True)
                 retval = p.wait()
                 print(retval == 0 and " - ok" or " - fail")
     else:
         print("\n\n\n================== %s not available =================\n" % simulator)
 
 print("\n\n\n================== Plotting results =================\n")
 for script in glob.glob("../*.py"):
-    cmd = "python plot_results.py %s" % os.path.basename(script)[:-3]
+    cmd = "%s plot_results.py %s" % (sys.executable, os.path.basename(script)[:-3])
     print(cmd)
     p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, close_fds=True)
     p.wait()
```

### Comparing `PyNN-0.9.5/examples/tsodyksmarkram.py` & `PyNN-0.9.6/examples/tsodyksmarkram.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/update_spike_source_array.py` & `PyNN-0.9.6/examples/update_spike_source_array.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/examples/varying_poisson.py` & `PyNN-0.9.6/examples/varying_poisson.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/__init__.py` & `PyNN-0.9.6/pyNN/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     brian
 
 Other modules:
     utility
     random
     space
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
-__version__ = '0.9.5'
-__all__ = ["common", "random", "nest", "neuron", "brian",
+__version__ = '0.9.6'
+__all__ = ["common", "random", "nest", "neuron", "brian", "brian2",
            "recording", "errors", "space", "descriptions",
            "standardmodels", "parameters", "core", "serialization"]
```

### Comparing `PyNN-0.9.5/pyNN/brian/__init__.py` & `PyNN-0.9.6/pyNN/brian/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Brian implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import logging
 import brian
 from pyNN import common, space
 from pyNN.common.control import DEFAULT_MAX_DELAY, DEFAULT_TIMESTEP, DEFAULT_MIN_DELAY
@@ -30,15 +30,15 @@
 def setup(timestep=DEFAULT_TIMESTEP, min_delay=DEFAULT_MIN_DELAY,
           **extra_params):
     """
     Should be called at the very beginning of a script.
     extra_params contains any keyword arguments that are required by a given
     simulator but not by others.
     """
-    
+
     max_delay = extra_params.get('max_delay', DEFAULT_MAX_DELAY)
     common.setup(timestep, min_delay, **extra_params)
     simulator.state.clear()
     brian.set_global_preferences(**extra_params)
     simulator.state.dt = timestep  # move to common.setup?
     simulator.state.min_delay = min_delay
     simulator.state.max_delay = max_delay
```

### Comparing `PyNN-0.9.5/pyNN/brian/cells.py` & `PyNN-0.9.6/pyNN/brian/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Definition of cell classes for the brian module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 
 import numpy
 import brian
@@ -119,15 +119,15 @@
 
     def __call__(self, P, spikes):
         P.v[spikes] = self.Vr[spikes]
         P.w[spikes] += self.b[spikes]
 
 
 class AdaptiveNeuronGroup(BaseNeuronGroup):
-    
+
     def __init__(self, n, equations, **parameters):
         threshold = brian.SimpleFunThreshold(self.check_threshold)
         period = simplify(parameters['tau_refrac'])
         assert not hasattr(period, "__len__"), "Brian does not support heterogenerous refractory periods with CustomRefractoriness"
         reset = brian.SimpleCustomRefractoriness(
                     AdaptiveReset(parameters.pop('v_reset'),
                                   parameters.pop('b')),
@@ -197,15 +197,15 @@
 
     def __call__(self, P, spikes):
         P.v[spikes] = self.Vr[spikes]
         P.u[spikes] += self.d[spikes]
 
 
 class IzhikevichNeuronGroup(BaseNeuronGroup):
-    
+
     def __init__(self, n, equations, **parameters):
         threshold = brian.SimpleFunThreshold(self.check_threshold)
         reset = brian.SimpleCustomRefractoriness(
                     IzhikevichReset(parameters['v_reset'],
                                     parameters['d']),
                     period=0 * ms)
         refractory = 0 * ms
@@ -217,18 +217,18 @@
         #self._S0 = self._S[:, 0]
 
     v_reset = _new_property('_resetfun.resetfun', 'Vr', mV)
     b = _new_property('_resetfun.resetfun', 'b', nA)
 
     def check_threshold(self, v):
         return v >= 30 * mV
-    
+
 
 class PoissonGroup(brian.PoissonGroup):
-    
+
     def __init__(self, n, equations, **parameters):
         for name, value in parameters.items():
             setattr(self, name, value)
         brian.PoissonGroup.__init__(self, n,
                                     rates=self.update_rates,
                                     clock=simulator.state.network.clock)
 
@@ -245,15 +245,15 @@
 
     def _set_rate(self, value):
         self.firing_rate = value
     rate = property(fset=_set_rate, fget=_get_rate)
 
 
 class SpikeGeneratorGroup(brian.SpikeGeneratorGroup):
-    
+
     def __init__(self, n, equations, spike_times=None):
         """
         Note that `equations` is not used: it is simply for compatibility with
         other NeuronGroup subclasses.
         """
         self._check_spike_times(spike_times)
         spiketimes = [(i, t) for i, seq in enumerate(spike_times) for t in seq.value]
```

### Comparing `PyNN-0.9.5/pyNN/brian/populations.py` & `PyNN-0.9.6/pyNN/brian/populations.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,24 @@
         return ParameterSpace(parameter_dict, shape=(self.size,))
 
     def _set_parameters(self, parameter_space):
         """parameter_space should contain native parameters"""
         parameter_space.evaluate(simplify=False)
         for name, value in parameter_space.items():
             if name == "spike_times":
-                self.brian_group._set_spike_times(value, self.mask)    
+                self.brian_group._set_spike_times(value, self.mask)
             else:
                 getattr(self.brian_group, name)[self.mask] = value
 
     def _set_initial_value_array(self, variable, initial_values):
         raise NotImplementedError
 
     def _get_view(self, selector, label=None):
         return PopulationView(self, selector, label)
-    
+
     @property
     def brian_group(self):
         return self.parent.brian_group
 
 
 class Population(common.Population):
     __doc__ = common.Population.__doc__
@@ -58,30 +58,30 @@
 
     def _create_cells(self):
         id_range = numpy.arange(simulator.state.id_counter,
                                 simulator.state.id_counter + self.size)
         self.all_cells = numpy.array([simulator.ID(id) for id in id_range],
                                      dtype=simulator.ID)
         self._mask_local = numpy.ones((self.size,), bool)  # all cells are local. This doesn't seem very efficient.
-        
+
         if isinstance(self.celltype, StandardCellType):
             parameter_space = self.celltype.native_parameters
         else:
             parameter_space = self.celltype.parameter_space
         parameter_space.shape = (self.size,)
         parameter_space.evaluate(simplify=False)
-        
+
         self.brian_group = self.celltype.brian_model(self.size,
                                                      self.celltype.eqs,
                                                      **parameter_space)
         for id in self.all_cells:
             id.parent = self
         simulator.state.id_counter += self.size
         simulator.state.network.add(self.brian_group)
-    
+
     def _set_initial_value_array(self, variable, value):
         D = self.celltype.state_variable_translations[variable]
         pname = D['translated_name']
         pval = eval(D['forward_transform'], globals(), {variable: value})
         pval = pval.evaluate(simplify=False)
         self.brian_group.initial_values[pname] = pval
         self.brian_group.initialize()
```

### Comparing `PyNN-0.9.5/pyNN/brian/projections.py` & `PyNN-0.9.6/pyNN/brian/projections.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/brian/recording.py` & `PyNN-0.9.6/pyNN/brian/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import logging
 import numpy
 import quantities as pq
 import brian
 from pyNN.core import is_listlike
 from pyNN import recording
 from . import simulator
 
+
 mV = brian.mV
 ms = brian.ms
 uS = brian.uS
 pq.uS = pq.UnitQuantity('microsiemens', 1e-6 * pq.S, 'uS')
 pq.nS = pq.UnitQuantity('nanosiemens', 1e-9 * pq.S, 'nS')
 
 logger = logging.getLogger("PyNN")
@@ -98,10 +99,11 @@
         return all_values
 
     def _local_count(self, variable, filter_ids=None):
         N = {}
         filtered_ids = self.filter_recorded(variable, filter_ids)
         padding = self.population.first_id
         indices = numpy.fromiter(filtered_ids, dtype=int) - padding
+
         for i, id in zip(indices, filtered_ids):
             N[id] = len(self._devices['spikes'].spiketimes[i])
         return N
```

### Comparing `PyNN-0.9.5/pyNN/brian/simulator.py` & `PyNN-0.9.6/pyNN/brian/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Attributes:
     state -- an instance of the _State class.
 
 All other functions and classes are private, and should not be used by other
 modules.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
 import brian
 import numpy
@@ -36,54 +36,54 @@
     def __init__(self, n):
         """Create an ID object with numerical value `n`."""
         int.__init__(n)
         common.IDMixin.__init__(self)
 
 
 class State(common.control.BaseState):
-    
+
     def __init__(self):
         common.control.BaseState.__init__(self)
         self.mpi_rank = 0
         self.num_processes = 1
         self.network = None
         self._min_delay = 'auto'
         self.current_sources = []
         self.clear()
-    
+
     def run(self, simtime):
         self.running = True
         self.network.run(simtime * ms)
-        
+
     def run_until(self, tstop):
         self.run(tstop - self.t)
-        
+
     def clear(self):
         self.recorders = set([])
         self.id_counter = 0
         self.current_sources = []
         self.segment_counter = -1
         if self.network:
             for item in self.network.groups + self.network._all_operations:
                 del item
         self.network = brian.Network()
         self.network.clock = brian.Clock()
         self.reset()
-        
+
     def reset(self):
         """Reset the state of the current network to time t = 0."""
         self.network.reinit()
         self.running = False
         self.t_start = 0
         self.segment_counter += 1
         for group in self.network.groups:
             if hasattr(group, "initialize"):
                 logger.debug("Re-initalizing %s" % group)
                 group.initialize()
-        
+
     def _get_dt(self):
         if self.network.clock is None:
             raise Exception("Simulation timestep not yet set. Need to call setup()")
         return float(self.network.clock.dt / ms)
 
     def _set_dt(self, timestep):
         logger.debug("Setting timestep to %s", timestep)
```

### Comparing `PyNN-0.9.5/pyNN/brian/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/brian/standardmodels/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Standard cells for the Brian module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from copy import deepcopy
 import brian
 from brian import mV, ms, nF, nA, uS, Hz, nS
 from pyNN.standardmodels import cells, build_translations
@@ -277,14 +277,21 @@
         v_offset               : mV
         c_m                    : nF
         i_offset               : nA
         i_inj                  : nA
     ''') + conductance_based_exponential_synapses
     post_synaptic_variables = {'excitatory': 'ge', 'inhibitory': 'gi'}
     state_variable_translations = conductance_based_variable_translations
+    state_variable_translations.update(
+        build_translations(
+                ('m', 'm'),
+                ('h', 'h'),
+                ('n', 'n')
+        )
+    )
     brian_model = BiophysicalNeuronGroup
 
 
 class Izhikevich(cells.Izhikevich):
     __doc__ = cells.Izhikevich.__doc__
 
     translations = build_translations(
@@ -305,30 +312,29 @@
         i_inj                                            : nA
         ''')
     post_synaptic_variables = {'excitatory': 'v', 'inhibitory': 'v'}
     state_variable_translations = build_translations(
                 ('v', 'v', mV),
                 ('u', 'u', mV / ms))
     brian_model = IzhikevichNeuronGroup
-    
+
 
 class SpikeSourcePoisson(cells.SpikeSourcePoisson):
     __doc__ = cells.SpikeSourcePoisson.__doc__
 
     translations = build_translations(
         ('rate',     'firing_rate',        Hz),
         ('start',    'start',       ms),
         ('duration', 'duration',    ms),
     )
     eqs = None
     brian_model = PoissonGroup
-    
+
 
 class SpikeSourceArray(cells.SpikeSourceArray):
     __doc__ = cells.SpikeSourceArray.__doc__
 
     translations = build_translations(
         ('spike_times', 'spike_times', ms),
     )
     eqs = None
     brian_model = SpikeGeneratorGroup
-
```

### Comparing `PyNN-0.9.5/pyNN/brian/standardmodels/electrodes.py` & `PyNN-0.9.6/pyNN/brian/standardmodels/electrodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Classes:
     DCSource           -- a single pulse of current of constant amplitude.
     StepCurrentSource  -- a step-wise time-varying current.
     ACSource           -- a sine modulated current.
     NoisyCurrentSource -- a Gaussian whitish noise current.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
 import numpy
 import brian
```

### Comparing `PyNN-0.9.5/pyNN/brian/standardmodels/synapses.py` & `PyNN-0.9.6/pyNN/brian/standardmodels/synapses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Standard cells for the Brian module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import logging
 from brian import ms
 from pyNN.standardmodels import synapses, build_translations
 from ..simulator import state
@@ -18,29 +18,28 @@
 class StaticSynapse(synapses.StaticSynapse):
     __doc__ = synapses.StaticSynapse.__doc__
 
     eqs = """weight : %(weight_units)s"""
     pre = "%(syn_var)s += weight"
     post = None
     initial_conditions = {}
-
     def __init__(self, **parameters):
         super(StaticSynapse, self).__init__(**parameters)
         # we have to define the translations on a per-instance basis because
         # they depend on whether the synapses are current-, conductance- or voltage-based.
         self.translations = build_translations(
                                 ('weight', 'weight', "weight*weight_units", "weight/weight_units"),
                                 ('delay', 'delay', ms))
 
     def _get_minimum_delay(self):
         d = state.min_delay
         if d == 'auto':
             d = state.dt
         return d
-    
+
     def _set_target_type(self, weight_units):
         for key, value in self.translations.items():
             for direction in ("forward_transform", "reverse_transform"):
                 self.translations[key][direction] = value[direction].replace("weight_units", str(float(weight_units)))
 
 
 class TsodyksMarkramSynapse(synapses.TsodyksMarkramSynapse):
@@ -73,15 +72,15 @@
              %(syn_var)s += weight*x*u
              y += x*u
              '''
     post = None
     initial_conditions = {"u": 0.0, "x": 1.0, "y": 0.0, "z": 0.0}
     tau_syn_var = {"excitatory": "tau_syn_E",
                    "inhibitory": "tau_syn_I"}
-    
+
     def _get_minimum_delay(self):
         d = state.min_delay
         if d == 'auto':
             d = state.dt
         return d
 
     def _set_target_type(self, weight_units):
@@ -141,15 +140,15 @@
             d = state.dt
         return d
 
     def _set_target_type(self, weight_units):
         for key, value in self.translations.items():
             for direction in ("forward_transform", "reverse_transform"):
                 self.translations[key][direction] = value[direction].replace("weight_units", str(float(weight_units)))
-    
+
 
 class AdditiveWeightDependence(synapses.AdditiveWeightDependence):
     __doc__ = synapses.AdditiveWeightDependence.__doc__
 
     translations = build_translations(
         ('w_max',     'w_max', "w_max*weight_units", "w_max/weight_units"),
         ('w_min',     'w_min', "w_min*weight_units", "w_min/weight_units"),
```

### Comparing `PyNN-0.9.5/pyNN/common/__init__.py` & `PyNN-0.9.6/pyNN/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,37 @@
 
 Base classes to be sub-classed by individual backends:
     IDMixin
     Population
     PopulationView
     Assembly
     Projection
-    
+
 Function-factories to generate backend-specific API functions:
     build_reset()
     build_state_queries()
     build_create()
     build_connect()
     build_record()
-    
+
 Common implementation of API functions:
     set()
     initialize()
 
 Function skeletons to be extended by backends:
     setup()
     end()
     run()
 
 Global constants:
     DEFAULT_MAX_DELAY
     DEFAULT_TIMESTEP
     DEFAULT_MIN_DELAY
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from .populations import IDMixin, BasePopulation, Population, PopulationView, Assembly, is_conductance
 from .projections import Projection, Connection
 from .procedural_api import build_create, build_connect, set, build_record, initialize
```

### Comparing `PyNN-0.9.5/pyNN/common/control.py` & `PyNN-0.9.6/pyNN/common/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 
 This module contains:
   * partial implementations of API functions which can be reused by
     backend-specific implementations (in some cases only the docstring
     is intended to be reused)
   * function factories for generating backend-specific API functions.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 DEFAULT_MAX_DELAY = 'auto'
 DEFAULT_TIMESTEP = 0.1
 DEFAULT_MIN_DELAY = 'auto'
 
 assert 'simulator' not in locals()
 
 
 class BaseState(object):
     """Base class for simulator _State classes."""
-    
+
     def __init__(self):
         """Initialize the simulator."""
         self.running = False
         self.t_start = 0
         self.write_on_end = []  # a list of (population, variable, filename) combinations that should be written to file on end()
         self.recorders = set([])
 
 
 def setup(timestep=DEFAULT_TIMESTEP, min_delay=DEFAULT_MIN_DELAY,
            **extra_params):
     """
     Initialises/reinitialises the simulator. Any existing network structure is
     destroyed.
-    
+
     `timestep`, `min_delay` and `max_delay` should all be in milliseconds.
 
     `extra_params` contains any keyword arguments that are required by a given
     simulator but not by others.
     """
     max_delay = extra_params.get('max_delay', DEFAULT_MAX_DELAY)
     invalid_extra_params = ('mindelay', 'maxdelay', 'dt', 'time_step')
@@ -58,15 +58,15 @@
     raise NotImplementedError
 
 
 def build_run(simulator):
     def run_until(time_point, callbacks=None):
         """
         Advance the simulation until `time_point` (in ms).
-        
+
         `callbacks` is an optional list of callables, each of which should
         accept the current time as an argument, and return the next time it
         wishes to be called.
 
         ``run_until()`` and ``run()`` may be combined freely. See the
         documentation of the ``run()`` function for further information.
         """
@@ -92,15 +92,15 @@
         else:
             simulator.state.run_until(time_point)
         return simulator.state.t
 
     def run(simtime, callbacks=None):
         """
         Advance the simulation by `simtime` ms.
-        
+
         `callbacks` is an optional list of callables, each of which should
         accept the current time as an argument, and return the next time it
         wishes to be called.
 
         ``run()`` may be called multiple times during a simulation.
         In between calls to ``run()`` it is possible to retrieve data
         and modify neuron/synapse parameters. Some backends allow modification of
@@ -112,15 +112,15 @@
     return run, run_until
 
 
 def build_reset(simulator):
     def reset(annotations={}):
         """
         Reset the time to zero, neuron membrane potentials and synaptic weights to
-        their initial values, and begin a new Segment for recorded data. 
+        their initial values, and begin a new Segment for recorded data.
         The network structure is not changed, nor are neuron/synapse parameters,
         nor the specification of which neurons to record from.
         """
         for recorder in simulator.state.recorders:
             recorder.store_to_cache(annotations)
         simulator.state.reset()
     return reset
```

### Comparing `PyNN-0.9.5/pyNN/common/populations.py` & `PyNN-0.9.6/pyNN/common/populations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # encoding: utf-8
 """
 Common implementation of ID, Population, PopulationView and Assembly classes.
 
 These base classes should be sub-classed by the backend-specific classes.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import numpy
 import logging
 import operator
 from itertools import chain
@@ -20,14 +20,15 @@
     from functools import reduce
 from collections import defaultdict
 from pyNN import random, recording, errors, standardmodels, core, space, descriptions
 from pyNN.models import BaseCellType
 from pyNN.parameters import ParameterSpace, LazyArray, simplify as simplify_parameter_array
 from pyNN.recording import files
 
+
 deprecated = core.deprecated
 logger = logging.getLogger("PyNN")
 
 
 def is_conductance(target_cell):
     """
     Returns True if the target cell uses conductance-based synapses, False if
@@ -295,15 +296,15 @@
         parameters = dict(parameter_space.items())
         if gather == True and self._simulator.state.num_processes > 1:
             # seems inefficient to do it in a loop - should do as single operation
             for name in parameter_names:
                 values = parameters[name]
                 if isinstance(values, numpy.ndarray):
                     all_values = {self._simulator.state.mpi_rank: values.tolist()}
-                    local_indices = numpy.arange(self.size)[self._mask_local].tolist()
+                    local_indices = numpy.arange(self.size,)[self._mask_local].tolist()
                     all_indices = {self._simulator.state.mpi_rank: local_indices}
                     all_values = recording.gather_dict(all_values)
                     all_indices = recording.gather_dict(all_indices)
                     if self._simulator.state.mpi_rank == 0:
                         values = reduce(operator.add, all_values.values())
                         indices = reduce(operator.add, all_indices.values())
                         idx = numpy.argsort(indices)
@@ -826,15 +827,15 @@
             if isinstance(self.mask, list):
                 self.mask = numpy.array(self.mask)
             if self.mask.dtype is numpy.dtype('bool'):
                 if len(self.mask) != len(self.parent):
                     raise Exception("Boolean masks should have the size of Parent Population")
                 self.mask = numpy.arange(len(self.parent))[self.mask]
             if len(numpy.unique(self.mask)) != len(self.mask):
-                logging.warning("PopulationView can contain only once each ID, duplicated IDs are remove")
+                logging.warning("PopulationView can contain only once each ID, duplicated IDs are removed")
                 self.mask = numpy.unique(self.mask)
         self.all_cells = self.parent.all_cells[self.mask]  # do we need to ensure this is ordered?
         idx = numpy.argsort(self.all_cells)
         self._is_sorted = numpy.all(idx == numpy.arange(len(self.all_cells)))
         self.size = len(self.all_cells)
         self.label = label or "view of '%s' with size %s" % (parent.label, self.size)
         self._mask_local = self.parent._mask_local[self.mask]
@@ -919,14 +920,39 @@
         """
         indices_in_parent = numpy.arange(self.parent.size)[self.mask][indices]
         if hasattr(self.parent, "parent"):
             return self.parent.index_in_grandparent(indices_in_parent)
         else:
             return indices_in_parent
 
+    def index_from_parent_index(self, indices):
+        """
+        Given an index(indices) in the parent population, return
+        the index(indices) within this view.
+        """
+        # todo: add check that all indices correspond to cells that are in this view
+        if isinstance(self.mask, slice):
+            start = self.mask.start or 0
+            step = self.mask.step or 1
+            return (indices - start) / step
+        else:
+            if isinstance(indices, int):
+                return np.nonzero(self.mask == indices)[0][0]
+            elif isinstance(indices, numpy.ndarray):
+                # Lots of ways to do this. Some profiling is in order.
+                # - https://stackoverflow.com/questions/16992713/translate-every-element-in-numpy-array-according-to-key
+                # - https://stackoverflow.com/questions/3403973/fast-replacement-of-values-in-a-numpy-array
+                # - https://stackoverflow.com/questions/13572448/replace-values-of-a-numpy-index-array-with-values-of-a-list
+                parent_indices = self.mask  # assert mask is sorted
+                view_indices = numpy.arange(self.size)
+                index = numpy.digitize(indices, parent_indices, right=True)
+                return view_indices[index]
+            else:
+                raise ValueError("indices must be an integer or an array of integers")
+
     def __eq__(self, other):
         """
         Determine whether two views are the same.
         """
         return not self.__ne__(other)
 
     def __ne__(self, other):
@@ -1055,19 +1081,20 @@
 
     @property
     def receptor_types(self):
         """
         Return a list of receptor types that are common to all populations
         within the assembly.
         """
-        rts = set(self.populations[0].celltype.receptor_types)
+        rts = self.populations[0].celltype.receptor_types
         if len(self.populations) > 1:
+            rts = set(rts)
             for p in self.populations[1:]:
                 rts = rts.intersection(set(p.celltype.receptor_types))
-        return rts
+        return list(rts)
 
     def find_units(self, variable):
         """
         Returns units of the specified variable or parameter, as a string.
         Works for all the recordable variables and neuron parameters of all standard models.
         """
         units = set(p.find_units(variable) for p in self.populations)
```

### Comparing `PyNN-0.9.5/pyNN/common/procedural_api.py` & `PyNN-0.9.6/pyNN/common/procedural_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Alternative, procedural API for creating, connecting and recording from individual neurons
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from .populations import IDMixin, BasePopulation, Assembly
 
 
 def build_create(population_class):
@@ -71,15 +71,15 @@
         Record variables to a file. source can be an individual cell, a
         Population, PopulationView or Assembly.
         """
         # would actually like to be able to record to an array and choose later
         # whether to write to a file.
         if not isinstance(source, (BasePopulation, Assembly)):
             if isinstance(source, (IDMixin)):
-                source = source.as_view()            
+                source = source.as_view()
         source.record(variables, to_file=filename, sampling_interval=sampling_interval)
         if annotations:
             source.annotate(**annotations)
     return record
 
 
 def initialize(cells, **initial_values):
```

### Comparing `PyNN-0.9.5/pyNN/common/projections.py` & `PyNN-0.9.6/pyNN/common/projections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # encoding: utf-8
 """
 Common implementation of the Projection class, to be sub-classed by
 backend-specific Projection classes.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     basestring
     reduce
     xrange
 except NameError:
     basestring = str
     from functools import reduce
     xrange = range
 import numpy
 import logging
 import operator
+from copy import deepcopy
 from pyNN import recording, errors, models, core, descriptions
 from pyNN.parameters import ParameterSpace, LazyArray
 from pyNN.space import Space
 from pyNN.standardmodels import StandardSynapseType
 from .populations import BasePopulation, Assembly
 
 logger = logging.getLogger("PyNN")
@@ -85,38 +86,58 @@
         if isinstance(postsynaptic_neurons, Assembly):
             if not postsynaptic_neurons._homogeneous_synapses:
                 raise errors.ConnectionError('Projection to an Assembly object can be made only with homogeneous synapses types')
 
         self.pre = presynaptic_neurons    # } these really
         self.source = source              # } should be
         self.post = postsynaptic_neurons  # } read-only
-        if receptor_type == "default":
-            receptor_type = None
-        self.receptor_type = receptor_type or sorted(postsynaptic_neurons.receptor_types)[0]
-        # TO FIX: if weights are negative, default should be the first inhibitory receptor type,
-        #         not necessarily the first in alphabetical order.
-        #         Should perhaps explicitly specify the default type(s)
-        if self.receptor_type not in postsynaptic_neurons.receptor_types:
-            valid_types = postsynaptic_neurons.receptor_types
-            assert len(valid_types) > 0
-            errmsg = "User gave receptor_types=%s, receptor_types must be one of: '%s'"
-            raise errors.ConnectionError(errmsg % (self.receptor_type, "', '".join(valid_types)))
         self.label = label
         self.space = space
         self._connector = connector
+
         self.synapse_type = synapse_type or self._static_synapse_class()
         assert isinstance(self.synapse_type, models.BaseSynapseType), \
               "The synapse_type argument must be a models.BaseSynapseType object, not a %s" % type(synapse_type)
+
+        self.receptor_type = receptor_type
+        if self.receptor_type in ("default", None):
+            self._guess_receptor_type()
+        if self.receptor_type not in postsynaptic_neurons.receptor_types:
+            valid_types = postsynaptic_neurons.receptor_types
+            assert len(valid_types) > 0
+            errmsg = "User gave receptor_types=%s, receptor_types must be one of: '%s'"
+            raise errors.ConnectionError(errmsg % (self.receptor_type, "', '".join(valid_types)))
+
         if label is None:
             if self.pre.label and self.post.label:
                 self.label = u"%s→%s" % (self.pre.label, self.post.label)
         self.initial_values = {}
         self.annotations = {}
         Projection._nProj += 1
 
+    def _guess_receptor_type(self):
+        """
+        If the receptor_type is not specified, we follow the convention that the first element
+        in the list of available post-synaptic receptor types is the default for excitatory
+        synapses and the second element is the default for inhibitory synapses.
+        """
+        if len(self.post.receptor_types) > 1:
+            ps = deepcopy(self.synapse_type.parameter_space)
+            ps = self._handle_distance_expressions(ps)
+            weights = ps["weight"]
+            if weights.shape is None:
+                weights.shape = self.shape
+            wl = weights[self.pre.size - 1, self.post.size - 1]
+            if wl >= 0:
+                self.receptor_type = self.post.receptor_types[0]
+            else:
+                self.receptor_type = self.post.receptor_types[1]
+        else:
+            self.receptor_type = self.post.receptor_types[0]
+
     def __len__(self):
         """Return the total number of local connections."""
         raise NotImplementedError
 
     def size(self, gather=True):
         """
         Return the total number of connections.
```

### Comparing `PyNN-0.9.5/pyNN/connectors.py` & `PyNN-0.9.6/pyNN/connectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Defines a common implementation of the built-in PyNN Connector classes.
 
 Simulator modules may use these directly, or may implement their own versions
 for improved performance.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from __future__ import division
 from pyNN.random import RandomDistribution, AbstractRNG, NumpyRNG, get_mpi_config
 from pyNN.core import IndexBasedExpression
 from pyNN import errors, descriptions
@@ -216,22 +216,29 @@
                 connection_parameters = {}
                 for name, map in parameter_space.items():
                     if map.is_homogeneous:
                         connection_parameters[name] = map.evaluate(simplify=True)
                     else:
                         connection_parameters[name] = map[source_mask, col]
 
-#                # Check that parameter values are valid
-#                if self.safe:
-#                    # (might be cheaper to do the weight and delay check before evaluating the larray)
-#                    weights = check_weights(weights, projection.synapse_type, is_conductance(projection.post.local_cells[0]))
-#                    delays = check_delays(delays,
-#                                          projection._simulator.state.min_delay,
-#                                          projection._simulator.state.max_delay)
-#                    # TODO: add checks for plasticity parameters
+                # Check that parameter values are valid
+                if self.safe:
+                    # it might be cheaper to do the weight and delay check before evaluating the larray,
+                    # however this is challenging to do if the base value is a function or if there are
+                    # a lot of operations, so for simplicity we do the check after evaluation
+                    syn = projection.synapse_type
+                    if hasattr(syn, "parameter_checks"):
+                        #raise Exception(f"{connection_parameters} {syn.parameter_checks}")
+                        for parameter_name, check in syn.parameter_checks.items():
+                            native_parameter_name = syn.translations[parameter_name]["translated_name"]
+                            # note that for delays we should also apply units scaling to the check values
+                            # since this currently only affects Brian we can probably handle that separately
+                            # (for weights the checks are all based on zero)
+                            if native_parameter_name in connection_parameters:
+                                check(connection_parameters[native_parameter_name], projection)
 
                 if local:
                     # Connect the neurons
                     #logger.debug("Connecting to %d from %s" % (postsynaptic_index, source_mask))
                     projection._convergent_connect(source_mask, postsynaptic_index, **connection_parameters)
                     if self.callback:
                         self.callback(count / projection.post.local_size)
@@ -935,18 +942,16 @@
 
     if haveCSA:
         def __init__(self, cset, safe=True, callback=None):
             """
             """
             Connector.__init__(self, safe=safe, callback=callback)
             self.cset = cset
-            if csa.arity(cset) == 0:
-                pass
-            else:
-                assert csa.arity(cset) == 2, 'must specify mask or connection-set with arity 2'
+            arity = csa.arity(cset)
+            assert arity in (0, 2), 'must specify mask or connection-set with arity 0 or 2'
     else:
         def __init__(self, cset, safe=True, callback=None):
             raise RuntimeError("CSAConnector not available---couldn't import csa module")
 
     def connect(self, projection):
         """Connect-up a Projection."""
         # Cut out finite part
```

### Comparing `PyNN-0.9.5/pyNN/core.py` & `PyNN-0.9.6/pyNN/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Assorted utility classes and functions.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import warnings
 import numpy
 
 
 def is_listlike(obj):
     """
     Check whether an object (a) can be converted into an array/list *and* has a
     length. This excludes iterators, for example.
 
     Maybe need to split into different functions, as don't always need length.
     """
-    return isinstance(obj, (list, numpy.ndarray, tuple, set))
+    return (
+        isinstance(obj, (list, tuple, set))
+        or (isinstance(obj, numpy.ndarray) and obj.ndim > 0)
+    )
 
 
 def iteritems(obj):
     """Handle the disappearance of `dict.iteritems` in Python 3"""
     try:
         itr = obj.iteritems()  # Python 2
     except AttributeError:
@@ -86,8 +89,7 @@
 
     @projection.setter
     def projection(self, projection):
         self._projection = projection
 
     def __call__(self, i, j):
         raise NotImplementedError
-
```

### Comparing `PyNN-0.9.5/pyNN/descriptions/__init__.py` & `PyNN-0.9.6/pyNN/descriptions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 providing their own templates for `describe()`), they may set the
 DEFAULT_TEMPLATE_ENGINE module attribute, e.g.::
 
 from pyNN import descriptions
 descriptions.DEFAULT_TEMPLATE_ENGINE = 'jinja2'
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     basestring
 except NameError:
     basestring = str
@@ -50,146 +50,146 @@
     else:
         if engine == 'default':
             engine = get_default_template_engine()
         elif isinstance(engine, basestring):
             engine = TEMPLATE_ENGINES[engine]
         assert issubclass(engine, TemplateEngine), str(engine)
         return engine.render(template, context)
-    
-    
+
+
 class TemplateEngine(object):
     """
     Base class.
     """
-    
+
     @classmethod
     def get_template(cls, template):
         """
         template may be either a string containing a template or the name of a
         file (relative to pyNN/descriptions/templates/<engine_name>)
         """
         raise NotImplementedError()
-        
+
     @classmethod
     def render(cls, template, context):
         """
         Render the template with the context.
-        
+
         template may be either a string containing a template or the name of a
         file (relative to pyNN/descriptions/templates/<engine_name>)
-        
+
         context should be a dict.
         """
         raise NotImplementedError()
 
 
 class StringTemplateEngine(TemplateEngine):
     """
     Interface to the built-in string.Template template engine.
     """
     template_dir = os.path.join(os.path.dirname(__file__), 'templates', 'string')
-    
+
     @classmethod
     def get_template(cls, template):
         """
         template may be either a string containing a template or the name of a
         file (relative to pyNN/descriptions/templates/string/)
         """
         template_path = os.path.join(cls.template_dir, template)
         if os.path.exists(template_path):
             f = open(template_path, 'r')
             template = f.read()
             f.close()
         return string.Template(template)
-        
+
     @classmethod
     def render(cls, template, context):
         """
         Render the template with the context.
-        
+
         template may be either a string containing a template or the name of a
         file (relative to pyNN/descriptions/templates/string/)
-        
+
         context should be a dict.
         """
         template = cls.get_template(template)
         return template.safe_substitute(context)
-    
+
 TEMPLATE_ENGINES['string'] = StringTemplateEngine
 
 
 try:
     import jinja2
 
     class Jinja2TemplateEngine(TemplateEngine):
         """
-        Interface to the Jinja2 template engine. 
+        Interface to the Jinja2 template engine.
         """
         env = jinja2.Environment(loader=jinja2.PackageLoader('pyNN.descriptions', 'templates/jinja2'))
-        
+
         @classmethod
         def get_template(cls, template):
             """
             template may be either a string containing a template or the name of a
             file (relative to pyNN/descriptions/templates/jinja2/)
             """
             assert isinstance(template, basestring)
             try:  # maybe template is a file
                 template = cls.env.get_template(template)
             except Exception:  # interpret template as a string
                 template = cls.env.from_string(template)
             return template
-        
+
         @classmethod
         def render(cls, template, context):
             """
             Render the template with the context.
-            
+
             template may be either a string containing a template or the name of a
             file (relative to pyNN/descriptions/templates/jinja2/)
-            
+
             context should be a dict.
             """
             template = cls.get_template(template)
             return template.render(context)
-        
+
     TEMPLATE_ENGINES['jinja2'] = Jinja2TemplateEngine
 except ImportError:
     pass   # jinja2 is an optional dependency
 
 
 try:
     import Cheetah.Template
 
     class CheetahTemplateEngine(TemplateEngine):
         """
         Interface to the Cheetah template engine.
         """
         template_dir = os.path.join(os.path.dirname(__file__), 'templates', 'cheetah')
-        
+
         @classmethod
         def get_template(cls, template):
             """
             template may be either a string containing a template or the name of a
             file (relative to pyNN/descriptions/templates/cheetah)
             """
             template_path = os.path.join(cls.template_dir, template)
             if os.path.exists(template_path):
                 return Cheetah.Template.Template.compile(file=template_path)
             else:
                 return Cheetah.Template.Template.compile(source=template)
-    
+
         @classmethod
         def render(cls, template, context):
             """
             Render the template with the context.
-            
+
             template may be either a string containing a template or the name of a
             file (relative to pyNN/descriptions/templates/cheetah/)
-            
+
             context should be a dict.
             """
             template = cls.get_template(template)(namespaces=[context])
             return template.respond()
 
     TEMPLATE_ENGINES['cheetah'] = CheetahTemplateEngine
 except ImportError:
```

### Comparing `PyNN-0.9.5/pyNN/descriptions/templates/jinja2/population_old.txt` & `PyNN-0.9.6/pyNN/descriptions/templates/jinja2/population_old.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/descriptions/templates/jinja2/projection_default.txt` & `PyNN-0.9.6/pyNN/descriptions/templates/jinja2/projection_default.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/errors.py` & `PyNN-0.9.6/pyNN/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     InvalidModelError
     RoundingWarning
     NothingToWriteError
     InvalidWeightError
     NotLocalError
     RecordingError
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 
 class InvalidParameterValueError(ValueError):
     """Inappropriate parameter value"""
     pass
```

### Comparing `PyNN-0.9.5/pyNN/hardware/__init__.py` & `PyNN-0.9.6/pyNN/hardware/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 hardware implementation of the PyNN API.
 It includes the submodules that stand on another directory.
-This solution is a clean way to make the submodules (brainscales, etc...) 
+This solution is a clean way to make the submodules (brainscales, etc...)
 be indeed submodules of hardware, even if they don't stand on the same directory
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
-from aux import get_path_to_analog_hardware_backend, import_all_submodules
+from auxiliary import get_path_to_analog_hardware_backend, import_all_submodules
 
 __path__.append(get_path_to_analog_hardware_backend())
 import_all_submodules(__path__)
```

### Comparing `PyNN-0.9.5/pyNN/mock/__init__.py` & `PyNN-0.9.6/pyNN/mock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Mock implementation of the PyNN API, for testing and documentation purposes.
 
 This simulator implements the PyNN API, but generates random data rather than
 really running simulations.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import logging
 from pyNN import common
 from pyNN.common.control import DEFAULT_MAX_DELAY, DEFAULT_TIMESTEP, DEFAULT_MIN_DELAY
 from pyNN.connectors import *
```

### Comparing `PyNN-0.9.5/pyNN/mock/populations.py` & `PyNN-0.9.6/pyNN/mock/populations.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/mock/projections.py` & `PyNN-0.9.6/pyNN/mock/projections.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/mock/recording.py` & `PyNN-0.9.6/pyNN/mock/recording.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/mock/simulator.py` & `PyNN-0.9.6/pyNN/mock/simulator.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/mock/standardmodels.py` & `PyNN-0.9.6/pyNN/mock/standardmodels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Standard cells for the mock module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from pyNN.standardmodels import cells, synapses, electrodes, build_translations, StandardCurrentSource
 from .simulator import state
 import logging
 
@@ -171,25 +171,25 @@
         ('e_rev_I',    'E_REV_I'),
         ('tau_syn_I',  'TAU_SYN_I'),
     )
 
 
 class Izhikevich(cells.Izhikevich):
     __doc__ = cells.Izhikevich.__doc__
-    
+
     translations = build_translations(
         ('a',        'a'),
         ('b',        'b'),
         ('c',        'c'),
         ('d',        'd'),
         ('i_offset', 'I_e'),
     )
     standard_receptor_type = True
     receptor_scale = 1e-3  # synaptic weight is in mV, so need to undo usual weight scaling
-    
+
 
 class MockCurrentSource(object):
 
     def inject_into(self, cells):
         __doc__ = StandardCurrentSource.inject_into.__doc__
         pass
 
@@ -260,15 +260,15 @@
         ('U', 'UU'),
         ('tau_rec', 'TAU_REC'),
         ('tau_facil', 'TAU_FACIL'),
         ('u0', 'U0'),
         ('x0', 'X'),
         ('y0', 'Y')
     )
-    
+
     def _get_minimum_delay(self):
         d = state.min_delay
         if d == 'auto':
             d = state.dt
         return d
 
 
@@ -282,15 +282,15 @@
     )
 
     def _get_minimum_delay(self):
         d = state.min_delay
         if d == 'auto':
             d = state.dt
         return d
-    
+
 
 class AdditiveWeightDependence(synapses.AdditiveWeightDependence):
     __doc__ = synapses.AdditiveWeightDependence.__doc__
 
     translations = build_translations(
         ('w_max',     'wmax'),
         ('w_min',     'wmin'),
```

### Comparing `PyNN-0.9.5/pyNN/models.py` & `PyNN-0.9.6/pyNN/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Base classes for cell and synapse models, whether "standard" (cross-simulator)
 or "native" (restricted to an individual simulator).
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from pyNN import descriptions
 from pyNN.parameters import ParameterSpace
 
 
@@ -68,29 +68,29 @@
 
 class BaseCellType(BaseModelType):
     """Base class for cell model classes."""
     recordable = []
     receptor_types = []
     conductance_based = True  # override for cells with current-based synapses
     injectable = True  # override for spike sources
-    
+
     def can_record(self, variable):
         return variable in self.recordable
 
 
 class BaseCurrentSource(BaseModelType):
     """Base class for current source model classes."""
     pass
 
 
 class BaseSynapseType(BaseModelType):
     """Base class for synapse model classes."""
-    
+
     connection_type = None  # override to specify a non-standard connection type (i.e. GapJunctions)
-    has_presynaptic_components = False  # override for synapses that include an active presynaptic components 
+    has_presynaptic_components = False  # override for synapses that include an active presynaptic components
 
     def __init__(self, **parameters):
         """
         `parameters` should be a mapping object, e.g. a dict
         """
         all_parameters = self.default_parameters.copy()
         if parameters:
```

### Comparing `PyNN-0.9.5/pyNN/moose/__init__.py` & `PyNN-0.9.6/pyNN/moose/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # encoding: utf-8
 """
 MOOSE implementation of the PyNN API
 
 Authors: Subhasis Ray and Andrew Davison
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import moose
 import numpy
 import shutil
@@ -95,15 +95,15 @@
 
     def _get_view(self, selector, label=None):
         return PopulationView(self, selector, label)
 
     def _create_cells(self, cellclass, cellparams, n):
         """
         Create cells in MOOSE.
-        
+
         `cellclass`  -- a PyNN standard cell or a native MOOSE model.
         `cellparams` -- a dictionary of cell parameters.
         `n`          -- the number of cells to create
         """
         assert n > 0, 'n must be a positive integer'
         if isinstance(cellclass, type) and issubclass(cellclass, standardmodels.StandardCellType):
             celltype = cellclass(cellparams)
@@ -158,36 +158,36 @@
         """
         common.Projection.__init__(self, presynaptic_population, postsynaptic_population,
                                    method, source, target,
                                    synapse_dynamics, label, rng)
         self.synapse_type = target or 'excitatory'
         assert synapse_dynamics is None, "don't yet handle synapse dynamics"
         self.synapse_model = None
-        self.connections = []        
-        
+        self.connections = []
+
         # Create connections
         method.connect(self)
-        
+
     def _divergent_connect(self, source, targets, weights, delays):
         """
         Connect a neuron to one or more other neurons with a static connection.
-        
+
         `source`  -- the ID of the pre-synaptic cell.
         `targets` -- a list/1D array of post-synaptic cell IDs, or a single ID.
         `weight`  -- a list/1D array of connection weights, or a single weight.
                      Must have the same length as `targets`.
         `delays`  -- a list/1D array of connection delays, or a single delay.
                      Must have the same length as `targets`.
         """
         if not isinstance(source, int) or source > simulator.state.gid_counter or source < 0:
             errmsg = "Invalid source ID: %s (gid_counter=%d)" % (source, simulator.state.gid_counter)
             raise errors.ConnectionError(errmsg)
         if not core.is_listlike(targets):
             targets = [targets]
-            
+
         weights = weights * 1000.0  # scale units
         if isinstance(weights, float):
             weights = [weights]
         if isinstance(delays, float):
             delays = [delays]
         assert len(targets) > 0
         # need to scale weights for appropriate units
@@ -203,15 +203,15 @@
                     synapse_object = getattr(target._cell, self.synapse_type)
                 source._cell.source.connect('event', synapse_object, 'synapse')
                 synapse_object.n_incoming_connections += 1
                 index = synapse_object.n_incoming_connections - 1
                 synapse_object.setWeight(index, weight)
                 synapse_object.setDelay(index, delay)
                 self.connections.append((source, target, index))
-                
+
 # ==============================================================================
 #   Low-level API for creating, connecting and recording from individual neurons
 # ==============================================================================
 
 create = common.build_create(Population)
 
 connect = common.build_connect(Projection, FixedProbabilityConnector)
@@ -221,8 +221,7 @@
 record = common.build_record('spikes', simulator)
 
 record_v = common.build_record('v', simulator)
 
 record_gsyn = common.build_record('gsyn', simulator)
 
 # ==============================================================================
-
```

### Comparing `PyNN-0.9.5/pyNN/moose/cells.py` & `PyNN-0.9.6/pyNN/moose/cells.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import moose
 import numpy
 import uuid
 import os
@@ -15,22 +15,22 @@
 ms = 1e-3
 nA = 1e-9
 uS = 1e-6
 nF = 1e-9
 
 
 class RecorderMixin(object):
-    
+
     def record_spikes(self):
         self.spike_table = moose.Table("spikes", self)
         self.spike_table.stepMode = 4
         self.spike_table.stepSize = 0.5
         self.spike_table.useClock(0)
         self.spike_table.connect('inputRequest', self.source, 'state')
-    
+
     def record_v(self):
         self.vmTable = moose.Table("Vm", self)
         self.vmTable.stepMode = 3
         self.vmTable.connect("inputRequest", self.comp, "Vm")
         self.vmTable.useClock(2)
         print("vmTable is at %s" % self.vmTable.path)
 
@@ -44,15 +44,15 @@
         self.gsyn_tables[syn_name] = moose.Table(syn_name, self)
         self.gsyn_tables[syn_name].stepMode = 3
         self.gsyn_tables[syn_name].connect("inputRequest", syn_map[syn_name], "Gk")
         self.gsyn_tables[syn_name].useClock(2)
 
 
 class SingleCompHH(moose.Neutral, RecorderMixin):
-    
+
     def __init__(self, path, GbarNa=20 * uS, GbarK=6 * uS, GLeak=0.01 * uS, Cm=0.2 * nF,
                  ENa=40 * mV, EK=-90 * mV, VLeak=-65 * mV, Voff=-63 * mV, ESynE=0 * mV,
                  ESynI=-70 * mV, tauE=2 * ms, tauI=5 * ms, inject=0 * nA, initVm=-65 * mV):
         moose.Neutral.__init__(self, path)
         self.comp = moose.Compartment("compartment", self)
         print("compartment is at %s" % self.comp.path)
         print(locals())
@@ -76,107 +76,107 @@
         self.k.Gbar = GbarK
         self.k.Xpower = 4
         self.k.setupAlpha("X", 3.2e4 * (15 * mV + Voff), -3.2e4, -1, -(15 * mV + Voff), -5 * mV,
                                500,                  0,       0, -(10 * mV + Voff),  40 * mV)
 
         self.esyn = moose.SynChan("excitatory", self.comp)
         self.esyn.Ek = ESynE
-        self.esyn.tau1 = tauE 
+        self.esyn.tau1 = tauE
         self.isyn = moose.SynChan("inhibitory", self.comp)
         self.isyn.Ek = ESynI
         self.isyn.tau1 = tauI
         for syn in self.esyn, self.isyn:
             syn.tau2 = 1e-6
             syn.Gbar = 1 * uS
             self.comp.connect("channel", syn, "channel")
             syn.n_incoming_connections = 0
 
         self.comp.connect("channel", self.na, "channel")
         self.comp.connect("channel", self.k,  "channel")
-        
+
         self.comp.useClock(0)
         self.comp.useClock(1, "init")
-        
+
         self.source = moose.SpikeGen("source", self.comp)
         self.source.thresh = 0.0
         self.source.abs_refract = 2.0
         self.comp.connect("VmSrc", self.source, "Vm")
 
     # need to create some properties, so we can update parameter values after creation
 
 
 class StandardIF(moose.IntFire, RecorderMixin):
-    
+
     def __init__(self, path, syn_shape, Cm=1.0, Em=0.0, Rm=1.0, Vr=0.0, Vt=1.0,
                  refractT=0.0, inject=0.0, tau_e=0.001, tau_i=0.001, e_e=0.0,
                  e_i=-0.07):
         moose.IntFire.__init__(self, path)
         self.Cm = Cm
         self.Em = Em
         self.Rm = Rm
         self.Vr = Vr
         self.Vt = Vt
         self.refractT = refractT
         self.inject = inject
-        
+
         self.syn_shape = syn_shape
         self.esyn = moose.SynChan("%s/excitatory" % path)
         self.isyn = moose.SynChan("%s/inhibitory" % path)
         for syn in self.esyn, self.isyn:
             syn.tau2 = 1e-6  # instantaneous rise, for shape=='exp'
             syn.Gbar = 1 * uS
             self.connect("channel", syn, "channel")
             syn.n_incoming_connections = 0
-        
+
         self.tau_e = tau_e
         self.tau_i = tau_i
         self.e_e = e_e
         self.e_i = e_i
-        
+
         self.source = moose.SpikeGen("source", self)
         self.source.thresh = 0.0
         self.source.abs_refract = 2.0
         self.connect("VmSrc", self.source, "Vm")
         self.comp = self  # for recorder mixin
-        
+
     def _get_tau_e(self):
         return self.esyn.tau1
 
     def _set_tau_e(self, val):
         self.esyn.tau1 = val
         if self.syn_shape == 'alpha':
             self.esyn.tau2 = val
     tau_e = property(fget=_get_tau_e, fset=_set_tau_e)
-    
+
     def _get_tau_i(self):
         return self.isyn.tau1
 
     def _set_tau_i(self, val):
         self.isyn.tau1 = val
         if self.syn_shape == 'alpha':
             self.isyn.tau2 = val
     tau_i = property(fget=_get_tau_i, fset=_set_tau_i)
-    
+
     def _get_e_e(self):
         return self.esyn.Ek
 
     def _set_e_e(self, val):
         self.esyn.Ek = val
     e_e = property(fget=_get_e_e, fset=_set_e_e)
-    
+
     def _get_e_i(self):
         return self.isyn.Ek
 
     def _set_e_i(self, val):
         self.isyn.Ek = val
     e_i = property(fget=_get_e_i, fset=_set_e_i)
- 
+
 
 class RandomSpikeSource(moose.RandomSpike):
-    
+
     def __init__(self, path, rate, start=0.0, duration=numpy.inf):
         moose.RandomSpike.__init__(self, path)
         self.minAmp = 1.0
         self.maxAmp = 1.0
         self.rate = rate
         self.reset = 1  # True
         self.resetValue = 0.0
@@ -189,27 +189,27 @@
         self.stateTable = moose.Table("state", self)
         self.stateTable.stepMode = 3
         self.stateTable.connect("inputRequest", self, "state")
         self.stateTable.useClock(2)
 
 
 class VectorSpikeSource(moose.TimeTable):
-    
+
     def __init__(self, path, spike_times):
         moose.TimeTable.__init__(self, path)
         self._save_spikes(spike_times)
         self.source = self
-        
+
     def _save_spikes(self, spike_times):
         ms = 1e-3
         self._spike_times = spike_times
         filename = self.filename or "%s/%s.spikes" % (temporary_directory,
                                                       uuid.uuid4().hex)
         numpy.savetxt(filename, spike_times * ms, "%g")
         self.filename = filename
-        
+
     def _get_spike_times(self):
         return self._spike_times
 
     def _set_spike_times(self, spike_times):
         self._save_spikes(spike_times)
     spike_times = property(fget=_get_spike_times, fset=_set_spike_times)
```

### Comparing `PyNN-0.9.5/pyNN/moose/recording.py` & `PyNN-0.9.6/pyNN/moose/recording.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import numpy
 from pyNN import recording
 from pyNN.moose import simulator
 
 # --- For implementation of record_X()/get_X()/print_X() -----------------------
 
 
 class Recorder(recording.Recorder):
     """Encapsulates data and functions related to recording model variables."""
-        
+
     def _record(self, new_ids):
         """Add the cells in `new_ids` to the set of recorded cells."""
         if self.variable == 'spikes':
             for id in new_ids:
                 id._cell.record_spikes()
         elif self.variable == 'v':
             for id in new_ids:
                 id._cell.record_v()
         elif self.variable == 'gsyn':
             for id in new_ids:
                 id._cell.record_gsyn("excitatory")
                 id._cell.record_gsyn("inhibitory")
         else:
             raise Exception("Recording of %s not implemented." % self.variable)
-    
+
     def _reset(self):
         raise NotImplementedError("TO DO")
-    
+
     def _get(self, gather=False, compatible_output=True, filter=None):
         """Return the recorded data as a Numpy array."""
         # compatible_output is not used, but is needed for compatibility with the nest module.
-        # Does nest really need it?                
+        # Does nest really need it?
         if self.variable == 'spikes':
             data = numpy.empty((0, 2))
             for id in self.recorded:
                 spikes = 1e3 * numpy.array(id._cell.spike_table)  # convert from s to ms
                 spikes = spikes[spikes <= simulator.state.t + 1e-9]
-                if len(spikes) > 0:    
+                if len(spikes) > 0:
                     new_data = numpy.array([numpy.ones(spikes.shape) * id, spikes]).T
                     data = numpy.concatenate((data, new_data))
         elif self.variable == 'v':
             data = numpy.empty((0, 3))
             for id in self.recorded:
                 v = 1e3 * numpy.array(id._cell.vmTable)  # convert from V to mV
                 t = simulator.state.dt * numpy.arange(0.0, v.size)
                 new_data = numpy.array([numpy.ones(v.shape) * id, t, v]).T
                 data = numpy.concatenate((data, new_data))
         elif self.variable == 'gsyn':
             data = numpy.empty((0, 4))
             for id in self.recorded:
                 ge = 1e6 * numpy.array(id._cell.gsyn_trace['excitatory'])  # convert from S to uS
                 gi = 1e6 * numpy.array(id._cell.gsyn_trace['inhibitory'])
-                t = simulator.state.dt * numpy.arange(0.0, ge.size)           
+                t = simulator.state.dt * numpy.arange(0.0, ge.size)
                 new_data = numpy.array([numpy.ones(ge.shape) * id, t, ge, gi]).T
                 data = numpy.concatenate((data, new_data))
         else:
             raise Exception("Recording of %s not implemented." % self.variable)
     #    if gather and simulator.state.num_processes > 1:
     #        data = recording.gather(data)
-    
+
         if filter is not None:
             filtered_ids = self.filter_recorded(filter)
             mask = reduce(numpy.add, (data[:, 0] == id for id in filtered_ids))
             data = data[mask]
         return data
-        
+
     def _local_count(self, filter=None):
         N = {}
         for id in self.filter_recorded(filter):
             N[int(id)] = len(id._cell.spike_table)
         return N
```

### Comparing `PyNN-0.9.5/pyNN/moose/simple_example.py` & `PyNN-0.9.6/pyNN/moose/simple_example.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/moose/simulator.py` & `PyNN-0.9.6/pyNN/moose/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Functions and classes useable by the common implementation:
     run()
 
 
 All other functions and classes are private, and should not be used by other
 modules.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import moose
 from pyNN import common, core
 
@@ -25,27 +25,27 @@
 in_ms = 1.0 / ms
 
 # --- For implementation of get_time_step() and similar functions --------------
 
 
 class _State(object):
     """Represent the simulator state."""
-    
+
     def __init__(self):
         self.ctx = moose.PyMooseBase.getContext()
         self.gid_counter = 0
         self.num_processes = 1  # we're not supporting MPI
         self.mpi_rank = 0      # for now
         self.min_delay = 0.0
         self.max_delay = 1e12
 
     @property
     def t(self):
         return self.ctx.getCurrentTime() * in_ms
-    
+
     def __get_dt(self):
         return self.ctx.getClocks()[0] * in_ms
 
     def __set_dt(self, dt):
         print("setting dt to %g ms" % dt)
         self.ctx.setClock(0, dt * ms, 0)  # integration clock
         self.ctx.setClock(1, dt * ms, 1)  # ?
@@ -63,41 +63,41 @@
     state.ctx.reset()
 
 # --- For implementation of access to individual neurons' parameters -----------
 
 
 class ID(int, common.IDMixin):
     __doc__ = common.IDMixin.__doc__
-    
+
     def __init__(self, n):
         """Create an ID object with numerical value `n`."""
         int.__init__(n)
         common.IDMixin.__init__(self)
-    
+
     def _build_cell(self, cell_model, cell_parameters):
         """
         Create a cell in MOOSE, and register its global ID.
-        
+
         `cell_model` -- one of the cell classes defined in the
                         `moose.cells` module (more generally, any class that
                         implements a certain interface, but I haven't
                         explicitly described that yet).
         `cell_parameters` -- a dictionary containing the parameters used to
                              initialise the cell model.
         """
         id = int(self)
         self._cell = cell_model("neuron%d" % id, **cell_parameters)          # create the cell object
-        
+
 #    def get_native_parameters(self):
 #        """Return a dictionary of parameters for the NEURON cell model."""
 #        D = {}
 #        for name in self._cell.parameter_names:
 #            D[name] = getattr(self._cell, name)
 #        return D
-    
+
 #    def set_native_parameters(self, parameters):
 #        """Set parameters of the NEURON cell model from a dictionary."""
 #        for name, val in parameters.items():
 #            setattr(self._cell, name, val)
 
 state = _State()  # a Singleton, so only a single instance ever exists
 del _State
```

### Comparing `PyNN-0.9.5/pyNN/moose/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/moose/standardmodels/cells.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 
 from pyNN.standardmodels import build_translations, cells
 from pyNN.moose.cells import StandardIF, SingleCompHH, RandomSpikeSource, VectorSpikeSource
 from pyNN.moose.cells import mV, ms, nA, uS, nF
 
-    
+
 class IF_cond_exp(cells.IF_cond_exp):
-    
-    __doc__ = cells.IF_cond_exp.__doc__    
-    
+
+    __doc__ = cells.IF_cond_exp.__doc__
+
     translations = build_translations(
         ('tau_m',      'Rm',        '1e6*tau_m/cm',     '1e3*Rm*Cm'),
         ('cm',         'Cm',        nF),
         ('v_rest',     'Em',        mV),
         ('v_thresh',   'Vt',        mV),
         ('v_reset',    'Vr',        mV),
         ('tau_refrac', 'refractT',  ms),
@@ -35,66 +35,59 @@
         self.parameters['syn_shape'] = 'exp'
 
 
 class IF_cond_alpha(cells.IF_cond_alpha):
     """Leaky integrate and fire model with fixed threshold and alpha-function-
     shaped post-synaptic conductance."""
 
-    __doc__ = cells.IF_cond_alpha.__doc__        
+    __doc__ = cells.IF_cond_alpha.__doc__
 
     translations = IF_cond_exp.translations
     model = StandardIF
-    
+
     def __init__(self, parameters):
         cells.IF_cond_alpha.__init__(self, parameters)
         self.parameters['syn_shape'] = 'alpha'
 
 
 class HH_cond_exp(cells.HH_cond_exp):
-    
-    __doc__ = cells.HH_cond_exp.__doc__    
+
+    __doc__ = cells.HH_cond_exp.__doc__
 
     translations = build_translations(
-        ('gbar_Na',    'GbarNa', 1e-9),   
-        ('gbar_K',     'GbarK', 1e-9),    
-        ('g_leak',     'GLeak', 1e-9),    
-        ('cm',         'Cm',    1e-9),  
+        ('gbar_Na',    'GbarNa', 1e-9),
+        ('gbar_K',     'GbarK', 1e-9),
+        ('g_leak',     'GLeak', 1e-9),
+        ('cm',         'Cm',    1e-9),
         ('v_offset',   'Voff', 1e-3),
         ('e_rev_Na',   'ENa', 1e-3),
-        ('e_rev_K',    'EK', 1e-3), 
+        ('e_rev_K',    'EK', 1e-3),
         ('e_rev_leak', 'VLeak', 1e-3),
         ('e_rev_E',    'ESynE', 1e-3),
         ('e_rev_I',    'ESynI', 1e-3),
         ('tau_syn_E',  'tauE', 1e-3),
         ('tau_syn_I',  'tauI', 1e-3),
         ('i_offset',   'inject', 1e-9),
     )
     model = SingleCompHH
 
 
 class SpikeSourcePoisson(cells.SpikeSourcePoisson):
-    
-    __doc__ = cells.SpikeSourcePoisson.__doc__     
+
+    __doc__ = cells.SpikeSourcePoisson.__doc__
 
     translations = build_translations(
         ('start',    'start'),
         ('rate',     'rate'),
         ('duration', 'duration'),
     )
     model = RandomSpikeSource
 
 
 class SpikeSourceArray(cells.SpikeSourceArray):
-    
-    __doc__ = cells.SpikeSourceArray.__doc__    
+
+    __doc__ = cells.SpikeSourceArray.__doc__
 
     translations = build_translations(
         ('spike_times', 'spike_times'),
     )
     model = VectorSpikeSource
-
-
-
-
-
-
-
```

### Comparing `PyNN-0.9.5/pyNN/multisim.py` & `PyNN-0.9.6/pyNN/multisim.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A small framework to make it easier to run the same model on multiple
 simulators.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from multiprocessing import Process, Queue
 
 
 def run_simulation(network_model, sim, parameters, input_queue, output_queue):
@@ -27,63 +27,63 @@
 
 
 class MultiSim(object):
     """
     Interface that runs a network model on different simulators, with each
     simulation in a separate process.
     """
-    
+
     def __init__(self, sim_list, network_model, parameters):
         """
         Build the model defined in the class `network_model`, with parameters
         `parameters`, for each of the simulator modules specified in `sim_list`.
-        
+
         The `network_model` constructor takes arguments `sim` and `parameters`.
         """
         self.processes = {}
         self.task_queues = {}
         self.result_queues = {}
         for sim in sim_list:
             task_queue = Queue()
             result_queue = Queue()
             p = Process(target=run_simulation,
                         args=(network_model, sim, parameters, task_queue, result_queue))
             p.start()
             self.processes[sim.__name__] = p
             self.task_queues[sim.__name__] = task_queue
             self.result_queues[sim.__name__] = result_queue
-            
+
     def __iter__(self):
         return self.processes.itervalues()
-    
+
     def __getattr__(self, name):
         """
         Assumes `name` is a method of the `network_model` model.
         Return a function that runs `net.name()` for all the simulators.
         """
         def iterate_over_nets(*args, **kwargs):
             retvals = {}
             for sim_name in self.processes:
                 self.task_queues[sim_name].put(('network', name, args, kwargs))
             for sim_name in self.processes:
                 retvals[sim_name] = self.result_queues[sim_name].get()
             return retvals
         return iterate_over_nets
-            
+
     def run(self, simtime, steps=1):  # , *callbacks):
         """
         Run the model for a time `simtime` in all simulators.
-        
+
         The run may be broken into a number of steps (each of equal duration).
         #Any functions in `callbacks` will be called after each step.
         """
         dt = float(simtime) / steps
         for i in range(steps):
             for sim_name in self.processes:
                 self.task_queues[sim_name].put(('sim', 'run', [dt], {}))
             for sim_name in self.processes:
                 t = self.result_queues[sim_name].get()
-                
+
     def end(self):
         for sim_name in self.processes:
             self.task_queues[sim_name].put('STOP')
             self.processes[sim_name].join()
```

### Comparing `PyNN-0.9.5/pyNN/nemo/__init__.py` & `PyNN-0.9.6/pyNN/nemo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Nemo implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
 import nemo
 from pyNN.nemo import simulator
```

### Comparing `PyNN-0.9.5/pyNN/nemo/connectors.py` & `PyNN-0.9.6/pyNN/nemo/connectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Connection method classes for the nemo module
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 from pyNN.space import Space
 from pyNN.random import RandomDistribution
 import numpy
 from pyNN import random, common, core
```

### Comparing `PyNN-0.9.5/pyNN/nemo/recording.py` & `PyNN-0.9.6/pyNN/nemo/recording.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import numpy
 from pyNN import recording
 from pyNN.nemo import simulator
 import logging
@@ -13,67 +13,67 @@
 
 # --- For implementation of record_X()/get_X()/print_X() -----------------------
 
 
 class Recorder(recording.Recorder):
     """Encapsulates data and functions related to recording model variables."""
     _simulator = simulator
-  
+
     def __init__(self, variable, population=None, file=None):
         __doc__ = recording.Recorder.__doc__
         recording.Recorder.__init__(self, variable, population, file)
         self._simulator.recorder_list.append(self)
         if self.variable is "spikes":
             self.data = numpy.empty([0, 2])
         elif self.variable is "v":
             self.data = numpy.empty([0, 3])
         elif self.variable is "gsyn":
             self.data = numpy.empty([0, 4])
         else:
-            raise Exception("Nemo can record only v and spikes for now !")    
+            raise Exception("Nemo can record only v and spikes for now !")
 
     def write(self, file=None, gather=False, compatible_output=True, filter=None):
         recording.Recorder.write(self, file, gather, compatible_output, filter)
 
     def record(self, ids):
         """Add the cells in `ids` to the set of recorded cells."""
         self.recorded = self.recorded.union(ids)
-        
+
     def _reset(self):
         raise NotImplementedError("Recording reset is not currently supported for pyNN.nemo")
 
     def _add_spike(self, fired, time):
         ids = self.recorded.intersection(fired)
-        self.data = numpy.vstack((self.data, numpy.array([list(ids), [time] * len(ids)]).T)) 
+        self.data = numpy.vstack((self.data, numpy.array([list(ids), [time] * len(ids)]).T))
         #  To file or memory?
 
     def _add_vm(self, time):
-        data = self._simulator.state.sim.get_membrane_potential(list(self.recorded))   
+        data = self._simulator.state.sim.get_membrane_potential(list(self.recorded))
         self.data = numpy.vstack((self.data, numpy.array([list(self.recorded), [time] * len(self.recorded), data]).T))
 
     def _add_gsyn(self, time):
         ge = self._simulator.state.sim.get_neuron_state(list(self.recorded), 1)
-        gi = self._simulator.state.sim.get_neuron_state(list(self.recorded), 2) 
+        gi = self._simulator.state.sim.get_neuron_state(list(self.recorded), 2)
         self.data = numpy.vstack((self.data, numpy.array([list(self.recorded), [time] * len(self.recorded), ge, gi]).T))
 
     def _get(self, gather=False, compatible_output=True, filter=None):
         """Return the recorded data as a Numpy array."""
         filtered_ids = self.filter_recorded(filter)
         if len(self.data) > 0:
-            mask = reduce(numpy.add, (self.data[:, 0] == id for id in filtered_ids))                            
+            mask = reduce(numpy.add, (self.data[:, 0] == id for id in filtered_ids))
             data = self.data[mask]
             return data
         else:
             return self.data
 
     def _local_count(self, filter=None):
         N = {}
         filtered_ids = self.filter_recorded(filter)
         cells = list(filtered_ids)
-        filtered_ids = numpy.array(cells)   
+        filtered_ids = numpy.array(cells)
         for id in filtered_ids:
             N[id] = 0
         spikes = self._get(gather=False, compatible_output=False, filter=filter)
         ids = numpy.sort(spikes[:, 0].astype(int))
         idx = numpy.unique(ids)
         left = numpy.searchsorted(ids, idx, 'left')
         right = numpy.searchsorted(ids, idx, 'right')
```

### Comparing `PyNN-0.9.5/pyNN/nemo/simulator.py` & `PyNN-0.9.6/pyNN/nemo/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     run()
 
 Classes:
     ID
     Recorder
     ConnectionManager
     Connection
-    
+
 Attributes:
     state -- a singleton instance of the _State class.
     recorder_list
 
 All other functions and classes are private, and should not be used by other
 modules.
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
 import nemo
 import numpy
@@ -42,19 +42,19 @@
 logger = logging.getLogger("PyNN")
 
 # --- For implementation of get_time_step() and similar functions --------------
 
 
 class _State(object):
     """Represent the simulator state."""
-    
+
     def __init__(self, timestep, min_delay, max_delay):
         """Initialize the simulator."""
         self.net = nemo.Network()
-        self.conf = nemo.Configuration()	
+        self.conf = nemo.Configuration()
         self.initialized = True
         self.num_processes = 1
         self.mpi_rank = 0
         self.min_delay = min_delay
         self.max_delay = max_delay
         self.gid = 0
         self.dt = timestep
@@ -63,137 +63,137 @@
         self.time = 0
         self._fired = []
 
     @property
     def sim(self):
         if self.simulation is None:
             raise Exception("Simulation object is empty, run() needs to be called first")
-        else: 
+        else:
             return self.simulation
-        
+
     @property
     def t(self):
         return self.time
 
     def set_stdp(self, stdp):
         self.stdp = stdp
         pre = self.stdp.timing_dependence.pre_fire(self.dt)
         post = self.stdp.timing_dependence.pre_fire(self.dt)
         pre *= self.stdp.weight_dependence.parameters['A_plus']
-        post *= -self.stdp.weight_dependence.parameters['A_minus']        
+        post *= -self.stdp.weight_dependence.parameters['A_minus']
         w_min = self.stdp.weight_dependence.parameters['w_min']
-        w_max = self.stdp.weight_dependence.parameters['w_max'] 
+        w_max = self.stdp.weight_dependence.parameters['w_max']
         self.conf.set_stdp_function(pre.tolist(), post.tolist(), float(w_min), float(w_max))
 
     def run(self, simtime):
-        
+
         if self.simulation is None:
             self.simulation = nemo.Simulation(self.net, self.conf)
 
         arrays_sources = []
 
         for source in spikes_array_list:
             if isinstance(source.celltype, SpikeSourceArray):
                 arrays_sources.append(source)
-        
+
         for t in numpy.arange(self.time, self.time + simtime, self.dt):
             spikes = []
             currents = []
             for source in arrays_sources:
                 if source.player.next_spike == t:
-                    source.player.update()                    
+                    source.player.update()
                     spikes += [source]
             for recorder in recorder_list:
                 if recorder.variable is "spikes":
                     recorder._add_spike(self._fired, self.t)
                 if recorder.variable is "v":
                     recorder._add_vm(self.t)
                 if recorder.variable is "gsyn":
                     recorder._add_gsyn(self.t)
 
             self._fired = self.sim.step(spikes, currents)
             self.time += self.dt
-        
+
             if self.stdp:
                 self.simulation.apply_stdp(self.dt)
-               
+
     @property
-    def next_id(self):        
+    def next_id(self):
         res = self.gid
         self.gid += 1
         return res
-        
+
 
 def reset():
     """Reset the state of the current network to time t = 0."""
     state.time = 0
     state._fired = []
-    
+
 # --- For implementation of access to individual neurons' parameters -----------
-    
+
 
 class ID(int, common.IDMixin):
     __doc__ = common.IDMixin.__doc__
 
     def __init__(self, n):
         int.__init__(n)
         common.IDMixin.__init__(self)
-    
+
     def get_native_parameters(self):
         if isinstance(self.celltype, SpikeSourceArray):
             return {'spike_times': self.player.spike_times}
         else:
             params = {}
             for key, value in self.celltype.indices.items():
                 if state.simulation is None:
-                    params[key] = state.net.get_neuron_parameter(self, value) 
+                    params[key] = state.net.get_neuron_parameter(self, value)
                 else:
                     params[key] = state.sim.get_neuron_parameter(self, value)
             return params
 
     def set_native_parameters(self, parameters):
         if isinstance(self.celltype, SpikeSourceArray):
             parameters['precision'] = state.dt
             self.player.reset(**parameters)
         else:
             indices = self.celltype.indices
             for key, value in parameters.items():
                 if state.simulation is None:
-                    state.net.set_neuron_parameter(self, indices[key], value) 
+                    state.net.set_neuron_parameter(self, indices[key], value)
                 else:
                     state.sim.set_neuron_parameter(self, indices[key], value)
-            
+
     def set_initial_value(self, variable, value):
         indices = self.celltype.initial_indices
         if state.simulation is None:
-            state.net.set_neuron_state(self, indices[variable], value) 
+            state.net.set_neuron_state(self, indices[variable], value)
         else:
             state.sim.set_neuron_state(self, indices[variable], value)
-            
+
     def get_initial_value(self, variable):
         index = self.celltype.initial_indices[variable]
         if state.simulation is None:
-            return state.net.get_neuron_state(self, index) 
+            return state.net.get_neuron_state(self, index)
         else:
             return state.sim.get_neuron_state(self, index)
 
 
 class Connection(object):
     """
     Provide an interface that allows access to the connection's weight, delay
     and other attributes.
     """
-    
+
     def __init__(self, synapse):
         """
         Create a new connection.
-        
+
         """
         # the index is the nth non-zero element
-        self.synapse = synapse 
+        self.synapse = synapse
 
     @property
     def target(self):
         return state.sim.get_synapse_target([self.synapse])[0]
 
     @property
     def source(self):
@@ -206,16 +206,16 @@
         return state.sim.get_synapse_weight([self.synapse])[0]
 
     def _set_delay(self, d):
         pass
 
     def _get_delay(self):
         return state.sim.get_synapse_delay([self.synapse])[0]
-        
+
     weight = property(_get_weight, _set_weight)
     delay = property(_get_delay, _set_delay)
-       
+
 
 # --- Initialization, and module attributes ------------------------------------
 
 state = None  # a Singleton, so only a single instance ever exists
 #del _State
```

### Comparing `PyNN-0.9.5/pyNN/nemo/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/nemo/standardmodels/cells.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Standard cells for the nemo module
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from pyNN.standardmodels import cells, build_translations, ModelNotAvailable, StandardCellType
 from pyNN import errors
 import numpy
 
 
 class Izhikevich(cells.Izhikevich):
-    
-    __doc__ = cells.Izhikevich.__doc__ 
+
+    __doc__ = cells.Izhikevich.__doc__
 
     translations = build_translations(
         ('a',    'a'),
         ('b',    'b'),
         ('v_reset', 'c'),
         ('d',    'd'),
         ('tau_refrac', 'tau_refrac')
@@ -27,83 +27,83 @@
     nemo_name = "Izhikevich"
 
     indices = {'a': 0, 'b': 1, 'c': 2, 'd': 3}
     initial_indices = {'u': 0, 'v': 1}
 
 
 class SpikeSourcePoisson(cells.SpikeSourcePoisson):
-    
-    __doc__ = cells.SpikeSourcePoisson.__doc__ 
+
+    __doc__ = cells.SpikeSourcePoisson.__doc__
 
     translations = build_translations(
         ('rate', 'rate', 0.001),
         ('start', 'start'),
         ('duration', 'duration')
     )
 
     nemo_name = "PoissonSource"
 
     indices = {'rate': 0}
 
 
 class SpikeSourceArray(cells.SpikeSourceArray):
 
-    __doc__ = cells.SpikeSourceArray.__doc__    
+    __doc__ = cells.SpikeSourceArray.__doc__
 
     translations = build_translations(
         ('spike_times', 'spike_times'),
     )
     nemo_name = "Input"
 
     class spike_player(object):
-        
+
         def __init__(self, spike_times=[], precision=1):
-            self.spike_times = precision * numpy.round(spike_times / precision)        
+            self.spike_times = precision * numpy.round(spike_times / precision)
             self.spike_times = numpy.unique(numpy.sort(self.spike_times))
             self.cursor = 0
             self.N = len(self.spike_times)
 
         @property
         def next_spike(self):
             if self.cursor < self.N:
                 return self.spike_times[self.cursor]
             else:
                 return numpy.inf
-        
+
         def update(self):
             self.cursor += 1
 
         def reset(self, spike_times, precision):
             self.spike_times = precision * numpy.round(spike_times / precision)
             self.spike_times = numpy.unique(numpy.sort(self.spike_times))
             self.N = len(self.spike_times)
             self.cursor = 0
 
     def __init__(self, parameters):
-        cells.SpikeSourceArray.__init__(self, parameters)        
+        cells.SpikeSourceArray.__init__(self, parameters)
 
 
 class IF_cond_exp_gsfa_grr(ModelNotAvailable):
     pass
 
 
 class IF_curr_alpha(cells.IF_curr_alpha):
-    
-    __doc__ = cells.IF_curr_alpha.__doc__    
+
+    __doc__ = cells.IF_curr_alpha.__doc__
 
     translations = build_translations(
         ('v_rest',     'v_rest'),
         ('v_reset',    'v_reset'),
-        ('cm',         'cm'), 
+        ('cm',         'cm'),
         ('tau_m',      'tau_m'),
         ('tau_refrac', 't_refrac'),
         ('tau_syn_E',  'tau_syn_E'),
         ('tau_syn_I',  'tau_syn_I'),
         ('v_thresh',   'v_thresh'),
-        ('i_offset',   'i_offset'), 
+        ('i_offset',   'i_offset'),
     )
 
     indices = {
             'v_rest': 0,
             'cm': 2,
             'tau_m': 3,
             't_refrac': 4,
@@ -115,27 +115,27 @@
         }
 
     initial_indices = {'v': 0, 'ie': 1, 'ii': 2}
     nemo_name = "IF_curr_alpha"
 
 
 class IF_curr_exp(cells.IF_curr_exp):
-    
-    __doc__ = cells.IF_curr_exp.__doc__    
+
+    __doc__ = cells.IF_curr_exp.__doc__
 
     translations = build_translations(
         ('v_rest',     'v_rest'),
         ('v_reset',    'v_reset'),
-        ('cm',         'cm'), 
+        ('cm',         'cm'),
         ('tau_m',      'tau_m'),
         ('tau_refrac', 't_refrac'),
         ('tau_syn_E',  'tau_syn_E'),
         ('tau_syn_I',  'tau_syn_I'),
         ('v_thresh',   'v_thresh'),
-        ('i_offset',   'i_offset'), 
+        ('i_offset',   'i_offset'),
     )
 
     indices = {
             'v_rest': 0,
             'cm': 2,
             'tau_m': 3,
             't_refrac': 4,
@@ -148,26 +148,26 @@
 
     initial_indices = {'v': 0, 'ie': 1, 'ii': 2}
     nemo_name = "IF_curr_exp"
 
 
 class IF_cond_alpha(cells.IF_cond_alpha):
 
-    __doc__ = cells.IF_cond_alpha.__doc__    
+    __doc__ = cells.IF_cond_alpha.__doc__
 
     translations = build_translations(
         ('v_rest',     'v_rest'),
         ('v_reset',    'v_reset'),
-        ('cm',         'cm'), 
+        ('cm',         'cm'),
         ('tau_m',      'tau_m'),
         ('tau_refrac', 't_refrac'),
         ('tau_syn_E',  'tau_syn_E'),
         ('tau_syn_I',  'tau_syn_I'),
         ('v_thresh',   'v_thresh'),
-        ('i_offset',   'i_offset'), 
+        ('i_offset',   'i_offset'),
         ('e_rev_E',    'e_rev_E'),
         ('e_rev_I',    'e_rev_I')
     )
 
     indices = {
             'v_rest': 0,
             'cm': 2,
@@ -183,27 +183,27 @@
         }
 
     initial_indices = {'v': 0, 'ie': 1, 'ii': 2}
     nemo_name = "IF_cond_alpha"
 
 
 class IF_cond_exp(cells.IF_cond_exp):
-    
-    __doc__ = cells.IF_cond_exp.__doc__    
+
+    __doc__ = cells.IF_cond_exp.__doc__
 
     translations = build_translations(
         ('v_rest',     'v_rest'),
         ('v_reset',    'v_reset'),
-        ('cm',         'cm'), 
+        ('cm',         'cm'),
         ('tau_m',      'tau_m'),
         ('tau_refrac', 't_refrac'),
         ('tau_syn_E',  'tau_syn_E'),
         ('tau_syn_I',  'tau_syn_I'),
         ('v_thresh',   'v_thresh'),
-        ('i_offset',   'i_offset'), 
+        ('i_offset',   'i_offset'),
         ('e_rev_E',    'e_rev_E'),
         ('e_rev_I',    'e_rev_I')
     )
 
     indices = {
             'v_rest': 0,
             'cm': 2,
@@ -227,15 +227,15 @@
 
 
 class EIF_cond_alpha_isfa_ista(ModelNotAvailable):
     pass
 
 
 class EIF_cond_exp_isfa_ista(ModelNotAvailable):
-    pass    
+    pass
 
 
 class HH_cond_exp(ModelNotAvailable):
     pass
 
 
 class SpikeSourceInhGamma(ModelNotAvailable):
```

### Comparing `PyNN-0.9.5/pyNN/nemo/standardmodels/electrodes.py` & `PyNN-0.9.6/pyNN/nemo/standardmodels/electrodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Classes:
     DCSource           -- a single pulse of current of constant amplitude.
     StepCurrentSource  -- a step-wise time-varying current.
     NoisyCurrentSource -- a Gaussian whitish noise current.
     ACSource           -- a sine modulated current.
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 from pyNN.standardmodels import electrodes, build_translations, StandardCurrentSource, ModelNotAvailable
 from pyNN.random import NumpyRNG, NativeRNG
@@ -20,38 +20,37 @@
 
 # should really use the StandardModel machinery to allow reverse translations
 
 
 class NemoCurrentSource(StandardCurrentSource):
     """Base class for a nest source of current to be injected into a neuron."""
 
-    def __init__(self, parameters):    
+    def __init__(self, parameters):
         super(StandardCurrentSource, self).__init__(parameters)
         self.set_native_parameters(parameters)
 
     def inject_into(self, cell_list):
         pass
 
     def set_native_parameters(self, parameters):
         parameters = self.translate(parameters)
         for key, value in parameters.items():
             self.parameters[key] = value
 
-    def get_native_parameters(self):    
+    def get_native_parameters(self):
         return self.parameters
-    
+
 
 class DCSource(ModelNotAvailable):
     pass
-    
+
 
 class ACSource(ModelNotAvailable):
     pass
 
 
 class StepCurrentSource(ModelNotAvailable):
     pass
 
 
 class NoisyCurrentSource(ModelNotAvailable):
     pass
-
```

### Comparing `PyNN-0.9.5/pyNN/nemo/standardmodels/synapses.py` & `PyNN-0.9.6/pyNN/nemo/standardmodels/synapses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 """
 Synapse Dynamics classes for the nemo module.
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 from pyNN.standardmodels import synapses, SynapseDynamics, STDPMechanism
 
 
 class STDPMechanism(STDPMechanism):
     """Specification of STDP models."""
-    
+
     def __init__(self, timing_dependence=None, weight_dependence=None,
                  voltage_dependence=None, dendritic_delay_fraction=0.0):
         assert dendritic_delay_fraction == 0, """Nemo does not currently support dendritic delays:
                                                  for the purpose of STDP calculations all delays
                                                  are assumed to be axonal."""
         super(STDPMechanism, self).__init__(timing_dependence, weight_dependence,
                                             voltage_dependence, dendritic_delay_fraction)
 
 
 class AdditiveWeightDependence(synapses.AdditiveWeightDependence):
-    
+
     __doc__ = synapses.AdditiveWeightDependence.__doc__
-    
+
     def __init__(self, w_min=0.0, w_max=1.0, A_plus=0.01, A_minus=0.01):  # units?
         parameters = dict(locals())
         parameters.pop('self')
         self.parameters = parameters
         self.parameters['mu_plus'] = 0.
         self.parameters['mu_minus'] = 0.
 
 
 class SpikePairRule(synapses.SpikePairRule):
 
-    __doc__ = synapses.SpikePairRule.__doc__    
+    __doc__ = synapses.SpikePairRule.__doc__
 
     def __init__(self, tau_plus=20.0, tau_minus=20.0):
         parameters = dict(locals())
         parameters.pop('self')
         self.parameters = parameters
 
     def pre_fire(self, precision=1.):
         return numpy.exp(-numpy.arange(0., 30, precision) / self.parameters['tau_plus'])
 
     def post_fire(self, precision=1.):
         return numpy.exp(-numpy.arange(0., 30, precision) / self.parameters['tau_minus'])
-
```

### Comparing `PyNN-0.9.5/pyNN/nest/__init__.py` & `PyNN-0.9.6/pyNN/nest/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 NEST v2 implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import warnings
 import numpy
 try:
@@ -43,19 +43,14 @@
 from pyNN.space import Space
 from pyNN.standardmodels import StandardCellType
 from pyNN.nest.populations import Population, PopulationView, Assembly
 from pyNN.nest.projections import Projection
 
 logger = logging.getLogger("PyNN")
 
-try:
-    nest.Install('pynn_extensions')
-except nest.kernel.NESTError as err:
-    warnings.warn("Unable to install NEST extensions. Certain models may not be available.")
-
 
 # ==============================================================================
 #   Utility functions
 # ==============================================================================
 
 
 def list_standard_models():
@@ -99,15 +94,15 @@
     simulator but not by others.
 
     NEST-specific extra_params:
 
     `spike_precision`:
         should be "off_grid" (default) or "on_grid"
     `verbosity`:
-        INSERT DESCRIPTION OF POSSIBLE VALUES
+        one of: "all", "info", "deprecated", "warning", "error", "fatal"
     `recording_precision`:
         number of decimal places (OR SIGNIFICANT FIGURES?) in recorded data
     `threads`:
         number of threads to use
     `grng_seed`:
         one seed for the global random number generator of NEST
     `rng_seeds`:
```

### Comparing `PyNN-0.9.5/pyNN/nest/cells.py` & `PyNN-0.9.6/pyNN/nest/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Definition of NativeCellType class for NEST.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import warnings
 import numpy as np
 import nest
 from pyNN.models import BaseCellType
```

### Comparing `PyNN-0.9.5/pyNN/nest/connectors.py` & `PyNN-0.9.6/pyNN/nest/connectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Connection method classes for nest
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
+from warnings import warn
 import nest
 try:
     import csa
     haveCSA = True
 except ImportError:
     haveCSA = False
 from pyNN import random
@@ -24,78 +25,64 @@
                              DisplacementDependentProbabilityConnector,
                              IndexBasedProbabilityConnector,
                              SmallWorldConnector,
                              FromListConnector,
                              FromFileConnector,
                              CloneConnector,
                              ArrayConnector,
-                             FixedTotalNumberConnector)
+                             FixedTotalNumberConnector,
+                             CSAConnector as DefaultCSAConnector)
 
 from .random import NativeRNG, NEST_RDEV_TYPES
 
 
 logger = logging.getLogger("PyNN")
 
 
-if not nest.ll_api.sli_func("statusdict/have_libneurosim ::"):
-
-    print(("CSAConnector: libneurosim support not available in NEST.\n" +
-           "Falling back on PyNN's default CSAConnector.\n" +
-           "Please re-compile NEST using --with-libneurosim=PATH"))
-
-    from pyNN.connectors import CSAConnector
-
-else:
-
-    class CSAConnector(Connector):
-        """
-        Use the Connection-Set Algebra (Djurfeldt, 2012) to connect
-        cells. This is an optimized variant of CSAConnector, which
-        iterates the connection-set on the C++ level in NEST.
-
-        See Djurfeldt et al. (2014) doi:10.3389/fninf.2014.00043 for
-        more details about the new interface and a comparison between
-        this and PyNN's native CSAConnector.
-
-        Takes any of the standard :class:`Connector` optional
-        arguments and, in addition:
-
-            `cset`:
-                a connection set object.
-        """
-        parameter_names = ('cset',)
-
-        if haveCSA:
-            def __init__(self, cset, safe=True, callback=None):
-                """
-                """
-                Connector.__init__(self, safe=safe, callback=callback)
-                self.cset = cset
-                arity = csa.arity(cset)
-                assert arity in (0, 2), 'must specify mask or connection-set with arity 0 or 2'
+class CSAConnector(DefaultCSAConnector):
+    """
+    Use the Connection-Set Algebra (Djurfeldt, 2012) to connect
+    cells. This is an optimized variant of CSAConnector, which
+    iterates the connection-set on the C++ level in NEST.
+
+    See Djurfeldt et al. (2014) doi:10.3389/fninf.2014.00043 for
+    more details about the new interface and a comparison between
+    this and PyNN's native CSAConnector.
+
+    Takes any of the standard :class:`Connector` optional
+    arguments and, in addition:
+
+        `cset`:
+            a connection set object.
+    """
+
+    def connect(self, projection):
+        if nest.ll_api.sli_func("statusdict/have_libneurosim ::"):
+            return self.cg_connect(projection)
         else:
-            def __init__(self, cset, safe=True, callback=None):
-                raise RuntimeError("CSAConnector not available---couldn't import csa module")
-
-        def connect(self, projection):
-            """Connect-up a Projection."""
-
-            presynaptic_cells = projection.pre.all_cells.astype('int64')
-            postsynaptic_cells = projection.post.all_cells.astype('int64')
-
-            if csa.arity(self.cset) == 2:
-                param_map = {'weight': 0, 'delay': 1}
-                nest.CGConnect(presynaptic_cells, postsynaptic_cells, self.cset,
-                               param_map, projection.nest_synapse_model)
-            else:
-                nest.CGConnect(presynaptic_cells, postsynaptic_cells, self.cset,
-                               model=projection.nest_synapse_model)
+            warn("Note: using the default CSAConnector. To use the accelerated version for NEST,\n"
+                    "Please re-compile NEST using --with-libneurosim=PATH")
+            return super(CSAConnector, self).connect(projection)
+
+    def cg_connect(self, projection):
+        """Connect-up a Projection using the Connection Generator interface"""
+
+        presynaptic_cells = projection.pre.all_cells.astype('int64')
+        postsynaptic_cells = projection.post.all_cells.astype('int64')
+
+        if csa.arity(self.cset) == 2:
+            param_map = {'weight': 0, 'delay': 1}
+            nest.CGConnect(presynaptic_cells, postsynaptic_cells, self.cset,
+                            param_map, projection.nest_synapse_model)
+        else:
+            nest.CGConnect(presynaptic_cells, postsynaptic_cells, self.cset,
+                            model=projection.nest_synapse_model)
 
-            projection._connections = None  # reset the caching of the connection list, since this will have to be recalculated
-            projection._sources.extend(presynaptic_cells)
+        projection._connections = None  # reset the caching of the connection list, since this will have to be recalculated
+        projection._sources.extend(presynaptic_cells)
 
 
 class NESTConnectorMixin(object):
 
     def synapse_parameters(self, projection):
         params = {'model': projection.nest_synapse_model}
         parameter_space = self._parameters_from_synapse_type(projection, distance_map=None)
```

### Comparing `PyNN-0.9.5/pyNN/nest/conversion.py` & `PyNN-0.9.6/pyNN/nest/conversion.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nest/electrodes.py` & `PyNN-0.9.6/pyNN/nest/electrodes.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nest/extensions/CMakeLists.txt` & `PyNN-0.9.6/pyNN/nest/extensions/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# :copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+# :copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 # :license: CeCILL, see LICENSE for details.
 
 cmake_minimum_required( VERSION 2.8.12 )
 
 # This CMakeLists.txt is configured to build your external module for NEST.
 #
-# The configuration requires a compiled and installed NEST; if `nest-config` is 
+# The configuration requires a compiled and installed NEST; if `nest-config` is
 # not in the PATH, please specify the absolute path with `-Dwith-nest=...`.
 #
 # For more informations on how to extend and use your module see:
 #           https://nest.github.io/nest-simulator/extension_modules
 
 # 1) Name your module here, i.e. add later with -Dexternal-modules=my:
 set( SHORT_NAME pynn )
```

### Comparing `PyNN-0.9.5/pyNN/nest/extensions/pynn_extensions.cpp` & `PyNN-0.9.6/pyNN/nest/extensions/pynn_extensions.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 */
 
 #include "pynn_extensions.h"
 
 // Generated includes:
@@ -20,14 +20,16 @@
 #include "connector_model_impl.h"
 #include "dynamicloader.h"
 #include "exceptions.h"
 #include "genericmodel.h"
 #include "kernel_manager.h"
 #include "model.h"
 #include "model_manager_impl.h"
+#include "nest.h"
+#include "nest_impl.h"
 #include "nestmodule.h"
 #include "target_identifier.h"
 
 // Includes from sli:
 #include "booldatum.h"
 #include "integerdatum.h"
 #include "sliexceptions.h"
@@ -106,15 +108,11 @@
          - nest::TargetIdentifierPtrRport
          - nest::TargetIdentifierIndex
      The first is the standard and you should usually stick to it.
      nest::TargetIdentifierIndex reduces the memory requirement of synapses
      even further, but limits the number of available rports. Please see
      Kunkel et al, Front Neurofinfom 8:78 (2014), Sec 3.3.2, for details.
   */
-  nest::kernel()
-    .model_manager.register_connection_model< SimpleStochasticConnection< nest::
-        TargetIdentifierPtrRport > >( "simple_stochastic_synapse" );
-  nest::kernel()
-    .model_manager.register_connection_model< StochasticStpConnection< nest::
-        TargetIdentifierPtrRport > >( "stochastic_stp_synapse" );
+  nest::register_connection_model< SimpleStochasticConnection >( "simple_stochastic_synapse" );
+  nest::register_connection_model< StochasticStpConnection >( "stochastic_stp_synapse" );
 
 } // PyNNExtensions::init()
```

### Comparing `PyNN-0.9.5/pyNN/nest/extensions/pynn_extensions.h` & `PyNN-0.9.6/pyNN/nest/extensions/pynn_extensions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 */
 
 #ifndef PYNNEXTENSIONS_H
 #define PYNNEXTENSIONS_H
```

### Comparing `PyNN-0.9.5/pyNN/nest/extensions/simple_stochastic_connection.h` & `PyNN-0.9.6/pyNN/nest/extensions/simple_stochastic_connection.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- *  :copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+ *  :copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
  *  :license: CeCILL, see LICENSE for details.
  *
  */
 
 #ifndef SIMPLE_STOCHASTIC_CONNECTION_H
 #define SIMPLE_STOCHASTIC_CONNECTION_H
```

### Comparing `PyNN-0.9.5/pyNN/nest/extensions/stochastic_stp_connection.h` & `PyNN-0.9.6/pyNN/nest/extensions/stochastic_stp_connection.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  *  stochastic_stp_connection.h
  *
- *  :copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+ *  :copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
  *  :license: CeCILL, see LICENSE for details.
  *
  */
 
 #ifndef STOCHASTIC_STP_CONNECTION_H
 #define STOCHASTIC_STP_CONNECTION_H
```

### Comparing `PyNN-0.9.5/pyNN/nest/extensions/stochastic_stp_connection_impl.h` & `PyNN-0.9.6/pyNN/nest/extensions/stochastic_stp_connection_impl.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  *  stochastic_stp_connection_impl.h
  *
- *  :copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+ *  :copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
  *  :license: CeCILL, see LICENSE for details.
  *
  */
 
 #ifndef STOCHASTIC_STP_CONNECTION_IMPL_H
 #define STOCHASTIC_STP_CONNECTION_IMPL_H
```

### Comparing `PyNN-0.9.5/pyNN/nest/nineml.py` & `PyNN-0.9.6/pyNN/nest/nineml.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Functions:
     nineml_cell_type_from_model - return a new NineMLCellType subclass
 
 Constants:
     NEST_DIR        - subdirectory to which NEST mechanisms will be written (TODO: not implemented)
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from __future__ import absolute_import  # Not compatible with Python 2.4
 import logging
 from pyNN.nest.cells import NativeCellType
@@ -27,51 +27,51 @@
 # TODO: This should go to a evironment variable, like PYNN_9ML_DIR
 # and then a sub-dir for nest, neuron, etc.
 # but default to ~/.pyNN or something to that regard.
 NEST_DIR = "nest_models"
 
 
 class NineMLCellType(NativeCellType):
-    
+
     def __init__(self, parameters):
         NativeCellType.__init__(self, parameters)
 
 
 def nineml_celltype_from_model(name, nineml_model, synapse_components):
     """
     Return a new NineMLCellType subclass from a NineML model.
     """
-    
+
     dct = {'nineml_model': nineml_model,
            'synapse_components': synapse_components}
     return _nest_build_nineml_celltype(name, (NineMLCellType,), dct)
 
 
 class _nest_build_nineml_celltype(type):
     """
     Metaclass for building NineMLCellType subclasses
     Called by nineml_celltype_from_model
     """
     def __new__(cls, name, bases, dct):
-        
+
         import nineml.abstraction as al
         from nineml.abstraction import flattening, writers, component_modifiers
         import nest
 
         # Extract Parameters Back out from Dict:
         nineml_model = dct['nineml_model']
         synapse_components = dct['synapse_components']
 
         # Flatten the model:
         assert isinstance(nineml_model, al.ComponentClass)
         if nineml_model.is_flat():
             flat_component = nineml_model
         else:
             flat_component = flattening.flatten(nineml_model, name)
-        
+
         # Make the substitutions:
         flat_component.backsub_all()
         #flat_component.backsub_aliases()
         #flat_component.backsub_equations()
 
         # Close any open reduce ports:
         component_modifiers.ComponentModifier.close_all_reduce_ports(component=flat_component)
@@ -97,29 +97,29 @@
 
         # New:
         dct["combined_model"] = flat_component
         # TODO: Override this with user layer
         #default_values = ModelToSingleComponentReducer.flatten_namespace_dict( parameters )
         dct["default_parameters"] = dict((p.name, 1.0) for p in flat_component.parameters)
         dct["default_initial_values"] = dict((s.name, 0.0) for s in flat_component.state_variables)
-        dct["synapse_types"] = [syn.namespace for syn in synapse_components] 
+        dct["synapse_types"] = [syn.namespace for syn in synapse_components]
         dct["standard_receptor_type"] = (dct["synapse_types"] == ('excitatory', 'inhibitory'))
         dct["injectable"] = True  # need to determine this. How??
         dct["conductance_based"] = True  # how to determine this??
         dct["model_name"] = name
         dct["nest_model"] = name
 
         # Recording from bindings:
         dct["recordable"] = [port.name for port in flat_component.analog_ports] + ['spikes', 'regime']
         # TODO bindings -> alias and support recording of them in nest template
         #+ [binding.name for binding in flat_component.bindings]
-        
+
         dct["weight_variables"] = dict([(syn.namespace, syn.namespace + '_' + syn.weight_connector)
                                         for syn in synapse_components])
-        
+
         logger.debug("Creating class '%s' with bases %s and dictionary %s" % (name, bases, dct))
 
         # TODO: UL configuration of initial regime.
         initial_regime = flat_component.regimes_map.keys()[0]
 
         from nestbuilder import NestFileBuilder
         nfb = NestFileBuilder(nest_classname=name,
@@ -127,9 +127,9 @@
                               synapse_ports=synapse_ports,
                               initial_regime=initial_regime,
                               initial_values=dct["default_initial_values"],
                               default_values=dct["default_parameters"],
                               )
         nfb.compile_files()
         nest.Install('mymodule')
-        
+
         return type.__new__(cls, name, bases, dct)
```

### Comparing `PyNN-0.9.5/pyNN/nest/populations.py` & `PyNN-0.9.6/pyNN/nest/populations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 NEST v2 implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 import nest
 import logging
```

### Comparing `PyNN-0.9.5/pyNN/nest/projections.py` & `PyNN-0.9.6/pyNN/nest/projections.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 """
 NEST v2 implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 import nest
 import logging
 from itertools import repeat
 try:
     xrange
 except NameError:  # Python 3
     xrange = range
 from pyNN import common, errors
 from pyNN.space import Space
+from pyNN.parameters import simplify
 from . import simulator
 from pyNN.random import RandomDistribution
 from .standardmodels.synapses import StaticSynapse
 from .conversion import make_sli_compatible
 
 logger = logging.getLogger("PyNN")
 
@@ -45,17 +46,15 @@
                                    connector, synapse_type, source, receptor_type,
                                    space, label)
         self.nest_synapse_model = self.synapse_type._get_nest_synapse_model()
         self.nest_synapse_label = Projection._nProj
         self.synapse_type._set_tau_minus(self.post.local_cells)
         self._sources = []
         self._connections = None
-        # This is used to keep track of common synapse properties (to my
-        # knowledge they only become apparent once connections are created
-        # within nest --obreitwi, 13-02-14)
+        # This is used to keep track of common synapse properties
         self._common_synapse_properties = {}
         self._common_synapse_property_names = None
 
         # Create connections
         connector.connect(self)
 
     def __getitem__(self, i):
@@ -69,32 +68,31 @@
             if i.stop < len(self):
                 return [simulator.Connection(self, j) for j in range(i.start, i.stop, i.step or 1)]
             else:
                 raise IndexError("%d > %d" % (i.stop, len(self) - 1))
 
     def __len__(self):
         """Return the number of connections on the local MPI node."""
-        #Disabling the following method pending resolution of https://github.com/nest/nest-simulator/issues/1085
-        #local_nodes = nest.GetNodes([0], local_only=True)[0]
-        #local_connections = nest.GetConnections(target=local_nodes,
-        #                                        synapse_model=self.nest_synapse_model,
-        #                                        synapse_label=self.nest_synapse_label)
-        local_connections = self.nest_connections
+        local_nodes = nest.GetNodes([0], local_only=True)[0]
+        local_connections = nest.GetConnections(target=local_nodes,
+                                                synapse_model=self.nest_synapse_model,
+                                                synapse_label=self.nest_synapse_label)
         return len(local_connections)
 
     @property
     def nest_connections(self):
-        if self._connections is None:
+        if self._connections is None or self._simulator.state.stale_connection_cache:
             self._sources = numpy.unique(self._sources)
             if self._sources.size > 0:
                 self._connections = nest.GetConnections(self._sources.tolist(),
                                                         synapse_model=self.nest_synapse_model,
                                                         synapse_label=self.nest_synapse_label)
             else:
                 self._connections = []
+            self._simulator.state.stale_connection_cache = False
         return self._connections
 
     @property
     def connections(self):
         """
         Returns an iterator over local connections in this projection, as `Connection` objects.
         """
@@ -115,141 +113,179 @@
             syn_params.update({'tau_psc': nest.GetStatus([self.nest_connections[0,1]], param_name)})
 
 
         syn_params.update({'synapse_label': self.nest_synapse_label})
         nest.Connect(self.pre.all_cells.astype(int).tolist(),
                      self.post.all_cells.astype(int).tolist(),
                      rule_params, syn_params)
+        self._simulator.state.stale_connection_cache = True
         self._sources = [cid[0] for cid in nest.GetConnections(synapse_model=self.nest_synapse_model,
                                                                synapse_label=self.nest_synapse_label)]
 
+    def _identify_common_synapse_properties(self):
+        """
+        Use the connection between the sample indices to distinguish
+        between local and common synapse properties.
+        """
+        sample_connection = nest.GetConnections(source=[int(self._sources[0])],
+                                                synapse_model=self.nest_synapse_model,
+                                                synapse_label=self.nest_synapse_label)[:1]
+
+        local_parameters = nest.GetStatus(sample_connection)[0].keys()
+        all_parameters = nest.GetDefaults(self.nest_synapse_model).keys()
+        self._common_synapse_property_names = [name for name in all_parameters
+                                               if name not in local_parameters]
+
+    def _update_syn_params(self, syn_dict, connection_parameters):
+        """
+        Update the paramaters to be passed in the nest.Connect method with the connection
+        parameters specific to the synapse type.
+
+        `syn_dict` - the dictionary to be passed to nest.Connect containing "local" parameters
+        `connection_parameters` - a dictionary containing all parameters (local and common)
+        """
+        # Set connection parameters other than weight and delay
+        if connection_parameters:
+            for name, value in connection_parameters.items():
+                if name not in self._common_synapse_property_names:
+                    value = make_sli_compatible(value)
+                    if isinstance(value, numpy.ndarray):
+                        # the str() is to work around a bug handling unicode names in SetStatus in NEST 2.4.1 when using Python 2
+                        syn_dict.update({str(name):numpy.array([value.tolist()])})
+                    else:
+                        syn_dict.update({str(name):value})
+        return syn_dict
+
     def _convergent_connect(self, presynaptic_indices, postsynaptic_index,
                             **connection_parameters):
         """
         Connect a neuron to one or more other neurons with a static connection.
 
-        `sources`  -- a 1D array of pre-synaptic cell IDs
-        `target`   -- the ID of the post-synaptic cell.
-
-        TO UPDATE
+        `presynaptic_indices` - 1D array of presynaptic indices
+        `postsynaptic_index` - integer - the index of the postsynaptic neuron
+        `connection_parameters` - dict whose keys are native NEST parameter names. Values may be scalars or arrays.
         """
         #logger.debug("Connecting to index %s from %s with %s" % (postsynaptic_index, presynaptic_indices, connection_parameters))
-        presynaptic_cells = self.pre.all_cells[presynaptic_indices]
+
+        presynaptic_cells = self.pre.all_cells[presynaptic_indices].astype(int).tolist()
         postsynaptic_cell = self.post[postsynaptic_index]
-        assert presynaptic_cells.size == presynaptic_indices.size
+        postsynaptic_cell_id = [int(postsynaptic_cell)]
         assert len(presynaptic_cells) > 0, presynaptic_cells
+        self._sources.extend(presynaptic_cells)
+
         syn_dict = {
             'model': self.nest_synapse_model,
             'synapse_label': self.nest_synapse_label,
         }
 
+        # Weights require some special handling
         weights = connection_parameters.pop('weight')
         if self.receptor_type == 'inhibitory' and self.post.conductance_based:
             weights *= -1  # NEST wants negative values for inhibitory weights, even if these are conductances
             if "stdp" in self.nest_synapse_model:
                 syn_dict["Wmax"] = -1.2345e6  # just some very large negative value to avoid
                                               # NEST complaining about weight and Wmax having different signs
                                               # (see https://github.com/NeuralEnsemble/PyNN/issues/636)
                                               # Will be overwritten below.
                 connection_parameters["Wmax"] *= -1
         if hasattr(self.post, "celltype") and hasattr(self.post.celltype, "receptor_scale"):  # this is a bit of a hack
             weights *= self.post.celltype.receptor_scale                                      # needed for the Izhikevich model
+
         delays = connection_parameters.pop('delay')
 
-        # Create connections, with weights and delays
-        # Setting other connection parameters is done afterwards
-        if postsynaptic_cell.celltype.standard_receptor_type:
-            try:
-                if not numpy.isscalar(weights):
-                    weights = numpy.array([weights])
-                if not numpy.isscalar(delays):
-                    delays = numpy.array([delays])
-                syn_dict.update({'weight': weights, 'delay': delays})
+        # Clean the connection parameters by removing parameters that are
+        # used by PyNN but should not be passed to NEST
+        connection_parameters.pop('tau_minus', None)  # TODO: set tau_minus on the post-synaptic cells
+        connection_parameters.pop('dendritic_delay_fraction', None)
+        connection_parameters.pop('w_min_always_zero_in_NEST', None)
 
+        # Create connections and set parameters
+        try:
+            # nest.Connect expects a 2D array
+            if not numpy.isscalar(weights):
+                weights = numpy.array([weights])
+            if not numpy.isscalar(delays):
+                delays = numpy.array([delays])
+            syn_dict.update({'weight': weights, 'delay': delays})
+
+            if postsynaptic_cell.celltype.standard_receptor_type:
+                # For Tsodyks-Markram synapses models we set the "tau_psc" parameter to match
+                # the relevant "tau_syn" parameter from the post-synaptic neuron.
                 if 'tsodyks' in self.nest_synapse_model:
                     if self.receptor_type == 'inhibitory':
-                        param_name = self.post.local_cells[0].celltype.translations['tau_syn_I']['translated_name']
+                        param_name = postsynaptic_cell.celltype.translations['tau_syn_I']['translated_name']
                     elif self.receptor_type == 'excitatory':
-                        param_name = self.post.local_cells[0].celltype.translations['tau_syn_E']['translated_name']
+                        param_name = postsynaptic_cell.celltype.translations['tau_syn_E']['translated_name']
                     else:
                         raise NotImplementedError()
-                    syn_dict.update({'tau_psc': numpy.array([[nest.GetStatus([postsynaptic_cell], param_name)[0]] * len(presynaptic_cells.astype(int).tolist())])})
-
-                nest.Connect(presynaptic_cells.astype(int).tolist(),
-                             [int(postsynaptic_cell)],
-                             'all_to_all',
-                             syn_dict)
-            except nest.kernel.NESTError as e:
-                errmsg = "%s. presynaptic_cells=%s, postsynaptic_cell=%s, weights=%s, delays=%s, synapse model='%s'" % (
-                            e, presynaptic_cells, postsynaptic_cell,
-                            weights, delays, self.nest_synapse_model)
-                raise errors.ConnectionError(errmsg)
-        else:
-            receptor_type = postsynaptic_cell.celltype.get_receptor_type(self.receptor_type)
-            if numpy.isscalar(weights):
-                weights = repeat(weights)
-            if numpy.isscalar(delays):
-                delays = repeat(delays)
-            for pre, w, d in zip(presynaptic_cells, weights, delays):
-                syn_dict.update({'weight': w, 'delay': d, 'receptor_type': receptor_type})
-                if 'tsodyks' in self.nest_synapse_model:
-                   syn_dict.update({'tau_psc': numpy.array([[nest.GetStatus([postsynaptic_cell], param_name)[0]] * len(presynaptic_cells.astype(int).tolist())])})
-
-                nest.Connect([pre], [postsynaptic_cell], 'one_to_one', syn_dict)
-
-
-        # Book-keeping
-        self._connections = None  # reset the caching of the connection list, since this will have to be recalculated
-        self._sources.extend(presynaptic_cells)
-
-        # Clean the connection parameters
-        connection_parameters.pop('tau_minus', None)  # TODO: set tau_minus on the post-synaptic cells
-        connection_parameters.pop('dendritic_delay_fraction', None)
-        connection_parameters.pop('w_min_always_zero_in_NEST', None)
-
-        # We need to distinguish between common synapse parameters and local ones
-        # We just get the parameters of the first connection (is there an easier way?)
-        if self._common_synapse_property_names is None:
-            self._identify_common_synapse_properties()
-
-        # Set connection parameters other than weight and delay
-        if connection_parameters:
-            #logger.debug(connection_parameters)
-            sort_indices = numpy.argsort(presynaptic_cells)
-            connections = nest.GetConnections(source=numpy.unique(presynaptic_cells.astype(int)).tolist(),
-                                              target=[int(postsynaptic_cell)],
-                                              synapse_model=self.nest_synapse_model,
-                                              synapse_label=self.nest_synapse_label)
-            for name, value in connection_parameters.items():
-                if name not in self._common_synapse_property_names:
-                    value = make_sli_compatible(value)
-                    #logger.debug("Setting %s=%s for connections %s" % (name, value, connections))
-                    if isinstance(value, numpy.ndarray):
-                        # the str() is to work around a bug handling unicode names in SetStatus in NEST 2.4.1 when using Python 2
-                        nest.SetStatus(connections, str(name), value[sort_indices].tolist())
+                    syn_dict["tau_psc"] = nest.GetStatus(postsynaptic_cell_id, param_name)[0]
+            else:
+                syn_dict.update(
+                    {"receptor_type": postsynaptic_cell.celltype.get_receptor_type(
+                        self.receptor_type)})
+
+            # For parameters other than weight and delay, we need to know if they are "common"
+            # parameters (the same for all synapses) or "local" (different synapses can have
+            # different values), as this affects how they are set.
+            #
+            # To introspect which parameters are common, we need an existing connection, so
+            # the first time we create connections we pass just the weight and delay, and set
+            # the other parameters later. We then get the list of common parameters and cache
+            # it so that in subsequent Connect() calls we can pass all of the local
+            # (non-common) parameters.
+            if self._common_synapse_property_names is None:
+                nest.Connect(presynaptic_cells,
+                                postsynaptic_cell_id,
+                                'all_to_all',
+                                syn_dict)
+                self._identify_common_synapse_properties()
+
+                # Retrieve connections so that we can set additional
+                # parameters using nest.SetStatus
+                connections = nest.GetConnections(source=presynaptic_cells,
+                                                    target=postsynaptic_cell_id,
+                                                    synapse_model=self.nest_synapse_model,
+                                                    synapse_label=self.nest_synapse_label)
+                sort_indices = numpy.argsort(presynaptic_cells)  # not sure why we need to sort here
+                for name, value in connection_parameters.items():
+                    if name not in self._common_synapse_property_names:
+                        value = make_sli_compatible(value)
+                        if isinstance(value, numpy.ndarray):
+                            nest.SetStatus(connections, name, value[sort_indices].tolist())
+                        else:
+                            nest.SetStatus(connections, name, value)
                     else:
-                        nest.SetStatus(connections, str(name), value)
-                else:
-                    self._set_common_synapse_property(name, value)
+                        self._set_common_synapse_property(name, value)
+            else:
+                # Since we know which parameters are common, we can set the non-common
+                # parameters directly in the nest.Connect call
+                syn_dict = self._update_syn_params(syn_dict, connection_parameters)
+                nest.Connect(presynaptic_cells,
+                                postsynaptic_cell_id,
+                                'all_to_all',
+                                syn_dict)
+                # and then set the common parameters
+                for name, value in connection_parameters.items():
+                    if name in self._common_synapse_property_names:
+                        self._set_common_synapse_property(name, value)
 
-    def _identify_common_synapse_properties(self):
-        """
-            Use the connection between the sample indices to distinguish
-            between local and common synapse properties.
-        """
-        sample_connection = nest.GetConnections(source=[int(self._sources[0])],
-                                                synapse_model=self.nest_synapse_model,
-                                                synapse_label=self.nest_synapse_label)[:1]
+        except nest.kernel.NESTError as e:
+            errmsg = "%s. presynaptic_cells=%s, postsynaptic_cell=%s, weights=%s, delays=%s, synapse model='%s'" % (
+                        e, presynaptic_cells, postsynaptic_cell,
+                        weights, delays, self.nest_synapse_model)
+            raise errors.ConnectionError(errmsg)
 
-        local_parameters = nest.GetStatus(sample_connection)[0].keys()
-        all_parameters = nest.GetDefaults(self.nest_synapse_model).keys()
-        self._common_synapse_property_names = [name for name in all_parameters
-                                               if name not in local_parameters]
+        # Reset the caching of the connection list, since this will have to be recalculated
+        self._connections = None
+        self._simulator.state.stale_connection_cache = True
 
     def _set_attributes(self, parameter_space):
+        if "tau_minus" in parameter_space.keys() and not parameter_space["tau_minus"].is_homogeneous:
+            raise ValueError("tau_minus cannot be heterogeneous "
+                             "within a single Projection with NEST.")
         parameter_space.evaluate(mask=(slice(None), self.post._mask_local))  # only columns for connections that exist on this machine
         sources = numpy.unique(self._sources).tolist()
         if self._common_synapse_property_names is None:
             self._identify_common_synapse_properties()
         for postsynaptic_cell, connection_parameters in zip(self.post.local_cells,
                                                             parameter_space.columns()):
             connections = nest.GetConnections(source=sources,
@@ -257,15 +293,18 @@
                                               synapse_model=self.nest_synapse_model,
                                               synapse_label=self.nest_synapse_label)
             if connections:
                 source_mask = self.pre.id_to_index([x[0] for x in connections])
                 for name, value in connection_parameters.items():
                     if name == "weight" and self.receptor_type == 'inhibitory' and self.post.conductance_based:
                         value *= -1  # NEST uses negative values for inhibitory weights, even if these are conductances
-                    if name not in self._common_synapse_property_names:
+                    if name == "tau_minus":  # set on the post-synaptic cell
+                        nest.SetStatus(self.post.local_cells.astype(int).tolist(),
+                                       {"tau_minus": simplify(value)})
+                    elif name not in self._common_synapse_property_names:
                         value = make_sli_compatible(value)
                         if len(source_mask) > 1:
                             nest.SetStatus(connections, name, value[source_mask])
                         elif isinstance(value, numpy.ndarray):  # OneToOneConnector
                             nest.SetStatus(connections, name, value[source_mask])
                         else:
                             nest.SetStatus(connections, name, value)
```

### Comparing `PyNN-0.9.5/pyNN/nest/random.py` & `PyNN-0.9.6/pyNN/nest/random.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nest/recording.py` & `PyNN-0.9.6/pyNN/nest/recording.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import numpy
 import logging
 import nest
 from pyNN import recording
@@ -54,15 +54,15 @@
         scale_factor = SCALE_FACTORS.get(variable, 1)
         nest_variable = VARIABLE_MAP.get(variable, variable)
         events = nest.GetStatus(self.device, 'events')[0]
         ids = events['senders']
         values = events[nest_variable] * scale_factor  # I'm hoping numpy optimises for the case where scale_factor = 1, otherwise should avoid this multiplication in that case
         data = {}
         recorded_ids = set(ids)
-        
+
         for id in recorded_ids:
             data[id]=[]
 
         for id,v in zip(ids,values):
             data[id].append(v)
 
         desired_and_existing_ids = numpy.intersect1d(numpy.array(list(recorded_ids)),numpy.array(desired_ids))
@@ -429,22 +429,22 @@
         simulator.state.recording_devices.remove(self._multimeter)
         simulator.state.recording_devices.remove(self._spike_detector)
         # I guess the existing devices still exist in NEST, can we delete them
         # or at least turn them off?
         # Maybe we can reset them, rather than create new ones?
         self._multimeter = Multimeter()
         self._spike_detector = SpikeDetector()
-    
+
     def _get_spiketimes(self, ids):
         return self._spike_detector.get_spiketimes(ids)  # hugely inefficient - to be optimized later
-    
+
     def _get_all_signals(self, variable, ids, clear=False):
         data = self._multimeter.get_data(variable, ids, clear=clear)
         if len(ids) > 0:
-            return numpy.array([data[i] for i in ids]).T #JACOMMENT: this is very expensive but not sure how to get rid of it 
+            return numpy.array([data[i] for i in ids]).T #JACOMMENT: this is very expensive but not sure how to get rid of it
         else:
             return numpy.array([])
 
     def _local_count(self, variable, filter_ids):
         assert variable == 'spikes'
         #N = {}
         #if self._device.in_memory():
```

### Comparing `PyNN-0.9.5/pyNN/nest/simulator.py` & `PyNN-0.9.6/pyNN/nest/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Attributes:
     state -- a singleton instance of the _State class.
 
 All other functions and classes are private, and should not be used by other
 modules.
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import nest
 import logging
 import tempfile
@@ -49,25 +49,31 @@
 
 
 class _State(common.control.BaseState):
     """Represent the simulator state."""
 
     def __init__(self):
         super(_State, self).__init__()
+        try:
+            nest.Install('pynn_extensions')
+            self.extensions_loaded = True
+        except nest.kernel.NESTError as err:
+            self.extensions_loaded = False
         self.initialized = False
         self.optimize = False
         self.spike_precision = "off_grid"
-        self.verbosity = "warning"
+        self.verbosity = "error"
         self._cache_num_processes = nest.GetKernelStatus()['num_processes']  # avoids blocking if only some nodes call num_processes
                                                                              # do the same for rank?
         # allow NEST to erase previously written files (defaut with all the other simulators)
         nest.SetKernelStatus({'overwrite_files': True})
         self.tempdirs = []
         self.recording_devices = []
         self.populations = []  # needed for reset
+        self.stale_connection_cache = False
 
     @property
     def t(self):
         return max(nest.GetKernelStatus('time') - self.dt, 0.0)  # note that we always simulate one time step past the requested time
 
     dt = nest_property('resolution', float)
```

### Comparing `PyNN-0.9.5/pyNN/nest/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/nest/standardmodels/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Standard cells for nest
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from pyNN.standardmodels import cells, build_translations
 from .. import simulator
 
@@ -24,39 +24,39 @@
         ('tau_syn_I',  'tau_syn_in'),
         ('v_thresh',   'V_th'),
         ('i_offset',   'I_e',      1000.0),  # I_e is in pA, i_offset in nA
     )
     nest_name = {"on_grid": "iaf_psc_alpha",
                  "off_grid": "iaf_psc_alpha"}
     standard_receptor_type = True
-    
+
 
 class IF_curr_exp(cells.IF_curr_exp):
-    
-    __doc__ = cells.IF_curr_exp.__doc__    
-    
+
+    __doc__ = cells.IF_curr_exp.__doc__
+
     translations = build_translations(
         ('v_rest',     'E_L'),
         ('v_reset',    'V_reset'),
         ('cm',         'C_m',      1000.0),  # C_m is in pF, cm in nF
         ('tau_m',      'tau_m'),
         ('tau_refrac', 't_ref'),
         ('tau_syn_E',  'tau_syn_ex'),
         ('tau_syn_I',  'tau_syn_in'),
         ('v_thresh',   'V_th'),
         ('i_offset',   'I_e',      1000.0),  # I_e is in pA, i_offset in nA
     )
     nest_name = {"on_grid": 'iaf_psc_exp',
                  "off_grid": 'iaf_psc_exp_ps'}
     standard_receptor_type = True
-    
+
 
 class IF_cond_alpha(cells.IF_cond_alpha):
 
-    __doc__ = cells.IF_cond_alpha.__doc__    
+    __doc__ = cells.IF_cond_alpha.__doc__
 
     translations = build_translations(
         ('v_rest',     'E_L'),
         ('v_reset',    'V_reset'),
         ('cm',         'C_m',        1000.0),  # C_m is in pF, cm in nF
         ('tau_m',      'g_L',        "cm/tau_m*1000.0", "C_m/g_L"),
         ('tau_refrac', 't_ref'),
@@ -66,20 +66,20 @@
         ('i_offset',   'I_e',        1000.0),  # I_e is in pA, i_offset in nA
         ('e_rev_E',    'E_ex'),
         ('e_rev_I',    'E_in'),
     )
     nest_name = {"on_grid": "iaf_cond_alpha",
                  "off_grid": "iaf_cond_alpha"}
     standard_receptor_type = True
-        
+
 
 class IF_cond_exp(cells.IF_cond_exp):
 
-    __doc__ = cells.IF_cond_exp.__doc__    
-    
+    __doc__ = cells.IF_cond_exp.__doc__
+
     translations = build_translations(
         ('v_rest',     'E_L'),
         ('v_reset',    'V_reset'),
         ('cm',         'C_m',        1000.0),  # C_m is in pF, cm in nF
         ('tau_m',      'g_L',        "cm/tau_m*1000.0", "C_m/g_L"),
         ('tau_refrac', 't_ref'),
         ('tau_syn_E',  'tau_syn_ex'),
@@ -92,15 +92,15 @@
     nest_name = {"on_grid": "iaf_cond_exp",
                  "off_grid": "iaf_cond_exp"}
     standard_receptor_type = True
 
 
 class IF_cond_exp_gsfa_grr(cells.IF_cond_exp_gsfa_grr):
 
-    __doc__ = cells.IF_cond_exp_gsfa_grr.__doc__    
+    __doc__ = cells.IF_cond_exp_gsfa_grr.__doc__
 
     translations = build_translations(
         ('v_rest',     'E_L'),
         ('v_reset',    'V_reset'),
         ('cm',         'C_m',        1000.0),  # C_m is in pF, cm in nF
         ('tau_m',      'g_L',        "cm/tau_m*1000.0", "C_m/g_L"),
         ('tau_refrac', 't_ref'),
@@ -119,18 +119,18 @@
     )
     nest_name = {"on_grid": "iaf_cond_exp_sfa_rr",
                  "off_grid": "iaf_cond_exp_sfa_rr"}
     standard_receptor_type = True
 
 
 class IF_facets_hardware1(cells.IF_facets_hardware1):
-    
-    __doc__ = cells.IF_facets_hardware1.__doc__        
 
-    # in 'iaf_cond_exp', the dimension of C_m is pF, 
+    __doc__ = cells.IF_facets_hardware1.__doc__
+
+    # in 'iaf_cond_exp', the dimension of C_m is pF,
     # while in the pyNN context, cm is given in nF
     translations = build_translations(
         ('v_reset',    'V_reset'),
         ('v_rest',     'E_L'),
         ('v_thresh',   'V_th'),
         ('e_rev_I',    'E_in'),
         ('tau_syn_E',  'tau_syn_ex'),
@@ -144,44 +144,44 @@
         'C_m': 200.0,
         't_ref': 1.0,
         'E_ex': 0.0
     }
 
 
 class HH_cond_exp(cells.HH_cond_exp):
-    
-    __doc__ = cells.HH_cond_exp.__doc__    
-    
+
+    __doc__ = cells.HH_cond_exp.__doc__
+
     translations = build_translations(
-        ('gbar_Na',    'g_Na',  1000.0), # uS --> nS   
+        ('gbar_Na',    'g_Na',  1000.0), # uS --> nS
         ('gbar_K',     'g_K',   1000.0),
         ('g_leak',     'g_L',   1000.0),
         ('cm',         'C_m',   1000.0),  # nF --> pF
         ('v_offset',   'V_T'),
         ('e_rev_Na',   'E_Na'),
-        ('e_rev_K',    'E_K'), 
+        ('e_rev_K',    'E_K'),
         ('e_rev_leak', 'E_L'),
         ('e_rev_E',    'E_ex'),
         ('e_rev_I',    'E_in'),
         ('tau_syn_E',  'tau_syn_ex'),
         ('tau_syn_I',  'tau_syn_in'),
         ('i_offset',   'I_e',   1000.0),  # nA --> pA
     )
     nest_name = {"on_grid": "hh_cond_exp_traub",
                  "off_grid": "hh_cond_exp_traub"}
     standard_receptor_type = True
-    
-   
+
+
 class EIF_cond_alpha_isfa_ista(cells.EIF_cond_alpha_isfa_ista):
 
-    __doc__ = cells.EIF_cond_alpha_isfa_ista.__doc__ 
+    __doc__ = cells.EIF_cond_alpha_isfa_ista.__doc__
 
     translations = build_translations(
         ('cm',         'C_m',       1000.0),  # nF -> pF
-        ('tau_refrac', 't_ref'), 
+        ('tau_refrac', 't_ref'),
         ('v_spike',    'V_peak'),
         ('v_reset',    'V_reset'),
         ('v_rest',     'E_L'),
         ('tau_m',      'g_L',       "cm/tau_m*1000.0", "C_m/g_L"),
         ('i_offset',   'I_e',       1000.0),  # nA -> pA
         ('a',          'a'),
         ('b',          'b',         1000.0),  # nA -> pA.
@@ -196,15 +196,15 @@
     nest_name = {"on_grid": "aeif_cond_alpha",
                  "off_grid": "aeif_cond_alpha"}
     standard_receptor_type = True
 
 
 class SpikeSourcePoisson(cells.SpikeSourcePoisson):
 
-    __doc__ = cells.SpikeSourcePoisson.__doc__ 
+    __doc__ = cells.SpikeSourcePoisson.__doc__
 
     translations = build_translations(
         ('rate',     'rate'),
         ('start',    'start'),
         ('duration', 'stop',    "start+duration", "stop-start"),
     )
     nest_name = {"on_grid": 'poisson_generator',
@@ -260,16 +260,16 @@
     uses_parrot = True
     extra_parameters = {
         'n_proc': 1
     }
 
 
 class SpikeSourceInhGamma(cells.SpikeSourceInhGamma):
-    
-    __doc__ = cells.SpikeSourceInhGamma.__doc__ 
+
+    __doc__ = cells.SpikeSourceInhGamma.__doc__
 
     translations = build_translations(
         ('a',        'a'),
         ('b',        'b'),
         ('tbins',    'tbins'),
         ('start',    'start'),
         ('duration', 'stop',   "duration+start", "stop-start"),
@@ -313,20 +313,20 @@
     nest_name = {"on_grid": 'spike_generator',
                  "off_grid": 'spike_generator'}
     uses_parrot = True
     always_local = True
 
 
 class EIF_cond_exp_isfa_ista(cells.EIF_cond_exp_isfa_ista):
-    
+
     __doc__ = cells.EIF_cond_exp_isfa_ista.__doc__
 
     translations = build_translations(
         ('cm',         'C_m',       1000.0),  # nF -> pF
-        ('tau_refrac', 't_ref'), 
+        ('tau_refrac', 't_ref'),
         ('v_spike',    'V_peak'),
         ('v_reset',    'V_reset'),
         ('v_rest',     'E_L'),
         ('tau_m',      'g_L',       "cm/tau_m*1000.0", "C_m/g_L"),
         ('i_offset',   'I_e',       1000.0),  # nA -> pA
         ('a',          'a'),
         ('b',          'b',         1000.0),  # nA -> pA.
@@ -341,15 +341,15 @@
     nest_name = {"on_grid": "aeif_cond_exp",
                  "off_grid": "aeif_cond_exp"}
     standard_receptor_type = True
 
 
 class Izhikevich(cells.Izhikevich):
     __doc__ = cells.Izhikevich.__doc__
-    
+
     translations = build_translations(
         ('a',        'a'),
         ('b',        'b'),
         ('c',        'c'),
         ('d',        'd'),
         ('i_offset', 'I_e', 1000.0),
     )
```

### Comparing `PyNN-0.9.5/pyNN/nest/standardmodels/electrodes.py` & `PyNN-0.9.6/pyNN/nest/standardmodels/electrodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Classes:
     DCSource           -- a single pulse of current of constant amplitude.
     StepCurrentSource  -- a step-wise time-varying current.
     NoisyCurrentSource -- a Gaussian whitish noise current.
     ACSource           -- a sine modulated current.
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 import nest
 from pyNN.standardmodels import electrodes, build_translations, StandardCurrentSource
@@ -106,15 +106,15 @@
     def set_native_parameters(self, parameters):
         parameters.evaluate(simplify=True)
         for key, value in parameters.items():
             if key == "amplitude_values":
                 assert isinstance(value, Sequence)
                 step_times = parameters["amplitude_times"].value
                 step_amplitudes = parameters["amplitude_values"].value
-                
+
                 step_times, step_amplitudes = self._check_step_times(step_times, step_amplitudes, self.timestep)
                 parameters["amplitude_times"].value = step_times
                 parameters["amplitude_values"].value = step_amplitudes
                 nest.SetStatus(self._device, {key: step_amplitudes,
                                               'amplitude_times': step_times})
             elif key in ("start", "stop"):
                 nest.SetStatus(self._device, {key: self._delay_correction(value)})
```

### Comparing `PyNN-0.9.5/pyNN/nest/standardmodels/synapses.py` & `PyNN-0.9.6/pyNN/nest/standardmodels/synapses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Synapse Dynamics classes for nest
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import nest
 from pyNN.standardmodels import synapses, build_translations
 from pyNN.nest.synapses import NESTSynapseMixin
@@ -23,21 +23,21 @@
         ('delay', 'delay')
     )
     nest_name = 'static_synapse'
 
 
 class STDPMechanism(synapses.STDPMechanism, NESTSynapseMixin):
     """Specification of STDP models."""
-    
+
     base_translations = build_translations(
         ('weight', 'weight', 1000.0),  # nA->pA, uS->nS
         ('delay', 'delay'),
         ('dendritic_delay_fraction', 'dendritic_delay_fraction')
     )  # will be extended by translations from timing_dependence, etc.
-    
+
     def __init__(self, timing_dependence=None, weight_dependence=None,
                  voltage_dependence=None, dendritic_delay_fraction=1.0,
                  weight=0.0, delay=None):
         if dendritic_delay_fraction != 1:
             raise ValueError("NEST does not currently support axonal delays: "
                              "for the purpose of STDP calculations all delays "
                              "are assumed to be dendritic.")
@@ -65,15 +65,15 @@
         for name, value in self.native_parameters.items():
             if value.is_homogeneous:
                 value.shape = (1,)
                 synapse_defaults[name] = value.evaluate(simplify=True)
         synapse_defaults.pop("dendritic_delay_fraction")
         synapse_defaults.pop("w_min_always_zero_in_NEST")
         # Tau_minus is a parameter of the post-synaptic cell, not of the connection
-        synapse_defaults.pop("tau_minus")
+        synapse_defaults.pop("tau_minus", None)
 
         synapse_defaults = make_sli_compatible(synapse_defaults)
         nest.SetDefaults(base_model + '_lbl', synapse_defaults)
         return base_model + '_lbl'
 
 
 class TsodyksMarkramSynapse(synapses.TsodyksMarkramSynapse, NESTSynapseMixin):
@@ -194,18 +194,41 @@
 
     def __init__(self, w_min=0.0, w_max=1.0, mu_plus=0.5, mu_minus=0.5):
         if w_min != 0:
             raise Exception("Non-zero minimum weight is not supported by NEST.")
         synapses.GutigWeightDependence.__init__(self, w_min, w_max)
 
 
+def _translate_A_minus_forwards(**parameters):
+    A_minus = parameters["A_minus"]
+    A_plus = parameters["A_plus"]
+    if A_plus == 0:
+        # can't divide by zero, and value of alpha has no
+        # effect (since it will be multiplied by zero in NEST)
+        # so we just store the provided value of A_minus
+        alpha = A_minus
+    # to-do: handle the case where A_plus is an array with some zero values
+    else:
+        alpha = A_minus / A_plus
+    return alpha
+
+def _translate_A_minus_reverse(**parameters):
+    alpha = parameters["alpha"]
+    lambda_ = parameters["lambda"]
+    if lambda_ == 0:
+        A_minus = alpha  # presumed to have been stored by _translate_A_minus_forwards
+    else:
+        A_minus = alpha * lambda_
+    return A_minus
+
+
 class SpikePairRule(synapses.SpikePairRule):
     __doc__ = synapses.SpikePairRule.__doc__
 
     translations = build_translations(
         ('tau_plus',  'tau_plus'),
         ('tau_minus', 'tau_minus'), # defined in post-synaptic neuron
         ('A_plus',    'lambda'),
-        ('A_minus',   'alpha', 'A_minus/A_plus', 'alpha*lambda'),
+        ('A_minus',   'alpha', _translate_A_minus_forwards, _translate_A_minus_reverse),
 
     )
     possible_models = set(['stdp_synapse']) #,'stdp_synapse_hom'])
```

### Comparing `PyNN-0.9.5/pyNN/nest/synapses.py` & `PyNN-0.9.6/pyNN/nest/synapses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Definition of NativeSynapseType class for NEST
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import nest
 
 from pyNN.models import BaseSynapseType
+from pyNN.errors import NoModelAvailableError
 from .simulator import state
 from .conversion import make_pynn_compatible, make_sli_compatible
 
 DEFAULT_TAU_MINUS = 20.0
 
 
 def get_synapse_defaults(model_name):
     defaults = nest.GetDefaults(model_name)
     ignore = ['max_delay', 'min_delay', 'num_connections',
               'num_connectors', 'receptor_type', 'synapsemodel',
               'property_object', 'element_type', 'type', 'sizeof',
               'has_delay', 'synapse_model', 'requires_symmetric',
-              'weight_recorder']
+              'weight_recorder', 'init_flag', 'next_readout_time',
+              'synapse_id']
     default_params = {}
     for name, value in defaults.items():
         if name not in ignore:
             default_params[name] = value
     default_params['tau_minus'] = DEFAULT_TAU_MINUS
     return default_params
 
@@ -35,15 +37,23 @@
         synapse_defaults = {}
         for name, value in self.native_parameters.items():
             if value.is_homogeneous:
                 value.shape = (1,)
                 synapse_defaults[name] = value.evaluate(simplify=True)
         synapse_defaults = make_sli_compatible(synapse_defaults)
         synapse_defaults.pop("tau_minus", None)
-        nest.SetDefaults(self.nest_name + '_lbl', synapse_defaults)
+        try:
+            nest.SetDefaults(self.nest_name + '_lbl', synapse_defaults)
+        except nest.lib.hl_api_exceptions.NESTError as err:
+            if not state.extensions_loaded:
+                raise NoModelAvailableError(
+                    "{self.__class__.__name__} is not available."
+                    "There was a problem loading NEST extensions".format(self=self)
+                )
+            raise
         return self.nest_name + '_lbl'
 
     def _get_minimum_delay(self):
         return state.min_delay
 
     def _set_tau_minus(self, cells):
         if len(cells) > 0 and self.has_parameter('tau_minus'):
```

### Comparing `PyNN-0.9.5/pyNN/network.py` & `PyNN-0.9.6/pyNN/network.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/__init__.py` & `PyNN-0.9.6/pyNN/neuroml/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/populations.py` & `PyNN-0.9.6/pyNN/neuroml/populations.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/projections.py` & `PyNN-0.9.6/pyNN/neuroml/projections.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/recording.py` & `PyNN-0.9.6/pyNN/neuroml/recording.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/simulator.py` & `PyNN-0.9.6/pyNN/neuroml/simulator.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/neuroml/standardmodels/cells.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/standardmodels/electrodes.py` & `PyNN-0.9.6/pyNN/neuroml/standardmodels/electrodes.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuroml/standardmodels/synapses.py` & `PyNN-0.9.6/pyNN/neuroml/standardmodels/synapses.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/__init__.py` & `PyNN-0.9.6/pyNN/neuron/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 nrnpython implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import warnings
 try:
     from mpi4py import MPI
```

### Comparing `PyNN-0.9.5/pyNN/neuron/cells.py` & `PyNN-0.9.6/pyNN/neuron/cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Definition of cell classes for the neuron module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
 from math import pi
 import numpy
```

### Comparing `PyNN-0.9.5/pyNN/neuron/connectors.py` & `PyNN-0.9.6/pyNN/neuron/connectors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Connection method classes for the neuron module
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from pyNN.neuron import simulator
 from pyNN.connectors import AllToAllConnector, \
                             OneToOneConnector, \
```

### Comparing `PyNN-0.9.5/pyNN/neuron/nineml.py` & `PyNN-0.9.6/pyNN/neuron/nineml.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Functions:
     nineml_cell_type - return a new NineMLCellType subclass
 
 Constants:
     NMODL_DIR        - subdirectory to which NMODL mechanisms will be written
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from __future__ import absolute_import
 import logging
 import os
@@ -101,8 +101,7 @@
     """
     Return a new NineMLCellType subclass.
     """
     return build_nineml_celltype(name, (NineMLCellType,),
                                  {'combined_model': combined_model,
                                   'weight_variables': weight_vars,
                                   'builder': _compile_nmodl})
-
```

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/adexp.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/adexp.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/alphaisyn.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/alphaisyn.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/alphasyn.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/alphasyn.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/gammastim.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/gammastim.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/gif.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/gif.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/gsfa_grr.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/gsfa_grr.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/hh_traub.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/hh_traub.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/izhikevich.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/izhikevich.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/netstim2.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/netstim2.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/poisson_stim_refractory.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/poisson_stim_refractory.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/quantal_stp.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/quantal_stp.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/refrac.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/refrac.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/reset.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/reset.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_guetig.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_guetig.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_softlimits.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_softlimits.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_songabbott.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_songabbott.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_symm.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_symm.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stdwa_vogels2011.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stdwa_vogels2011.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stochastic_synapse.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stochastic_synapse.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/stochastic_tsodyksmarkram.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/stochastic_tsodyksmarkram.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/tmgsyn.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/tmgsyn.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/tmisyn.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/tmisyn.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/tsodyksmarkram.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/tsodyksmarkram.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/nmodl/vecstim.mod` & `PyNN-0.9.6/pyNN/neuron/nmodl/vecstim.mod`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/populations.py` & `PyNN-0.9.6/pyNN/neuron/populations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 nrnpython implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 import logging
 from pyNN import common
@@ -52,15 +52,15 @@
             value = initial_values.evaluate(simplify=True)
             for cell in self:  # only on local node
                 setattr(cell._cell, "%s_init" % variable, value)
         else:
             if isinstance(initial_values.base_value, RandomDistribution) and initial_values.base_value.rng.parallel_safe:
                 local_values = initial_values.evaluate()[self._mask_local]
             else:
-                local_values = initial_values[self._mask_local]            
+                local_values = initial_values[self._mask_local]
             for cell, value in zip(self, local_values):
                 setattr(cell._cell, "%s_init" % variable, value)
 
 
 class Assembly(common.Assembly):
     __doc__ = common.Assembly.__doc__
     _simulator = simulator
@@ -95,15 +95,15 @@
         """
         Create cells in NEURON using the celltype of the current Population.
         """
         # this method should never be called more than once
         # perhaps should check for that
         self.first_id = simulator.state.gid_counter
         self.last_id = simulator.state.gid_counter + self.size - 1
-        self.all_cells = numpy.array([id for id in range(self.first_id, self.last_id + 1)], 
+        self.all_cells = numpy.array([id for id in range(self.first_id, self.last_id + 1)],
                                      simulator.ID)
 
         # mask_local is used to extract those elements from arrays that apply to the cells on the current node
         # round-robin distribution of cells between nodes
         self._mask_local = self.all_cells % simulator.state.num_processes == simulator.state.mpi_rank
 
         if isinstance(self.celltype, StandardCellType):
```

### Comparing `PyNN-0.9.5/pyNN/neuron/projections.py` & `PyNN-0.9.6/pyNN/neuron/projections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 nrnpython implementation of the PyNN API.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 from copy import deepcopy
 import numpy
 import logging
 try:
@@ -37,15 +37,15 @@
                  space=Space(), label=None):
         __doc__ = common.Projection.__init__.__doc__
         common.Projection.__init__(self, presynaptic_population, postsynaptic_population,
                                    connector, synapse_type, source, receptor_type,
                                    space, label)
         self._connections = dict((index, defaultdict(list)) for index in self.post._mask_local.nonzero()[0])
         connector.connect(self)
-        self._presynaptic_components = dict((index, {}) for index in 
+        self._presynaptic_components = dict((index, {}) for index in
                                             self.pre._mask_local.nonzero()[0])
         if self.synapse_type.presynaptic_type:
             self._configure_presynaptic_components()
         _projections.append(self)
         logger.info("--- Projection[%s].__init__() ---" % self.label)
 
     @property
@@ -96,39 +96,39 @@
             parameters = dict(zip(connection_parameters.keys(), values))
             #logger.debug("Connecting neuron #%s to neuron #%s with synapse type %s, receptor type %s, parameters %s", pre_idx, postsynaptic_index, self.synapse_type, self.receptor_type, parameters)
             self._connections[postsynaptic_index][pre_idx].append(
                 self.synapse_type.connection_type(self, pre_idx, postsynaptic_index, **parameters))
 
     def _configure_presynaptic_components(self):
         """
-        For gap junctions potentially other complex synapse types the presynaptic side of the 
+        For gap junctions potentially other complex synapse types the presynaptic side of the
         connection also needs to be initiated. This is a little tricky with sources distributed on
-        different nodes as the parameters need to be gathered to the node where the source is 
+        different nodes as the parameters need to be gathered to the node where the source is
         hosted before it can be set
         """
         # Get the list of all connections on all nodes
-        conn_list = numpy.array(self.get(self.synapse_type.get_parameter_names(), 'list', 
+        conn_list = numpy.array(self.get(self.synapse_type.get_parameter_names(), 'list',
                                                gather='all', with_address=True))
-        # Loop through each of the connections where the presynaptic index (first column) is on 
+        # Loop through each of the connections where the presynaptic index (first column) is on
         # the local node
-        mask_local = numpy.array(numpy.in1d(numpy.squeeze(conn_list[:, 0]), 
+        mask_local = numpy.array(numpy.in1d(numpy.squeeze(conn_list[:, 0]),
                                             numpy.nonzero(self.pre._mask_local)[0]), dtype=bool)
         for conn in conn_list[mask_local, :]:
             pre_idx = int(conn[0])
             post_idx = int(conn[1])
             params = dict(zip(self.synapse_type.get_parameter_names(), conn[2:]))
             self._presynaptic_components[pre_idx][post_idx] = \
                                 self.synapse_type.presynaptic_type(self, pre_idx, post_idx, **params)
 
     def _set_attributes(self, parameter_space):
         # If synapse has pre-synaptic components evaluate the parameters for them
         if self.synapse_type.presynaptic_type:
             presyn_param_space = deepcopy(parameter_space)
             presyn_param_space.evaluate(mask=(slice(None), self.pre._mask_local))
-            for component, connection_parameters in zip(self._presynaptic_components.values(), 
+            for component, connection_parameters in zip(self._presynaptic_components.values(),
                                                         presyn_param_space.columns()):
                 for name, value in connection_parameters.items():
                     for index in component:
                         setattr(component[index], name, value[index])
         # Evaluate the parameters for the post-synaptic components (typically the "Connection" object)
         parameter_space.evaluate(mask=(slice(None), self.post._mask_local))  # only columns for connections that exist on this machine
         for connection_group, connection_parameters in zip(self._connections.values(),
```

### Comparing `PyNN-0.9.5/pyNN/neuron/random.py` & `PyNN-0.9.6/pyNN/neuron/random.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/neuron/recording.py` & `PyNN-0.9.6/pyNN/neuron/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import numpy
 from pyNN import recording
 from pyNN.neuron import simulator
 import re
```

### Comparing `PyNN-0.9.5/pyNN/neuron/simulator.py` & `PyNN-0.9.6/pyNN/neuron/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Attributes:
     state -- a singleton instance of the _State class.
 
 All other functions and classes are private, and should not be used by other
 modules.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 try:
     xrange
 except NameError:
@@ -31,17 +31,17 @@
 import os.path
 from neuron import h, nrn_dll_loaded
 from operator import itemgetter
 
 logger = logging.getLogger("PyNN")
 name = "NEURON"  # for use in annotating output data
 
-# Instead of starting the projection var-GID range from 0, the first _MIN_PROJECTION_VARGID are 
+# Instead of starting the projection var-GID range from 0, the first _MIN_PROJECTION_VARGID are
 # reserved for other potential uses
-_MIN_PROJECTION_VARGID = 1000000 
+_MIN_PROJECTION_VARGID = 1000000
 
 # --- Internal NEURON functionality --------------------------------------------
 
 
 def load_mechanisms(path):
     """
     Search for and load NMODL mechanisms from the path given.
@@ -270,33 +270,33 @@
         self.parallel_context.done()
         if quit:
             logger.info("Finishing up with NEURON.")
             h.quit()
 
     def get_vargids(self, projection, pre_idx, post_idx):
         """
-        Get new "variable"-GIDs (as opposed to the "cell"-GIDs) for a given pre->post connection 
-        pair for a given projection. 
+        Get new "variable"-GIDs (as opposed to the "cell"-GIDs) for a given pre->post connection
+        pair for a given projection.
 
         `projection`  -- projection
         `pre_idx`     -- index of the presynaptic cell
         `post_idx`     -- index of the postsynaptic cell
         """
         try:
             offset = self.vargid_offsets[projection]
         except KeyError:
             # Get the projection with the current maximum vargid offset
             if len(self.vargid_offsets):
                 newest_proj, offset = max(self.vargid_offsets.items(), key=itemgetter(1))
-                # Allocate it a large enough range for a mutual all-to-all connection (assumes that 
+                # Allocate it a large enough range for a mutual all-to-all connection (assumes that
                 # there are no duplicate pre_idx->post_idx connections for the same projection. If
                 # that is really desirable a new projection will need to be used)
                 offset += 2 * len(newest_proj.pre) * len(newest_proj.post)
             else:
-                offset = _MIN_PROJECTION_VARGID 
+                offset = _MIN_PROJECTION_VARGID
             self.vargid_offsets[projection] = offset
         pre_post_vargid = offset + 2 * (pre_idx + post_idx * len(projection.pre))
         post_pre_vargid = pre_post_vargid + 1
         return (pre_post_vargid, post_pre_vargid)
 
 # --- For implementation of access to individual neurons' parameters -----------
 
@@ -459,88 +459,88 @@
     """
 
     def __init__(self, projection, pre, post, **parameters):
         self.presynaptic_index = pre
         self.postsynaptic_index = post
         segment_name = projection.receptor_type
         # Strip 'gap' string from receptor_type (not sure about this, it is currently appended to
-        # the available synapse types in the NCML model segments but is not really necessary and 
+        # the available synapse types in the NCML model segments but is not really necessary and
         # it feels a bit hacky but it makes the list of receptor types more comprehensible)
-        if segment_name.endswith('.gap'): 
+        if segment_name.endswith('.gap'):
             segment_name = segment_name[:-4]
         self.segment = getattr(projection.post[post]._cell, segment_name)
         pre_post_vargid, post_pre_vargid = state.get_vargids(projection, pre, post)
-        self._make_connection(self.segment, parameters.pop('weight'), pre_post_vargid,   
+        self._make_connection(self.segment, parameters.pop('weight'), pre_post_vargid,
                               post_pre_vargid, projection.pre[pre], projection.post[post])
-        
+
     def _make_connection(self, segment, weight, local_to_remote_vargid, remote_to_local_vargid,
-                         local_gid, remote_gid):       
+                         local_gid, remote_gid):
         logger.debug("Setting source_var on local cell {} to connect to target_var on remote "
                      "cell {} with vargid {} on process {}"
-                    .format(local_gid, remote_gid, local_to_remote_vargid, 
+                    .format(local_gid, remote_gid, local_to_remote_vargid,
                             state.mpi_rank))
-        # Set up the source reference for the local->remote connection 
-        state.parallel_context.source_var(segment(0.5)._ref_v, local_to_remote_vargid)              
+        # Set up the source reference for the local->remote connection
+        state.parallel_context.source_var(segment(0.5)._ref_v, local_to_remote_vargid)
         # Create the gap_junction and set its weight
         self.gap = h.Gap(0.5, sec=segment)
         self.gap.g = weight
         # Connect the gap junction with the source_var
         logger.debug("Setting target_var on local cell {} to connect to source_var on remote "
                      "cell {} with vargid {} on process {}"
-                    .format(local_gid, remote_gid, remote_to_local_vargid, 
+                    .format(local_gid, remote_gid, remote_to_local_vargid,
                             state.mpi_rank))
         # set up the target reference for the remote->local connection
         state.parallel_context.target_var(self.gap._ref_vgap, remote_to_local_vargid)
-        
+
     def _set_weight(self, w):
         self.gap.g = w
 
     def _get_weight(self):
         """Gap junction conductance in µS."""
         return self.gap.g
-    
+
     weight = property(_get_weight, _set_weight)
-    
+
     def as_tuple(self, *attribute_names):
         return tuple(getattr(self, name) for name in attribute_names)
-    
+
 
 class GapJunctionPresynaptic(GapJunction):
     """
     The presynaptic component of a gap junction. Gap junctions in NEURON are actually symmetrical
     so it shares its functionality with the GapJunction connection object, with the exception that
     the pre and post synaptic cells are switched
     """
-    
+
     def __init__(self, projection, pre, post, **parameters):
         self.presynaptic_index = pre
         self.postsynaptic_index = post
-        if projection.source.endswith('.gap'): 
+        if projection.source.endswith('.gap'):
             segment_name = projection.source[:-4]
         else:
             segment_name = projection.source
         self.segment = getattr(projection.pre[pre]._cell, segment_name)
         pre_post_vargid, post_pre_vargid = state.get_vargids(projection, pre, post)
-        self._make_connection(self.segment, parameters.pop('weight'), post_pre_vargid, 
+        self._make_connection(self.segment, parameters.pop('weight'), post_pre_vargid,
                               pre_post_vargid, projection.post[post], projection.pre[pre])
-    
+
 
 def generate_synapse_property(name):
     def _get(self):
         return getattr(self.weight_adjuster, name)
 
     def _set(self, val):
         setattr(self.weight_adjuster, name, val)
     return property(_get, _set)
-setattr(Connection, 'w_max', generate_synapse_property('wmax'))
-setattr(Connection, 'w_min', generate_synapse_property('wmin'))
-setattr(Connection, 'A_plus', generate_synapse_property('aLTP'))
-setattr(Connection, 'A_minus', generate_synapse_property('aLTD'))
-setattr(Connection, 'tau_plus', generate_synapse_property('tauLTP'))
-setattr(Connection, 'tau_minus', generate_synapse_property('tauLTD'))
+setattr(Connection, 'wmax', generate_synapse_property('wmax'))
+setattr(Connection, 'wmin', generate_synapse_property('wmin'))
+setattr(Connection, 'aLTP', generate_synapse_property('aLTP'))
+setattr(Connection, 'aLTD', generate_synapse_property('aLTD'))
+setattr(Connection, 'tauLTP', generate_synapse_property('tauLTP'))
+setattr(Connection, 'tauLTD', generate_synapse_property('tauLTD'))
 setattr(Connection, 'U', generate_synapse_property('U'))
 setattr(Connection, 'tau_rec', generate_synapse_property('tau_rec'))
 setattr(Connection, 'tau_facil', generate_synapse_property('tau_facil'))
 setattr(Connection, 'u0', generate_synapse_property('u0'))
 setattr(Connection, 'tau', generate_synapse_property('tau'))
 setattr(Connection, 'eta', generate_synapse_property('eta'))
 setattr(Connection, 'rho', generate_synapse_property('rho'))
```

### Comparing `PyNN-0.9.5/pyNN/neuron/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/neuron/standardmodels/cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Standard base_cells for the neuron module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from pyNN.standardmodels import cells as base_cells, build_translations
 from pyNN.neuron.cells import (StandardIF, SingleCompartmentTraub,
                                RandomSpikeSource, VectorSpikeSource,
```

### Comparing `PyNN-0.9.5/pyNN/neuron/standardmodels/electrodes.py` & `PyNN-0.9.6/pyNN/neuron/standardmodels/electrodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Classes:
     DCSource           -- a single pulse of current of constant amplitude.
     StepCurrentSource  -- a step-wise time-varying current.
     NoisyCurrentSource -- a Gaussian whitish noise current.
     ACSource           -- a sine modulated current.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from neuron import h
 import numpy
 from pyNN.standardmodels import electrodes, build_translations, StandardCurrentSource
```

### Comparing `PyNN-0.9.5/pyNN/neuron/standardmodels/synapses.py` & `PyNN-0.9.6/pyNN/neuron/standardmodels/synapses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Synapse Dynamics classes for the neuron module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from pyNN.standardmodels import synapses, build_translations
 from pyNN.neuron.simulator import state, Connection, GapJunction, GapJunctionPresynaptic
 
@@ -39,15 +39,15 @@
 
     translations = build_translations(
         ('weight', 'weight'),
     )
     model = 'Gap'
 
     def _get_minimum_delay(self):
-        return state.min_delay    
+        return state.min_delay
 
 
 class STDPMechanism(BaseSynapse, synapses.STDPMechanism):
     __doc__ = synapses.STDPMechanism.__doc__
     postsynaptic_variable = 'spikes'
 
     base_translations = build_translations(
@@ -196,14 +196,14 @@
 
     )
     possible_models = set(['StdwaSA', 'StdwaSoft', 'StdwaGuetig'])
 
 
 class Vogels2011Rule(synapses.Vogels2011Rule):
     __doc__ = synapses.Vogels2011Rule.__doc__
-    
+
     translations = build_translations(
         ('tau',  'tau'),
         ('eta', 'eta'),
         ('rho', 'rho'),
     )
     possible_models = set(['StdwaVogels2011'])
```

### Comparing `PyNN-0.9.5/pyNN/nineml/__init__.py` & `PyNN-0.9.6/pyNN/nineml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Export of PyNN scripts as NineML.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 import logging
 import nineml.user as ul
 from neo.io import get_io
 
 from .. import common, random, standardmodels as std
```

### Comparing `PyNN-0.9.5/pyNN/nineml/cells.py` & `PyNN-0.9.6/pyNN/nineml/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Cell models generated from 9ML
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import logging
 from itertools import chain
 import nineml.abstraction as nineml
 from pyNN.models import BaseCellType
@@ -114,8 +114,7 @@
                              + [alias.lhs for alias in flat_component.aliases]
                              + [statevar.name for statevar in flat_component.state_variables])
 
         logger.debug("Creating class '%s' with bases %s and dictionary %s" % (name, bases, dct))
         dct["builder"](flat_component, dct["weight_variables"], hierarchical_mode=True)
 
         return type.__new__(cls, name, bases, dct)
-
```

### Comparing `PyNN-0.9.5/pyNN/nineml/connectors.py` & `PyNN-0.9.6/pyNN/nineml/connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Export of PyNN scripts as NineML.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import nineml.user as nineml
 
 from pyNN import connectors
 from utility import build_parameter_set, catalog_url
@@ -22,15 +22,15 @@
                                     definition=nineml.Definition(self.definition_url,
                                                                  "connection_generator"),
                                     parameters=build_parameter_set(connector_parameters))
         return connection_rule
 
 
 class FixedProbabilityConnector(ConnectorMixin, connectors.FixedProbabilityConnector):
-    definition_url = "%s/connectionrules/random_fixed_probability.xml" % catalog_url 
+    definition_url = "%s/connectionrules/random_fixed_probability.xml" % catalog_url
     parameter_names = ('p_connect', 'allow_self_connections')
 
 
 class DistanceDependentProbabilityConnector(ConnectorMixin, connectors.DistanceDependentProbabilityConnector):
     definition_url = "%s/connectionrules/distance_dependent_probability.xml" % catalog_url
     parameter_names = ('d_expression', 'allow_self_connections')  # space
```

### Comparing `PyNN-0.9.5/pyNN/nineml/populations.py` & `PyNN-0.9.6/pyNN/nineml/populations.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nineml/projections.py` & `PyNN-0.9.6/pyNN/nineml/projections.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nineml/read.py` & `PyNN-0.9.6/pyNN/nineml/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Enables creating neuronal network models in PyNN from a 9ML description.
 
 Classes:
     Network -- container for a network model.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 import nineml.user as nineml
 import nineml.abstraction as al
 import pyNN.nineml
 import pyNN.random
```

### Comparing `PyNN-0.9.5/pyNN/nineml/recording.py` & `PyNN-0.9.6/pyNN/nineml/recording.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nineml/simulator.py` & `PyNN-0.9.6/pyNN/nineml/simulator.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nineml/standardmodels.py` & `PyNN-0.9.6/pyNN/nineml/standardmodels.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/pyNN/nineml/utility.py` & `PyNN-0.9.6/pyNN/nineml/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # encoding: utf-8
 """
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from __future__ import division
 from lazyarray import larray
 from pyNN import random
 from pyNN.parameters import Sequence
```

### Comparing `PyNN-0.9.5/pyNN/parameters.py` & `PyNN-0.9.6/pyNN/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Parameter set handling
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:  # Python 2
     basestring
     long
 except NameError:  # Python 3
@@ -13,14 +13,15 @@
     long = int
 import numpy
 import collections
 from pyNN.core import is_listlike
 from pyNN import errors
 from pyNN.random import RandomDistribution, NativeRNG
 from lazyarray import larray, partial_shape
+import numpy as np
 
 
 class LazyArray(larray):
     """
     Optimises storage of arrays in various ways:
       - stores only a single value if all the values in the array are the same
       - if the array is created from a :class:`~pyNN.random.RandomDistribution`
```

### Comparing `PyNN-0.9.5/pyNN/random.py` & `PyNN-0.9.6/pyNN/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     NumpyRNG           - uses the numpy.random.RandomState RNG
     GSLRNG             - uses the RNGs from the Gnu Scientific Library
     NativeRNG          - indicates to the simulator that it should use it's own,
                          built-in RNG
     RandomDistribution - produces random numbers from a specific distribution
 
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from copy import deepcopy
 import logging
 import numpy.random
@@ -89,28 +89,28 @@
         If:
             * `n` is None, return a float,
             * `n` >= 1, return a Numpy array,
             * `n` < 0, raise an Exception,
             * `n` is 0, return an empty array.
 
         If called with distribution=None, returns uniformly distributed floats in the range [0, 1)
-        
+
         If `mask` is provided, it should be a boolean or integer NumPy array,
         indicating that only a subset of the random numbers should be returned.
-        
+
         Example::
-            
+
             rng.next(5, mask=np.array([True, False, True, False, True]))
-            
+
         or::
-        
+
             rng.next(5, mask=np.array([0, 2, 4]))
-            
+
         will each return only three values.
-        
+
         If the rng is "parallel safe", an array of n values will be drawn from the rng,
         and the mask applied.
         If the rng is not parallel safe, the contents of the mask are disregarded, only its
         size (for an integer mask) or the number of True values (for a boolean mask)
         is used in determining how many values to draw.
         """
         raise NotImplementedError
@@ -415,18 +415,18 @@
                 return dict((name, value) for name, value in zip(expected_parameter_names, positional))
         else:
             raise ValueError("Mixed positional and named parameters")
 
     def lazily_evaluate(self, mask=None, shape=None):
         """
         Generate an array of random numbers of the requested shape.
-        
+
         If a mask is given, produce only enough numbers to fill the
         region defined by the mask (hence 'lazily').
-        
+
         This method is called by the lazyarray `evaluate()` and
         `_partially_evaluate()` methods.
         """
         if mask is None:
             # produce an array of random numbers with the requested shape
             n = reduce(operator.mul, shape)
             res = self.next(n)
```

### Comparing `PyNN-0.9.5/pyNN/recording/__init__.py` & `PyNN-0.9.6/pyNN/recording/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Defines classes and functions for managing recordings (spikes, membrane
 potential etc).
 
 These classes and functions are not part of the PyNN API, and are only for
 internal use.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import logging
 import numpy
 import os
@@ -217,26 +217,36 @@
         self.sampling_interval = self._simulator.state.dt
 
     def record(self, variables, ids, sampling_interval=None):
         """
         Add the cells in `ids` to the sets of recorded cells for the given variables.
         """
         logger.debug('Recorder.record(<%d cells>)' % len(ids))
-        if sampling_interval is not None:
-            if sampling_interval != self.sampling_interval and len(self.recorded) > 0:
-                raise ValueError("All neurons in a population must be recorded with the same sampling interval.")
+        self._check_sampling_interval(sampling_interval)
 
         ids = set([id for id in ids if id.local])
         for variable in normalize_variables_arg(variables):
             if not self.population.can_record(variable):
                 raise errors.RecordingError(variable, self.population.celltype)
             new_ids = ids.difference(self.recorded[variable])
             self.recorded[variable] = self.recorded[variable].union(ids)
             self._record(variable, new_ids, sampling_interval)
 
+    def _check_sampling_interval(self, sampling_interval):
+        """
+        Check whether record() has been called previously with a different sampling interval
+        (we exclude recording of spikes, as the sampling interval does not apply in that case)
+        """
+        if sampling_interval is not None and sampling_interval != self.sampling_interval:
+            recorded_variables = list(self.recorded.keys())
+            if "spikes" in recorded_variables:
+                recorded_variables.remove("spikes")
+            if len(recorded_variables) > 0:
+                raise ValueError("All neurons in a population must be recorded with the same sampling interval.")
+
     def reset(self):
         """Reset the list of things to be recorded."""
         self._reset()
         self.recorded = defaultdict(set)
 
     def filter_recorded(self, variable, filter_ids):
         if filter_ids is not None:
```

### Comparing `PyNN-0.9.5/pyNN/recording/files.py` & `PyNN-0.9.6/pyNN/recording/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Classes:
     StandardTextFile
     PickleFile
     NumpyBinaryFile
     HDF5ArrayFile - requires PyTables
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 import numpy
 import os
 import shutil
```

### Comparing `PyNN-0.9.5/pyNN/serialization/sonata.py` & `PyNN-0.9.6/pyNN/serialization/sonata.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,19 @@
 import json
 import logging
 try:
     basestring
 except NameError:  # Python 3
     basestring = str
 
-import h5py
+try:
+    import h5py
+    HAVE_H5PY = True
+except ImportError:
+    HAVE_H5PY = False
 import numpy as np
 from pyNN.network import Network
 from pyNN.parameters import Sequence
 
 
 # Note: The SonataIO class will be moved to Neo once fully implemented
 
@@ -65,14 +69,16 @@
     """
 
     def __init__(self, base_dir,
                  spikes_file="spikes.h5",
                  spikes_sort_order=None,
                  report_config=None,
                  node_sets=None):
+        if not HAVE_H5PY:
+            raise Exception("You need to install h5py to use SonataIO")
         self.base_dir = base_dir
         self.spike_file = spikes_file
         self.spikes_sort_order = spikes_sort_order
         self.report_config = report_config
         self.node_sets = node_sets
 
     def read(self):
@@ -84,15 +90,15 @@
         (*Currently only spike data supported)
         """
         file_path = join(self.base_dir, self.spike_file)
         block = neo.Block(file_origin=file_path)
         segment = neo.Segment(file_origin=file_path)
         spikes_file = h5py.File(file_path, 'r')
         for gid in np.unique(spikes_file['spikes']['gids']):
-            index = spikes_file['spikes']['gids'].value == gid
+            index = spikes_file['spikes']['gids'][()] == gid
             spike_times = spikes_file['spikes']['timestamps'][index]
             segment.spiketrains.append(
                 neo.SpikeTrain(spike_times,
                                t_stop = spike_times.max() + 1.0,
                                t_start=0.0,
                                units='ms',
                                source_id=gid)
@@ -186,14 +192,20 @@
         try:
             value = float(value)
         except ValueError:
             pass
     return value
 
 
+def to_string(s):
+    if isinstance(s, bytes):
+        s = s.decode('utf-8')
+    return s
+
+
 def read_types_file(file_path, node_or_edge):
     """Read node type or edge type parameters from a SONATA CSV file.
 
     Returns a dict representing the parameters row-wise, indexed by the type id.
     """
     with open(file_path) as csv_file:
         csv_reader = csv.DictReader(csv_file, delimiter=' ', quotechar='"')
@@ -313,14 +325,16 @@
     node populations must be disjoint, whereas a given neuron may be in more than one
     PyNN Assembly (it is PyNN Populations that are disjoint).
 
     In this first version of the export, we simplify this by exporting each Population
     as an implicit Assembly with a single member, at the cost of losing some information about
     the PyNN network structure. This approach could be improved in future.
     """
+    if not HAVE_H5PY:
+        raise Exception("You need to install h5py to use SONATA")
 
     # --- define directory layout ---
     config = {
         "target_simulator": target,
         "manifest": {
             "$BASE_DIR": "{}".format(output_path),
             "$NETWORK_DIR": "$BASE_DIR/networks",
@@ -382,22 +396,25 @@
         n = population.size
         population_label = asciify(population.label)
         csv_rows = []
         csv_columns = set()
         node_type_info = {
             "node_type_id": i,
         }
-        if target.lower() == "neuron":
-            node_type_info["model_type"] = "single_compartment"
-        elif target.lower() in ("pynn", "nest"):
-            node_type_info["model_type"] = "point_neuron"
-            node_type_info["model_template"] = "{}:{}".format(target.lower(),
-                                                              population.celltype.__class__.__name__)
+        if "SpikeSource" in population.celltype.__class__.__name__:
+            node_type_info["model_type"] = "virtual"
         else:
-            raise NotImplementedError
+            if target.lower() == "neuron":
+                node_type_info["model_type"] = "single_compartment"
+            elif target.lower() in ("pynn", "nest"):
+                node_type_info["model_type"] = "point_neuron"
+                node_type_info["model_template"] = "{}:{}".format(target.lower(),
+                                                                population.celltype.__class__.__name__)
+            else:
+                raise NotImplementedError
         group_label = 0  #"default"
         # todo: add "population" column
 
         # write HDF5 file
         nodes_file = h5py.File(nodes_path, 'w')
         nodes_file.attrs["version"] = (0, 1)  # ??? unclear what is the required format or the current version!
         nodes_file.attrs["magic"] = MAGIC  # needs to be uint32
@@ -410,24 +427,27 @@
                                                                           # required data type not specified. Optional?
         default.create_dataset("node_group_index", data=np.arange(n, dtype=int), dtype='i2')
 
         # parameters
         node_group = default.create_group(str(group_label))
         node_params_group = node_group.create_group("dynamics_params")
         for parameter_name in population.celltype.default_parameters:
-            # we could make a single get call to get all params at once, at the expense
-            # of higher memory usage. To profile...
-            values = population.get(parameter_name, gather=True, simplify=True)
-            if isinstance(values, np.ndarray):
-                # array, put into the HDF5 file and put 'NONE' in the CSV file
-                node_params_group.create_dataset(parameter_name, data=values)
-                node_type_info[parameter_name] = "NONE"
+            if parameter_name == "spike_times":
+                warn("spike times should be added manually to simulation_config")
             else:
-                # scalar, put into the CSV file
-                node_type_info[parameter_name] = values
+                # we could make a single get call to get all params at once, at the expense
+                # of higher memory usage. To profile...
+                values = population.get(parameter_name, gather=True, simplify=True)
+                if isinstance(values, np.ndarray):
+                    # array, put into the HDF5 file and put 'NONE' in the CSV file
+                    node_params_group.create_dataset(parameter_name, data=values)
+                    node_type_info[parameter_name] = "NONE"
+                else:
+                    # scalar, put into the CSV file
+                    node_type_info[parameter_name] = values
 
         # positions in space
         x, y, z = population.positions
         node_group.create_dataset('x', data=x)
         node_group.create_dataset('y', data=y)
         node_group.create_dataset('z', data=z)
 
@@ -453,16 +473,16 @@
 
     # --- export edges ---
     # - we define a separate group and edge-type for each PyNN Projection
 
     for i, projection in enumerate(network.projections):
         projection_label = asciify(projection.label)
         config["networks"]["edges"].append({
-            "edges_file": "$NETWORK_DIR/edges_{}.h5".format(projection_label.decode('utf-8')),
-            "edge_types_file": "$NETWORK_DIR/edge_types_{}.csv".format(projection_label.decode('utf-8'))
+            "edges_file": "$NETWORK_DIR/edges_{}.h5".format(projection_label),
+            "edge_types_file": "$NETWORK_DIR/edge_types_{}.csv".format(projection_label)
         })
         edge_type_path = Template(config["networks"]["edges"][i]["edge_types_file"]).substitute(NETWORK_DIR=network_dir)
         edges_path = Template(config["networks"]["edges"][i]["edges_file"]).substitute(NETWORK_DIR=network_dir)
 
         n = projection.size()
         csv_rows = []
         edge_type_info = {
@@ -537,14 +557,17 @@
     We map a SONATA node group to a PyNN Population, since both have homogeneous parameter
     namespaces.
     SONATA node types are used to give different parameters to different subsets of nodes in a group.
     This can be handled in PyNN by indexing and, equivalently, by defining PopulationViews.
     We map a SONATA edge group to a PyNN Projection, i.e. a SONATA edge population may
     result in multiple PyNN Projections.
     """
+    if not HAVE_H5PY:
+        raise Exception("You need to install h5py to use SONATA")
+
     config = load_config(config_file)
 
     if config.get("target_simulator", None) not in  ("PyNN", "NEST"):
         warn("`target_simulator` is not set to 'PyNN' or 'NEST'. Proceeding with caution...")
 
     sonata_node_populations = []
     for nodes_config in config["networks"]["nodes"]:
@@ -635,20 +658,21 @@
             Circuit config loaded from JSON.
         """
         obj = cls()
         obj.name = name
         obj.node_groups = []
         obj.node_ids = h5_data['node_id']
 
-        for ng_label in np.unique(h5_data['node_group_id'].value):
-            mask = h5_data['node_group_id'].value == ng_label
+        node_group_ids = h5_data['node_group_id'][()]
+        for ng_label in np.unique(node_group_ids):
+            mask = node_group_ids == ng_label
             logger.info("NODE GROUP {}, size {}".format(ng_label, mask.sum()))
 
             node_type_array = h5_data['node_type_id'][mask]
-            node_group_index = h5_data['node_group_index'][mask]
+            node_group_index = h5_data['node_group_index'][mask].tolist()
             obj.node_groups.append(
                 NodeGroup.from_data(ng_label,
                                     node_type_array,
                                     node_group_index,
                                     h5_data[str(ng_label)],
                                     node_types_map,
                                     config)
@@ -661,15 +685,15 @@
 
     def to_assembly(self, sim):
         """Create a PyNN Assembly from this NodePopulation.
 
         The Assembly will contain one Population for each NodeGroup.
         """
         assembly = sim.Assembly(label=self.name)
-        assembly.annotations["first_sonata_id"] = self.node_ids.value.min()
+        assembly.annotations["first_sonata_id"] = self.node_ids[()].min()
         for node_group in self.node_groups:
             pop = node_group.to_population(sim)
             assembly += pop
         return assembly
 
 
 class NodeGroup(object):
@@ -690,15 +714,15 @@
         ---------
 
         id : integer
             Taken from the SONATA nodes HDF5 file.
         node_types_array : NumPy array
             Subset of the data from "/nodes/<population_name>/node_type_id"
             that applies to this group.
-        index : NumPy array
+        index : list
             Subset of the data from "/nodes/<population_name>/node_group_index"
             that applies to this group.
         h5_data : HDF5 Group
             The "/nodes/<population_name>/<group_id>" group.
         node_types_map : dict
             Data loaded from node types CSV file. Top-level keys are node type ids.
         config : dict
@@ -729,15 +753,15 @@
                     parameters[name][node_type_id] = value
 
         # parameters defined in .h5 files
         if 'dynamics_params' in h5_data:
             dynamics_params_group = h5_data['dynamics_params']
             # not sure the next bit is using `index` correctly
             for key in dynamics_params_group.keys():
-                parameters[key] = dynamics_params_group[key].value[index]
+                parameters[key] = dynamics_params_group[key][index]
 
         obj.parameters = parameters
         obj.config = config
         logger.info(parameters)
 
         return obj
 
@@ -824,26 +848,26 @@
             Data loaded from edge types CSV file. Top-level keys are edge type ids.
         config : dict
             Circuit config loaded from JSON.
         """
 
         obj = cls()
         obj.name = name
-        obj.source_node_ids = h5_data["source_node_id"].value
-        obj.source_node_population = h5_data["source_node_id"].attrs["node_population"].decode('utf-8')
-        obj.target_node_ids = h5_data["target_node_id"].value
-        obj.target_node_population = h5_data["target_node_id"].attrs["node_population"].decode('utf-8')
+        obj.source_node_ids = h5_data["source_node_id"][()]
+        obj.source_node_population = to_string(h5_data["source_node_id"].attrs["node_population"])
+        obj.target_node_ids = h5_data["target_node_id"][()]
+        obj.target_node_population = to_string(h5_data["target_node_id"].attrs["node_population"])
 
         obj.edge_groups = []
-        for eg_label in np.unique(h5_data['edge_group_id'].value):
-            mask = h5_data['edge_group_id'].value == eg_label
+        for eg_label in np.unique(h5_data['edge_group_id'][()]):
+            mask = h5_data['edge_group_id'][()] == eg_label
             logger.info("EDGE GROUP {}, size {}".format(eg_label, mask.sum()))
 
             edge_type_array = h5_data['edge_type_id'][mask]
-            edge_group_index = h5_data['edge_group_index'][mask]
+            edge_group_index = h5_data['edge_group_index'][mask].tolist()
             source_ids = obj.source_node_ids[mask]
             target_ids = obj.target_node_ids[mask]
             # note: it may be more efficient in an MPI context
             #       to defer the extraction of source_ids, etc.
 
             obj.edge_groups.append(
                 EdgeGroup.from_data(eg_label,
@@ -885,15 +909,15 @@
         ---------
 
         id : integer
             Taken from the SONATA edges HDF5 file.
         node_types_array : NumPy array
             Subset of the data from "/edges/<population_name>/edge_type_id"
             that applies to this group.
-        index : NumPy array
+        index : list
             Subset of the data from "/edges/<population_name>/edge_group_index"
             that applies to this group.
         h5_data : HDF5 Group
             The "/edges/<population_name>/<group_id>" group.
         edge_types_map : dict
             Data loaded from edge types CSV file. Top-level keys are edge type ids.
         config : dict
@@ -926,19 +950,19 @@
                     parameters[name][edge_type_id] = value
 
         # parameters defined in .h5 files
         if 'dynamics_params' in h5_data:
             dynamics_params_group = h5_data['dynamics_params']
             # not sure the next bit is using `index` correctly
             for key in dynamics_params_group.keys():
-                parameters[key] = dynamics_params_group[key].value[index]
+                parameters[key] = dynamics_params_group[key][index]
         if 'nsyns' in h5_data:
-            parameters['nsyns'] = h5_data['nsyns'].value[index]
+            parameters['nsyns'] = h5_data['nsyns'][index]
         if 'syn_weight' in h5_data:
-            parameters['syn_weight'] = h5_data['syn_weight'].value[index]
+            parameters['syn_weight'] = h5_data['syn_weight'][index]
 
         obj.parameters = parameters
         obj.config = config
         logger.info(parameters)
         return obj
 
     def __repr__(self):
```

### Comparing `PyNN-0.9.5/pyNN/space.py` & `PyNN-0.9.6/pyNN/space.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   Grid3D          - represents a structure with neurons distributed on a 3D grid.
   RandomStructure - represents a structure with neurons distributed randomly
                     within a given volume.
 
   Cuboid          - representation of a cuboidal volume, for use with RandomStructure.
   Sphere          - representation of a spherical volume, for use with RandomStructure.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 # There must be some Python package out there that provides most of this stuff.
 # Distance computations are provided by scipy.spatial, but scipy is a fairly heavy dependency.
 
 try:
```

### Comparing `PyNN-0.9.5/pyNN/standardmodels/__init__.py` & `PyNN-0.9.6/pyNN/standardmodels/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 Classes:
     StandardModelType
     StandardCellType
     ModelNotAvailable
     STDPWeightDependence
     STDPTimingDependence
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from pyNN import errors, models
 from pyNN.parameters import ParameterSpace
 import numpy
 from pyNN.core import is_listlike, itervalues
 from copy import deepcopy
 import neo
 import quantities as pq
 
+
 # ==============================================================================
 #   Standard cells
 # ==============================================================================
 
 
 def build_translations(*translation_list):
     """
@@ -240,33 +241,38 @@
 
 # ==============================================================================
 #   Synapse Dynamics classes
 # ==============================================================================
 
 
 def check_weights(weights, projection):
-    # if projection.post is an Assembly, some components might have cond-synapses, others curr, so need a more sophisticated check here
-    synapse_sign = projection.receptor_type
-    is_conductance = projection.post.conductance_based
+    # if projection.post is an Assembly, some components might have cond-synapses, others curr,
+    # so need a more sophisticated check here. For now, skipping check and emitting a warning
+    if hasattr(projection.post, "_homogeneous_synapses") and not projection.post._homogeneous_synapses:
+        warnings.warn("Not checking weights due to due mixture of synapse types")
     if isinstance(weights, numpy.ndarray):
         all_negative = (weights <= 0).all()
         all_positive = (weights >= 0).all()
         if not (all_negative or all_positive):
             raise errors.ConnectionError("Weights must be either all positive or all negative")
     elif numpy.isreal(weights):
         all_positive = weights >= 0
-        all_negative = weights < 0
+        all_negative = weights <= 0
     else:
         raise errors.ConnectionError("Weights must be a number or an array of numbers.")
-    if is_conductance or synapse_sign == 'excitatory':
+    if projection.post.conductance_based or projection.receptor_type == 'excitatory':
         if not all_positive:
-            raise errors.ConnectionError("Weights must be positive for conductance-based and/or excitatory synapses")
-    elif is_conductance is False and synapse_sign == 'inhibitory':
+            raise errors.ConnectionError(
+                "Weights must be positive for conductance-based and/or excitatory synapses"
+            )
+    elif projection.post.conductance_based is False and projection.receptor_type == 'inhibitory':
         if not all_negative:
-            raise errors.ConnectionError("Weights must be negative for current-based, inhibitory synapses")
+            raise errors.ConnectionError(
+                "Weights must be negative for current-based, inhibitory synapses"
+            )
     else:  # This should never happen.
         raise Exception("Can't check weight, conductance status unknown.")
 
 
 def check_delays(delays, projection):
     min_delay = projection._simulator.state.min_delay
     max_delay = projection._simulator.state.max_delay
@@ -281,15 +287,15 @@
     if not in_range:
         raise errors.ConnectionError("Delay (%s) is out of range [%s, %s]" % (delays, min_delay, max_delay))
 
 
 class StandardSynapseType(StandardModelType, models.BaseSynapseType):
     parameter_checks = {
         'weight': check_weights,
-        'delay': check_delays
+        #'delay': check_delays   # this needs to be revisited in the context of min_delay = "auto"
     }
 
     def get_schema(self):
         """
         Returns the model schema: i.e. a mapping of parameter names to allowed
         parameter types.
         """
```

### Comparing `PyNN-0.9.5/pyNN/standardmodels/cells.py` & `PyNN-0.9.6/pyNN/standardmodels/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     HH_cond_exp
 
 Spike sources (input neurons)
     SpikeSourcePoisson
     SpikeSourceArray
     SpikeSourceInhGamma
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from pyNN.standardmodels import StandardCellType
 from pyNN.parameters import ArrayParameter, Sequence
 
 
@@ -321,21 +321,25 @@
         'e_rev_K':    -90.0,
         'e_rev_leak': -65.0,
         'e_rev_E':      0.0,
         'e_rev_I':    -80.0,
         'tau_syn_E':    0.2,   # ms
         'tau_syn_I':    2.0,
         'i_offset':     0.0,   # nA
+
     }
     recordable = ['spikes', 'v', 'gsyn_exc', 'gsyn_inh']
     receptor_types = ('excitatory', 'inhibitory', 'source_section.gap')
     default_initial_values = {
         'v': -65.0,  # 'v_rest',
         'gsyn_exc': 0.0,
         'gsyn_inh': 0.0,
+        'h': 1.0,
+        'm': 0.0,
+        'n': 0.0,
     }
     units = {
         'v': 'mV',
         'gsyn_exc': 'uS',
         'gsyn_inh': 'uS',
         'gbar_Na': 'uS',
         'gbar_K': 'uS',
@@ -346,14 +350,17 @@
         'e_rev_K': 'mV',
         'e_rev_leak': 'mV',
         'e_rev_E': 'mV',
         'e_rev_I': 'mV',
         'tau_syn_E': 'ms',
         'tau_syn_I': 'ms',
         'i_offset': 'nA',
+        'h': '',
+        'm': '',
+        'n': '',
     }
 
 
 class EIF_cond_alpha_isfa_ista(StandardCellType):
     """
     Exponential integrate and fire neuron with spike triggered and
     sub-threshold adaptation currents (isfa, ista reps.) according to:
```

### Comparing `PyNN-0.9.5/pyNN/standardmodels/electrodes.py` & `PyNN-0.9.6/pyNN/standardmodels/electrodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Definition of default parameters (and hence, standard parameter names) for
 standard current source models.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from pyNN.standardmodels import StandardCurrentSource
 from pyNN.parameters import Sequence
```

### Comparing `PyNN-0.9.5/pyNN/standardmodels/synapses.py` & `PyNN-0.9.6/pyNN/standardmodels/synapses.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Classes for defining STDP rules:
     AdditiveWeightDependence
     MultiplicativeWeightDependence
     AdditivePotentiationMultiplicativeDepression
     GutigWeightDependence
     SpikePairRule
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     long
 except NameError:
     long = int
@@ -36,15 +36,15 @@
     }
 
 
 class ElectricalSynapse(StandardSynapseType):
     """
     A bidirectional electrical synapse (gap junction) with fixed conductance
     """
-       
+
     default_parameters = {
         'weight': 0.0  # the (bidirectional) conductance of the gap junction (uS)
     }
 
 
 class TsodyksMarkramSynapse(StandardSynapseType):
     """
@@ -60,15 +60,15 @@
     Arguments:
         `U`:
             use parameter.
         `tau_rec`:
             depression time constant (ms).
         `tau_facil`:
             facilitation time constant (ms).
-    
+
     .. _`Tsodyks, Uziel and Markram (2000)`: http://www.jneurosci.org/content/20/1/RC50.long
     """
     default_parameters = {
         'weight':     0.0,
         'delay':     None,
         'U':          0.5,  # use parameter
         'tau_rec':  100.0,  # depression time constant (ms)
@@ -172,15 +172,15 @@
         self.timing_dependence = timing_dependence
         self.weight_dependence = weight_dependence
         self.voltage_dependence = voltage_dependence
         self.dendritic_delay_fraction = dendritic_delay_fraction
         self.weight = weight
         self.delay = delay or self._get_minimum_delay()
         self._build_translations()
-        
+
     def _build_translations(self):
         self.translations = self.__class__.base_translations  # weight and delay
         for component in (self.timing_dependence, self.weight_dependence, self.voltage_dependence):
             if component:
                 self.translations.update(component.translations)
 
     @property
@@ -414,25 +414,25 @@
         parameters = dict(locals())
         parameters.pop('self')
         STDPTimingDependence.__init__(self, **parameters)
 
 
 class Vogels2011Rule(STDPTimingDependence):
     """
-    Timing-dependence rule from 
+    Timing-dependence rule from
 
       Vogels TP, Sprekeler H, Zenke F, Clopath C, Gerstner W (2011)
       Inhibitory plasticity balances excitation and inhibition in sensory
       pathways and memory networks. Science 334:1569-73
       http://dx.doi.org/10.1126/science.1211095
-  
+
     Potentiation depends on the coincidence of pre- and post-synaptic spikes
     but not on their order. Pre-synaptic spikes in the absence of post-
     synaptic ones produce depression.
-    
+
     Also see http://senselab.med.yale.edu/modeldb/ShowModel.asp?model=143751
     """
 
     default_parameters = {
         'tau': 20.0,
         'eta': 1e-10,
         'rho': 3.0
```

### Comparing `PyNN-0.9.5/pyNN/utility/__init__.py` & `PyNN-0.9.6/pyNN/utility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                         it was run (python, nrniv, mpirun, etc.).
     init_logging()    - convenience function for setting up logging to file and
                         to the screen.
 
     Timer    - a convenience wrapper around the time.time() function from the
                standard library.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from __future__ import print_function, division
 # If there is a settings.py file on the path, defaults will be
 # taken from there.
@@ -33,15 +33,15 @@
 import logging
 import time
 import os
 from datetime import datetime
 import functools
 import numpy
 from importlib import import_module
-    
+
 from pyNN.core import deprecated
 
 
 def notify(msg="Simulation finished.", subject="Simulation finished.",
            smtphost=SMTPHOST, address=EMAIL):
     """Send an e-mail stating that the simulation has finished."""
     if not (smtphost and address):
@@ -84,20 +84,20 @@
     return args
 
 
 def get_simulator(*arguments):
     """
     Import and return a PyNN simulator backend module based on command-line
     arguments.
-    
+
     The simulator name should be the first positional argument. If your script
     needs additional arguments, you can specify them as (name, help_text) tuples.
     If you need more complex argument handling, you should use argparse
     directly.
-    
+
     Returns (simulator, command-line arguments)
     """
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument("simulator",
                         help="neuron, nest, brian or another backend simulator")
     for argument in arguments:
@@ -185,33 +185,41 @@
     # set the variables
     for variable, value in s['variables'].items():
         setattr(population, variable, value)
     s.close()
     return population
 
 
-def normalized_filename(root, basename, extension, simulator, num_processes=None):
+def normalized_filename(root, basename, extension, simulator, num_processes=None, use_iso8601=False):
     """
     Generate a file path containing a timestamp and information about the
     simulator used and the number of MPI processes.
-    
+
     The date is used as a sub-directory name, the date & time are included in the
     filename.
+    If use_iso8601 is True, follow https://en.wikipedia.org/wiki/ISO_8601
     """
     timestamp = datetime.now()
+    if use_iso8601:
+        date = timestamp.strftime("%Y-%m-%d")
+        date_time = timestamp.strftime("%Y-%m-%dT%H:%M:%S")
+    else:
+        date = timestamp.strftime("%Y%m%d")
+        date_time = timestamp.strftime("%Y%m%d-%H%M%S")
+
     if num_processes:
         np = "_np%d" % num_processes
     else:
         np = ""
     return os.path.join(root,
-                        timestamp.strftime("%Y%m%d"),
+                        date,
                         "%s_%s%s_%s.%s" % (basename,
                                            simulator,
                                            np,
-                                           timestamp.strftime("%Y%m%d-%H%M%S"),
+                                           date_time,
                                            extension))
 
 
 def connection_plot(projection, positive='O', zero='.', empty=' ', spacer=''):
     """ """
     connection_array = projection.get('weight', format='array')
     image = numpy.zeros_like(connection_array, dtype=unicode)
@@ -405,15 +413,14 @@
 
     def __init__(self, func):
         self.func = func
         self.cached_args = None
         self.cached_value = None
 
     def __call__(self, *args):
-        import pdb; pdb.set_trace()
         if args == self.cached_args:
             print("using cached value")
             return self.cached_value
         else:
             #print("calculating value")
             value = self.func(*args)
             self.cached_args = args
```

### Comparing `PyNN-0.9.5/pyNN/utility/plotting.py` & `PyNN-0.9.6/pyNN/utility/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Simple tools for plotting Neo-format data.
 
 These tools are intended for quickly producing basic plots with simple
 formatting. If you need to produce more complex and/or publication-quality
 figures, it will probably be easier to use matplotlib or another plotting
 package directly rather than trying to extend this module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 
 """
 
 from collections import defaultdict
 from numbers import Number
 from itertools import repeat
```

### Comparing `PyNN-0.9.5/setup.py` & `PyNN-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,22 @@
                 cmd = abs_name
                 break
         return cmd
 
 
 setup(
     name="PyNN",
-    version="0.9.5",
+    version="0.9.6",
     packages=['pyNN', 'pyNN.nest', 'pyNN.neuron',
-                'pyNN.brian', 'pyNN.common', 'pyNN.mock', 'pyNN.neuroml',
-                'pyNN.recording', 'pyNN.standardmodels', 'pyNN.descriptions',
-                'pyNN.nest.standardmodels', 'pyNN.neuroml.standardmodels',
-                'pyNN.neuron.standardmodels', 'pyNN.brian.standardmodels',
-                'pyNN.utility', 'pyNN.nineml', 'pyNN.serialization'],
+              'pyNN.brian', 'pyNN.brian2', 'pyNN.common', 'pyNN.mock', 'pyNN.neuroml',
+              'pyNN.recording', 'pyNN.standardmodels', 'pyNN.descriptions',
+              'pyNN.nest.standardmodels', 'pyNN.neuroml.standardmodels',
+              'pyNN.neuron.standardmodels', 'pyNN.brian.standardmodels',
+              'pyNN.brian2.standardmodels', 'pyNN.utility', 'pyNN.nineml',
+              'pyNN.serialization'],
     package_data={'pyNN': ['neuron/nmodl/*.mod',
                            'nest/extensions/*.h',
                            'nest/extensions/*.cpp',
                            'nest/extensions/CMakeLists.txt',
                            'nest/extensions/sli/*.sli',
                            "descriptions/templates/*/*"]},
     author="The PyNN team",
@@ -112,22 +113,20 @@
                  'Intended Audience :: Science/Research',
                  'License :: Other/Proprietary License',
                  'Natural Language :: English',
                  'Operating System :: OS Independent',
                  'Programming Language :: Python :: 2',
                  'Programming Language :: Python :: 2.7',
                  'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
                  'Programming Language :: Python :: 3.6',
                  'Programming Language :: Python :: 3.7',
+                 'Programming Language :: Python :: 3.8',
                  'Topic :: Scientific/Engineering'],
     cmdclass={'build_py': build},
-    install_requires=['numpy>=1.8.2', 'lazyarray>=0.3.2', 'neo>=0.5.2',
+    install_requires=['numpy>=1.13.0', 'lazyarray>=0.3.4', 'neo>=0.8.0',
                       'quantities>=0.12.1'],
     extras_require={
         'examples': ['matplotlib', 'scipy'],
         'plotting': ['matplotlib', 'scipy'],
         'MPI': ['mpi4py'],
         'sonata': ['h5py']
     },
```

### Comparing `PyNN-0.9.5/test/benchmarks/Benchmark_PyNN-0.8dev_FixedNumberPost.py` & `PyNN-0.9.6/test/benchmarks/Benchmark_PyNN-0.8dev_FixedNumberPost.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,18 @@
 noise_ie_prj.set(weight=w_noise_inh)
 noise_ii_prj.set(weight=w_noise_inh)
 times['t_connect_noise'] = timer.diff()
 
 
 # === Setup recording ==========================================================
 print("%s Setting up recording..." % node_id)
-exc_cells.record()
-inh_cells.record()
+exc_cells.record('spikes')
+inh_cells.record('spikes')
 cells_to_record = range(n_cells_to_record)
-exc_cells[cells_to_record].record_v()
+exc_cells[list(cells_to_record)].record_v()
 times['t_record'] = timer.diff()
 
 
 print("%d Print(exc spikes to file..." % node_id)
 if not(os.path.isdir(folder_name)) and (rank() == 0):
     os.mkdir(folder_name)
 
@@ -158,21 +158,21 @@
 # === Run simulation ===========================================================
 print("%d Running simulation..." % node_id)
 run(t_sim)
 times['t_run'] = timer.diff()
 
 
 # === Print(results to file ====================================================
-exc_spike_fn = "%s/VAbenchmark_%s_exc_%s_np%d_%d.ras" % (folder_name, benchmark, simulator_name, np, node_id)
+exc_spike_fn = "%s/VAbenchmark_%s_exc_%s_np%d_%d.pkl" % (folder_name, benchmark, simulator_name, np, node_id)
 exc_cells.printSpikes(exc_spike_fn, gather=gather)
 print("%d Print(inh spikes to file..." % node_id)
-inh_spike_fn = "%s/VAbenchmark_%s_inh_%s_np%d_%d.ras" % (folder_name, benchmark, simulator_name, np, node_id)
+inh_spike_fn = "%s/VAbenchmark_%s_inh_%s_np%d_%d.pkl" % (folder_name, benchmark, simulator_name, np, node_id)
 inh_cells.printSpikes(inh_spike_fn, gather=gather)
 print("%d Print(voltage to file..." % node_id)
-exc_cells[cells_to_record].print_v("%s/VAbenchmark_%s_exc_%s_np%d_%d.v" % (folder_name, benchmark, simulator_name, np, node_id), gather=gather)
+exc_cells[list(cells_to_record)].print_v("%s/VAbenchmark_%s_exc_%s_np%d_%d.pkl" % (folder_name, benchmark, simulator_name, np, node_id), gather=gather)
 times['t_printSpikes'] = timer.diff()
 
 # === Load spike file and calculate conductances ====================
 #exc_spikes = np.loadtxt(exc_spike_fn)
 #E_count = exc_cells.meanSpikeCount()
 #I_count = inh_cells.meanSpikeCount()
 #f_exc = E_count*1000.0/t_sim
```

### Comparing `PyNN-0.9.5/test/benchmarks/README.txt` & `PyNN-0.9.6/test/benchmarks/README.txt`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/benchmarks/all_to_all_network.param` & `PyNN-0.9.6/test/benchmarks/all_to_all_network.param`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/benchmarks/connectors_benchmark.py` & `PyNN-0.9.6/test/benchmarks/connectors_benchmark.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/benchmarks/ddpc.py` & `PyNN-0.9.6/test/benchmarks/ddpc.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/benchmarks/plot_figure.py` & `PyNN-0.9.6/test/benchmarks/plot_figure.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/benchmarks/simple_network.py` & `PyNN-0.9.6/test/benchmarks/simple_network.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/hardware/unittests/mocks.py` & `PyNN-0.9.6/test/unittests/mocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Mock classes for unit tests
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from pyNN import random
 import numpy
 
 
@@ -51,7 +51,26 @@
     def _next(self, distribution, n, parameters):
         x = self.numbers[self.i:self.i + n]
         self.i += n
         return x
 
     def permutation(self, arr):
         return arr[::-1]
+
+
+class MockRNG3(random.WrappedRNG):
+    """
+    returns [1, 0, 0, 0,..]
+    """
+    rng = None
+
+    def __init__(self, parallel_safe=True):
+        random.WrappedRNG.__init__(self, parallel_safe=parallel_safe)
+
+    def _next(self, distribution, n, parameters):
+        x = numpy.zeros(n)
+        x.dtype = int
+        x[0] = 1
+        return x
+
+    def permutation(self, arr):
+        return arr[::-1]
```

### Comparing `PyNN-0.9.5/test/hardware/unittests/test_connectors.py` & `PyNN-0.9.6/test/unittests/test_connectors_parallel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,78 @@
 """
 Tests of the Connector classes, using the pyNN.mock backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 from pyNN import connectors, random, errors, space, recording
 import numpy
 import os
+import sys
 from numpy.testing import assert_array_equal, assert_array_almost_equal
 from .mocks import MockRNG, MockRNG2
 import pyNN.mock as sim
 
+
 orig_mpi_get_config = random.get_mpi_config
 
 
 def setUp():
     random.get_mpi_config = lambda: (0, 2)
 
 
 def tearDown():
     random.get_mpi_config = orig_mpi_get_config
 
 
 class TestOneToOneConnector(unittest.TestCase):
 
-    def setUp(self):
-        sim.setup(num_processes=2, rank=0)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(num_processes=2, rank=0, **extra)
         self.p1 = sim.Population(5, sim.IF_cond_exp())
         self.p2 = sim.Population(5, sim.HH_cond_exp())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_connect_with_scalar_weights_and_delays(self):
+    def tearDown(self, sim=sim):
+        sim.end()
+
+    def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         C = connectors.OneToOneConnector(safe=False)
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(1, 1, 5.0, 0.5),
                           (3, 3, 5.0, 0.5)])
 
-    def test_connect_with_random_weights(self):
+    def test_connect_with_random_weights(self, sim=sim):
         rd = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(delta=1.0))
         syn = sim.StaticSynapse(weight=rd, delay=0.5)
         C = connectors.OneToOneConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(1, 1, 1.0, 0.5),
                           (3, 3, 3.0, 0.5)])
 
 
 class TestAllToAllConnector(unittest.TestCase):
 
-    def setUp(self):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p1._mask_local, numpy.array([0, 1, 0, 1], dtype=bool))
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_connect_with_scalar_weights_and_delays(self):
+    def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         C = connectors.AllToAllConnector(safe=False)
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 5.0, 0.5),
                           (1, 1, 5.0, 0.5),
                           (2, 1, 5.0, 0.5),
@@ -79,20 +84,21 @@
         nan = numpy.nan
         assert_array_equal(prj.get('weight', format='array', gather=False),
                            numpy.array([[nan, 5.0, nan, 5.0, nan],
                                         [nan, 5.0, nan, 5.0, nan],
                                         [nan, 5.0, nan, 5.0, nan],
                                         [nan, 5.0, nan, 5.0, nan]]))
 
-    def test_connect_with_array_weights(self):
+    def test_connect_with_array_weights(self, sim=sim):
         C = connectors.AllToAllConnector(safe=False)
         syn = sim.StaticSynapse(weight=numpy.arange(0.0, 2.0, 0.1).reshape(4, 5), delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         assert_array_almost_equal(
-            numpy.array(prj.get(["weight", "delay"], format='list', gather=False)),  # use gather False because we are faking the MPI
+            # use gather False because we are faking the MPI
+            numpy.array(prj.get(["weight", "delay"], format='list', gather=False)),
             numpy.array([(0, 1, 0.1, 0.5),
                          (1, 1, 0.6, 0.5),
                          (2, 1, 1.1, 0.5),
                          (3, 1, 1.6, 0.5),
                          (0, 3, 0.3, 0.5),
                          (1, 3, 0.8, 0.5),
                          (2, 3, 1.3, 0.5),
@@ -101,16 +107,17 @@
         assert_array_almost_equal(prj.get('weight', format='array', gather=False),
                                   numpy.array([[nan, 0.1, nan, 0.3, nan],
                                                [nan, 0.6, nan, 0.8, nan],
                                                [nan, 1.1, nan, 1.3, nan],
                                                [nan, 1.6, nan, 1.8, nan]]),
                                   9)
 
-    def test_connect_with_random_weights_parallel_safe(self):
-        rd = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(delta=1.0, parallel_safe=True))
+    def test_connect_with_random_weights_parallel_safe(self, sim=sim):
+        rd = random.RandomDistribution(
+            'uniform', (0, 1), rng=MockRNG(delta=1.0, parallel_safe=True))
         syn = sim.StaticSynapse(weight=rd, delay=0.5)
         C = connectors.AllToAllConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         # note that the outer loop is over the post-synaptic cells, the inner loop over the pre-synaptic
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 4.0, 0.5),
                           (1, 1, 5.0, 0.5),
@@ -124,90 +131,91 @@
         assert_array_almost_equal(prj.get('weight', format='array', gather=False),
                                   numpy.array([[nan, 4.0, nan, 12.0, nan],
                                                [nan, 5.0, nan, 13.0, nan],
                                                [nan, 6.0, nan, 14.0, nan],
                                                [nan, 7.0, nan, 15.0, nan]]),
                                   9)
 
-    def test_connect_with_distance_dependent_weights(self):
+    def test_connect_with_distance_dependent_weights(self, sim=sim):
         d_expr = "d+100"
         syn = sim.StaticSynapse(weight=d_expr, delay=0.5)
         C = connectors.AllToAllConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 101.0, 0.5),
                           (1, 1, 100.0, 0.5),
                           (2, 1, 101.0, 0.5),
                           (3, 1, 102.0, 0.5),
                           (0, 3, 103.0, 0.5),
                           (1, 3, 102.0, 0.5),
                           (2, 3, 101.0, 0.5),
                           (3, 3, 100.0, 0.5)])
 
-    def test_connect_with_distance_dependent_weights_and_delays(self):
+    def test_connect_with_distance_dependent_weights_and_delays(self, sim=sim):
         syn = sim.StaticSynapse(weight="d+100", delay="0.2+2*d")
         C = connectors.AllToAllConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 101.0, 2.2),
                           (1, 1, 100.0, 0.2),
                           (2, 1, 101.0, 2.2),
                           (3, 1, 102.0, 4.2),
                           (0, 3, 103.0, 6.2),
                           (1, 3, 102.0, 4.2),
                           (2, 3, 101.0, 2.2),
                           (3, 3, 100.0, 0.2)])
 
-    def test_connect_with_delays_None(self):
+    def test_connect_with_delays_None(self, sim=sim):
         syn = sim.StaticSynapse(weight=0.1, delay=None)
         C = connectors.AllToAllConnector()
         assert C.safe
         assert C.allow_self_connections
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False)[0][3], prj._simulator.state.min_delay)
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False)[
+                         0][3], prj._simulator.state.min_delay)
 
-    @unittest.skip('skipping this tests until I figure out how I want to refactor checks')
-    def test_connect_with_delays_too_small(self):
-        C = connectors.AllToAllConnector()
+    @unittest.skip('skipping this test until refactoring of delay checks is complete')
+    def test_connect_with_delays_too_small(self, sim=sim):
+        C = connectors.AllToAllConnector(safe=True)
         syn = sim.StaticSynapse(weight=0.1, delay=0.0)
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, self.p2, C, syn)
 
-    @unittest.skip('skipping this tests until I figure out how I want to refactor checks')
-    def test_connect_with_list_delays_too_small(self):
+    @unittest.skip('skipping this tests until refactoring of delay checks is complete')
+    def test_connect_with_list_delays_too_small(self, sim=sim):
         delays = numpy.ones((self.p1.size, self.p2.size), float)
         delays[2, 3] = sim.Projection._simulator.state.min_delay - 0.01
         syn = sim.StaticSynapse(weight=0.1, delay=delays)
         C = connectors.AllToAllConnector()
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, self.p2, C, syn)
 
 
 class TestFixedProbabilityConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_connect_with_default_args(self):
+    def test_connect_with_default_args(self, sim=sim):
         C = connectors.FixedProbabilityConnector(p_connect=0.85,
                                                  rng=MockRNG(delta=0.1, parallel_safe=True))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
 
         # 20 possible connections. Due to the mock RNG, only the
         # first 9 are created (0,0), (1,0), (2,0), (3,0), (0,1), (1,1), (2,1), (3,1), (0,2)
         # of these, (0,1), (1,1), (2,1), (3,1) are created on this node
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123)])
 
-    def test_connect_with_default_args_again(self):
+    def test_connect_with_default_args_again(self, sim=sim):
         C = connectors.FixedProbabilityConnector(p_connect=0.5,
                                                  rng=MockRNG2(1 - numpy.array([1, 0, 0, 1,
                                                                                0, 0, 0, 1,
                                                                                1, 1, 0, 0,
                                                                                1, 0, 1, 0,
                                                                                1, 1, 0, 1]),
                                                               parallel_safe=True))
@@ -226,27 +234,47 @@
                                                [nan, 0.123, nan, nan,   nan]]),
                                   9)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(3, 1, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123)])
 
-    def test_connect_with_weight_function(self):
+    def test_connect_with_probability_1(self, sim=sim):
+        # see https://github.com/NeuralEnsemble/PyNN/issues/309
+        C = connectors.FixedProbabilityConnector(p_connect=1,
+                                                 rng=MockRNG(delta=0.01, parallel_safe=True))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+
+        # 20 connections, only some of which are created on this node
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(0, 1, 0.0, 0.123),
+                          (1, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
+                          (3, 3, 0.0, 0.123)
+                          ])
+
+    def test_connect_with_weight_function(self, sim=sim):
         C = connectors.FixedProbabilityConnector(p_connect=0.85,
                                                  rng=MockRNG(delta=0.1))
         syn = sim.StaticSynapse(weight=lambda d: 0.1 * d)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.1, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.1, 0.123),
                           (3, 1, 0.2, 0.123)])
 
-    def test_connect_with_random_delays_parallel_safe(self):
-        rd = random.RandomDistribution('uniform', low=0.1, high=1.1, rng=MockRNG(start=1.0, delta=0.2, parallel_safe=True))
+    def test_connect_with_random_delays_parallel_safe(self, sim=sim):
+        rd = random.RandomDistribution('uniform', low=0.1, high=1.1,
+                                       rng=MockRNG(start=1.0, delta=0.2, parallel_safe=True))
         syn = sim.StaticSynapse(delay=rd)
         C = connectors.FixedProbabilityConnector(p_connect=0.5,
                                                  rng=MockRNG2(1 - numpy.array([1, 0, 0, 1,
                                                                                0, 0, 0, 1,
                                                                                1, 1, 0, 0,
                                                                                1, 0, 1, 0,
                                                                                1, 1, 0, 1]),
@@ -256,15 +284,15 @@
         assert_array_almost_equal(prj.get('delay', format='array', gather=False),
                                   numpy.array([[nan, nan, nan, 2.0, nan],
                                                [nan, nan, nan, nan, nan],
                                                [nan, nan, nan, 2.2, nan],
                                                [nan, 1.4, nan, nan, nan]]),
                                   9)
 
-    #def test_connect_with_random_delays_parallel_unsafe(self):
+    # def test_connect_with_random_delays_parallel_unsafe(self, sim=sim):
     #    rd = random.RandomDistribution('uniform', [0.1, 1.1], rng=MockRNG(start=1.0, delta=0.2, parallel_safe=False))
     #    syn = sim.StaticSynapse(delay=rd)
     #    C = connectors.FixedProbabilityConnector(p_connect=0.5,
     #                                             rng=MockRNG2(1 - numpy.array([1, 0, 0, 1,
     #                                                                           0, 0, 0, 1,
     #                                                                           1, 1, 0, 0,
     #                                                                           1, 0, 1, 0,
@@ -278,21 +306,21 @@
     #                                           [nan, nan, nan, 1.4, nan],
     #                                           [nan, 1.0, nan, nan, nan]]),
     #                              9)
 
 
 class TestDistanceDependentProbabilityConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_connect_with_default_args(self):
+    def test_connect_with_default_args(self, sim=sim):
         C = connectors.DistanceDependentProbabilityConnector(d_expression="d<1.5",
                                                              rng=MockRNG(delta=0.01))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         # 20 possible connections. Only those with a sufficiently small distance
         # are created
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
@@ -301,160 +329,274 @@
                           (2, 1, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
                           (3, 3, 0.0, 0.123)])
 
 
 class TestFromListConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_connect_with_valid_list(self):
+    def test_connect_with_valid_list(self, sim=sim):
         connection_list = [
             (0, 0, 0.1, 0.1),
             (3, 0, 0.2, 0.11),
             (2, 3, 0.3, 0.12),  # local
             (2, 2, 0.4, 0.13),
             (0, 1, 0.5, 0.14),  # local
-            ]
+        ]
         C = connectors.FromListConnector(connection_list)
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.5, 0.14),
                           (2, 3, 0.3, 0.12)])
 
-    def test_connect_with_out_of_range_index(self):
+    def test_connect_with_out_of_range_index(self, sim=sim):
         connection_list = [
             (0, 0, 0.1, 0.1),
             (3, 0, 0.2, 0.11),
             (2, 3, 0.3, 0.12),  # local
             (5, 1, 0.4, 0.13),  # NON-EXISTENT
             (0, 1, 0.5, 0.14),  # local
-            ]
+        ]
         C = connectors.FromListConnector(connection_list)
         syn = sim.StaticSynapse()
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, self.p2, C, syn)
 
-    def test_with_plastic_synapse(self):
+    def test_with_plastic_synapse(self, sim=sim):
         connection_list = [
             (0, 0, 0.1, 0.1, 100, 400),
             (3, 0, 0.2, 0.11, 101, 500),
             (2, 3, 0.3, 0.12, 102, 600),  # local
             (2, 2, 0.4, 0.13, 103, 700),
             (0, 1, 0.5, 0.14, 104, 800),  # local
-            ]
-        C = connectors.FromListConnector(connection_list, column_names=["weight", "delay", "U", "tau_rec"])
+        ]
+        C = connectors.FromListConnector(connection_list, column_names=[
+                                         "weight", "delay", "U", "tau_rec"])
         syn = sim.TsodyksMarkramSynapse(U=99, tau_facil=88.8)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay", "tau_facil", "tau_rec", "U"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.5, 0.14, 88.8, 800.0, 104.0),
                           (2, 3, 0.3, 0.12, 88.8, 600.0, 102.0)])
 
+    def test_with_stdp_synapse(self, sim=sim):
+        connection_list = [
+            (0, 0, 0.1, 0.1, 10.0, 0.4),
+            (3, 0, 0.2, 0.11, 10.1, 0.5),
+            (2, 3, 0.3, 0.12, 10.2, 0.6),  # local
+            (2, 2, 0.4, 0.13, 10.3, 0.7),
+            (0, 1, 0.5, 0.14, 10.4, 0.8),  # local
+        ]
+        C = connectors.FromListConnector(connection_list, column_names=[
+                                         "weight", "delay", "tau_plus", "w_max"])
+        syn = sim.STDPMechanism(timing_dependence=sim.SpikePairRule(tau_plus=12.3, tau_minus=33.3),
+                                weight_dependence=sim.MultiplicativeWeightDependence(w_max=1.11),
+                                weight=0.321, delay=0.2)
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        self.assertEqual(prj.get(["weight", "delay", "tau_plus", "tau_minus", "w_max"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(0, 1, 0.5, 0.14, 10.4, 33.3, 0.8),
+                          (2, 3, 0.3, 0.12, 10.2, 33.3, 0.6)])
+
 
 class TestFromFileConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
         self.connection_list = [
             (0, 0, 0.1, 0.1),
             (3, 0, 0.2, 0.11),
             (2, 3, 0.3, 0.12),  # local
             (2, 2, 0.4, 0.13),
             (0, 1, 0.5, 0.14),  # local
-            ]
+        ]
 
-    def tearDown(self):
+    def tearDown(self, sim=sim):
         for path in ("test.connections", "test.connections.1", "test.connections.2"):
             if os.path.exists(path):
                 os.remove(path)
 
-    def test_connect_with_standard_text_file_not_distributed(self):
+    def test_connect_with_standard_text_file_not_distributed(self, sim=sim):
         numpy.savetxt("test.connections", self.connection_list)
         C = connectors.FromFileConnector("test.connections", distributed=False)
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.5, 0.14),
                           (2, 3, 0.3, 0.12)])
 
-    def test_connect_with_standard_text_file_distributed(self):
+    def test_connect_with_standard_text_file_distributed(self, sim=sim):
         local_connection_list = [c for c in self.connection_list if c[1] % 2 == 1]
         numpy.savetxt("test.connections.1", local_connection_list)
         C = connectors.FromFileConnector("test.connections", distributed=True)
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.5, 0.14),
                           (2, 3, 0.3, 0.12)])
 
-    def test_with_plastic_synapses_not_distributed(self):
+    def test_with_plastic_synapses_not_distributed(self, sim=sim):
         connection_list = [
             (0, 0, 0.1, 0.1,  100, 100),
             (3, 0, 0.2, 0.11, 110, 99),
             (2, 3, 0.3, 0.12, 120, 98),  # local
             (2, 2, 0.4, 0.13, 130, 97),
             (0, 1, 0.5, 0.14, 140, 96),  # local
-            ]
+        ]
         file = recording.files.StandardTextFile("test.connections.2", mode='wb')
         file.write(connection_list, {"columns": ["i", "j", "weight", "delay", "U", "tau_rec"]})
         C = connectors.FromFileConnector("test.connections.2", distributed=False)
         syn = sim.TsodyksMarkramSynapse(tau_facil=88.8)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay", "U", "tau_rec", "tau_facil"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.5, 0.14, 140.0, 96.0, 88.8),
                           (2, 3, 0.3, 0.12, 120.0, 98.0, 88.8)])
 
 
-#class TestFixedNumberPostConnector(unittest.TestCase):
-#
-#    def setUp(self):
-#        sim.setup(num_processes=2, rank=1, min_delay=0.123)
-#        self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
-#        self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-#        assert_array_equal(self.p2._mask_local, numpy.array([0,1,0,1,0], dtype=bool))
-#
-#    def test_with_n_smaller_than_population_size(self):
-#        C = connectors.FixedNumberPostConnector(n=3, rng=MockRNG(delta=1))
-#        syn = sim.StaticSynapse()
-#        prj = sim.Projection(self.p1, self.p2, C, syn)
-#        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-#                         [(0, 3, 0.0, 0.123),
-#                          (1, 3, 0.0, 0.123),
-#                          (2, 3, 0.0, 0.123),
-#                          (3, 3, 0.0, 0.123),])
+class TestFixedNumberPostConnector(unittest.TestCase):
+
+    def setUp(self, sim=sim):
+        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+        self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
+        self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
+        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+
+    def test_with_n_smaller_than_population_size(self, sim=sim):
+        C = connectors.FixedNumberPostConnector(n=3, rng=MockRNG(delta=1))
+        syn = sim.StaticSynapse(weight="0.5*d")
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        # MockRNG.permutation(arr) returns the reverse of arr, so each pre neuron will connect to neurons 4, 3, 2
+        # however, only neuron 3 is on the "local" (fake MPI) node
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(0, 3, 1.5, 0.123),
+                          (1, 3, 1.0, 0.123),
+                          (2, 3, 0.5, 0.123),
+                          (3, 3, 0.0, 0.123)])
+
+    def test_with_n_larger_than_population_size(self, sim=sim):
+        C = connectors.FixedNumberPostConnector(n=7, rng=MockRNG(delta=1))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        # each pre neuron will connect to all post neurons (population size 5 is less than n), then to 4, 3 (MockRNG.permutation)
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(0, 1, 0.0, 0.123),
+                          (1, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
+                          (3, 3, 0.0, 0.123),
+                          (3, 3, 0.0, 0.123)])
+
+    def test_with_n_larger_than_population_size_no_self_connections(self, sim=sim):
+        C = connectors.FixedNumberPostConnector(
+            n=7, allow_self_connections=False, rng=MockRNG(delta=1))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p2, self.p2, C, syn)
+        # connections as follows: (pre - list of post)
+        #   0 - 1 2 3 4 4 3 2
+        #   1 - 0 2 3 4 4 3 2
+        #   2 - 0 1 3 4 4 3 1
+        #   3 - 0 1 2 4 4 2 1
+        #   4 - 0 1 2 3 3 2 1
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(0, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (4, 1, 0.0, 0.123),
+                          (4, 1, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
+                          (4, 3, 0.0, 0.123),
+                          (4, 3, 0.0, 0.123), ])
+
+    def test_with_replacement(self, sim=sim):
+        C = connectors.FixedNumberPostConnector(n=3, with_replacement=True, rng=MockRNG(delta=1))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        # 0 - 0 1 2
+        # 1 - 3 4 0
+        # 2 - 1 2 3
+        # 3 - 4 0 1
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(0, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123)])
+
+    def test_with_replacement_with_variable_n(self, sim=sim):
+        n = random.RandomDistribution('binomial', (5, 0.5), rng=MockRNG(start=1, delta=2))
+        # should give (1, 3, 0, 2)
+        C = connectors.FixedNumberPostConnector(n=n, with_replacement=True, rng=MockRNG(delta=1))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        # 0 - 0
+        # 1 - 1 2 3
+        # 2 -
+        # 3 - 4 0
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(1, 1, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123)])
+
+    def test_with_replacement_no_self_connections(self, sim=sim):
+        C = connectors.FixedNumberPostConnector(n=3, with_replacement=True,
+                                                allow_self_connections=False, rng=MockRNG(start=2, delta=1))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p2, self.p2, C, syn)
+        # 0 - 2 3 4
+        # 1 - 0 2 3
+        # 2 - 4 0 1
+        # 3 - 2 4 0
+        # 4 - 1 2 3
+        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+                         [(2, 1, 0.0, 0.123),
+                          (4, 1, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (4, 3, 0.0, 0.123)])
 
 
 class TestFixedNumberPreConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_with_n_smaller_than_population_size(self):
+    def test_with_n_smaller_than_population_size(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse(weight="0.1*d")
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(3, 1, 0.2, 0.123),
                           (2, 1, 0.1, 0.123),
                           (1, 1, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (2, 3, 0.1, 0.123),
-                          (1, 3, 0.2, 0.123),])
+                          (1, 3, 0.2, 0.123), ])
 
-    def test_with_n_larger_than_population_size(self):
+    def test_with_n_larger_than_population_size(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=7, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
@@ -464,18 +606,19 @@
                           (1, 1, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
                           (1, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),])
+                          (1, 3, 0.0, 0.123), ])
 
-    def test_with_n_larger_than_population_size_no_self_connections(self):
-        C = connectors.FixedNumberPreConnector(n=7, allow_self_connections=False, rng=MockRNG(delta=1))
+    def test_with_n_larger_than_population_size_no_self_connections(self, sim=sim):
+        C = connectors.FixedNumberPreConnector(
+            n=7, allow_self_connections=False, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p2, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (4, 1, 0.0, 0.123),
@@ -484,187 +627,191 @@
                           (2, 1, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
                           (1, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
                           (4, 3, 0.0, 0.123),
                           (4, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),])
+                          (1, 3, 0.0, 0.123), ])
 
-    def test_with_replacement(self):
+    def test_with_replacement(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, with_replacement=True, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [#(0, 0, 0.0, 0.123),
-                          #(1, 0, 0.0, 0.123),
-                          #(2, 0, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (0, 1, 0.0, 0.123),
-                          (1, 1, 0.0, 0.123),
-                          #(2, 2, 0.0, 0.123),
-                          #(3, 2, 0.0, 0.123),
-                          #(0, 2, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123),
-                          (3, 3, 0.0, 0.123),])
+                         [  # (0, 0, 0.0, 0.123),
+            #(1, 0, 0.0, 0.123),
+            #(2, 0, 0.0, 0.123),
+            (3, 1, 0.0, 0.123),
+            (0, 1, 0.0, 0.123),
+            (1, 1, 0.0, 0.123),
+            #(2, 2, 0.0, 0.123),
+            #(3, 2, 0.0, 0.123),
+            #(0, 2, 0.0, 0.123),
+            (1, 3, 0.0, 0.123),
+            (2, 3, 0.0, 0.123),
+            (3, 3, 0.0, 0.123), ])
 
-    def test_with_replacement_with_variable_n(self):
+    def test_with_replacement_with_variable_n(self, sim=sim):
         n = random.RandomDistribution('binomial', (5, 0.5), rng=MockRNG(start=1, delta=2))
-            # should give (1, 3, 0, 2, 4)
+        # should give (1, 3, 0, 2, 4)
         C = connectors.FixedNumberPreConnector(n=n, with_replacement=True, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [#(0, 0, 0.0, 0.123),
-                          (1, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123)])
+                         [  # (0, 0, 0.0, 0.123),
+            (1, 1, 0.0, 0.123),
+            (2, 1, 0.0, 0.123),
+            (3, 1, 0.0, 0.123),
+            (0, 3, 0.0, 0.123),
+            (1, 3, 0.0, 0.123)])
 
-    def test_with_replacement_no_self_connections(self):
+    def test_with_replacement_no_self_connections(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, with_replacement=True,
                                                allow_self_connections=False, rng=MockRNG(start=2, delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p2, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [#(2, 0, 0.0, 0.123),  # [2, 3, 4] --> [2, 3, 4]
-                          #(3, 0, 0.0, 0.123),
-                          #(4, 0, 0.0, 0.123),
-                          (0, 1, 0.0, 0.123),   # [0, 1, 2] --> [0, 3, 2]
-                          #(1, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
-                          #(4, 2, 0.0, 0.123),  # [4, 0, 1] --> [4, 0, 1]
-                          #(0, 2, 0.0, 0.123),
-                          #(1, 2, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123),   # [2, 3, 4] --> [2, 0, 4]
-                          #(3, 3, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (4, 3, 0.0, 0.123),
-                          ])
+                         [  # (2, 0, 0.0, 0.123),  # [2, 3, 4] --> [2, 3, 4]
+            #(3, 0, 0.0, 0.123),
+            #(4, 0, 0.0, 0.123),
+            (0, 1, 0.0, 0.123),   # [0, 1, 2] --> [0, 3, 2]
+            #(1, 1, 0.0, 0.123),
+            (3, 1, 0.0, 0.123),
+            (2, 1, 0.0, 0.123),
+            # (4, 2, 0.0, 0.123),  # [4, 0, 1] --> [4, 0, 1]
+            #(0, 2, 0.0, 0.123),
+            #(1, 2, 0.0, 0.123),
+            (2, 3, 0.0, 0.123),   # [2, 3, 4] --> [2, 0, 4]
+            #(3, 3, 0.0, 0.123),
+            (0, 3, 0.0, 0.123),
+            (4, 3, 0.0, 0.123),
+        ])
 
-    def test_no_replacement_no_self_connections(self):
+    def test_no_replacement_no_self_connections(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, with_replacement=False,
                                                allow_self_connections=False, rng=MockRNG(start=2, delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p2, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(4, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (4, 3, 0.0, 0.123),
                           #(3, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),])
+                          (1, 3, 0.0, 0.123), ])
 
-    def test_with_replacement_parallel_unsafe(self):
-        C = connectors.FixedNumberPreConnector(n=3, with_replacement=True, rng=MockRNG(delta=1, parallel_safe=False))
+    def test_with_replacement_parallel_unsafe(self, sim=sim):
+        C = connectors.FixedNumberPreConnector(
+            n=3, with_replacement=True, rng=MockRNG(delta=1, parallel_safe=False))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),])
+                          (1, 3, 0.0, 0.123), ])
 
-    def test_no_replacement_parallel_unsafe(self):
-        C = connectors.FixedNumberPreConnector(n=3, with_replacement=False, rng=MockRNG(delta=1, parallel_safe=False))
+    def test_no_replacement_parallel_unsafe(self, sim=sim):
+        C = connectors.FixedNumberPreConnector(
+            n=3, with_replacement=False, rng=MockRNG(delta=1, parallel_safe=False))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(3, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),])
+                          (1, 3, 0.0, 0.123), ])
 
 
 class TestArrayConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(3, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(4, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([1,0,1,0], dtype=bool))
+        assert_array_equal(self.p2._mask_local, numpy.array([1, 0, 1, 0], dtype=bool))
 
-    def test_connect_with_scalar_weights_and_delays(self):
+    def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         connections = numpy.array([
-                [0, 1, 1, 0],
-                [1, 1, 0, 1],
-                [0, 0, 1, 0],
-            ], dtype=bool)
+            [0, 1, 1, 0],
+            [1, 1, 0, 1],
+            [0, 0, 1, 0],
+        ], dtype=bool)
         C = connectors.ArrayConnector(connections, safe=False)
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(1, 0, 5.0, 0.5),
                           (0, 2, 5.0, 0.5),
                           (2, 2, 5.0, 0.5)])
 
-    def test_connect_with_random_weights_parallel_safe(self):
-        rd_w = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(delta=1.0, parallel_safe=True))
-        rd_d = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(start=1.0, delta=0.1, parallel_safe=True))
+    def test_connect_with_random_weights_parallel_safe(self, sim=sim):
+        rd_w = random.RandomDistribution(
+            'uniform', (0, 1), rng=MockRNG(delta=1.0, parallel_safe=True))
+        rd_d = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(
+            start=1.0, delta=0.1, parallel_safe=True))
         syn = sim.StaticSynapse(weight=rd_w, delay=rd_d)
         connections = numpy.array([
-                [0, 1, 1, 0],
-                [1, 1, 0, 1],
-                [0, 0, 1, 0],
-            ], dtype=bool)
+            [0, 1, 1, 0],
+            [1, 1, 0, 1],
+            [0, 0, 1, 0],
+        ], dtype=bool)
         C = connectors.ArrayConnector(connections, safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(1, 0, 0.0, 1.0),
                           (0, 2, 3.0, 1.3),
                           (2, 2, 4.0, 1.4000000000000001)])  # better to do an "almost-equal" check
 
 
 class TestCloneConnector(unittest.TestCase):
 
-    def setUp(self):
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
         connection_list = [
             (0, 0, 0.0, 1.0),
             (3, 0, 0.0, 1.0),
             (2, 3, 0.0, 1.0),  # local
             (2, 2, 0.0, 1.0),
             (0, 1, 0.0, 1.0),  # local
-            ]
+        ]
         list_connector = connectors.FromListConnector(connection_list)
         syn = sim.StaticSynapse()
         self.ref_prj = sim.Projection(self.p1, self.p2, list_connector, syn)
         self.orig_gather_dict = recording.gather_dict  # create reference to original function
         # The gather_dict function in recording needs to be temporarily replaced so it can work with
         # a mock version of the function to avoid it throwing an mpi4py import error when setting
         # the rank in pyNN.mock by hand to > 1
 
         def mock_gather_dict(D, all=False):
             return D
         recording.gather_dict = mock_gather_dict
 
-    def tearDown(self):
+    def tearDown(self, sim=sim):
         # restore original gather_dict function
         recording.gather_dict = self.orig_gather_dict
 
-    def test_connect(self):
+    def test_connect(self, sim=sim):
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         C = connectors.CloneConnector(self.ref_prj)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 1, 5.0, 0.5),
                           (2, 3, 5.0, 0.5)])
 
-    def test_connect_with_pre_post_mismatch(self):
+    def test_connect_with_pre_post_mismatch(self, sim=sim):
         syn = sim.StaticSynapse()
         C = connectors.CloneConnector(self.ref_prj)
         p3 = sim.Population(5, sim.IF_cond_exp(), structure=space.Line())
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, p3, C, syn)
 
 
 class TestIndexBasedProbabilityConnector(unittest.TestCase):
@@ -680,65 +827,66 @@
             return numpy.array(i * j + 1, dtype=float)
 
     class IndexBasedDelays(connectors.IndexBasedExpression):
 
         def __call__(self, i, j):
             return numpy.array(i + j + 1, dtype=float)
 
-    def setUp(self):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
         self.p1 = sim.Population(5, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
         assert_array_equal(self.p2._mask_local, numpy.array([1, 0, 1, 0, 1], dtype=bool))
 
-    def test_connect_with_scalar_weights_and_delays(self):
+    def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         syn = sim.StaticSynapse(weight=1.0, delay=2)
         C = connectors.IndexBasedProbabilityConnector(self.IndexBasedProbability())
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 0, 1, 2),
                           (3, 0, 1, 2),
                           (1, 2, 1, 2),
                           (4, 2, 1, 2),
                           (2, 4, 1, 2)])
 
-    def test_connect_with_index_based_weights(self):
+    def test_connect_with_index_based_weights(self, sim=sim):
         syn = sim.StaticSynapse(weight=self.IndexBasedWeights(), delay=2)
         C = connectors.IndexBasedProbabilityConnector(self.IndexBasedProbability())
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 0, 1, 2),
                           (3, 0, 1, 2),
                           (1, 2, 3, 2),
                           (4, 2, 9, 2),
                           (2, 4, 9, 2)])
 
-    def test_connect_with_index_based_delays(self):
+    def test_connect_with_index_based_delays(self, sim=sim):
         syn = sim.StaticSynapse(weight=1.0, delay=self.IndexBasedDelays())
         C = connectors.IndexBasedProbabilityConnector(self.IndexBasedProbability())
         prj = sim.Projection(self.p1, self.p2, C, syn)
         self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
                          [(0, 0, 1, 1),
                           (3, 0, 1, 4),
                           (1, 2, 1, 4),
                           (4, 2, 1, 7),
                           (2, 4, 1, 7)])
 
 
 class TestDisplacementDependentProbabilityConnector(unittest.TestCase):
 
-    def setUp(self):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
         self.p1 = sim.Population(9, sim.IF_cond_exp(),
                                  structure=space.Grid2D(aspect_ratio=1.0, dx=1.0, dy=1.0))
         self.p2 = sim.Population(9, sim.HH_cond_exp(),
                                  structure=space.Grid2D(aspect_ratio=1.0, dx=1.0, dy=1.0))
-        assert_array_equal(self.p2._mask_local, numpy.array([1, 0, 1, 0, 1, 0, 1, 0, 1], dtype=bool))
+        assert_array_equal(self.p2._mask_local, numpy.array(
+            [1, 0, 1, 0, 1, 0, 1, 0, 1], dtype=bool))
 
-    def test_connect(self):
+    def test_connect(self, sim=sim):
         syn = sim.StaticSynapse(weight=1.0, delay=2)
 
         def displacement_expression(d):
             return 0.5 * ((d[0] >= -1) * (d[0] <= 2)) + 0.25 * (d[1] >= 0) * (d[1] <= 1)
         C = connectors.DisplacementDependentProbabilityConnector(displacement_expression,
                                                                  rng=MockRNG(delta=0.01))
         prj = sim.Projection(self.p1, self.p2, C, syn)
@@ -768,53 +916,22 @@
                           (0, 6, 1.0, 2.0),
                           (3, 6, 1.0, 2.0),
                           (6, 6, 1.0, 2.0),
                           (1, 8, 1.0, 2.0),
                           (2, 8, 1.0, 2.0)])
 
 
-@unittest.skip('skipping these tests until I figure out how I want to refactor checks')
-class CheckTest(unittest.TestCase):
+class TestFixedTotalNumberConnector(unittest.TestCase):
 
-    def setUp(self):
-        self.MIN_DELAY = 0.123
+    def setUp(self, sim=sim):
         sim.setup(num_processes=2, rank=1, min_delay=0.123)
+        self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
+        self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
+        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
-    def test_check_weights_with_scalar(self):
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'excitatory', is_conductance=True))
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'excitatory', is_conductance=False))
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'inhibitory', is_conductance=True))
-        self.assertEqual(-4.3, connectors.check_weights(-4.3, 'inhibitory', is_conductance=False))
-        self.assertEqual(connectors.DEFAULT_WEIGHT, connectors.check_weights(None, 'excitatory', is_conductance=True))
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, 4.3, 'inhibitory', is_conductance=False)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, -4.3, 'inhibitory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, -4.3, 'excitatory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, -4.3, 'excitatory', is_conductance=False)
-
-    def test_check_weights_with_array(self):
-        w = numpy.arange(10)
-        assert_array_equal(w, connectors.check_weights(w, 'excitatory', is_conductance=True))
-        assert_array_equal(w, connectors.check_weights(w, 'excitatory', is_conductance=False))
-        assert_array_equal(w, connectors.check_weights(w, 'inhibitory', is_conductance=True))
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'inhibitory', is_conductance=False)
-        w = numpy.arange(-10, 0)
-        assert_array_equal(w, connectors.check_weights(w, 'inhibitory', is_conductance=False))
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'inhibitory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'excitatory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'excitatory', is_conductance=False)
-        w = numpy.arange(-5, 5)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'excitatory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'excitatory', is_conductance=False)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'inhibitory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, w, 'inhibitory', is_conductance=False)
-
-    def test_check_weights_with_invalid_value(self):
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, "butterflies", 'excitatory', is_conductance=True)
-
-    def test_check_weight_is_conductance_is_None(self):
-        # need to check that a log message was created
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'excitatory', is_conductance=None))
-
-    def test_check_delay(self):
-        self.assertEqual(connectors.check_delays(2 * self.MIN_DELAY, self.MIN_DELAY, 1e99), 2 * self.MIN_DELAY)
-        self.assertRaises(errors.ConnectionError, connectors.check_delays, 0.5 * self.MIN_DELAY, self.MIN_DELAY, 1e99)
-        self.assertRaises(errors.ConnectionError, connectors.check_delays, 3.0, self.MIN_DELAY, 2.0)
+    def test_1(self):
+        C = connectors.FixedTotalNumberConnector(n=12, rng=random.NumpyRNG())
+        syn = sim.StaticSynapse(weight="0.5*d")
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        connections = prj.get(["weight", "delay"], format='list', gather=False)
+        self.assertLess(len(connections), 12)    # unlikely to be 12, since we have 2 MPI nodes
+        self.assertGreater(len(connections), 0)  # unlikely to be 0
```

### Comparing `PyNN-0.9.5/test/hardware/unittests/test_population.py` & `PyNN-0.9.6/test/unittests/test_population.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,507 +1,622 @@
 """
 Tests of the common implementation of the Population class, using the pyNN.mock
 backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
+try:
+    basestring
+except NameError:
+    basestring = str
 import numpy
+import sys
 from numpy.testing import assert_array_equal, assert_array_almost_equal
 import quantities as pq
-from mock import Mock
-from mocks import MockRNG
+try:
+    from unittest.mock import Mock, patch
+except ImportError:
+    from mock import Mock, patch
+from .mocks import MockRNG
+import pyNN.mock as sim
 from pyNN import random, errors, space
 from pyNN.parameters import Sequence
 
-if True:
-    import pyNN.hardware.brainscales as sim
-    ParameterValueOutOfRangeError = sim.range_checker.ParameterValueOutOfRangeError
-    IF_cond_exp = sim.Hardware_IF_cond_exp
-    EIF_cond_exp_isfa_ista = sim.Hardware_EIF_cond_exp_isfa_ista
-else:
-    import pyNN.mock as sim
-    IF_cond_exp = sim.IF_cond_exp
-    EIF_cond_exp_isfa_ista = sim.EIF_cond_exp_isfa_ista
+
+def setUp():
+    pass
+
+
+def tearDown():
+    pass
 
 
 class PopulationTest(unittest.TestCase):
 
-    def setUp(self):
-        if True:
-            extra = {'loglevel': 0, 'useSystemSim': True, 'hardware': sim.hardwareSetup['one-hicann']}
-        else:
-            extra = {}
+    def setUp(self, sim=sim, **extra):
         sim.setup(**extra)
-        
-    def tearDown(self):
-        sim.end()
 
-    def test_create_with_standard_cell_simple(self):
+    def tearDown(self, sim=sim):
+        sim.end()
 
-        p = sim.Population(11, IF_cond_exp())
+    def test_create_with_standard_cell_simple(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
         self.assertEqual(p.size, 11)
         self.assertIsInstance(p.label, basestring)
-        self.assertIsInstance(p.celltype, IF_cond_exp)
+        self.assertIsInstance(p.celltype, sim.IF_cond_exp)
         self.assertIsInstance(p._structure, space.Line)
         self.assertEqual(p._positions, None)
         self.assertEqual(p.initial_values.keys(), p.celltype.default_initial_values.keys())
 
-    def test_create_with_parameters(self):
-        p = sim.Population(4, IF_cond_exp(**{'tau_m': lambda i: 12.3 + 0.1 * i,
-                                                 'cm': 0.2,
-                                                 'tau_syn_E': numpy.array([1.0, 2.0, 3.0, 4.0])}))
-        cm, tau_m, tau_syn_E = p.get(('cm', 'tau_m', 'tau_syn_E'), gather=True)
-        assert_array_almost_equal(tau_m, numpy.array([12.3, 12.4, 12.5, 12.6]), decimal=12)
-        self.assertEqual(cm, 0.2)
-        assert_array_equal(tau_syn_E, numpy.array([1.0, 2.0, 3.0, 4.0]))
+    def test_create_with_parameters(self, sim=sim):
+        p = sim.Population(4, sim.IF_cond_exp(**{'tau_m': 12.3,
+                                                 'tau_syn_E': lambda i: 0.987 + 0.01 * i,
+                                                 'tau_syn_I': numpy.array([0.5, 0.6, 0.7, 0.8])}))
+        tau_syn_E, tau_m, tau_syn_I = p.get(('tau_syn_E', 'tau_m', 'tau_syn_I'), gather=True)
+        assert_array_almost_equal(tau_syn_E, numpy.array([0.987, 0.997, 1.007, 1.017]))
+        self.assertAlmostEqual(tau_m, 12.3)
+        assert_array_equal(tau_syn_I, numpy.array([0.5, 0.6, 0.7, 0.8]))
 
     # test create native cell
 
     # test create native cell with params
 
     # test create with structure
-    def test_create_with_implicit_grid(self):
-        p = sim.Population((11,), IF_cond_exp())
+
+    def test_create_with_implicit_grid(self, sim=sim):
+        p = sim.Population((11,), sim.IF_cond_exp())
         self.assertEqual(p.size, 11)
         self.assertIsInstance(p.structure, space.Line)
-        p = sim.Population((5, 6), IF_cond_exp())
+        p = sim.Population((5, 6), sim.IF_cond_exp())
         self.assertEqual(p.size, 30)
         self.assertIsInstance(p.structure, space.Grid2D)
-        p = sim.Population((2, 3, 4), IF_cond_exp())
+        p = sim.Population((2, 3, 4), sim.IF_cond_exp())
         self.assertEqual(p.size, 24)
         self.assertIsInstance(p.structure, space.Grid3D)
-        self.assertRaises(Exception, sim.Population, (2, 3, 4, 5), IF_cond_exp())
+        self.assertRaises(Exception, sim.Population, (2, 3, 4, 5), sim.IF_cond_exp())
 
-    #def test_create_with_initial_values():
+    def test_create_with_empty_spike_source_array(self, sim=sim):
+        # regression test for https://github.com/NeuralEnsemble/PyNN/issues/378
+        p = sim.Population(11, sim.SpikeSourceArray(spike_times=[]))
 
-    def test_id_to_index(self):
-        p = sim.Population(11, IF_cond_exp())
+    # def test_create_with_initial_values():
+
+    def test_id_to_index(self, sim=sim):
+        p = sim.Population(11, sim.IF_curr_alpha())
         self.assertEqual(p.id_to_index(p[0]), 0)
         self.assertEqual(p.id_to_index(p[10]), 10)
 
-    def test_id_to_index_with_array(self):
-        p = sim.Population(11, IF_cond_exp())
+    def test_id_to_index_with_array(self, sim=sim):
+        p = sim.Population(11, sim.IF_curr_alpha())
         assert_array_equal(p.id_to_index(p.all_cells[3:9:2]), numpy.arange(3, 9, 2))
 
-    def test_id_to_index_with_populationview(self):
-        p = sim.Population(11, IF_cond_exp())
+    def test_id_to_index_with_populationview(self, sim=sim):
+        p = sim.Population(11, sim.IF_curr_alpha())
         view = p[3:7]
         self.assertIsInstance(view, sim.PopulationView)
         assert_array_equal(p.id_to_index(view), numpy.arange(3, 7))
 
-    def test_id_to_index_with_invalid_id(self):
-        p = sim.Population(11, IF_cond_exp())
+    def test_id_to_index_with_invalid_id(self, sim=sim):
+        p = sim.Population(11, sim.IF_curr_alpha())
         self.assertRaises(ValueError, p.id_to_index, p.last_id + 1)
         self.assertRaises(ValueError, p.id_to_index, p.first_id - 1)
 
-    def test_id_to_index_with_invalid_ids(self):
-        p = sim.Population(11, IF_cond_exp())
+    def test_id_to_index_with_invalid_ids(self, sim=sim):
+        p = sim.Population(11, sim.IF_curr_alpha())
         self.assertRaises(ValueError, p.id_to_index, [p.first_id - 1] + p.all_cells[0:3].tolist())
 
-    #def test_id_to_local_index():
+    # def test_id_to_local_index():
 
     # test structure property
-    def test_set_structure(self):
-        p = sim.Population(11, IF_cond_exp())
+
+    def test_set_structure(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
         p.positions = numpy.arange(33).reshape(3, 11)
         new_struct = space.Grid2D()
         p.structure = new_struct
         self.assertEqual(p.structure, new_struct)
         self.assertEqual(p._positions, None)
 
     # test positions property
-    def test_get_positions(self):
-        p = sim.Population(11, IF_cond_exp())
+
+    def test_get_positions(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
         pos1 = numpy.arange(33).reshape(3, 11)
         p._structure = Mock()
         p._structure.generate_positions = Mock(return_value=pos1)
         self.assertEqual(p._positions, None)
         assert_array_equal(p.positions, pos1)
 
         pos2 = 1 + numpy.arange(33).reshape(3, 11)
         p.positions = pos2
         assert_array_equal(p.positions, pos2)
 
-    def test_set_positions(self):
-        p = sim.Population(11, IF_cond_exp())
-        assert p._structure != None
+    def test_set_positions(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
+        assert p._structure is not None
         new_positions = numpy.random.uniform(size=(3, 11))
         p.positions = new_positions
         self.assertEqual(p.structure, None)
         assert_array_equal(p.positions, new_positions)
         new_positions[0, 0] = 99.9
         self.assertNotEqual(p.positions[0, 0], 99.9)
 
-    def test_position_generator(self):
-        p = sim.Population(11, IF_cond_exp())
+    def test_position_generator(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
         assert_array_equal(p.position_generator(0), p.positions[:, 0])
         assert_array_equal(p.position_generator(10), p.positions[:, 10])
         assert_array_equal(p.position_generator(-1), p.positions[:, 10])
         assert_array_equal(p.position_generator(-11), p.positions[:, 0])
         self.assertRaises(IndexError, p.position_generator, 11)
         self.assertRaises(IndexError, p.position_generator, -12)
 
-    def test__getitem__int(self):
+    def test__getitem__int(self, sim=sim):
         # Should return the correct ID object
-        p = sim.Population(12, IF_cond_exp())
-        self.assertEqual(p[11], 11 + p[0])
+        p = sim.Population(12, sim.IF_cond_exp())
+        self.assertEqual(p[11], p[0] + 11)
         self.assertRaises(IndexError, p.__getitem__, 12)
-        self.assertEqual(p[-1], 11 + p[0])
+        self.assertEqual(p[-1], p[11])
 
-    def test__getitem__slice(self):
+    def test__getitem__slice(self, sim=sim):
         # Should return a PopulationView with the correct parent and value
         # of all_cells
-        p = sim.Population(17, IF_cond_exp())
+        p = sim.Population(17, sim.HH_cond_exp())
         pv = p[3:9]
         self.assertEqual(pv.parent, p)
         assert_array_almost_equal(pv.all_cells, p.all_cells[3:9])
 
-    def test__getitem__list(self):
-       p = sim.Population(23, IF_cond_exp())
-       pv = p[range(3, 9)]
-       self.assertEqual(pv.parent, p)
-       assert_array_almost_equal(pv.all_cells, p.all_cells[3:9])
+    def test__getitem__list(self, sim=sim):
+        p = sim.Population(23, sim.HH_cond_exp())
+        pv = p[list(range(3, 9))]
+        self.assertEqual(pv.parent, p)
+        assert_array_almost_equal(pv.all_cells, p.all_cells[3:9])
 
-    def test__getitem__tuple(self):
-        p = sim.Population(23, IF_cond_exp())
+    def test__getitem__tuple(self, sim=sim):
+        p = sim.Population(23, sim.HH_cond_exp())
         pv = p[(3, 5, 7)]
         self.assertEqual(pv.parent, p)
         assert_array_almost_equal(pv.all_cells, p.all_cells[[3, 5, 7]])
 
-    def test__getitem__invalid(self):
-        p = sim.Population(23, IF_cond_exp())
+    def test__getitem__invalid(self, sim=sim):
+        p = sim.Population(23, sim.IF_curr_alpha())
         self.assertRaises(TypeError, p.__getitem__, "foo")
 
-    def test__len__(self):
+    def test__len__(self, sim=sim):
         # len(p) should give the global size (all MPI nodes)
-        p = sim.Population(77, IF_cond_exp())
+        p = sim.Population(77, sim.IF_cond_exp())
         self.assertEqual(len(p), p.size, 77)
 
-    def test_iter(self):
-        p = sim.Population(6, IF_cond_exp())
+    def test_iter(self, sim=sim):
+        p = sim.Population(6, sim.IF_curr_exp())
         itr = p.__iter__()
-        assert hasattr(itr, "next")
+        assert hasattr(itr, "next") or hasattr(itr, "__next__")
         self.assertEqual(len(list(itr)), 6)
 
-    def test___add__two(self):
+    def test___add__two(self, sim=sim):
         # adding two populations should give an Assembly
-        p1 = sim.Population(6, EIF_cond_exp_isfa_ista())
-        p2 = sim.Population(17, IF_cond_exp())
+        p1 = sim.Population(6, sim.IF_curr_exp())
+        p2 = sim.Population(17, sim.IF_cond_exp())
         assembly = p1 + p2
         self.assertIsInstance(assembly, sim.Assembly)
         self.assertEqual(assembly.populations, [p1, p2])
 
-    def test___add__three(self):
+    def test___add__three(self, sim=sim):
         # adding three populations should give an Assembly
-        p1 = sim.Population(6, IF_cond_exp())
-        p2 = sim.Population(17, EIF_cond_exp_isfa_ista())
-        p3 = sim.Population(9, sim.SpikeSourceArray())
+        p1 = sim.Population(6, sim.IF_curr_exp())
+        p2 = sim.Population(17, sim.IF_cond_exp())
+        p3 = sim.Population(9, sim.HH_cond_exp())
         assembly = p1 + p2 + p3
         self.assertIsInstance(assembly, sim.Assembly)
         self.assertEqual(assembly.populations, [p1, p2, p3])
 
-    def test_nearest(self):
-        p = sim.Population(13, IF_cond_exp())
+    def test_nearest(self, sim=sim):
+        p = sim.Population(13, sim.IF_cond_exp())
         p.positions = numpy.arange(39).reshape((13, 3)).T
         self.assertEqual(p.nearest((0.0, 1.0, 2.0)), p[0])
         self.assertEqual(p.nearest((3.0, 4.0, 5.0)), p[1])
         self.assertEqual(p.nearest((36.0, 37.0, 38.0)), p[12])
         self.assertEqual(p.nearest((1.49, 2.49, 3.49)), p[0])
         self.assertEqual(p.nearest((1.51, 2.51, 3.51)), p[1])
 
         x, y, z = 4, 5, 6
-        p = sim.Population((x, y, z), IF_cond_exp())
+        p = sim.Population((x, y, z), sim.IF_cond_alpha())
         self.assertEqual(p.nearest((0.0, 0.0, 0.0)), p[0])
         self.assertEqual(p.nearest((0.0, 0.0, 1.0)), p[1])
         self.assertEqual(p.nearest((0.0, 1.0, 0.0)), p[z])
         self.assertEqual(p.nearest((1.0, 0.0, 0.0)), p[y * z])
         self.assertEqual(p.nearest((3.0, 2.0, 1.0)), p[3 * y * z + 2 * z + 1])
         self.assertEqual(p.nearest((3.49, 2.49, 1.49)), p[3 * y * z + 2 * z + 1])
         self.assertEqual(p.nearest((3.49, 2.49, 1.51)), p[3 * y * z + 2 * z + 2])
-        #self.assertEqual(p.nearest((3.49,2.49,1.5)), p[3*y*z+2*z+2]) # known to fail
+        # self.assertEqual(p.nearest((3.49,2.49,1.5)), p[3*y*z+2*z+2]) # known to fail
         #self.assertEqual(p.nearest((2.5,2.5,1.5)), p[3*y*z+3*y+2])
 
-    def test_sample(self):
-        p = sim.Population(13, IF_cond_exp())
+    def test_sample(self, sim=sim):
+        p = sim.Population(13, sim.IF_cond_exp())
         rng = Mock()
-        rng.permutation = Mock(return_value=numpy.array([7, 4, 8, 12, 0, 3, 9, 1, 2, 11, 5, 10, 6]))
+        rng.permutation = Mock(return_value=numpy.array(
+            [7, 4, 8, 12, 0, 3, 9, 1, 2, 11, 5, 10, 6]))
         pv = p.sample(5, rng=rng)
         assert_array_equal(pv.all_cells,
                            p.all_cells[[7, 4, 8, 12, 0]])
 
-    def test_get_multiple_homogeneous_params_with_gather(self):
-        p = sim.Population(4, IF_cond_exp(**{'tau_m': 12.3, 'cm': 0.2, 'i_offset': 0.0}))
-        cm, tau_m = p.get(('cm', 'tau_m'), gather=True)
-        self.assertIsInstance(cm, float)
-        self.assertEqual(cm, 0.2)
-        self.assertEqual(tau_m, 12.3)
+    def test_get_multiple_homogeneous_params_with_gather(self, sim=sim):
+        p = sim.Population(4, sim.IF_cond_exp(
+            **{'tau_m': 12.3, 'tau_syn_E': 0.987, 'tau_syn_I': 0.7}))
+        tau_syn_E, tau_m = p.get(('tau_syn_E', 'tau_m'), gather=True)
+        self.assertIsInstance(tau_syn_E, float)
+        self.assertEqual(tau_syn_E, 0.987)
+        self.assertAlmostEqual(tau_m, 12.3)
+
+    def test_get_single_param_with_gather(self, sim=sim):
+        p = sim.Population(4, sim.IF_cond_exp(tau_m=12.3, tau_syn_E=0.987, tau_syn_I=0.7))
+        tau_syn_E = p.get('tau_syn_E', gather=True)
+        self.assertEqual(tau_syn_E, 0.987)
+
+    def test_get_multiple_inhomogeneous_params_with_gather(self, sim=sim):
+        p = sim.Population(4, sim.IF_cond_exp(tau_m=12.3,
+                                              tau_syn_E=[0.987, 0.988, 0.989, 0.990],
+                                              tau_syn_I=lambda i: 0.5 + 0.1 * i))
+        tau_syn_E, tau_m, tau_syn_I = p.get(('tau_syn_E', 'tau_m', 'tau_syn_I'), gather=True)
+        self.assertIsInstance(tau_m, float)
+        self.assertIsInstance(tau_syn_E, numpy.ndarray)
+        assert_array_equal(tau_syn_E, numpy.array([0.987, 0.988, 0.989, 0.990]))
+        self.assertAlmostEqual(tau_m, 12.3)
+        assert_array_almost_equal(tau_syn_I, numpy.array([0.5, 0.6, 0.7, 0.8]), decimal=12)
 
-    def test_get_single_param_with_gather(self):
-        p = sim.Population(4, IF_cond_exp(tau_m=12.3, cm=0.2, i_offset=0.))
-        tau_m = p.get('tau_m', gather=True)
+    def test_get_multiple_params_no_gather(self, sim=sim):
+        sim.simulator.state.num_processes = 2
+        sim.simulator.state.mpi_rank = 1
+        p = sim.Population(4, sim.IF_cond_exp(tau_m=12.3,
+                                              tau_syn_E=[0.987, 0.988, 0.989, 0.990],
+                                              i_offset=lambda i: -0.2 * i))
+        tau_syn_E, tau_m, i_offset = p.get(('tau_syn_E', 'tau_m', 'i_offset'), gather=False)
+        self.assertIsInstance(tau_m, float)
+        self.assertIsInstance(tau_syn_E, numpy.ndarray)
+        assert_array_equal(tau_syn_E, numpy.array([0.988, 0.990]))
         self.assertEqual(tau_m, 12.3)
+        assert_array_almost_equal(i_offset, numpy.array([-0.2, -0.6]), decimal=12)
+        sim.simulator.state.num_processes = 1
+        sim.simulator.state.mpi_rank = 0
 
-    def test_get_multiple_inhomogeneous_params_with_gather(self):
-        p = sim.Population(4, IF_cond_exp(tau_m=[12.3, 12.4, 12.5, 12.6],
-                                              cm=0.2,
-                                              tau_syn_E=lambda i: 1.0 + 1.0 * i))
-        cm, tau_m, tau_syn_E = p.get(('cm', 'tau_m', 'tau_syn_E'), gather=True)
-        self.assertIsInstance(cm, float)
-        self.assertIsInstance(tau_m, numpy.ndarray)
-        assert_array_equal(tau_m, numpy.array([12.3, 12.4, 12.5, 12.6]))
-        self.assertEqual(cm, 0.2)
-        assert_array_almost_equal(tau_syn_E, numpy.array([1.0, 2.0, 3.0, 4.0]), decimal=12)
-
-    def test_get_sequence_param(self):
+    def test_get_sequence_param(self, sim=sim):
         p = sim.Population(3, sim.SpikeSourceArray(spike_times=[Sequence([1, 2, 3, 4]),
                                                                 Sequence([2, 3, 4, 5]),
                                                                 Sequence([3, 4, 5, 6])]))
         spike_times = p.get('spike_times')
         self.assertEqual(spike_times.size, 3)
         assert_array_equal(spike_times[1], Sequence([2, 3, 4, 5]))
 
-    def test_set(self):
-        p = sim.Population(4, IF_cond_exp, {'tau_m': 14.0, 'v_reset': -50., 'tau_syn_E': 1.0})
-        rng = MockRNG(start=12.31, delta=0.01, parallel_safe=True)
-        p.set(tau_m=random.RandomDistribution('uniform', (0.5, 1.5), rng=rng), v_reset=-60)
-        tau_m, v_reset, tau_syn_E = p.get(('tau_m', 'v_reset', 'tau_syn_E'), gather=True)
-        assert_array_equal(tau_m, numpy.array([12.31, 12.32, 12.33, 12.34]))
-        assert_array_equal(v_reset, -60.0**numpy.ones((4,)))
-        assert_array_equal(tau_syn_E, 1.0 * numpy.ones((4,)))
+    def test_set(self, sim=sim):
+        p = sim.Population(4, sim.IF_cond_exp, {
+                           'tau_m': 12.3, 'tau_syn_E': 0.987, 'tau_syn_I': 0.7})
+        rng = MockRNG(start=1.21, delta=0.01, parallel_safe=True)
+        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.5, 1.5), rng=rng), tau_m=9.87)
+        tau_m, tau_syn_E, tau_syn_I = p.get(('tau_m', 'tau_syn_E', 'tau_syn_I'), gather=True)
+        assert_array_equal(tau_syn_E, numpy.array([1.21, 1.22, 1.23, 1.24]))
+        assert_array_almost_equal(tau_m, 9.87 * numpy.ones((4,)))
+        assert_array_equal(tau_syn_I, 0.7 * numpy.ones((4,)))
 
-    def test_set_invalid_name(self):
-        p = sim.Population(9, IF_cond_exp())
+    def test_set_invalid_name(self, sim=sim):
+        p = sim.Population(9, sim.HH_cond_exp())
         self.assertRaises(errors.NonExistentParameterError, p.set, foo=13.2)
 
-    def test_set_invalid_type(self):
-        p = sim.Population(9, IF_cond_exp())
+    def test_set_invalid_type(self, sim=sim):
+        p = sim.Population(9, sim.IF_cond_exp())
         self.assertRaises(errors.InvalidParameterValueError, p.set, tau_m={})
         self.assertRaises(errors.InvalidParameterValueError, p.set, v_reset='bar')
 
-    def test_set_sequence(self):
+    def test_set_sequence(self, sim=sim):
         p = sim.Population(3, sim.SpikeSourceArray())
         p.set(spike_times=[Sequence([1, 2, 3, 4]),
                            Sequence([2, 3, 4, 5]),
                            Sequence([3, 4, 5, 6])])
         spike_times = p.get('spike_times', gather=True)
         self.assertEqual(spike_times.size, 3)
         assert_array_equal(spike_times[1], Sequence([2, 3, 4, 5]))
 
-    def test_set_array(self):
-        p = sim.Population(5, IF_cond_exp())
+    def test_set_array(self, sim=sim):
+        p = sim.Population(5, sim.IF_cond_exp())
         p.set(v_thresh=-50.0 + numpy.arange(5))
         assert_array_equal(p.get('v_thresh', gather=True),
                            numpy.array([-50.0, -49.0, -48.0, -47.0, -46.0]))
 
-    def test_set_random_distribution_parallel_unsafe(self):
+    def test_set_random_distribution_parallel_unsafe(self, sim=sim):
         orig_rcfg = random.get_mpi_config
         random.get_mpi_config = lambda: (1, 2)
         sim.simulator.state.num_processes = 2
         sim.simulator.state.mpi_rank = 1
-        p = sim.Population(4, IF_cond_exp(tau_syn_E=1.0))
-        rng = MockRNG(start=1.5, delta=0.01, parallel_safe=False)
-        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.8, 3.0), rng=rng))
+        p = sim.Population(4, sim.IF_cond_exp(tau_syn_E=0.987))
+        rng = MockRNG(start=1.21, delta=0.01, parallel_safe=False)
+        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.8, 1.2), rng=rng))
         tau_syn_E = p.get('tau_syn_E', gather=False)
-        assert_array_equal(tau_syn_E, numpy.array([1.5, 1.51]))
+        assert_array_equal(tau_syn_E, numpy.array([1.21, 1.22]))
         random.get_mpi_config = orig_rcfg
         sim.simulator.state.num_processes = 1
         sim.simulator.state.mpi_rank = 0
 
-    def test_set_random_distribution_parallel_safe(self):
+    def test_set_random_distribution_parallel_safe(self, sim=sim):
         orig_rcfg = random.get_mpi_config
         random.get_mpi_config = lambda: (1, 2)
         sim.simulator.state.num_processes = 2
         sim.simulator.state.mpi_rank = 1
-        p = sim.Population(4, IF_cond_exp(tau_syn_E=1.0))
-        rng = MockRNG(start=2.0, delta=0.01, parallel_safe=True)
-        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.1, 3.0), rng=rng))
+        p = sim.Population(4, sim.IF_cond_exp(tau_syn_E=0.987))
+        rng = MockRNG(start=1.21, delta=0.01, parallel_safe=True)
+        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.1, 1), rng=rng))
         tau_syn_E = p.get('tau_syn_E', gather=False)
-        assert_array_equal(tau_syn_E, numpy.array([2.01, 2.03]))
+        assert_array_equal(tau_syn_E, numpy.array([1.22, 1.24]))
         random.get_mpi_config = orig_rcfg
         sim.simulator.state.num_processes = 1
         sim.simulator.state.mpi_rank = 0
 
-    def test_tset(self):
-        p = sim.Population(17, IF_cond_exp())
+    def test_tset(self, sim=sim):
+        p = sim.Population(17, sim.IF_cond_alpha())
         p.set = Mock()
         tau_m = numpy.linspace(10.0, 20.0, num=p.size)
         p.tset("tau_m", tau_m)
         p.set.assert_called_with(tau_m=tau_m)
 
-    def test_rset(self):
-        p = sim.Population(17, IF_cond_exp())
+    def test_rset(self, sim=sim):
+        p = sim.Population(17, sim.IF_cond_alpha())
         p.set = Mock()
-        v_reset = random.RandomDistribution('uniform', low=-70.0, high=-60.0)
-        p.rset("v_reset", v_reset)
-        p.set.assert_called_with(v_reset=v_reset)
+        v_rest = random.RandomDistribution('uniform', low=-70.0, high=-60.0)
+        p.rset("v_rest", v_rest)
+        p.set.assert_called_with(v_rest=v_rest)
 
-    ##def test_set_with_native_rng():
+    # def test_set_with_native_rng():
 
-    def test_initialize(self):
-        p = sim.Population(17, EIF_cond_exp_isfa_ista())
+    def test_initialize(self, sim=sim):
+        p = sim.Population(17, sim.EIF_cond_exp_isfa_ista())
         v_init = numpy.linspace(-70.0, -60.0, num=p.size)
         w_init = 0.1
         p.initialize(v=v_init, w=w_init)
         assert_array_equal(p.initial_values['v'].evaluate(simplify=True), v_init)
         assert_array_equal(p.initial_values['w'].evaluate(simplify=True), w_init)
         # should call p.record(('v', 'w')) and check that the recorded data starts with the initial value
 
-    def test_can_record(self):
-        p = sim.Population(17, EIF_cond_exp_isfa_ista())
+    def test_can_record(self, sim=sim):
+        p = sim.Population(17, sim.EIF_cond_exp_isfa_ista())
         assert p.can_record('v')
+        assert p.can_record('w')
+        assert p.can_record('gsyn_inh')
         assert p.can_record('spikes')
         assert not p.can_record('foo')
-        assert not p.can_record('w')
-        assert not p.can_record('gsyn_inh')
 
-    def test_record_with_single_variable(self):
-        p = sim.Population(14, EIF_cond_exp_isfa_ista())
+    def test_record_with_single_variable(self, sim=sim):
+        p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
         p.record('v')
         sim.run(12.3)
         data = p.get_data(gather=True).segments[0]
         self.assertEqual(len(data.analogsignals), 1)
         n_values = int(round(12.3 / sim.get_time_step())) + 1
         self.assertEqual(data.analogsignals[0].name, 'v')
         self.assertEqual(data.analogsignals[0].shape, (n_values, p.size))
 
-    def test_record_with_multiple_variables(self):
-        p = sim.Population(2, EIF_cond_exp_isfa_ista())
+    def test_record_with_multiple_variables(self, sim=sim):
+        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
+        p.record(('v', 'w', 'gsyn_exc'))
+        sim.run(10.0)
+        data = p.get_data(gather=True).segments[0]
+        self.assertEqual(len(data.analogsignals), 3)
+        n_values = int(round(10.0 / sim.get_time_step())) + 1
+        names = set(arr.name for arr in data.analogsignals)
+        self.assertEqual(names, set(('v', 'w', 'gsyn_exc')))
+        for arr in data.analogsignals:
+            self.assertEqual(arr.shape, (n_values, p.size))
+
+    def test_record_with_v_and_spikes(self, sim=sim):
+        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
         p.record(('v', 'spikes'))
         sim.run(10.0)
         data = p.get_data(gather=True).segments[0]
         self.assertEqual(len(data.analogsignals), 1)
         n_values = int(round(10.0 / sim.get_time_step())) + 1
         names = set(arr.name for arr in data.analogsignals)
         self.assertEqual(names, set(('v')))
         for arr in data.analogsignals:
             self.assertEqual(arr.shape, (n_values, p.size))
 
-    def test_record_v(self):
-        p = sim.Population(2, EIF_cond_exp_isfa_ista())
+    def test_record_v(self, sim=sim):
+        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
         p.record = Mock()
         p.record_v("arg1")
         p.record.assert_called_with('v', "arg1")
 
-    def test_record_gsyn(self):
-        p = sim.Population(2, EIF_cond_exp_isfa_ista())
+    def test_record_gsyn(self, sim=sim):
+        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
         p.record = Mock()
         p.record_gsyn("arg1")
         p.record.assert_called_with(['gsyn_exc', 'gsyn_inh'], "arg1")
 
-    def test_record_invalid_variable(self):
-        p = sim.Population(14, IF_cond_exp())
+    def test_record_invalid_variable(self, sim=sim):
+        p = sim.Population(14, sim.IF_curr_alpha())
         self.assertRaises(errors.RecordingError,
-                          p.record, ('v', 'w'))  # can't record w from this celltype
+                          p.record, ('v', 'gsyn_exc'))  # can't record gsyn_exc from this celltype
 
-    def test_get_data_no_gather(self):
-       self.fail()
+    # def test_write_data(self, sim=sim):
+    #    self.fail()
+    #
+
+    def test_get_data_with_gather(self, sim=sim):
+        t1 = 12.3
+        t2 = 13.4
+        t3 = 14.5
+        p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
+        p.record('v')
+        sim.run(t1)
+        # what if we call p.record between two run statements?
+        # would be nice to get an AnalogSignal with a non-zero t_start
+        # but then need to make sure we get the right initial value
+        sim.run(t2)
+        sim.reset()
+        p.record('spikes')
+        p.record('w')
+        sim.run(t3)
+        data = p.get_data(gather=True)
+        self.assertEqual(len(data.segments), 2)
+
+        seg0 = data.segments[0]
+        self.assertEqual(len(seg0.analogsignals), 1)
+        v = seg0.analogsignals[0]
+        self.assertEqual(v.name, 'v')
+        num_points = int(round((t1 + t2) / sim.get_time_step())) + 1
+        self.assertEqual(v.shape, (num_points, p.size))
+        self.assertEqual(v.t_start, 0.0 * pq.ms)
+        self.assertEqual(v.units, pq.mV)
+        self.assertEqual(v.sampling_period, 0.1 * pq.ms)
+        self.assertEqual(len(seg0.spiketrains), 0)
+
+        seg1 = data.segments[1]
+        self.assertEqual(len(seg1.analogsignals), 2)
+        w = seg1.filter(name='w')[0]
+        self.assertEqual(w.name, 'w')
+        num_points = int(round(t3 / sim.get_time_step())) + 1
+        self.assertEqual(w.shape, (num_points, p.size))
+        self.assertEqual(v.t_start, 0.0)
+        self.assertEqual(len(seg1.spiketrains), p.size)
+
+    def test_get_spikes_with_gather(self, sim=sim):
+        t1 = 12.3
+        t2 = 13.4
+        t3 = 14.5
+        p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
+        p.record('v')
+        sim.run(t1)
+        sim.run(t2)
+        sim.reset()
+        p.record('spikes')
+        p.record('w')
+        sim.run(t3)
+        data = p.get_data(gather=True)
+        self.assertEqual(len(data.segments), 2)
+
+        seg0 = data.segments[0]
+        self.assertEqual(len(seg0.analogsignals), 1)
+        self.assertEqual(len(seg0.spiketrains), 0)
+
+        seg1 = data.segments[1]
+        self.assertEqual(len(seg1.analogsignals), 2)
+        self.assertEqual(len(seg1.spiketrains), p.size)
+        assert_array_equal(seg1.spiketrains[7],
+                           numpy.array([p.first_id + 7, p.first_id + 7 + 5]) % t3)
 
-    def test_printSpikes(self):
+    # def test_get_data_no_gather(self, sim=sim):
+    #    self.fail()
+
+    def test_printSpikes(self, sim=sim):
         # TODO: implement assert_deprecated
-        p = sim.Population(3, IF_cond_exp())
+        p = sim.Population(3, sim.IF_curr_alpha())
         p.record('spikes')
         sim.run(10.0)
         p.write_data = Mock()
         p.printSpikes("foo.txt")
         p.write_data.assert_called_with('foo.txt', 'spikes', True)
 
-    def test_getSpikes(self):
-        p = sim.Population(3, IF_cond_exp())
+    def test_getSpikes(self, sim=sim):
+        p = sim.Population(3, sim.IF_curr_alpha())
         p.record('spikes')
         sim.run(10.0)
         p.get_data = Mock()
         p.getSpikes()
         p.get_data.assert_called_with('spikes', True)
 
-    def test_print_v(self):
-        p = sim.Population(3, IF_cond_exp())
+    def test_print_v(self, sim=sim):
+        p = sim.Population(3, sim.IF_curr_alpha())
         p.record_v()
         sim.run(10.0)
         p.write_data = Mock()
         p.print_v("foo.txt")
         p.write_data.assert_called_with('foo.txt', 'v', True)
 
-    def test_get_v(self):
-        p = sim.Population(3, IF_cond_exp())
+    def test_get_v(self, sim=sim):
+        p = sim.Population(3, sim.IF_curr_alpha())
         p.record_v()
         sim.run(10.0)
         p.get_data = Mock()
         p.get_v()
         p.get_data.assert_called_with('v', True)
 
-    def test_get_spike_counts(self):
-        p = sim.Population(3, EIF_cond_exp_isfa_ista())
+    def test_print_gsyn(self, sim=sim):
+        p = sim.Population(3, sim.IF_cond_alpha())
+        p.record_gsyn()
+        sim.run(10.0)
+        p.write_data = Mock()
+        p.print_gsyn("foo.txt")
+        p.write_data.assert_called_with('foo.txt', ['gsyn_exc', 'gsyn_inh'], True)
+
+    def test_get_gsyn(self, sim=sim):
+        p = sim.Population(3, sim.IF_cond_alpha())
+        p.record_gsyn()
+        sim.run(10.0)
+        p.get_data = Mock()
+        p.get_gsyn()
+        p.get_data.assert_called_with(['gsyn_exc', 'gsyn_inh'], True)
+
+    def test_get_spike_counts(self, sim=sim):
+        p = sim.Population(3, sim.EIF_cond_exp_isfa_ista())
         p.record('spikes')
         sim.run(100.0)
         self.assertEqual(p.get_spike_counts(),
                          {p.all_cells[0]: 2,
-                          p.all_cells[1]: 2,
-                          p.all_cells[2]: 2})
+                             p.all_cells[1]: 2,
+                             p.all_cells[2]: 2})
 
-    def test_mean_spike_count(self):
-        p = sim.Population(14, EIF_cond_exp_isfa_ista())
+    def test_mean_spike_count(self, sim=sim):
+        p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
         p.record('spikes')
         sim.run(100.0)
+        # mock backend always produces two spikes per population
         self.assertEqual(p.mean_spike_count(), 2.0)
 
-    def test_meanSpikeCount(self):
-        p = sim.Population(14, EIF_cond_exp_isfa_ista())
+    # def test_mean_spike_count_on_slave_node():
+
+    def test_meanSpikeCount(self, sim=sim):
+        p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
         p.record('spikes')
         sim.run(100.0)
         p.mean_spike_count = Mock()
         p.meanSpikeCount()
         self.assertTrue(p.mean_spike_count.called)
 
-    def test_inject(self):
-        p = sim.Population(3, IF_cond_exp())
+    def test_inject(self, sim=sim):
+        p = sim.Population(3, sim.IF_curr_alpha())
         cs = Mock()
         p.inject(cs)
         meth, args, kwargs = cs.method_calls[0]
         self.assertEqual(meth, "inject_into")
         self.assertEqual(args, (p,))
 
-    def test_inject_into_invalid_celltype(self):
+    def test_inject_into_invalid_celltype(self, sim=sim):
         p = sim.Population(3, sim.SpikeSourceArray())
         self.assertRaises(TypeError, p.inject, Mock())
 
+    # def test_save_positions(self, sim=sim):
+    #    self.fail()
+
     # test describe method
-    def test_describe(self):
-        p = sim.Population(11, IF_cond_exp())
+
+    def test_describe(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
         self.assertIsInstance(p.describe(), basestring)
         self.assertIsInstance(p.describe(template=None), dict)
-        
-# ------------------------------------------
-# specific hardware test
-# ------------------------------------------
-    #def test_out_of_range_parameter_homogeneous(self):
-        #ifcell = IF_cond_exp(cm=0.2)
-        #self.assertRaises(ParameterValueOutOfRangeError, IF_cond_exp, cm=0.9)
-        
-    #def test_out_of_range_parameter_function(self):
-        #ifcell = IF_cond_exp(**{'cm': lambda i: 0.2 + 0.1*i})
-        #self.assertRaises(ParameterValueOutOfRangeError, sim.Population, 4, ifcell)     
-    
-    #def test_out_of_range_parameter_array_one_cell(self):
-        #self.assertRaises(ParameterValueOutOfRangeError, IF_cond_exp,**{'cm': numpy.array([0.9])})
-        
-    #def test_out_of_range_parameter_function_one_cell(self):
-        #ifcell = IF_cond_exp(**{'cm': lambda i: 0.3 + 0.1*i})
-        #self.assertRaises(ParameterValueOutOfRangeError, sim.Population, 1, ifcell)
-        
-    #def test_out_of_range_parameter_homogeneous_pop(self):
-        #self.assertRaises(ParameterValueOutOfRangeError, sim.Population, 4, IF_cond_exp(**{'cm': 0.9}))
-        
-    #def test_out_of_range_parameter_array_pop(self):
-        #self.assertRaises(ParameterValueOutOfRangeError, sim.Population, 4, IF_cond_exp(**{'cm': numpy.array([0.2, 0.2, 0.9, 0.2])}))
-        
-    #def test_out_of_range_parameter_function_pop(self):
-        #p = sim.Population(4, IF_cond_exp(**{'cm': lambda i: 0.2 + 0.0*i}))
-        #self.assertRaises(ParameterValueOutOfRangeError, sim.Population, 4, IF_cond_exp(**{'cm': lambda i: 0.2 + 0.1*i}))
+
+    def test_save_positions(self, sim=sim):
+        import os
+        p = sim.Population(4, sim.IF_cond_exp(), )
+        p.positions = numpy.arange(15, 27).reshape((4, 3)).T
+        output_file = Mock()
+        p.save_positions(output_file)
+        assert_array_equal(output_file.write.call_args[0][0],
+                           numpy.array([[0, 15, 16, 17],
+                                        [1, 18, 19, 20],
+                                        [2, 21, 22, 23],
+                                        [3, 24, 25, 26]]))
+        self.assertEqual(output_file.write.call_args[0][1], {'population': p.label})
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `PyNN-0.9.5/test/system/scenarios/__init__.py` & `PyNN-0.9.6/test/system/scenarios/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # encoding: utf-8
 from testconfig import config
 
-#import pdb
-#pdb.set_trace()
 
 if 'testFile' in config:
     file_name = config['testFile']
     exec("from . import ( %s )" % file_name)
 else:
     from . import ( scenario1,
                     scenario2,
```

### Comparing `PyNN-0.9.5/test/system/scenarios/issue231.py` & `PyNN-0.9.6/test/system/scenarios/issue231.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/issue274.py` & `PyNN-0.9.6/test/system/scenarios/issue274.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/scenario1.py` & `PyNN-0.9.6/test/system/scenarios/scenario1.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/scenario2.py` & `PyNN-0.9.6/test/system/scenarios/scenario2.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/scenario3.py` & `PyNN-0.9.6/test/system/scenarios/scenario3.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 from nose.tools import assert_equal
 from nose.plugins.skip import SkipTest
 from pyNN.utility import init_logging
 from pyNN.random import RandomDistribution
 from .registry import register
 
 
-@register(exclude=["moose", "nemo", "brian"])
+@register(exclude=["moose", "nemo", "brian", "brian2"])
 def scenario3(sim):
     """
     Simple feed-forward network network with additive STDP. The second half of
     the presynaptic neurons fires faster than the second half, so their
     connections should be potentiated more.
     """
+    try:
+        import scipy.stats
+    except ImportError:
+        raise SkipTest
 
     init_logging(logfile=None, debug=True)
     second = 1000.0
     duration = 10
     tau_m = 20  # ms
     cm = 1.0  # nF
     v_reset = -60
@@ -77,29 +81,21 @@
 
     sim.run(duration * second)
 
     actual_rate = pre.mean_spike_count() / duration
     expected_rate = (r1 + r2) / 2
     errmsg = "actual rate: %g  expected rate: %g" % (actual_rate, expected_rate)
     assert abs(actual_rate - expected_rate) < 1, errmsg
-    #assert abs(pre[:50].mean_spike_count()/duration - r1) < 1
-    #assert abs(pre[50:].mean_spike_count()/duration- r2) < 1
     final_weights = connections.get('weight', format='array', gather=False)
     assert initial_weights[0, 0] != final_weights[0, 0]
 
-    try:
-        import scipy.stats
-    except ImportError:
-        raise SkipTest
-    t, p = scipy.stats.ttest_ind(initial_weights[:50, :].flat, initial_weights[50:, :].flat)
-    assert p > 0.05, p
     t, p = scipy.stats.ttest_ind(final_weights[:50, :].flat, final_weights[50:, :].flat)
     assert p < 0.01, p
     assert final_weights[:50, :].mean() < final_weights[50:, :].mean()
     sim.end()
     return initial_weights, final_weights, pre, post, connections
-    
+
 
 if __name__ == '__main__':
     from pyNN.utility import get_simulator
     sim, args = get_simulator()
     scenario3(sim)
```

### Comparing `PyNN-0.9.5/test/system/scenarios/scenario4.py` & `PyNN-0.9.6/test/system/scenarios/scenario4.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pyNN.utility import init_logging
 from .registry import register
 
 
 logger = logging.getLogger("TEST")
 
 
-@register(exclude=["nemo"])
+@register(exclude=["nemo", "brian2"])  # to fix for Brian 2
 def scenario4(sim):
     """
     Network with spatial structure
     """
     init_logging(logfile=None, debug=True)
     sim.setup()
     rng = NumpyRNG(seed=76454, parallel_safe=False)
```

### Comparing `PyNN-0.9.5/test/system/scenarios/test_cell_types.py` & `PyNN-0.9.6/test/system/scenarios/test_cell_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     sim.setup(timestep=0.01, min_delay=0.1, max_delay=4.0)
     ifcell = sim.create(sim.EIF_cond_alpha_isfa_ista(
                             i_offset=1.0, tau_refrac=2.0, v_spike=-40))
     ifcell.record(['spikes', 'v', 'w'])
     ifcell.initialize(v=-65, w=0)
     sim.run(200.0)
     data = ifcell.get_data().segments[0]
-    expected_spike_times = numpy.array([10.02, 25.52, 43.18, 63.42, 86.67, 113.13, 142.69, 174.79])
+    expected_spike_times = numpy.array([10.015, 25.515, 43.168, 63.41, 86.649, 113.112, 142.663, 174.76])
     if plot_figure:
         import matplotlib.pyplot as plt
-        vm = data.analogsignals[0]
+        vm = data.filter(name="v")[0]
         plt.plot(vm.times, vm)
         plt.plot(expected_spike_times, -40 * numpy.ones_like(expected_spike_times), "ro")
         plt.savefig("test_EIF_cond_alpha_isfa_ista_%s.png" % sim.__name__)
     diff = (data.spiketrains[0].rescale(pq.ms).magnitude - expected_spike_times) / expected_spike_times
     assert abs(diff).max() < 0.01, abs(diff).max()
     sim.end()
     return data
@@ -58,21 +58,25 @@
         'i_offset': 1.0,
     }
     hhcell = sim.create(sim.HH_cond_exp(**cellparams))
     sim.initialize(hhcell, v=-64.0)
     hhcell.record('v')
     sim.run(20.0)
     v = hhcell.get_data().segments[0].filter(name='v')[0]
+    if plot_figure:
+        import matplotlib.pyplot as plt
+        plt.plot(v.times, v)
+        plt.savefig("test_HH_cond_exp_%s.png" % sim.__name__)
     sim.end()
     first_spike = v.times[numpy.where(v > 0)[0][0]]
     assert first_spike / pq.ms - 2.95 < 0.01
 test_HH_cond_exp.__test__ = False
 
 
-@register(exclude=['nemo', 'brian'])
+@register(exclude=['nemo', 'brian', 'brian2'])  # see issue 370
 def issue367(sim, plot_figure=False):
     # AdEx dynamics for delta_T=0
     sim.setup(timestep=0.001, min_delay=0.1, max_delay=4.0)
     v_thresh = -50
     ifcell = sim.create(sim.EIF_cond_exp_isfa_ista(
                         delta_T=0.0, i_offset=1.0, v_thresh=v_thresh, v_spike=-45))
     ifcell.record(('spikes', 'v'))
@@ -146,15 +150,15 @@
         print(expected_rate, expected_mean_isi, isi.mean(), p, D)
         assert_less(D, 0.1)
 
     return data
 test_SpikeSourcePoisson.__test__ = False
 
 
-@register(exclude=['brian'])
+@register(exclude=['brian','brian2'])
 def test_SpikeSourceGamma(sim, plot_figure=False):
     try:
         from scipy.stats import kstest
     except ImportError:
         raise SkipTest("scipy not available")
     sim.setup()
     params = {
@@ -202,15 +206,15 @@
         print(alpha, beta, expected_mean_isi, isi.mean(), p, D)
         assert_less(D, 0.1)
 
     return data
 test_SpikeSourceGamma.__test__ = False
 
 
-@register(exclude=['brian'])
+@register(exclude=['brian','brian2'])
 def test_SpikeSourcePoissonRefractory(sim, plot_figure=False):
     try:
         from scipy.stats import kstest
     except ImportError:
         raise SkipTest("scipy not available")
     sim.setup()
     params = {
```

### Comparing `PyNN-0.9.5/test/system/scenarios/test_connectors.py` & `PyNN-0.9.6/test/system/scenarios/test_connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                  sorted(prj_fp1.get('weight', format='list', gather=False)))
     assert_equal(sorted(prj_a2a.get('delay', format='list', gather=False)),
                  sorted(prj_fp1.get('delay', format='list', gather=False)))
     assert_equal(prj_fp1.size(), 20)  # 20 rather than 25 because self-connections are excluded
     sim.end()
 
 
-@register(exclude=['brian'])
+@register(exclude=['brian', 'brian2'])  # need to implement projection.get() for pre/post assemblies in Brian
 def issue622(sim):
     sim.setup()
     pop = sim.Population(10, sim.IF_cond_exp, {}, label="pop")
 
     view1 = sim.PopulationView(pop, [2, 3, 4])
     view2 = sim.PopulationView(pop, [2, 3, 4])
```

### Comparing `PyNN-0.9.5/test/system/scenarios/test_electrodes.py` & `PyNN-0.9.6/test/system/scenarios/test_electrodes.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/test_parameter_handling.py` & `PyNN-0.9.6/test/system/scenarios/test_parameter_handling.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/test_procedural_api.py` & `PyNN-0.9.6/test/system/scenarios/test_procedural_api.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/scenarios/test_recording.py` & `PyNN-0.9.6/test/system/scenarios/test_recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     assert_array_equal(gsyn_p1.channel_index.channel_ids, numpy.arange(4))
     assert_array_equal(gsyn_all.channel_index.channel_ids, numpy.arange(2, 9))
 
     sim.end()
 test_record_vm_and_gsyn_from_assembly.__test__ = False
 
 
-@register(exclude='brian')  # brian does not support off_grid. To fix?
+@register(exclude=["brian", "brian2"])  # brian does not support off_grid. To fix?
 def issue259(sim):
     """
     A test that retrieving data with "clear=True" gives correct spike trains.
     """
     sim.setup(timestep=0.05, spike_precision="off_grid")
     p = sim.Population(1, sim.SpikeSourceArray(spike_times=[0.075, 10.025, 12.34, 1000.025]))
     p.record('spikes')
@@ -162,15 +162,15 @@
                        data_oo.segments[0].analogsignals[0])
 
     os.remove(fn_proc)
     os.remove(fn_oo)
 test_mix_procedural_and_oo.__test__ = False
 
 
-@register(exclude=['brian'])  # todo: known to fail with Brian, but should work
+@register(exclude=['brian', 'brian2'])  # todo: known to fail with Brian, but should work
 def test_record_with_filename(sim):
     """
     Test to ensure that Simulator and Population recording work properly
     The following 12 scenarios are explored:
         Note: var1 = "spikes", var2 = "v"
         1) sim.record()
             i) cell[0]
```

### Comparing `PyNN-0.9.5/test/system/scenarios/test_simulation_control.py` & `PyNN-0.9.6/test/system/scenarios/test_simulation_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     data = p.get_data(clear=False)
     sim.end()
 
     assert len(data.segments) == repeats
     for segment in data.segments[1:]:
         assert_array_almost_equal(segment.analogsignals[0],
                                   data.segments[0].analogsignals[0], 10)
+        
 test_reset.__test__ = False
 
 
 @register()
 def test_reset_with_clear(sim):
     """
     Run the same simulation n times without recreating the network,
```

### Comparing `PyNN-0.9.5/test/system/scenarios/test_synapse_types.py` & `PyNN-0.9.6/test/system/scenarios/test_synapse_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except ImportError:
     have_scipy = False
 from nose.tools import assert_equal, assert_less, assert_greater, assert_not_equal
 
 from .registry import register
 
 
-@register(exclude=['moose', 'nemo', 'brian'])
+@register(exclude=['moose', 'nemo', 'brian', 'brian2'])
 def test_simple_stochastic_synapse(sim, plot_figure=False):
     # in this test we connect
     sim.setup(min_delay=0.5)
     t_stop = 1000.0
     spike_times = np.arange(2.5, t_stop, 5.0)
     source = sim.Population(1, sim.SpikeSourceArray(spike_times=spike_times))
     neurons = sim.Population(4, sim.IF_cond_exp(tau_syn_E=1.0))
```

### Comparing `PyNN-0.9.5/test/system/scenarios/ticket166.py` & `PyNN-0.9.6/test/system/scenarios/ticket166.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/test_brian.py` & `PyNN-0.9.6/test/system/test_brian.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/test_hardware_brainscales.py` & `PyNN-0.9.6/test/system/test_hardware_brainscales.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/test_moose.py` & `PyNN-0.9.6/test/system/test_moose.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/test_nest.py` & `PyNN-0.9.6/test/system/test_nest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from nose.plugins.skip import SkipTest
 from .scenarios.registry import registry
-from nose.tools import assert_equal, assert_not_equal
+from nose.tools import assert_equal, assert_not_equal, assert_raises
 from pyNN.utility import init_logging, assert_arrays_equal
+from pyNN.random import RandomDistribution
 import numpy
 
 try:
     import pyNN.nest
     have_nest = True
 except ImportError:
     have_nest = False
@@ -266,10 +267,66 @@
     ]
 
     ee_connector = sim.FromListConnector(connections, column_names=["weight"])
 
     prj_plastic = sim.Projection(p1, p2, ee_connector, receptor_type='excitatory', synapse_type=stdp)
 
 
+def test_issue662a():
+    """Setting tau_minus to a random distribution fails..."""
+    if not have_nest:
+        raise SkipTest
+    import nest
+    sim = pyNN.nest
+
+    sim.setup()
+    p1 = sim.Population(5, sim.SpikeSourcePoisson(rate=100.0))
+    p2 = sim.Population(10, sim.IF_cond_exp())
+
+    syn = sim.STDPMechanism(
+        timing_dependence=sim.SpikePairRule(
+            A_plus = 0.2,
+            A_minus = 0.1,
+            tau_minus = RandomDistribution('uniform', (20,40)),
+            tau_plus = RandomDistribution('uniform', (10,20))
+        ),
+        weight_dependence=sim.AdditiveWeightDependence(w_min=0.0, w_max=0.01)
+    )
+
+    assert_raises(ValueError, sim.Projection, p1, p2, sim.AllToAllConnector(),
+                  synapse_type=syn, receptor_type='excitatory')
+
+
+def test_issue662b():
+    """Setting tau_minus to a random distribution fails..."""
+    if not have_nest:
+        raise SkipTest
+    import nest
+    sim = pyNN.nest
+
+    sim.setup(min_delay=0.5)
+    p1 = sim.Population(5, sim.SpikeSourcePoisson(rate=100.0))
+    p2 = sim.Population(10, sim.IF_cond_exp())
+
+    syn = sim.STDPMechanism(
+        timing_dependence=sim.SpikePairRule(
+            A_plus = 0.2,
+            A_minus = 0.1,
+            tau_minus = 30,
+            tau_plus = RandomDistribution('uniform', (10,20))
+        ),
+        weight_dependence=sim.AdditiveWeightDependence(w_min=0.0, w_max=0.01),
+        weight=0.005
+    )
+
+    connections = sim.Projection(p1, p2, sim.AllToAllConnector(),
+                                 synapse_type=syn,
+                                 receptor_type='inhibitory')
+
+    connections.set(tau_minus=25)  #RandomDistribution('uniform', (20,40)))
+    # todo: check this worked
+    assert_raises(ValueError, connections.set, tau_minus=RandomDistribution('uniform', (20,40)))
+
+
 if __name__ == '__main__':
     #data = test_random_seeds()
     test_native_electrode_types()
```

### Comparing `PyNN-0.9.5/test/system/test_neuroml.py` & `PyNN-0.9.6/test/system/test_neuroml.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/system/test_neuron.py` & `PyNN-0.9.6/test/system/test_neuron.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,22 +179,24 @@
     syn = nrn.StaticSynapse(weight=0.1)
     prj_alpha = nrn.Projection(p2, p1, connector, syn, receptor_type='apical.ampa')
 
     nrn.run(250.0)
 
     data = p1.get_data().segments[0].analogsignals
     assert_equal(len(data), 2)  # one array per variable
-    assert_equal(data[0].name, 'apical(1.0).v')
-    assert_equal(data[1].name, 'soma(0.5).ina')
-    assert_equal(data[0].sampling_rate, 10.0 * pq.kHz)
-    assert_equal(data[0].units, pq.mV)
-    assert_equal(data[1].units, pq.mA / pq.cm**2)
-    assert_equal(data[0].t_start, 0.0 * pq.ms)
-    assert_equal(data[0].t_stop, 250.1 * pq.ms)  # would prefer if it were 250.0, but this is a fundamental Neo issue
-    assert_equal(data[0].shape, (2501, 10))
+    names = set(sig.name for sig in data)
+    assert_equal(names, set(('apical(1.0).v', 'soma(0.5).ina')))
+    apical_v = [sig for sig in data if sig.name == 'apical(1.0).v'][0]
+    soma_i = [sig for sig in data if sig.name == 'soma(0.5).ina'][0]
+    assert_equal(apical_v.sampling_rate, 10.0 * pq.kHz)
+    assert_equal(apical_v.units, pq.mV)
+    assert_equal(soma_i.units, pq.mA / pq.cm**2)
+    assert_equal(apical_v.t_start, 0.0 * pq.ms)
+    assert_equal(apical_v.t_stop, 250.1 * pq.ms)  # would prefer if it were 250.0, but this is a fundamental Neo issue
+    assert_equal(apical_v.shape, (2501, 10))
     return data
 
 
 def test_tsodyks_markram_synapse():
     if not have_neuron:
         raise SkipTest
     sim = pyNN.neuron
```

### Comparing `PyNN-0.9.5/test/system/test_serialization.py` & `PyNN-0.9.6/test/system/test_serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 
-
+from nose.plugins.skip import SkipTest
 from numpy.testing import assert_array_almost_equal
 
 import pyNN.nest as sim
 from pyNN.random import RandomDistribution as RD
 from pyNN.network import Network
 from pyNN.serialization import export_to_sonata, import_from_sonata, asciify
 
+try:
+    import h5py
+    HAVE_H5PY = True
+except ImportError:
+    HAVE_H5PY = False
+
 
 def test():
+    if not HAVE_H5PY:
+        raise SkipTest
+
     sim.setup()
 
     p1 = sim.Population(10,
                         sim.IF_cond_exp(
                             v_rest=-65,
                             tau_m=lambda i: 10 + 0.1*i,
                             cm=RD('normal', (0.5, 0.05))),
```

### Comparing `PyNN-0.9.5/test/unittests/test_assembly.py` & `PyNN-0.9.6/test/unittests/test_assembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tests of the common implementation of the Assembly class, using the pyNN.mock
 backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
```

### Comparing `PyNN-0.9.5/test/unittests/test_brian.py` & `PyNN-0.9.6/test/unittests/test_brian.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_connectors_parallel.py` & `PyNN-0.9.6/test/unittests/test_connectors_serial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Tests of the Connector classes, using the pyNN.mock backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 from pyNN import connectors, random, errors, space, recording
 import numpy
+from numpy import nan
 import os
 import sys
 from numpy.testing import assert_array_equal, assert_array_almost_equal
-from .mocks import MockRNG, MockRNG2
+from .mocks import MockRNG, MockRNG2, MockRNG3
 import pyNN.mock as sim
 
 
 orig_mpi_get_config = random.get_mpi_config
 
 
 def setUp():
@@ -29,153 +30,218 @@
 def tearDown():
     random.get_mpi_config = orig_mpi_get_config
 
 
 class TestOneToOneConnector(unittest.TestCase):
 
     def setUp(self, sim=sim, **extra):
-        sim.setup(num_processes=2, rank=0, **extra)
+        sim.setup(**extra)
         self.p1 = sim.Population(5, sim.IF_cond_exp())
         self.p2 = sim.Population(5, sim.HH_cond_exp())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
 
     def tearDown(self, sim=sim):
         sim.end()
 
     def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         C = connectors.OneToOneConnector(safe=False)
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(1, 1, 5.0, 0.5),
-                          (3, 3, 5.0, 0.5)])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 5.0, 0.5),
+                          (1, 1, 5.0, 0.5),
+                          (2, 2, 5.0, 0.5),
+                          (3, 3, 5.0, 0.5),
+                          (4, 4, 5.0, 0.5)])
 
     def test_connect_with_random_weights(self, sim=sim):
         rd = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(delta=1.0))
         syn = sim.StaticSynapse(weight=rd, delay=0.5)
         C = connectors.OneToOneConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(1, 1, 1.0, 0.5),
-                          (3, 3, 3.0, 0.5)])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.5),
+                          (1, 1, 1.0, 0.5),
+                          (2, 2, 2.0, 0.5),
+                          (3, 3, 3.0, 0.5),
+                          (4, 4, 4.0, 0.5)])
 
 
 class TestAllToAllConnector(unittest.TestCase):
 
     def setUp(self, sim=sim, **extra):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p1._mask_local, numpy.array([0, 1, 0, 1], dtype=bool))
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
 
     def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         C = connectors.AllToAllConnector(safe=False)
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 5.0, 0.5),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 5.0, 0.5),
+                          (1, 0, 5.0, 0.5),
+                          (2, 0, 5.0, 0.5),
+                          (3, 0, 5.0, 0.5),
+                          (0, 1, 5.0, 0.5),
                           (1, 1, 5.0, 0.5),
                           (2, 1, 5.0, 0.5),
                           (3, 1, 5.0, 0.5),
+                          (0, 2, 5.0, 0.5),
+                          (1, 2, 5.0, 0.5),
+                          (2, 2, 5.0, 0.5),
+                          (3, 2, 5.0, 0.5),
                           (0, 3, 5.0, 0.5),
                           (1, 3, 5.0, 0.5),
                           (2, 3, 5.0, 0.5),
-                          (3, 3, 5.0, 0.5)])
-        nan = numpy.nan
-        assert_array_equal(prj.get('weight', format='array', gather=False),
-                           numpy.array([[nan, 5.0, nan, 5.0, nan],
-                                        [nan, 5.0, nan, 5.0, nan],
-                                        [nan, 5.0, nan, 5.0, nan],
-                                        [nan, 5.0, nan, 5.0, nan]]))
+                          (3, 3, 5.0, 0.5),
+                          (0, 4, 5.0, 0.5),
+                          (1, 4, 5.0, 0.5),
+                          (2, 4, 5.0, 0.5),
+                          (3, 4, 5.0, 0.5)])
+        assert_array_equal(prj.get('weight', format='array'),
+                           numpy.array([[5.0, 5.0, 5.0, 5.0, 5.0],
+                                        [5.0, 5.0, 5.0, 5.0, 5.0],
+                                        [5.0, 5.0, 5.0, 5.0, 5.0],
+                                        [5.0, 5.0, 5.0, 5.0, 5.0]]))
 
     def test_connect_with_array_weights(self, sim=sim):
         C = connectors.AllToAllConnector(safe=False)
         syn = sim.StaticSynapse(weight=numpy.arange(0.0, 2.0, 0.1).reshape(4, 5), delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         assert_array_almost_equal(
-            # use gather False because we are faking the MPI
-            numpy.array(prj.get(["weight", "delay"], format='list', gather=False)),
-            numpy.array([(0, 1, 0.1, 0.5),
-                         (1, 1, 0.6, 0.5),
-                         (2, 1, 1.1, 0.5),
-                         (3, 1, 1.6, 0.5),
-                         (0, 3, 0.3, 0.5),
-                         (1, 3, 0.8, 0.5),
-                         (2, 3, 1.3, 0.5),
-                         (3, 3, 1.8, 0.5)]))
-        nan = numpy.nan
-        assert_array_almost_equal(prj.get('weight', format='array', gather=False),
-                                  numpy.array([[nan, 0.1, nan, 0.3, nan],
-                                               [nan, 0.6, nan, 0.8, nan],
-                                               [nan, 1.1, nan, 1.3, nan],
-                                               [nan, 1.6, nan, 1.8, nan]]),
+            numpy.array(prj.get(["weight", "delay"], format='list')),
+            numpy.array([
+                        (0, 0, 0.0, 0.5),
+                        (1, 0, 0.5, 0.5),
+                        (2, 0, 1.0, 0.5),
+                        (3, 0, 1.5, 0.5),
+                        (0, 1, 0.1, 0.5),
+                        (1, 1, 0.6, 0.5),
+                        (2, 1, 1.1, 0.5),
+                        (3, 1, 1.6, 0.5),
+                        (0, 2, 0.2, 0.5),
+                        (1, 2, 0.7, 0.5),
+                        (2, 2, 1.2, 0.5),
+                        (3, 2, 1.7, 0.5),
+                        (0, 3, 0.3, 0.5),
+                        (1, 3, 0.8, 0.5),
+                        (2, 3, 1.3, 0.5),
+                        (3, 3, 1.8, 0.5),
+                        (0, 4, 0.4, 0.5),
+                        (1, 4, 0.9, 0.5),
+                        (2, 4, 1.4, 0.5),
+                        (3, 4, 1.9, 0.5)]
+                        )
+        )
+        assert_array_almost_equal(prj.get('weight', format='array'),
+                                  numpy.array([[0.,  0.1,  0.2,  0.3,  0.4],
+                                               [0.5,  0.6,  0.7,  0.8,  0.9],
+                                               [1.,  1.1,  1.2,  1.3,  1.4],
+                                               [1.5,  1.6,  1.7,  1.8,  1.9]]),
                                   9)
 
     def test_connect_with_random_weights_parallel_safe(self, sim=sim):
         rd = random.RandomDistribution(
             'uniform', (0, 1), rng=MockRNG(delta=1.0, parallel_safe=True))
         syn = sim.StaticSynapse(weight=rd, delay=0.5)
         C = connectors.AllToAllConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
         # note that the outer loop is over the post-synaptic cells, the inner loop over the pre-synaptic
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 4.0, 0.5),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.5),
+                          (1, 0, 1.0, 0.5),
+                          (2, 0, 2.0, 0.5),
+                          (3, 0, 3.0, 0.5),
+                          (0, 1, 4.0, 0.5),
                           (1, 1, 5.0, 0.5),
                           (2, 1, 6.0, 0.5),
                           (3, 1, 7.0, 0.5),
+                          (0, 2, 8.0, 0.5),
+                          (1, 2, 9.0, 0.5),
+                          (2, 2, 10.0, 0.5),
+                          (3, 2, 11.0, 0.5),
                           (0, 3, 12.0, 0.5),
                           (1, 3, 13.0, 0.5),
                           (2, 3, 14.0, 0.5),
-                          (3, 3, 15.0, 0.5)])
-        nan = numpy.nan
-        assert_array_almost_equal(prj.get('weight', format='array', gather=False),
-                                  numpy.array([[nan, 4.0, nan, 12.0, nan],
-                                               [nan, 5.0, nan, 13.0, nan],
-                                               [nan, 6.0, nan, 14.0, nan],
-                                               [nan, 7.0, nan, 15.0, nan]]),
+                          (3, 3, 15.0, 0.5),
+                          (0, 4, 16.0, 0.5),
+                          (1, 4, 17.0, 0.5),
+                          (2, 4, 18.0, 0.5),
+                          (3, 4, 19.0, 0.5)])
+        assert_array_almost_equal(prj.get('weight', format='array'),
+                                  numpy.array([[0., 4.,  8., 12., 16.],
+                                               [1., 5.,  9., 13., 17.],
+                                               [2., 6., 10., 14., 18.],
+                                               [3., 7., 11., 15., 19.]]),
                                   9)
 
     def test_connect_with_distance_dependent_weights(self, sim=sim):
         d_expr = "d+100"
         syn = sim.StaticSynapse(weight=d_expr, delay=0.5)
         C = connectors.AllToAllConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 101.0, 0.5),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 100.0, 0.5),
+                          (1, 0, 101.0, 0.5),
+                          (2, 0, 102.0, 0.5),
+                          (3, 0, 103.0, 0.5),
+                          (0, 1, 101.0, 0.5),
                           (1, 1, 100.0, 0.5),
                           (2, 1, 101.0, 0.5),
                           (3, 1, 102.0, 0.5),
+                          (0, 2, 102.0, 0.5),
+                          (1, 2, 101.0, 0.5),
+                          (2, 2, 100.0, 0.5),
+                          (3, 2, 101.0, 0.5),
                           (0, 3, 103.0, 0.5),
                           (1, 3, 102.0, 0.5),
                           (2, 3, 101.0, 0.5),
-                          (3, 3, 100.0, 0.5)])
+                          (3, 3, 100.0, 0.5),
+                          (0, 4, 104.0, 0.5),
+                          (1, 4, 103.0, 0.5),
+                          (2, 4, 102.0, 0.5),
+                          (3, 4, 101.0, 0.5)])
 
     def test_connect_with_distance_dependent_weights_and_delays(self, sim=sim):
         syn = sim.StaticSynapse(weight="d+100", delay="0.2+2*d")
         C = connectors.AllToAllConnector(safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 101.0, 2.2),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 100.0, 0.2),
+                          (1, 0, 101.0, 2.2),
+                          (2, 0, 102.0, 4.2),
+                          (3, 0, 103.0, 6.2),
+                          (0, 1, 101.0, 2.2),
                           (1, 1, 100.0, 0.2),
                           (2, 1, 101.0, 2.2),
                           (3, 1, 102.0, 4.2),
+                          (0, 2, 102.0, 4.2),
+                          (1, 2, 101.0, 2.2),
+                          (2, 2, 100.0, 0.2),
+                          (3, 2, 101.0, 2.2),
                           (0, 3, 103.0, 6.2),
                           (1, 3, 102.0, 4.2),
                           (2, 3, 101.0, 2.2),
-                          (3, 3, 100.0, 0.2)])
+                          (3, 3, 100.0, 0.2),
+                          (0, 4, 104.0, 8.2),
+                          (1, 4, 103.0, 6.2),
+                          (2, 4, 102.0, 4.2),
+                          (3, 4, 101.0, 2.2)])
 
     def test_connect_with_delays_None(self, sim=sim):
         syn = sim.StaticSynapse(weight=0.1, delay=None)
         C = connectors.AllToAllConnector()
         assert C.safe
         assert C.allow_self_connections
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False)[
-                         0][3], prj._simulator.state.min_delay)
+        self.assertEqual(prj.get(["weight", "delay"], format='list')
+                         [0][3], prj._simulator.state.min_delay)
 
     @unittest.skip('skipping this tests until I figure out how I want to refactor checks')
     def test_connect_with_delays_too_small(self, sim=sim):
         C = connectors.AllToAllConnector()
         syn = sim.StaticSynapse(weight=0.1, delay=0.0)
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, self.p2, C, syn)
 
@@ -186,177 +252,240 @@
         syn = sim.StaticSynapse(weight=0.1, delay=delays)
         C = connectors.AllToAllConnector()
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, self.p2, C, syn)
 
 
 class TestFixedProbabilityConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
 
     def test_connect_with_default_args(self, sim=sim):
         C = connectors.FixedProbabilityConnector(p_connect=0.85,
                                                  rng=MockRNG(delta=0.1, parallel_safe=True))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
 
         # 20 possible connections. Due to the mock RNG, only the
         # first 9 are created (0,0), (1,0), (2,0), (3,0), (0,1), (1,1), (2,1), (3,1), (0,2)
-        # of these, (0,1), (1,1), (2,1), (3,1) are created on this node
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123)])
+                          (3, 1, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123)
+                          ])
 
     def test_connect_with_default_args_again(self, sim=sim):
         C = connectors.FixedProbabilityConnector(p_connect=0.5,
                                                  rng=MockRNG2(1 - numpy.array([1, 0, 0, 1,
                                                                                0, 0, 0, 1,
                                                                                1, 1, 0, 0,
                                                                                1, 0, 1, 0,
                                                                                1, 1, 0, 1]),
                                                               parallel_safe=True))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
 
         # 20 possible connections. Due to the mock RNG, only the following
         # are created (0,0), (3,0), (3,1), (0,2), (1,2), (0,3), (2,3), (0,4), (1,4), (3,4)
-        # of these, (3,1), (0,3), (2,3) are created on this node
         # (note that the outer loop is over post-synaptic cells (columns), the inner loop over pre-synaptic (rows))
-        nan = numpy.nan
-        assert_array_almost_equal(prj.get('delay', format='array', gather=False),
-                                  numpy.array([[nan, nan,   nan, 0.123, nan],
-                                               [nan, nan,   nan, nan,   nan],
-                                               [nan, nan,   nan, 0.123, nan],
-                                               [nan, 0.123, nan, nan,   nan]]),
+        assert_array_almost_equal(prj.get('delay', format='array'),
+                                  numpy.array([[0.123,   nan, 0.123, 0.123, 0.123],
+                                               [nan,   nan, 0.123,   nan, 0.123],
+                                               [nan,   nan,   nan, 0.123,   nan],
+                                               [0.123, 0.123,   nan,   nan, 0.123]]),
                                   9)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(3, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123)])
+                          (2, 3, 0.0, 0.123),
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123)
+                          ])
 
-    def test_connect_with_probability_1(self, sim=sim):
-        # see https://github.com/NeuralEnsemble/PyNN/issues/309
-        C = connectors.FixedProbabilityConnector(p_connect=1,
-                                                 rng=MockRNG(delta=0.01, parallel_safe=True))
+    def test_connect_with_probability_one(self, sim=sim):
+        C = connectors.FixedProbabilityConnector(p_connect=1.)
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-
-        # 20 connections, only some of which are created on this node
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
                           (1, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (3, 3, 0.0, 0.123)
+                          (3, 3, 0.0, 0.123),
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
                           ])
 
+    def test_connect_weight_function_and_one_post_synaptic_neuron_not_connected(self, sim=sim):
+        C = connectors.FixedProbabilityConnector(p_connect=0.8,
+                                                 rng=MockRNG(delta=0.05))
+        syn = sim.StaticSynapse(weight=lambda d: 0.1 * d)
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        assert_array_almost_equal(prj.get(["weight", "delay"], format='array'),
+                                  numpy.array([
+                                      [[0., 0.1, 0.2, 0.3, nan],
+                                       [0.1,  0., 0.1, 0.2, nan],
+                                          [0.2, 0.1, 0.0, 0.1, nan],
+                                          [0.3, 0.2, 0.1, 0.0, nan]],
+                                      [[0.123, 0.123, 0.123, 0.123, nan],
+                                       [0.123, 0.123,   0.123, 0.123, nan],
+                                       [0.123, 0.123,   0.123, 0.123, nan],
+                                       [0.123, 0.123,   0.123, 0.123, nan]]
+                                  ]),
+                                  9)
+
     def test_connect_with_weight_function(self, sim=sim):
         C = connectors.FixedProbabilityConnector(p_connect=0.85,
                                                  rng=MockRNG(delta=0.1))
         syn = sim.StaticSynapse(weight=lambda d: 0.1 * d)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.1, 0.123),
-                          (1, 1, 0.0, 0.123),
-                          (2, 1, 0.1, 0.123),
-                          (3, 1, 0.2, 0.123)])
+
+        # 20 possible connections. Due to the mock RNG, only the
+        # first 9 are created (0,0), (1,0), (2,0), (3,0), (0,1), (1,1), (2,1), (3,1), (0,2)
+        assert_array_almost_equal(prj.get(["weight", "delay"], format='array'),
+                                  numpy.array([
+                                      [[0., 0.1, 0.2, nan, nan],
+                                       [0.1,  0., nan, nan, nan],
+                                          [0.2, 0.1, nan, nan, nan],
+                                          [0.3, 0.2, nan, nan, nan]],
+                                      [[0.123, 0.123, 0.123, nan, nan],
+                                       [0.123, 0.123,   nan, nan, nan],
+                                       [0.123, 0.123,   nan, nan, nan],
+                                       [0.123, 0.123,   nan, nan, nan]]
+                                  ]),
+                                  9)
 
     def test_connect_with_random_delays_parallel_safe(self, sim=sim):
         rd = random.RandomDistribution('uniform', low=0.1, high=1.1,
                                        rng=MockRNG(start=1.0, delta=0.2, parallel_safe=True))
         syn = sim.StaticSynapse(delay=rd)
         C = connectors.FixedProbabilityConnector(p_connect=0.5,
                                                  rng=MockRNG2(1 - numpy.array([1, 0, 0, 1,
                                                                                0, 0, 0, 1,
                                                                                1, 1, 0, 0,
                                                                                1, 0, 1, 0,
                                                                                1, 1, 0, 1]),
                                                               parallel_safe=True))
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        nan = numpy.nan
-        assert_array_almost_equal(prj.get('delay', format='array', gather=False),
-                                  numpy.array([[nan, nan, nan, 2.0, nan],
-                                               [nan, nan, nan, nan, nan],
-                                               [nan, nan, nan, 2.2, nan],
-                                               [nan, 1.4, nan, nan, nan]]),
+        # 20 possible connections. Due to the mock RNG, only the following
+        # are created (0,0), (3,0), (3,1), (0,2), (1,2), (0,3), (2,3), (0,4), (1,4), (3,4)
+        # (note that the outer loop is over post-synaptic cells (columns), the inner loop over pre-synaptic (rows))
+        assert_array_almost_equal(prj.get('delay', format='array'),
+                                  numpy.array([[1.0,   nan,   1.6,   2.0,   2.4],
+                                               [nan,   nan,   1.8,   nan,   2.6],
+                                               [nan,   nan,   nan,   2.2,   nan],
+                                               [1.2,   1.4,   nan,   nan,   2.8]]),
                                   9)
 
-    # def test_connect_with_random_delays_parallel_unsafe(self, sim=sim):
-    #    rd = random.RandomDistribution('uniform', [0.1, 1.1], rng=MockRNG(start=1.0, delta=0.2, parallel_safe=False))
-    #    syn = sim.StaticSynapse(delay=rd)
-    #    C = connectors.FixedProbabilityConnector(p_connect=0.5,
-    #                                             rng=MockRNG2(1 - numpy.array([1, 0, 0, 1,
-    #                                                                           0, 0, 0, 1,
-    #                                                                           1, 1, 0, 0,
-    #                                                                           1, 0, 1, 0,
-    #                                                                           1, 1, 0, 1]),
-    #                                                          parallel_safe=False))
-    #    prj = sim.Projection(self.p1, self.p2, C, syn)
-    #    nan = numpy.nan
-    #    assert_array_almost_equal(prj.get('delay', format='array', gather=False),
-    #                              numpy.array([[nan, nan, nan, 1.2, nan],
-    #                                           [nan, nan, nan, nan, nan],
-    #                                           [nan, nan, nan, 1.4, nan],
-    #                                           [nan, 1.0, nan, nan, nan]]),
-    #                              9)
-
 
 class TestDistanceDependentProbabilityConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
 
     def test_connect_with_default_args(self, sim=sim):
         C = connectors.DistanceDependentProbabilityConnector(d_expression="d<1.5",
                                                              rng=MockRNG(delta=0.01))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
         # 20 possible connections. Only those with a sufficiently small distance
         # are created
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (3, 3, 0.0, 0.123)])
+                          (3, 3, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123)])
 
 
 class TestFromListConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
+
+    def test_connect_unique_connection_neuron_0_to_neuron_0(self, sim=sim):
+        connection_list = [
+            (0, 0, 0.1, 0.18)
+        ]
+        C = connectors.FromListConnector(connection_list)
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.1, 0.18)])
+
+    def test_connect_with_empty_list(self, sim=sim):
+        connection_list = []
+        C = connectors.FromListConnector(connection_list)
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [])
 
     def test_connect_with_valid_list(self, sim=sim):
         connection_list = [
-            (0, 0, 0.1, 0.1),
-            (3, 0, 0.2, 0.11),
-            (2, 3, 0.3, 0.12),  # local
-            (2, 2, 0.4, 0.13),
+            (0, 0, 0.1, 0.18),
+            (3, 0, 0.2, 0.17),
+            (2, 3, 0.3, 0.16),  # local
+            (2, 2, 0.4, 0.15),
             (0, 1, 0.5, 0.14),  # local
         ]
         C = connectors.FromListConnector(connection_list)
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.5, 0.14),
-                          (2, 3, 0.3, 0.12)])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.1, 0.18),
+                          (3, 0, 0.2, 0.17),
+                          (0, 1, 0.5, 0.14),
+                          (2, 2, 0.4, 0.15),
+                          (2, 3, 0.3, 0.16)])
 
     def test_connect_with_out_of_range_index(self, sim=sim):
         connection_list = [
             (0, 0, 0.1, 0.1),
             (3, 0, 0.2, 0.11),
             (2, 3, 0.3, 0.12),  # local
             (5, 1, 0.4, 0.13),  # NON-EXISTENT
@@ -374,74 +503,52 @@
             (2, 2, 0.4, 0.13, 103, 700),
             (0, 1, 0.5, 0.14, 104, 800),  # local
         ]
         C = connectors.FromListConnector(connection_list, column_names=[
                                          "weight", "delay", "U", "tau_rec"])
         syn = sim.TsodyksMarkramSynapse(U=99, tau_facil=88.8)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay", "tau_facil", "tau_rec", "U"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.5, 0.14, 88.8, 800.0, 104.0),
+        self.assertEqual(prj.get(["weight", "delay", "tau_facil", "tau_rec", "U"], format='list'),
+                         [(0, 0, 0.1, 0.1, 88.8, 400.0, 100.0),
+                          (3, 0, 0.2, 0.11, 88.8, 500.0, 101.0),
+                          (0, 1, 0.5, 0.14, 88.8, 800.0, 104.0),
+                          (2, 2, 0.4, 0.13, 88.8, 700.0, 103.0),
                           (2, 3, 0.3, 0.12, 88.8, 600.0, 102.0)])
 
-    def test_with_stdp_synapse(self, sim=sim):
-        connection_list = [
-            (0, 0, 0.1, 0.1, 10.0, 0.4),
-            (3, 0, 0.2, 0.11, 10.1, 0.5),
-            (2, 3, 0.3, 0.12, 10.2, 0.6),  # local
-            (2, 2, 0.4, 0.13, 10.3, 0.7),
-            (0, 1, 0.5, 0.14, 10.4, 0.8),  # local
-        ]
-        C = connectors.FromListConnector(connection_list, column_names=[
-                                         "weight", "delay", "tau_plus", "w_max"])
-        syn = sim.STDPMechanism(timing_dependence=sim.SpikePairRule(tau_plus=12.3, tau_minus=33.3),
-                                weight_dependence=sim.MultiplicativeWeightDependence(w_max=1.11),
-                                weight=0.321, delay=0.2)
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay", "tau_plus", "tau_minus", "w_max"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.5, 0.14, 10.4, 33.3, 0.8),
-                          (2, 3, 0.3, 0.12, 10.2, 33.3, 0.6)])
-
 
 class TestFromFileConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
         self.connection_list = [
             (0, 0, 0.1, 0.1),
             (3, 0, 0.2, 0.11),
             (2, 3, 0.3, 0.12),  # local
             (2, 2, 0.4, 0.13),
             (0, 1, 0.5, 0.14),  # local
         ]
 
     def tearDown(self, sim=sim):
+        sim.end()
         for path in ("test.connections", "test.connections.1", "test.connections.2"):
             if os.path.exists(path):
                 os.remove(path)
 
     def test_connect_with_standard_text_file_not_distributed(self, sim=sim):
         numpy.savetxt("test.connections", self.connection_list)
         C = connectors.FromFileConnector("test.connections", distributed=False)
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.5, 0.14),
-                          (2, 3, 0.3, 0.12)])
-
-    def test_connect_with_standard_text_file_distributed(self, sim=sim):
-        local_connection_list = [c for c in self.connection_list if c[1] % 2 == 1]
-        numpy.savetxt("test.connections.1", local_connection_list)
-        C = connectors.FromFileConnector("test.connections", distributed=True)
-        syn = sim.StaticSynapse()
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.5, 0.14),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.1, 0.1),
+                          (3, 0, 0.2, 0.11),
+                          (0, 1, 0.5, 0.14),
+                          (2, 2, 0.4, 0.13),
                           (2, 3, 0.3, 0.12)])
 
     def test_with_plastic_synapses_not_distributed(self, sim=sim):
         connection_list = [
             (0, 0, 0.1, 0.1,  100, 100),
             (3, 0, 0.2, 0.11, 110, 99),
             (2, 3, 0.3, 0.12, 120, 98),  # local
@@ -449,337 +556,342 @@
             (0, 1, 0.5, 0.14, 140, 96),  # local
         ]
         file = recording.files.StandardTextFile("test.connections.2", mode='wb')
         file.write(connection_list, {"columns": ["i", "j", "weight", "delay", "U", "tau_rec"]})
         C = connectors.FromFileConnector("test.connections.2", distributed=False)
         syn = sim.TsodyksMarkramSynapse(tau_facil=88.8)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay", "U", "tau_rec", "tau_facil"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.5, 0.14, 140.0, 96.0, 88.8),
+        self.assertEqual(prj.get(["weight", "delay", "U", "tau_rec", "tau_facil"], format='list'),
+                         [(0, 0, 0.1, 0.1,  100.0, 100.0, 88.8),
+                          (3, 0, 0.2, 0.11, 110.0, 99.0, 88.8),
+                          (0, 1, 0.5, 0.14, 140.0, 96.0, 88.8),
+                          (2, 2, 0.4, 0.13, 130.0, 97.0, 88.8),
                           (2, 3, 0.3, 0.12, 120.0, 98.0, 88.8)])
 
 
-class TestFixedNumberPostConnector(unittest.TestCase):
-
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
-        self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
-        self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
-
-    def test_with_n_smaller_than_population_size(self, sim=sim):
-        C = connectors.FixedNumberPostConnector(n=3, rng=MockRNG(delta=1))
-        syn = sim.StaticSynapse(weight="0.5*d")
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        # MockRNG.permutation(arr) returns the reverse of arr, so each pre neuron will connect to neurons 4, 3, 2
-        # however, only neuron 3 is on the "local" (fake MPI) node
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 3, 1.5, 0.123),
-                          (1, 3, 1.0, 0.123),
-                          (2, 3, 0.5, 0.123),
-                          (3, 3, 0.0, 0.123)])
-
-    def test_with_n_larger_than_population_size(self, sim=sim):
-        C = connectors.FixedNumberPostConnector(n=7, rng=MockRNG(delta=1))
-        syn = sim.StaticSynapse()
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        # each pre neuron will connect to all post neurons (population size 5 is less than n), then to 4, 3 (MockRNG.permutation)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
-                          (1, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123),
-                          (3, 3, 0.0, 0.123),
-                          (3, 3, 0.0, 0.123)])
-
-    def test_with_n_larger_than_population_size_no_self_connections(self, sim=sim):
-        C = connectors.FixedNumberPostConnector(
-            n=7, allow_self_connections=False, rng=MockRNG(delta=1))
-        syn = sim.StaticSynapse()
-        prj = sim.Projection(self.p2, self.p2, C, syn)
-        # connections as follows: (pre - list of post)
-        #   0 - 1 2 3 4 4 3 2
-        #   1 - 0 2 3 4 4 3 2
-        #   2 - 0 1 3 4 4 3 1
-        #   3 - 0 1 2 4 4 2 1
-        #   4 - 0 1 2 3 3 2 1
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (4, 1, 0.0, 0.123),
-                          (4, 1, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123),
-                          (4, 3, 0.0, 0.123),
-                          (4, 3, 0.0, 0.123), ])
-
-    def test_with_replacement(self, sim=sim):
-        C = connectors.FixedNumberPostConnector(n=3, with_replacement=True, rng=MockRNG(delta=1))
-        syn = sim.StaticSynapse()
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        # 0 - 0 1 2
-        # 1 - 3 4 0
-        # 2 - 1 2 3
-        # 3 - 4 0 1
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
-                          (3, 1, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (2, 3, 0.0, 0.123)])
-
-    def test_with_replacement_with_variable_n(self, sim=sim):
-        n = random.RandomDistribution('binomial', (5, 0.5), rng=MockRNG(start=1, delta=2))
-        # should give (1, 3, 0, 2)
-        C = connectors.FixedNumberPostConnector(n=n, with_replacement=True, rng=MockRNG(delta=1))
-        syn = sim.StaticSynapse()
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        # 0 - 0
-        # 1 - 1 2 3
-        # 2 -
-        # 3 - 4 0
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(1, 1, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123)])
-
-    def test_with_replacement_no_self_connections(self, sim=sim):
-        C = connectors.FixedNumberPostConnector(n=3, with_replacement=True,
-                                                allow_self_connections=False, rng=MockRNG(start=2, delta=1))
-        syn = sim.StaticSynapse()
-        prj = sim.Projection(self.p2, self.p2, C, syn)
-        # 0 - 2 3 4
-        # 1 - 0 2 3
-        # 2 - 4 0 1
-        # 3 - 2 4 0
-        # 4 - 1 2 3
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(2, 1, 0.0, 0.123),
-                          (4, 1, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123),
-                          (4, 3, 0.0, 0.123)])
-
-
 class TestFixedNumberPreConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
 
     def test_with_n_smaller_than_population_size(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse(weight="0.1*d")
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(3, 1, 0.2, 0.123),
-                          (2, 1, 0.1, 0.123),
-                          (1, 1, 0.0, 0.123),
-                          (3, 3, 0.0, 0.123),
-                          (2, 3, 0.1, 0.123),
-                          (1, 3, 0.2, 0.123), ])
+        rec = prj.get(["weight", "delay"], format='list')
+        assert_array_almost_equal([list(r) for r in rec],
+                                  [(3, 0, 0.3, 0.123),
+                                   (2, 0, 0.2, 0.123),
+                                   (1, 0, 0.1, 0.123),
+                                   (3, 1, 0.2, 0.123),
+                                   (2, 1, 0.1, 0.123),
+                                   (1, 1, 0.0, 0.123),
+                                   (3, 2, 0.1, 0.123),
+                                   (2, 2, 0.0, 0.123),
+                                   (1, 2, 0.1, 0.123),
+                                   (3, 3, 0.0, 0.123),
+                                   (2, 3, 0.1, 0.123),
+                                   (1, 3, 0.2, 0.123),
+                                   (3, 4, 0.1, 0.123),
+                                   (2, 4, 0.2, 0.123),
+                                   (1, 4, 0.3, 0.123)])
 
     def test_with_n_larger_than_population_size(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=7, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
                           (1, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123), ])
+                          (1, 3, 0.0, 0.123),
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123)])
 
     def test_with_n_larger_than_population_size_no_self_connections(self, sim=sim):
         C = connectors.FixedNumberPreConnector(
             n=7, allow_self_connections=False, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p2, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(1, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (4, 0, 0.0, 0.123),
+                          (4, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (4, 1, 0.0, 0.123),
                           (4, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (4, 2, 0.0, 0.123),
+                          (4, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
                           (0, 3, 0.0, 0.123),
                           (1, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
                           (4, 3, 0.0, 0.123),
                           (4, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123), ])
+                          (1, 3, 0.0, 0.123),
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123)])
 
     def test_with_replacement(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, with_replacement=True, rng=MockRNG(delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [  # (0, 0, 0.0, 0.123),
-            #(1, 0, 0.0, 0.123),
-            #(2, 0, 0.0, 0.123),
-            (3, 1, 0.0, 0.123),
-            (0, 1, 0.0, 0.123),
-            (1, 1, 0.0, 0.123),
-            #(2, 2, 0.0, 0.123),
-            #(3, 2, 0.0, 0.123),
-            #(0, 2, 0.0, 0.123),
-            (1, 3, 0.0, 0.123),
-            (2, 3, 0.0, 0.123),
-            (3, 3, 0.0, 0.123), ])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
+                          (1, 1, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
+                          (3, 3, 0.0, 0.123),
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123), ])
+
+    def test_with_replacement_with_neuron_0_connecting_neuron_0(self, sim=sim):
+        n = random.RandomDistribution('binomial', (5, 0.5), rng=MockRNG3())
+        C = connectors.FixedNumberPreConnector(
+            n=n, with_replacement=True, rng=MockRNG(start=0, delta=1))
+        syn = sim.StaticSynapse()
+        prj = sim.Projection(self.p1, self.p2, C, syn)
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          ])
 
     def test_with_replacement_with_variable_n(self, sim=sim):
         n = random.RandomDistribution('binomial', (5, 0.5), rng=MockRNG(start=1, delta=2))
         # should give (1, 3, 0, 2, 4)
-        C = connectors.FixedNumberPreConnector(n=n, with_replacement=True, rng=MockRNG(delta=1))
+        C = connectors.FixedNumberPreConnector(
+            n=n, with_replacement=True, rng=MockRNG(start=0, delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [  # (0, 0, 0.0, 0.123),
-            (1, 1, 0.0, 0.123),
-            (2, 1, 0.0, 0.123),
-            (3, 1, 0.0, 0.123),
-            (0, 3, 0.0, 0.123),
-            (1, 3, 0.0, 0.123)])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123)
+                          ])
+
+    # TOCHECK
 
     def test_with_replacement_no_self_connections(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, with_replacement=True,
                                                allow_self_connections=False, rng=MockRNG(start=2, delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p2, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [  # (2, 0, 0.0, 0.123),  # [2, 3, 4] --> [2, 3, 4]
-            #(3, 0, 0.0, 0.123),
-            #(4, 0, 0.0, 0.123),
-            (0, 1, 0.0, 0.123),   # [0, 1, 2] --> [0, 3, 2]
-            #(1, 1, 0.0, 0.123),
-            (3, 1, 0.0, 0.123),
-            (2, 1, 0.0, 0.123),
-            # (4, 2, 0.0, 0.123),  # [4, 0, 1] --> [4, 0, 1]
-            #(0, 2, 0.0, 0.123),
-            #(1, 2, 0.0, 0.123),
-            (2, 3, 0.0, 0.123),   # [2, 3, 4] --> [2, 0, 4]
-            #(3, 3, 0.0, 0.123),
-            (0, 3, 0.0, 0.123),
-            (4, 3, 0.0, 0.123),
-        ])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(2, 0, 0.0, 0.123),  # [2, 3, 4] --> [2, 3, 4]
+                          (3, 0, 0.0, 0.123),
+                          (4, 0, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),   # [0, 1, 2] --> [0, 3, 2]
+                          #(1, 1, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (2, 1, 0.0, 0.123),
+                          (4, 2, 0.0, 0.123),  # [4, 0, 1] --> [4, 0, 1]
+                          (0, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),   # [2, 3, 4] --> [2, 0, 4]
+                          #(3, 3, 0.0, 0.123),
+                          (0, 3, 0.0, 0.123),
+                          (4, 3, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          ])
+
+    # TOCHECK
 
     def test_no_replacement_no_self_connections(self, sim=sim):
         C = connectors.FixedNumberPreConnector(n=3, with_replacement=False,
                                                allow_self_connections=False, rng=MockRNG(start=2, delta=1))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p2, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(4, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(4, 0, 0.0, 0.123),
+                          (3, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (4, 1, 0.0, 0.123),
                           (3, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
+                          (4, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
                           (4, 3, 0.0, 0.123),
-                          #(3, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123), ])
+                          (1, 3, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123)])
+
+    # TOCHECK
 
     def test_with_replacement_parallel_unsafe(self, sim=sim):
         C = connectors.FixedNumberPreConnector(
             n=3, with_replacement=True, rng=MockRNG(delta=1, parallel_safe=False))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
+                          (0, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
-                          (2, 1, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (0, 2, 0.0, 0.123),
+                          (1, 3, 0.0, 0.123),
+                          (2, 3, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
-                          (0, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123), ])
+                          (0, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123), ])
 
     def test_no_replacement_parallel_unsafe(self, sim=sim):
         C = connectors.FixedNumberPreConnector(
             n=3, with_replacement=False, rng=MockRNG(delta=1, parallel_safe=False))
         syn = sim.StaticSynapse()
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(3, 1, 0.0, 0.123),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(3, 0, 0.0, 0.123),
+                          (2, 0, 0.0, 0.123),
+                          (1, 0, 0.0, 0.123),
+                          (3, 1, 0.0, 0.123),
                           (2, 1, 0.0, 0.123),
                           (1, 1, 0.0, 0.123),
+                          (3, 2, 0.0, 0.123),
+                          (2, 2, 0.0, 0.123),
+                          (1, 2, 0.0, 0.123),
                           (3, 3, 0.0, 0.123),
                           (2, 3, 0.0, 0.123),
-                          (1, 3, 0.0, 0.123), ])
+                          (1, 3, 0.0, 0.123),
+                          (3, 4, 0.0, 0.123),
+                          (2, 4, 0.0, 0.123),
+                          (1, 4, 0.0, 0.123), ])
 
 
 class TestArrayConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(3, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(4, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([1, 0, 1, 0], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
 
     def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         connections = numpy.array([
             [0, 1, 1, 0],
             [1, 1, 0, 1],
             [0, 0, 1, 0],
         ], dtype=bool)
         C = connectors.ArrayConnector(connections, safe=False)
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
                          [(1, 0, 5.0, 0.5),
+                          (0, 1, 5.0, 0.5),
+                          (1, 1, 5.0, 0.5),
                           (0, 2, 5.0, 0.5),
-                          (2, 2, 5.0, 0.5)])
+                          (2, 2, 5.0, 0.5),
+                          (1, 3, 5.0, 0.5)])
 
     def test_connect_with_random_weights_parallel_safe(self, sim=sim):
         rd_w = random.RandomDistribution(
             'uniform', (0, 1), rng=MockRNG(delta=1.0, parallel_safe=True))
         rd_d = random.RandomDistribution('uniform', (0, 1), rng=MockRNG(
             start=1.0, delta=0.1, parallel_safe=True))
         syn = sim.StaticSynapse(weight=rd_w, delay=rd_d)
         connections = numpy.array([
             [0, 1, 1, 0],
             [1, 1, 0, 1],
             [0, 0, 1, 0],
         ], dtype=bool)
         C = connectors.ArrayConnector(connections, safe=False)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(1, 0, 0.0, 1.0),
-                          (0, 2, 3.0, 1.3),
-                          (2, 2, 4.0, 1.4000000000000001)])  # better to do an "almost-equal" check
+        rec = prj.get(["weight", "delay"], format='list')
+        assert_array_almost_equal([tuple(r) for r in rec],
+                                  [(1, 0, 0.0, 1.0),
+                                   (0, 1, 1.0, 1.1),
+                                   (1, 1, 2.0, 1.2),
+                                   (0, 2, 3.0, 1.3),
+                                   (2, 2, 4.0, 1.4),
+                                   (1, 3, 5.0, 1.5)])
 
 
 class TestCloneConnector(unittest.TestCase):
 
-    def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+    def setUp(self, sim=sim, **extra):
+        sim.setup(min_delay=0.123, **extra)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
         connection_list = [
             (0, 0, 0.0, 1.0),
             (3, 0, 0.0, 1.0),
             (2, 3, 0.0, 1.0),  # local
             (2, 2, 0.0, 1.0),
             (0, 1, 0.0, 1.0),  # local
         ]
@@ -794,21 +906,25 @@
         def mock_gather_dict(D, all=False):
             return D
         recording.gather_dict = mock_gather_dict
 
     def tearDown(self, sim=sim):
         # restore original gather_dict function
         recording.gather_dict = self.orig_gather_dict
+        sim.end()
 
     def test_connect(self, sim=sim):
         syn = sim.StaticSynapse(weight=5.0, delay=0.5)
         C = connectors.CloneConnector(self.ref_prj)
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 1, 5.0, 0.5),
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 5.0, 0.5),
+                          (3, 0, 5.0, 0.5),
+                          (0, 1, 5.0, 0.5),
+                          (2, 2, 5.0, 0.5),
                           (2, 3, 5.0, 0.5)])
 
     def test_connect_with_pre_post_mismatch(self, sim=sim):
         syn = sim.StaticSynapse()
         C = connectors.CloneConnector(self.ref_prj)
         p3 = sim.Population(5, sim.IF_cond_exp(), structure=space.Line())
         self.assertRaises(errors.ConnectionError, sim.Projection, self.p1, p3, C, syn)
@@ -828,175 +944,125 @@
 
     class IndexBasedDelays(connectors.IndexBasedExpression):
 
         def __call__(self, i, j):
             return numpy.array(i + j + 1, dtype=float)
 
     def setUp(self, sim=sim, **extra):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
+        sim.setup(nmin_delay=0.123, **extra)
         self.p1 = sim.Population(5, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([1, 0, 1, 0, 1], dtype=bool))
+
+    def tearDown(self, sim=sim):
+        sim.end()
 
     def test_connect_with_scalar_weights_and_delays(self, sim=sim):
         syn = sim.StaticSynapse(weight=1.0, delay=2)
         C = connectors.IndexBasedProbabilityConnector(self.IndexBasedProbability())
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 0, 1, 2),
-                          (3, 0, 1, 2),
-                          (1, 2, 1, 2),
-                          (4, 2, 1, 2),
-                          (2, 4, 1, 2)])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 1., 2),
+                          (3, 0, 1., 2),
+                          (2, 1, 1., 2),
+                          (1, 2, 1., 2),
+                          (4, 2, 1., 2),
+                          (0, 3, 1., 2),
+                          (3, 3, 1., 2),
+                          (2, 4, 1., 2)])
 
     def test_connect_with_index_based_weights(self, sim=sim):
         syn = sim.StaticSynapse(weight=self.IndexBasedWeights(), delay=2)
         C = connectors.IndexBasedProbabilityConnector(self.IndexBasedProbability())
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 0, 1, 2),
-                          (3, 0, 1, 2),
-                          (1, 2, 3, 2),
-                          (4, 2, 9, 2),
-                          (2, 4, 9, 2)])
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 1., 2),
+                          (3, 0, 1., 2),
+                          (2, 1, 3., 2),
+                          (1, 2, 3., 2),
+                          (4, 2, 9., 2),
+                          (0, 3, 1., 2),
+                          (3, 3, 10., 2),
+                          (2, 4, 9., 2)])
 
     def test_connect_with_index_based_delays(self, sim=sim):
         syn = sim.StaticSynapse(weight=1.0, delay=self.IndexBasedDelays())
         C = connectors.IndexBasedProbabilityConnector(self.IndexBasedProbability())
         prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 0, 1, 1),
-                          (3, 0, 1, 4),
-                          (1, 2, 1, 4),
-                          (4, 2, 1, 7),
-                          (2, 4, 1, 7)])
-
-
-class TestDisplacementDependentProbabilityConnector(unittest.TestCase):
-
-    def setUp(self, sim=sim, **extra):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
-        self.p1 = sim.Population(9, sim.IF_cond_exp(),
-                                 structure=space.Grid2D(aspect_ratio=1.0, dx=1.0, dy=1.0))
-        self.p2 = sim.Population(9, sim.HH_cond_exp(),
-                                 structure=space.Grid2D(aspect_ratio=1.0, dx=1.0, dy=1.0))
-        assert_array_equal(self.p2._mask_local, numpy.array(
-            [1, 0, 1, 0, 1, 0, 1, 0, 1], dtype=bool))
-
-    def test_connect(self, sim=sim):
-        syn = sim.StaticSynapse(weight=1.0, delay=2)
-
-        def displacement_expression(d):
-            return 0.5 * ((d[0] >= -1) * (d[0] <= 2)) + 0.25 * (d[1] >= 0) * (d[1] <= 1)
-        C = connectors.DisplacementDependentProbabilityConnector(displacement_expression,
-                                                                 rng=MockRNG(delta=0.01))
-        prj = sim.Projection(self.p1, self.p2, C, syn)
-        self.assertEqual(prj.get(["weight", "delay"], format='list', gather=False),  # use gather False because we are faking the MPI
-                         [(0, 0, 1.0, 2.0),
-                          (1, 0, 1.0, 2.0),
-                          (2, 0, 1.0, 2.0),
-                          (3, 0, 1.0, 2.0),
-                          (4, 0, 1.0, 2.0),
-                          (5, 0, 1.0, 2.0),
-                          (6, 0, 1.0, 2.0),
-                          (0, 2, 1.0, 2.0),
-                          (1, 2, 1.0, 2.0),
-                          (2, 2, 1.0, 2.0),
-                          (3, 2, 1.0, 2.0),
-                          (4, 2, 1.0, 2.0),
-                          (5, 2, 1.0, 2.0),
-                          (0, 4, 1.0, 2.0),
-                          (1, 4, 1.0, 2.0),
-                          (2, 4, 1.0, 2.0),
-                          (3, 4, 1.0, 2.0),
-                          (4, 4, 1.0, 2.0),
-                          (5, 4, 1.0, 2.0),
-                          (6, 4, 1.0, 2.0),
-                          (7, 4, 1.0, 2.0),
-                          (8, 4, 1.0, 2.0),
-                          (0, 6, 1.0, 2.0),
-                          (3, 6, 1.0, 2.0),
-                          (6, 6, 1.0, 2.0),
-                          (1, 8, 1.0, 2.0),
-                          (2, 8, 1.0, 2.0)])
-
-
-@unittest.skip('skipping these tests until I figure out how I want to refactor checks')
-class CheckTest(unittest.TestCase):
-
-    def setUp(self, sim=sim, **extra):
-        self.MIN_DELAY = 0.123
-        sim.setup(num_processes=2, rank=1, min_delay=0.123, **extra)
-
-    def test_check_weights_with_scalar(self, sim=sim):
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'excitatory', is_conductance=True))
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'excitatory', is_conductance=False))
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'inhibitory', is_conductance=True))
-        self.assertEqual(-4.3, connectors.check_weights(-4.3, 'inhibitory', is_conductance=False))
-        self.assertEqual(connectors.DEFAULT_WEIGHT, connectors.check_weights(
-            None, 'excitatory', is_conductance=True))
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          4.3, 'inhibitory', is_conductance=False)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, -
-                          4.3, 'inhibitory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, -
-                          4.3, 'excitatory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights, -
-                          4.3, 'excitatory', is_conductance=False)
-
-    def test_check_weights_with_array(self, sim=sim):
-        w = numpy.arange(10)
-        assert_array_equal(w, connectors.check_weights(w, 'excitatory', is_conductance=True))
-        assert_array_equal(w, connectors.check_weights(w, 'excitatory', is_conductance=False))
-        assert_array_equal(w, connectors.check_weights(w, 'inhibitory', is_conductance=True))
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'inhibitory', is_conductance=False)
-        w = numpy.arange(-10, 0)
-        assert_array_equal(w, connectors.check_weights(w, 'inhibitory', is_conductance=False))
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'inhibitory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'excitatory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'excitatory', is_conductance=False)
-        w = numpy.arange(-5, 5)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'excitatory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'excitatory', is_conductance=False)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'inhibitory', is_conductance=True)
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          w, 'inhibitory', is_conductance=False)
-
-    def test_check_weights_with_invalid_value(self, sim=sim):
-        self.assertRaises(errors.ConnectionError, connectors.check_weights,
-                          "butterflies", 'excitatory', is_conductance=True)
-
-    def test_check_weight_is_conductance_is_None(self, sim=sim):
-        # need to check that a log message was created
-        self.assertEqual(4.3, connectors.check_weights(4.3, 'excitatory', is_conductance=None))
-
-    def test_check_delay(self, sim=sim):
-        self.assertEqual(connectors.check_delays(2 * self.MIN_DELAY,
-                                                 self.MIN_DELAY, 1e99), 2 * self.MIN_DELAY)
-        self.assertRaises(errors.ConnectionError, connectors.check_delays,
-                          0.5 * self.MIN_DELAY, self.MIN_DELAY, 1e99)
-        self.assertRaises(errors.ConnectionError, connectors.check_delays,
-                          3.0, self.MIN_DELAY, 2.0)
+        self.assertEqual(prj.get(["weight", "delay"], format='list'),
+                         [(0, 0, 1., 1),
+                          (3, 0, 1., 4),
+                          (2, 1, 1., 4),
+                          (1, 2, 1., 4),
+                          (4, 2, 1., 7),
+                          (0, 3, 1., 4),
+                          (3, 3, 1., 7),
+                          (2, 4, 1., 7)])
+
+
+#TOCHECK, not included
+# class TestDisplacementDependentProbabilityConnector(unittest.TestCase):
+
+    # def setUp(self, sim=sim, **extra):
+        #sim.setup(min_delay=0.123, **extra)
+        # self.p1 = sim.Population(9, sim.IF_cond_exp(),
+        # structure=space.Grid2D(aspect_ratio=1.0, dx=1.0, dy=1.0))
+        # self.p2 = sim.Population(9, sim.HH_cond_exp(),
+        # structure=space.Grid2D(aspect_ratio=1.0, dx=1.0, dy=1.0))
+
+    # def tearDown(self, sim=sim):
+        # sim.end()
+
+    # def test_connect(self, sim=sim):
+        #syn = sim.StaticSynapse(weight=1.0, delay=2)
+        # def displacement_expression(d):
+        # return 0.5 * ((d[0] >= -1) * (d[0] <= 2)) + 0.25 * (d[1] >= 0) * (d[1] <= 1)
+        # C = connectors.DisplacementDependentProbabilityConnector(displacement_expression,
+        # rng=MockRNG(delta=0.01))
+        #prj = sim.Projection(self.p1, self.p2, C, syn)
+        # self.assertEqual(prj.get(["weight", "delay"], format='list'),
+        # [(0, 0, 1.0, 2.0),
+        #(1, 0, 1.0, 2.0),
+        #(2, 0, 1.0, 2.0),
+        #(3, 0, 1.0, 2.0),
+        #(4, 0, 1.0, 2.0),
+        #(5, 0, 1.0, 2.0),
+        #(6, 0, 1.0, 2.0),
+        #(0, 2, 1.0, 2.0),
+        #(1, 2, 1.0, 2.0),
+        #(2, 2, 1.0, 2.0),
+        #(3, 2, 1.0, 2.0),
+        #(4, 2, 1.0, 2.0),
+        #(5, 2, 1.0, 2.0),
+        #(0, 4, 1.0, 2.0),
+        #(1, 4, 1.0, 2.0),
+        #(2, 4, 1.0, 2.0),
+        #(3, 4, 1.0, 2.0),
+        #(4, 4, 1.0, 2.0),
+        #(5, 4, 1.0, 2.0),
+        #(6, 4, 1.0, 2.0),
+        #(7, 4, 1.0, 2.0),
+        #(8, 4, 1.0, 2.0),
+        #(0, 6, 1.0, 2.0),
+        #(3, 6, 1.0, 2.0),
+        #(6, 6, 1.0, 2.0),
+        #(1, 8, 1.0, 2.0),
+        # (2, 8, 1.0, 2.0)])
 
 
 class TestFixedTotalNumberConnector(unittest.TestCase):
 
     def setUp(self, sim=sim):
-        sim.setup(num_processes=2, rank=1, min_delay=0.123)
+        sim.setup(num_processes=1, rank=0, min_delay=0.123)
         self.p1 = sim.Population(4, sim.IF_cond_exp(), structure=space.Line())
         self.p2 = sim.Population(5, sim.HH_cond_exp(), structure=space.Line())
-        assert_array_equal(self.p2._mask_local, numpy.array([0, 1, 0, 1, 0], dtype=bool))
+        assert_array_equal(self.p2._mask_local, numpy.array([1, 1, 1, 1, 1], dtype=bool))
 
     def test_1(self):
         C = connectors.FixedTotalNumberConnector(n=12, rng=random.NumpyRNG())
         syn = sim.StaticSynapse(weight="0.5*d")
         prj = sim.Projection(self.p1, self.p2, C, syn)
         connections = prj.get(["weight", "delay"], format='list', gather=False)
-        self.assertLess(len(connections), 12)    # unlikely to be 12, since we have 2 MPI nodes
-        self.assertGreater(len(connections), 0)  # unlikely to be 0
+        self.assertEqual(len(connections), 12)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `PyNN-0.9.5/test/unittests/test_core.py` & `PyNN-0.9.6/test/unittests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_descriptions.py` & `PyNN-0.9.6/test/unittests/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_files.py` & `PyNN-0.9.6/test/unittests/test_files.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_idmixin.py` & `PyNN-0.9.6/test/unittests/test_idmixin.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_lowlevelapi.py` & `PyNN-0.9.6/test/unittests/test_lowlevelapi.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_nest.py` & `PyNN-0.9.6/test/unittests/test_nest.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_neuron.py` & `PyNN-0.9.6/test/unittests/test_neuron.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,16 +317,16 @@
         self.c.delay = 23.4
         self.assertEqual(self.c.nc.delay, 23.4)
 
     def test_w_max_property(self):
         self.c._setup_plasticity(MockPlasticSynapseType(),
                                  {'wmax': 0.04,
                                   'dendritic_delay_fraction': 0})
-        self.assertEqual(self.c.w_max, 0.04)
-        self.c.w_max = 0.05
+        self.assertEqual(self.c.wmax, 0.04)
+        self.c.wmax = 0.05
         self.assertEqual(self.c.weight_adjuster.wmax, 0.05)
 
 
 @unittest.skipUnless(sim, "Requires NEURON")
 class TestProjection(unittest.TestCase):
 
     def setUp(self):
```

### Comparing `PyNN-0.9.5/test/unittests/test_parameters.py` & `PyNN-0.9.6/test/unittests/test_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Tests of the parameters module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
```

### Comparing `PyNN-0.9.5/test/unittests/test_population.py` & `PyNN-0.9.6/test/unittests/test_populationview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,622 +1,596 @@
 """
-Tests of the common implementation of the Population class, using the pyNN.mock
-backend.
+Tests of the common implementation of the PopulationView class, using the
+pyNN.mock backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
-try:
-    basestring
-except NameError:
-    basestring = str
 import numpy
 import sys
 from numpy.testing import assert_array_equal, assert_array_almost_equal
 import quantities as pq
 try:
     from unittest.mock import Mock, patch
 except ImportError:
     from mock import Mock, patch
+try:
+    basestring
+except NameError:
+    basestring = str
 from .mocks import MockRNG
 import pyNN.mock as sim
 from pyNN import random, errors, space
 from pyNN.parameters import Sequence
 
 
 def setUp():
     pass
 
 
 def tearDown():
     pass
 
 
-class PopulationTest(unittest.TestCase):
+class PopulationViewTest(unittest.TestCase):
 
     def setUp(self, sim=sim, **extra):
         sim.setup(**extra)
 
     def tearDown(self, sim=sim):
         sim.end()
 
-    def test_create_with_standard_cell_simple(self, sim=sim):
-        p = sim.Population(11, sim.IF_cond_exp())
-        self.assertEqual(p.size, 11)
-        self.assertIsInstance(p.label, basestring)
-        self.assertIsInstance(p.celltype, sim.IF_cond_exp)
-        self.assertIsInstance(p._structure, space.Line)
-        self.assertEqual(p._positions, None)
-        self.assertEqual(p.initial_values.keys(), p.celltype.default_initial_values.keys())
-
-    def test_create_with_parameters(self, sim=sim):
-        p = sim.Population(4, sim.IF_cond_exp(**{'tau_m': 12.3,
-                                                 'tau_syn_E': lambda i: 0.987 + 0.01 * i,
-                                                 'tau_syn_I': numpy.array([0.5, 0.6, 0.7, 0.8])}))
-        tau_syn_E, tau_m, tau_syn_I = p.get(('tau_syn_E', 'tau_m', 'tau_syn_I'), gather=True)
-        assert_array_almost_equal(tau_syn_E, numpy.array([0.987, 0.997, 1.007, 1.017]))
-        self.assertAlmostEqual(tau_m, 12.3)
-        assert_array_equal(tau_syn_I, numpy.array([0.5, 0.6, 0.7, 0.8]))
+    # test create with population parent and mask selector
 
-    # test create native cell
-
-    # test create native cell with params
+    def test_create_with_slice_selector(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
+        mask = slice(3, 9, 2)
+        pv = sim.PopulationView(parent=p, selector=mask)
+        self.assertEqual(pv.parent, p)
+        self.assertEqual(pv.size, 3)
+        self.assertEqual(pv.mask, mask)
+        assert_array_equal(pv.all_cells, numpy.array(
+            [p.all_cells[3], p.all_cells[5], p.all_cells[7]]))
+        #assert_array_equal(pv.local_cells, numpy.array([p.all_cells[3]]))
+        #assert_array_equal(pv._mask_local, numpy.array([1,0,0], dtype=bool))
+        self.assertEqual(pv.celltype, p.celltype)
+        self.assertEqual(pv.first_id, p.all_cells[3])
+        self.assertEqual(pv.last_id, p.all_cells[7])
 
-    # test create with structure
+    def test_create_with_boolean_array_selector(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_exp())
+        mask = numpy.array([0, 0, 0, 1, 0, 1, 0, 1, 0, 0, 0], dtype=bool)
+        pv = sim.PopulationView(parent=p, selector=mask)
+        assert_array_equal(pv.all_cells, numpy.array(
+            [p.all_cells[3], p.all_cells[5], p.all_cells[7]]))
+        #assert_array_equal(pv.mask, mask)
+
+    def test_create_with_index_array_selector(self, sim=sim):
+        p = sim.Population(11, sim.IF_cond_alpha())
+        mask = numpy.array([3, 5, 7])
+        pv = sim.PopulationView(parent=p, selector=mask)
+        assert_array_equal(pv.all_cells, numpy.array(
+            [p.all_cells[3], p.all_cells[5], p.all_cells[7]]))
+        assert_array_equal(pv.mask, mask)
+
+    # test create with populationview parent and mask selector
+
+    def test_create_with_slice_selector(self, sim=sim):
+        p = sim.Population(11, sim.HH_cond_exp())
+        mask1 = slice(0, 9, 1)
+        pv1 = sim.PopulationView(parent=p, selector=mask1)
+        assert_array_equal(pv1.all_cells, p.all_cells[0:9])
+        mask2 = slice(3, 9, 2)
+        pv2 = sim.PopulationView(parent=pv1, selector=mask2)
+        # or would it be better to resolve the parent chain up to an actual Population?
+        self.assertEqual(pv2.parent, pv1)
+        assert_array_equal(pv2.all_cells, numpy.array(
+            [p.all_cells[3], p.all_cells[5], p.all_cells[7]]))
+        #assert_array_equal(pv2._mask_local, numpy.array([1,0,0], dtype=bool))
+
+    # test initial values property
+
+    def test_structure_property(self, sim=sim):
+        p = sim.Population(11, sim.SpikeSourcePoisson())
+        mask = slice(3, 9, 2)
+        pv = sim.PopulationView(parent=p, selector=mask)
+        self.assertEqual(pv.structure, p.structure)
 
-    def test_create_with_implicit_grid(self, sim=sim):
-        p = sim.Population((11,), sim.IF_cond_exp())
-        self.assertEqual(p.size, 11)
-        self.assertIsInstance(p.structure, space.Line)
-        p = sim.Population((5, 6), sim.IF_cond_exp())
-        self.assertEqual(p.size, 30)
-        self.assertIsInstance(p.structure, space.Grid2D)
-        p = sim.Population((2, 3, 4), sim.IF_cond_exp())
-        self.assertEqual(p.size, 24)
-        self.assertIsInstance(p.structure, space.Grid3D)
-        self.assertRaises(Exception, sim.Population, (2, 3, 4, 5), sim.IF_cond_exp())
-
-    def test_create_with_empty_spike_source_array(self, sim=sim):
-        # regression test for https://github.com/NeuralEnsemble/PyNN/issues/378
-        p = sim.Population(11, sim.SpikeSourceArray(spike_times=[]))
+    # test positions property
 
-    # def test_create_with_initial_values():
+    def test_get_positions(self, sim=sim):
+        p = sim.Population(11, sim.IF_curr_exp())
+        ppos = numpy.random.uniform(size=(3, 11))
+        p._positions = ppos
+        pv = sim.PopulationView(parent=p, selector=slice(3, 9, 2))
+        assert_array_equal(pv.positions, numpy.array([ppos[:, 3], ppos[:, 5], ppos[:, 7]]).T)
 
     def test_id_to_index(self, sim=sim):
         p = sim.Population(11, sim.IF_curr_alpha())
-        self.assertEqual(p.id_to_index(p[0]), 0)
-        self.assertEqual(p.id_to_index(p[10]), 10)
+        pv = p[2, 5, 7, 8]
+        self.assertEqual(pv.id_to_index(pv[0]), 0)
+        self.assertEqual(pv.id_to_index(pv[3]), 3)
+        self.assertEqual(pv.id_to_index(p[2]), 0)
+        self.assertEqual(pv.id_to_index(p[8]), 3)
 
     def test_id_to_index_with_array(self, sim=sim):
-        p = sim.Population(11, sim.IF_curr_alpha())
-        assert_array_equal(p.id_to_index(p.all_cells[3:9:2]), numpy.arange(3, 9, 2))
-
-    def test_id_to_index_with_populationview(self, sim=sim):
-        p = sim.Population(11, sim.IF_curr_alpha())
-        view = p[3:7]
-        self.assertIsInstance(view, sim.PopulationView)
-        assert_array_equal(p.id_to_index(view), numpy.arange(3, 7))
+        p = sim.Population(121, sim.IF_curr_alpha())
+        pv = p[2, 5, 7, 8, 19, 37, 49, 82, 83, 99]
+        assert_array_equal(pv.id_to_index(pv.all_cells[3:9:2]), numpy.arange(3, 9, 2))
 
     def test_id_to_index_with_invalid_id(self, sim=sim):
         p = sim.Population(11, sim.IF_curr_alpha())
-        self.assertRaises(ValueError, p.id_to_index, p.last_id + 1)
-        self.assertRaises(ValueError, p.id_to_index, p.first_id - 1)
-
-    def test_id_to_index_with_invalid_ids(self, sim=sim):
-        p = sim.Population(11, sim.IF_curr_alpha())
-        self.assertRaises(ValueError, p.id_to_index, [p.first_id - 1] + p.all_cells[0:3].tolist())
+        pv = p[2, 5, 7, 8]
+        self.assertRaises(IndexError, pv.id_to_index, p[0])
+        self.assertRaises(IndexError, pv.id_to_index, p[9])
+
+#    def test_id_to_index_with_invalid_ids(self, sim=sim):
+#        p = sim.Population(11, sim.IF_curr_alpha())
+#        pv = p[2, 5, 7, 8]
+#        self.assertRaises(IndexError, pv.id_to_index, p.all_cells[[2, 5, 6]])
+# currently failing
 
     # def test_id_to_local_index():
 
     # test structure property
 
     def test_set_structure(self, sim=sim):
-        p = sim.Population(11, sim.IF_cond_exp())
-        p.positions = numpy.arange(33).reshape(3, 11)
-        new_struct = space.Grid2D()
-        p.structure = new_struct
-        self.assertEqual(p.structure, new_struct)
-        self.assertEqual(p._positions, None)
+        p = sim.Population(11, sim.IF_cond_exp(), structure=space.Grid2D())
+        pv = p[2, 5, 7, 8]
+        new_struct = space.Line()
+
+        def set_struct(struct):
+            pv.structure = struct
+        self.assertRaises(AttributeError, set_struct, new_struct)
 
     # test positions property
 
     def test_get_positions(self, sim=sim):
         p = sim.Population(11, sim.IF_cond_exp())
-        pos1 = numpy.arange(33).reshape(3, 11)
-        p._structure = Mock()
-        p._structure.generate_positions = Mock(return_value=pos1)
-        self.assertEqual(p._positions, None)
-        assert_array_equal(p.positions, pos1)
-
-        pos2 = 1 + numpy.arange(33).reshape(3, 11)
-        p.positions = pos2
-        assert_array_equal(p.positions, pos2)
-
-    def test_set_positions(self, sim=sim):
-        p = sim.Population(11, sim.IF_cond_exp())
-        assert p._structure is not None
-        new_positions = numpy.random.uniform(size=(3, 11))
-        p.positions = new_positions
-        self.assertEqual(p.structure, None)
-        assert_array_equal(p.positions, new_positions)
-        new_positions[0, 0] = 99.9
-        self.assertNotEqual(p.positions[0, 0], 99.9)
+        pos = numpy.arange(33).reshape(3, 11)
+        p.positions = pos
+        pv = p[2, 5, 7, 8]
+        assert_array_equal(pv.positions, pos[:, [2, 5, 7, 8]])
 
     def test_position_generator(self, sim=sim):
         p = sim.Population(11, sim.IF_cond_exp())
-        assert_array_equal(p.position_generator(0), p.positions[:, 0])
-        assert_array_equal(p.position_generator(10), p.positions[:, 10])
-        assert_array_equal(p.position_generator(-1), p.positions[:, 10])
-        assert_array_equal(p.position_generator(-11), p.positions[:, 0])
-        self.assertRaises(IndexError, p.position_generator, 11)
-        self.assertRaises(IndexError, p.position_generator, -12)
+        pv = p[2, 5, 7, 8]
+        assert_array_equal(pv.position_generator(0), p.positions[:, 2])
+        assert_array_equal(pv.position_generator(3), p.positions[:, 8])
+        assert_array_equal(pv.position_generator(-1), p.positions[:, 8])
+        assert_array_equal(pv.position_generator(-4), p.positions[:, 2])
+        self.assertRaises(IndexError, pv.position_generator, 4)
+        self.assertRaises(IndexError, pv.position_generator, -5)
 
     def test__getitem__int(self, sim=sim):
         # Should return the correct ID object
         p = sim.Population(12, sim.IF_cond_exp())
-        self.assertEqual(p[11], p[0] + 11)
-        self.assertRaises(IndexError, p.__getitem__, 12)
-        self.assertEqual(p[-1], p[11])
+        pv = p[1, 5, 6, 8, 11]
+
+        self.assertEqual(pv[0], p[1], 42)
+        self.assertEqual(pv[4], p[11], 53)
+        self.assertRaises(IndexError, pv.__getitem__, 6)
+        self.assertEqual(pv[-1], p[11], 53)
 
     def test__getitem__slice(self, sim=sim):
         # Should return a PopulationView with the correct parent and value
         # of all_cells
         p = sim.Population(17, sim.HH_cond_exp())
-        pv = p[3:9]
-        self.assertEqual(pv.parent, p)
-        assert_array_almost_equal(pv.all_cells, p.all_cells[3:9])
+        pv1 = p[1, 5, 6, 8, 11, 12, 15, 16]
+
+        pv2 = pv1[2:6]
+        self.assertEqual(pv2.parent, pv1)
+        self.assertEqual(pv2.grandparent, p)
+        assert_array_equal(pv2.all_cells, pv1.all_cells[[2, 3, 4, 5]])
+        assert_array_equal(pv2.all_cells, p.all_cells[[6, 8, 11, 12]])
 
     def test__getitem__list(self, sim=sim):
         p = sim.Population(23, sim.HH_cond_exp())
-        pv = p[list(range(3, 9))]
-        self.assertEqual(pv.parent, p)
-        assert_array_almost_equal(pv.all_cells, p.all_cells[3:9])
+        pv1 = p[1, 5, 6, 8, 11, 12, 15, 16, 19, 20]
+
+        pv2 = pv1[list(range(3, 8))]
+        self.assertEqual(pv2.parent, pv1)
+        assert_array_almost_equal(pv2.all_cells, p.all_cells[[8, 11, 12, 15, 16]])
 
     def test__getitem__tuple(self, sim=sim):
         p = sim.Population(23, sim.HH_cond_exp())
-        pv = p[(3, 5, 7)]
-        self.assertEqual(pv.parent, p)
-        assert_array_almost_equal(pv.all_cells, p.all_cells[[3, 5, 7]])
+        pv1 = p[1, 5, 6, 8, 11, 12, 15, 16, 19, 20]
+
+        pv2 = pv1[(3, 5, 7)]
+        self.assertEqual(pv2.parent, pv1)
+        assert_array_almost_equal(pv2.all_cells, p.all_cells[[8, 12, 16]])
 
     def test__getitem__invalid(self, sim=sim):
         p = sim.Population(23, sim.IF_curr_alpha())
-        self.assertRaises(TypeError, p.__getitem__, "foo")
+        pv = p[1, 5, 6, 8, 11, 12, 15, 16, 19, 20]
+        self.assertRaises(TypeError, pv.__getitem__, "foo")
 
     def test__len__(self, sim=sim):
         # len(p) should give the global size (all MPI nodes)
         p = sim.Population(77, sim.IF_cond_exp())
-        self.assertEqual(len(p), p.size, 77)
+        pv = p[1, 5, 6, 8, 11, 12, 15, 16, 19, 20]
+        self.assertEqual(len(pv), pv.size, 10)
 
     def test_iter(self, sim=sim):
-        p = sim.Population(6, sim.IF_curr_exp())
-        itr = p.__iter__()
+        p = sim.Population(33, sim.IF_curr_exp())
+        pv = p[1, 5, 6, 8, 11, 12]
+        itr = pv.__iter__()
         assert hasattr(itr, "next") or hasattr(itr, "__next__")
         self.assertEqual(len(list(itr)), 6)
 
     def test___add__two(self, sim=sim):
-        # adding two populations should give an Assembly
-        p1 = sim.Population(6, sim.IF_curr_exp())
-        p2 = sim.Population(17, sim.IF_cond_exp())
-        assembly = p1 + p2
+        # adding two population views should give an Assembly
+        pv1 = sim.Population(6, sim.IF_curr_exp())[2, 3, 5]
+        pv2 = sim.Population(17, sim.IF_cond_exp())[4, 2, 16]
+        assembly = pv1 + pv2
         self.assertIsInstance(assembly, sim.Assembly)
-        self.assertEqual(assembly.populations, [p1, p2])
+        self.assertEqual(assembly.populations, [pv1, pv2])
 
     def test___add__three(self, sim=sim):
-        # adding three populations should give an Assembly
-        p1 = sim.Population(6, sim.IF_curr_exp())
-        p2 = sim.Population(17, sim.IF_cond_exp())
-        p3 = sim.Population(9, sim.HH_cond_exp())
-        assembly = p1 + p2 + p3
+        # adding three population views should give an Assembly
+        pv1 = sim.Population(6, sim.IF_curr_exp())[0:3]
+        pv2 = sim.Population(17, sim.IF_cond_exp())[1, 5, 14]
+        pv3 = sim.Population(9, sim.HH_cond_exp())[3:8]
+        assembly = pv1 + pv2 + pv3
         self.assertIsInstance(assembly, sim.Assembly)
-        self.assertEqual(assembly.populations, [p1, p2, p3])
+        self.assertEqual(assembly.populations, [pv1, pv2, pv3])
 
     def test_nearest(self, sim=sim):
         p = sim.Population(13, sim.IF_cond_exp())
         p.positions = numpy.arange(39).reshape((13, 3)).T
-        self.assertEqual(p.nearest((0.0, 1.0, 2.0)), p[0])
-        self.assertEqual(p.nearest((3.0, 4.0, 5.0)), p[1])
-        self.assertEqual(p.nearest((36.0, 37.0, 38.0)), p[12])
-        self.assertEqual(p.nearest((1.49, 2.49, 3.49)), p[0])
-        self.assertEqual(p.nearest((1.51, 2.51, 3.51)), p[1])
-
-        x, y, z = 4, 5, 6
-        p = sim.Population((x, y, z), sim.IF_cond_alpha())
-        self.assertEqual(p.nearest((0.0, 0.0, 0.0)), p[0])
-        self.assertEqual(p.nearest((0.0, 0.0, 1.0)), p[1])
-        self.assertEqual(p.nearest((0.0, 1.0, 0.0)), p[z])
-        self.assertEqual(p.nearest((1.0, 0.0, 0.0)), p[y * z])
-        self.assertEqual(p.nearest((3.0, 2.0, 1.0)), p[3 * y * z + 2 * z + 1])
-        self.assertEqual(p.nearest((3.49, 2.49, 1.49)), p[3 * y * z + 2 * z + 1])
-        self.assertEqual(p.nearest((3.49, 2.49, 1.51)), p[3 * y * z + 2 * z + 2])
-        # self.assertEqual(p.nearest((3.49,2.49,1.5)), p[3*y*z+2*z+2]) # known to fail
-        #self.assertEqual(p.nearest((2.5,2.5,1.5)), p[3*y*z+3*y+2])
+        pv = p[0, 2, 5, 11]
+        self.assertEqual(pv.nearest((0.0, 1.0, 2.0)), pv[0])
+        self.assertEqual(pv.nearest((3.0, 4.0, 5.0)), pv[0])
+        self.assertEqual(pv.nearest((36.0, 37.0, 38.0)), pv[3])
+        self.assertEqual(pv.nearest((1.49, 2.49, 3.49)), pv[0])
+        self.assertEqual(pv.nearest((1.51, 2.51, 3.51)), pv[0])
 
     def test_sample(self, sim=sim):
         p = sim.Population(13, sim.IF_cond_exp())
+        pv1 = p[0, 3, 7, 10, 12]
+
         rng = Mock()
-        rng.permutation = Mock(return_value=numpy.array(
-            [7, 4, 8, 12, 0, 3, 9, 1, 2, 11, 5, 10, 6]))
-        pv = p.sample(5, rng=rng)
-        assert_array_equal(pv.all_cells,
-                           p.all_cells[[7, 4, 8, 12, 0]])
+        rng.permutation = Mock(return_value=numpy.array([3, 1, 0, 2, 4]))
+        pv2 = pv1.sample(3, rng=rng)
+        assert_array_equal(pv2.all_cells,
+                           p.all_cells[[10, 3, 0]])
 
     def test_get_multiple_homogeneous_params_with_gather(self, sim=sim):
-        p = sim.Population(4, sim.IF_cond_exp(
-            **{'tau_m': 12.3, 'tau_syn_E': 0.987, 'tau_syn_I': 0.7}))
-        tau_syn_E, tau_m = p.get(('tau_syn_E', 'tau_m'), gather=True)
-        self.assertIsInstance(tau_syn_E, float)
+        p = sim.Population(10, sim.IF_cond_exp, {
+                           'tau_m': 12.3, 'tau_syn_E': 0.987, 'tau_syn_I': 0.7})
+        pv = p[3:7]
+        tau_syn_E, tau_m = pv.get(('tau_syn_E', 'tau_m'), gather=True)
         self.assertEqual(tau_syn_E, 0.987)
         self.assertAlmostEqual(tau_m, 12.3)
 
-    def test_get_single_param_with_gather(self, sim=sim):
-        p = sim.Population(4, sim.IF_cond_exp(tau_m=12.3, tau_syn_E=0.987, tau_syn_I=0.7))
-        tau_syn_E = p.get('tau_syn_E', gather=True)
+    def test_get_single_homogeneous_param_with_gather(self, sim=sim):
+        p = sim.Population(4, sim.IF_cond_exp, {
+                           'tau_m': 12.3, 'tau_syn_E': 0.987, 'tau_syn_I': 0.7})
+        pv = p[:]
+        tau_syn_E = pv.get('tau_syn_E', gather=True)
         self.assertEqual(tau_syn_E, 0.987)
 
     def test_get_multiple_inhomogeneous_params_with_gather(self, sim=sim):
         p = sim.Population(4, sim.IF_cond_exp(tau_m=12.3,
                                               tau_syn_E=[0.987, 0.988, 0.989, 0.990],
                                               tau_syn_I=lambda i: 0.5 + 0.1 * i))
-        tau_syn_E, tau_m, tau_syn_I = p.get(('tau_syn_E', 'tau_m', 'tau_syn_I'), gather=True)
+        pv = p[0, 1, 3]
+        tau_syn_E, tau_m, tau_syn_I = pv.get(('tau_syn_E', 'tau_m', 'tau_syn_I'), gather=True)
         self.assertIsInstance(tau_m, float)
         self.assertIsInstance(tau_syn_E, numpy.ndarray)
-        assert_array_equal(tau_syn_E, numpy.array([0.987, 0.988, 0.989, 0.990]))
+        assert_array_equal(tau_syn_E, numpy.array([0.987, 0.988, 0.990]))
         self.assertAlmostEqual(tau_m, 12.3)
-        assert_array_almost_equal(tau_syn_I, numpy.array([0.5, 0.6, 0.7, 0.8]), decimal=12)
+        assert_array_almost_equal(tau_syn_I, numpy.array([0.5, 0.6, 0.8]), decimal=12)
 
-    def test_get_multiple_params_no_gather(self, sim=sim):
-        sim.simulator.state.num_processes = 2
-        sim.simulator.state.mpi_rank = 1
-        p = sim.Population(4, sim.IF_cond_exp(tau_m=12.3,
-                                              tau_syn_E=[0.987, 0.988, 0.989, 0.990],
-                                              i_offset=lambda i: -0.2 * i))
-        tau_syn_E, tau_m, i_offset = p.get(('tau_syn_E', 'tau_m', 'i_offset'), gather=False)
-        self.assertIsInstance(tau_m, float)
-        self.assertIsInstance(tau_syn_E, numpy.ndarray)
-        assert_array_equal(tau_syn_E, numpy.array([0.988, 0.990]))
-        self.assertEqual(tau_m, 12.3)
-        assert_array_almost_equal(i_offset, numpy.array([-0.2, -0.6]), decimal=12)
-        sim.simulator.state.num_processes = 1
-        sim.simulator.state.mpi_rank = 0
+    # def test_get_multiple_params_no_gather(self, sim=sim):
 
     def test_get_sequence_param(self, sim=sim):
-        p = sim.Population(3, sim.SpikeSourceArray(spike_times=[Sequence([1, 2, 3, 4]),
-                                                                Sequence([2, 3, 4, 5]),
-                                                                Sequence([3, 4, 5, 6])]))
-        spike_times = p.get('spike_times')
-        self.assertEqual(spike_times.size, 3)
-        assert_array_equal(spike_times[1], Sequence([2, 3, 4, 5]))
+        p = sim.Population(3, sim.SpikeSourceArray,
+                           {'spike_times': [Sequence([1, 2, 3, 4]),
+                                            Sequence([2, 3, 4, 5]),
+                                            Sequence([3, 4, 5, 6])]})
+        pv = p[1:]
+        spike_times = pv.get('spike_times')
+        self.assertEqual(spike_times.size, 2)
+        assert_array_equal(spike_times[1], Sequence([3, 4, 5, 6]))
 
     def test_set(self, sim=sim):
         p = sim.Population(4, sim.IF_cond_exp, {
                            'tau_m': 12.3, 'tau_syn_E': 0.987, 'tau_syn_I': 0.7})
+        pv = p[:3]
         rng = MockRNG(start=1.21, delta=0.01, parallel_safe=True)
-        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.5, 1.5), rng=rng), tau_m=9.87)
+        pv.set(tau_syn_E=random.RandomDistribution('uniform', (0.8, 1.2), rng=rng), tau_m=9.87)
         tau_m, tau_syn_E, tau_syn_I = p.get(('tau_m', 'tau_syn_E', 'tau_syn_I'), gather=True)
-        assert_array_equal(tau_syn_E, numpy.array([1.21, 1.22, 1.23, 1.24]))
-        assert_array_almost_equal(tau_m, 9.87 * numpy.ones((4,)))
+        assert_array_equal(tau_syn_E, numpy.array([1.21, 1.22, 1.23, 0.987]))
+        assert_array_almost_equal(tau_m, numpy.array([9.87, 9.87, 9.87, 12.3]))
         assert_array_equal(tau_syn_I, 0.7 * numpy.ones((4,)))
 
+        tau_m, tau_syn_E, tau_syn_I = pv.get(('tau_m', 'tau_syn_E', 'tau_syn_I'), gather=True)
+        assert_array_equal(tau_syn_E, numpy.array([1.21, 1.22, 1.23]))
+        assert_array_almost_equal(tau_m, numpy.array([9.87, 9.87, 9.87]))
+        assert_array_equal(tau_syn_I, 0.7 * numpy.ones((3,)))
+
     def test_set_invalid_name(self, sim=sim):
         p = sim.Population(9, sim.HH_cond_exp())
-        self.assertRaises(errors.NonExistentParameterError, p.set, foo=13.2)
+        pv = p[3:5]
+        self.assertRaises(errors.NonExistentParameterError, pv.set, foo=13.2)
 
     def test_set_invalid_type(self, sim=sim):
         p = sim.Population(9, sim.IF_cond_exp())
-        self.assertRaises(errors.InvalidParameterValueError, p.set, tau_m={})
-        self.assertRaises(errors.InvalidParameterValueError, p.set, v_reset='bar')
+        pv = p[::3]
+        self.assertRaises(errors.InvalidParameterValueError, pv.set, tau_m={})
+        self.assertRaises(errors.InvalidParameterValueError, pv.set, v_reset='bar')
 
     def test_set_sequence(self, sim=sim):
-        p = sim.Population(3, sim.SpikeSourceArray())
-        p.set(spike_times=[Sequence([1, 2, 3, 4]),
-                           Sequence([2, 3, 4, 5]),
-                           Sequence([3, 4, 5, 6])])
+        p = sim.Population(5, sim.SpikeSourceArray())
+        pv = p[0, 2, 4]
+        pv.set(spike_times=[Sequence([1, 2, 3, 4]),
+                            Sequence([2, 3, 4, 5]),
+                            Sequence([3, 4, 5, 6])])
         spike_times = p.get('spike_times', gather=True)
-        self.assertEqual(spike_times.size, 3)
-        assert_array_equal(spike_times[1], Sequence([2, 3, 4, 5]))
+        self.assertEqual(spike_times.size, 5)
+        assert_array_equal(spike_times[1], Sequence([]))
+        assert_array_equal(spike_times[2], Sequence([2, 3, 4, 5]))
 
     def test_set_array(self, sim=sim):
-        p = sim.Population(5, sim.IF_cond_exp())
-        p.set(v_thresh=-50.0 + numpy.arange(5))
+        p = sim.Population(5, sim.IF_cond_exp, {'v_thresh': -54.3})
+        pv = p[2:]
+        pv.set(v_thresh=-50.0 + numpy.arange(3))
         assert_array_equal(p.get('v_thresh', gather=True),
-                           numpy.array([-50.0, -49.0, -48.0, -47.0, -46.0]))
-
-    def test_set_random_distribution_parallel_unsafe(self, sim=sim):
-        orig_rcfg = random.get_mpi_config
-        random.get_mpi_config = lambda: (1, 2)
-        sim.simulator.state.num_processes = 2
-        sim.simulator.state.mpi_rank = 1
-        p = sim.Population(4, sim.IF_cond_exp(tau_syn_E=0.987))
-        rng = MockRNG(start=1.21, delta=0.01, parallel_safe=False)
-        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.8, 1.2), rng=rng))
-        tau_syn_E = p.get('tau_syn_E', gather=False)
-        assert_array_equal(tau_syn_E, numpy.array([1.21, 1.22]))
-        random.get_mpi_config = orig_rcfg
-        sim.simulator.state.num_processes = 1
-        sim.simulator.state.mpi_rank = 0
-
-    def test_set_random_distribution_parallel_safe(self, sim=sim):
-        orig_rcfg = random.get_mpi_config
-        random.get_mpi_config = lambda: (1, 2)
-        sim.simulator.state.num_processes = 2
-        sim.simulator.state.mpi_rank = 1
-        p = sim.Population(4, sim.IF_cond_exp(tau_syn_E=0.987))
-        rng = MockRNG(start=1.21, delta=0.01, parallel_safe=True)
-        p.set(tau_syn_E=random.RandomDistribution('uniform', (0.1, 1), rng=rng))
-        tau_syn_E = p.get('tau_syn_E', gather=False)
-        assert_array_equal(tau_syn_E, numpy.array([1.22, 1.24]))
-        random.get_mpi_config = orig_rcfg
-        sim.simulator.state.num_processes = 1
-        sim.simulator.state.mpi_rank = 0
+                           numpy.array([-54.3, -54.3, -50.0, -49.0, -48.0]))
 
     def test_tset(self, sim=sim):
         p = sim.Population(17, sim.IF_cond_alpha())
-        p.set = Mock()
-        tau_m = numpy.linspace(10.0, 20.0, num=p.size)
-        p.tset("tau_m", tau_m)
-        p.set.assert_called_with(tau_m=tau_m)
+        pv = p[::4]
+        pv.set = Mock()
+        tau_m = numpy.linspace(10.0, 20.0, num=pv.size)
+        pv.tset("tau_m", tau_m)
+        pv.set.assert_called_with(tau_m=tau_m)
 
     def test_rset(self, sim=sim):
         p = sim.Population(17, sim.IF_cond_alpha())
-        p.set = Mock()
+        pv = p[::4]
+        pv.set = Mock()
         v_rest = random.RandomDistribution('uniform', low=-70.0, high=-60.0)
-        p.rset("v_rest", v_rest)
-        p.set.assert_called_with(v_rest=v_rest)
+        pv.rset("v_rest", v_rest)
+        pv.set.assert_called_with(v_rest=v_rest)
 
     # def test_set_with_native_rng():
 
-    def test_initialize(self, sim=sim):
-        p = sim.Population(17, sim.EIF_cond_exp_isfa_ista())
-        v_init = numpy.linspace(-70.0, -60.0, num=p.size)
-        w_init = 0.1
-        p.initialize(v=v_init, w=w_init)
-        assert_array_equal(p.initial_values['v'].evaluate(simplify=True), v_init)
-        assert_array_equal(p.initial_values['w'].evaluate(simplify=True), w_init)
-        # should call p.record(('v', 'w')) and check that the recorded data starts with the initial value
+    # def test_initialize(self, sim=sim):
+    #    p = sim.Population(7, sim.EIF_cond_exp_isfa_ista,
+    #                       initial_values={'v': -65.4, 'w': 0.0})
+    #    pv = p[::2]
+    #
+    #    v_init = numpy.linspace(-70.0, -67.0, num=pv.size)
+    #    w_init = 0.1
+    #    pv.initialize(v=v_init, w=w_init)
+    #    assert_array_equal(p.initial_values['v'].evaluate(simplify=True),
+    #                       numpy.array([-70.0, -65.4, -69.0, -65.4, -68.0, -65.4, -67.0]))
+    #    assert_array_equal(p.initial_values['w'].evaluate(simplify=True),
+    #                       numpy.array([0.1, 0.0, 0.1, 0.0, 0.1, 0.0, 0.1]))
+    #    # should call p.record(('v', 'w')) and check that the recorded data starts with the initial value
 
     def test_can_record(self, sim=sim):
-        p = sim.Population(17, sim.EIF_cond_exp_isfa_ista())
-        assert p.can_record('v')
-        assert p.can_record('w')
-        assert p.can_record('gsyn_inh')
-        assert p.can_record('spikes')
-        assert not p.can_record('foo')
+        pv = sim.Population(17, sim.EIF_cond_exp_isfa_ista())[::2]
+        assert pv.can_record('v')
+        assert pv.can_record('w')
+        assert pv.can_record('gsyn_inh')
+        assert pv.can_record('spikes')
+        assert not pv.can_record('foo')
 
     def test_record_with_single_variable(self, sim=sim):
         p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
-        p.record('v')
+        pv = p[0, 4, 6, 13]
+        pv.record('v')
         sim.run(12.3)
         data = p.get_data(gather=True).segments[0]
         self.assertEqual(len(data.analogsignals), 1)
         n_values = int(round(12.3 / sim.get_time_step())) + 1
         self.assertEqual(data.analogsignals[0].name, 'v')
-        self.assertEqual(data.analogsignals[0].shape, (n_values, p.size))
+        self.assertEqual(data.analogsignals[0].shape, (n_values, pv.size))
 
     def test_record_with_multiple_variables(self, sim=sim):
-        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
-        p.record(('v', 'w', 'gsyn_exc'))
+        p = sim.Population(4, sim.EIF_cond_exp_isfa_ista())
+        pv = p[0, 3]
+        pv.record(('v', 'w', 'gsyn_exc'))
         sim.run(10.0)
         data = p.get_data(gather=True).segments[0]
         self.assertEqual(len(data.analogsignals), 3)
         n_values = int(round(10.0 / sim.get_time_step())) + 1
         names = set(arr.name for arr in data.analogsignals)
         self.assertEqual(names, set(('v', 'w', 'gsyn_exc')))
         for arr in data.analogsignals:
-            self.assertEqual(arr.shape, (n_values, p.size))
+            self.assertEqual(arr.shape, (n_values, pv.size))
 
-    def test_record_with_v_and_spikes(self, sim=sim):
-        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
-        p.record(('v', 'spikes'))
+    def test_record_with_v_spikes(self, sim=sim):
+        p = sim.Population(4, sim.EIF_cond_exp_isfa_ista())
+        pv = p[0, 3]
+        pv.record(('v', 'spikes'))
         sim.run(10.0)
         data = p.get_data(gather=True).segments[0]
         self.assertEqual(len(data.analogsignals), 1)
         n_values = int(round(10.0 / sim.get_time_step())) + 1
         names = set(arr.name for arr in data.analogsignals)
         self.assertEqual(names, set(('v')))
         for arr in data.analogsignals:
-            self.assertEqual(arr.shape, (n_values, p.size))
+            self.assertEqual(arr.shape, (n_values, pv.size))
 
     def test_record_v(self, sim=sim):
-        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
-        p.record = Mock()
-        p.record_v("arg1")
-        p.record.assert_called_with('v', "arg1")
+        pv = sim.Population(2, sim.EIF_cond_exp_isfa_ista())[0:1]
+        pv.record = Mock()
+        pv.record_v("arg1")
+        pv.record.assert_called_with('v', "arg1")
 
     def test_record_gsyn(self, sim=sim):
-        p = sim.Population(2, sim.EIF_cond_exp_isfa_ista())
-        p.record = Mock()
-        p.record_gsyn("arg1")
-        p.record.assert_called_with(['gsyn_exc', 'gsyn_inh'], "arg1")
+        pv = sim.Population(2, sim.EIF_cond_exp_isfa_ista())[1:]
+        pv.record = Mock()
+        pv.record_gsyn("arg1")
+        pv.record.assert_called_with(['gsyn_exc', 'gsyn_inh'], "arg1")
 
     def test_record_invalid_variable(self, sim=sim):
-        p = sim.Population(14, sim.IF_curr_alpha())
+        pv = sim.Population(14, sim.IF_curr_alpha())[::3]
         self.assertRaises(errors.RecordingError,
-                          p.record, ('v', 'gsyn_exc'))  # can't record gsyn_exc from this celltype
+                          pv.record, ('v', 'gsyn_exc'))  # can't record gsyn_exc from this celltype
 
     # def test_write_data(self, sim=sim):
     #    self.fail()
     #
 
     def test_get_data_with_gather(self, sim=sim):
         t1 = 12.3
         t2 = 13.4
         t3 = 14.5
         p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
-        p.record('v')
+        pv = p[::3]
+        pv.record('v')
         sim.run(t1)
         # what if we call p.record between two run statements?
         # would be nice to get an AnalogSignal with a non-zero t_start
         # but then need to make sure we get the right initial value
         sim.run(t2)
         sim.reset()
-        p.record('spikes')
-        p.record('w')
+        pv.record('spikes')
+        pv.record('w')
         sim.run(t3)
         data = p.get_data(gather=True)
         self.assertEqual(len(data.segments), 2)
 
         seg0 = data.segments[0]
         self.assertEqual(len(seg0.analogsignals), 1)
         v = seg0.analogsignals[0]
         self.assertEqual(v.name, 'v')
         num_points = int(round((t1 + t2) / sim.get_time_step())) + 1
-        self.assertEqual(v.shape, (num_points, p.size))
+        self.assertEqual(v.shape, (num_points, pv.size))
         self.assertEqual(v.t_start, 0.0 * pq.ms)
         self.assertEqual(v.units, pq.mV)
         self.assertEqual(v.sampling_period, 0.1 * pq.ms)
         self.assertEqual(len(seg0.spiketrains), 0)
 
         seg1 = data.segments[1]
         self.assertEqual(len(seg1.analogsignals), 2)
         w = seg1.filter(name='w')[0]
         self.assertEqual(w.name, 'w')
         num_points = int(round(t3 / sim.get_time_step())) + 1
-        self.assertEqual(w.shape, (num_points, p.size))
+        self.assertEqual(w.shape, (num_points, pv.size))
         self.assertEqual(v.t_start, 0.0)
-        self.assertEqual(len(seg1.spiketrains), p.size)
+        self.assertEqual(len(seg1.spiketrains), pv.size)
 
-    def test_get_spikes_with_gather(self, sim=sim):
+    def test_get_data_with_gather(self, sim=sim):
         t1 = 12.3
         t2 = 13.4
         t3 = 14.5
         p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
-        p.record('v')
+        pv = p[::3]
+        pv.record('v')
         sim.run(t1)
+        # what if we call p.record between two run statements?
+        # would be nice to get an AnalogSignal with a non-zero t_start
+        # but then need to make sure we get the right initial value
         sim.run(t2)
         sim.reset()
-        p.record('spikes')
-        p.record('w')
+        pv.record('spikes')
+        pv.record('w')
         sim.run(t3)
         data = p.get_data(gather=True)
         self.assertEqual(len(data.segments), 2)
 
         seg0 = data.segments[0]
         self.assertEqual(len(seg0.analogsignals), 1)
         self.assertEqual(len(seg0.spiketrains), 0)
 
         seg1 = data.segments[1]
         self.assertEqual(len(seg1.analogsignals), 2)
-        self.assertEqual(len(seg1.spiketrains), p.size)
-        assert_array_equal(seg1.spiketrains[7],
-                           numpy.array([p.first_id + 7, p.first_id + 7 + 5]) % t3)
+        self.assertEqual(len(seg1.spiketrains), pv.size)
+        assert_array_equal(seg1.spiketrains[2],
+                           numpy.array([p.first_id + 6, p.first_id + 6 + 5]) % t3)
 
     # def test_get_data_no_gather(self, sim=sim):
     #    self.fail()
 
-    def test_printSpikes(self, sim=sim):
-        # TODO: implement assert_deprecated
-        p = sim.Population(3, sim.IF_curr_alpha())
-        p.record('spikes')
-        sim.run(10.0)
-        p.write_data = Mock()
-        p.printSpikes("foo.txt")
-        p.write_data.assert_called_with('foo.txt', 'spikes', True)
-
-    def test_getSpikes(self, sim=sim):
-        p = sim.Population(3, sim.IF_curr_alpha())
-        p.record('spikes')
-        sim.run(10.0)
-        p.get_data = Mock()
-        p.getSpikes()
-        p.get_data.assert_called_with('spikes', True)
-
-    def test_print_v(self, sim=sim):
-        p = sim.Population(3, sim.IF_curr_alpha())
-        p.record_v()
-        sim.run(10.0)
-        p.write_data = Mock()
-        p.print_v("foo.txt")
-        p.write_data.assert_called_with('foo.txt', 'v', True)
-
-    def test_get_v(self, sim=sim):
-        p = sim.Population(3, sim.IF_curr_alpha())
-        p.record_v()
-        sim.run(10.0)
-        p.get_data = Mock()
-        p.get_v()
-        p.get_data.assert_called_with('v', True)
-
-    def test_print_gsyn(self, sim=sim):
-        p = sim.Population(3, sim.IF_cond_alpha())
-        p.record_gsyn()
-        sim.run(10.0)
-        p.write_data = Mock()
-        p.print_gsyn("foo.txt")
-        p.write_data.assert_called_with('foo.txt', ['gsyn_exc', 'gsyn_inh'], True)
-
-    def test_get_gsyn(self, sim=sim):
-        p = sim.Population(3, sim.IF_cond_alpha())
-        p.record_gsyn()
-        sim.run(10.0)
-        p.get_data = Mock()
-        p.get_gsyn()
-        p.get_data.assert_called_with(['gsyn_exc', 'gsyn_inh'], True)
-
     def test_get_spike_counts(self, sim=sim):
-        p = sim.Population(3, sim.EIF_cond_exp_isfa_ista())
-        p.record('spikes')
+        p = sim.Population(5, sim.EIF_cond_exp_isfa_ista())
+        pv = p[0, 1, 4]
+        pv.record('spikes')
         sim.run(100.0)
         self.assertEqual(p.get_spike_counts(),
                          {p.all_cells[0]: 2,
-                             p.all_cells[1]: 2,
-                             p.all_cells[2]: 2})
+                          p.all_cells[1]: 2,
+                          p.all_cells[4]: 2})
 
     def test_mean_spike_count(self, sim=sim):
         p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
-        p.record('spikes')
+        pv = p[2::3]
+        pv.record('spikes')
         sim.run(100.0)
-        # mock backend always produces two spikes per population
         self.assertEqual(p.mean_spike_count(), 2.0)
 
     # def test_mean_spike_count_on_slave_node():
 
-    def test_meanSpikeCount(self, sim=sim):
-        p = sim.Population(14, sim.EIF_cond_exp_isfa_ista())
-        p.record('spikes')
-        sim.run(100.0)
-        p.mean_spike_count = Mock()
-        p.meanSpikeCount()
-        self.assertTrue(p.mean_spike_count.called)
-
     def test_inject(self, sim=sim):
-        p = sim.Population(3, sim.IF_curr_alpha())
+        pv = sim.Population(3, sim.IF_curr_alpha())[1, 2]
         cs = Mock()
-        p.inject(cs)
+        pv.inject(cs)
         meth, args, kwargs = cs.method_calls[0]
         self.assertEqual(meth, "inject_into")
-        self.assertEqual(args, (p,))
+        self.assertEqual(args, (pv,))
 
     def test_inject_into_invalid_celltype(self, sim=sim):
-        p = sim.Population(3, sim.SpikeSourceArray())
-        self.assertRaises(TypeError, p.inject, Mock())
+        pv = sim.Population(3, sim.SpikeSourceArray())[:2]
+        self.assertRaises(TypeError, pv.inject, Mock())
 
     # def test_save_positions(self, sim=sim):
     #    self.fail()
 
     # test describe method
 
     def test_describe(self, sim=sim):
-        p = sim.Population(11, sim.IF_cond_exp())
-        self.assertIsInstance(p.describe(), basestring)
-        self.assertIsInstance(p.describe(template=None), dict)
+        pv = sim.Population(11, sim.IF_cond_exp())[::4]
+        self.assertIsInstance(pv.describe(), basestring)
+        self.assertIsInstance(pv.describe(template=None), dict)
+
+    def test_index_in_grandparent(self, sim=sim):
+        pv1 = sim.Population(11, sim.IF_cond_exp())[0, 1, 3, 4, 6, 7, 9]
+        pv2 = pv1[2, 3, 5, 6]
+        assert_array_equal(pv1.index_in_grandparent([2, 4, 6]), numpy.array([3, 6, 9]))
+        assert_array_equal(pv2.index_in_grandparent([0, 1, 3]), numpy.array([3, 4, 9]))
+
+    def test_index_from_parent_index(self, sim=sim):
+        parent = sim.Population(20, sim.IF_cond_exp())
+
+        # test with slice mask
+        pv1 = parent[2:16:3]
+        assert_array_equal(
+            pv1.index_from_parent_index(numpy.array([2, 5, 8, 11, 14])),
+            numpy.array([0, 1, 2, 3, 4])
+        )
+        self.assertEqual(pv1.index_from_parent_index(11), 3)
+
+        # test with array mask
+        pv2 = parent[numpy.array([1, 2, 3, 5, 8, 13])]
+        assert_array_equal(
+            pv2.index_from_parent_index(numpy.array([2, 5, 13])),
+            numpy.array([1, 3, 5])
+        )
+
 
     def test_save_positions(self, sim=sim):
         import os
-        p = sim.Population(4, sim.IF_cond_exp(), )
-        p.positions = numpy.arange(15, 27).reshape((4, 3)).T
+        p = sim.Population(7, sim.IF_cond_exp())
+        p.positions = numpy.arange(15, 36).reshape((7, 3)).T
+        pv = p[2, 4, 5]
         output_file = Mock()
-        p.save_positions(output_file)
+        pv.save_positions(output_file)
         assert_array_equal(output_file.write.call_args[0][0],
-                           numpy.array([[0, 15, 16, 17],
-                                        [1, 18, 19, 20],
-                                        [2, 21, 22, 23],
-                                        [3, 24, 25, 26]]))
-        self.assertEqual(output_file.write.call_args[0][1], {'population': p.label})
+                           numpy.array([[0, 21, 22, 23],
+                                        [1, 27, 28, 29],
+                                        [2, 30, 31, 32]]))
+        self.assertEqual(output_file.write.call_args[0][1], {'population': pv.label})
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `PyNN-0.9.5/test/unittests/test_projection.py` & `PyNN-0.9.6/test/unittests/test_projection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tests of the common implementation of the Projection class, using the
 pyNN.mock backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
@@ -22,15 +22,15 @@
 try:
     basestring
 except NameError:
     basestring = str
 from .mocks import MockRNG
 import pyNN.mock as sim
 
-from pyNN import random, errors, space
+from pyNN import random, errors, space, standardmodels
 from pyNN.parameters import Sequence
 
 
 def _sort_by_column(A, col):
     A = numpy.array(A)
     array_index = numpy.argsort(A[:, col], kind='mergesort')
     return A[array_index]
@@ -77,14 +77,25 @@
                              synapse_type=depressing)
 
     def test_create_with_invalid_type(self, sim=sim):
         self.assertRaises(errors.ConnectionError, sim.Projection,
                           self.p1, "foo", connector=self.all2all,
                           synapse_type=self.syn2)
 
+    def test_create_with_default_receptor_type(self, sim=sim):
+        prj = sim.Projection(self.p1, self.p3, connector=self.all2all,
+                             synapse_type=sim.StaticSynapse())
+        self.assertEqual(prj.receptor_type, "excitatory")
+        prj = sim.Projection(self.p1, self.p3, connector=self.all2all,
+                             synapse_type=sim.TsodyksMarkramSynapse(weight=0.5))
+        self.assertEqual(prj.receptor_type, "excitatory")
+        prj = sim.Projection(self.p1, self.p3, connector=self.all2all,
+                             synapse_type=sim.StaticSynapse(weight=lambda d: -0.1 * d))
+        self.assertEqual(prj.receptor_type, "inhibitory")
+
     def test_size_with_gather(self, sim=sim):
         prj = sim.Projection(self.p1, self.p2, connector=self.all2all, synapse_type=self.syn2)
         self.assertEqual(prj.size(gather=True), self.p1.size * self.p2.size)
 
 # Need to extend the mock backend before setting synaptic parameters can be properly tested
 
     # def test_set_weights(self, sim=sim):
@@ -285,7 +296,97 @@
 
     def test_weightHistogram(self, sim=sim):
         prj = sim.Projection(self.p1, self.p2, connector=self.all2all,
                              synapse_type=self.syn2)
         n, bins = prj.weightHistogram(min=0.0, max=0.05)
         assert_array_equal(bins, numpy.linspace(0, 0.05, num=11))
         assert_array_equal(n, numpy.array([0, prj.size(), 0, 0, 0, 0, 0, 0, 0, 0]))
+
+
+class CheckTest(unittest.TestCase):
+
+    def setUp(self, sim=sim, **extra):
+        self.MIN_DELAY = 0.123
+        sim.setup(num_processes=2, rank=1, min_delay=self.MIN_DELAY, **extra)
+        self.p1 = sim.Population(7, sim.IF_cond_exp())
+        self.p2 = sim.Population(4, sim.IF_cond_exp())
+        self.p3 = sim.Population(5, sim.IF_curr_alpha())
+        self.projections = {
+            "cond": {},
+            "curr": {}
+        }
+        for psr, post in (("cond", self.p2), ("curr", self.p3)):
+            for rt in ("excitatory", "inhibitory"):
+                self.projections[psr][rt] = sim.Projection(
+                    self.p1, post, sim.AllToAllConnector(safe=True),
+                    sim.StaticSynapse(), receptor_type=rt
+                )
+
+    def test_check_weights_with_scalar(self, sim=sim):
+        # positive weight
+        for prj in [
+            self.projections["cond"]["excitatory"],
+            self.projections["curr"]["excitatory"],
+            self.projections["cond"]["inhibitory"],
+        ]:
+            standardmodels.check_weights(4.3, prj)
+        for prj in [
+            self.projections["curr"]["inhibitory"],
+        ]:
+            self.assertRaises(errors.ConnectionError, standardmodels.check_weights, 4.3, prj)
+
+        # negative weight
+        for prj in [
+            self.projections["cond"]["excitatory"],
+            self.projections["curr"]["excitatory"],
+            self.projections["cond"]["inhibitory"],
+        ]:
+            self.assertRaises(errors.ConnectionError, standardmodels.check_weights, -4.3, prj)
+        for prj in [
+            self.projections["curr"]["inhibitory"],
+        ]:
+            standardmodels.check_weights(-4.3, prj)
+
+    def test_check_weights_with_array(self, sim=sim):
+        # all positive weights
+        w = numpy.arange(10)
+        for prj in [
+            self.projections["cond"]["excitatory"],
+            self.projections["curr"]["excitatory"],
+            self.projections["cond"]["inhibitory"],
+        ]:
+            standardmodels.check_weights(w, prj)
+        for prj in [
+            self.projections["curr"]["inhibitory"],
+        ]:
+            self.assertRaises(errors.ConnectionError, standardmodels.check_weights, w, prj)
+        # all negative weights
+        w = numpy.arange(-10, 0)
+        for prj in [
+            self.projections["cond"]["excitatory"],
+            self.projections["curr"]["excitatory"],
+            self.projections["cond"]["inhibitory"],
+        ]:
+            self.assertRaises(errors.ConnectionError, standardmodels.check_weights, w, prj)
+        for prj in [
+            self.projections["curr"]["inhibitory"],
+        ]:
+            standardmodels.check_weights(w, prj)
+        # mixture of positive and negative weights
+        w = numpy.arange(-5, 5)
+        for prj in [
+            self.projections["cond"]["excitatory"],
+            self.projections["curr"]["excitatory"],
+            self.projections["cond"]["inhibitory"],
+            self.projections["curr"]["inhibitory"]
+        ]:
+            self.assertRaises(errors.ConnectionError, standardmodels.check_weights, w, prj)
+
+    def test_check_weights_with_invalid_value(self, sim=sim):
+        w = "butterflies"
+        for prj in [
+            self.projections["cond"]["excitatory"],
+            self.projections["curr"]["excitatory"],
+            self.projections["cond"]["inhibitory"],
+            self.projections["curr"]["inhibitory"]
+        ]:
+            self.assertRaises(errors.ConnectionError, standardmodels.check_weights, w, prj)
```

### Comparing `PyNN-0.9.5/test/unittests/test_random.py` & `PyNN-0.9.6/test/unittests/test_random.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_recording.py` & `PyNN-0.9.6/test/unittests/test_recording.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_simulation_control.py` & `PyNN-0.9.6/test/unittests/test_simulation_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tests of the common implementation of the simulation control functions, using
 the pyNN.mock backend.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
```

### Comparing `PyNN-0.9.5/test/unittests/test_space.py` & `PyNN-0.9.6/test/unittests/test_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Tests of the `space` module.
 
-:copyright: Copyright 2006-2019 by the PyNN team, see AUTHORS.
+:copyright: Copyright 2006-2020 by the PyNN team, see AUTHORS.
 :license: CeCILL, see LICENSE for details.
 """
 
 from pyNN import space
 import unittest
 import numpy
 try:
```

### Comparing `PyNN-0.9.5/test/unittests/test_standardmodels.py` & `PyNN-0.9.6/test/unittests/test_standardmodels.py`

 * *Files identical despite different names*

### Comparing `PyNN-0.9.5/test/unittests/test_utility_functions.py` & `PyNN-0.9.6/test/unittests/test_utility_functions.py`

 * *Files identical despite different names*

