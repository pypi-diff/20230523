# Comparing `tmp/smac-2.0.0b1.tar.gz` & `tmp/smac-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smac-2.0.0b1.tar", last modified: Sat Jan  7 10:48:09 2023, max compression
+gzip compressed data, was "smac-2.0.1.tar", last modified: Tue May 23 12:28:37 2023, max compression
```

## Comparing `smac-2.0.0b1.tar` & `smac-2.0.1.tar`

### file list

```diff
@@ -1,145 +1,148 @@
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.628440 smac-2.0.0b1/
--rw-r--r--   0 rene       (501) staff       (20)     3377 2022-10-26 10:50:54.000000 smac-2.0.0b1/LICENSE.txt
--rw-r--r--   0 rene       (501) staff       (20)      127 2022-10-27 09:47:53.000000 smac-2.0.0b1/MANIFEST.in
--rw-r--r--   0 rene       (501) staff       (20)     6594 2023-01-07 10:48:09.628230 smac-2.0.0b1/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     5438 2022-12-20 14:56:19.000000 smac-2.0.0b1/README.md
--rw-r--r--   0 rene       (501) staff       (20)     2887 2022-12-20 14:56:00.000000 smac-2.0.0b1/pyproject.toml
--rw-r--r--   0 rene       (501) staff       (20)       38 2023-01-07 10:48:09.628484 smac-2.0.0b1/setup.cfg
--rw-r--r--   0 rene       (501) staff       (20)     2278 2022-12-20 14:56:00.000000 smac-2.0.0b1/setup.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.594038 smac-2.0.0b1/smac/
--rw-r--r--   0 rene       (501) staff       (20)     1620 2022-12-20 15:26:32.000000 smac-2.0.0b1/smac/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.595226 smac-2.0.0b1/smac/acquisition/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/acquisition/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.597499 smac-2.0.0b1/smac/acquisition/function/
--rw-r--r--   0 rene       (501) staff       (20)      717 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/acquisition/function/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3552 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/acquisition/function/abstract_acquisition_function.py
--rw-r--r--   0 rene       (501) staff       (20)     3086 2022-12-20 19:32:04.000000 smac-2.0.0b1/smac/acquisition/function/confidence_bound.py
--rw-r--r--   0 rene       (501) staff       (20)     9061 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/acquisition/function/expected_improvement.py
--rw-r--r--   0 rene       (501) staff       (20)     4002 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/acquisition/function/integrated_acquisition_function.py
--rw-r--r--   0 rene       (501) staff       (20)     9380 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/acquisition/function/prior_acqusition_function.py
--rw-r--r--   0 rene       (501) staff       (20)     2692 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/acquisition/function/probability_improvement.py
--rw-r--r--   0 rene       (501) staff       (20)     1930 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/acquisition/function/thompson.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.599807 smac-2.0.0b1/smac/acquisition/maximizer/
--rw-r--r--   0 rene       (501) staff       (20)      649 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/acquisition/maximizer/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     5969 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/acquisition/maximizer/abstract_acqusition_maximizer.py
--rw-r--r--   0 rene       (501) staff       (20)     1695 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/acquisition/maximizer/differential_evolution.py
--rw-r--r--   0 rene       (501) staff       (20)     4212 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/acquisition/maximizer/helpers.py
--rw-r--r--   0 rene       (501) staff       (20)     9942 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/acquisition/maximizer/local_and_random_search.py
--rw-r--r--   0 rene       (501) staff       (20)    17428 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/acquisition/maximizer/local_search.py
--rw-r--r--   0 rene       (501) staff       (20)     1764 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/acquisition/maximizer/random_search.py
--rw-r--r--   0 rene       (501) staff       (20)     2519 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/callback.py
--rw-r--r--   0 rene       (501) staff       (20)      270 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/constants.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.601533 smac-2.0.0b1/smac/facade/
--rw-r--r--   0 rene       (501) staff       (20)      674 2022-11-30 15:29:30.000000 smac-2.0.0b1/smac/facade/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    18808 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/abstract_facade.py
--rw-r--r--   0 rene       (501) staff       (20)     6199 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/algorithm_configuration_facade.py
--rw-r--r--   0 rene       (501) staff       (20)    11605 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/blackbox_facade.py
--rw-r--r--   0 rene       (501) staff       (20)     2394 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/hyperband_facade.py
--rw-r--r--   0 rene       (501) staff       (20)     7578 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/hyperparameter_optimization_facade.py
--rw-r--r--   0 rene       (501) staff       (20)     3930 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/multi_fidelity_facade.py
--rw-r--r--   0 rene       (501) staff       (20)     5976 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/facade/random_facade.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.603816 smac-2.0.0b1/smac/initial_design/
--rw-r--r--   0 rene       (501) staff       (20)      621 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/initial_design/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     7513 2022-12-30 10:48:08.000000 smac-2.0.0b1/smac/initial_design/abstract_initial_design.py
--rw-r--r--   0 rene       (501) staff       (20)      536 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/initial_design/default_design.py
--rw-r--r--   0 rene       (501) staff       (20)     2201 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/initial_design/factorial_design.py
--rw-r--r--   0 rene       (501) staff       (20)     1083 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/initial_design/latin_hypercube_design.py
--rw-r--r--   0 rene       (501) staff       (20)      655 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/initial_design/random_design.py
--rw-r--r--   0 rene       (501) staff       (20)     1670 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/initial_design/sobol_design.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.605824 smac-2.0.0b1/smac/intensifier/
--rw-r--r--   0 rene       (501) staff       (20)      341 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/intensifier/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    31249 2022-12-30 10:47:47.000000 smac-2.0.0b1/smac/intensifier/abstract_intensifier.py
--rw-r--r--   0 rene       (501) staff       (20)     2628 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/intensifier/hyperband.py
--rw-r--r--   0 rene       (501) staff       (20)    17257 2022-12-30 10:43:52.000000 smac-2.0.0b1/smac/intensifier/intensifier.py
--rw-r--r--   0 rene       (501) staff       (20)    23689 2022-12-30 11:10:08.000000 smac-2.0.0b1/smac/intensifier/successive_halving.py
--rw-r--r--   0 rene       (501) staff       (20)      553 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/logging.yml
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.607027 smac-2.0.0b1/smac/main/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/main/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    14824 2022-12-20 15:21:57.000000 smac-2.0.0b1/smac/main/config_selector.py
--rw-r--r--   0 rene       (501) staff       (20)    22946 2022-12-20 15:01:27.000000 smac-2.0.0b1/smac/main/smbo.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.608700 smac-2.0.0b1/smac/model/
--rw-r--r--   0 rene       (501) staff       (20)      247 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    11457 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/model/abstract_model.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.610482 smac-2.0.0b1/smac/model/gaussian_process/
--rw-r--r--   0 rene       (501) staff       (20)      350 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     6523 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/abstract_gaussian_process.py
--rw-r--r--   0 rene       (501) staff       (20)    10482 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/model/gaussian_process/gaussian_process.py
--rw-r--r--   0 rene       (501) staff       (20)    35950 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/model/gaussian_process/gpytorch_gaussian_process.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.612937 smac-2.0.0b1/smac/model/gaussian_process/kernels/
--rw-r--r--   0 rene       (501) staff       (20)      607 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    23169 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/_boing.py
--rw-r--r--   0 rene       (501) staff       (20)    17034 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/base_kernels.py
--rw-r--r--   0 rene       (501) staff       (20)     3648 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/hamming_kernel.py
--rw-r--r--   0 rene       (501) staff       (20)     4121 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/matern_kernel.py
--rw-r--r--   0 rene       (501) staff       (20)     2738 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/rbf_kernel.py
--rw-r--r--   0 rene       (501) staff       (20)     1881 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/kernels/white_kernel.py
--rw-r--r--   0 rene       (501) staff       (20)    16808 2022-12-20 15:25:23.000000 smac-2.0.0b1/smac/model/gaussian_process/mcmc_gaussian_process.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.614909 smac-2.0.0b1/smac/model/gaussian_process/priors/
--rw-r--r--   0 rene       (501) staff       (20)      435 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/priors/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     4306 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/priors/abstract_prior.py
--rw-r--r--   0 rene       (501) staff       (20)     2013 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/priors/gamma_prior.py
--rw-r--r--   0 rene       (501) staff       (20)     2402 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/priors/horseshoe_prior.py
--rw-r--r--   0 rene       (501) staff       (20)     1900 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/priors/log_normal_prior.py
--rw-r--r--   0 rene       (501) staff       (20)     5338 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/gaussian_process/priors/tophat_prior.py
--rw-r--r--   0 rene       (501) staff       (20)     3002 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/multi_objective_model.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.615772 smac-2.0.0b1/smac/model/random_forest/
--rw-r--r--   0 rene       (501) staff       (20)      208 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/random_forest/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1741 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/random_forest/abstract_random_forest.py
--rw-r--r--   0 rene       (501) staff       (20)    11615 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/random_forest/random_forest.py
--rw-r--r--   0 rene       (501) staff       (20)     1206 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/model/random_model.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.617012 smac-2.0.0b1/smac/multi_objective/
--rw-r--r--   0 rene       (501) staff       (20)      333 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/multi_objective/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1038 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/multi_objective/abstract_multi_objective_algorithm.py
--rw-r--r--   0 rene       (501) staff       (20)     1399 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/multi_objective/aggregation_strategy.py
--rw-r--r--   0 rene       (501) staff       (20)     1902 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/multi_objective/parego.py
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-10-26 10:50:54.000000 smac-2.0.0b1/smac/py.typed
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.618786 smac-2.0.0b1/smac/random_design/
--rw-r--r--   0 rene       (501) staff       (20)      585 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/random_design/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1362 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/random_design/abstract_random_design.py
--rw-r--r--   0 rene       (501) staff       (20)     2691 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/random_design/annealing_design.py
--rw-r--r--   0 rene       (501) staff       (20)     3489 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/random_design/modulus_design.py
--rw-r--r--   0 rene       (501) staff       (20)     2439 2022-12-20 15:14:23.000000 smac-2.0.0b1/smac/random_design/probability_design.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.620363 smac-2.0.0b1/smac/runhistory/
--rw-r--r--   0 rene       (501) staff       (20)      393 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/runhistory/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     4337 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runhistory/dataclasses.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.623007 smac-2.0.0b1/smac/runhistory/encoder/
--rw-r--r--   0 rene       (501) staff       (20)     1076 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/runhistory/encoder/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    10551 2022-12-21 15:39:39.000000 smac-2.0.0b1/smac/runhistory/encoder/abstract_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)     2443 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/runhistory/encoder/boing_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)     2878 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runhistory/encoder/eips_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)     2540 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/runhistory/encoder/encoder.py
--rw-r--r--   0 rene       (501) staff       (20)     1372 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runhistory/encoder/inverse_scaled_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)      867 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runhistory/encoder/log_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)     1180 2022-12-08 13:43:08.000000 smac-2.0.0b1/smac/runhistory/encoder/log_scaled_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)      978 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/runhistory/encoder/scaled_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)     1354 2022-11-07 08:51:35.000000 smac-2.0.0b1/smac/runhistory/encoder/sqrt_scaled_encoder.py
--rw-r--r--   0 rene       (501) staff       (20)      356 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runhistory/enumerations.py
--rw-r--r--   0 rene       (501) staff       (20)       48 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/runhistory/errors.py
--rw-r--r--   0 rene       (501) staff       (20)    41099 2022-12-30 10:58:11.000000 smac-2.0.0b1/smac/runhistory/runhistory.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.625012 smac-2.0.0b1/smac/runner/
--rw-r--r--   0 rene       (501) staff       (20)      472 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/runner/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     8732 2022-12-30 10:52:09.000000 smac-2.0.0b1/smac/runner/abstract_runner.py
--rw-r--r--   0 rene       (501) staff       (20)     1787 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runner/abstract_serial_runner.py
--rw-r--r--   0 rene       (501) staff       (20)     8413 2022-12-30 10:54:43.000000 smac-2.0.0b1/smac/runner/dask_runner.py
--rw-r--r--   0 rene       (501) staff       (20)      419 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/runner/exceptions.py
--rw-r--r--   0 rene       (501) staff       (20)     8008 2022-12-30 10:55:38.000000 smac-2.0.0b1/smac/runner/target_function_runner.py
--rw-r--r--   0 rene       (501) staff       (20)     7486 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/runner/target_function_script_runner.py
--rw-r--r--   0 rene       (501) staff       (20)     9908 2022-12-30 11:06:26.000000 smac-2.0.0b1/smac/scenario.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.626590 smac-2.0.0b1/smac/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-10-26 10:50:54.000000 smac-2.0.0b1/smac/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     9225 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/utils/configspace.py
--rw-r--r--   0 rene       (501) staff       (20)     2276 2022-12-20 14:55:46.000000 smac-2.0.0b1/smac/utils/data_structures.py
--rw-r--r--   0 rene       (501) staff       (20)     1084 2022-12-20 19:32:32.000000 smac-2.0.0b1/smac/utils/logging.py
--rw-r--r--   0 rene       (501) staff       (20)     1159 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/utils/multi_objective.py
--rw-r--r--   0 rene       (501) staff       (20)     6018 2022-12-20 14:56:19.000000 smac-2.0.0b1/smac/utils/pareto_front.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.627660 smac-2.0.0b1/smac/utils/subspaces/
--rw-r--r--   0 rene       (501) staff       (20)    29592 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/utils/subspaces/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     8717 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/utils/subspaces/boing_subspace.py
--rw-r--r--   0 rene       (501) staff       (20)    13823 2022-10-27 09:47:53.000000 smac-2.0.0b1/smac/utils/subspaces/turbo_subspace.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-01-07 10:48:09.595095 smac-2.0.0b1/smac.egg-info/
--rw-r--r--   0 rene       (501) staff       (20)     6594 2023-01-07 10:48:09.000000 smac-2.0.0b1/smac.egg-info/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     4474 2023-01-07 10:48:09.000000 smac-2.0.0b1/smac.egg-info/SOURCES.txt
--rw-r--r--   0 rene       (501) staff       (20)        1 2023-01-07 10:48:09.000000 smac-2.0.0b1/smac.egg-info/dependency_links.txt
--rw-r--r--   0 rene       (501) staff       (20)       53 2023-01-07 10:48:09.000000 smac-2.0.0b1/smac.egg-info/entry_points.txt
--rw-r--r--   0 rene       (501) staff       (20)      442 2023-01-07 10:48:09.000000 smac-2.0.0b1/smac.egg-info/requires.txt
--rw-r--r--   0 rene       (501) staff       (20)       11 2023-01-07 10:48:09.000000 smac-2.0.0b1/smac.egg-info/top_level.txt
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3377 2023-03-03 09:52:31.000000 smac-2.0.1/LICENSE.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      127 2023-03-03 09:52:31.000000 smac-2.0.1/MANIFEST.in
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7272 2023-05-23 12:28:37.844321 smac-2.0.1/PKG-INFO
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6116 2023-05-22 12:55:22.000000 smac-2.0.1/README.md
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2887 2023-03-03 09:52:31.000000 smac-2.0.1/pyproject.toml
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       38 2023-05-23 12:28:37.844321 smac-2.0.1/setup.cfg
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2303 2023-05-22 12:55:22.000000 smac-2.0.1/setup.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1555 2023-05-22 12:55:22.000000 smac-2.0.1/smac/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/acquisition/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/acquisition/function/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      717 2023-05-16 11:11:34.000000 smac-2.0.1/smac/acquisition/function/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3552 2023-05-16 11:11:34.000000 smac-2.0.1/smac/acquisition/function/abstract_acquisition_function.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3086 2023-05-16 11:11:34.000000 smac-2.0.1/smac/acquisition/function/confidence_bound.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9061 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/expected_improvement.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4002 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/integrated_acquisition_function.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9380 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/prior_acqusition_function.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2692 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/probability_improvement.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1930 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/thompson.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/acquisition/maximizer/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      649 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/maximizer/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6213 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/abstract_acqusition_maximizer.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2344 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/differential_evolution.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4165 2023-05-22 12:55:22.000000 smac-2.0.1/smac/acquisition/maximizer/helpers.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10116 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/local_and_random_search.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    19915 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/local_search.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1828 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/random_search.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/callback/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      160 2023-05-22 12:55:22.000000 smac-2.0.1/smac/callback/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2519 2023-05-22 12:55:22.000000 smac-2.0.1/smac/callback/callback.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1013 2023-05-22 12:55:22.000000 smac-2.0.1/smac/callback/metadata_callback.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      270 2023-03-03 09:52:31.000000 smac-2.0.1/smac/constants.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/facade/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      674 2023-03-03 09:52:31.000000 smac-2.0.1/smac/facade/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    20537 2023-05-22 12:55:22.000000 smac-2.0.1/smac/facade/abstract_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6199 2023-03-03 09:52:31.000000 smac-2.0.1/smac/facade/algorithm_configuration_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11605 2023-04-11 12:42:46.000000 smac-2.0.1/smac/facade/blackbox_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2394 2023-05-16 11:11:34.000000 smac-2.0.1/smac/facade/hyperband_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7578 2023-05-16 11:11:34.000000 smac-2.0.1/smac/facade/hyperparameter_optimization_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4387 2023-05-16 11:11:34.000000 smac-2.0.1/smac/facade/multi_fidelity_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5976 2023-03-03 09:52:31.000000 smac-2.0.1/smac/facade/random_facade.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/initial_design/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      621 2023-03-03 09:52:31.000000 smac-2.0.1/smac/initial_design/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8211 2023-05-22 12:55:22.000000 smac-2.0.1/smac/initial_design/abstract_initial_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      552 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/default_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2202 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/factorial_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1084 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/latin_hypercube_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      656 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/random_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1671 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/sobol_design.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/intensifier/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      341 2023-03-03 09:52:31.000000 smac-2.0.1/smac/intensifier/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    33241 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/abstract_intensifier.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2159 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/hyperband.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17357 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/intensifier.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24457 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/successive_halving.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      553 2023-03-03 09:52:31.000000 smac-2.0.1/smac/logging.yml
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/main/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-05-05 11:32:22.000000 smac-2.0.1/smac/main/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14833 2023-05-22 12:55:22.000000 smac-2.0.1/smac/main/config_selector.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24432 2023-05-22 12:55:22.000000 smac-2.0.1/smac/main/smbo.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/model/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      247 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11457 2023-05-16 11:11:34.000000 smac-2.0.1/smac/model/abstract_model.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/model/gaussian_process/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      350 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6523 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/abstract_gaussian_process.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10482 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/gaussian_process.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    35950 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/gpytorch_gaussian_process.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/model/gaussian_process/kernels/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      607 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    23169 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/_boing.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17034 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/base_kernels.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3648 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/hamming_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4121 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/matern_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2738 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/rbf_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1881 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/white_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    16808 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/mcmc_gaussian_process.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/model/gaussian_process/priors/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      435 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4306 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/abstract_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2013 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/gamma_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2402 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/horseshoe_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1900 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/log_normal_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5338 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/tophat_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3002 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/multi_objective_model.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/model/random_forest/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      208 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/random_forest/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1741 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/random_forest/abstract_random_forest.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10805 2023-03-03 10:08:13.000000 smac-2.0.1/smac/model/random_forest/random_forest.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1206 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/random_model.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/multi_objective/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      333 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1038 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/abstract_multi_objective_algorithm.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1399 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/aggregation_strategy.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1902 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/parego.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.1/smac/py.typed
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/random_design/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      585 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1362 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/abstract_random_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2691 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/annealing_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3489 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/modulus_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2439 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/probability_design.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/runhistory/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      393 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4337 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/dataclasses.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/runhistory/encoder/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1076 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/encoder/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10551 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/abstract_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2443 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/encoder/boing_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2878 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/eips_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2540 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1372 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/encoder/inverse_scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      867 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/log_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1180 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/log_scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      978 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1354 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/sqrt_scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      356 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/enumerations.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       48 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/errors.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    41541 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runhistory/runhistory.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/runner/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      472 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9402 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runner/abstract_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1787 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/abstract_serial_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9153 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runner/dask_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      419 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/exceptions.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8927 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runner/target_function_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7486 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/target_function_script_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10868 2023-05-22 12:55:22.000000 smac-2.0.1/smac/scenario.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/utils/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9225 2023-05-16 11:11:34.000000 smac-2.0.1/smac/utils/configspace.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2276 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/data_structures.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1252 2023-05-22 12:55:22.000000 smac-2.0.1/smac/utils/logging.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1159 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/multi_objective.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6018 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/pareto_front.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/utils/subspaces/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    29592 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/subspaces/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8717 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/subspaces/boing_subspace.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13823 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/subspaces/turbo_subspace.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac.egg-info/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7272 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/PKG-INFO
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4544 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/SOURCES.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        1 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/dependency_links.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       53 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/entry_points.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      456 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/requires.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       11 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/top_level.txt
```

### Comparing `smac-2.0.0b1/LICENSE.txt` & `smac-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/PKG-INFO` & `smac-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smac
-Version: 2.0.0b1
+Version: 2.0.1
 Summary: SMAC3, a Python implementation of 'Sequential Model-based Algorithm Configuration'.
 Home-page: https://www.automl.org/
 Author: 	Marius Lindauer, Katharina Eggensperger, Matthias Feurer, André Biedenkapp, Difan Deng,
 	Carolin Benjamins, Tim Ruhkopf, René Sass and Frank Hutter
 Author-email: fh@cs.uni-freiburg.de
 License: BSD 3-Clause License
 Project-URL: Documentation, https://https://github.com/automl.github.io/SMAC3/main
@@ -31,17 +31,17 @@
 [![Tests](https://github.com/automl/SMAC3/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/pytest.yml)
 [![Documentation](https://github.com/automl/SMAC3/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/docs.yml)
 [![codecov
 Status](https://codecov.io/gh/automl/SMAC3/branch/master/graph/badge.svg)](https://codecov.io/gh/automl/SMAC3)
 
 <img src="docs/images/logo.png" style="width: 50%;" />
 
-SMAC is a tool for algorithm configuration to optimize the parameters of arbitrary algorithms, including hyperparameter 
-optimization of Machine Learning algorithms. The main core consists of Bayesian Optimization in combination with an 
-aggressive racing mechanism to efficiently decide which of two configurations performs better.
+SMAC offers a robust and flexible framework for Bayesian Optimization to support users in determining well-performing 
+hyperparameter configurations for their (Machine Learning) algorithms, datasets and applications at hand. The main core 
+consists of Bayesian Optimization in combination with an aggressive racing mechanism to efficiently decide which of two configurations performs better.
 
 SMAC3 is written in Python3 and continuously tested with Python 3.8, 3.9, and 3.10. Its Random
 Forest is written in C++. In further texts, SMAC is representatively mentioned for SMAC3.
 
 > [Documentation](https://automl.github.io/SMAC3)
 
 > [Roadmap](https://github.com/orgs/automl/projects/5/views/2)
@@ -80,18 +80,18 @@
 ```
 
 Install SMAC via PyPI:
 ```
 pip install smac
 ```
 
-Or alternatively, clone the environment:
+If you want to contribute to SMAC, use the following steps instead:
 ```
 git clone https://github.com/automl/SMAC3.git && cd SMAC3
-pip install -e .[dev]
+make install-dev
 ```
 
 
 ## Minimal Example
 
 ```py
 from ConfigSpace import Configuration, ConfigurationSpace
@@ -119,28 +119,37 @@
 # Use SMAC to find the best configuration/hyperparameters
 smac = HyperparameterOptimizationFacade(scenario, train)
 incumbent = smac.optimize()
 ```
 
 More examples can be found in the [documentation](https://automl.github.io/SMAC3/main/examples/).
 
+## Visualization via DeepCAVE
+
+With DeepCAVE ([Repo](https://github.com/automl/DeepCAVE), [Paper](https://arxiv.org/abs/2206.03493)) you can visualize your SMAC runs. It is a visualization and analysis tool for AutoML (especially for the sub-problem
+hyperparameter optimization) runs.
 
 ## License
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the 3-clause BSD license (please see the LICENSE file).
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
 You should have received a copy of the 3-clause BSD license
 along with this program (see LICENSE file).
 If not, see [here](https://opensource.org/licenses/BSD-3-Clause).
 
+## Contacting us
+
+If you have trouble using SMAC, a concrete question or found a bug, please create an [issue](https://github.com/automl/SMAC3/issues). This is the easiest way to communicate about these things with us. 
+
+For all other inquiries, please write an email to smac[at]ai[dot]uni[dash]hannover[dot]de.
 
 ## Miscellaneous
 
 SMAC3 is developed by the [AutoML Groups of the Universities of Hannover and
 Freiburg](http://www.automl.org/).
 
 If you have found a bug, please report to [issues](https://github.com/automl/SMAC3/issues). Moreover, we are 
@@ -159,7 +168,9 @@
   number  = {54},
   pages   = {1--9},
   url     = {http://jmlr.org/papers/v23/21-0888.html}
 }
 ```
 
 Copyright (C) 2016-2022  [AutoML Group](http://www.automl.org).
+
+
```

### Comparing `smac-2.0.0b1/README.md` & `smac-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 [![Tests](https://github.com/automl/SMAC3/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/pytest.yml)
 [![Documentation](https://github.com/automl/SMAC3/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/docs.yml)
 [![codecov
 Status](https://codecov.io/gh/automl/SMAC3/branch/master/graph/badge.svg)](https://codecov.io/gh/automl/SMAC3)
 
 <img src="docs/images/logo.png" style="width: 50%;" />
 
-SMAC is a tool for algorithm configuration to optimize the parameters of arbitrary algorithms, including hyperparameter 
-optimization of Machine Learning algorithms. The main core consists of Bayesian Optimization in combination with an 
-aggressive racing mechanism to efficiently decide which of two configurations performs better.
+SMAC offers a robust and flexible framework for Bayesian Optimization to support users in determining well-performing 
+hyperparameter configurations for their (Machine Learning) algorithms, datasets and applications at hand. The main core 
+consists of Bayesian Optimization in combination with an aggressive racing mechanism to efficiently decide which of two configurations performs better.
 
 SMAC3 is written in Python3 and continuously tested with Python 3.8, 3.9, and 3.10. Its Random
 Forest is written in C++. In further texts, SMAC is representatively mentioned for SMAC3.
 
 > [Documentation](https://automl.github.io/SMAC3)
 
 > [Roadmap](https://github.com/orgs/automl/projects/5/views/2)
@@ -53,18 +53,18 @@
 ```
 
 Install SMAC via PyPI:
 ```
 pip install smac
 ```
 
-Or alternatively, clone the environment:
+If you want to contribute to SMAC, use the following steps instead:
 ```
 git clone https://github.com/automl/SMAC3.git && cd SMAC3
-pip install -e .[dev]
+make install-dev
 ```
 
 
 ## Minimal Example
 
 ```py
 from ConfigSpace import Configuration, ConfigurationSpace
@@ -92,28 +92,37 @@
 # Use SMAC to find the best configuration/hyperparameters
 smac = HyperparameterOptimizationFacade(scenario, train)
 incumbent = smac.optimize()
 ```
 
 More examples can be found in the [documentation](https://automl.github.io/SMAC3/main/examples/).
 
+## Visualization via DeepCAVE
+
+With DeepCAVE ([Repo](https://github.com/automl/DeepCAVE), [Paper](https://arxiv.org/abs/2206.03493)) you can visualize your SMAC runs. It is a visualization and analysis tool for AutoML (especially for the sub-problem
+hyperparameter optimization) runs.
 
 ## License
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the 3-clause BSD license (please see the LICENSE file).
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
 You should have received a copy of the 3-clause BSD license
 along with this program (see LICENSE file).
 If not, see [here](https://opensource.org/licenses/BSD-3-Clause).
 
+## Contacting us
+
+If you have trouble using SMAC, a concrete question or found a bug, please create an [issue](https://github.com/automl/SMAC3/issues). This is the easiest way to communicate about these things with us. 
+
+For all other inquiries, please write an email to smac[at]ai[dot]uni[dash]hannover[dot]de.
 
 ## Miscellaneous
 
 SMAC3 is developed by the [AutoML Groups of the Universities of Hannover and
 Freiburg](http://www.automl.org/).
 
 If you have found a bug, please report to [issues](https://github.com/automl/SMAC3/issues). Moreover, we are
```

### Comparing `smac-2.0.0b1/pyproject.toml` & `smac-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/setup.py` & `smac-2.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,20 @@
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=[
         "numpy>=1.23.3",
         "scipy>=1.9.2",
         "psutil",
         "pynisher>=1.0.0",
-        "ConfigSpace>=0.6.0",
+        "ConfigSpace>=0.6.1",
         "joblib",
         "scikit-learn>=1.1.2",
-        "pyrfr>=0.8.3",
+        "pyrfr>=0.9.0",
         "dask[distributed]",
+        "dask_jobqueue",
         "emcee>=3.0.0",
         "regex",
         "pyyaml",
     ],
     extras_require=extras_require,
     test_suite="pytest",
     platforms=["Linux"],
```

### Comparing `smac-2.0.0b1/smac/__init__.py` & `smac-2.0.1/smac/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,19 @@
     "Documentation": "https://https://github.com/automl.github.io/SMAC3/main",
     "Source Code": "https://github.com/https://github.com/automl/smac",
 }
 copyright = f"""
     Copyright {datetime.date.today().strftime('%Y')}, Marius Lindauer, Katharina Eggensperger,
     Matthias Feurer, André Biedenkapp, Difan Deng, Carolin Benjamins, Tim Ruhkopf, René Sass
     and Frank Hutter"""
-version = "2.0.0b1"
+version = "2.0.1"
 
 
 try:
-    from smac.utils.logging import setup_logging
-
-    setup_logging(0)
-
-    from smac.callback import Callback
+    from smac.callback.callback import Callback
     from smac.facade import (
         AlgorithmConfigurationFacade,
         BlackBoxFacade,
         HyperbandFacade,
         HyperparameterOptimizationFacade,
         MultiFidelityFacade,
         RandomFacade,
```

### Comparing `smac-2.0.0b1/smac/acquisition/function/__init__.py` & `smac-2.0.1/smac/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/abstract_acquisition_function.py` & `smac-2.0.1/smac/acquisition/function/abstract_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/confidence_bound.py` & `smac-2.0.1/smac/acquisition/function/confidence_bound.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/expected_improvement.py` & `smac-2.0.1/smac/acquisition/function/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/integrated_acquisition_function.py` & `smac-2.0.1/smac/acquisition/function/integrated_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/prior_acqusition_function.py` & `smac-2.0.1/smac/acquisition/function/prior_acqusition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/probability_improvement.py` & `smac-2.0.1/smac/acquisition/function/probability_improvement.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/function/thompson.py` & `smac-2.0.1/smac/acquisition/function/thompson.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/__init__.py` & `smac-2.0.1/smac/acquisition/maximizer/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/abstract_acqusition_maximizer.py` & `smac-2.0.1/smac/acquisition/maximizer/abstract_acqusition_maximizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     @acquisition_function.setter
     def acquisition_function(self, acquisition_function: AbstractAcquisitionFunction) -> None:
         self._acquisition_function = acquisition_function
 
     @property
     def meta(self) -> dict[str, Any]:
-        """Return the meta data of the created object."""
+        """Return the meta-data of the created object."""
         acquisition_function_meta = None
         if self._acquisition_function is not None:
             acquisition_function_meta = self._acquisition_function.meta
 
         return {
             "name": self.__class__.__name__,
             "acquisition_function": acquisition_function_meta,
@@ -81,29 +81,34 @@
         """Maximize acquisition function using `_maximize`, implemented by a subclass.
 
         Parameters
         ----------
         previous_configs: list[Configuration]
             Previous evaluated configurations.
         n_points: int, defaults to None
-            Number of points to be sampled. If `n_points` is not specified, `self._challengers` is used.
+            Number of points to be sampled. If `n_points` is not specified,
+            `self._challengers` is used.
         random_design: AbstractRandomDesign, defaults to None
-            Part of the returned ChallengerList such that we can interleave random configurations by a scheme defined by
-            the random design. The method `random_design.next_iteration()` is called at the end of this function.
+            Part of the returned ChallengerList such that we can interleave random configurations
+            by a scheme defined by the random design. The method `random_design.next_iteration()`
+            is called at the end of this function.
 
         Returns
         -------
         challengers : Iterator[Configuration]
             An iterable consisting of configurations.
         """
         if n_points is None:
             n_points = self._challengers
 
         def next_configs_by_acquisition_value() -> list[Configuration]:
             assert n_points is not None
+            # since maximize returns a tuple of acquisition value and configuration,
+            # and we only need the configuration, we return the second element of the tuple
+            # for each element in the list
             return [t[1] for t in self._maximize(previous_configs, n_points)]
 
         challengers = ChallengerList(
             self._configspace,
             next_configs_by_acquisition_value,
             random_design,
         )
```

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/differential_evolution.py` & `smac-2.0.1/smac/acquisition/maximizer/differential_evolution.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,27 @@
 from smac.acquisition.maximizer import AbstractAcquisitionMaximizer
 
 __copyright__ = "Copyright 2022, automl.org"
 __license__ = "3-clause BSD"
 
 
 class DifferentialEvolution(AbstractAcquisitionMaximizer):
-    """Get candidate solutions via `DifferentialEvolutionSolvers` from scipy."""
+    """Get candidate solutions via `DifferentialEvolutionSolvers` from scipy.
+
+    According to scipy 1.9.2 documentation:
+
+    'Finds the global minimum of a multivariate function.
+    Differential Evolution is stochastic in nature (does not use gradient methods) to find the minimum,
+    and can search large areas of candidate space, but often requires larger numbers of function
+    evaluations than conventional gradient-based techniques.
+    The algorithm is due to Storn and Price [1].'
+
+    [1] Storn, R and Price, K, Differential Evolution - a Simple and Efficient Heuristic for Global
+     Optimization over Continuous Spaces, Journal of Global Optimization, 1997, 11, 341 - 359.
+    """
 
     def _maximize(
         self,
         previous_configs: list[Configuration],
         n_points: int,
     ) -> list[tuple[float, Configuration]]:
 
@@ -42,14 +54,14 @@
             init="latinhypercube",
             atol=0,
         )
 
         _ = ds.solve()
         for pop, val in zip(ds.population, ds.population_energies):
             rc = Configuration(self._configspace, vector=pop)
-            rc.origin = "Differential Evolution"
+            rc.origin = "Acquisition Function Maximizer: Differential Evolution"
             configs.append((-val, rc))
 
         configs.sort(key=lambda t: t[0])
         configs.reverse()
 
         return configs
```

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/helpers.py` & `smac-2.0.1/smac/acquisition/maximizer/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     in each iteration which are never looked at.
 
     Parameters
     ----------
     configspace : ConfigurationSpace
     challenger_callback : Callable
         Callback function which returns a list of challengers (without interleaved random configurations, must a be a
-        closure: https://www.programiz.com/python-programming/closure)
+        python closure.
     random_design : AbstractRandomDesign | None, defaults to ModulusRandomDesign(modulus=2.0)
         Which random design should be used.
     """
 
     def __init__(
         self,
         configspace: ConfigurationSpace,
```

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/local_and_random_search.py` & `smac-2.0.1/smac/acquisition/maximizer/local_and_random_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,20 @@
 
 logger = get_logger(__name__)
 
 
 class LocalAndSortedRandomSearch(AbstractAcquisitionMaximizer):
     """Implement SMAC's default acquisition function optimization.
 
-    This optimizer performs local search from the previous best points according, to the acquisition function, uses the
-    acquisition function to sort randomly sampled configurations. Random configurations are interleaved by the main SMAC
-    code.
+    This optimizer performs local search from the previous best points according, to the acquisition
+    function, uses the acquisition function to sort randomly sampled configurations.
+    Random configurations are interleaved by the main SMAC code.
+
+    The Random configurations are interleaved to circumvent issues from a constant prediction
+    from the Random Forest model at the beginning of the optimization process.
 
     Parameters
     ----------
     configspace : ConfigurationSpace
     acquisition_function : AbstractAcquisitionFunction | None, defaults to None
     challengers : int, defaults to 5000
         Number of challengers.
```

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/local_search.py` & `smac-2.0.1/smac/acquisition/maximizer/local_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,18 +86,23 @@
 
     def _maximize(
         self,
         previous_configs: list[Configuration],
         n_points: int,
         additional_start_points: list[tuple[float, Configuration]] | None = None,
     ) -> list[tuple[float, Configuration]]:
-        """Start a local search from the given startpoint.
+        """Start a local search from the given startpoints. Iteratively collect neighbours
+        using Configspace.utils.get_one_exchange_neighbourhood and evaluate them.
+        If the new config is better than the current best, the local search is coninued from the
+        new config.
 
         Quit if either the max number of steps is reached or
-        no neighbor with an higher improvement was found.
+        no neighbor with a higher improvement was found or the number of local steps self._n_steps_plateau_walk
+        for each of the starting point is depleted.
+
 
         Parameters
         ----------
         previous_configs : list[Configuration]
             Previous configuration (e.g., from the runhistory).
         n_points : int
             Number of initial points to be generated.
@@ -114,15 +119,15 @@
 
         # Shuffle for random tie-break
         self._rng.shuffle(configs_acq)
 
         # Sort according to acq value
         configs_acq.sort(reverse=True, key=lambda x: x[0])
         for a, inc in configs_acq:
-            inc.origin = "Local Search"
+            inc.origin = "Acquisition Function Maximizer: Local Search"
 
         return configs_acq
 
     def _get_initial_points(
         self,
         previous_configs: list[Configuration],
         n_points: int,
@@ -161,15 +166,25 @@
         n_points: int,
         additional_start_points: list[tuple[float, Configuration]] | None,
     ) -> list[Configuration]:
         """
         Generate a set of initial points from the previous configurations and possibly additional points.
 
         The idea is to decouple runhistory from the local search model and replace it with a more general
-        form (list[Configuration]).
+        form (list[Configuration]). This is useful to more quickly collect new configurations
+        along the iterations, rather than feeding it to the runhistory every time.
+
+        create three lists and concatenate them:
+        1. sorted the previous configs by acquisition value
+        2. sorted the previous configs by marginal predictive costs
+        3. additional start points
+
+        and create a list that carries unique configurations only. Crucially,
+        when reading from left to right, all but the first occurrence of a configuration
+        are dropped.
 
         Parameters
         ----------
         previous_configs: list[Configuration]
             Previous configuration (e.g., from the runhistory).
         n_points: int
             Number of initial points to be generated.
@@ -197,20 +212,18 @@
             # (for example multi-objective or EIPS) it is not immediately clear how to sort according to the cost
             # of a configuration. Therefore, we simply follow the ParEGO approach and use a random scalarization.
             if len(costs.shape) == 2 and costs.shape[1] > 1:
                 weights = np.array([self._rng.rand() for _ in range(costs.shape[1])])
                 weights = weights / np.sum(weights)
                 costs = costs @ weights
 
-            # From here
+            # From here: make argsort result to be random between equal values
             # http://stackoverflow.com/questions/20197990/how-to-make-argsort-result-to-be-random-between-equal-values
             random = self._rng.rand(len(costs))
-
-            # Last column is primary sort key!
-            indices = np.lexsort((random.flatten(), costs.flatten()))
+            indices = np.lexsort((random.flatten(), costs.flatten()))  # Last column is primary sort key!
 
             # Cannot use zip here because the indices array cannot index the
             # rand_configs list, because the second is a pure python list
             previous_configs_sorted_by_cost = [previous_configs[ind] for ind in indices][:n_points]
         else:
             previous_configs_sorted_by_cost = []
 
@@ -234,14 +247,29 @@
 
     def _search(
         self,
         start_points: list[Configuration],
     ) -> list[tuple[float, Configuration]]:
         """Optimize the acquisition function.
 
+        Execution:
+        1. Neighbour generation strategy for each of the starting points is according to
+        ConfigSpace.utils.get_one_exchange_neighbourhood.
+        2. Each of the starting points create a local search, that can be active.
+        if it is active, request a neighbour of its neightbourhood and evaluate it.
+        3. Comparing the acquisition function of the neighbors with the acquisition value of the
+        candidate.
+        If it improved, then the candidate is replaced by the neighbor. And this candidate is
+        investigated again with two new neighbours.
+        If it did not improve, it is investigated with twice as many new neighbours
+        (at most self._vectorization_max_obtain neighbours).
+        The local search for a starting point is stopped if the number of evaluations is larger
+        than self._n_steps_plateau_walk.
+
+
         Parameters
         ----------
         start_points : list[Configuration]
             Starting points for the search.
 
         Returns
         -------
@@ -282,14 +310,23 @@
         # Tracking the time it takes to compute the acquisition function
         times = []
 
         # Set up the neighborhood generators
         neighborhood_iterators = []
         for i, inc in enumerate(candidates):
             neighborhood_iterators.append(
+                # get_one_exchange_neighbourhood implementational details:
+                # https://github.com/automl/ConfigSpace/blob/05ab3da2a06c084ba920e8e4e3f62f2e87e81442/ConfigSpace/util.pyx#L95
+                # Return all configurations in a one-exchange neighborhood.
+                #
+                #     The method is implemented as defined by:
+                #     Frank Hutter, Holger H. Hoos and Kevin Leyton-Brown
+                #     Sequential Model-Based Optimization for General Algorithm Configuration
+                #     In Proceedings of the conference on Learning and Intelligent
+                #     Optimization(LION 5)
                 get_one_exchange_neighbourhood(inc, seed=self._rng.randint(low=0, high=100000))
             )
             local_search_steps[i] += 1
 
         # Keeping track of configurations with equal acquisition value for plateau walking
         neighbors_w_equal_acq: list[list[Configuration]] = [[] for _ in range(num_candidates)]
```

### Comparing `smac-2.0.0b1/smac/acquisition/maximizer/random_search.py` & `smac-2.0.1/smac/acquisition/maximizer/random_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         if n_points > 1:
             rand_configs = self._configspace.sample_configuration(size=n_points)
         else:
             rand_configs = [self._configspace.sample_configuration(size=1)]
 
         if _sorted:
             for i in range(len(rand_configs)):
-                rand_configs[i].origin = "Random Search (sorted)"
+                rand_configs[i].origin = "Acquisition Function Maximizer: Random Search (sorted)"
 
             return self._sort_by_acquisition_value(rand_configs)
         else:
             for i in range(len(rand_configs)):
-                rand_configs[i].origin = "Random Search"
+                rand_configs[i].origin = "Acquisition Function Maximizer: Random Search"
 
             return [(0, rand_configs[i]) for i in range(len(rand_configs))]
```

### Comparing `smac-2.0.0b1/smac/callback.py` & `smac-2.0.1/smac/callback/callback.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/facade/__init__.py` & `smac-2.0.1/smac/facade/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/facade/abstract_facade.py` & `smac-2.0.1/smac/facade/abstract_facade.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from abc import abstractmethod
 from typing import Any, Callable
 
 from pathlib import Path
 
 import joblib
 from ConfigSpace import Configuration
+from dask.distributed import Client
+from typing_extensions import Literal
 
 import smac
 from smac.acquisition.function.abstract_acquisition_function import (
     AbstractAcquisitionFunction,
 )
 from smac.acquisition.maximizer.abstract_acqusition_maximizer import (
     AbstractAcquisitionMaximizer,
 )
-from smac.callback import Callback
+from smac.callback.callback import Callback
 from smac.initial_design.abstract_initial_design import AbstractInitialDesign
 from smac.intensifier.abstract_intensifier import AbstractIntensifier
 from smac.main.config_selector import ConfigSelector
 from smac.main.smbo import SMBO
 from smac.model.abstract_model import AbstractModel
 from smac.multi_objective.abstract_multi_objective_algorithm import (
     AbstractMultiObjectiveAlgorithm,
@@ -77,23 +79,29 @@
     multi_objective_algorithm : AbstractMultiObjectiveAlgorithm | None, defaults to None
         In case of multiple objectives, the objectives need to be interpreted so that an optimization is possible.
         The multi-objective algorithm takes care of that.
     runhistory_encoder : RunHistoryEncoder | None, defaults to None
         Based on the runhistory, the surrogate model is trained. However, the data first needs to be encoded, which
         is done by the runhistory encoder. For example, inactive hyperparameters need to be encoded or cost values
         can be log transformed.
-    logging_level: int | Path | None
+    logging_level: int | Path | Literal[False] | None
         The level of logging (the lowest level 0 indicates the debug level). If a path is passed, a yaml file is
         expected with the logging configuration. If nothing is passed, the default logging.yml from SMAC is used.
+        If False is passed, SMAC will not do any customization of the logging setup and the responsibility is left
+        to the user.
     callbacks: list[Callback], defaults to []
         Callbacks, which are incorporated into the optimization loop.
     overwrite: bool, defaults to False
         When True, overwrites the run results if a previous run is found that is
         inconsistent in the meta data with the current setup. If ``overwrite`` is set to False, the user is asked
         for the exact behaviour (overwrite completely, save old run, or use old results).
+    dask_client: Client | None, defaults to None
+        User-created dask client, which can be used to start a dask cluster and then attach SMAC to it. This will not
+        be closed automatically and will have to be closed manually if provided explicitly. If none is provided
+        (default), a local one will be created for you and closed upon completion.
     """
 
     def __init__(
         self,
         scenario: Scenario,
         target_function: Callable | str | AbstractRunner,
         *,
@@ -102,17 +110,18 @@
         acquisition_maximizer: AbstractAcquisitionMaximizer | None = None,
         initial_design: AbstractInitialDesign | None = None,
         random_design: AbstractRandomDesign | None = None,
         intensifier: AbstractIntensifier | None = None,
         multi_objective_algorithm: AbstractMultiObjectiveAlgorithm | None = None,
         runhistory_encoder: AbstractRunHistoryEncoder | None = None,
         config_selector: ConfigSelector | None = None,
-        logging_level: int | Path | None = None,
+        logging_level: int | Path | Literal[False] | None = None,
         callbacks: list[Callback] = [],
         overwrite: bool = False,
+        dask_client: Client | None = None,
     ):
         setup_logging(logging_level)
 
         if model is None:
             model = self.get_model(scenario)
 
         if acquisition_function is None:
@@ -174,22 +183,27 @@
             runner = TargetFunctionRunner(
                 scenario=scenario,
                 target_function=target_function,
                 required_arguments=self._get_signature_arguments(),
             )
 
         # In case of multiple jobs, we need to wrap the runner again using DaskParallelRunner
-        if (n_workers := scenario.n_workers) > 1:
-            available_workers = joblib.cpu_count()
-            if n_workers > available_workers:
-                logger.info(f"Workers are reduced to {n_workers}.")
-                n_workers = available_workers
+        if (n_workers := scenario.n_workers) > 1 or dask_client is not None:
+            if dask_client is not None:
+                logger.warning(
+                    "Provided `dask_client`. Ignore `scenario.n_workers`, directly set `n_workers` in `dask_client`."
+                )
+            else:
+                available_workers = joblib.cpu_count()
+                if n_workers > available_workers:
+                    logger.info(f"Workers are reduced to {n_workers}.")
+                    n_workers = available_workers
 
             # We use a dask runner for parallelization
-            runner = DaskParallelRunner(single_worker=runner)
+            runner = DaskParallelRunner(single_worker=runner, dask_client=dask_client)
 
         # Set the runner to access it globally
         self._runner = runner
 
         # Adding dependencies of the components
         self._update_dependencies()
 
@@ -201,19 +215,19 @@
 
         # Finally we configure our optimizer
         self._optimizer = self._get_optimizer()
         assert self._optimizer
 
         # Register callbacks here
         for callback in callbacks:
-            self._optimizer._register_callback(callback)
+            self._optimizer.register_callback(callback)
 
         # Additionally, we register the runhistory callback from the intensifier to efficiently update our incumbent
         # every time new information are available
-        self._optimizer._register_callback(self._intensifier.get_callback())
+        self._optimizer.register_callback(self._intensifier.get_callback(), index=0)
 
     @property
     def scenario(self) -> Scenario:
         """The scenario object which holds all environment information."""
         return self._scenario
 
     @property
@@ -271,26 +285,37 @@
         value: TrialValue
             Contains relevant information regarding the execution of a trial.
         save : bool, optional to True
             Whether the runhistory should be saved.
         """
         return self._optimizer.tell(info, value, save=save)
 
-    def optimize(self) -> Configuration | list[Configuration]:
+    def optimize(self, *, data_to_scatter: dict[str, Any] | None = None) -> Configuration | list[Configuration]:
         """
         Optimizes the configuration of the algorithm.
 
+        Parameters
+        ----------
+        data_to_scatter: dict[str, Any] | None
+            We first note that this argument is valid only dask_runner!
+            When a user scatters data from their local process to the distributed network,
+            this data is distributed in a round-robin fashion grouping by number of cores.
+            Roughly speaking, we can keep this data in memory and then we do not have to (de-)serialize the data
+            every time we would like to execute a target function with a big dataset.
+            For example, when your target function has a big dataset shared across all the target function,
+            this argument is very useful.
+
         Returns
         -------
         incumbent : Configuration
             Best found configuration.
         """
         incumbents = None
         try:
-            incumbents = self._optimizer.optimize()
+            incumbents = self._optimizer.optimize(data_to_scatter=data_to_scatter)
         finally:
             self._optimizer.save()
 
         return incumbents
 
     def validate(
         self,
```

### Comparing `smac-2.0.0b1/smac/facade/algorithm_configuration_facade.py` & `smac-2.0.1/smac/facade/algorithm_configuration_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/facade/blackbox_facade.py` & `smac-2.0.1/smac/facade/blackbox_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/facade/hyperband_facade.py` & `smac-2.0.1/smac/facade/hyperband_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/facade/hyperparameter_optimization_facade.py` & `smac-2.0.1/smac/facade/hyperparameter_optimization_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/facade/multi_fidelity_facade.py` & `smac-2.0.1/smac/facade/multi_fidelity_facade.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,21 @@
             * None: No shuffling at all and use the instance-seed order provided by the user.
             * "shuffle_once": Shuffle the instance-seed keys once and use the same order across all runs.
             * "shuffle": Shuffles the instance-seed keys for each bracket individually.
         incumbent_selection : str, defaults to "any_budget"
             How to select the incumbent when using budgets. Can be set to:
             * "any_budget": Incumbent is the best on any budget, i.e., the best performance regardless of budget.
             * "highest_observed_budget": Incumbent is the best in the highest budget run so far.
-            * "highest_budget": Incumbent is selected only based on the highest budget.
+            refer to `runhistory.get_trials` for more details. Crucially, if true, then a
+            for a given config-instance-seed, only the highest (so far executed) budget is used for
+            comparison against the incumbent. Notice, that if the highest observed budget is smaller
+            than the highest budget of the incumbent, the configuration will be queued again to
+            be intensified again.
+            * "highest_budget": Incumbent is selected only based on the absolute highest budget
+            available only.
         max_incumbents : int, defaults to 10
             How many incumbents to keep track of in the case of multi-objective.
         """
         return Hyperband(
             scenario=scenario,
             eta=eta,
             n_seeds=n_seeds,
```

### Comparing `smac-2.0.0b1/smac/facade/random_facade.py` & `smac-2.0.1/smac/facade/random_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/initial_design/__init__.py` & `smac-2.0.1/smac/initial_design/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/initial_design/abstract_initial_design.py` & `smac-2.0.1/smac/initial_design/abstract_initial_design.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import OrderedDict
 
 import numpy as np
 from ConfigSpace.configuration_space import Configuration, ConfigurationSpace
 from ConfigSpace.hyperparameters import (
     CategoricalHyperparameter,
     Constant,
+    IntegerHyperparameter,
     NumericalHyperparameter,
     OrdinalHyperparameter,
 )
 from ConfigSpace.util import ForbiddenValueError, deactivate_inactive_hyperparameters
 
 from smac.scenario import Scenario
 from smac.utils.logging import get_logger
@@ -46,25 +47,38 @@
 
     def __init__(
         self,
         scenario: Scenario,
         n_configs: int | None = None,
         n_configs_per_hyperparameter: int | None = 10,
         max_ratio: float = 0.25,
-        additional_configs: list[Configuration] = [],
+        additional_configs: list[Configuration] = None,
         seed: int | None = None,
     ):
         self._configspace = scenario.configspace
 
         if seed is None:
             seed = scenario.seed
 
+        self.use_default_config = scenario.use_default_config
+
         self._seed = seed
         self._rng = np.random.RandomState(seed)
         self._n_configs_per_hyperparameter = n_configs_per_hyperparameter
+
+        # make sure that additional configs is not a mutable default value
+        # this avoids issues
+        if additional_configs is None:
+            additional_configs = []
+
+        if self.use_default_config:
+            default_config = self._configspace.get_default_configuration()
+            default_config.origin = "Initial Design: Default configuration"
+            additional_configs.append(default_config)
+
         self._additional_configs = additional_configs
 
         n_params = len(self._configspace.get_hyperparameters())
         if n_configs is not None:
             logger.info("Using `n_configs` and ignoring `n_configs_per_hyperparameter`.")
             self._n_configs = n_configs
         elif n_configs_per_hyperparameter is not None:
@@ -158,15 +172,18 @@
         Returns
         -------
         configs : list[Configuration]
             Continuous transformed configs.
         """
         params = configspace.get_hyperparameters()
         for idx, param in enumerate(params):
-            if isinstance(param, NumericalHyperparameter):
+
+            if isinstance(param, IntegerHyperparameter):
+                design[:, idx] = param._inverse_transform(param._transform(design[:, idx]))
+            elif isinstance(param, NumericalHyperparameter):
                 continue
             elif isinstance(param, Constant):
                 design_ = np.zeros(np.array(design.shape) + np.array((0, 1)))
                 design_[:, :idx] = design[:, :idx]
                 design_[:, idx + 1 :] = design[:, idx:]
                 design = design_
             elif isinstance(param, CategoricalHyperparameter):
@@ -174,15 +191,15 @@
                 v_design[v_design == 1] = 1 - 10**-10
                 design[:, idx] = np.array(v_design * len(param.choices), dtype=int)
             elif isinstance(param, OrdinalHyperparameter):
                 v_design = design[:, idx]
                 v_design[v_design == 1] = 1 - 10**-10
                 design[:, idx] = np.array(v_design * len(param.sequence), dtype=int)
             else:
-                raise ValueError("Hyperparameter not supported in LHD.")
+                raise ValueError("Hyperparameter not supported when transforming a continuous design.")
 
         configs = []
         for vector in design:
             try:
                 conf = deactivate_inactive_hyperparameters(
                     configuration=None, configuration_space=configspace, vector=vector
                 )
```

### Comparing `smac-2.0.0b1/smac/initial_design/default_design.py` & `smac-2.0.1/smac/initial_design/default_design.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 
 class DefaultInitialDesign(AbstractInitialDesign):
     """Initial design that evaluates only the default configuration."""
 
     def _select_configurations(self) -> list[Configuration]:
         config = self._configspace.get_default_configuration()
-        config.origin = "Default"
+        config.origin = "Initial Design: Default"
         return [config]
```

### Comparing `smac-2.0.0b1/smac/initial_design/factorial_design.py` & `smac-2.0.1/smac/initial_design/factorial_design.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,11 +51,11 @@
         middle_conf = deactivate_inactive_hyperparameters(conf_dict, self._configspace)
         configs.append(middle_conf)
 
         # Add corner points
         for design in factorial_design:
             conf_dict = dict([(p.name, v) for p, v in zip(params, design)])
             conf = deactivate_inactive_hyperparameters(conf_dict, self._configspace)
-            conf.origin = "Factorial Initial Design"
+            conf.origin = "Initial Design: Factorial"
             configs.append(conf)
 
         return configs
```

### Comparing `smac-2.0.0b1/smac/initial_design/latin_hypercube_design.py` & `smac-2.0.1/smac/initial_design/latin_hypercube_design.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,9 +22,9 @@
         for p in params:
             if isinstance(p, Constant):
                 constants += 1
 
         lhd = LatinHypercube(d=len(params) - constants, seed=self._rng.randint(0, 1000000)).random(n=self._n_configs)
 
         return self._transform_continuous_designs(
-            design=lhd, origin="Latin Hypercube Initial Design", configspace=self._configspace
+            design=lhd, origin="Initial Design: Latin Hypercube", configspace=self._configspace
         )
```

### Comparing `smac-2.0.0b1/smac/initial_design/random_design.py` & `smac-2.0.1/smac/initial_design/random_design.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """Initial design that evaluates random configurations."""
 
     def _select_configurations(self) -> list[Configuration]:
         configs = self._configspace.sample_configuration(size=self._n_configs)
         if self._n_configs == 1:
             configs = [configs]
         for config in configs:
-            config.origin = "Random Initial Design"
+            config.origin = "Initial Design: Random"
         return configs
```

### Comparing `smac-2.0.0b1/smac/initial_design/sobol_design.py` & `smac-2.0.1/smac/initial_design/sobol_design.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,9 +40,9 @@
         sobol_gen = Sobol(d=dim, scramble=True, seed=self._rng.randint(low=0, high=10000000))
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             sobol = sobol_gen.random(self._n_configs)
 
         return self._transform_continuous_designs(
-            design=sobol, origin="Sobol Initial Design", configspace=self._configspace
+            design=sobol, origin="Initial Design: Sobol", configspace=self._configspace
         )
```

### Comparing `smac-2.0.0b1/smac/intensifier/abstract_intensifier.py` & `smac-2.0.1/smac/intensifier/abstract_intensifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from collections import defaultdict
 from pathlib import Path
 
 import numpy as np
 from ConfigSpace import Configuration
 
 import smac
-from smac.callback import Callback
+from smac.callback.callback import Callback
 from smac.constants import MAXINT
 from smac.main.config_selector import ConfigSelector
 from smac.runhistory import TrialInfo
 from smac.runhistory.dataclasses import (
     InstanceSeedBudgetKey,
     InstanceSeedKey,
     TrajectoryItem,
@@ -267,21 +267,20 @@
             if validate:
                 rng = np.random.RandomState(seed)
             else:
                 rng = self._rng
 
             i = 0
             while True:
-                # We have two conditions to stop the loop:
-                # A) We found enough configs
-                # B) We used enough seeds
-                A = self._max_config_calls is not None and len(instance_seed_keys) >= self._max_config_calls
-                B = self._n_seeds is not None and i >= self._n_seeds
+                found_enough_configs = (
+                    self._max_config_calls is not None and len(instance_seed_keys) >= self._max_config_calls
+                )
+                used_enough_seeds = self._n_seeds is not None and i >= self._n_seeds
 
-                if A or B:
+                if found_enough_configs or used_enough_seeds:
                     break
 
                 if validate:
                     next_seed = int(rng.randint(low=0, high=MAXINT, size=1)[0])
                 else:
                     try:
                         next_seed = self._tf_seeds[i]
@@ -415,15 +414,18 @@
         if len(incumbents) > 0:
             # We want to calculate the differences so that we can evaluate the other incumbents on the same instances
             incumbent_isb_keys = [self.get_instance_seed_budget_keys(incumbent, compare) for incumbent in incumbents]
 
             if len(incumbent_isb_keys) <= 1:
                 return []
 
-            incumbent_isb_keys = list(set.difference(*map(set, incumbent_isb_keys)))  # type: ignore
+            # Compute the actual differences
+            intersection_isb_keys = set.intersection(*map(set, incumbent_isb_keys))  # type: ignore
+            union_isb_keys = set.union(*map(set, incumbent_isb_keys))  # type: ignore
+            incumbent_isb_keys = list(union_isb_keys - intersection_isb_keys)  # type: ignore
 
             if len(incumbent_isb_keys) == 0:
                 return []
 
             return incumbent_isb_keys  # type: ignore
 
         return []
@@ -451,14 +453,33 @@
 
         return RunHistoryCallback(self)
 
     def update_incumbents(self, config: Configuration) -> None:
         """Updates the incumbents. This method is called everytime a trial is added to the runhistory. Since only
         the affected config and the current incumbents are used, this method is very efficient. Furthermore, a
         configuration is only considered incumbent if it has a better performance on all incumbent instances.
+
+        Crucially, if there is no incumbent (at the start) then, the first configuration assumes
+        incumbent status. For the next configuration, we need to check if the configuration
+        is better on all instances that have been evaluated for the incumbent. If this is the
+        case, then we can replace the incumbent. Otherwise, a) we need to requeue the config to
+        obtain the missing instance-seed-budget combination or b) mark this configuration as
+        inferior ("rejected") to not consider it again. The comparison behaviour is controlled by
+        self.get_instance_seed_budget_keys() and self.get_incumbent_instance_seed_budget_keys().
+
+        Notably, this method is written to support both multi-fidelity and multi-objective
+        optimization. While the get_instance_seed_budget_keys() method and
+        self.get_incumbent_instance_seed_budget_keys() are used for the multi-fidelity behaviour,
+        calculate_pareto_front() is used as a hard coded way to support multi-objective
+        optimization, including the single objective as special case. calculate_pareto_front()
+        is called on the set of all (in case of MO) incumbents amended with the challenger
+        configuration, provided it has a sufficient overlap in seed-instance-budget combinations.
+
+        Lastly, if we have a self._max_incumbents and the pareto front provides more than this
+        specified amount, we cut the incumbents using crowding distance.
         """
         rh = self.runhistory
 
         # What happens if a config was rejected, but it appears again? Give it another try even if it
         # has already been evaluated? Yes!
 
         # Associated trials and id
@@ -472,14 +493,15 @@
         if len(config_isb_keys) == 0:
             logger.debug(f"No relevant instances evaluated for config {config_hash}. Updating incumbents is skipped.")
             return
 
         # Now we get the incumbents and see which trials have been used
         incumbents = self.get_incumbents()
         incumbent_ids = [rh.get_config_id(c) for c in incumbents]
+        # Find the lowest intersection of instance-seed-budget keys for all incumbents.
         incumbent_isb_keys = self.get_incumbent_instance_seed_budget_keys()
 
         # Save for later
         previous_incumbents = incumbents.copy()
         previous_incumbent_ids = incumbent_ids.copy()
 
         # Little sanity check here for consistency
@@ -502,15 +524,18 @@
         # 1) Any budget/highest observed budget: We want to get rid of the budgets because if we know it is calculated
         # on the same instance-seed already then we are ready to go. Imagine we would check for the same budgets,
         # then the configs can not be compared although the user does not care on which budgets configurations have
         # been evaluated.
         # 2) Highest budget: We only want to compare the configs if they are evaluated on the highest budget.
         # Here we do actually care about the budgets. Please see the ``get_instance_seed_budget_keys`` method from
         # Successive Halving to get more information.
+        # Noitce: compare=True only takes effect when subclass implemented it. -- e.g. in SH it
+        # will remove the budgets from the keys.
         config_isb_comparison_keys = self.get_instance_seed_budget_keys(config, compare=True)
+        # Find the lowest intersection of instance-seed-budget keys for all incumbents.
         config_incumbent_isb_comparison_keys = self.get_incumbent_instance_seed_budget_keys(compare=True)
 
         # Now we have to check if the new config has been evaluated on the same keys as the incumbents
         if not all([key in config_isb_comparison_keys for key in config_incumbent_isb_comparison_keys]):
             # We can not tell if the new config is better/worse than the incumbents because it has not been
             # evaluated on the necessary trials
             logger.debug(
```

### Comparing `smac-2.0.0b1/smac/intensifier/hyperband.py` & `smac-2.0.1/smac/intensifier/hyperband.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 from typing import Any
 
-import numpy as np
-
 from smac.intensifier.successive_halving import SuccessiveHalving
 
 
 class Hyperband(SuccessiveHalving):
     """See ``SuccessiveHalving`` for documentation."""
 
     def reset(self) -> None:
@@ -18,44 +16,30 @@
         self._next_bracket: int = 0
 
     def __post_init__(self) -> None:
         super().__post_init__()
 
         min_budget = self._min_budget
         max_budget = self._max_budget
+        assert min_budget is not None and max_budget is not None
         eta = self._eta
 
         # The only difference we have to do is change max_iterations, n_configs_in_stage, budgets_in_stage
-        s_max = int(np.floor(np.log(max_budget / min_budget) / np.log(eta)))
-
-        max_iterations: dict[int, int] = {}
-        n_configs_in_stage: dict[int, list] = {}
-        budgets_in_stage: dict[int, list] = {}
-
-        for i in range(s_max + 1):
-            max_iter = s_max - i
-            n_initial_challengers = int(eta**max_iter)
-
-            # How many configs in each stage
-            linspace = -np.linspace(0, max_iter, max_iter + 1)
-            n_configs_ = n_initial_challengers * np.power(eta, linspace)
-            n_configs = np.array(np.round(n_configs_), dtype=int).tolist()
-
-            # How many budgets in each stage
-            linspace = -np.linspace(max_iter, 0, max_iter + 1)
-            budgets = (max_budget * np.power(eta, linspace)).tolist()
-
-            max_iterations[i] = max_iter + 1
-            n_configs_in_stage[i] = n_configs
-            budgets_in_stage[i] = budgets
-
-        self._s_max = s_max
-        self._max_iterations = max_iterations
-        self._n_configs_in_stage = n_configs_in_stage
-        self._budgets_in_stage = budgets_in_stage
+        self._s_max = self._get_max_iterations(eta, max_budget, min_budget)  # type: ignore[operator]
+        self._max_iterations: dict[int, int] = {}
+        self._n_configs_in_stage: dict[int, list] = {}
+        self._budgets_in_stage: dict[int, list] = {}
+
+        for i in range(self._s_max + 1):
+            max_iter = self._s_max - i
+
+            self._budgets_in_stage[i], self._n_configs_in_stage[i] = self._compute_configs_and_budgets_for_stages(
+                eta, max_budget, max_iter, self._s_max
+            )
+            self._max_iterations[i] = max_iter + 1
 
     def get_state(self) -> dict[str, Any]:  # noqa: D102
         state = super().get_state()
         state["next_bracket"] = self._next_bracket
 
         return state
```

### Comparing `smac-2.0.0b1/smac/intensifier/intensifier.py` & `smac-2.0.1/smac/intensifier/intensifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,19 @@
         if self._scenario.instances is None:
             return False
 
         return True
 
     def get_state(self) -> dict[str, Any]:  # noqa: D102
         return {
-            "queue": [(self.runhistory.get_config_id(config), n) for config, n in self._queue],
+            "queue": [
+                (self.runhistory.get_config_id(config), n)
+                for config, n in self._queue
+                if self.runhistory.has_config(config)
+            ],
         }
 
     def set_state(self, state: dict[str, Any]) -> None:  # noqa: D102
         self._queue = [(self.runhistory.get_config(id), n) for id, n in state["queue"]]
 
     def __iter__(self) -> Iterator[TrialInfo]:
         """This iter method holds the logic for the intensification loop.
```

### Comparing `smac-2.0.0b1/smac/intensifier/successive_halving.py` & `smac-2.0.1/smac/intensifier/successive_halving.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Iterator
 
+import math
 from collections import defaultdict
 
 import numpy as np
 from ConfigSpace import Configuration
 
 from smac.constants import MAXINT
 from smac.intensifier.abstract_intensifier import AbstractIntensifier
@@ -86,14 +87,18 @@
         )
 
         self._eta = eta
         self._instance_seed_order = instance_seed_order
         self._incumbent_selection = incumbent_selection
         self._highest_observed_budget_only = False if incumbent_selection == "any_budget" else True
 
+        # Global variables derived from scenario
+        self._min_budget = self._scenario.min_budget
+        self._max_budget = self._scenario.max_budget
+
     @property
     def meta(self) -> dict[str, Any]:  # noqa: D102
         meta = super().meta
         meta.update(
             {
                 "eta": self._eta,
                 "instance_seed_order": self._instance_seed_order,
@@ -116,16 +121,16 @@
         super().__post_init__()
 
         # We generate our instance seed pairs once
         is_keys = self.get_instance_seed_keys_of_interest()
 
         # Budgets, followed by lots of sanity-checking
         eta = self._eta
-        min_budget = self._scenario.min_budget
-        max_budget = self._scenario.max_budget
+        min_budget = self._min_budget
+        max_budget = self._max_budget
 
         if max_budget is not None and min_budget is not None and max_budget < min_budget:
             raise ValueError("Max budget has to be larger than min budget.")
 
         if self.uses_instances:
             if isinstance(min_budget, float) or isinstance(max_budget, float):
                 raise ValueError("Successive Halving requires integer budgets when using instances.")
@@ -158,35 +163,50 @@
         budget_type = "INSTANCES" if self.uses_instances else "BUDGETS"
         logger.info(
             f"Successive Halving uses budget type {budget_type} with eta {eta}, "
             f"min budget {min_budget}, and max budget {max_budget}."
         )
 
         # Pre-computing Successive Halving variables
-        max_iter = int(np.floor(np.log(max_budget / min_budget) / np.log(eta)))
-        n_initial_challengers = int(eta**max_iter)
-
-        # How many configs in each stage
-        linspace = -np.linspace(0, max_iter, max_iter + 1)
-        n_configs_ = n_initial_challengers * np.power(eta, linspace)
-        n_configs = np.array(np.round(n_configs_), dtype=int).tolist()
-
-        # How many budgets in each stage
-        linspace = -np.linspace(max_iter, 0, max_iter + 1)
-        budgets = (max_budget * np.power(eta, linspace)).tolist()
+        max_iter = self._get_max_iterations(eta, max_budget, min_budget)
+        budgets, n_configs = self._compute_configs_and_budgets_for_stages(eta, max_budget, max_iter)
 
         # Global variables
         self._min_budget = min_budget
         self._max_budget = max_budget
 
         # Stage variables, depending on the bracket (0 is the bracket here since SH only has one bracket)
         self._max_iterations: dict[int, int] = {0: max_iter + 1}
         self._n_configs_in_stage: dict[int, list] = {0: n_configs}
         self._budgets_in_stage: dict[int, list] = {0: budgets}
 
+    @staticmethod
+    def _get_max_iterations(eta: int, max_budget: float | int, min_budget: float | int) -> int:
+        return int(np.floor(np.log(max_budget / min_budget) / np.log(eta)))
+
+    @staticmethod
+    def _compute_configs_and_budgets_for_stages(
+        eta: int, max_budget: float | int, max_iter: int, s_max: int | None = None
+    ) -> tuple[list[int], list[int]]:
+        if s_max is None:
+            s_max = max_iter
+
+        n_initial_challengers = math.ceil((eta**max_iter) * (s_max + 1) / (max_iter + 1))
+
+        # How many configs in each stage
+        lin_space = -np.linspace(0, max_iter, max_iter + 1)
+        n_configs_ = np.floor(n_initial_challengers * np.power(eta, lin_space))
+        n_configs = np.array(np.round(n_configs_), dtype=int).tolist()
+
+        # How many budgets in each stage
+        lin_space = -np.linspace(max_iter, 0, max_iter + 1)
+        budgets = (max_budget * np.power(eta, lin_space)).tolist()
+
+        return budgets, n_configs
+
     def get_state(self) -> dict[str, Any]:  # noqa: D102
         # Replace config by dict
         tracker: dict[str, list[tuple[int | None, list[dict]]]] = defaultdict(list)
         for key in list(self._tracker.keys()):
             for seed, configs in self._tracker[key]:
                 # We have to make key serializable
                 new_key = f"{key[0]},{key[1]}"
```

### Comparing `smac-2.0.0b1/smac/logging.yml` & `smac-2.0.1/smac/logging.yml`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/main/config_selector.py` & `smac-2.0.1/smac/main/config_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from smac.acquisition.function.abstract_acquisition_function import (
     AbstractAcquisitionFunction,
 )
 from smac.acquisition.maximizer.abstract_acqusition_maximizer import (
     AbstractAcquisitionMaximizer,
 )
-from smac.callback import Callback
+from smac.callback.callback import Callback
 from smac.initial_design import AbstractInitialDesign
 from smac.model.abstract_model import AbstractModel
 from smac.random_design.abstract_random_design import AbstractRandomDesign
 from smac.runhistory.encoder.abstract_encoder import AbstractRunHistoryEncoder
 from smac.runhistory.runhistory import RunHistory
 from smac.scenario import Scenario
 from smac.utils.logging import get_logger
```

### Comparing `smac-2.0.0b1/smac/main/smbo.py` & `smac-2.0.1/smac/main/smbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 import json
 import time
 from pathlib import Path
 
 import numpy as np
 from ConfigSpace import Configuration
+from numpy import ndarray
 
 from smac.acquisition.function.abstract_acquisition_function import (
     AbstractAcquisitionFunction,
 )
-from smac.callback import Callback
+from smac.callback.callback import Callback
 from smac.intensifier.abstract_intensifier import AbstractIntensifier
 from smac.model.abstract_model import AbstractModel
 from smac.runhistory import StatusType, TrialInfo, TrialValue
 from smac.runhistory.runhistory import RunHistory
 from smac.runner import FirstRunCrashedException
 from smac.runner.abstract_runner import AbstractRunner
+from smac.runner.dask_runner import DaskParallelRunner
 from smac.scenario import Scenario
 from smac.utils.data_structures import recursively_compare_dicts
 from smac.utils.logging import get_logger
 
 __copyright__ = "Copyright 2022, automl.org"
 __license__ = "3-clause BSD"
 
@@ -240,17 +242,27 @@
         if (config_selector := self._intensifier._config_selector) is not None:
             config_selector._acquisition_function = acquisition_function
             config_selector._acquisition_function.model = config_selector._model
 
             assert config_selector._acquisition_maximizer is not None
             config_selector._acquisition_maximizer.acquisition_function = acquisition_function
 
-    def optimize(self) -> Configuration | list[Configuration]:
+    def optimize(self, *, data_to_scatter: dict[str, Any] | None = None) -> Configuration | list[Configuration]:
         """Runs the Bayesian optimization loop.
 
+        Parameters
+        ----------
+        data_to_scatter: dict[str, Any] | None
+            When a user scatters data from their local process to the distributed network,
+            this data is distributed in a round-robin fashion grouping by number of cores.
+            Roughly speaking, we can keep this data in memory and then we do not have to (de-)serialize the data
+            every time we would like to execute a target function with a big dataset.
+            For example, when your target function has a big dataset shared across all the target function,
+            this argument is very useful.
+
         Returns
         -------
         incumbent : Configuration
             The best found configuration.
         """
         # We return the incumbent if we already finished the a process (we don't want to allow to call
         # optimize more than once).
@@ -265,26 +277,35 @@
         # If we continue the optimization, the starting time is set by the load method
         if self._start_time is None:
             self._start_time = time.time()
 
         for callback in self._callbacks:
             callback.on_start(self)
 
+        dask_data_to_scatter = {}
+        if isinstance(self._runner, DaskParallelRunner) and data_to_scatter is not None:
+            dask_data_to_scatter = dict(data_to_scatter=self._runner._client.scatter(data_to_scatter, broadcast=True))
+        elif data_to_scatter is not None:
+            raise ValueError(
+                "data_to_scatter is valid only for DaskParallelRunner, "
+                f"but {dask_data_to_scatter} was provided for {self._runner.__class__.__name__}"
+            )
+
         # Main BO loop
         while True:
             for callback in self._callbacks:
                 callback.on_iteration_start(self)
 
             try:
                 # Sample next trial from the intensification
                 trial_info = self.ask()
 
                 # We submit the trial to the runner
                 # In multi-worker mode, SMAC waits till a new worker is available here
-                self._runner.submit_trial(trial_info=trial_info)
+                self._runner.submit_trial(trial_info=trial_info, **dask_data_to_scatter)
             except StopIteration:
                 self._stop = True
 
             # We add results from the runner if results are available
             self._add_results()
 
             # Some statistics
@@ -436,17 +457,27 @@
                 if len(cost) != len(cost_threshold):
                     raise RuntimeError("You must specify a termination cost threshold for each objective.")
 
                 if all(cost[i] < cost_threshold[i] for i in range(len(cost))):
                     logger.info("Cost threshold was reached. Abort is requested.")
                     self._stop = True
 
-    def _register_callback(self, callback: Callback) -> None:
-        """Registers a callback to be called before, in between, and after the Bayesian optimization loop."""
-        self._callbacks += [callback]
+    def register_callback(self, callback: Callback, index: int = -1) -> None:
+        """
+        Registers a callback to be called before, in between, and after the Bayesian optimization loop.
+
+
+        Parameters
+        ----------
+        callback : Callback
+            The callback to be registered.
+        index : int
+            The index at which the callback should be registered.
+        """
+        self._callbacks.insert(index, callback)
 
     def _initialize_state(self) -> None:
         """Detects whether the optimization is restored from a previous state."""
         # Here we actually check whether the run should be continued or not.
         # More precisely, we update our smbo/runhistory/intensifier object if all component arguments
         # and scenario object are the same. For doing so, we create a specific hash.
         # The SMBO object recognizes that stats (based on runhistory) is not empty and hence does not the run initial
@@ -508,36 +539,35 @@
         self.save()
 
     def validate(
         self,
         config: Configuration,
         *,
         seed: int | None = None,
-    ) -> float | list[float]:
+    ) -> float | ndarray[float]:
         """Validates a configuration on other seeds than the ones used in the optimization process and on the highest
-        budget (if budget type is real-valued).
+        budget (if budget type is real-valued). Does not exceed the maximum number of config calls or seeds as defined
+        in the scenario.
 
         Parameters
         ----------
         config : Configuration
             Configuration to validate
-        instances : list[str] | None, defaults to None
-            Which instances to validate. If None, all instances specified in the scenario are used.
             In case that the budget type is real-valued budget, this argument is ignored.
         seed : int | None, defaults to None
             If None, the seed from the scenario is used.
 
         Returns
         -------
-        cost : float | list[float]
+        cost : float | ndarray[float]
             The averaged cost of the configuration. In case of multi-fidelity, the cost of each objective is
             averaged.
         """
         if seed is None:
-            seed = 0
+            seed = self._scenario.seed
 
         costs = []
         for trial in self._intensifier.get_trials_of_interest(config, validate=True, seed=seed):
             kwargs: dict[str, Any] = {}
             if trial.seed is not None:
                 kwargs["seed"] = trial.seed
             if trial.budget is not None:
```

### Comparing `smac-2.0.0b1/smac/model/abstract_model.py` & `smac-2.0.1/smac/model/abstract_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/abstract_gaussian_process.py` & `smac-2.0.1/smac/model/gaussian_process/abstract_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/gaussian_process.py` & `smac-2.0.1/smac/model/gaussian_process/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/gpytorch_gaussian_process.py` & `smac-2.0.1/smac/model/gaussian_process/gpytorch_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/__init__.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/_boing.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/_boing.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/base_kernels.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/base_kernels.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/hamming_kernel.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/hamming_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/matern_kernel.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/matern_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/rbf_kernel.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/kernels/white_kernel.py` & `smac-2.0.1/smac/model/gaussian_process/kernels/white_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/mcmc_gaussian_process.py` & `smac-2.0.1/smac/model/gaussian_process/mcmc_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/priors/abstract_prior.py` & `smac-2.0.1/smac/model/gaussian_process/priors/abstract_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/priors/gamma_prior.py` & `smac-2.0.1/smac/model/gaussian_process/priors/gamma_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/priors/horseshoe_prior.py` & `smac-2.0.1/smac/model/gaussian_process/priors/horseshoe_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/priors/log_normal_prior.py` & `smac-2.0.1/smac/model/gaussian_process/priors/log_normal_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/gaussian_process/priors/tophat_prior.py` & `smac-2.0.1/smac/model/gaussian_process/priors/tophat_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/multi_objective_model.py` & `smac-2.0.1/smac/model/multi_objective_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/random_forest/abstract_random_forest.py` & `smac-2.0.1/smac/model/random_forest/abstract_random_forest.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/model/random_forest/random_forest.py` & `smac-2.0.1/smac/model/random_forest/random_forest.py`

 * *Files 11% similar despite different names*

```diff
@@ -270,34 +270,17 @@
 
         if X.shape[1] != len(self._bounds):
             raise ValueError("Rows in X should have %d entries but have %d!" % (len(self._bounds), X.shape[1]))
 
         assert self._rf is not None
         X = self._impute_inactive(X)
 
-        dat_ = np.zeros((X.shape[0], self._rf_opts.num_trees))  # Marginalized predictions for each tree
-        for i, x in enumerate(X):
-
-            # Marginalize over instances
-            # 1. get all leaf values for each tree
-            preds_trees: list[list[float]] = [[] for i in range(self._rf_opts.num_trees)]
-
-            for feat in self._instance_features.values():
-                x_ = np.concatenate([x, feat])
-                preds_per_tree = self._rf.all_leaf_values(x_)
-                for tree_id, preds in enumerate(preds_per_tree):
-                    preds_trees[tree_id] += preds
-
-            # 2. average in each tree
-            if self._log_y:
-                for tree_id in range(self._rf_opts.num_trees):
-                    dat_[i, tree_id] = np.log(np.exp(np.array(preds_trees[tree_id])).mean())
-            else:
-                for tree_id in range(self._rf_opts.num_trees):
-                    dat_[i, tree_id] = np.array(preds_trees[tree_id]).mean()
+        X_feat = list(self._instance_features.values())
+        dat_ = self._rf.predict_marginalized_over_instances_batch(X, X_feat, self._log_y)
+        dat_ = np.array(dat_)
 
         # 3. compute statistics across trees
         mean_ = dat_.mean(axis=1)
         var = dat_.var(axis=1)
 
         if var is None:
             raise RuntimeError("The variance must not be none.")
```

### Comparing `smac-2.0.0b1/smac/model/random_model.py` & `smac-2.0.1/smac/model/random_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/multi_objective/abstract_multi_objective_algorithm.py` & `smac-2.0.1/smac/multi_objective/abstract_multi_objective_algorithm.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/multi_objective/aggregation_strategy.py` & `smac-2.0.1/smac/multi_objective/aggregation_strategy.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/multi_objective/parego.py` & `smac-2.0.1/smac/multi_objective/parego.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/random_design/__init__.py` & `smac-2.0.1/smac/random_design/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/random_design/abstract_random_design.py` & `smac-2.0.1/smac/random_design/abstract_random_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/random_design/annealing_design.py` & `smac-2.0.1/smac/random_design/annealing_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/random_design/modulus_design.py` & `smac-2.0.1/smac/random_design/modulus_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/random_design/probability_design.py` & `smac-2.0.1/smac/random_design/probability_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/dataclasses.py` & `smac-2.0.1/smac/runhistory/dataclasses.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/__init__.py` & `smac-2.0.1/smac/runhistory/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/abstract_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/abstract_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/boing_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/boing_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/eips_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/eips_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/encoder.py` & `smac-2.0.1/smac/runhistory/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/inverse_scaled_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/inverse_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/log_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/log_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/log_scaled_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/log_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/scaled_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/encoder/sqrt_scaled_encoder.py` & `smac-2.0.1/smac/runhistory/encoder/sqrt_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runhistory/runhistory.py` & `smac-2.0.1/smac/runhistory/runhistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,17 @@
         if config_id is None:
             self._n_id += 1
             self._config_ids[config] = self._n_id
             self._ids_config[self._n_id] = config
 
             config_id = self._n_id
 
+        # Set the id attribute of the config object, so that users can access it
+        config.config_id = config_id
+
         if status != StatusType.RUNNING:
             if self._n_objectives == -1:
                 self._n_objectives = n_objectives
             elif self._n_objectives != n_objectives:
                 raise ValueError(
                     f"Cost is not of the same length ({n_objectives}) as the number of "
                     f"objectives ({self._n_objectives})."
@@ -589,14 +592,18 @@
         """Returns the configuration from the configuration id."""
         return self._ids_config[config_id]
 
     def get_config_id(self, config: Configuration) -> int:
         """Returns the configuration id from a configuration."""
         return self._config_ids[config]
 
+    def has_config(self, config: Configuration) -> bool:
+        """Check if the config is stored in the runhistory"""
+        return config in self._config_ids
+
     def get_configs(self, sort_by: str | None = None) -> list[Configuration]:
         """Return all configurations in this RunHistory object.
 
         Parameters
         ----------
         sort_by : str | None, defaults to None
             Sort the configs by ``cost`` (lowest cost first) or ``num_trials`` (config with lowest number of trials
@@ -670,14 +677,16 @@
         Does not return running trials. Please use ``get_running_trials`` to receive running trials.
 
         Parameters
         ----------
         config : Configuration
         highest_observed_budget_only : bool
             Select only the highest observed budget run for this configuration.
+            Meaning on multiple executions of the same instance-seed pair for a
+            a given configuration, only the highest observed budget is returned.
 
         Returns
         -------
         trials : list[InstanceSeedBudgetKey]
             List of trials for the passed configuration.
         """
         config_id = self._config_ids.get(config)
```

### Comparing `smac-2.0.0b1/smac/runner/abstract_runner.py` & `smac-2.0.1/smac/runner/abstract_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,23 +72,32 @@
 
         # We need to exapdn crash cost if the user did not do it
         if self._n_objectives > 1:
             if not isinstance(scenario.crash_cost, list):
                 assert isinstance(scenario.crash_cost, float)
                 self._crash_cost = [scenario.crash_cost for _ in range(self._n_objectives)]
 
-    def run_wrapper(self, trial_info: TrialInfo) -> tuple[TrialInfo, TrialValue]:
+    def run_wrapper(
+        self, trial_info: TrialInfo, **dask_data_to_scatter: dict[str, Any]
+    ) -> tuple[TrialInfo, TrialValue]:
         """Wrapper around run() to execute and check the execution of a given config.
         This function encapsulates common
         handling/processing, so that run() implementation is simplified.
 
         Parameters
         ----------
         trial_info : RunInfo
             Object that contains enough information to execute a configuration run in isolation.
+        dask_data_to_scatter: dict[str, Any]
+            When a user scatters data from their local process to the distributed network,
+            this data is distributed in a round-robin fashion grouping by number of cores.
+            Roughly speaking, we can keep this data in memory and then we do not have to (de-)serialize the data
+            every time we would like to execute a target function with a big dataset.
+            For example, when your target function has a big dataset shared across all the target function,
+            this argument is very useful.
 
         Returns
         -------
         info : TrialInfo
             An object containing the configuration launched.
         value : TrialValue
             Contains information about the status/performance of config.
@@ -97,14 +106,15 @@
 
         try:
             status, cost, runtime, additional_info = self.run(
                 config=trial_info.config,
                 instance=trial_info.instance,
                 budget=trial_info.budget,
                 seed=trial_info.seed,
+                **dask_data_to_scatter,
             )
         except Exception as e:
             status = StatusType.CRASHED
             cost = self._crash_cost
             runtime = time.time() - start
 
             # Add context information to the error message
```

### Comparing `smac-2.0.0b1/smac/runner/abstract_serial_runner.py` & `smac-2.0.1/smac/runner/abstract_serial_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/runner/dask_runner.py` & `smac-2.0.1/smac/runner/dask_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator
+from typing import Any, Iterator
 
 import time
 from pathlib import Path
 
 import dask
 from ConfigSpace import Configuration
 from dask.distributed import Client, Future, wait
@@ -94,15 +94,15 @@
                 self._scheduler_file = self._scenario.output_directory / ".dask_scheduler_file"
                 self._client.write_scheduler_file(scheduler_file=str(self._scheduler_file))
         else:
             # We just use their set up
             self._client = dask_client
             self._close_client_at_del = False
 
-    def submit_trial(self, trial_info: TrialInfo) -> None:
+    def submit_trial(self, trial_info: TrialInfo, **dask_data_to_scatter: dict[str, Any]) -> None:
         """This function submits a configuration embedded in a ``trial_info`` object, and uses one of
         the workers to produce a result locally to each worker.
 
         The execution of a configuration follows this procedure:
 
         #. The SMBO/intensifier generates a `TrialInfo`.
         #. SMBO calls `submit_trial` so that a worker launches the `trial_info`.
@@ -111,14 +111,22 @@
 
         All results will be only available locally to each worker, so the main node needs to collect them.
 
         Parameters
         ----------
         trial_info : TrialInfo
             An object containing the configuration launched.
+
+        dask_data_to_scatter: dict[str, Any]
+            When a user scatters data from their local process to the distributed network,
+            this data is distributed in a round-robin fashion grouping by number of cores.
+            Roughly speaking, we can keep this data in memory and then we do not have to (de-)serialize the data
+            every time we would like to execute a target function with a big dataset.
+            For example, when your target function has a big dataset shared across all the target function,
+            this argument is very useful.
         """
         # Check for resources or block till one is available
         if self.count_available_workers() <= 0:
             logger.debug("No worker available. Waiting for one to be available...")
             wait(self._pending_trials, return_when="FIRST_COMPLETED")
             self._process_pending_trials()
 
@@ -129,15 +137,15 @@
             if self.count_available_workers() <= 0:
                 raise RuntimeError(
                     "Tried to execute a job, but no worker was ever available."
                     "This likely means that a worker crashed or no workers were properly configured."
                 )
 
         # At this point we can submit the job
-        trial = self._client.submit(self._single_worker.run_wrapper, trial_info=trial_info)
+        trial = self._client.submit(self._single_worker.run_wrapper, trial_info=trial_info, **dask_data_to_scatter)
         self._pending_trials.append(trial)
 
     def iter_results(self) -> Iterator[tuple[TrialInfo, TrialValue]]:  # noqa: D102
         self._process_pending_trials()
         while self._results_queue:
             yield self._results_queue.pop(0)
 
@@ -150,16 +158,19 @@
 
     def run(
         self,
         config: Configuration,
         instance: str | None = None,
         budget: float | None = None,
         seed: int | None = None,
+        **dask_data_to_scatter: dict[str, Any],
     ) -> tuple[StatusType, float | list[float], float, dict]:  # noqa: D102
-        return self._single_worker.run(config=config, instance=instance, seed=seed, budget=budget)
+        return self._single_worker.run(
+            config=config, instance=instance, seed=seed, budget=budget, **dask_data_to_scatter
+        )
 
     def count_available_workers(self) -> int:
         """Total number of workers available. This number is dynamic as more resources
         can be allocated.
         """
         return sum(self._client.nthreads().values()) - len(self._pending_trials)
```

### Comparing `smac-2.0.0b1/smac/runner/target_function_runner.py` & `smac-2.0.1/smac/runner/target_function_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,15 +68,20 @@
         # However, we only want to warn the user and not
         for key in list(signature.keys())[1:]:
             if key not in required_arguments:
                 logger.warning(f"The argument {key} is not set by SMAC: Consider removing it from the target function.")
 
         # Pynisher limitations
         if (memory := self._scenario.trial_memory_limit) is not None:
+            unit = None
+            if isinstance(memory, (tuple, list)):
+                memory, unit = memory
             memory = int(math.ceil(memory))
+            if unit is not None:
+                memory = (memory, unit)
 
         if (time := self._scenario.trial_walltime_limit) is not None:
             time = int(math.ceil(time))
 
         self._memory_limit = memory
         self._algorithm_walltime_limit = time
 
@@ -89,42 +94,52 @@
 
     def run(
         self,
         config: Configuration,
         instance: str | None = None,
         budget: float | None = None,
         seed: int | None = None,
+        **dask_data_to_scatter: dict[str, Any],
     ) -> tuple[StatusType, float | list[float], float, dict]:
         """Calls the target function with pynisher if algorithm wall time limit or memory limit is
         set. Otherwise, the function is called directly.
 
         Parameters
         ----------
         config : Configuration
             Configuration to be passed to the target function.
         instance : str | None, defaults to None
             The Problem instance.
         budget : float | None, defaults to None
             A positive, real-valued number representing an arbitrary limit to the target function
             handled by the target function internally.
         seed : int, defaults to None
+        dask_data_to_scatter: dict[str, Any]
+            This kwargs must be empty when we do not use dask! ()
+            When a user scatters data from their local process to the distributed network,
+            this data is distributed in a round-robin fashion grouping by number of cores.
+            Roughly speaking, we can keep this data in memory and then we do not have to (de-)serialize the data
+            every time we would like to execute a target function with a big dataset.
+            For example, when your target function has a big dataset shared across all the target function,
+            this argument is very useful.
 
         Returns
         -------
         status : StatusType
             Status of the trial.
         cost : float | list[float]
             Resulting cost(s) of the trial.
         runtime : float
             The time the target function took to run.
         additional_info : dict
             All further additional trial information.
         """
         # The kwargs are passed to the target function.
         kwargs: dict[str, Any] = {}
+        kwargs.update(dask_data_to_scatter)
 
         if "seed" in self._required_arguments:
             kwargs["seed"] = seed
 
         if "instance" in self._required_arguments:
             kwargs["instance"] = instance
```

### Comparing `smac-2.0.0b1/smac/runner/target_function_script_runner.py` & `smac-2.0.1/smac/runner/target_function_script_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/scenario.py` & `smac-2.0.1/smac/scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,19 @@
         no constraints are enforced. Otherwise, the process will be spawned by pynisher.
     trial_memory_limit : int | None, defaults to None
         The maximum memory in MB that a trial is allowed to use. If not specified,
         no constraints are enforced. Otherwise, the process will be spawned by pynisher.
     n_trials : int, defaults to 100
         The maximum number of trials (combination of configuration, seed, budget, and instance, depending on the task)
         to run.
+    use_default_config: bool, defaults to False.
+        If True, the configspace's default configuration is evaluated in the initial design.
+        For historic benchmark reasons, this is False by default.
+        Notice, that this will result in n_configs + 1 for the initial design. Respecting n_trials,
+        this will result in one fewer evaluated configuration in the optimization.
     instances : list[str] | None, defaults to None
         Names of the instances to use. If None, no instances are used.
         Instances could be dataset names, seeds, subsets, etc.
     instance_features : dict[str, list[float]] | None, defaults to None
         Instances can be associated with features. For example, meta data of the dataset (mean, var, ...) can be
         incorporated which are then further used to expand the training data of the surrogate model.
     min_budget : float | int | None, defaults to None
@@ -89,14 +94,15 @@
 
     # Limitations
     walltime_limit: float = np.inf
     cputime_limit: float = np.inf
     trial_walltime_limit: float | None = None
     trial_memory_limit: int | None = None
     n_trials: int = 100
+    use_default_config: bool = False
 
     # Algorithm Configuration
     instances: list[str] | None = None
     instance_features: dict[str, list[float]] | None = None
 
     # Budgets
     min_budget: float | int | None = None
@@ -109,14 +115,24 @@
     def __post_init__(self) -> None:
         """Checks whether the config is valid."""
         # Use random seed if seed is -1
         if self.seed == -1:
             seed = random.randint(0, 999999)
             object.__setattr__(self, "seed", seed)
 
+        # Transform instances to string if they are not
+        if self.instances is not None:
+            instances = [str(instance) for instance in self.instances]
+            object.__setattr__(self, "instances", instances)
+
+        # Transform instance features to string if they are not
+        if self.instance_features is not None:
+            instance_features = {str(instance): features for instance, features in self.instance_features.items()}
+            object.__setattr__(self, "instance_features", instance_features)
+
         # Change directory wrt name and seed
         self._change_output_directory()
 
         # Set empty meta
         object.__setattr__(self, "_meta", {})
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `smac-2.0.0b1/smac/utils/configspace.py` & `smac-2.0.1/smac/utils/configspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/utils/data_structures.py` & `smac-2.0.1/smac/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/utils/logging.py` & `smac-2.0.1/smac/utils/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 from pathlib import Path
 
 import yaml
+from typing_extensions import Literal
 
 import smac
 
 __copyright__ = "Copyright 2022, automl.org"
 __license__ = "3-clause BSD"
 
 
-def setup_logging(level: int | Path | None = None) -> None:
+def setup_logging(
+    level: int | Path | Literal[False] | None = False,
+) -> None:
     """Sets up the logging configuration for all modules.
 
     Parameters
     ----------
-    level : int | Path | None, defaults to None
+    level : int | Path | Literal[False] | None, defaults to None
         An integer representing the logging level. An custom logging configuration can be used when passing a path.
+        If False, no logging setup is performed.
     """
+    if level is False:
+        return
+
     if isinstance(level, Path):
         log_filename = level
     else:
         path = Path() / smac.__file__
         log_filename = path.parent / "logging.yml"
 
     with (log_filename).open("r") as stream:
```

### Comparing `smac-2.0.0b1/smac/utils/multi_objective.py` & `smac-2.0.1/smac/utils/multi_objective.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/utils/pareto_front.py` & `smac-2.0.1/smac/utils/pareto_front.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/utils/subspaces/__init__.py` & `smac-2.0.1/smac/utils/subspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/utils/subspaces/boing_subspace.py` & `smac-2.0.1/smac/utils/subspaces/boing_subspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac/utils/subspaces/turbo_subspace.py` & `smac-2.0.1/smac/utils/subspaces/turbo_subspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.0b1/smac.egg-info/PKG-INFO` & `smac-2.0.1/smac.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smac
-Version: 2.0.0b1
+Version: 2.0.1
 Summary: SMAC3, a Python implementation of 'Sequential Model-based Algorithm Configuration'.
 Home-page: https://www.automl.org/
 Author: 	Marius Lindauer, Katharina Eggensperger, Matthias Feurer, André Biedenkapp, Difan Deng,
 	Carolin Benjamins, Tim Ruhkopf, René Sass and Frank Hutter
 Author-email: fh@cs.uni-freiburg.de
 License: BSD 3-Clause License
 Project-URL: Documentation, https://https://github.com/automl.github.io/SMAC3/main
@@ -31,17 +31,17 @@
 [![Tests](https://github.com/automl/SMAC3/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/pytest.yml)
 [![Documentation](https://github.com/automl/SMAC3/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/docs.yml)
 [![codecov
 Status](https://codecov.io/gh/automl/SMAC3/branch/master/graph/badge.svg)](https://codecov.io/gh/automl/SMAC3)
 
 <img src="docs/images/logo.png" style="width: 50%;" />
 
-SMAC is a tool for algorithm configuration to optimize the parameters of arbitrary algorithms, including hyperparameter 
-optimization of Machine Learning algorithms. The main core consists of Bayesian Optimization in combination with an 
-aggressive racing mechanism to efficiently decide which of two configurations performs better.
+SMAC offers a robust and flexible framework for Bayesian Optimization to support users in determining well-performing 
+hyperparameter configurations for their (Machine Learning) algorithms, datasets and applications at hand. The main core 
+consists of Bayesian Optimization in combination with an aggressive racing mechanism to efficiently decide which of two configurations performs better.
 
 SMAC3 is written in Python3 and continuously tested with Python 3.8, 3.9, and 3.10. Its Random
 Forest is written in C++. In further texts, SMAC is representatively mentioned for SMAC3.
 
 > [Documentation](https://automl.github.io/SMAC3)
 
 > [Roadmap](https://github.com/orgs/automl/projects/5/views/2)
@@ -80,18 +80,18 @@
 ```
 
 Install SMAC via PyPI:
 ```
 pip install smac
 ```
 
-Or alternatively, clone the environment:
+If you want to contribute to SMAC, use the following steps instead:
 ```
 git clone https://github.com/automl/SMAC3.git && cd SMAC3
-pip install -e .[dev]
+make install-dev
 ```
 
 
 ## Minimal Example
 
 ```py
 from ConfigSpace import Configuration, ConfigurationSpace
@@ -119,28 +119,37 @@
 # Use SMAC to find the best configuration/hyperparameters
 smac = HyperparameterOptimizationFacade(scenario, train)
 incumbent = smac.optimize()
 ```
 
 More examples can be found in the [documentation](https://automl.github.io/SMAC3/main/examples/).
 
+## Visualization via DeepCAVE
+
+With DeepCAVE ([Repo](https://github.com/automl/DeepCAVE), [Paper](https://arxiv.org/abs/2206.03493)) you can visualize your SMAC runs. It is a visualization and analysis tool for AutoML (especially for the sub-problem
+hyperparameter optimization) runs.
 
 ## License
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the 3-clause BSD license (please see the LICENSE file).
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 
 You should have received a copy of the 3-clause BSD license
 along with this program (see LICENSE file).
 If not, see [here](https://opensource.org/licenses/BSD-3-Clause).
 
+## Contacting us
+
+If you have trouble using SMAC, a concrete question or found a bug, please create an [issue](https://github.com/automl/SMAC3/issues). This is the easiest way to communicate about these things with us. 
+
+For all other inquiries, please write an email to smac[at]ai[dot]uni[dash]hannover[dot]de.
 
 ## Miscellaneous
 
 SMAC3 is developed by the [AutoML Groups of the Universities of Hannover and
 Freiburg](http://www.automl.org/).
 
 If you have found a bug, please report to [issues](https://github.com/automl/SMAC3/issues). Moreover, we are 
@@ -159,7 +168,9 @@
   number  = {54},
   pages   = {1--9},
   url     = {http://jmlr.org/papers/v23/21-0888.html}
 }
 ```
 
 Copyright (C) 2016-2022  [AutoML Group](http://www.automl.org).
+
+
```

### Comparing `smac-2.0.0b1/smac.egg-info/SOURCES.txt` & `smac-2.0.1/smac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 smac/__init__.py
-smac/callback.py
 smac/constants.py
 smac/logging.yml
 smac/py.typed
 smac/scenario.py
 smac.egg-info/PKG-INFO
 smac.egg-info/SOURCES.txt
 smac.egg-info/dependency_links.txt
@@ -27,14 +26,17 @@
 smac/acquisition/maximizer/__init__.py
 smac/acquisition/maximizer/abstract_acqusition_maximizer.py
 smac/acquisition/maximizer/differential_evolution.py
 smac/acquisition/maximizer/helpers.py
 smac/acquisition/maximizer/local_and_random_search.py
 smac/acquisition/maximizer/local_search.py
 smac/acquisition/maximizer/random_search.py
+smac/callback/__init__.py
+smac/callback/callback.py
+smac/callback/metadata_callback.py
 smac/facade/__init__.py
 smac/facade/abstract_facade.py
 smac/facade/algorithm_configuration_facade.py
 smac/facade/blackbox_facade.py
 smac/facade/hyperband_facade.py
 smac/facade/hyperparameter_optimization_facade.py
 smac/facade/multi_fidelity_facade.py
```

