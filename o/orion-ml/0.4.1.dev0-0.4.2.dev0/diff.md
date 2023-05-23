# Comparing `tmp/orion-ml-0.4.1.dev0.tar.gz` & `tmp/orion-ml-0.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orion-ml-0.4.1.dev0.tar", last modified: Wed Jan  4 14:12:46 2023, max compression
+gzip compressed data, was "orion-ml-0.4.2.dev0.tar", last modified: Mon May 22 18:50:32 2023, max compression
```

## Comparing `orion-ml-0.4.1.dev0.tar` & `orion-ml-0.4.2.dev0.tar`

### file list

```diff
@@ -1,263 +1,291 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/
--rw-r--r--   0 sarah      (501) staff       (20)      173 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     7431 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)     9391 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/HISTORY.md
--rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      297 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)    19060 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     8827 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      606 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/Makefile
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/api_reference/
--rw-r--r--   0 sarah      (501) staff       (20)      455 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/api_reference/evaluation.rst
--rw-r--r--   0 sarah      (501) staff       (20)      206 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/api_reference/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      389 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/api_reference/orion.rst
--rw-r--r--   0 sarah      (501) staff       (20)      573 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/api_reference/prim.rst
--rw-r--r--   0 sarah      (501) staff       (20)     6400 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/conf.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/developer_guides/
--rw-r--r--   0 sarah      (501) staff       (20)     7428 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/developer_guides/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)      352 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/developer_guides/index.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/getting_started/
--rw-r--r--   0 sarah      (501) staff       (20)       30 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/getting_started/docker.rst
--rw-r--r--   0 sarah      (501) staff       (20)      123 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/getting_started/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1895 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/getting_started/install.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3336 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/getting_started/quickstart.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/history.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)    17513 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/Scoring.png
--rw-r--r--   0 sarah      (501) staff       (20)    11638 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/orion-logo-small.png
--rw-r--r--   0 sarah      (501) staff       (20)     7096 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/orion-logo-white-200.png
--rw-r--r--   0 sarah      (501) staff       (20)    68645 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/orion-logo.png
--rw-r--r--   0 sarah      (501) staff       (20)    18705 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/scoring-300.png
--rw-r--r--   0 sarah      (501) staff       (20)     2283 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/slack.png
--rw-r--r--   0 sarah      (501) staff       (20)   386774 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/tulog-part-1.png
--rw-r--r--   0 sarah      (501) staff       (20)   214698 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/tulog-part-2.png
--rw-r--r--   0 sarah      (501) staff       (20)   295778 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/images/tulog-part-3.png
--rw-r--r--   0 sarah      (501) staff       (20)     5830 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      767 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/make.bat
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/user_guides/
--rw-r--r--   0 sarah      (501) staff       (20)     2710 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/benchmarking.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2541 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/data.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5510 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/evaluation_doc.rst
--rw-r--r--   0 sarah      (501) staff       (20)      234 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/index.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/
--rw-r--r--   0 sarah      (501) staff       (20)      345 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8489 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/pipelines.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)     3094 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/AER.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4091 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/DenseSeq2Seq.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4322 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMSeq2Seq.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4319 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMTimeSeriesRegressor.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1911 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/MinMaxScaler.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2885 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/SimpleImputer.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3686 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/TadGAN.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3639 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/VAE.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1753 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/arima.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3375 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/fillna.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3072 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/find_anomalies.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1941 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/intervals_to_mask.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2348 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/reconstruction_errors.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2166 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/regression_errors.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3539 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/rolling_window_sequences.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3382 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/score_anomalies.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2768 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/time_segments_aggregate.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1046 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/docs/user_guides/system/
--rw-r--r--   0 sarah      (501) staff       (20)       47 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/system/api.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8506 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/system/database.rst
--rw-r--r--   0 sarah      (501) staff       (20)      166 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/system/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)       80 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/docs/user_guides/system/interface.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/
--rw-r--r--   0 sarah      (501) staff       (20)      581 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     3736 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/__main__.py
--rw-r--r--   0 sarah      (501) staff       (20)     1612 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/analysis.py
--rw-r--r--   0 sarah      (501) staff       (20)    14366 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/benchmark.py
--rw-r--r--   0 sarah      (501) staff       (20)    10571 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/core.py
--rw-r--r--   0 sarah      (501) staff       (20)     5824 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/data.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/evaluation/
--rw-r--r--   0 sarah      (501) staff       (20)      999 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/evaluation/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     2003 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/evaluation/common.py
--rw-r--r--   0 sarah      (501) staff       (20)     8298 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/evaluation/contextual.py
--rw-r--r--   0 sarah      (501) staff       (20)     6060 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/evaluation/point.py
--rw-r--r--   0 sarah      (501) staff       (20)     4173 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/evaluation/utils.py
--rw-r--r--   0 sarah      (501) staff       (20)     8827 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/functional.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/dummy/
--rw-r--r--   0 sarah      (501) staff       (20)      439 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/dummy/dummy.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/
--rw-r--r--   0 sarah      (501) staff       (20)     1788 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)      152 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      151 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      152 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)     2633 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_viz.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/
--rw-r--r--   0 sarah      (501) staff       (20)     1981 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer.json
--rw-r--r--   0 sarah      (501) staff       (20)      253 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)      178 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      254 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      253 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      253 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      176 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      178 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)      174 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      251 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      251 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      251 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/
--rw-r--r--   0 sarah      (501) staff       (20)     1694 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima.json
--rw-r--r--   0 sarah      (501) staff       (20)      738 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)      740 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      739 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      738 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      738 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      738 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      740 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)      735 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      735 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      735 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      735 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/
--rw-r--r--   0 sarah      (501) staff       (20)     1401 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure.json
--rw-r--r--   0 sarah      (501) staff       (20)      340 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)      342 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      342 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      340 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      340 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      340 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      342 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)      336 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      336 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      336 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      336 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/
--rw-r--r--   0 sarah      (501) staff       (20)     1846 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)      152 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      151 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      152 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/
--rw-r--r--   0 sarah      (501) staff       (20)     1843 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)     3139 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_gpu.json
--rw-r--r--   0 sarah      (501) staff       (20)      152 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      151 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      150 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      152 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      148 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/
--rw-r--r--   0 sarah      (501) staff       (20)     1534 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold.json
--rw-r--r--   0 sarah      (501) staff       (20)      485 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)     2914 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_gpu.json
--rw-r--r--   0 sarah      (501) staff       (20)      492 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      486 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      485 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      485 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      485 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      492 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)     1936 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_viz.json
--rw-r--r--   0 sarah      (501) staff       (20)      483 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      483 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      483 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      483 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa4.json
--rw-r--r--   0 sarah      (501) staff       (20)     1192 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/mean_24h_lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     1194 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/median_24h_lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     1192 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/skew_24h_lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     1191 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/sum_24h_lstm.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/
--rw-r--r--   0 sarah      (501) staff       (20)     1996 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan.json
--rw-r--r--   0 sarah      (501) staff       (20)      290 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_artificialwithanomaly.json
--rw-r--r--   0 sarah      (501) staff       (20)      362 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_msl.json
--rw-r--r--   0 sarah      (501) staff       (20)      316 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_realadexchange.json
--rw-r--r--   0 sarah      (501) staff       (20)      289 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_realawscloudwatch.json
--rw-r--r--   0 sarah      (501) staff       (20)      316 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_realtraffic.json
--rw-r--r--   0 sarah      (501) staff       (20)      316 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_realtweets.json
--rw-r--r--   0 sarah      (501) staff       (20)      362 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_smap.json
--rw-r--r--   0 sarah      (501) staff       (20)     2465 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_viz.json
--rw-r--r--   0 sarah      (501) staff       (20)     6501 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_without_dropout_gpu.json
--rw-r--r--   0 sarah      (501) staff       (20)      385 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa1.json
--rw-r--r--   0 sarah      (501) staff       (20)      358 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa2.json
--rw-r--r--   0 sarah      (501) staff       (20)      360 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa3.json
--rw-r--r--   0 sarah      (501) staff       (20)      359 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa4.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    12234 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/aer.py
--rw-r--r--   0 sarah      (501) staff       (20)     5910 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/azure_anomaly_detector.py
--rw-r--r--   0 sarah      (501) staff       (20)     1358 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/detectors.py
--rw-r--r--   0 sarah      (501) staff       (20)      614 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/estimators.py
--rw-r--r--   0 sarah      (501) staff       (20)     1647 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/intervals.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/
--rw-r--r--   0 sarah      (501) staff       (20)     5613 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/keras.Sequential.DenseSeq2Seq.json
--rw-r--r--   0 sarah      (501) staff       (20)     4418 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/keras.Sequential.LSTMSeq2Seq.json
--rw-r--r--   0 sarah      (501) staff       (20)     4688 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.aer.AER.json
--rw-r--r--   0 sarah      (501) staff       (20)     1635 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.aer.score_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     2122 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.detect_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     1252 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.split_sequence.json
--rw-r--r--   0 sarah      (501) staff       (20)     1647 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.detectors.ThresholdDetector.json
--rw-r--r--   0 sarah      (501) staff       (20)     1045 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.estimators.MeanEstimator.json
--rw-r--r--   0 sarah      (501) staff       (20)     1172 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.intervals.build_anomaly_intervals.json
--rw-r--r--   0 sarah      (501) staff       (20)    12517 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.tadgan.TadGAN.json
--rw-r--r--   0 sarah      (501) staff       (20)     2357 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.tadgan.score_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     2450 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_anomalies.find_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     1790 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.reconstruction_errors.json
--rw-r--r--   0 sarah      (501) staff       (20)     1553 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.regression_errors.json
--rw-r--r--   0 sarah      (501) staff       (20)     1240 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.fillna.json
--rw-r--r--   0 sarah      (501) staff       (20)      942 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.slice_array_by_dims.json
--rw-r--r--   0 sarah      (501) staff       (20)     4279 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.vae.VAE.json
--rw-r--r--   0 sarah      (501) staff       (20)    21040 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/tadgan.py
--rw-r--r--   0 sarah      (501) staff       (20)    17233 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)     7402 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/timeseries_errors.py
--rw-r--r--   0 sarah      (501) staff       (20)     3625 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/timeseries_preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)     8903 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/primitives/vae.py
--rw-r--r--   0 sarah      (501) staff       (20)     2011 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/progress.py
--rw-r--r--   0 sarah      (501) staff       (20)     4965 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/results.py
--rw-r--r--   0 sarah      (501) staff       (20)      762 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/orion/utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    19060 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)    11412 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)      134 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      881 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        6 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/orion_ml.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)      968 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     3171 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/tests/evaluation/
--rw-r--r--   0 sarah      (501) staff       (20)     1222 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/evaluation/test_common.py
--rw-r--r--   0 sarah      (501) staff       (20)     4991 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/evaluation/test_contextual.py
--rw-r--r--   0 sarah      (501) staff       (20)     2105 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/evaluation/test_point.py
--rw-r--r--   0 sarah      (501) staff       (20)     2449 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/evaluation/test_utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/tests/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)     7574 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/primitives/test_timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)     3911 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/primitives/test_timeseries_errors.py
--rw-r--r--   0 sarah      (501) staff       (20)     2664 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/primitives/test_timeseries_preprocessing.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-04 14:12:46.000000 orion-ml-0.4.1.dev0/tests/requirement_files/
--rw-r--r--   0 sarah      (501) staff       (20)     2003 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/requirement_files/latest_requirements.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1939 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/test_analysis.py
--rw-r--r--   0 sarah      (501) staff       (20)    21557 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/test_benchmark.py
--rw-r--r--   0 sarah      (501) staff       (20)     4824 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/test_core.py
--rw-r--r--   0 sarah      (501) staff       (20)     4165 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/test_data.py
--rw-r--r--   0 sarah      (501) staff       (20)    10897 2023-01-04 14:10:26.000000 orion-ml-0.4.1.dev0/tests/test_functional.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.221114 orion-ml-0.4.2.dev0/
+-rw-r--r--   0 sarah      (501) staff       (20)      173 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7431 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     9856 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      297 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    20219 2023-05-22 18:50:32.221362 orion-ml-0.4.2.dev0/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     9521 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.017142 orion-ml-0.4.2.dev0/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      606 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/Makefile
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.019445 orion-ml-0.4.2.dev0/docs/api_reference/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.042862 orion-ml-0.4.2.dev0/docs/api_reference/api/
+-rw-r--r--   0 sarah      (501) staff       (20)       96 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.Orion.detect.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      102 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.Orion.evaluate.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       87 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.Orion.fit.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       90 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.Orion.load.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      457 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.Orion.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       90 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.Orion.save.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      119 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.benchmark.benchmark.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      112 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.detect_anomalies.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      115 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluate_pipeline.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      154 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.contextual_accuracy.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      180 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.contextual_confusion_matrix.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      156 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.contextual_f1_score.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      157 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.contextual_precision.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      148 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.contextual_recall.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      139 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.point_accuracy.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      165 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.point_confusion_matrix.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      141 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.point_f1_score.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      142 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.point_precision.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      133 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.evaluation.point_recall.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      100 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.fit_pipeline.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      218 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.azure_anomaly_detector.detect_anomalies.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      212 2023-05-12 17:43:16.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.azure_anomaly_detector.split_sequence.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      301 2023-05-12 17:43:21.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.tadgan.TadGAN.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      163 2023-05-12 17:43:21.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.tadgan.score_anomalies.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      204 2023-05-12 17:43:21.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.timeseries_anomalies.find_anomalies.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      216 2023-05-12 17:43:21.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.timeseries_errors.reconstruction_errors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      204 2023-05-12 17:43:21.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.timeseries_errors.regression_errors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      190 2023-05-12 17:43:21.000000 orion-ml-0.4.2.dev0/docs/api_reference/api/orion.primitives.timeseries_preprocessing.fillna.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      455 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/api_reference/evaluation.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      206 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/api_reference/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      389 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/api_reference/orion.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      573 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/api_reference/prim.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     6400 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/conf.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.044278 orion-ml-0.4.2.dev0/docs/developer_guides/
+-rw-r--r--   0 sarah      (501) staff       (20)     7428 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/developer_guides/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      352 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/developer_guides/index.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.049229 orion-ml-0.4.2.dev0/docs/getting_started/
+-rw-r--r--   0 sarah      (501) staff       (20)       30 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/getting_started/docker.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      123 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/getting_started/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1895 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/docs/getting_started/install.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3336 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/getting_started/quickstart.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.064386 orion-ml-0.4.2.dev0/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)    17513 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/Scoring.png
+-rw-r--r--   0 sarah      (501) staff       (20)    11638 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/orion-logo-small.png
+-rw-r--r--   0 sarah      (501) staff       (20)     7096 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/orion-logo-white-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)    68645 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/orion-logo.png
+-rw-r--r--   0 sarah      (501) staff       (20)    18705 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/scoring-300.png
+-rw-r--r--   0 sarah      (501) staff       (20)     2283 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/slack.png
+-rw-r--r--   0 sarah      (501) staff       (20)   386774 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/tulog-part-1.png
+-rw-r--r--   0 sarah      (501) staff       (20)   214698 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/tulog-part-2.png
+-rw-r--r--   0 sarah      (501) staff       (20)   295778 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/images/tulog-part-3.png
+-rw-r--r--   0 sarah      (501) staff       (20)     5830 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      767 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/make.bat
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.072228 orion-ml-0.4.2.dev0/docs/user_guides/
+-rw-r--r--   0 sarah      (501) staff       (20)     2710 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/benchmarking.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2541 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/data.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5510 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/evaluation_doc.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      234 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/index.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.076350 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/
+-rw-r--r--   0 sarah      (501) staff       (20)      345 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8477 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/pipelines.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.092005 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)     3089 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/AER.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4086 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/DenseSeq2Seq.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4317 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMSeq2Seq.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4304 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMTimeSeriesRegressor.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1896 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/MinMaxScaler.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2870 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/SimpleImputer.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3681 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/TadGAN.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3634 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/VAE.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1738 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/arima.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3370 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/fillna.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3067 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/find_anomalies.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1911 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/intervals_to_mask.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2343 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/reconstruction_errors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2161 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/regression_errors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3509 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/rolling_window_sequences.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3377 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/score_anomalies.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2738 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/time_segments_aggregate.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1039 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.095559 orion-ml-0.4.2.dev0/docs/user_guides/system/
+-rw-r--r--   0 sarah      (501) staff       (20)       47 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/system/api.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8506 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/system/database.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      166 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/system/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       80 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/docs/user_guides/system/interface.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.105333 orion-ml-0.4.2.dev0/orion/
+-rw-r--r--   0 sarah      (501) staff       (20)      581 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/orion/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3736 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/__main__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1612 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/analysis.py
+-rw-r--r--   0 sarah      (501) staff       (20)    14359 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/benchmark.py
+-rw-r--r--   0 sarah      (501) staff       (20)    10635 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/orion/core.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5825 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/data.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.109775 orion-ml-0.4.2.dev0/orion/evaluation/
+-rw-r--r--   0 sarah      (501) staff       (20)      999 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/evaluation/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2003 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/evaluation/common.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8298 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/evaluation/contextual.py
+-rw-r--r--   0 sarah      (501) staff       (20)     6060 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/evaluation/point.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4173 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/evaluation/utils.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8827 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/functional.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.006181 orion-ml-0.4.2.dev0/orion/pipelines/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.006028 orion-ml-0.4.2.dev0/orion/pipelines/sandbox/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.110516 orion-ml-0.4.2.dev0/orion/pipelines/sandbox/dummy/
+-rw-r--r--   0 sarah      (501) staff       (20)      439 2023-04-26 15:39:52.000000 orion-ml-0.4.2.dev0/orion/pipelines/sandbox/dummy/dummy.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.007673 orion-ml-0.4.2.dev0/orion/pipelines/verified/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.121183 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/
+-rw-r--r--   0 sarah      (501) staff       (20)     1956 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer.json
+-rw-r--r--   0 sarah      (501) staff       (20)      248 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      173 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      249 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      248 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      248 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      171 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      173 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2337 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_viz.json
+-rw-r--r--   0 sarah      (501) staff       (20)      169 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      246 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      246 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      246 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.130766 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/
+-rw-r--r--   0 sarah      (501) staff       (20)     1674 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima.json
+-rw-r--r--   0 sarah      (501) staff       (20)      728 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      730 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      729 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      728 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      728 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      728 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      730 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)      725 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      725 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      725 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      725 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.140743 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/
+-rw-r--r--   0 sarah      (501) staff       (20)     1391 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure.json
+-rw-r--r--   0 sarah      (501) staff       (20)      335 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      337 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      337 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      335 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      335 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      335 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      337 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)      331 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      331 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      331 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      331 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.150147 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/
+-rw-r--r--   0 sarah      (501) staff       (20)     1821 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      147 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      146 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      147 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.159738 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/
+-rw-r--r--   0 sarah      (501) staff       (20)     1818 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      147 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      146 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      147 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.171817 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/
+-rw-r--r--   0 sarah      (501) staff       (20)     1514 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold.json
+-rw-r--r--   0 sarah      (501) staff       (20)      475 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      482 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      476 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      475 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      475 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      475 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      482 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1916 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_viz.json
+-rw-r--r--   0 sarah      (501) staff       (20)      473 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      473 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      473 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      473 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_yahooa4.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1172 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/mean_24h_lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1174 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/median_24h_lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1172 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/skew_24h_lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/sum_24h_lstm.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.181254 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/
+-rw-r--r--   0 sarah      (501) staff       (20)     1971 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan.json
+-rw-r--r--   0 sarah      (501) staff       (20)      285 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      357 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      311 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      284 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      311 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      311 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      357 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2440 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_viz.json
+-rw-r--r--   0 sarah      (501) staff       (20)     6476 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_without_dropout_gpu.json
+-rw-r--r--   0 sarah      (501) staff       (20)      380 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      353 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      355 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      354 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.190806 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/
+-rw-r--r--   0 sarah      (501) staff       (20)     1763 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_artificialwithanomaly.json
+-rw-r--r--   0 sarah      (501) staff       (20)      147 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_msl.json
+-rw-r--r--   0 sarah      (501) staff       (20)      146 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_realadexchange.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_realawscloudwatch.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_realtraffic.json
+-rw-r--r--   0 sarah      (501) staff       (20)      145 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_realtweets.json
+-rw-r--r--   0 sarah      (501) staff       (20)      147 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_smap.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2603 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_viz.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_yahooa1.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_yahooa2.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_yahooa3.json
+-rw-r--r--   0 sarah      (501) staff       (20)      143 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_yahooa4.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.198421 orion-ml-0.4.2.dev0/orion/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/primitives/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    12229 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/primitives/aer.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5910 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/primitives/azure_anomaly_detector.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1358 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/primitives/detectors.py
+-rw-r--r--   0 sarah      (501) staff       (20)      614 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/primitives/estimators.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1647 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/primitives/intervals.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.209058 orion-ml-0.4.2.dev0/orion/primitives/jsons/
+-rw-r--r--   0 sarah      (501) staff       (20)     5608 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/keras.Sequential.DenseSeq2Seq.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4413 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/keras.Sequential.LSTMSeq2Seq.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4688 2023-04-26 15:39:53.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.aer.AER.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1635 2023-04-26 15:39:53.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.aer.score_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2122 2023-04-26 15:39:54.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.detect_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1252 2023-04-26 15:39:55.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.split_sequence.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1647 2023-04-26 15:39:56.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.detectors.ThresholdDetector.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1045 2023-04-26 15:39:56.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.estimators.MeanEstimator.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1172 2023-04-26 15:39:57.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.intervals.build_anomaly_intervals.json
+-rw-r--r--   0 sarah      (501) staff       (20)    12517 2023-04-26 15:39:58.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.tadgan.TadGAN.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2357 2023-04-26 15:39:59.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.tadgan.score_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2450 2023-04-26 15:40:00.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_anomalies.find_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1790 2023-04-26 15:40:05.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.reconstruction_errors.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1553 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.regression_errors.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1240 2023-04-26 15:40:06.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.fillna.json
+-rw-r--r--   0 sarah      (501) staff       (20)      942 2023-04-26 15:40:07.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.slice_array_by_dims.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4279 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.vae.VAE.json
+-rw-r--r--   0 sarah      (501) staff       (20)    21035 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/primitives/tadgan.py
+-rw-r--r--   0 sarah      (501) staff       (20)    17262 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/orion/primitives/timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)     7404 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/primitives/timeseries_errors.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3625 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/primitives/timeseries_preprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8898 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/orion/primitives/vae.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2011 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/progress.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4965 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/results.py
+-rw-r--r--   0 sarah      (501) staff       (20)      762 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/orion/utils.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.211662 orion-ml-0.4.2.dev0/orion_ml.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    20219 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)    13023 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)      134 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      909 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        6 2023-05-22 18:50:31.000000 orion-ml-0.4.2.dev0/orion_ml.egg-info/top_level.txt
+-rw-r--r--   0 sarah      (501) staff       (20)      968 2023-05-22 18:50:32.222249 orion-ml-0.4.2.dev0/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     3244 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.214805 orion-ml-0.4.2.dev0/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.217650 orion-ml-0.4.2.dev0/tests/evaluation/
+-rw-r--r--   0 sarah      (501) staff       (20)     1222 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/evaluation/test_common.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4991 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/evaluation/test_contextual.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2105 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/evaluation/test_point.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2449 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/evaluation/test_utils.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.219735 orion-ml-0.4.2.dev0/tests/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)     7556 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/tests/primitives/test_timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3911 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/primitives/test_timeseries_errors.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2664 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/primitives/test_timeseries_preprocessing.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-22 18:50:32.220639 orion-ml-0.4.2.dev0/tests/requirement_files/
+-rw-r--r--   0 sarah      (501) staff       (20)     1983 2023-05-18 18:11:17.000000 orion-ml-0.4.2.dev0/tests/requirement_files/latest_requirements.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1929 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/tests/test_analysis.py
+-rw-r--r--   0 sarah      (501) staff       (20)    21557 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/test_benchmark.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4824 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/test_core.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4166 2023-05-22 18:14:38.000000 orion-ml-0.4.2.dev0/tests/test_data.py
+-rw-r--r--   0 sarah      (501) staff       (20)    10897 2023-03-29 20:54:33.000000 orion-ml-0.4.2.dev0/tests/test_functional.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `orion-ml-0.4.1.dev0/CONTRIBUTING.rst` & `orion-ml-0.4.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/HISTORY.md` & `orion-ml-0.4.2.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 History
 =======
 
+## 0.4.1 - 2023-01-31
+
+### Issues resolved
+
+* Move VAE from sandbox to verified – [Issue #377](https://github.com/signals-dev/Orion/issues/377) by @sarahmish
+* Pin ``opencv`` – [Issue #372](https://github.com/signals-dev/Orion/issues/372) by @sarahmish
+* Pin ``scikit-learn`` – [Issue #367](https://github.com/signals-dev/Orion/issues/367) by @sarahmish
+* Fix VAE documentation – [Issue #360](https://github.com/signals-dev/Orion/issues/360) by @sarahmish
+
 ## 0.4.0 - 2022-11-08
 
 This version introduces several new enhancements:
 
 * Support to python 3.8
 * Migrating to Tensorflow 2.0
 * New pipeline, namely ``VAE``, a Variational AutoEncoder model.
```

### Comparing `orion-ml-0.4.1.dev0/LICENSE` & `orion-ml-0.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/PKG-INFO` & `orion-ml-0.4.2.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orion-ml
-Version: 0.4.1.dev0
+Version: 0.4.2.dev0
 Summary: Orion is a machine learning library built for unsupervised time series anomaly detection.
 Home-page: https://github.com/sintel-dev/Orion
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: orion
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,30 +38,28 @@
 [![Downloads](https://pepy.tech/badge/orion-ml)](https://pepy.tech/project/orion-ml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sintel-dev/Orion/master?filepath=tutorials)
 
 # Orion
 
 A machine learning library for unsupervised time series anomaly detection.
 
-| Important Links                     |                                                                      |
-| ----------------------------------- | -------------------------------------------------------------------- |
-| :computer: **[Website]**            | Check out the Sintel Website for more information about the project. |
-| :book: **[Documentation]**          | Quickstarts, User and Development Guides, and API Reference.         |
-| :star: **[Tutorials]**              | Checkout our notebooks                                               |
-| :octocat: **[Repository]**          | The link to the Github Repository of this library.                   |
-| :scroll: **[License]**              | The repository is published under the MIT License.                   |
-| :keyboard: **[Development Status]** | This software is in its Pre-Alpha stage.                             |
+| Important Links                               |                                                                      |
+| --------------------------------------------- | -------------------------------------------------------------------- |
+| :computer: **[Website]**                      | Check out the Sintel Website for more information about the project. |
+| :book: **[Documentation]**                    | Quickstarts, User and Development Guides, and API Reference.         |
+| :star: **[Tutorials]**                        | Checkout our notebooks                                               |
+| :octocat: **[Repository]**                    | The link to the Github Repository of this library.                   |
+| :scroll: **[License]**                        | The repository is published under the MIT License.                   |
 | [![][Slack Logo] **Community**][Community]    | Join our Slack Workspace for announcements and discussions.          |
 
 [Website]: https://sintel.dev/
 [Documentation]: https://sintel-dev.github.io/Orion
 [Tutorials]: https://github.com/sintel-dev/Orion/tree/master/tutorials
 [Repository]: https://github.com/sintel-dev/Orion
 [License]: https://github.com/sintel-dev/Orion/blob/master/LICENSE
-[Development Status]: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
 [Community]: https://join.slack.com/t/sintel-space/shared_invite/zt-q147oimb-4HcphcxPfDAM0O9_4PaUtw
 [Slack Logo]: https://github.com/sintel-dev/Orion/blob/master/docs/images/slack.png
 
 # Overview
 
 Orion is a machine learning library built for *unsupervised time series anomaly detection*. With a given time series data, we provide a number of “verified” ML pipelines (a.k.a Orion pipelines) that identify rare patterns and flag them for expert review.
 
@@ -107,28 +105,28 @@
 0  1222819200 -0.366359
 1  1222840800 -0.394108
 2  1222862400  0.403625
 3  1222884000 -0.362759
 4  1222905600 -0.370746
 ```
 
-In this example we use `lstm_dynamic_threshold` pipeline and set some hyperparameters (in this case training epochs as 5).
+In this example we use `aer` pipeline and set some hyperparameters (in this case training epochs as 5).
 
 ```python3
 from orion import Orion
 
 hyperparameters = {
-    'keras.Sequential.LSTMTimeSeriesRegressor#1': {
+    'orion.primitives.aer.AER#1': {
         'epochs': 5,
         'verbose': True
     }
 }
 
 orion = Orion(
-    pipeline='lstm_dynamic_threshold',
+    pipeline='aer',
     hyperparameters=hyperparameters
 )
 
 orion.fit(train_data)
 ```
 
 ## Detect anomalies using the fitted pipeline
@@ -150,52 +148,51 @@
 # Leaderboard
 In every release, we run Orion benchmark. We maintain an up-to-date leaderboard with the current scoring of the verified pipelines according to the benchmarking procedure.
 
 We run the benchmark on **11** datasets with their known grounth truth. We record the score of the pipelines on each datasets. To compute the leaderboard table, we showcase the number of wins each pipeline has over the ARIMA pipeline.
 
 | Pipeline                  |  Outperforms ARIMA |
 |---------------------------|--------------------|
-| AER                       |         10         |
+| AER                       |         11         |
 | TadGAN                    |          7         |
-| LSTM Dynamic Thresholding |          8         |
+| LSTM Dynamic Thresholding |          7         |
 | LSTM Autoencoder          |          6         |
 | Dense Autoencoder         |          6         |
-| VAE                       |          6         |
-| Azure                     |          0         |
+| VAE                       |          7         |
+| [GANF](https://arxiv.org/pdf/2202.07857.pdf)                                                  |          6         |
+| [Azure](https://azure.microsoft.com/en-us/products/cognitive-services/anomaly-detector/)      |          0         |
 
 
 You can find the scores of each pipeline on every signal recorded in the [details Google Sheets document](https://docs.google.com/spreadsheets/d/1HaYDjY-BEXEObbi65fwG0om5d8kbRarhpK4mvOZVmqU/edit?usp=sharing). The summarized results can also be browsed in the following [summary Google Sheets document](https://docs.google.com/spreadsheets/d/1ZPUwYH8LhDovVeuJhKYGXYny7472HXVCzhX6D6PObmg/edit?usp=sharing).
 
 # Resources
 
 Additional resources that might be of interest:
 * Learn about [benchmarking pipelines](BENCHMARK.md).
 * Read about [pipeline evaluation](orion/evaluation/README.md).
 * Find out more about [TadGAN](https://arxiv.org/pdf/2009.07769v3.pdf).
 
 # Citation
 
-If you use **Orion** which is part of the **Sintel** ecosystem for your research, please consider citing the following paper:
+If you use **AER** for your research, please consider citing the following paper:
+
+Lawrence Wong, Dongyu Liu, Laure Berti-Equille, Sarah Alnegheimish, Kalyan Veeramachaneni. [AER: Auto-Encoder with Regression for Time Series Anomaly Detection](https://arxiv.org/pdf/2212.13558.pdf).
 
-Sarah Alnegheimish, Dongyu Liu, Carles Sala, Laure Berti-Equille, Kalyan Veeramachaneni. [Sintel: A Machine Learning Framework to Extract Insights from Signals](https://dl.acm.org/doi/pdf/10.1145/3514221.3517910).
 ```
-@inproceedings{alnegheimish2022sintel,
-  title={Sintel: A Machine Learning Framework to Extract Insights from Signals},
-  author={Alnegheimish, Sarah and Liu, Dongyu and Sala, Carles and Berti-Equille, Laure and Veeramachaneni, Kalyan},  
-  booktitle={Proceedings of the 2022 International Conference on Management of Data},
-  pages = {1855–1865},
-  numpages = {11},
-  publisher={Association for Computing Machinery},
-  doi = {10.1145/3514221.3517910},
-  series = {SIGMOD '22},
+@inproceedings{wong2022aer,
+  title={AER: Auto-Encoder with Regression for Time Series Anomaly Detection},
+  author={Wong, Lawrence and Liu, Dongyu and Berti-Equille, Laure and Alnegheimish, Sarah and Veeramachaneni, Kalyan},
+  booktitle={2022 IEEE International Conference on Big Data (IEEE BigData)},
+  pages={1152-1161},
+  doi={10.1109/BigData55660.2022.10020857},
+  organization={IEEE},
   year={2022}
 }
 ```
 
-
 If you use **TadGAN** for your research, please consider citing the following paper:
 
 Alexander Geiger, Dongyu Liu, Sarah Alnegheimish, Alfredo Cuesta-Infante, Kalyan Veeramachaneni. [TadGAN - Time Series Anomaly Detection Using Generative Adversarial Networks](https://arxiv.org/pdf/2009.07769v3.pdf).
 
 ```
 @inproceedings{geiger2020tadgan,
   title={TadGAN: Time Series Anomaly Detection Using Generative Adversarial Networks},
@@ -204,18 +201,44 @@
   pages={33-43},
   doi={10.1109/BigData50022.2020.9378139},
   organization={IEEE},
   year={2020}
 }
 ```
 
+If you use **Orion** which is part of the **Sintel** ecosystem for your research, please consider citing the following paper:
+
+Sarah Alnegheimish, Dongyu Liu, Carles Sala, Laure Berti-Equille, Kalyan Veeramachaneni. [Sintel: A Machine Learning Framework to Extract Insights from Signals](https://dl.acm.org/doi/pdf/10.1145/3514221.3517910).
+```
+@inproceedings{alnegheimish2022sintel,
+  title={Sintel: A Machine Learning Framework to Extract Insights from Signals},
+  author={Alnegheimish, Sarah and Liu, Dongyu and Sala, Carles and Berti-Equille, Laure and Veeramachaneni, Kalyan},  
+  booktitle={Proceedings of the 2022 International Conference on Management of Data},
+  pages={1855–1865},
+  numpages={11},
+  publisher={Association for Computing Machinery},
+  doi={10.1145/3514221.3517910},
+  series={SIGMOD '22},
+  year={2022}
+}
+```
+
 
 History
 =======
 
+## 0.4.1 - 2023-01-31
+
+### Issues resolved
+
+* Move VAE from sandbox to verified – [Issue #377](https://github.com/signals-dev/Orion/issues/377) by @sarahmish
+* Pin ``opencv`` – [Issue #372](https://github.com/signals-dev/Orion/issues/372) by @sarahmish
+* Pin ``scikit-learn`` – [Issue #367](https://github.com/signals-dev/Orion/issues/367) by @sarahmish
+* Fix VAE documentation – [Issue #360](https://github.com/signals-dev/Orion/issues/360) by @sarahmish
+
 ## 0.4.0 - 2022-11-08
 
 This version introduces several new enhancements:
 
 * Support to python 3.8
 * Migrating to Tensorflow 2.0
 * New pipeline, namely ``VAE``, a Variational AutoEncoder model.
```

### Comparing `orion-ml-0.4.1.dev0/README.md` & `orion-ml-0.4.2.dev0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 [![Downloads](https://pepy.tech/badge/orion-ml)](https://pepy.tech/project/orion-ml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sintel-dev/Orion/master?filepath=tutorials)
 
 # Orion
 
 A machine learning library for unsupervised time series anomaly detection.
 
-| Important Links                     |                                                                      |
-| ----------------------------------- | -------------------------------------------------------------------- |
-| :computer: **[Website]**            | Check out the Sintel Website for more information about the project. |
-| :book: **[Documentation]**          | Quickstarts, User and Development Guides, and API Reference.         |
-| :star: **[Tutorials]**              | Checkout our notebooks                                               |
-| :octocat: **[Repository]**          | The link to the Github Repository of this library.                   |
-| :scroll: **[License]**              | The repository is published under the MIT License.                   |
-| :keyboard: **[Development Status]** | This software is in its Pre-Alpha stage.                             |
+| Important Links                               |                                                                      |
+| --------------------------------------------- | -------------------------------------------------------------------- |
+| :computer: **[Website]**                      | Check out the Sintel Website for more information about the project. |
+| :book: **[Documentation]**                    | Quickstarts, User and Development Guides, and API Reference.         |
+| :star: **[Tutorials]**                        | Checkout our notebooks                                               |
+| :octocat: **[Repository]**                    | The link to the Github Repository of this library.                   |
+| :scroll: **[License]**                        | The repository is published under the MIT License.                   |
 | [![][Slack Logo] **Community**][Community]    | Join our Slack Workspace for announcements and discussions.          |
 
 [Website]: https://sintel.dev/
 [Documentation]: https://sintel-dev.github.io/Orion
 [Tutorials]: https://github.com/sintel-dev/Orion/tree/master/tutorials
 [Repository]: https://github.com/sintel-dev/Orion
 [License]: https://github.com/sintel-dev/Orion/blob/master/LICENSE
-[Development Status]: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
 [Community]: https://join.slack.com/t/sintel-space/shared_invite/zt-q147oimb-4HcphcxPfDAM0O9_4PaUtw
 [Slack Logo]: https://github.com/sintel-dev/Orion/blob/master/docs/images/slack.png
 
 # Overview
 
 Orion is a machine learning library built for *unsupervised time series anomaly detection*. With a given time series data, we provide a number of “verified” ML pipelines (a.k.a Orion pipelines) that identify rare patterns and flag them for expert review.
 
@@ -83,28 +81,28 @@
 0  1222819200 -0.366359
 1  1222840800 -0.394108
 2  1222862400  0.403625
 3  1222884000 -0.362759
 4  1222905600 -0.370746
 ```
 
-In this example we use `lstm_dynamic_threshold` pipeline and set some hyperparameters (in this case training epochs as 5).
+In this example we use `aer` pipeline and set some hyperparameters (in this case training epochs as 5).
 
 ```python3
 from orion import Orion
 
 hyperparameters = {
-    'keras.Sequential.LSTMTimeSeriesRegressor#1': {
+    'orion.primitives.aer.AER#1': {
         'epochs': 5,
         'verbose': True
     }
 }
 
 orion = Orion(
-    pipeline='lstm_dynamic_threshold',
+    pipeline='aer',
     hyperparameters=hyperparameters
 )
 
 orion.fit(train_data)
 ```
 
 ## Detect anomalies using the fitted pipeline
@@ -126,52 +124,51 @@
 # Leaderboard
 In every release, we run Orion benchmark. We maintain an up-to-date leaderboard with the current scoring of the verified pipelines according to the benchmarking procedure.
 
 We run the benchmark on **11** datasets with their known grounth truth. We record the score of the pipelines on each datasets. To compute the leaderboard table, we showcase the number of wins each pipeline has over the ARIMA pipeline.
 
 | Pipeline                  |  Outperforms ARIMA |
 |---------------------------|--------------------|
-| AER                       |         10         |
+| AER                       |         11         |
 | TadGAN                    |          7         |
-| LSTM Dynamic Thresholding |          8         |
+| LSTM Dynamic Thresholding |          7         |
 | LSTM Autoencoder          |          6         |
 | Dense Autoencoder         |          6         |
-| VAE                       |          6         |
-| Azure                     |          0         |
+| VAE                       |          7         |
+| [GANF](https://arxiv.org/pdf/2202.07857.pdf)                                                  |          6         |
+| [Azure](https://azure.microsoft.com/en-us/products/cognitive-services/anomaly-detector/)      |          0         |
 
 
 You can find the scores of each pipeline on every signal recorded in the [details Google Sheets document](https://docs.google.com/spreadsheets/d/1HaYDjY-BEXEObbi65fwG0om5d8kbRarhpK4mvOZVmqU/edit?usp=sharing). The summarized results can also be browsed in the following [summary Google Sheets document](https://docs.google.com/spreadsheets/d/1ZPUwYH8LhDovVeuJhKYGXYny7472HXVCzhX6D6PObmg/edit?usp=sharing).
 
 # Resources
 
 Additional resources that might be of interest:
 * Learn about [benchmarking pipelines](BENCHMARK.md).
 * Read about [pipeline evaluation](orion/evaluation/README.md).
 * Find out more about [TadGAN](https://arxiv.org/pdf/2009.07769v3.pdf).
 
 # Citation
 
-If you use **Orion** which is part of the **Sintel** ecosystem for your research, please consider citing the following paper:
+If you use **AER** for your research, please consider citing the following paper:
+
+Lawrence Wong, Dongyu Liu, Laure Berti-Equille, Sarah Alnegheimish, Kalyan Veeramachaneni. [AER: Auto-Encoder with Regression for Time Series Anomaly Detection](https://arxiv.org/pdf/2212.13558.pdf).
 
-Sarah Alnegheimish, Dongyu Liu, Carles Sala, Laure Berti-Equille, Kalyan Veeramachaneni. [Sintel: A Machine Learning Framework to Extract Insights from Signals](https://dl.acm.org/doi/pdf/10.1145/3514221.3517910).
 ```
-@inproceedings{alnegheimish2022sintel,
-  title={Sintel: A Machine Learning Framework to Extract Insights from Signals},
-  author={Alnegheimish, Sarah and Liu, Dongyu and Sala, Carles and Berti-Equille, Laure and Veeramachaneni, Kalyan},  
-  booktitle={Proceedings of the 2022 International Conference on Management of Data},
-  pages = {1855–1865},
-  numpages = {11},
-  publisher={Association for Computing Machinery},
-  doi = {10.1145/3514221.3517910},
-  series = {SIGMOD '22},
+@inproceedings{wong2022aer,
+  title={AER: Auto-Encoder with Regression for Time Series Anomaly Detection},
+  author={Wong, Lawrence and Liu, Dongyu and Berti-Equille, Laure and Alnegheimish, Sarah and Veeramachaneni, Kalyan},
+  booktitle={2022 IEEE International Conference on Big Data (IEEE BigData)},
+  pages={1152-1161},
+  doi={10.1109/BigData55660.2022.10020857},
+  organization={IEEE},
   year={2022}
 }
 ```
 
-
 If you use **TadGAN** for your research, please consider citing the following paper:
 
 Alexander Geiger, Dongyu Liu, Sarah Alnegheimish, Alfredo Cuesta-Infante, Kalyan Veeramachaneni. [TadGAN - Time Series Anomaly Detection Using Generative Adversarial Networks](https://arxiv.org/pdf/2009.07769v3.pdf).
 
 ```
 @inproceedings{geiger2020tadgan,
   title={TadGAN: Time Series Anomaly Detection Using Generative Adversarial Networks},
@@ -179,7 +176,24 @@
   booktitle={2020 IEEE International Conference on Big Data (IEEE BigData)},
   pages={33-43},
   doi={10.1109/BigData50022.2020.9378139},
   organization={IEEE},
   year={2020}
 }
 ```
+
+If you use **Orion** which is part of the **Sintel** ecosystem for your research, please consider citing the following paper:
+
+Sarah Alnegheimish, Dongyu Liu, Carles Sala, Laure Berti-Equille, Kalyan Veeramachaneni. [Sintel: A Machine Learning Framework to Extract Insights from Signals](https://dl.acm.org/doi/pdf/10.1145/3514221.3517910).
+```
+@inproceedings{alnegheimish2022sintel,
+  title={Sintel: A Machine Learning Framework to Extract Insights from Signals},
+  author={Alnegheimish, Sarah and Liu, Dongyu and Sala, Carles and Berti-Equille, Laure and Veeramachaneni, Kalyan},  
+  booktitle={Proceedings of the 2022 International Conference on Management of Data},
+  pages={1855–1865},
+  numpages={11},
+  publisher={Association for Computing Machinery},
+  doi={10.1145/3514221.3517910},
+  series={SIGMOD '22},
+  year={2022}
+}
+```
```

### Comparing `orion-ml-0.4.1.dev0/docs/Makefile` & `orion-ml-0.4.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/api_reference/prim.rst` & `orion-ml-0.4.2.dev0/docs/api_reference/prim.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/conf.py` & `orion-ml-0.4.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/developer_guides/contributing.rst` & `orion-ml-0.4.2.dev0/docs/developer_guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/getting_started/install.rst` & `orion-ml-0.4.2.dev0/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/getting_started/quickstart.rst` & `orion-ml-0.4.2.dev0/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/Scoring.png` & `orion-ml-0.4.2.dev0/docs/images/Scoring.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/orion-logo-small.png` & `orion-ml-0.4.2.dev0/docs/images/orion-logo-small.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/orion-logo-white-200.png` & `orion-ml-0.4.2.dev0/docs/images/orion-logo-white-200.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/orion-logo.png` & `orion-ml-0.4.2.dev0/docs/images/orion-logo.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/scoring-300.png` & `orion-ml-0.4.2.dev0/docs/images/scoring-300.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/slack.png` & `orion-ml-0.4.2.dev0/docs/images/slack.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/tulog-part-1.png` & `orion-ml-0.4.2.dev0/docs/images/tulog-part-1.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/tulog-part-2.png` & `orion-ml-0.4.2.dev0/docs/images/tulog-part-2.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/images/tulog-part-3.png` & `orion-ml-0.4.2.dev0/docs/images/tulog-part-3.png`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/index.rst` & `orion-ml-0.4.2.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/make.bat` & `orion-ml-0.4.2.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/benchmarking.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/benchmarking.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/data.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/data.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/evaluation_doc.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/evaluation_doc.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/pipelines.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/pipelines.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Pipelines
 =========
 
 The main component in the Orion project are the **Orion Pipelines**, which consist of `MLBlocks Pipelines <https://mlbazaar.github.io/MLBlocks/advanced_usage/pipelines.html>`__ specialized in detecting anomalies in time series.
 
 As ``MLPipeline`` instances, **Orion Pipelines**:
 
-* consist of a list of one or more `MLPrimitives <https://mlbazaar.github.io/MLPrimitives/>`__
+* consist of a list of one or more `mlstars <https://sintel-dev.github.io/ml-stars/>`__
 * can be *fitted* on some data and later on used to *predict* anomalies on more data
 * can be *scored* by comparing their predictions with some known anomalies
 * have *hyperparameters* that can be *tuned* to improve their anomaly detection performance
 * can be stored as a JSON file that includes all the primitives that compose them, as well as other required configuration options.
 
 Pipeline Representation
 -----------------------
@@ -149,15 +149,15 @@
     from orion import Orion
 
     np.random.seed(0)
     custom_data = pd.DataFrame({"timestamp": np.arange(0, 150000, 300),
                                 "value": np.random.randint(0, 10, 500)})
 
     hyperparameters = {
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 300
         },
         'keras.Sequential.LSTMTimeSeriesRegressor#1': {
             'epochs': 5,
             'verbose': True
         }
     }
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/AER.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/AER.rst`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ========================== =================== =================================================================================================
 
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.ones((64, 100, 1))
     y = X[:,:, [0]] # signal to reconstruct from X (channel 0)
     primitive = load_primitive('orion.primitives.aer.AER',
         arguments={"X": X, "y": y, "epochs": 1, "batch_size": 1})
 
     primitive.fit()
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/DenseSeq2Seq.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/DenseSeq2Seq.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  ``y``                  ``numpy.ndarray``   predicted values
 ====================== =================== ===========================================================================================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 100).reshape(1, -1, 1)
 
     primitive = load_primitive('keras.Sequential.DenseSeq2Seq', 
         arguments={"X": X, "y": X, "input_shape":(100, 1), "target_shape":(100, 1), 
                    "window_size": 100, "batch_size": 1, "validation_split": 0, "epochs": 5})
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMSeq2Seq.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMSeq2Seq.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  ``y``                  ``numpy.ndarray``   predicted values
 ====================== =================== ===========================================================================================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 100).reshape(1, -1, 1)
 
     primitive = load_primitive('keras.Sequential.LSTMSeq2Seq', 
         arguments={"X": X, "y": X, "input_shape":(100, 1), "target_shape":(100, 1), 
                    "window_size": 100, "batch_size": 1, "validation_split": 0, "epochs": 5})
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMTimeSeriesRegressor.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/LSTMTimeSeriesRegressor.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 LSTM
 ~~~~
 
 **path**: ``keras.Sequential.LSTMTimeSeriesRegressor``
 
 **description**: this is a prediction model with double stacked LSTM layers used as a time series regressor. you can read more about it in the `related paper <https://arxiv.org/pdf/1802.04431.pdf>`__.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json>`__.
 
 ====================== =================== ===========================================================================================================================================
 argument                type                description  
 
 **parameters**
 --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  ``X``                  ``numpy.ndarray``   n-dimensional array containing the input sequences for the model 
@@ -44,15 +44,15 @@
  ``y``                  ``numpy.ndarray``   predicted values
 ====================== =================== ===========================================================================================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 100).reshape(1, -1, 1)
     y = np.array([[1]])
     primitive = load_primitive('keras.Sequential.LSTMTimeSeriesRegressor', 
         arguments={"X": X, "y": y, "input_shape":(100, 1), "batch_size": 1, "validation_split": 0})
 
     primitive.fit()
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/MinMaxScaler.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/MinMaxScaler.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MinMaxScaler
 ~~~~~~~~~~~~
 
 **path**: ``sklearn.preprocessing.MinMaxScaler``
 
 **description**: this primitive transforms features by scaling each feature to a given range.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/sklearn.preprocessing.MinMaxScaler.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/sklearn.preprocessing.MinMaxScaler.json>`__.
 
 ==================== =================== =============================================================================================================
 argument              type                description  
 **parameters**
 ------------------------------------------------------------------------------------------------------------------------------------------------------
 
  ``X``                ``numpy.ndarray``   the data used to compute the per-feature minimum and maximum used for later scaling along the features axis
@@ -29,15 +29,15 @@
 ==================== =================== =============================================================================================================
 
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array(range(5)).reshape(-1, 1)
     primitive = load_primitive('sklearn.preprocessing.MinMaxScaler', 
         arguments={"X": X, "feature_range":[0, 1]})
 
     primitive.fit()
     primitive.produce(X=X)
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/SimpleImputer.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/SimpleImputer.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 SimpleImputer
 ~~~~~~~~~~~~~
 
 **path**: ``sklearn.impute.SimpleImputer``
 
 **description**: this primitive is an imputation transformer for filling missing values.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/sklearn.impute.SimpleImputer.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/sklearn.impute.SimpleImputer.json>`__.
 
 ==================== ========================================================= ==========================================
 argument              type                                                      description  
 
 **parameters**
 -------------------------------------------------------------------------------------------------------------------------
  ``X``                ``numpy.ndarray``                                         n-dimensional sequence of values
@@ -31,15 +31,15 @@
  ``X``                ``numpy.ndarray``                                         a transformed version of X
 ==================== ========================================================= ==========================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 4 + [np.nan]).reshape(-1, 1)
     primitive = load_primitive('sklearn.impute.SimpleImputer', 
         arguments={"X": X})
 
     primitive.fit()
     primitive.produce(X=X)
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/TadGAN.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/TadGAN.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ========================== =================== =================================================================================================
 
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 100).reshape(1, -1, 1)
     y = X[:,:, [0]] # signal to reconstruct from X (channel 0)
     primitive = load_primitive('orion.primitives.tadgan.TadGAN', 
         arguments={"X": X, "y":X, "epochs": 5, "batch_size": 1,
                    "iterations_critic": 1})
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/VAE.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/VAE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
  ``y``                      ``numpy.ndarray``   predicted values
 ========================== =================== =================================================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 100).reshape(1, -1, 1)
 
     primitive = load_primitive('orion.primitives.vae.VAE',
         arguments={"X": X, "y": X, "input_shape":(100, 1), "output_shape":(100, 1),
                    "validation_split": 0, "batch_size": 1, "epochs": 5})
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/arima.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/arima.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ARIMA
 ~~~~~
 
 **path**: ``statsmodels.tsa.arima_model.Arima``
 
 **description**: this is an Autoregressive Integrated Moving Average (ARIMA) prediction model.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/statsmodels.tsa.arima_model.Arima.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/statsmodels.tsa.arima_model.Arima.json>`__.
 
 ==================== =================== ==================================================================
 argument              type                description  
 
 **parameters**
 -----------------------------------------------------------------------------------------------------------
 
@@ -31,14 +31,14 @@
  ``y``                ``numpy.ndarray``   predicted values
 ==================== =================== ==================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array(range(100)).reshape(-1, 1)
     primitive = load_primitive('statsmodels.tsa.arima_model.Arima', 
         arguments={"X": X, "steps": 1, })
 
     primitive.produce(X=X)
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/fillna.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/fillna.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  ``X``              ``numpy.ndarray``                                               Array of input sequence with imputed values
 ================== =============================================================== ============================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     X = np.array([1] * 4 + [np.nan]).reshape(-1, 1)
     primitive = load_primitive('orion.primitives.timeseries_preprocessing.fillna', 
         arguments={"X": X, "value": 0})
 
     primitive.fit()
     primitive.produce(X=X)
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/find_anomalies.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/find_anomalies.rst`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  ``y``                      ``numpy.ndarray``    array containing start-index, end-index, score for each anomalous sequence that was found
 ========================== ==================== ===================================================================================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     primitive = load_primitive('orion.primitives.timeseries_anomalies.find_anomalies',
         arguments={"anomaly_padding": 1})
 
     errors = np.array([0.01] * 45 + [1] * 10 + [0.01] * 45)
     index = np.array(range(100))
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/intervals_to_mask.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/intervals_to_mask.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .. highlight:: shell
 
 intervals to mask
 ~~~~~~~~~~~~~~~~~
 
-**path**: ``mlprimitives.custom.timeseries_preprocessing.intervals_to_mask``
+**path**: ``mlstars.custom.timeseries_preprocessing.intervals_to_mask``
 
 **description**: this primitive creates boolean mask from given intervals.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.intervals_to_mask.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/mlstars.custom.timeseries_preprocessing.intervals_to_mask.json>`__.
 
 ==================== =============================== =================================================================================================================================
 argument              type                            description  
 
 **parameters**
 --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
@@ -24,15 +24,15 @@
  ``mask``             ``numpy.ndarray``               array of boolean values, with one boolean value for each index value (True if the index value is contained in a given interval)
 ==================== =============================== =================================================================================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
-    primitive = load_primitive('mlprimitives.custom.timeseries_preprocessing.intervals_to_mask')
+    primitive = load_primitive('mlstars.custom.timeseries_preprocessing.intervals_to_mask')
 
     index = np.array(range(10))
     intervals = [(1, 3), (7, 7)]
 
     primitive.produce(index=index, intervals=intervals)
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/reconstruction_errors.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/reconstruction_errors.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ========================== =================== ======================================================================
 
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     primitive = load_primitive('orion.primitives.timeseries_errors.reconstruction_errors')
     y = np.array([[1]] * 100)
     y_hat = np.array([[.99]] * 100)
 
     errors, predictions = primitive.produce(y=y, y_hat=y_hat)
     print("average error value: {:.2f}".format(errors.mean()))
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/regression_errors.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/regression_errors.rst`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ========================== =================== ======================================================================
 
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     primitive = load_primitive('orion.primitives.timeseries_errors.regression_errors')
     y = np.array([[1]] * 100)
     y_hat = np.array([[.99]] * 100)
 
     errors = primitive.produce(y=y, y_hat=y_hat)
     print("average error value: {:.2f}".format(errors.mean()))
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/rolling_window_sequences.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/rolling_window_sequences.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .. highlight:: shell
 
 rolling window sequence
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-**path**: ``mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences``
+**path**: ``mlstars.custom.timeseries_preprocessing.rolling_window_sequences``
 
 **description**: this primitive generates many sub-sequences of the original sequence. it uses a rolling window approach to create the sub-sequences out of time series data.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/mlstars.custom.timeseries_preprocessing.rolling_window_sequences.json>`__.
 
 ==================== ============================================================== ==================================================================
  argument             type                                                           description  
 
 **parameters**
 ------------------------------------------------------------------------------------------------------------------------------------------------------
 
@@ -37,17 +37,17 @@
  ``target_index``     ``numpy.ndarray``                                              first index value of each target sequence
 ==================== ============================================================== ==================================================================
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
-    primitive = load_primitive('mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences', 
+    primitive = load_primitive('mlstars.custom.timeseries_preprocessing.rolling_window_sequences', 
         arguments={"window_size": 10, "target_size": 1, "step_size": 1, "target_column": 0})
 
     X = np.array([1] * 50).reshape(-1, 1)
     index = np.array(range(50)).reshape(-1, 1)
 
     X, y, index, target_index = primitive.produce(X=X, index=index)
     print("X shape = {}\ny shape = {}\nindex shape = {}\ntarget index shape = {}".format(
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/score_anomalies.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/score_anomalies.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ========================== =================== =================================================================================================
 
 
 .. ipython:: python
     :okwarning:
 
     import numpy as np
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
     primitive = load_primitive('orion.primitives.tadgan.score_anomalies', 
         arguments={"error_smooth_window": 10, "critic_smooth_window": 10,
                    "score_window": 10, "comb": "rec"})
 
     y = np.array([1] * 100).reshape(1, -1, 1)
     y_hat = [0.9] * 40 + [0.5] * 10 + [1.1] * 10 + [0.99] * 40
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives/time_segments_aggregate.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives/time_segments_aggregate.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .. highlight:: shell
 
 time segments aggregate
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-**path**: ``mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate``
+**path**: ``mlstars.custom.timeseries_preprocessing.time_segments_aggregate``
 
 **description**: this primitive creates an equi-spaced time series by aggregating values over fixed specified interval.
 
-see `json <https://github.com/MLBazaar/MLPrimitives/blob/master/mlprimitives/primitives/mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate.json>`__.
+see `json <https://github.com/MLBazaar/mlstars/blob/master/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_aggregate.json>`__.
 
 ==================== =========================================== =============================================================================================================================
 argument              type                                        description  
 **parameters**
 ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  ``X``                ``numpy.ndarray`` or ``pandas.DataFrame``   n-dimensional sequence of values
  ``time_column``      ``str``                                     column of ``X`` that contains time values
@@ -24,17 +24,17 @@
  ``X``                ``numpy.ndarray``                           sequence of aggregated values, one column for each aggregation method
  ``index``            ``numpy.ndarray``                           sequence of index values (first index of each aggregated segment)
 ==================== =========================================== =============================================================================================================================
 
 .. ipython:: python
     :okwarning:
 
-    from mlprimitives import load_primitive
+    from mlstars import load_primitive
 
-    primitive = load_primitive('mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate', 
+    primitive = load_primitive('mlstars.custom.timeseries_preprocessing.time_segments_aggregate', 
         arguments={"time_column": "timestamp", "interval":10, "method":'mean'})
 
     df = pd.DataFrame({
         'timestamp': list(range(50)),
         'value': [1] * 50})
 
     X, index = primitive.produce(X=df)
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/primitives_pipelines/primitives.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/primitives_pipelines/primitives.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _primitives:
 
 ==========
 Primitives
 ==========
 
-Primitives are data processing units. They are defined by the code that performs the actual processing and an annotated ``json`` file. To read more about primitives and their composition, visit `MLPrimitives <https://mlbazaar.github.io/MLPrimitives/>`__.
+Primitives are data processing units. They are defined by the code that performs the actual processing and an annotated ``json`` file. To read more about primitives and their composition, visit `mlstars <https://sintel-dev.github.io/ml-stars/>`__.
 
 Preprocessing
 -------------
 
 .. toctree::
     :maxdepth: 1
```

### Comparing `orion-ml-0.4.1.dev0/docs/user_guides/system/database.rst` & `orion-ml-0.4.2.dev0/docs/user_guides/system/database.rst`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/__init__.py` & `orion-ml-0.4.2.dev0/orion/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 __author__ = """MIT Data To AI Lab"""
 __email__ = 'dailabmit@gmail.com'
-__version__ = '0.4.1.dev0'
+__version__ = '0.4.2.dev0'
 
 import os
 
 from orion.core import Orion
 from orion.functional import detect_anomalies, evaluate_pipeline, fit_pipeline
 
 _BASE_PATH = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `orion-ml-0.4.1.dev0/orion/__main__.py` & `orion-ml-0.4.2.dev0/orion/__main__.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/analysis.py` & `orion-ml-0.4.2.dev0/orion/analysis.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/benchmark.py` & `orion-ml-0.4.2.dev0/orion/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from orion.evaluation import contextual_confusion_matrix
 from orion.progress import TqdmLogger, progress
 
 warnings.simplefilter('ignore')
 
 LOGGER = logging.getLogger(__name__)
 
-BUCKET = 'd3-ai-orion'
+BUCKET = 'sintel-orion'
 S3_URL = 'https://{}.s3.amazonaws.com/{}'
 
 BENCHMARK_PATH = os.path.join(os.path.join(
     os.path.dirname(os.path.abspath(__file__)), '..'),
     'benchmark'
 )
 
@@ -46,19 +46,19 @@
 VERIFIED_PIPELINES = [
     'arima', 'lstm_dynamic_threshold', 'azure', 'tadgan',
     'aer', 'lstm_autoencoder', 'dense_autoencoder', 'vae'
 ]
 
 VERIFIED_PIPELINES_GPU = {
     'arima': 'arima',
-    'lstm_dynamic_threshold': 'lstm_dynamic_threshold_gpu',
+    'lstm_dynamic_threshold': 'lstm_dynamic_threshold',
     'azure': 'azure',
     'tadgan': 'tadgan_without_dropout_gpu',
     'aer': 'aer',
-    'lstm_autoencoder': 'lstm_autoencoder_gpu',
+    'lstm_autoencoder': 'lstm_autoencoder',
     'dense_autoencoder': 'dense_autoencoder',
     'vae': 'vae'
 }
 
 
 def _load_signal(signal, test_split):
     if isinstance(test_split, float):
```

### Comparing `orion-ml-0.4.1.dev0/orion/core.py` & `orion-ml-0.4.2.dev0/orion/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,16 @@
                 metric applied, with the metric name as index.
         """
         if not fit:
             method = self._mlpipeline.predict
         else:
             if not self._fitted:
                 mlpipeline = self._get_mlpipeline()
+            else:
+                mlpipeline = self._mlpipeline
 
             if train_data is not None:
                 # Fit first and then predict
                 mlpipeline.fit(train_data)
                 method = mlpipeline.predict
             else:
                 # Fit and predict at once
```

### Comparing `orion-ml-0.4.1.dev0/orion/data.py` & `orion-ml-0.4.2.dev0/orion/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 LOGGER = logging.getLogger(__name__)
 
 DATA_PATH = os.path.join(
     os.path.dirname(os.path.abspath(__file__)),
     'data'
 )
-BUCKET = 'd3-ai-orion'
+BUCKET = 'sintel-orion'
 S3_URL = 'https://{}.s3.amazonaws.com/{}'
 
 NASA_SIGNALS = (
     'P-1', 'S-1', 'E-1', 'E-2', 'E-3', 'E-4', 'E-5', 'E-6', 'E-7',
     'E-8', 'E-9', 'E-10', 'E-11', 'E-12', 'E-13', 'A-1', 'D-1', 'P-3',
     'D-2', 'D-3', 'D-4', 'A-2', 'A-3', 'A-4', 'G-1', 'G-2', 'D-5',
     'D-6', 'D-7', 'F-1', 'P-4', 'G-3', 'T-1', 'T-2', 'D-8', 'D-9',
```

### Comparing `orion-ml-0.4.1.dev0/orion/evaluation/__init__.py` & `orion-ml-0.4.2.dev0/orion/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/evaluation/common.py` & `orion-ml-0.4.2.dev0/orion/evaluation/common.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/evaluation/contextual.py` & `orion-ml-0.4.2.dev0/orion/evaluation/contextual.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/evaluation/point.py` & `orion-ml-0.4.2.dev0/orion/evaluation/point.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/evaluation/utils.py` & `orion-ml-0.4.2.dev0/orion/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/functional.py` & `orion-ml-0.4.2.dev0/orion/functional.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4340277777777778%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 250)]), "*

 * *                  "'keras.Sequential.LSTMTimeSeriesRegressor': OrderedDict([('epochs', 35)]), "*

 * *                  'delete: […]*

```diff
@@ -1,52 +1,46 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "keras.Sequential.LSTMTimeSeriesRegressor": {
+            "epochs": 35
+        },
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
-            "target_size": 1,
-            "window_size": 100
+            "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "fixed_threshold": true,
             "window_size_portion": 0.33,
             "window_step_size_portion": 0.1
         },
-        "orion.primitives.timeseries_preprocessing.slice_array_by_dims": {
-            "axis": 2,
-            "target_index": 0
-        },
-        "orion.primitives.vae.VAE#1": {
-            "epochs": 35,
-            "verbose": false
-        },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
+    "input_names": {
+        "orion.primitives.timeseries_anomalies.find_anomalies#1": {
+            "index": "target_index"
+        }
+    },
     "output_names": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
-            "index": "X_index",
-            "target_index": "y_index"
-        },
-        "orion.primitives.vae.VAE#1": {
+        "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
-        "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
-        "orion.primitives.vae.VAE",
-        "orion.primitives.timeseries_errors.reconstruction_errors",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
+        "keras.Sequential.LSTMTimeSeriesRegressor",
+        "orion.primitives.timeseries_errors.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/sandbox/vae/vae_viz.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/vae/vae_viz.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8022135416666667%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100), ('target_size', 1)]), "*

 * *                  'delete: '*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_se […]*

```diff
@@ -1,15 +1,15 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "target_size": 1,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "fixed_threshold": true,
             "window_size_portion": 0.33,
@@ -27,15 +27,15 @@
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "output_names": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         },
         "orion.primitives.vae.VAE#1": {
             "y": "y_hat"
         }
     },
@@ -53,26 +53,26 @@
             },
             {
                 "name": "y_hat",
                 "variable": "orion.primitives.vae.VAE#1.y_hat"
             },
             {
                 "name": "index",
-                "variable": "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1.index"
+                "variable": "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1.index"
             },
             {
                 "name": "errors",
                 "variable": "orion.primitives.timeseries_errors.reconstruction_errors#1.errors"
             }
         ]
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "orion.primitives.vae.VAE",
         "orion.primitives.timeseries_errors.reconstruction_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/aer/aer.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7694444444444445%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100), ('target_size', 1)]), "*

 * *                  'delete: '*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_se […]*

```diff
@@ -1,15 +1,15 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "target_size": 1,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.aer.AER#1": {
             "epochs": 35
         },
@@ -37,23 +37,23 @@
     },
     "input_names": {
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "index": "index"
         }
     },
     "output_names": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "orion.primitives.aer.AER",
         "orion.primitives.aer.score_anomalies",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8875%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 250)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                   […]*

```diff
@@ -1,14 +1,14 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "numpy.reshape#1": {
             "newshape": [
                 -1,
@@ -41,17 +41,17 @@
             "y": "X"
         },
         "statsmodels.tsa.arima_model.Arima#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "numpy.reshape",
         "statsmodels.tsa.arima_model.Arima",
         "orion.primitives.timeseries_errors.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_artificialwithanomaly.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_artificialwithanomaly.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_msl.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_msl.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 21600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realadexchange.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realadexchange.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 3600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realawscloudwatch.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realawscloudwatch.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realtraffic.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realtraffic.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_realtweets.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_realtweets.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_smap.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_smap.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 21600,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa1.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa1.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 1,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa2.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa2.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 1,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa3.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa3.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 1,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/arima/arima_yahooa4.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/arima/arima_yahooa4.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1'": "OrderedDict([('target_column', "*

 * *                                                                         "0), ('window_size', "*

 * *                                                                         '250)])',*

 * * "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1'": "OrderedDict([('time_column', "*

 * *                                                                        "'timestamp'), "*

 * *                                  […]*

```diff
@@ -1,13 +1,13 @@
 {
-    "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+    "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
         "target_column": 0,
         "window_size": 250
     },
-    "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+    "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
         "interval": 1,
         "method": "mean",
         "time_column": "timestamp"
     },
     "numpy.reshape#1": {
         "newshape": [
             -1,
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/azure/azure.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/azure/azure.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8777777777777778%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1']}",*

 * * "'primitives'": '{insert: [(0, '*

 * *                 "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate')], delete: "*

 * *                 '[0]}'}*

```diff
@@ -1,10 +1,10 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.azure_anomaly_detector.detect_anomalies#1": {
             "endpoint": "your-endpoint",
             "interval": 21600,
@@ -30,14 +30,14 @@
         },
         "orion.primitives.azure_anomaly_detector.split_sequence#1": {
             "y": "X",
             "y_index": "index"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "orion.primitives.azure_anomaly_detector.split_sequence",
         "orion.primitives.azure_anomaly_detector.detect_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/dense_autoencoder/dense_autoencoder.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7388888888888889%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                   […]*

```diff
@@ -9,19 +9,19 @@
             "target_shape": [
                 100,
                 1
             ],
             "verbose": false,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "fixed_threshold": true,
             "window_size_portion": 0.33,
@@ -38,23 +38,23 @@
             ]
         }
     },
     "output_names": {
         "keras.Sequential.DenseSeq2Seq#1": {
             "y": "y_hat"
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "keras.Sequential.DenseSeq2Seq",
         "orion.primitives.timeseries_errors.reconstruction_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7388888888888889%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                   […]*

```diff
@@ -9,19 +9,19 @@
             "target_shape": [
                 100,
                 1
             ],
             "verbose": false,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "fixed_threshold": true,
             "window_size_portion": 0.33,
@@ -38,23 +38,23 @@
             ]
         }
     },
     "output_names": {
         "keras.Sequential.LSTMSeq2Seq#1": {
             "y": "y_hat"
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "keras.Sequential.LSTMSeq2Seq",
         "orion.primitives.timeseries_errors.reconstruction_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/median_24h_lstm.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.56171875%*

 * *Differences: {"'init_params'": "{'keras.Sequential.LSTMTimeSeriesRegressor': {'epochs': 5}, "*

 * *                  "'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 84600), ('method', "*

 * *                  "'median')]), 'sklear.preprocessing.MinMaxScaler#1': "*

 * *                  "OrderedDict([('feature_range', [-1, 1])]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  […]*

```diff
@@ -1,46 +1,36 @@
 {
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesRegressor": {
-            "epochs": 35
+            "epochs": 5
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
-            "interval": 21600,
-            "method": "mean",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+            "interval": 84600,
+            "method": "median",
             "time_column": "timestamp"
         },
-        "orion.primitives.timeseries_anomalies.find_anomalies#1": {
-            "fixed_threshold": true,
-            "window_size_portion": 0.33,
-            "window_step_size_portion": 0.1
-        },
-        "sklearn.preprocessing.MinMaxScaler#1": {
+        "sklear.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
-    "input_names": {
-        "orion.primitives.timeseries_anomalies.find_anomalies#1": {
-            "index": "target_index"
-        }
-    },
     "output_names": {
         "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "keras.Sequential.LSTMTimeSeriesRegressor",
-        "orion.primitives.timeseries_errors.regression_errors",
+        "orion.primitives.timeseries_anomalies.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_gpu.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/aer/aer_viz.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.52%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100), ('target_size', 1)]), "*

 * *                  "'orion.primitives.timeseries_preprocessing.slice_array_by_dims': "*

 * *                 […]*

```diff
@@ -1,82 +1,73 @@
 {
     "init_params": {
-        "keras.Sequential.LSTMTimeSeriesRegressor": {
-            "epochs": 35,
-            "layers": [
-                {
-                    "class": "keras.layers.CuDNNLSTM",
-                    "parameters": {
-                        "input_shape": "input_shape",
-                        "return_sequences": true,
-                        "units": "lstm_1_units"
-                    }
-                },
-                {
-                    "class": "keras.layers.Dropout",
-                    "parameters": {
-                        "rate": "dropout_1_rate"
-                    }
-                },
-                {
-                    "class": "keras.layers.CuDNNLSTM",
-                    "parameters": {
-                        "return_sequences": false,
-                        "units": "lstm_2_units"
-                    }
-                },
-                {
-                    "class": "keras.layers.Dropout",
-                    "parameters": {
-                        "rate": "dropout_2_rate"
-                    }
-                },
-                {
-                    "class": "keras.layers.Dense",
-                    "parameters": {
-                        "activation": "linear",
-                        "units": "dense_units"
-                    }
-                }
-            ],
-            "verbose": false
-        },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
-            "window_size": 250
+            "target_size": 1,
+            "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
+            "method": "mean",
             "time_column": "timestamp"
         },
+        "orion.primitives.aer.AER#1": {
+            "epochs": 35
+        },
+        "orion.primitives.aer.score_anomalies#1": {
+            "comb": "mult",
+            "lambda_rec": 0.5,
+            "mask": true,
+            "rec_error_type": "dtw"
+        },
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "fixed_threshold": true,
             "window_size_portion": 0.33,
             "window_step_size_portion": 0.1
         },
+        "orion.primitives.timeseries_preprocessing.slice_array_by_dims": {
+            "axis": 2,
+            "target_index": 0
+        },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
-            "index": "target_index"
+            "index": "index"
         }
     },
     "output_names": {
-        "keras.Sequential.LSTMTimeSeriesRegressor#1": {
-            "y": "y_hat"
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+            "index": "X_index",
+            "target_index": "y_index"
         }
     },
+    "outputs": {
+        "default": [
+            {
+                "name": "events",
+                "variable": "orion.primitives.timeseries_anomalies.find_anomalies#1.y"
+            }
+        ],
+        "visualization": [
+            {
+                "name": "generated_timeseries",
+                "variable": "orion.primitives.aer.AER#1.y_hat"
+            }
+        ]
+    },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
-        "keras.Sequential.LSTMTimeSeriesRegressor",
-        "orion.primitives.timeseries_errors.regression_errors",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
+        "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
+        "orion.primitives.aer.AER",
+        "orion.primitives.aer.score_anomalies",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_viz.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_viz.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8984126984126984%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 250)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                   […]*

```diff
@@ -1,17 +1,17 @@
 {
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesRegressor": {
             "epochs": 35
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "fixed_threshold": true,
             "window_size_portion": 0.33,
@@ -45,16 +45,16 @@
             {
                 "name": "generated_timeseries",
                 "variable": "keras.Sequential.LSTMTimeSeriesRegressor#1.y_hat"
             }
         ]
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "keras.Sequential.LSTMTimeSeriesRegressor",
         "orion.primitives.timeseries_errors.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/mean_24h_lstm.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/mean_24h_lstm.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8148148148148149%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 84600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 250)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                   […]*

```diff
@@ -1,17 +1,17 @@
 {
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesRegressor": {
             "epochs": 5
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 84600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "sklear.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
@@ -21,16 +21,16 @@
     },
     "output_names": {
         "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "keras.Sequential.LSTMTimeSeriesRegressor",
         "orion.primitives.timeseries_anomalies.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/median_24h_lstm.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/sum_24h_lstm.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8148148148148149%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 84600), ('method', "*

 * *                  "'sum')]), 'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 250)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                  "'mlprimitives.custom. […]*

```diff
@@ -1,19 +1,19 @@
 {
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesRegressor": {
             "epochs": 5
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 84600,
-            "method": "median",
+            "method": "sum",
             "time_column": "timestamp"
         },
         "sklear.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
@@ -21,16 +21,16 @@
     },
     "output_names": {
         "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "keras.Sequential.LSTMTimeSeriesRegressor",
         "orion.primitives.timeseries_anomalies.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/skew_24h_lstm.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/lstm_dynamic_threshold/skew_24h_lstm.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8148148148148149%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 84600), ('method', "*

 * *                  "'skew')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 250)]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1', "*

 * *                   […]*

```diff
@@ -1,17 +1,17 @@
 {
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesRegressor": {
             "epochs": 5
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 250
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 84600,
             "method": "skew",
             "time_column": "timestamp"
         },
         "sklear.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
@@ -21,16 +21,16 @@
     },
     "output_names": {
         "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "keras.Sequential.LSTMTimeSeriesRegressor",
         "orion.primitives.timeseries_anomalies.regression_errors",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/lstm_dynamic_threshold/sum_24h_lstm.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.fillna.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('name', 'orion.primitives.timeseries_preprocessing.fillna'), "*

 * *            "('contributors', ['Sarah Alnegheimiish <smish@mit.edu>']), ('documentation', ''), "*

 * *            "('description', 'Fill missing values with the last known value.'), ('classifiers', "*

 * *            "OrderedDict([('type', 'preprocessor'), ('subtype', 'transformer')])), ('modalities', "*

 * *            "[]), ('primitive', 'orion.primitives.timeseries_preprocessing.fillna'), ('produce', "*

 * *            "OrderedDict([(' […]*

```diff
@@ -1,36 +1,52 @@
 {
-    "init_params": {
-        "keras.Sequential.LSTMTimeSeriesRegressor": {
-            "epochs": 5
-        },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
-            "target_column": 0,
-            "window_size": 250
-        },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
-            "interval": 84600,
-            "method": "sum",
-            "time_column": "timestamp"
-        },
-        "sklear.preprocessing.MinMaxScaler#1": {
-            "feature_range": [
-                -1,
-                1
-            ]
-        }
+    "classifiers": {
+        "subtype": "transformer",
+        "type": "preprocessor"
     },
-    "output_names": {
-        "keras.Sequential.LSTMTimeSeriesRegressor#1": {
-            "y": "y_hat"
+    "contributors": [
+        "Sarah Alnegheimiish <smish@mit.edu>"
+    ],
+    "description": "Fill missing values with the last known value.",
+    "documentation": "",
+    "hyperparameters": {
+        "fixed": {
+            "axis": {
+                "default": null,
+                "type": "int"
+            },
+            "downcast": {
+                "default": null,
+                "type": "dict"
+            },
+            "limit": {
+                "default": null,
+                "type": "int"
+            },
+            "method": {
+                "default": null,
+                "type": "str"
+            },
+            "value": {
+                "default": null,
+                "type": "int"
+            }
         }
     },
-    "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
-        "sklearn.impute.SimpleImputer",
-        "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
-        "keras.Sequential.LSTMTimeSeriesRegressor",
-        "orion.primitives.timeseries_anomalies.regression_errors",
-        "orion.primitives.timeseries_anomalies.find_anomalies"
-    ]
+    "modalities": [],
+    "name": "orion.primitives.timeseries_preprocessing.fillna",
+    "primitive": "orion.primitives.timeseries_preprocessing.fillna",
+    "produce": {
+        "args": [
+            {
+                "name": "X",
+                "type": "ndarray"
+            }
+        ],
+        "output": [
+            {
+                "name": "X",
+                "type": "ndarray"
+            }
+        ]
+    }
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8111111111111111%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100), ('target_size', 1)]), "*

 * *                  'delete: '*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_se […]*

```diff
@@ -1,15 +1,15 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "target_size": 1,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.tadgan.TadGAN#1": {
             "epochs": 35
         },
@@ -34,26 +34,26 @@
     },
     "input_names": {
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "index": "index"
         }
     },
     "output_names": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         },
         "orion.primitives.tadgan.TadGAN#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "orion.primitives.tadgan.TadGAN",
         "orion.primitives.tadgan.score_anomalies",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_viz.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_viz.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8488888888888889%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100), ('target_size', 1)]), "*

 * *                  'delete: '*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_se […]*

```diff
@@ -1,15 +1,15 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "target_size": 1,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.tadgan.TadGAN#1": {
             "epochs": 35,
             "input_shape": [
@@ -42,15 +42,15 @@
     },
     "input_names": {
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "index": "index"
         }
     },
     "output_names": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         },
         "orion.primitives.tadgan.TadGAN#1": {
             "y": "y_hat"
         }
     },
@@ -65,17 +65,17 @@
             {
                 "name": "generated_timeseries",
                 "variable": "orion.primitives.tadgan.score_anomalies#1.predictions"
             }
         ]
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "orion.primitives.tadgan.TadGAN",
         "orion.primitives.tadgan.score_anomalies",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/pipelines/verified/tadgan/tadgan_without_dropout_gpu.json` & `orion-ml-0.4.2.dev0/orion/pipelines/verified/tadgan/tadgan_without_dropout_gpu.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8111111111111111%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1': "*

 * *                  "OrderedDict([('time_column', 'timestamp'), ('interval', 21600), ('method', "*

 * *                  "'mean')]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1': "*

 * *                  "OrderedDict([('target_column', 0), ('window_size', 100), ('target_size', 1)]), "*

 * *                  'delete: '*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.time_se […]*

```diff
@@ -1,15 +1,15 @@
 {
     "init_params": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "target_size": 1,
             "window_size": 100
         },
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 21600,
             "method": "mean",
             "time_column": "timestamp"
         },
         "orion.primitives.tadgan.TadGAN#1": {
             "epochs": 35,
             "layers_encoder": [
@@ -148,26 +148,26 @@
     },
     "input_names": {
         "orion.primitives.timeseries_anomalies.find_anomalies#1": {
             "index": "index"
         }
     },
     "output_names": {
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "index": "X_index",
             "target_index": "y_index"
         },
         "orion.primitives.tadgan.TadGAN#1": {
             "y": "y_hat"
         }
     },
     "primitives": [
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate",
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences",
         "orion.primitives.timeseries_preprocessing.slice_array_by_dims",
         "orion.primitives.tadgan.TadGAN",
         "orion.primitives.tadgan.score_anomalies",
         "orion.primitives.timeseries_anomalies.find_anomalies"
     ]
 }
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/aer.py` & `orion-ml-0.4.2.dev0/orion/primitives/aer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import logging
 import tempfile
 
 import numpy as np
 import tensorflow as tf
-from mlprimitives.utils import import_object
+from mlstars.utils import import_object
 from numpy import ndarray
 from sklearn.preprocessing import MinMaxScaler
 from tensorflow.keras.layers import Input
 from tensorflow.keras.models import Model
 
 from orion.primitives.timeseries_errors import reconstruction_errors, regression_errors
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/azure_anomaly_detector.py` & `orion-ml-0.4.2.dev0/orion/primitives/azure_anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/detectors.py` & `orion-ml-0.4.2.dev0/orion/primitives/detectors.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/estimators.py` & `orion-ml-0.4.2.dev0/orion/primitives/estimators.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/intervals.py` & `orion-ml-0.4.2.dev0/orion/primitives/intervals.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/keras.Sequential.DenseSeq2Seq.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/keras.Sequential.DenseSeq2Seq.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'primitive'": "'mlstars.adapters.keras.Sequential'"}*

```diff
@@ -174,15 +174,15 @@
                 ],
                 "type": "float"
             }
         }
     },
     "modalities": [],
     "name": "keras.Sequential.DenseSeq2Seq",
-    "primitive": "mlprimitives.adapters.keras.Sequential",
+    "primitive": "mlstars.adapters.keras.Sequential",
     "produce": {
         "args": [
             {
                 "name": "X",
                 "type": "ndarray"
             }
         ],
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/keras.Sequential.LSTMSeq2Seq.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/keras.Sequential.LSTMSeq2Seq.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'primitive'": "'mlstars.adapters.keras.Sequential'"}*

```diff
@@ -135,15 +135,15 @@
                 "default": 250,
                 "type": "int"
             }
         }
     },
     "modalities": [],
     "name": "keras.Sequential.LSTMSeq2Seq",
-    "primitive": "mlprimitives.adapters.keras.Sequential",
+    "primitive": "mlstars.adapters.keras.Sequential",
     "produce": {
         "args": [
             {
                 "name": "X",
                 "type": "ndarray"
             }
         ],
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.aer.AER.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.aer.AER.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.aer.score_anomalies.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.aer.score_anomalies.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.detect_anomalies.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.detect_anomalies.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.split_sequence.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.azure_anomaly_detector.split_sequence.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.detectors.ThresholdDetector.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.detectors.ThresholdDetector.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.estimators.MeanEstimator.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.estimators.MeanEstimator.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.intervals.build_anomaly_intervals.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.intervals.build_anomaly_intervals.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.tadgan.TadGAN.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.tadgan.TadGAN.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.tadgan.score_anomalies.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.tadgan.score_anomalies.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_anomalies.find_anomalies.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_anomalies.find_anomalies.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.reconstruction_errors.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.reconstruction_errors.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.regression_errors.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_errors.regression_errors.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.slice_array_by_dims.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.timeseries_preprocessing.slice_array_by_dims.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/jsons/orion.primitives.vae.VAE.json` & `orion-ml-0.4.2.dev0/orion/primitives/jsons/orion.primitives.vae.VAE.json`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/tadgan.py` & `orion-ml-0.4.2.dev0/orion/primitives/tadgan.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 import tempfile
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-from mlprimitives.utils import import_object
+from mlstars.utils import import_object
 from numpy import ndarray
 from scipy import stats
 from tensorflow.keras import Model
 
 from orion.primitives.timeseries_errors import reconstruction_errors
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/timeseries_anomalies.py` & `orion-ml-0.4.2.dev0/orion/primitives/timeseries_anomalies.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     best_z = min_z
     best_cost = np.inf
     for z in range(min_z, max_z):
         best = fmin(z_cost, z, args=(errors, mean, std), full_output=True, disp=False)
         z, cost = best[0:2]
         if cost < best_cost:
             best_z = z[0]
+            best_cost = cost
 
     return mean + best_z * std
 
 
 def _fixed_threshold(errors, k=4):
     """Calculate the threshold.
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/timeseries_errors.py` & `orion-ml-0.4.2.dev0/orion/primitives/timeseries_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             Array of errors.
     """
     errors = np.abs(y - y_hat)[:, 0]
 
     if not smooth:
         return errors
 
-    smoothing_window = max(1, int(len(y)*smoothing_window))
+    smoothing_window = max(1, int(len(y) * smoothing_window))
     errors = pd.Series(errors).ewm(span=smoothing_window).mean().values
 
     if mask:
         mask_length = int(masking_window * len(errors))
         errors[:mask_length] = min(errors)
     return errors
```

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/timeseries_preprocessing.py` & `orion-ml-0.4.2.dev0/orion/primitives/timeseries_preprocessing.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/primitives/vae.py` & `orion-ml-0.4.2.dev0/orion/primitives/vae.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     - https://github.com/twairball/keras_lstm_vae/blob/master/lstm_vae/vae.py
 """
 import logging
 import tempfile
 
 import numpy as np
 import tensorflow as tf
-from mlprimitives.utils import import_object
+from mlstars.utils import import_object
 from tensorflow.keras import backend as K
 from tensorflow.keras.layers import Input
 from tensorflow.keras.models import Model
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `orion-ml-0.4.1.dev0/orion/progress.py` & `orion-ml-0.4.2.dev0/orion/progress.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/results.py` & `orion-ml-0.4.2.dev0/orion/results.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion/utils.py` & `orion-ml-0.4.2.dev0/orion/utils.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/orion_ml.egg-info/PKG-INFO` & `orion-ml-0.4.2.dev0/orion_ml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orion-ml
-Version: 0.4.1.dev0
+Version: 0.4.2.dev0
 Summary: Orion is a machine learning library built for unsupervised time series anomaly detection.
 Home-page: https://github.com/sintel-dev/Orion
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: orion
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,30 +38,28 @@
 [![Downloads](https://pepy.tech/badge/orion-ml)](https://pepy.tech/project/orion-ml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sintel-dev/Orion/master?filepath=tutorials)
 
 # Orion
 
 A machine learning library for unsupervised time series anomaly detection.
 
-| Important Links                     |                                                                      |
-| ----------------------------------- | -------------------------------------------------------------------- |
-| :computer: **[Website]**            | Check out the Sintel Website for more information about the project. |
-| :book: **[Documentation]**          | Quickstarts, User and Development Guides, and API Reference.         |
-| :star: **[Tutorials]**              | Checkout our notebooks                                               |
-| :octocat: **[Repository]**          | The link to the Github Repository of this library.                   |
-| :scroll: **[License]**              | The repository is published under the MIT License.                   |
-| :keyboard: **[Development Status]** | This software is in its Pre-Alpha stage.                             |
+| Important Links                               |                                                                      |
+| --------------------------------------------- | -------------------------------------------------------------------- |
+| :computer: **[Website]**                      | Check out the Sintel Website for more information about the project. |
+| :book: **[Documentation]**                    | Quickstarts, User and Development Guides, and API Reference.         |
+| :star: **[Tutorials]**                        | Checkout our notebooks                                               |
+| :octocat: **[Repository]**                    | The link to the Github Repository of this library.                   |
+| :scroll: **[License]**                        | The repository is published under the MIT License.                   |
 | [![][Slack Logo] **Community**][Community]    | Join our Slack Workspace for announcements and discussions.          |
 
 [Website]: https://sintel.dev/
 [Documentation]: https://sintel-dev.github.io/Orion
 [Tutorials]: https://github.com/sintel-dev/Orion/tree/master/tutorials
 [Repository]: https://github.com/sintel-dev/Orion
 [License]: https://github.com/sintel-dev/Orion/blob/master/LICENSE
-[Development Status]: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
 [Community]: https://join.slack.com/t/sintel-space/shared_invite/zt-q147oimb-4HcphcxPfDAM0O9_4PaUtw
 [Slack Logo]: https://github.com/sintel-dev/Orion/blob/master/docs/images/slack.png
 
 # Overview
 
 Orion is a machine learning library built for *unsupervised time series anomaly detection*. With a given time series data, we provide a number of “verified” ML pipelines (a.k.a Orion pipelines) that identify rare patterns and flag them for expert review.
 
@@ -107,28 +105,28 @@
 0  1222819200 -0.366359
 1  1222840800 -0.394108
 2  1222862400  0.403625
 3  1222884000 -0.362759
 4  1222905600 -0.370746
 ```
 
-In this example we use `lstm_dynamic_threshold` pipeline and set some hyperparameters (in this case training epochs as 5).
+In this example we use `aer` pipeline and set some hyperparameters (in this case training epochs as 5).
 
 ```python3
 from orion import Orion
 
 hyperparameters = {
-    'keras.Sequential.LSTMTimeSeriesRegressor#1': {
+    'orion.primitives.aer.AER#1': {
         'epochs': 5,
         'verbose': True
     }
 }
 
 orion = Orion(
-    pipeline='lstm_dynamic_threshold',
+    pipeline='aer',
     hyperparameters=hyperparameters
 )
 
 orion.fit(train_data)
 ```
 
 ## Detect anomalies using the fitted pipeline
@@ -150,52 +148,51 @@
 # Leaderboard
 In every release, we run Orion benchmark. We maintain an up-to-date leaderboard with the current scoring of the verified pipelines according to the benchmarking procedure.
 
 We run the benchmark on **11** datasets with their known grounth truth. We record the score of the pipelines on each datasets. To compute the leaderboard table, we showcase the number of wins each pipeline has over the ARIMA pipeline.
 
 | Pipeline                  |  Outperforms ARIMA |
 |---------------------------|--------------------|
-| AER                       |         10         |
+| AER                       |         11         |
 | TadGAN                    |          7         |
-| LSTM Dynamic Thresholding |          8         |
+| LSTM Dynamic Thresholding |          7         |
 | LSTM Autoencoder          |          6         |
 | Dense Autoencoder         |          6         |
-| VAE                       |          6         |
-| Azure                     |          0         |
+| VAE                       |          7         |
+| [GANF](https://arxiv.org/pdf/2202.07857.pdf)                                                  |          6         |
+| [Azure](https://azure.microsoft.com/en-us/products/cognitive-services/anomaly-detector/)      |          0         |
 
 
 You can find the scores of each pipeline on every signal recorded in the [details Google Sheets document](https://docs.google.com/spreadsheets/d/1HaYDjY-BEXEObbi65fwG0om5d8kbRarhpK4mvOZVmqU/edit?usp=sharing). The summarized results can also be browsed in the following [summary Google Sheets document](https://docs.google.com/spreadsheets/d/1ZPUwYH8LhDovVeuJhKYGXYny7472HXVCzhX6D6PObmg/edit?usp=sharing).
 
 # Resources
 
 Additional resources that might be of interest:
 * Learn about [benchmarking pipelines](BENCHMARK.md).
 * Read about [pipeline evaluation](orion/evaluation/README.md).
 * Find out more about [TadGAN](https://arxiv.org/pdf/2009.07769v3.pdf).
 
 # Citation
 
-If you use **Orion** which is part of the **Sintel** ecosystem for your research, please consider citing the following paper:
+If you use **AER** for your research, please consider citing the following paper:
+
+Lawrence Wong, Dongyu Liu, Laure Berti-Equille, Sarah Alnegheimish, Kalyan Veeramachaneni. [AER: Auto-Encoder with Regression for Time Series Anomaly Detection](https://arxiv.org/pdf/2212.13558.pdf).
 
-Sarah Alnegheimish, Dongyu Liu, Carles Sala, Laure Berti-Equille, Kalyan Veeramachaneni. [Sintel: A Machine Learning Framework to Extract Insights from Signals](https://dl.acm.org/doi/pdf/10.1145/3514221.3517910).
 ```
-@inproceedings{alnegheimish2022sintel,
-  title={Sintel: A Machine Learning Framework to Extract Insights from Signals},
-  author={Alnegheimish, Sarah and Liu, Dongyu and Sala, Carles and Berti-Equille, Laure and Veeramachaneni, Kalyan},  
-  booktitle={Proceedings of the 2022 International Conference on Management of Data},
-  pages = {1855–1865},
-  numpages = {11},
-  publisher={Association for Computing Machinery},
-  doi = {10.1145/3514221.3517910},
-  series = {SIGMOD '22},
+@inproceedings{wong2022aer,
+  title={AER: Auto-Encoder with Regression for Time Series Anomaly Detection},
+  author={Wong, Lawrence and Liu, Dongyu and Berti-Equille, Laure and Alnegheimish, Sarah and Veeramachaneni, Kalyan},
+  booktitle={2022 IEEE International Conference on Big Data (IEEE BigData)},
+  pages={1152-1161},
+  doi={10.1109/BigData55660.2022.10020857},
+  organization={IEEE},
   year={2022}
 }
 ```
 
-
 If you use **TadGAN** for your research, please consider citing the following paper:
 
 Alexander Geiger, Dongyu Liu, Sarah Alnegheimish, Alfredo Cuesta-Infante, Kalyan Veeramachaneni. [TadGAN - Time Series Anomaly Detection Using Generative Adversarial Networks](https://arxiv.org/pdf/2009.07769v3.pdf).
 
 ```
 @inproceedings{geiger2020tadgan,
   title={TadGAN: Time Series Anomaly Detection Using Generative Adversarial Networks},
@@ -204,18 +201,44 @@
   pages={33-43},
   doi={10.1109/BigData50022.2020.9378139},
   organization={IEEE},
   year={2020}
 }
 ```
 
+If you use **Orion** which is part of the **Sintel** ecosystem for your research, please consider citing the following paper:
+
+Sarah Alnegheimish, Dongyu Liu, Carles Sala, Laure Berti-Equille, Kalyan Veeramachaneni. [Sintel: A Machine Learning Framework to Extract Insights from Signals](https://dl.acm.org/doi/pdf/10.1145/3514221.3517910).
+```
+@inproceedings{alnegheimish2022sintel,
+  title={Sintel: A Machine Learning Framework to Extract Insights from Signals},
+  author={Alnegheimish, Sarah and Liu, Dongyu and Sala, Carles and Berti-Equille, Laure and Veeramachaneni, Kalyan},  
+  booktitle={Proceedings of the 2022 International Conference on Management of Data},
+  pages={1855–1865},
+  numpages={11},
+  publisher={Association for Computing Machinery},
+  doi={10.1145/3514221.3517910},
+  series={SIGMOD '22},
+  year={2022}
+}
+```
+
 
 History
 =======
 
+## 0.4.1 - 2023-01-31
+
+### Issues resolved
+
+* Move VAE from sandbox to verified – [Issue #377](https://github.com/signals-dev/Orion/issues/377) by @sarahmish
+* Pin ``opencv`` – [Issue #372](https://github.com/signals-dev/Orion/issues/372) by @sarahmish
+* Pin ``scikit-learn`` – [Issue #367](https://github.com/signals-dev/Orion/issues/367) by @sarahmish
+* Fix VAE documentation – [Issue #360](https://github.com/signals-dev/Orion/issues/360) by @sarahmish
+
 ## 0.4.0 - 2022-11-08
 
 This version introduces several new enhancements:
 
 * Support to python 3.8
 * Migrating to Tensorflow 2.0
 * New pipeline, namely ``VAE``, a Variational AutoEncoder model.
```

### Comparing `orion-ml-0.4.1.dev0/orion_ml.egg-info/SOURCES.txt` & `orion-ml-0.4.2.dev0/orion_ml.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,42 @@
 docs/history.rst
 docs/index.rst
 docs/make.bat
 docs/api_reference/evaluation.rst
 docs/api_reference/index.rst
 docs/api_reference/orion.rst
 docs/api_reference/prim.rst
+docs/api_reference/api/orion.Orion.detect.rst
+docs/api_reference/api/orion.Orion.evaluate.rst
+docs/api_reference/api/orion.Orion.fit.rst
+docs/api_reference/api/orion.Orion.load.rst
+docs/api_reference/api/orion.Orion.rst
+docs/api_reference/api/orion.Orion.save.rst
+docs/api_reference/api/orion.benchmark.benchmark.rst
+docs/api_reference/api/orion.detect_anomalies.rst
+docs/api_reference/api/orion.evaluate_pipeline.rst
+docs/api_reference/api/orion.evaluation.contextual_accuracy.rst
+docs/api_reference/api/orion.evaluation.contextual_confusion_matrix.rst
+docs/api_reference/api/orion.evaluation.contextual_f1_score.rst
+docs/api_reference/api/orion.evaluation.contextual_precision.rst
+docs/api_reference/api/orion.evaluation.contextual_recall.rst
+docs/api_reference/api/orion.evaluation.point_accuracy.rst
+docs/api_reference/api/orion.evaluation.point_confusion_matrix.rst
+docs/api_reference/api/orion.evaluation.point_f1_score.rst
+docs/api_reference/api/orion.evaluation.point_precision.rst
+docs/api_reference/api/orion.evaluation.point_recall.rst
+docs/api_reference/api/orion.fit_pipeline.rst
+docs/api_reference/api/orion.primitives.azure_anomaly_detector.detect_anomalies.rst
+docs/api_reference/api/orion.primitives.azure_anomaly_detector.split_sequence.rst
+docs/api_reference/api/orion.primitives.tadgan.TadGAN.rst
+docs/api_reference/api/orion.primitives.tadgan.score_anomalies.rst
+docs/api_reference/api/orion.primitives.timeseries_anomalies.find_anomalies.rst
+docs/api_reference/api/orion.primitives.timeseries_errors.reconstruction_errors.rst
+docs/api_reference/api/orion.primitives.timeseries_errors.regression_errors.rst
+docs/api_reference/api/orion.primitives.timeseries_preprocessing.fillna.rst
 docs/developer_guides/contributing.rst
 docs/developer_guides/index.rst
 docs/getting_started/docker.rst
 docs/getting_started/index.rst
 docs/getting_started/install.rst
 docs/getting_started/quickstart.rst
 docs/images/Scoring.png
@@ -70,35 +98,23 @@
 orion/utils.py
 orion/evaluation/__init__.py
 orion/evaluation/common.py
 orion/evaluation/contextual.py
 orion/evaluation/point.py
 orion/evaluation/utils.py
 orion/pipelines/sandbox/dummy/dummy.json
-orion/pipelines/sandbox/vae/vae.json
-orion/pipelines/sandbox/vae/vae_artificialwithanomaly.json
-orion/pipelines/sandbox/vae/vae_msl.json
-orion/pipelines/sandbox/vae/vae_realadexchange.json
-orion/pipelines/sandbox/vae/vae_realawscloudwatch.json
-orion/pipelines/sandbox/vae/vae_realtraffic.json
-orion/pipelines/sandbox/vae/vae_realtweets.json
-orion/pipelines/sandbox/vae/vae_smap.json
-orion/pipelines/sandbox/vae/vae_viz.json
-orion/pipelines/sandbox/vae/vae_yahooa1.json
-orion/pipelines/sandbox/vae/vae_yahooa2.json
-orion/pipelines/sandbox/vae/vae_yahooa3.json
-orion/pipelines/sandbox/vae/vae_yahooa4.json
 orion/pipelines/verified/aer/aer.json
 orion/pipelines/verified/aer/aer_artificialwithanomaly.json
 orion/pipelines/verified/aer/aer_msl.json
 orion/pipelines/verified/aer/aer_realadexchange.json
 orion/pipelines/verified/aer/aer_realawscloudwatch.json
 orion/pipelines/verified/aer/aer_realtraffic.json
 orion/pipelines/verified/aer/aer_realtweets.json
 orion/pipelines/verified/aer/aer_smap.json
+orion/pipelines/verified/aer/aer_viz.json
 orion/pipelines/verified/aer/aer_yahooa1.json
 orion/pipelines/verified/aer/aer_yahooa2.json
 orion/pipelines/verified/aer/aer_yahooa3.json
 orion/pipelines/verified/aer/aer_yahooa4.json
 orion/pipelines/verified/arima/arima.json
 orion/pipelines/verified/arima/arima_artificialwithanomaly.json
 orion/pipelines/verified/arima/arima_msl.json
@@ -133,28 +149,26 @@
 orion/pipelines/verified/dense_autoencoder/dense_autoencoder_smap.json
 orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa1.json
 orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa2.json
 orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa3.json
 orion/pipelines/verified/dense_autoencoder/dense_autoencoder_yahooa4.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_artificialwithanomaly.json
-orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_gpu.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_msl.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realadexchange.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realawscloudwatch.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realtraffic.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_realtweets.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_smap.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa1.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa2.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa3.json
 orion/pipelines/verified/lstm_autoencoder/lstm_autoencoder_yahooa4.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_artificialwithanomaly.json
-orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_gpu.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_msl.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realadexchange.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realawscloudwatch.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realtraffic.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_realtweets.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_smap.json
 orion/pipelines/verified/lstm_dynamic_threshold/lstm_dynamic_threshold_viz.json
@@ -176,14 +190,27 @@
 orion/pipelines/verified/tadgan/tadgan_smap.json
 orion/pipelines/verified/tadgan/tadgan_viz.json
 orion/pipelines/verified/tadgan/tadgan_without_dropout_gpu.json
 orion/pipelines/verified/tadgan/tadgan_yahooa1.json
 orion/pipelines/verified/tadgan/tadgan_yahooa2.json
 orion/pipelines/verified/tadgan/tadgan_yahooa3.json
 orion/pipelines/verified/tadgan/tadgan_yahooa4.json
+orion/pipelines/verified/vae/vae.json
+orion/pipelines/verified/vae/vae_artificialwithanomaly.json
+orion/pipelines/verified/vae/vae_msl.json
+orion/pipelines/verified/vae/vae_realadexchange.json
+orion/pipelines/verified/vae/vae_realawscloudwatch.json
+orion/pipelines/verified/vae/vae_realtraffic.json
+orion/pipelines/verified/vae/vae_realtweets.json
+orion/pipelines/verified/vae/vae_smap.json
+orion/pipelines/verified/vae/vae_viz.json
+orion/pipelines/verified/vae/vae_yahooa1.json
+orion/pipelines/verified/vae/vae_yahooa2.json
+orion/pipelines/verified/vae/vae_yahooa3.json
+orion/pipelines/verified/vae/vae_yahooa4.json
 orion/primitives/__init__.py
 orion/primitives/aer.py
 orion/primitives/azure_anomaly_detector.py
 orion/primitives/detectors.py
 orion/primitives/estimators.py
 orion/primitives/intervals.py
 orion/primitives/tadgan.py
```

### Comparing `orion-ml-0.4.1.dev0/orion_ml.egg-info/requires.txt` & `orion-ml-0.4.2.dev0/orion_ml.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 s3fs<0.5,>=0.2.2
 mlblocks<0.5,>=0.4.1
-mlprimitives<0.4,>=0.3.2
+ml-stars<0.2,>=0.1.1
 numpy<1.19,>=1.17.4
 pandas<2,>=1
 scikit-learn<1.2,>=0.22
 tabulate<0.9,>=0.8.3
 numba<0.52,>=0.48
 pyts<0.11,>=0.9
 azure-cognitiveservices-anomalydetector<0.4,>=0.3
-xlsxwriter>=1.3.6<1.4
+xlsxwriter<1.4,>=1.3.6
+tqdm>=4.36.1
 h5py<2.11.0,>=2.10.0
 protobuf<4
+opencv-python<4.7
 
 [:python_version < "3.8"]
 tensorflow<2.5,>=2.0
 
 [:python_version >= "3.8"]
 tensorflow<2.5,>=2.2
```

### Comparing `orion-ml-0.4.1.dev0/setup.cfg` & `orion-ml-0.4.2.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.1.dev0
+current_version = 0.4.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `orion-ml-0.4.1.dev0/setup.py` & `orion-ml-0.4.2.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 
 
 install_requires = [
     "tensorflow>=2.0,<2.5;python_version<'3.8'",
     "tensorflow>=2.2,<2.5;python_version>='3.8'",
     's3fs>=0.2.2,<0.5',
     'mlblocks>=0.4.1,<0.5',
-    'mlprimitives>=0.3.2,<0.4',
+    'ml-stars>=0.1.1,<0.2',
     'numpy>=1.17.4,<1.19',
     'pandas>=1,<2',
     'scikit-learn>=0.22,<1.2',
     'tabulate>=0.8.3,<0.9',
     'numba>=0.48,<0.52',
     'pyts>=0.9,<0.11',
     'azure-cognitiveservices-anomalydetector>=0.3,<0.4',
-    'xlsxwriter>=1.3.6<1.4',
+    'xlsxwriter>=1.3.6,<1.4',
+    'tqdm>=4.36.1',
 
     # fix conflict
     'h5py<2.11.0,>=2.10.0',
     'protobuf<4',
+    
+    # fails on python 3.6
+    'opencv-python<4.7',
 ]
 
 setup_requires = [
     'pytest-runner>=2.11.1',
 ]
 
 tests_require = [
@@ -118,10 +122,10 @@
     name='orion-ml',
     packages=find_packages(include=['orion', 'orion.*']),
     python_requires='>=3.6,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/Orion',
-    version='0.4.1.dev0',
+    version='0.4.2.dev0',
     zip_safe=False,
 )
```

### Comparing `orion-ml-0.4.1.dev0/tests/evaluation/test_common.py` & `orion-ml-0.4.2.dev0/tests/evaluation/test_common.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/evaluation/test_contextual.py` & `orion-ml-0.4.2.dev0/tests/evaluation/test_contextual.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/evaluation/test_point.py` & `orion-ml-0.4.2.dev0/tests/evaluation/test_point.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/evaluation/test_utils.py` & `orion-ml-0.4.2.dev0/tests/evaluation/test_utils.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/primitives/test_timeseries_anomalies.py` & `orion-ml-0.4.2.dev0/tests/primitives/test_timeseries_anomalies.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,33 +199,33 @@
 
         assert_allclose(found, expected)
 
     def test_find_anomalies_no_anomalies(self):
         self._run([0, 0, 0, 0], np.array([]))
 
     def test_find_anomalies_one_anomaly(self):
-        self._run([0, 0.5, 0.5, 0], np.array([[1., 4., 0.025]]))
+        self._run([0, 0.5, 0.5, 0], np.array([[1., 4., 0.5]]))
 
     def test_find_anomalies_open_start(self):
-        self._run([0.5, 0.5, 0, 0], np.array([[1., 3., 0.025]]))
+        self._run([0.5, 0.5, 0, 0], np.array([[1., 3., 0.5]]))
 
     def test_find_anomalies_open_end(self):
-        self._run([0, 0, 0.5, 0.5], np.array([[2., 4., 0.025]]))
+        self._run([0, 0, 0.5, 0.5], np.array([[2., 4., 0.5]]))
 
     def test_find_anomalies_two_anomalies(self):
-        self._run([0.5, 0, 0.5, 0], np.array([[1., 4., 0.025]]))
-        self._run([0, 0.5, 0, 0.5], np.array([[1., 4., 0.025]]))
+        self._run([0.5, 0, 0.5, 0], np.array([[1., 4., 0.5]]))
+        self._run([0, 0.5, 0, 0.5], np.array([[1., 4., 0.5]]))
 
     def test_find_anomalies_multiple_non_overlapping_thresholds(self):
         self._run([0, 0, 0.5, 0.5, 0, 0, 0.5, 0.5, 0, 0],
-                  np.array([[2., 4., 0.025], [6., 8., 0.025]]), index=self.INDEX_LONG,
+                  np.array([[2., 4., 0.5], [6., 8., 0.5]]), index=self.INDEX_LONG,
                   window_size=4, window_step_size=4)
 
     def test_find_anomalies_multiple_overlapping_thresholds(self):
-        self._run([0, 0, 0.5, 0.5, 0, 0, 0.5, 0.5, 0, 0], np.array([[2., 9., 0.025]]),
+        self._run([0, 0, 0.5, 0.5, 0, 0, 0.5, 0.5, 0, 0], np.array([[2., 9., 0.5]]),
                   index=self.INDEX_LONG, window_size=4, window_step_size=2)
 
     def test_find_anomalies_lower_threshold(self):
-        self._run([0.5, 0.5, 0, 0], np.array([[1., 4., 0.025]]), lower_threshold=True)
+        self._run([0.5, 0.5, 0, 0], np.array([[1., 4., 0.5]]), lower_threshold=True)
 
     def test_find_anomalies_fixed_threshold(self):
         self._run([0.5, 0.5, 0, 0], np.array([]), fixed_threshold=True)
```

### Comparing `orion-ml-0.4.1.dev0/tests/primitives/test_timeseries_errors.py` & `orion-ml-0.4.2.dev0/tests/primitives/test_timeseries_errors.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/primitives/test_timeseries_preprocessing.py` & `orion-ml-0.4.2.dev0/tests/primitives/test_timeseries_preprocessing.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/requirement_files/latest_requirements.txt` & `orion-ml-0.4.2.dev0/tests/requirement_files/latest_requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,113 @@
-absl-py==1.3.0
+absl-py==1.4.0
 astunparse==1.6.3
-attrs==22.2.0
 azure-cognitiveservices-anomalydetector==0.3.0
 azure-common==1.1.28
-azure-core==1.26.1
-beautifulsoup4==4.11.1
-botocore==1.29.37
-cachetools==5.2.0
+azure-core==1.26.4
+beautifulsoup4==4.12.2
+botocore==1.29.109
+cachetools==5.3.0
 certifi==2022.12.7
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
 click==7.1.2
-cloudpickle==2.2.0
-coverage==7.0.1
+cloudpickle==2.2.1
+coverage==7.2.3
 dask==2022.2.0
 distributed==2022.2.0
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
 featuretools==0.22.0
-fsspec==2022.11.0
+fsspec==2023.1.0
 gast==0.3.3
-google-auth==2.15.0
+google-auth==2.17.2
 google-auth-oauthlib==0.4.6
 google-pasta==0.2.0
 graphviz==0.20.1
-grpcio==1.51.1
+grpcio==1.53.0
 h5py==2.10.0
 HeapDict==1.0.1
 idna==3.4
-imageio==2.23.0
-importlib-metadata==5.2.0
-iniconfig==1.1.1
-invoke==1.7.3
+imageio==2.27.0
+importlib-metadata==6.2.1
+iniconfig==2.0.0
+invoke==2.0.0
 iso639==0.1.4
 isodate==0.6.1
 Jinja2==3.1.2
 jmespath==1.0.1
 joblib==1.2.0
 Keras==2.4.3
 Keras-Preprocessing==1.1.2
 langdetect==1.0.9
-lightfm==1.16
+lightfm==1.17
 llvmlite==0.34.0
 locket==1.0.0
 Markdown==2.6.11
 markdown-rundoc==0.3.1
-MarkupSafe==2.1.1
+MarkupSafe==2.1.2
 mlblocks==0.4.1
-mlprimitives==0.3.2
-msgpack==1.0.4
+mlprimitives==0.3.4
+msgpack==1.0.5
 msrest==0.7.1
 networkx==2.6.3
-nltk==3.8
+nltk==3.8.1
 numba==0.51.2
 numpy==1.18.5
 oauthlib==3.2.2
 opencv-python==4.6.0.66
 opt-einsum==3.3.0
-orion-ml==0.4.1.dev0
-packaging==22.0
+orion-ml==0.4.2.dev0
+packaging==23.0
 pandas==1.3.5
 partd==1.3.0
 patsy==0.5.3
-Pillow==9.3.0
+Pillow==9.5.0
 pluggy==1.0.0
-prompt-toolkit==3.0.36
+prompt-toolkit==3.0.38
 protobuf==3.20.3
 psutil==5.9.4
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
-Pygments==2.13.0
-pytest==7.2.0
+Pygments==2.14.0
+pytest==7.3.0
 pytest-cov==4.0.0
 python-dateutil==2.8.2
 python-louvain==0.13
 pyts==0.10.0
-pytz==2022.7
+pytz==2023.3
 PyWavelets==1.3.0
 PyYAML==6.0
 regex==2022.10.31
-requests==2.28.1
+requests==2.28.2
 requests-oauthlib==1.3.1
 rsa==4.9
 rundoc==0.4.5
 s3fs==0.4.2
 scikit-image==0.19.3
 scikit-learn==1.0.2
 scipy==1.7.3
 six==1.16.0
 sortedcontainers==2.4.0
-soupsieve==2.3.2.post1
+soupsieve==2.4
 statsmodels==0.12.2
 tabulate==0.8.10
 tblib==1.7.0
-tensorboard==2.11.0
+tensorboard==2.11.2
 tensorboard-data-server==0.6.1
 tensorboard-plugin-wit==1.8.1
 tensorflow==2.3.4
 tensorflow-estimator==2.3.0
-termcolor==2.1.1
+termcolor==2.2.0
 threadpoolctl==3.1.0
 tifffile==2021.11.2
 tomli==2.0.1
 toolz==0.12.0
 tornado==6.2
-tqdm==4.64.1
-typing_extensions==4.4.0
-urllib3==1.26.13
-wcwidth==0.2.5
-Werkzeug==2.2.2
-wrapt==1.14.1
+tqdm==4.65.0
+typing_extensions==4.5.0
+urllib3==1.26.15
+wcwidth==0.2.6
+Werkzeug==2.2.3
+wrapt==1.15.0
 xgboost==0.90
-XlsxWriter==3.0.3
+XlsxWriter==1.3.9
 zict==2.2.0
-zipp==3.11.0
+zipp==3.15.0
```

### Comparing `orion-ml-0.4.1.dev0/tests/test_analysis.py` & `orion-ml-0.4.2.dev0/tests/test_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from orion import analysis
 
 
 @pytest.fixture
 def tadgan_hyperparameters():
     return {
-        "mlprimitives.custom.timeseries_preprocessing.time_segments_aggregate#1": {
+        "mlstars.custom.timeseries_preprocessing.time_segments_aggregate#1": {
             "interval": 1,
             "time_column": "timestamp",
         },
-        "mlprimitives.custom.timeseries_preprocessing.rolling_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.rolling_window_sequences#1": {
             "target_column": 0,
             "window_size": 100,
             "target_size": 1
         },
         'orion.primitives.tadgan.TadGAN#1': {
             'epochs': 2,
             'verbose': False
```

### Comparing `orion-ml-0.4.1.dev0/tests/test_benchmark.py` & `orion-ml-0.4.2.dev0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/test_core.py` & `orion-ml-0.4.2.dev0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `orion-ml-0.4.1.dev0/tests/test_data.py` & `orion-ml-0.4.2.dev0/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     # run
     returned = download('a_signal_name')
 
     # assert
     assert returned == read_csv_mock.return_value
 
-    expected_url = 'https://d3-ai-orion.s3.amazonaws.com/a_signal_name.csv'
+    expected_url = 'https://sintel-orion.s3.amazonaws.com/a_signal_name.csv'
     read_csv_mock.assert_called_once_with(expected_url)
 
     expected_filename = os.path.join(DATA_PATH, 'a_signal_name.csv')
     returned.to_csv.assert_called_once_with(expected_filename, index=False)
 
 
 # ########### #
```

### Comparing `orion-ml-0.4.1.dev0/tests/test_functional.py` & `orion-ml-0.4.2.dev0/tests/test_functional.py`

 * *Files identical despite different names*

