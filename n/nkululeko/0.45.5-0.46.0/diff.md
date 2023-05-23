# Comparing `tmp/nkululeko-0.45.5.tar.gz` & `tmp/nkululeko-0.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.45.5.tar", last modified: Mon May 22 09:13:44 2023, max compression
+gzip compressed data, was "nkululeko-0.46.0.tar", last modified: Tue May 23 12:36:44 2023, max compression
```

## Comparing `nkululeko-0.45.5.tar` & `nkululeko-0.46.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-22 09:13:44.156439 nkululeko-0.45.5/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6029 2023-05-22 09:13:10.000000 nkululeko-0.45.5/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.5/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17051 2023-05-22 09:13:44.156439 nkululeko-0.45.5/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10469 2023-05-11 10:04:04.000000 nkululeko-0.45.5/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-22 09:13:44.156439 nkululeko-0.45.5/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.45.5/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.5/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.5/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.5/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.5/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-22 09:12:46.000000 nkululeko-0.45.5/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.5/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.5/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.5/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.45.5/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.5/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20481 2023-05-11 13:35:15.000000 nkululeko-0.45.5/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.45.5/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3728 2023-05-11 10:12:48.000000 nkululeko-0.45.5/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.5/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.5/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.5/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.5/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.5/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.5/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.5/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.5/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.5/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.5/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.5/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.5/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.5/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.5/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.5/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.5/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.5/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.5/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.5/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.5/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.5/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.5/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.5/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.5/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.5/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.5/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.5/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.5/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.5/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.5/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.5/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.5/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.45.5/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.5/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.5/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.5/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.5/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.5/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.45.5/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.5/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8381 2023-05-11 09:13:01.000000 nkululeko-0.45.5/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-22 09:13:44.156439 nkululeko-0.45.5/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17051 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.5/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-05-22 09:13:44.156439 nkululeko-0.45.5/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.45.5/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-23 12:36:44.480542 nkululeko-0.46.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6151 2023-05-23 12:27:48.000000 nkululeko-0.46.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.46.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17173 2023-05-23 12:36:44.480542 nkululeko-0.46.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10469 2023-05-11 10:04:04.000000 nkululeko-0.46.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-23 12:36:44.476542 nkululeko-0.46.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.46.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.46.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.46.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.46.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.46.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-05-23 12:26:49.000000 nkululeko-0.46.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-23 12:23:55.000000 nkululeko-0.46.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.46.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.46.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.46.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.46.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20319 2023-05-23 12:09:53.000000 nkululeko-0.46.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.46.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.46.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.46.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.46.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.46.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.46.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.46.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.46.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.46.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2130 2023-05-23 11:53:38.000000 nkululeko-0.46.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.46.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.46.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.46.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.46.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.46.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.46.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.46.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.46.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.46.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.46.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.46.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.46.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.46.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.46.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.46.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.46.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.46.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.46.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.46.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.46.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.46.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.46.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.46.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.46.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.46.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.46.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.46.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.46.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.46.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.46.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.46.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.46.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.46.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-23 12:36:44.476542 nkululeko-0.46.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17173 2023-05-23 12:36:44.000000 nkululeko-0.46.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-23 12:36:44.000000 nkululeko-0.46.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-23 12:36:44.000000 nkululeko-0.46.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-23 12:36:44.000000 nkululeko-0.46.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-23 12:36:44.000000 nkululeko-0.46.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.46.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-05-23 12:36:44.480542 nkululeko-0.46.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.46.0/setup.py
```

### Comparing `nkululeko-0.45.5/CHANGELOG.md` & `nkululeko-0.46.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.46.0
+--------------
+* added warnings for non-existent parameters
+* added sample selection for scatter plotting
+
 Version 0.45.4
 --------------
 * added version attribute to setup.cfg
 
 Version 0.45.4
 --------------
 * added __version__ attribute
```

### Comparing `nkululeko-0.45.5/LICENSE` & `nkululeko-0.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/PKG-INFO` & `nkululeko-0.46.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.5
+Version: 0.46.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -208,14 +208,19 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.46.0
+--------------
+* added warnings for non-existent parameters
+* added sample selection for scatter plotting
+
 Version 0.45.4
 --------------
 * added version attribute to setup.cfg
 
 Version 0.45.4
 --------------
 * added __version__ attribute
```

### Comparing `nkululeko-0.45.5/README.md` & `nkululeko-0.46.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/augment.py` & `nkululeko-0.46.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/augmenter.py` & `nkululeko-0.46.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/cacheddataset.py` & `nkululeko-0.46.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/dataset.py` & `nkululeko-0.46.0/nkululeko/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
         # except KeyError:
         #     pass
         # remember in case they get encoded later
         df['class_label'] = df[target]
         return df
 
     def check_continuous_classification(self):
-        datatype = self.util.config_val('DATA', 'type', 'dummy')
+        datatype = self.util.config_val('DATA', 'type', 'False')
         if self.util.exp_is_classification() and datatype == 'continuous':
             return True
         return False
 
     def map_continuous_classification(self, df):
         """Map labels to bins for continuous data that should be classified"""
         if self.check_continuous_classification():
```

### Comparing `nkululeko-0.45.5/nkululeko/dataset_csv.py` & `nkululeko-0.46.0/nkululeko/dataset_csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     def load(self):
         """Load the dataframe with files, speakers and task labels"""
         self.got_target, self.got_speaker, self.got_gender = False, False, False
         root = self.util.config_val_data(self.name, '', '')
         absolut_path = eval(self.util.config_val_data(self.name, 'absolute_path', True))
         self.util.debug(f'loading {self.name}')
 #        df = pd.read_csv(root, index_col='file')       
+        if not os.path.isabs(root):
+            exp_root = self.util.config_val('EXP', 'root', '')
+            root = exp_root + root
         df = audformat.utils.read_csv(root)       
         if not absolut_path:
             # add the root folder to the relative paths of the files 
             if audformat.index_type(df.index) == 'segmented':
                 df = df.set_index(df.index.set_levels(df.index.levels[0].map(lambda x: os.path.dirname(root)+'/'+x), 0))
             else:
                 df = df.set_index(df.index.to_series().apply(lambda x: os.path.dirname(root)+'/'+x))
```

### Comparing `nkululeko-0.45.5/nkululeko/dataset_ravdess.py` & `nkululeko-0.46.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/demo.py` & `nkululeko-0.46.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/demo_predictor.py` & `nkululeko-0.46.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/experiment.py` & `nkululeko-0.46.0/nkululeko/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,18 +337,16 @@
 
         # check if a scatterplot should be done
         scatter_var = eval(self.util.config_val('EXPL', 'scatter', 'False'))
         if scatter_var:
             scatters = ast.literal_eval(glob_conf.config['EXPL']['scatter'])
             if self.util.exp_is_classification():
                 plots = Plots()
-                all_feats = pd.concat([self.feats_train, self.feats_test])
-                all_labels = pd.concat([self.df_train['class_label'], self.df_test['class_label']])
                 for scatter in scatters:
-                    plots.scatter_plot(all_feats, all_labels, scatter)
+                    plots.scatter_plot(df_feats, df_labels['class_label'], scatter)
             else:
                  self.util.debug('can\'t do scatterplot if not classification')
 
 
         # check if a tsne should be plotted
         tsne = eval(self.util.config_val('EXPL', 'tsne', 'False'))
         if tsne:
```

### Comparing `nkululeko-0.45.5/nkululeko/explore.py` & `nkululeko-0.46.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_analyser.py` & `nkululeko-0.46.0/nkululeko/feats_analyser.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             f'{str(df_imp.feats.values)}\n')
 
         df_imp.to_csv(file_name, mode='a')
 
                 # check if feature distributions should be plotted
         plot_feats = self.util.config_val('EXPL', 'feature_distributions', False)
         if plot_feats: 
+            sample_selection = self.util.config_val('EXPL', 'sample_selection', 'all')
             if self.util.exp_is_classification():
                 for feature in df_imp.feats:
                     # plot_feature(self, title, feature, label, df_labels, df_features):
                     _plots = Plots()
-                    _plots.plot_feature(plot_feats, feature, 'class_label', self.df_labels, self.X)
+                    _plots.plot_feature(sample_selection, feature, 'class_label', self.df_labels, self.X)
             else:
                 self.util.debug('can\'t plot feature distributions if not classification')
```

### Comparing `nkululeko-0.45.5/nkululeko/feats_audmodel.py` & `nkululeko-0.46.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.46.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_clap.py` & `nkululeko-0.46.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_import.py` & `nkululeko-0.46.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_mld.py` & `nkululeko-0.46.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_opensmile.py` & `nkululeko-0.46.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_oxbow.py` & `nkululeko-0.46.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_praat.py` & `nkululeko-0.46.0/nkululeko/feats_praat.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         storage = f'{store}{self.name}.{store_format}'
         extract = self.util.config_val('FEATS', 'needs_feature_extraction', False)
         no_reuse = eval(self.util.config_val('FEATS', 'no_reuse', 'False'))
         if extract or no_reuse or not os.path.isfile(storage):
             self.util.debug('extracting Praat features, this might take a while...')
             self.df = feinberg_praat.compute_features(self.data_df.index)
             self.df = self.df.set_index(self.data_df.index)
+            for i, col in enumerate(self.df.columns):
+                if self.df[col].isnull().values.any():
+                    self.util.debug(f'{col} includes {self.df[col].isnull().sum()} nan, inserting mean values')
+                    self.df[col] = self.df[col].fillna(self.df[col].mean())
+
             self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config['DATA']['needs_feature_extraction'] = 'false'
             except KeyError:
                 pass
         else:
             self.util.debug('reusing extracted Praat features.')
```

### Comparing `nkululeko-0.45.5/nkululeko/feats_trill.py` & `nkululeko-0.46.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feats_wav2vec2.py` & `nkululeko-0.46.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feature_extractor.py` & `nkululeko-0.46.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/featureset.py` & `nkululeko-0.46.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/feinberg_praat.py` & `nkululeko-0.46.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/filter_data.py` & `nkululeko-0.46.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/loss_ccc.py` & `nkululeko-0.46.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/loss_softf1loss.py` & `nkululeko-0.46.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model.py` & `nkululeko-0.46.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_cnn.py` & `nkululeko-0.46.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_gmm.py` & `nkululeko-0.46.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_knn.py` & `nkululeko-0.46.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_knn_reg.py` & `nkululeko-0.46.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_mlp.py` & `nkululeko-0.46.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_mlp_regression.py` & `nkululeko-0.46.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/model_svm.py` & `nkululeko-0.46.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/modelrunner.py` & `nkululeko-0.46.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/nkululeko.py` & `nkululeko-0.46.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/plots.py` & `nkululeko-0.46.0/nkululeko/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,16 @@
             plt.tight_layout()
             plt.savefig(f'{fig_dir}{filename}.{self.format}')
             fig.clear()
             plt.close(fig)
 
     def scatter_plot(self, feats, labels, dimred_type):
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
-        filename = self.util.get_exp_name()+dimred_type
+        sample_selection = self.util.config_val('EXPL', 'sample_selection', 'all')
+        filename = self.util.get_exp_name()+sample_selection+'_'+dimred_type
         filename = f'{fig_dir}{filename}.{self.format}'
         self.util.debug(f'computing {dimred_type}, this might take a while...')
         data = None
         if dimred_type == 'tsne':
             data = self.getTsne(feats)
         elif dimred_type == 'umap':
             import umap
```

### Comparing `nkululeko-0.45.5/nkululeko/reporter.py` & `nkululeko-0.46.0/nkululeko/reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             text_file.write(rpt)
 
     def print_results(self, epoch):
         """Print all evaluation values to text file"""
         res_dir = self.util.get_path('res_dir')
         file_name = f'{res_dir}{self.util.get_exp_name()}_{epoch}.txt'
         if self.util.exp_is_classification():
-            data_type = self.util.config_val('DATA', 'type', 'whatever')
+            data_type = self.util.config_val('DATA', 'type', 'False')
             if data_type == 'continuous' or data_type == 'continous':
                 labels = ast.literal_eval(glob_conf.config['DATA']['labels'])
             else:
                 labels = glob_conf.label_encoder.classes_
             try:
                 rpt = classification_report(self.truths, self.preds, target_names=labels, output_dict=True)
             except ValueError as e:
```

### Comparing `nkululeko-0.45.5/nkululeko/runmanager.py` & `nkululeko-0.46.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/scaler.py` & `nkululeko-0.46.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/test.py` & `nkululeko-0.46.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/test_predictor.py` & `nkululeko-0.46.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/nkululeko/util.py` & `nkululeko-0.46.0/nkululeko/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import os.path
 import configparser
 import audformat
 import pandas as pd
 
 class Util:
 
+    stopvals = [False, 'False', 'classification', 'png']
+
     def __init__(self):
         self.got_data_roots = self.config_val('DATA', 'root_folders', False)
         if self.got_data_roots:
             # if there is a global data rootfolder file, read from there
             if not os.path.isfile(self.got_data_roots):
                 self.error(f'no such file: {self.got_data_roots}')
             self.data_roots = configparser.ConfigParser()
@@ -65,15 +67,19 @@
             if self.got_data_roots:
                 try:
                     if len(key)>0:
                         return self.data_roots['DATA'][dataset+'.'+key]
                     else:
                         return self.data_roots['DATA'][dataset]
                 except KeyError:
+                    if not default in self.stopvals:
+                        self.debug(f'value for {key} not found, using default: {default}')
                     return default
+            if not default in self.stopvals:
+                self.debug(f'value for {key} not found, using default: {default}')
             return default
 
 
 
     def get_save_name(self):
         """Return a relative path to a name to save the experiment"""
         store = self.get_path('store')
@@ -174,21 +180,25 @@
         print(df.head(1)
         )
     def config_val(self, section, key, default):
         try:
             # strategy is either traintest (default)  or cross_data
             return glob_conf.config[section][key]
         except KeyError:
+            if not default in self.stopvals:
+                self.debug(f'value for {key} not found, using default: {default}')
             return default
             
     def config_val_list(self, section, key, default):
         try:
             # strategy is either traintest (default)  or cross_data
             return ast.literal_eval(glob_conf.config[section][key])
         except KeyError:
+            if not default in self.stopvals:
+                self.debug(f'value for {key} not found, using default: {default}')
             return default
             
     def get_labels(self):
         # try:
         #     labels = glob_conf.label_encoder.classes_
         # except AttributeError:
         labels = ast.literal_eval(glob_conf.config['DATA']['labels'])
```

### Comparing `nkululeko-0.45.5/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.46.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.5
+Version: 0.46.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -208,14 +208,19 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.46.0
+--------------
+* added warnings for non-existent parameters
+* added sample selection for scatter plotting
+
 Version 0.45.4
 --------------
 * added version attribute to setup.cfg
 
 Version 0.45.4
 --------------
 * added __version__ attribute
```

### Comparing `nkululeko-0.45.5/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.46.0/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.5/setup.cfg` & `nkululeko-0.46.0/setup.cfg`

 * *Files identical despite different names*

