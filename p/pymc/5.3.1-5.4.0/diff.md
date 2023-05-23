# Comparing `tmp/pymc-5.3.1.tar.gz` & `tmp/pymc-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.3.1.tar", last modified: Wed Apr 26 17:34:50 2023, max compression
+gzip compressed data, was "dist/pymc-5.4.0.tar", last modified: Tue May 23 08:47:51 2023, max compression
```

## Comparing `pymc-5.3.1.tar` & `pymc-5.4.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-26 17:34:28.000000 pymc-5.3.1/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-26 17:34:28.000000 pymc-5.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-26 17:34:28.000000 pymc-5.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-04-26 17:34:28.000000 pymc-5.3.1/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-26 17:34:28.000000 pymc-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 17:34:28.000000 pymc-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-26 17:34:50.000000 pymc-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-26 17:34:28.000000 pymc-5.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-26 17:34:28.000000 pymc-5.3.1/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    39317 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    34442 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    90135 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-26 17:34:28.000000 pymc-5.3.1/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 17:34:50.000000 pymc-5.3.1/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-26 17:34:28.000000 pymc-5.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 17:34:28.000000 pymc-5.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:34:50.000000 pymc-5.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-04-26 17:34:28.000000 pymc-5.3.1/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-04-26 17:34:28.000000 pymc-5.3.1/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-26 17:34:50.000000 pymc-5.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-04-26 17:34:28.000000 pymc-5.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-04-26 17:34:28.000000 pymc-5.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-23 08:47:43.000000 pymc-5.4.0/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-23 08:47:43.000000 pymc-5.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-23 08:47:43.000000 pymc-5.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-05-23 08:47:43.000000 pymc-5.4.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-05-23 08:47:43.000000 pymc-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 08:47:43.000000 pymc-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-23 08:47:51.000000 pymc-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-23 08:47:43.000000 pymc-5.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-23 08:47:43.000000 pymc-5.4.0/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116464 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42225 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36499 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90135 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50483 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 08:47:43.000000 pymc-5.4.0/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 08:47:51.000000 pymc-5.4.0/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 08:47:43.000000 pymc-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-23 08:47:43.000000 pymc-5.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:47:51.000000 pymc-5.4.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-05-23 08:47:43.000000 pymc-5.4.0/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-05-23 08:47:43.000000 pymc-5.4.0/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 08:47:51.000000 pymc-5.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-05-23 08:47:43.000000 pymc-5.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-05-23 08:47:43.000000 pymc-5.4.0/versioneer.py
```

### Comparing `pymc-5.3.1/ARCHITECTURE.md` & `pymc-5.4.0/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/CODE_OF_CONDUCT.md` & `pymc-5.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/CONTRIBUTING.md` & `pymc-5.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/GOVERNANCE.md` & `pymc-5.4.0/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/LICENSE` & `pymc-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/PKG-INFO` & `pymc-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.3.1
+Version: 5.4.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.3.1/README.rst` & `pymc-5.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/RELEASE-NOTES.md` & `pymc-5.4.0/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/__init__.py` & `pymc-5.4.0/pymc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 # pylint: disable=wildcard-import
 
 import logging
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
         _log.addHandler(handler)
```

### Comparing `pymc-5.3.1/pymc/backends/__init__.py` & `pymc-5.4.0/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/backends/arviz.py` & `pymc-5.4.0/pymc/backends/arviz.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from pymc.util import get_default_varnames
 
 if TYPE_CHECKING:
     from pymc.backends.base import MultiTrace  # pylint: disable=invalid-name
 
 ___all__ = [""]
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 # random variable object ...
 Var = Any  # pylint: disable=invalid-name
 
 
 def find_observations(model: "Model") -> Dict[str, Var]:
     """If there are observations available, return them as a dictionary."""
```

### Comparing `pymc-5.3.1/pymc/backends/base.py` & `pymc-5.4.0/pymc/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 import numpy as np
 
 from pymc.backends.report import SamplerReport
 from pymc.model import modelcontext
 from pymc.util import get_var_name
 
-logger = logging.getLogger("pymc")
+logger = logging.getLogger(__name__)
 
 
 class BackendError(Exception):
     pass
 
 
 class IBaseTrace(ABC, Sized):
```

### Comparing `pymc-5.3.1/pymc/backends/mcbackend.py` & `pymc-5.4.0/pymc/backends/mcbackend.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     BlockedStep,
     CompoundStep,
     StatsBijection,
     flat_statname,
     flatten_steps,
 )
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 
 def find_data(pmodel: Model) -> List[mcb.DataVariable]:
     """Extracts data variables from a model."""
     observed_rvs = {pmodel.rvs_to_values[rv] for rv in pmodel.observed_RVs}
     dvars = []
     # All data containers are named vars!
```

### Comparing `pymc-5.3.1/pymc/backends/ndarray.py` & `pymc-5.4.0/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/backends/report.py` & `pymc-5.4.0/pymc/backends/report.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import dataclasses
 import logging
 
 from typing import Dict, List, Optional
 
 from pymc.stats.convergence import _LEVELS, SamplerWarning
 
-logger = logging.getLogger("pymc")
+logger = logging.getLogger(__name__)
 
 
 class SamplerReport:
     """Bundle warnings, convergence stats and metadata of a sampling run."""
 
     def __init__(self) -> None:
         self._chain_warnings: Dict[int, List[SamplerWarning]] = {}
```

### Comparing `pymc-5.3.1/pymc/blocking.py` & `pymc-5.4.0/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/data.py` & `pymc-5.4.0/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/__init__.py` & `pymc-5.4.0/pymc/distributions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,37 +51,43 @@
     Weibull,
 )
 from pymc.distributions.discrete import (
     Bernoulli,
     BetaBinomial,
     Binomial,
     Categorical,
-    Constant,
-    DiracDelta,
     DiscreteUniform,
     DiscreteWeibull,
     Geometric,
     HyperGeometric,
     NegativeBinomial,
     OrderedLogistic,
     OrderedProbit,
     Poisson,
-    ZeroInflatedBinomial,
-    ZeroInflatedNegativeBinomial,
-    ZeroInflatedPoisson,
 )
 from pymc.distributions.distribution import (
     Continuous,
     CustomDist,
     DensityDist,
+    DiracDelta,
     Discrete,
     Distribution,
     SymbolicRandomVariable,
 )
-from pymc.distributions.mixture import Mixture, NormalMixture
+from pymc.distributions.mixture import (
+    HurdleGamma,
+    HurdleLogNormal,
+    HurdleNegativeBinomial,
+    HurdlePoisson,
+    Mixture,
+    NormalMixture,
+    ZeroInflatedBinomial,
+    ZeroInflatedNegativeBinomial,
+    ZeroInflatedPoisson,
+)
 from pymc.distributions.multivariate import (
     CAR,
     Dirichlet,
     DirichletMultinomial,
     KroneckerNormal,
     LKJCholeskyCov,
     LKJCorr,
@@ -135,15 +141,14 @@
     "VonMises",
     "Binomial",
     "BetaBinomial",
     "Bernoulli",
     "Poisson",
     "NegativeBinomial",
     "DiracDelta",
-    "Constant",
     "ZeroInflatedPoisson",
     "ZeroInflatedNegativeBinomial",
     "ZeroInflatedBinomial",
     "DiscreteUniform",
     "Geometric",
     "HyperGeometric",
     "Categorical",
@@ -190,8 +195,12 @@
     "Rice",
     "Moyal",
     "Simulator",
     "Truncated",
     "Censored",
     "CAR",
     "PolyaGamma",
+    "HurdleGamma",
+    "HurdleLogNormal",
+    "HurdleNegativeBinomial",
+    "HurdlePoisson",
 ]
```

### Comparing `pymc-5.3.1/pymc/distributions/bound.py` & `pymc-5.4.0/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/censored.py` & `pymc-5.4.0/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/continuous.py` & `pymc-5.4.0/pymc/distributions/continuous.py`

 * *Files 0% similar despite different names*

```diff
@@ -1343,23 +1343,32 @@
     Variance  :math:`\dfrac{1}{\lambda^2}`
     ========  ============================
 
     Parameters
     ----------
     lam : tensor_like of float
         Rate or inverse scale (``lam`` > 0).
+    scale: tensor_like of float
+        Alternative parameter (scale = 1/lam).
     """
     rv_op = exponential
 
     @classmethod
-    def dist(cls, lam: DIST_PARAMETER_TYPES, *args, **kwargs):
-        lam = pt.as_tensor_variable(floatX(lam))
+    def dist(cls, lam=None, scale=None, *args, **kwargs):
+        if lam is not None and scale is not None:
+            raise ValueError("Incompatible parametrization. Can't specify both lam and scale.")
+        elif lam is None and scale is None:
+            raise ValueError("Incompatible parametrization. Must specify either lam or scale.")
 
+        if scale is None:
+            scale = pt.reciprocal(lam)
+
+        scale = pt.as_tensor_variable(floatX(scale))
         # PyTensor exponential op is parametrized in terms of mu (1/lam)
-        return super().dist([pt.reciprocal(lam)], **kwargs)
+        return super().dist([scale], **kwargs)
 
     def moment(rv, size, mu):
         if not rv_size_is_none(size):
             mu = pt.full(size, mu)
         return mu
 
     def logp(value, mu):
@@ -1476,14 +1485,21 @@
 
         return check_parameters(
             res,
             b > 0,
             msg="b > 0",
         )
 
+    def icdf(value, mu, b):
+        res = pt.switch(
+            pt.le(value, 0.5), mu + b * np.log(2 * value), mu - b * np.log(2 - 2 * value)
+        )
+        res = check_icdf_value(res, value)
+        return check_icdf_parameters(res, b > 0, msg="b > 0")
+
 
 class AsymmetricLaplaceRV(RandomVariable):
     name = "asymmetriclaplace"
     ndim_supp = 0
     ndims_params = [0, 0, 0]
     dtype = "floatX"
     _print_name = ("AsymmetricLaplace", "\\operatorname{AsymmetricLaplace}")
@@ -1926,14 +1942,24 @@
         return check_parameters(
             res,
             alpha > 0,
             m > 0,
             msg="alpha > 0, m > 0",
         )
 
+    def icdf(value, alpha, m):
+        res = m * pt.pow(1 - value, -1 / alpha)
+        res = check_icdf_value(res, value)
+        return check_icdf_parameters(
+            res,
+            alpha > 0,
+            m > 0,
+            msg="alpha > 0, m > 0",
+        )
+
 
 @_default_transform.register(Pareto)
 def pareto_default_transform(op, rv):
     return bounded_cont_transform(op, rv, Pareto.bound_args_indices)
 
 
 class Cauchy(Continuous):
```

### Comparing `pymc-5.3.1/pymc/distributions/discrete.py` & `pymc-5.4.0/pymc/distributions/discrete.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,33 +42,26 @@
     factln,
     log_diff_normal_cdf,
     logpow,
     normal_lccdf,
     normal_lcdf,
 )
 from pymc.distributions.distribution import Discrete
-from pymc.distributions.mixture import Mixture
 from pymc.distributions.shape_utils import rv_size_is_none
-from pymc.logprob.basic import logp
+from pymc.logprob.basic import logcdf, logp
 from pymc.math import sigmoid
 from pymc.pytensorf import floatX, intX
-from pymc.vartypes import continuous_types
 
 __all__ = [
     "Binomial",
     "BetaBinomial",
     "Bernoulli",
     "DiscreteWeibull",
     "Poisson",
     "NegativeBinomial",
-    "DiracDelta",
-    "Constant",
-    "ZeroInflatedPoisson",
-    "ZeroInflatedBinomial",
-    "ZeroInflatedNegativeBinomial",
     "DiscreteUniform",
     "Geometric",
     "HyperGeometric",
     "Categorical",
     "OrderedLogistic",
     "OrderedProbit",
 ]
@@ -819,14 +812,18 @@
             0 <= p,
             p <= 1,
             msg="0 <= p <= 1",
         )
 
     def icdf(value, p):
         res = pt.ceil(pt.log1p(-value) / pt.log1p(-p)).astype("int64")
+        res_1m = pt.maximum(res - 1, 0)
+        dist = pm.Geometric.dist(p=p)
+        value_1m = pt.exp(logcdf(dist, res_1m))
+        res = pt.switch(value_1m >= value, res_1m, res)
         res = check_icdf_value(res, value)
         return check_icdf_parameters(
             res,
             0 <= p,
             p <= 1,
             msg="0 <= p <= 1",
         )
@@ -1056,14 +1053,19 @@
             res,
             lower <= upper,
             msg="lower <= upper",
         )
 
     def icdf(value, lower, upper):
         res = pt.ceil(value * (upper - lower + 1)).astype("int64") + lower - 1
+        res_1m = pt.maximum(res - 1, lower)
+        dist = pm.DiscreteUniform.dist(lower=lower, upper=upper)
+        value_1m = pt.exp(logcdf(dist, res_1m))
+        res = pt.switch(value_1m >= value, res_1m, res)
+
         res = check_icdf_value(res, value)
         return check_icdf_parameters(
             res,
             lower <= upper,
             msg="lower <= upper",
         )
 
@@ -1171,338 +1173,14 @@
             0 <= p_,
             p_ <= 1,
             pt.isclose(pt.sum(p, axis=-1), 1),
             msg="0 <= p <=1, sum(p) = 1",
         )
 
 
-class DiracDeltaRV(RandomVariable):
-    name = "diracdelta"
-    ndim_supp = 0
-    ndims_params = [0]
-    _print_name = ("DiracDelta", "\\operatorname{DiracDelta}")
-
-    def make_node(self, rng, size, dtype, c):
-        c = pt.as_tensor_variable(c)
-        return super().make_node(rng, size, c.dtype, c)
-
-    @classmethod
-    def rng_fn(cls, rng, c, size=None):
-        if size is None:
-            return c.copy()
-        return np.full(size, c)
-
-
-diracdelta = DiracDeltaRV()
-
-
-class DiracDelta(Discrete):
-    r"""
-    DiracDelta log-likelihood.
-
-    Parameters
-    ----------
-    c : tensor_like of float or int
-        Dirac Delta parameter. The dtype of `c` determines the dtype of the distribution.
-        This can affect which sampler is assigned to DiracDelta variables, or variables
-        that use DiracDelta, such as Mixtures.
-    """
-
-    rv_op = diracdelta
-
-    @classmethod
-    def dist(cls, c, *args, **kwargs):
-        c = pt.as_tensor_variable(c)
-        if c.dtype in continuous_types:
-            c = floatX(c)
-        return super().dist([c], **kwargs)
-
-    def moment(rv, size, c):
-        if not rv_size_is_none(size):
-            c = pt.full(size, c)
-        return c
-
-    def logp(value, c):
-        return pt.switch(
-            pt.eq(value, c),
-            pt.zeros_like(value),
-            -np.inf,
-        )
-
-    def logcdf(value, c):
-        return pt.switch(
-            pt.lt(value, c),
-            -np.inf,
-            0,
-        )
-
-
-class Constant:
-    def __new__(cls, *args, **kwargs):
-        warnings.warn(
-            "pm.Constant has been deprecated. Use pm.DiracDelta instead.",
-            FutureWarning,
-        )
-        return DiracDelta(*args, **kwargs)
-
-    @classmethod
-    def dist(cls, *args, **kwargs):
-        warnings.warn(
-            "pm.Constant has been deprecated. Use pm.DiracDelta instead.",
-            FutureWarning,
-        )
-        return DiracDelta.dist(*args, **kwargs)
-
-
-def _zero_inflated_mixture(*, name, nonzero_p, nonzero_dist, **kwargs):
-    """Helper function to create a zero-inflated mixture
-
-    If name is `None`, this function returns an unregistered variable
-    """
-    nonzero_p = pt.as_tensor_variable(floatX(nonzero_p))
-    weights = pt.stack([1 - nonzero_p, nonzero_p], axis=-1)
-    comp_dists = [
-        DiracDelta.dist(0),
-        nonzero_dist,
-    ]
-    if name is not None:
-        return Mixture(name, weights, comp_dists, **kwargs)
-    else:
-        return Mixture.dist(weights, comp_dists, **kwargs)
-
-
-class ZeroInflatedPoisson:
-    R"""
-    Zero-inflated Poisson log-likelihood.
-
-    Often used to model the number of events occurring in a fixed period
-    of time when the times at which events occur are independent.
-    The pmf of this distribution is
-
-    .. math::
-
-        f(x \mid \psi, \mu) = \left\{ \begin{array}{l}
-            (1-\psi) + \psi e^{-\mu}, \text{if } x = 0 \\
-            \psi \frac{e^{-\mu}\mu^x}{x!}, \text{if } x=1,2,3,\ldots
-            \end{array} \right.
-
-    .. plot::
-        :context: close-figs
-
-        import matplotlib.pyplot as plt
-        import numpy as np
-        import scipy.stats as st
-        import arviz as az
-        plt.style.use('arviz-darkgrid')
-        x = np.arange(0, 22)
-        psis = [0.7, 0.4]
-        mus = [8, 4]
-        for psi, mu in zip(psis, mus):
-            pmf = st.poisson.pmf(x, mu)
-            pmf[0] = (1 - psi) + pmf[0]
-            pmf[1:] =  psi * pmf[1:]
-            pmf /= pmf.sum()
-            plt.plot(x, pmf, '-o', label='$\\psi$ = {}, $\\mu$ = {}'.format(psi, mu))
-        plt.xlabel('x', fontsize=12)
-        plt.ylabel('f(x)', fontsize=12)
-        plt.legend(loc=1)
-        plt.show()
-
-    ========  ==========================
-    Support   :math:`x \in \mathbb{N}_0`
-    Mean      :math:`\psi\mu`
-    Variance  :math:`\mu + \frac{1-\psi}{\psi}\mu^2`
-    ========  ==========================
-
-    Parameters
-    ----------
-    psi : tensor_like of float
-        Expected proportion of Poisson variates (0 < psi < 1)
-    mu : tensor_like of float
-        Expected number of occurrences during the given interval
-        (mu >= 0).
-    """
-
-    def __new__(cls, name, psi, mu, **kwargs):
-        return _zero_inflated_mixture(
-            name=name, nonzero_p=psi, nonzero_dist=Poisson.dist(mu=mu), **kwargs
-        )
-
-    @classmethod
-    def dist(cls, psi, mu, **kwargs):
-        return _zero_inflated_mixture(
-            name=None, nonzero_p=psi, nonzero_dist=Poisson.dist(mu=mu), **kwargs
-        )
-
-
-class ZeroInflatedBinomial:
-    R"""
-    Zero-inflated Binomial log-likelihood.
-
-    The pmf of this distribution is
-
-    .. math::
-
-        f(x \mid \psi, n, p) = \left\{ \begin{array}{l}
-            (1-\psi) + \psi (1-p)^{n}, \text{if } x = 0 \\
-            \psi {n \choose x} p^x (1-p)^{n-x}, \text{if } x=1,2,3,\ldots,n
-            \end{array} \right.
-
-    .. plot::
-        :context: close-figs
-
-        import matplotlib.pyplot as plt
-        import numpy as np
-        import scipy.stats as st
-        import arviz as az
-        plt.style.use('arviz-darkgrid')
-        x = np.arange(0, 25)
-        ns = [10, 20]
-        ps = [0.5, 0.7]
-        psis = [0.7, 0.4]
-        for n, p, psi in zip(ns, ps, psis):
-            pmf = st.binom.pmf(x, n, p)
-            pmf[0] = (1 - psi) + pmf[0]
-            pmf[1:] =  psi * pmf[1:]
-            pmf /= pmf.sum()
-            plt.plot(x, pmf, '-o', label='n = {}, p = {}, $\\psi$ = {}'.format(n, p, psi))
-        plt.xlabel('x', fontsize=12)
-        plt.ylabel('f(x)', fontsize=12)
-        plt.legend(loc=1)
-        plt.show()
-
-    ========  ==========================
-    Support   :math:`x \in \mathbb{N}_0`
-    Mean      :math:`\psi n p`
-    Variance  :math:`(1-\psi) n p [1 - p(1 - \psi n)].`
-    ========  ==========================
-
-    Parameters
-    ----------
-    psi : tensor_like of float
-        Expected proportion of Binomial variates (0 < psi < 1)
-    n : tensor_like of int
-        Number of Bernoulli trials (n >= 0).
-    p : tensor_like of float
-        Probability of success in each trial (0 < p < 1).
-
-    """
-
-    def __new__(cls, name, psi, n, p, **kwargs):
-        return _zero_inflated_mixture(
-            name=name, nonzero_p=psi, nonzero_dist=Binomial.dist(n=n, p=p), **kwargs
-        )
-
-    @classmethod
-    def dist(cls, psi, n, p, **kwargs):
-        return _zero_inflated_mixture(
-            name=None, nonzero_p=psi, nonzero_dist=Binomial.dist(n=n, p=p), **kwargs
-        )
-
-
-class ZeroInflatedNegativeBinomial:
-    R"""
-    Zero-Inflated Negative binomial log-likelihood.
-
-    The Zero-inflated version of the Negative Binomial (NB).
-    The NB distribution describes a Poisson random variable
-    whose rate parameter is gamma distributed.
-    The pmf of this distribution is
-
-    .. math::
-
-       f(x \mid \psi, \mu, \alpha) = \left\{
-         \begin{array}{l}
-           (1-\psi) + \psi \left (
-             \frac{\alpha}{\alpha+\mu}
-           \right) ^\alpha, \text{if } x = 0 \\
-           \psi \frac{\Gamma(x+\alpha)}{x! \Gamma(\alpha)} \left (
-             \frac{\alpha}{\mu+\alpha}
-           \right)^\alpha \left(
-             \frac{\mu}{\mu+\alpha}
-           \right)^x, \text{if } x=1,2,3,\ldots
-         \end{array}
-       \right.
-
-    .. plot::
-        :context: close-figs
-
-        import matplotlib.pyplot as plt
-        import numpy as np
-        import scipy.stats as st
-        from scipy import special
-        import arviz as az
-        plt.style.use('arviz-darkgrid')
-
-        def ZeroInfNegBinom(a, m, psi, x):
-            pmf = special.binom(x + a - 1, x) * (a / (m + a))**a * (m / (m + a))**x
-            pmf[0] = (1 - psi) + pmf[0]
-            pmf[1:] =  psi * pmf[1:]
-            pmf /= pmf.sum()
-            return pmf
-
-        x = np.arange(0, 25)
-        alphas = [2, 4]
-        mus = [2, 8]
-        psis = [0.7, 0.7]
-        for a, m, psi in zip(alphas, mus, psis):
-            pmf = ZeroInfNegBinom(a, m, psi, x)
-            plt.plot(x, pmf, '-o', label=r'$\alpha$ = {}, $\mu$ = {}, $\psi$ = {}'.format(a, m, psi))
-        plt.xlabel('x', fontsize=12)
-        plt.ylabel('f(x)', fontsize=12)
-        plt.legend(loc=1)
-        plt.show()
-
-    ========  ==========================
-    Support   :math:`x \in \mathbb{N}_0`
-    Mean      :math:`\psi\mu`
-    Var       :math:`\psi\mu +  \left (1 + \frac{\mu}{\alpha} + \frac{1-\psi}{\mu} \right)`
-    ========  ==========================
-
-    The zero inflated negative binomial distribution can be parametrized
-    either in terms of mu or p, and either in terms of alpha or n.
-    The link between the parametrizations is given by
-
-    .. math::
-
-        \mu &= \frac{n(1-p)}{p} \\
-        \alpha &= n
-
-    Parameters
-    ----------
-    psi : tensor_like of float
-        Expected proportion of NegativeBinomial variates (0 < psi < 1)
-    mu : tensor_like of float
-        Poisson distribution parameter (mu > 0).
-    alpha : tensor_like of float
-        Gamma distribution parameter (alpha > 0).
-    p : tensor_like of float
-        Alternative probability of success in each trial (0 < p < 1).
-    n : tensor_like of float
-        Alternative number of target success trials (n > 0)
-    """
-
-    def __new__(cls, name, psi, mu=None, alpha=None, p=None, n=None, **kwargs):
-        return _zero_inflated_mixture(
-            name=name,
-            nonzero_p=psi,
-            nonzero_dist=NegativeBinomial.dist(mu=mu, alpha=alpha, p=p, n=n),
-            **kwargs,
-        )
-
-    @classmethod
-    def dist(cls, psi, mu=None, alpha=None, p=None, n=None, **kwargs):
-        return _zero_inflated_mixture(
-            name=None,
-            nonzero_p=psi,
-            nonzero_dist=NegativeBinomial.dist(mu=mu, alpha=alpha, p=p, n=n),
-            **kwargs,
-        )
-
-
 class _OrderedLogistic(Categorical):
     r"""
     Underlying class for ordered logistic distributions.
     See docs for the OrderedLogistic wrapper class for more details on how to use it in models.
     """
     rv_op = categorical
```

### Comparing `pymc-5.3.1/pymc/distributions/dist_math.py` & `pymc-5.4.0/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/distribution.py` & `pymc-5.4.0/pymc/distributions/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,34 +41,36 @@
     Dims,
     Shape,
     _change_dist_size,
     convert_dims,
     convert_shape,
     convert_size,
     find_size,
+    rv_size_is_none,
     shape_from_dims,
 )
 from pymc.exceptions import BlockModelAccessError
 from pymc.logprob.abstract import (
     MeasurableVariable,
     _get_measurable_outputs,
     _icdf,
     _logcdf,
     _logprob,
 )
 from pymc.logprob.rewriting import logprob_rewrites_db
 from pymc.model import BlockModelAccess
 from pymc.printing import str_for_dist
-from pymc.pytensorf import collect_default_updates, convert_observed_data
+from pymc.pytensorf import collect_default_updates, convert_observed_data, floatX
 from pymc.util import UNSET, _add_future_warning_tag
-from pymc.vartypes import string_types
+from pymc.vartypes import continuous_types, string_types
 
 __all__ = [
     "CustomDist",
     "DensityDist",
+    "DiracDelta",
     "Distribution",
     "Continuous",
     "Discrete",
     "SymbolicRandomVariable",
 ]
 
 DIST_PARAMETER_TYPES: TypeAlias = Union[np.ndarray, int, float, TensorVariable]
@@ -590,15 +592,15 @@
     default_output = -1
 
     _print_name = ("CustomSymbolicDist", "\\operatorname{CustomSymbolicDist}")
 
     def update(self, node: Node):
         op = node.op
         inner_updates = collect_default_updates(
-            op.inner_inputs, op.inner_outputs, must_be_shared=False
+            inputs=op.inner_inputs, outputs=op.inner_outputs, must_be_shared=False
         )
 
         # Map inner updates to outer inputs/outputs
         updates = {}
         for rng, update in inner_updates.items():
             inp_idx = op.inner_inputs.index(rng)
             out_idx = op.inner_outputs.index(update)
@@ -662,15 +664,15 @@
         dummy_size_param = size.type()
         dummy_dist_params = [dist_param.type() for dist_param in dist_params]
         with BlockModelAccess(
             error_msg_on_access="Model variables cannot be created in the dist function. Use the `.dist` API"
         ):
             dummy_rv = dist(*dummy_dist_params, dummy_size_param)
         dummy_params = [dummy_size_param] + dummy_dist_params
-        dummy_updates_dict = collect_default_updates(dummy_params, (dummy_rv,))
+        dummy_updates_dict = collect_default_updates(inputs=dummy_params, outputs=(dummy_rv,))
 
         rv_type = type(
             class_name,
             (CustomSymbolicDistRV,),
             # If logp is not provided, we try to infer it from the dist graph
             dict(
                 inline_logprob=logp is None,
@@ -707,15 +709,15 @@
             old_size, *old_dist_params = node.inputs[: len(dist_params) + 1]
 
             # OpFromGraph has to be recreated if the size type changes!
             dummy_size_param = new_size.type()
             dummy_dist_params = [dist_param.type() for dist_param in old_dist_params]
             dummy_rv = dist(*dummy_dist_params, dummy_size_param)
             dummy_params = [dummy_size_param] + dummy_dist_params
-            dummy_updates_dict = collect_default_updates(dummy_params, (dummy_rv,))
+            dummy_updates_dict = collect_default_updates(inputs=dummy_params, outputs=(dummy_rv,))
             new_rv_op = rv_type(
                 inputs=dummy_params,
                 outputs=[*dummy_updates_dict.values(), dummy_rv],
                 ndim_supp=ndim_supp,
             )
             new_rv = new_rv_op(new_size, *dist_params)
 
@@ -1101,7 +1103,68 @@
         return pt.zeros_like(rv)
     else:
         raise TypeError(
             "Cannot safely infer the size of a multivariate random variable's moment. "
             f"Please provide a moment function when instantiating the {rv_name} "
             "random variable."
         )
+
+
+class DiracDeltaRV(RandomVariable):
+    name = "diracdelta"
+    ndim_supp = 0
+    ndims_params = [0]
+    _print_name = ("DiracDelta", "\\operatorname{DiracDelta}")
+
+    def make_node(self, rng, size, dtype, c):
+        c = pt.as_tensor_variable(c)
+        return super().make_node(rng, size, c.dtype, c)
+
+    @classmethod
+    def rng_fn(cls, rng, c, size=None):
+        if size is None:
+            return c.copy()
+        return np.full(size, c)
+
+
+diracdelta = DiracDeltaRV()
+
+
+class DiracDelta(Discrete):
+    r"""
+    DiracDelta log-likelihood.
+
+    Parameters
+    ----------
+    c : tensor_like of float or int
+        Dirac Delta parameter. The dtype of `c` determines the dtype of the distribution.
+        This can affect which sampler is assigned to DiracDelta variables, or variables
+        that use DiracDelta, such as Mixtures.
+    """
+
+    rv_op = diracdelta
+
+    @classmethod
+    def dist(cls, c, *args, **kwargs):
+        c = pt.as_tensor_variable(c)
+        if c.dtype in continuous_types:
+            c = floatX(c)
+        return super().dist([c], **kwargs)
+
+    def moment(rv, size, c):
+        if not rv_size_is_none(size):
+            c = pt.full(size, c)
+        return c
+
+    def logp(value, c):
+        return pt.switch(
+            pt.eq(value, c),
+            pt.zeros_like(value),
+            -np.inf,
+        )
+
+    def logcdf(value, c):
+        return pt.switch(
+            pt.lt(value, c),
+            -np.inf,
+            0,
+        )
```

### Comparing `pymc-5.3.1/pymc/distributions/multivariate.py` & `pymc-5.4.0/pymc/distributions/multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/shape_utils.py` & `pymc-5.4.0/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/simulator.py` & `pymc-5.4.0/pymc/distributions/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from pymc.distributions.distribution import Distribution, _moment
 from pymc.logprob.abstract import _logprob
 from pymc.pytensorf import floatX
 
 __all__ = ["Simulator"]
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 
 class SimulatorRV(RandomVariable):
     """
     Base class for SimulatorRVs
 
     This should be subclassed when defining custom Simulator objects.
```

### Comparing `pymc-5.3.1/pymc/distributions/timeseries.py` & `pymc-5.4.0/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/transforms.py` & `pymc-5.4.0/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/distributions/truncated.py` & `pymc-5.4.0/pymc/distributions/truncated.py`

 * *Files 10% similar despite different names*

```diff
@@ -348,14 +348,58 @@
             pt.le(lower, upper),
             msg="lower_bound <= upper_bound",
         )
 
     return logp
 
 
+@_logcdf.register(TruncatedRV)
+def truncated_logcdf(op, value, *inputs, **kwargs):
+    *rv_inputs, lower, upper, rng = inputs
+    rv_inputs = [rng, *rv_inputs]
+
+    base_rv_op = op.base_rv_op
+    logcdf = _logcdf(base_rv_op, value, *rv_inputs, **kwargs)
+
+    # For left truncated discrete RVs, we don't want to include the lower bound in the
+    # normalization term
+    lower_value = lower - 1 if base_rv_op.dtype.startswith("int") else lower
+    lower_logcdf = _logcdf(base_rv_op, lower_value, *rv_inputs, **kwargs)
+    upper_logcdf = _logcdf(base_rv_op, upper, *rv_inputs, **kwargs)
+
+    is_lower_bounded = not (isinstance(lower, TensorConstant) and np.all(np.isneginf(lower.value)))
+    is_upper_bounded = not (isinstance(upper, TensorConstant) and np.all(np.isinf(upper.value)))
+
+    lognorm = 0
+    if is_lower_bounded and is_upper_bounded:
+        lognorm = logdiffexp(upper_logcdf, lower_logcdf)
+    elif is_lower_bounded:
+        lognorm = pt.log1mexp(lower_logcdf)
+    elif is_upper_bounded:
+        lognorm = upper_logcdf
+
+    logcdf_numerator = logdiffexp(logcdf, lower_logcdf) if is_lower_bounded else logcdf
+    logcdf_trunc = logcdf_numerator - lognorm
+
+    if is_lower_bounded:
+        logcdf_trunc = pt.switch(value < lower, -np.inf, logcdf_trunc)
+
+    if is_upper_bounded:
+        logcdf_trunc = pt.switch(value <= upper, logcdf_trunc, 0.0)
+
+    if is_lower_bounded and is_upper_bounded:
+        logcdf_trunc = check_parameters(
+            logcdf_trunc,
+            pt.le(lower, upper),
+            msg="lower_bound <= upper_bound",
+        )
+
+    return logcdf_trunc
+
+
 @_truncated.register(NormalRV)
 def _truncated_normal(op, lower, upper, size, rng, old_size, dtype, mu, sigma):
     return TruncatedNormal.dist(
         mu=mu,
         sigma=sigma,
         lower=lower,
         upper=upper,
```

### Comparing `pymc-5.3.1/pymc/exceptions.py` & `pymc-5.4.0/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/func_utils.py` & `pymc-5.4.0/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/gp/__init__.py` & `pymc-5.4.0/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/gp/cov.py` & `pymc-5.4.0/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/gp/gp.py` & `pymc-5.4.0/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/gp/hsgp_approx.py` & `pymc-5.4.0/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/gp/mean.py` & `pymc-5.4.0/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/gp/util.py` & `pymc-5.4.0/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/initial_point.py` & `pymc-5.4.0/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/__init__.py` & `pymc-5.4.0/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/abstract.py` & `pymc-5.4.0/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/basic.py` & `pymc-5.4.0/pymc/logprob/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/binary.py` & `pymc-5.4.0/pymc/logprob/binary.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import numpy as np
 import pytensor.tensor as pt
 
 from pytensor.graph.basic import Node
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.rewriting.basic import node_rewriter
-from pytensor.scalar.basic import GE, GT, LE, LT
+from pytensor.scalar.basic import GE, GT, LE, LT, Invert
 from pytensor.tensor import TensorVariable
-from pytensor.tensor.math import ge, gt, le, lt
+from pytensor.tensor.math import ge, gt, invert, le, lt
 
 from pymc.logprob.abstract import (
     MeasurableElemwise,
     MeasurableVariable,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
@@ -132,7 +132,61 @@
             return pt.switch(condn_exp, pt.logaddexp(logccdf, logpmf), logcdf_prev)
 
     if base_rv_op.name:
         logprob.name = f"{base_rv_op}_logprob"
         logcdf.name = f"{base_rv_op}_logcdf"
 
     return logprob
+
+
+class MeasurableBitwise(MeasurableElemwise):
+    """A placeholder used to specify a log-likelihood for a bitwise operation RV sub-graph."""
+
+    valid_scalar_types = (Invert,)
+
+
+@node_rewriter(tracks=[invert])
+def find_measurable_bitwise(fgraph: FunctionGraph, node: Node) -> Optional[List[MeasurableBitwise]]:
+    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    if rv_map_feature is None:
+        return None  # pragma: no cover
+
+    if isinstance(node.op, MeasurableBitwise):
+        return None  # pragma: no cover
+
+    base_var = node.inputs[0]
+    if not (
+        base_var.owner
+        and isinstance(base_var.owner.op, MeasurableVariable)
+        and base_var not in rv_map_feature.rv_values
+    ):
+        return None
+
+    if not base_var.dtype.startswith("bool"):
+        raise None
+
+    # Make base_var unmeasurable
+    unmeasurable_base_var = ignore_logprob(base_var)
+
+    node_scalar_op = node.op.scalar_op
+
+    bitwise_op = MeasurableBitwise(node_scalar_op)
+    bitwise_rv = bitwise_op.make_node(unmeasurable_base_var).default_output()
+    bitwise_rv.name = node.outputs[0].name
+    return [bitwise_rv]
+
+
+measurable_ir_rewrites_db.register(
+    "find_measurable_bitwise",
+    find_measurable_bitwise,
+    "basic",
+    "bitwise",
+)
+
+
+@_logprob.register(MeasurableBitwise)
+def bitwise_not_logprob(op, values, base_rv, **kwargs):
+    (value,) = values
+
+    logprob = _logprob_helper(base_rv, invert(value), **kwargs)
+
+    return logprob
```

### Comparing `pymc-5.3.1/pymc/logprob/censoring.py` & `pymc-5.4.0/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/checks.py` & `pymc-5.4.0/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/cumsum.py` & `pymc-5.4.0/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/mixture.py` & `pymc-5.4.0/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/rewriting.py` & `pymc-5.4.0/pymc/logprob/rewriting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/scan.py` & `pymc-5.4.0/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/tensor.py` & `pymc-5.4.0/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/logprob/transforms.py` & `pymc-5.4.0/pymc/logprob/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,36 +38,58 @@
 
 from copy import copy
 from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pytensor.tensor as pt
 
+from pytensor import scan
 from pytensor.gradient import DisconnectedType, jacobian
 from pytensor.graph.basic import Apply, Node, Variable
 from pytensor.graph.features import AlreadyThere, Feature
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.op import Op
 from pytensor.graph.replace import clone_replace
 from pytensor.graph.rewriting.basic import GraphRewriter, in2out, node_rewriter
-from pytensor.scalar import Abs, Add, Exp, Log, Mul, Pow, Sqr, Sqrt
+from pytensor.scalar import (
+    Abs,
+    Add,
+    Cosh,
+    Erf,
+    Erfc,
+    Erfcx,
+    Exp,
+    Log,
+    Mul,
+    Pow,
+    Sinh,
+    Sqr,
+    Sqrt,
+    Tanh,
+)
 from pytensor.scan.op import Scan
 from pytensor.tensor.exceptions import NotScalarConstantError
 from pytensor.tensor.math import (
     abs,
     add,
+    cosh,
+    erf,
+    erfc,
+    erfcx,
     exp,
     log,
     mul,
     neg,
     pow,
     reciprocal,
+    sinh,
     sqr,
     sqrt,
     sub,
+    tanh,
     true_div,
 )
 from pytensor.tensor.rewriting.basic import (
     register_specialize,
     register_stabilize,
     register_useless,
 )
@@ -118,33 +140,39 @@
 @node_rewriter([TransformedVariable])
 def remove_TransformedVariables(fgraph, node):
     if isinstance(node.op, TransformedVariable):
         return [node.inputs[0]]
 
 
 class RVTransform(abc.ABC):
+    ndim_supp = None
+
     @abc.abstractmethod
     def forward(self, value: TensorVariable, *inputs: Variable) -> TensorVariable:
         """Apply the transformation."""
 
     @abc.abstractmethod
     def backward(
         self, value: TensorVariable, *inputs: Variable
     ) -> Union[TensorVariable, Tuple[TensorVariable, ...]]:
         """Invert the transformation. Multiple values may be returned when the
         transformation is not 1-to-1"""
 
     def log_jac_det(self, value: TensorVariable, *inputs) -> TensorVariable:
         """Construct the log of the absolute value of the Jacobian determinant."""
-        # jac = pt.reshape(
-        #     gradient(pt.sum(self.backward(value, *inputs)), [value]), value.shape
-        # )
-        # return pt.log(pt.abs(jac))
-        phi_inv = self.backward(value, *inputs)
-        return pt.log(pt.abs(pt.nlinalg.det(pt.atleast_2d(jacobian(phi_inv, [value])[0]))))
+        if self.ndim_supp not in (0, 1):
+            raise NotImplementedError(
+                f"RVTransform default log_jac_det only implemented for ndim_supp in (0, 1), got {self.ndim_supp=}"
+            )
+        if self.ndim_supp == 0:
+            jac = pt.reshape(pt.grad(pt.sum(self.backward(value, *inputs)), [value]), value.shape)
+            return pt.log(pt.abs(jac))
+        else:
+            phi_inv = self.backward(value, *inputs)
+            return pt.log(pt.abs(pt.nlinalg.det(pt.atleast_2d(jacobian(phi_inv, [value])[0]))))
 
 
 @node_rewriter(tracks=None)
 def transform_values(fgraph: FunctionGraph, node: Node) -> Optional[List[Node]]:
     """Apply transforms to value variables.
 
     It is assumed that the input value variables correspond to forward
@@ -336,15 +364,15 @@
         self.transform_rewrite.rewrite(fgraph)
         self.scan_transform_rewrite.rewrite(fgraph)
 
 
 class MeasurableTransform(MeasurableElemwise):
     """A placeholder used to specify a log-likelihood for a transformed measurable variable"""
 
-    valid_scalar_types = (Exp, Log, Add, Mul, Pow, Abs)
+    valid_scalar_types = (Exp, Log, Add, Mul, Pow, Abs, Sinh, Cosh, Tanh, Erf, Erfc, Erfcx)
 
     # Cannot use `transform` as name because it would clash with the property added by
     # the `TransformValuesRewrite`
     transform_elemwise: RVTransform
     measurable_input_idx: int
 
     def __init__(self, *args, transform: RVTransform, measurable_input_idx: int, **kwargs):
@@ -536,15 +564,15 @@
     if all(measurable_var in rv_map_feature.rv_values for measurable_var in measurable_vars):
         return None  # pragma: no cover
 
     minuend, subtrahend = node.inputs
     return [pt.add(minuend, pt.neg(subtrahend))]
 
 
-@node_rewriter([exp, log, add, mul, pow, abs])
+@node_rewriter([exp, log, add, mul, pow, abs, sinh, cosh, tanh, erf, erfc, erfcx])
 def find_measurable_transforms(fgraph: FunctionGraph, node: Node) -> Optional[List[Node]]:
     """Find measurable transformations from Elemwise operators."""
 
     # Node was already converted
     if isinstance(node.op, MeasurableVariable):
         return None  # pragma: no cover
 
@@ -581,21 +609,28 @@
     # This seems to be the only thing preventing nested rewrites from being erased
     measurable_input = ignore_logprob(measurable_input)
 
     scalar_op = node.op.scalar_op
     measurable_input_idx = 0
     transform_inputs: Tuple[TensorVariable, ...] = (measurable_input,)
     transform: RVTransform
-    if isinstance(scalar_op, Exp):
-        transform = ExpTransform()
-    elif isinstance(scalar_op, Log):
-        transform = LogTransform()
-    elif isinstance(scalar_op, Abs):
-        transform = AbsTransform()
-    elif isinstance(scalar_op, Pow):
+
+    transform_dict = {
+        Exp: ExpTransform(),
+        Log: LogTransform(),
+        Abs: AbsTransform(),
+        Sinh: SinhTransform(),
+        Cosh: CoshTransform(),
+        Tanh: TanhTransform(),
+        Erf: ErfTransform(),
+        Erfc: ErfcTransform(),
+        Erfcx: ErfcxTransform(),
+    }
+    transform = transform_dict.get(type(scalar_op), None)
+    if isinstance(scalar_op, Pow):
         # We only allow for the base to be measurable
         if measurable_input_idx != 0:
             return None
         try:
             (power,) = other_inputs
             power = pt.get_underlying_scalar_constant_value(power).item()
         # Power needs to be a constant
@@ -604,15 +639,15 @@
         transform_inputs = (measurable_input, power)
         transform = PowerTransform(power=power)
     elif isinstance(scalar_op, Add):
         transform_inputs = (measurable_input, pt.add(*other_inputs))
         transform = LocTransform(
             transform_args_fn=lambda *inputs: inputs[-1],
         )
-    else:
+    elif transform is None:
         transform_inputs = (measurable_input, pt.mul(*other_inputs))
         transform = ScaleTransform(
             transform_args_fn=lambda *inputs: inputs[-1],
         )
 
     transform_op = MeasurableTransform(
         scalar_op=scalar_op,
@@ -667,14 +702,95 @@
     "find_measurable_transforms",
     find_measurable_transforms,
     "basic",
     "transform",
 )
 
 
+class SinhTransform(RVTransform):
+    name = "sinh"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.sinh(value)
+
+    def backward(self, value, *inputs):
+        return pt.arcsinh(value)
+
+
+class CoshTransform(RVTransform):
+    name = "cosh"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.cosh(value)
+
+    def backward(self, value, *inputs):
+        return pt.arccosh(value)
+
+
+class TanhTransform(RVTransform):
+    name = "tanh"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.tanh(value)
+
+    def backward(self, value, *inputs):
+        return pt.arctanh(value)
+
+
+class ErfTransform(RVTransform):
+    name = "erf"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.erf(value)
+
+    def backward(self, value, *inputs):
+        return pt.erfinv(value)
+
+
+class ErfcTransform(RVTransform):
+    name = "erfc"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.erfc(value)
+
+    def backward(self, value, *inputs):
+        return pt.erfcinv(value)
+
+
+class ErfcxTransform(RVTransform):
+    name = "erfcx"
+    ndim_supp = 0
+
+    def forward(self, value, *inputs):
+        return pt.erfcx(value)
+
+    def backward(self, value, *inputs):
+        # computes the inverse of erfcx, this was adapted from
+        # https://tinyurl.com/4mxfd3cz
+        x = pt.switch(value <= 1, 1.0 / (value * pt.sqrt(np.pi)), -pt.sqrt(pt.log(value)))
+
+        def calc_delta_x(value, prior_result):
+            return prior_result - (pt.erfcx(prior_result) - value) / (
+                2 * prior_result * pt.erfcx(prior_result) - 2 / pt.sqrt(np.pi)
+            )
+
+        result, updates = scan(
+            fn=calc_delta_x,
+            outputs_info=pt.ones_like(x),
+            non_sequences=value,
+            n_steps=10,
+        )
+        return result[-1]
+
+
 class LocTransform(RVTransform):
     name = "loc"
 
     def __init__(self, transform_args_fn):
         self.transform_args_fn = transform_args_fn
 
     def forward(self, value, *inputs):
```

### Comparing `pymc-5.3.1/pymc/logprob/utils.py` & `pymc-5.4.0/pymc/logprob/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 ) -> List[TensorVariable]:
     """Return duplicated variables that are ignored when creating logprob graphs.
 
     This function keeps any interdependencies between variables intact, after
     making each "unmeasurable", whereas a sequential call to `ignore_logprob`
     would not do this correctly.
     """
-    from pymc.pytensorf import _replace_rvs_in_graphs
+    from pymc.pytensorf import _replace_vars_in_graphs
 
     measurable_vars_to_unmeasurable_vars = {
         measurable_var: ignore_logprob(measurable_var) for measurable_var in vars
     }
 
     def replacement_fn(var, replacements):
         if var in measurable_vars_to_unmeasurable_vars:
@@ -349,9 +349,9 @@
         # We don't want to clone valued nodes. Assigning a var to itself in the
         # replacements prevents this
         elif var in rvs_to_values:
             replacements[var] = var
 
         return []
 
-    unmeasurable_vars, _ = _replace_rvs_in_graphs(graphs=vars, replacement_fn=replacement_fn)
+    unmeasurable_vars, _ = _replace_vars_in_graphs(graphs=vars, replacement_fn=replacement_fn)
     return unmeasurable_vars
```

### Comparing `pymc-5.3.1/pymc/math.py` & `pymc-5.4.0/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/model.py` & `pymc-5.4.0/pymc/model.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/model_graph.py` & `pymc-5.4.0/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/ode/__init__.py` & `pymc-5.4.0/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/ode/ode.py` & `pymc-5.4.0/pymc/ode/ode.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pytensor.graph.basic import Apply
 from pytensor.graph.op import Op, get_test_value
 from pytensor.tensor.type import TensorType
 
 from pymc.exceptions import DtypeError, ShapeError
 from pymc.ode import utils
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 floatX = pytensor.config.floatX
 
 
 class DifferentialEquation(Op):
     r"""
     Specify an ordinary differential equation
```

### Comparing `pymc-5.3.1/pymc/ode/utils.py` & `pymc-5.4.0/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/plots/__init__.py` & `pymc-5.4.0/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/printing.py` & `pymc-5.4.0/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/pytensorf.py` & `pymc-5.4.0/pymc/pytensorf.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     clone_get_equiv,
     graph_inputs,
     walk,
 )
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.op import Op
 from pytensor.scalar.basic import Cast
+from pytensor.scan.op import Scan
 from pytensor.tensor.basic import _as_tensor_variable
 from pytensor.tensor.elemwise import Elemwise
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.random.type import RandomType
 from pytensor.tensor.random.var import (
     RandomGeneratorSharedVariable,
     RandomStateSharedVariable,
@@ -201,27 +202,30 @@
             new_vars.extend(reversed(var.owner.inputs))
 
         return new_vars
 
     yield from walk(graphs, expand, bfs=False)
 
 
-def _replace_rvs_in_graphs(
+def _replace_vars_in_graphs(
     graphs: Iterable[TensorVariable],
     replacement_fn: Callable[[TensorVariable], Dict[TensorVariable, TensorVariable]],
     **kwargs,
 ) -> Tuple[List[TensorVariable], Dict[TensorVariable, TensorVariable]]:
-    """Replace random variables in graphs
+    """Replace variables in graphs.
 
     This will *not* recompute test values.
 
     Parameters
     ----------
     graphs
         The graphs in which random variables are to be replaced.
+    replacement_fn
+        A callable called on each graph output that populates a replacement dictionary and returns
+        nodes that should be investigated further.
 
     Returns
     -------
     Tuple containing the transformed graphs and a ``dict`` of the replacements
     that were made.
     """
     replacements = {}
@@ -252,15 +256,16 @@
         )
 
         # replacements have to be done in reverse topological order so that nested
         # expressions get recursively replaced correctly
         toposort = fg.toposort()
         sorted_replacements = sorted(
             tuple(replacements.items()),
-            key=lambda pair: toposort.index(pair[0].owner),
+            # Root inputs don't have owner, we give them negative priority -1
+            key=lambda pair: toposort.index(pair[0].owner) if pair[0].owner is not None else -1,
             reverse=True,
         )
         fg.replace_all(sorted_replacements, import_missing=True)
 
         graphs = list(fg.outputs)
 
     return graphs, replacements
@@ -313,15 +318,15 @@
         return [value_var]
 
     # Clone original graphs
     inputs = [i for i in graph_inputs(graphs) if not isinstance(i, Constant)]
     equiv = clone_get_equiv(inputs, graphs, False, False, {})
     graphs = [equiv[n] for n in graphs]
 
-    graphs, _ = _replace_rvs_in_graphs(
+    graphs, _ = _replace_vars_in_graphs(
         graphs,
         replacement_fn=populate_replacements,
         **kwargs,
     )
 
     return graphs
 
@@ -381,15 +386,15 @@
                 value.name = rv.name
 
         replacements[rv] = value
         # Also walk the graph of the value variable to make any additional
         # replacements if that is not a simple input variable
         return [value]
 
-    graphs, _ = _replace_rvs_in_graphs(
+    graphs, _ = _replace_vars_in_graphs(
         graphs,
         replacement_fn=poulate_replacements,
         **kwargs,
     )
 
     return graphs
 
@@ -996,24 +1001,57 @@
             new_rng = np.random.RandomState(bit_generator)
         else:
             new_rng = np.random.Generator(bit_generator)
         rng.set_value(new_rng, borrow=True)
 
 
 def collect_default_updates(
-    inputs: Sequence[Variable],
     outputs: Sequence[Variable],
+    *,
+    inputs: Optional[Sequence[Variable]] = None,
     must_be_shared: bool = True,
 ) -> Dict[Variable, Variable]:
     """Collect default update expression for shared-variable RNGs used by RVs between inputs and outputs.
 
-    If `must_be_shared` is False, update expressions will also be returned for non-shared input RNGs.
-    This can be useful to obtain the symbolic update expressions from inner graphs.
-    """
+    Parameters
+    ----------
+    outputs: list of PyTensor variables
+        List of variables in which graphs default updates will be collected.
+    inputs: list of PyTensor variables, optional
+        Input nodes above which default updates should not be collected.
+        When not provided, search will include top level inputs (roots).
+    must_be_shared: bool, default True
+        Used internally by PyMC. Whether updates should be collected for non-shared
+        RNG input variables. This is used to collect update expressions for inner graphs.
+
+    Examples
+    --------
+    .. code:: python
+        import pymc as pm
+        from pytensor.scan import scan
+        from pymc.pytensorf import collect_default_updates
 
+        def scan_step(xtm1):
+            x = xtm1 + pm.Normal.dist()
+            x_update = collect_default_updates([x])
+            return x, x_update
+
+        x0 = pm.Normal.dist()
+
+        xs, updates = scan(
+            fn=scan_step,
+            outputs_info=[x0],
+            n_steps=10,
+        )
+
+        # PyMC makes use of the updates to seed xs properly.
+        # Without updates, it would raise an error.
+        xs_draws = pm.draw(xs, draws=10)
+
+    """
     # Avoid circular import
     from pymc.distributions.distribution import SymbolicRandomVariable
 
     def find_default_update(clients, rng: Variable) -> Union[None, Variable]:
         rng_clients = clients.get(rng, None)
 
         # Root case, RNG is not used elsewhere
@@ -1040,24 +1078,39 @@
 
         elif isinstance(client.op, SymbolicRandomVariable):
             # SymbolicRandomVariable have an explicit method that returns an
             # update mapping for their RNG(s)
             next_rng = client.op.update(client).get(rng)
             if next_rng is None:
                 raise ValueError(
-                    f"No update mapping found for RNG used in SymbolicRandomVariable Op {client.op}"
+                    f"No update found for at least one RNG used in SymbolicRandomVariable Op {client.op}"
+                )
+        elif isinstance(client.op, Scan):
+            # Check if any shared output corresponds to the RNG
+            rng_idx = client.inputs.index(rng)
+            io_map = client.op.get_oinp_iinp_iout_oout_mappings()["outer_out_from_outer_inp"]
+            out_idx = io_map.get(rng_idx, -1)
+            if out_idx != -1:
+                next_rng = client.outputs[out_idx]
+            else:  # No break
+                raise ValueError(
+                    f"No update found for at least one RNG used in Scan Op {client.op}.\n"
+                    "You can use `pytensorf.collect_default_updates` inside the Scan function to return updates automatically."
                 )
         else:
-            # We don't know how this RNG should be updated (e.g., Scan).
+            # We don't know how this RNG should be updated (e.g., OpFromGraph).
             # The user should provide an update manually
             return None
 
         # Recurse until we find final update for RNG
         return find_default_update(clients, next_rng)
 
+    if inputs is None:
+        inputs = []
+
     outputs = makeiter(outputs)
     fg = FunctionGraph(outputs=outputs, clone=False)
     clients = fg.clients
 
     rng_updates = {}
     # Iterate over input RNGs. Only consider shared RNGs if `must_be_shared==True`
     for input_rng in (
@@ -1121,15 +1174,15 @@
         Replaces CheckParameterValue assertions is logp expressions. This is used
         as an alteranative to the default local_check_parameter_to_ninf_switch whenenver
         this function is called within a model context and the model `check_bounds` flag
         is set to False.
     """
     # Create an update mapping of RandomVariable's RNG so that it is automatically
     # updated after every function call
-    rng_updates = collect_default_updates(inputs, outputs)
+    rng_updates = collect_default_updates(inputs=inputs, outputs=outputs)
 
     # We always reseed random variables as this provides RNGs with no chances of collision
     if rng_updates:
         reseed_rngs(rng_updates.keys(), random_seed)
 
     # If called inside a model context, see if check_bounds flag is set to False
     try:
```

### Comparing `pymc-5.3.1/pymc/sampling/__init__.py` & `pymc-5.4.0/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/sampling/forward.py` & `pymc-5.4.0/pymc/sampling/forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     "sample_posterior_predictive_w",
 )
 
 
 ArrayLike: TypeAlias = Union[np.ndarray, List[float]]
 PointList: TypeAlias = List[PointType]
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 
 def get_vars_in_point_list(trace, model):
     """Get the list of Variable instances in the model that have values stored in the trace."""
     if not isinstance(trace, MultiTrace):
         names_in_trace = list(trace[0])
     else:
```

### Comparing `pymc-5.3.1/pymc/sampling/jax.py` & `pymc-5.4.0/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/sampling/mcmc.py` & `pymc-5.4.0/pymc/sampling/mcmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,26 @@
 import logging
 import pickle
 import sys
 import time
 import warnings
 
 from collections import defaultdict
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    overload,
+)
 
 import numpy as np
 import pytensor.gradient as tg
 
 from arviz import InferenceData
 from fastprogress.fastprogress import progress_bar
 from typing_extensions import Protocol, TypeAlias
@@ -71,15 +82,15 @@
 class SamplingIteratorCallback(Protocol):
     """Signature of the callable that may be passed to `pm.sample(callable=...)`."""
 
     def __call__(self, trace: IBaseTrace, draw: Draw):
         pass
 
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 
 def instantiate_steppers(
     model, steps: List[Step], selected_steps, step_kwargs=None
 ) -> Union[Step, List[Step]]:
     """Instantiate steppers assigned to the model variables.
 
@@ -314,14 +325,73 @@
 
     else:
         raise ValueError(
             f"Sampler {sampler} not found. Choose one of ['nutpie', 'numpyro', 'blackjax', 'pymc']."
         )
 
 
+@overload
+def sample(
+    draws: int = 1000,
+    *,
+    tune: int = 1000,
+    chains: Optional[int] = None,
+    cores: Optional[int] = None,
+    random_seed: RandomState = None,
+    progressbar: bool = True,
+    step=None,
+    nuts_sampler: str = "pymc",
+    initvals: Optional[Union[StartDict, Sequence[Optional[StartDict]]]] = None,
+    init: str = "auto",
+    jitter_max_retries: int = 10,
+    n_init: int = 200_000,
+    trace: Optional[TraceOrBackend] = None,
+    discard_tuned_samples: bool = True,
+    compute_convergence_checks: bool = True,
+    keep_warning_stat: bool = False,
+    return_inferencedata: Literal[True],
+    idata_kwargs: Optional[Dict[str, Any]] = None,
+    nuts_sampler_kwargs: Optional[Dict[str, Any]] = None,
+    callback=None,
+    mp_ctx=None,
+    **kwargs,
+) -> InferenceData:
+    ...
+
+
+@overload
+def sample(
+    draws: int = 1000,
+    *,
+    tune: int = 1000,
+    chains: Optional[int] = None,
+    cores: Optional[int] = None,
+    random_seed: RandomState = None,
+    progressbar: bool = True,
+    step=None,
+    nuts_sampler: str = "pymc",
+    initvals: Optional[Union[StartDict, Sequence[Optional[StartDict]]]] = None,
+    init: str = "auto",
+    jitter_max_retries: int = 10,
+    n_init: int = 200_000,
+    trace: Optional[TraceOrBackend] = None,
+    discard_tuned_samples: bool = True,
+    compute_convergence_checks: bool = True,
+    keep_warning_stat: bool = False,
+    return_inferencedata: Literal[False],
+    idata_kwargs: Optional[Dict[str, Any]] = None,
+    nuts_sampler_kwargs: Optional[Dict[str, Any]] = None,
+    callback=None,
+    mp_ctx=None,
+    model: Optional[Model] = None,
+    **kwargs,
+) -> MultiTrace:
+    ...
+
+
 def sample(
     draws: int = 1000,
     *,
     tune: int = 1000,
     chains: Optional[int] = None,
     cores: Optional[int] = None,
     random_seed: RandomState = None,
```

### Comparing `pymc-5.3.1/pymc/sampling/parallel.py` & `pymc-5.4.0/pymc/sampling/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from fastprogress.fastprogress import progress_bar
 
 from pymc.blocking import DictToArrayBijection
 from pymc.exceptions import SamplingError
 from pymc.util import RandomSeed
 
-logger = logging.getLogger("pymc")
+logger = logging.getLogger(__name__)
 
 
 class ParallelSamplingError(Exception):
     def __init__(self, message, chain):
         super().__init__(message)
         self._chain = chain
```

### Comparing `pymc-5.3.1/pymc/sampling/population.py` & `pymc-5.4.0/pymc/sampling/population.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 __all__ = ()
 
 
 Step: TypeAlias = Union[BlockedStep, CompoundStep]
 
 
-_log = logging.getLogger("pymc")
+_log = logging.getLogger(__name__)
 
 
 def _sample_population(
     *,
     initial_points: Sequence[PointType],
     draws: int,
     start: Sequence[PointType],
```

### Comparing `pymc-5.3.1/pymc/sampling_jax.py` & `pymc-5.4.0/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/smc/__init__.py` & `pymc-5.4.0/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/smc/kernels.py` & `pymc-5.4.0/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/smc/sampling.py` & `pymc-5.4.0/pymc/smc/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     else:
         cores = min(chains, cores)
 
     random_seed = _get_seeds_per_chain(random_state=random_seed, chains=chains)
 
     model = modelcontext(model)
 
-    _log = logging.getLogger("pymc")
+    _log = logging.getLogger(__name__)
     _log.info("Initializing SMC sampler...")
     _log.info(
         f"Sampling {chains} chain{'s' if chains > 1 else ''} "
         f"in {cores} job{'s' if cores > 1 else ''}"
     )
 
     params = (
```

### Comparing `pymc-5.3.1/pymc/stats/__init__.py` & `pymc-5.4.0/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/stats/convergence.py` & `pymc-5.4.0/pymc/stats/convergence.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "info": logging.INFO,
     "error": logging.ERROR,
     "warn": logging.WARN,
     "debug": logging.DEBUG,
     "critical": logging.CRITICAL,
 }
 
-logger = logging.getLogger("pymc")
+logger = logging.getLogger(__name__)
 
 
 @enum.unique
 class WarningType(enum.Enum):
     # For HMC and NUTS
     DIVERGENCE = 1
     TUNING_DIVERGENCE = 2
```

### Comparing `pymc-5.3.1/pymc/stats/log_likelihood.py` & `pymc-5.4.0/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/__init__.py` & `pymc-5.4.0/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/arraystep.py` & `pymc-5.4.0/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/compound.py` & `pymc-5.4.0/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/hmc/__init__.py` & `pymc-5.4.0/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.4.0/pymc/step_methods/hmc/base_hmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from pymc.step_methods.arraystep import GradientSharedStep
 from pymc.step_methods.hmc import integration
 from pymc.step_methods.hmc.integration import IntegrationError, State
 from pymc.step_methods.hmc.quadpotential import QuadPotentialDiagAdapt, quad_potential
 from pymc.tuning import guess_scaling
 from pymc.util import get_value_vars_from_user_vars
 
-logger = logging.getLogger("pymc")
+logger = logging.getLogger(__name__)
 
 
 class DivergenceInfo(NamedTuple):
     message: str
     exec_info: IntegrationError | None
     state: State
     state_div: State | None
```

### Comparing `pymc-5.3.1/pymc/step_methods/hmc/hmc.py` & `pymc-5.4.0/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/hmc/integration.py` & `pymc-5.4.0/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/hmc/nuts.py` & `pymc-5.4.0/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.4.0/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/metropolis.py` & `pymc-5.4.0/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/step_methods/slicer.py` & `pymc-5.4.0/pymc/step_methods/slicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,26 @@
 from typing import Tuple
 
 import numpy as np
 import numpy.random as nr
 
 from pymc.blocking import RaveledVars, StatsType
 from pymc.model import modelcontext
-from pymc.step_methods.arraystep import ArrayStep
+from pymc.pytensorf import compile_pymc, join_nonshared_inputs, make_shared_replacements
+from pymc.step_methods.arraystep import ArrayStepShared
 from pymc.step_methods.compound import Competence
 from pymc.util import get_value_vars_from_user_vars
 from pymc.vartypes import continuous_types
 
 __all__ = ["Slice"]
 
 LOOP_ERR_MSG = "max slicer iters %d exceeded"
 
 
-class Slice(ArrayStep):
+class Slice(ArrayStepShared):
     """
     Univariate slice sampler step method.
 
     Parameters
     ----------
     vars: list
         List of value variables for sampler.
@@ -47,78 +48,83 @@
         Optional model for sampling step. Defaults to None (taken from context).
 
     """
 
     name = "slice"
     default_blocked = False
     stats_dtypes_shapes = {
+        "tune": (bool, []),
         "nstep_out": (int, []),
         "nstep_in": (int, []),
     }
 
     def __init__(self, vars=None, w=1.0, tune=True, model=None, iter_limit=np.inf, **kwargs):
-        self.model = modelcontext(model)
-        self.w = w
+        model = modelcontext(model)
+        self.w = np.asarray(w).copy()
         self.tune = tune
         self.n_tunes = 0.0
         self.iter_limit = iter_limit
 
         if vars is None:
-            vars = self.model.continuous_value_vars
+            vars = model.continuous_value_vars
         else:
-            vars = get_value_vars_from_user_vars(vars, self.model)
+            vars = get_value_vars_from_user_vars(vars, model)
 
-        super().__init__(vars, [self.model.compile_logp()], **kwargs)
+        point = model.initial_point()
+        shared = make_shared_replacements(point, vars, model)
+        [logp], raveled_inp = join_nonshared_inputs(
+            point=point, outputs=[model.logp()], inputs=vars, shared_inputs=shared
+        )
+        self.logp = compile_pymc([raveled_inp], logp)
+        self.logp.trust_input = True
 
-    def astep(self, apoint: RaveledVars, *args) -> Tuple[RaveledVars, StatsType]:
+        super().__init__(vars, shared)
+
+    def astep(self, apoint: RaveledVars) -> Tuple[RaveledVars, StatsType]:
         # The arguments are determined by the list passed via `super().__init__(..., fs, ...)`
-        logp = args[0]
         q0_val = apoint.data
-        self.w = np.resize(self.w, len(q0_val))  # this is a repmat
+
+        if q0_val.shape != self.w.shape:
+            self.w = np.resize(self.w, len(q0_val))  # this is a repmat
 
         nstep_out = nstep_in = 0
 
         q = np.copy(q0_val)
         ql = np.copy(q0_val)  # l for left boundary
         qr = np.copy(q0_val)  # r for right boundary
 
-        # The points are not copied, so it's fine to update them inplace in the
-        # loop below
-        q_ra = RaveledVars(q, apoint.point_map_info)
-        ql_ra = RaveledVars(ql, apoint.point_map_info)
-        qr_ra = RaveledVars(qr, apoint.point_map_info)
-
+        logp = self.logp
         for i, wi in enumerate(self.w):
             # uniformly sample from 0 to p(q), but in log space
-            y = logp(q_ra) - nr.standard_exponential()
+            y = logp(q) - nr.standard_exponential()
 
             # Create initial interval
             ql[i] = q[i] - nr.uniform() * wi  # q[i] + r * w
             qr[i] = ql[i] + wi  # Equivalent to q[i] + (1-r) * w
 
             # Stepping out procedure
             cnt = 0
-            while y <= logp(ql_ra):  # changed lt to leq  for locally uniform posteriors
+            while y <= logp(ql):  # changed lt to leq  for locally uniform posteriors
                 ql[i] -= wi
                 cnt += 1
                 if cnt > self.iter_limit:
                     raise RuntimeError(LOOP_ERR_MSG % self.iter_limit)
             nstep_out += cnt
 
             cnt = 0
-            while y <= logp(qr_ra):
+            while y <= logp(qr):
                 qr[i] += wi
                 cnt += 1
                 if cnt > self.iter_limit:
                     raise RuntimeError(LOOP_ERR_MSG % self.iter_limit)
             nstep_out += cnt
 
             cnt = 0
             q[i] = nr.uniform(ql[i], qr[i])
-            while y > logp(q_ra):  # Changed leq to lt, to accommodate for locally flat posteriors
+            while y > logp(q):  # Changed leq to lt, to accommodate for locally flat posteriors
                 # Sample uniformly from slice
                 if q[i] > q0_val[i]:
                     qr[i] = q[i]
                 elif q[i] < q0_val[i]:
                     ql[i] = q[i]
                 q[i] = nr.uniform(ql[i], qr[i])
                 cnt += 1
@@ -136,14 +142,15 @@
             # Set qr and ql to the accepted points (they matter for subsequent iterations)
             qr[i] = ql[i] = q[i]
 
         if self.tune:
             self.n_tunes += 1
 
         stats = {
+            "tune": self.tune,
             "nstep_out": nstep_out,
             "nstep_in": nstep_in,
         }
 
         return RaveledVars(q, apoint.point_map_info), [stats]
 
     @staticmethod
```

### Comparing `pymc-5.3.1/pymc/step_methods/step_sizes.py` & `pymc-5.4.0/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/testing.py` & `pymc-5.4.0/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/tuning/__init__.py` & `pymc-5.4.0/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/tuning/scaling.py` & `pymc-5.4.0/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/tuning/starting.py` & `pymc-5.4.0/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/util.py` & `pymc-5.4.0/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/__init__.py` & `pymc-5.4.0/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/approximations.py` & `pymc-5.4.0/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/callbacks.py` & `pymc-5.4.0/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/inference.py` & `pymc-5.4.0/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/minibatch_rv.py` & `pymc-5.4.0/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/operators.py` & `pymc-5.4.0/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/opvi.py` & `pymc-5.4.0/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/stein.py` & `pymc-5.4.0/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/test_functions.py` & `pymc-5.4.0/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/variational/updates.py` & `pymc-5.4.0/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc/vartypes.py` & `pymc-5.4.0/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/pymc.egg-info/PKG-INFO` & `pymc-5.4.0/pymc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.3.1
+Version: 5.4.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.3.1/pymc.egg-info/SOURCES.txt` & `pymc-5.4.0/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/scripts/docker_container.sh` & `pymc-5.4.0/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/setup.py` & `pymc-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.3.1/versioneer.py` & `pymc-5.4.0/versioneer.py`

 * *Files identical despite different names*

