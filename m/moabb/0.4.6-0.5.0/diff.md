# Comparing `tmp/moabb-0.4.6.tar.gz` & `tmp/moabb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moabb-0.4.6.tar", max compression
+gzip compressed data, was "moabb-0.5.0.tar", max compression
```

## Comparing `moabb-0.4.6.tar` & `moabb-0.5.0.tar`

### file list

```diff
@@ -1,60 +1,81 @@
--rw-r--r--   0        0        0     1524 2021-06-21 22:26:19.960528 moabb-0.4.6/LICENSE
--rw-r--r--   0        0        0    10610 2022-04-07 12:26:21.898245 moabb-0.4.6/README.md
--rw-r--r--   0        0        0       76 2022-04-07 12:26:21.898934 moabb-0.4.6/moabb/__init__.py
--rw-r--r--   0        0        0     2299 2021-06-21 22:25:58.207651 moabb-0.4.6/moabb/analysis/__init__.py
--rw-r--r--   0        0        0    10869 2021-06-21 22:25:59.447204 moabb-0.4.6/moabb/analysis/meta_analysis.py
--rw-r--r--   0        0        0     9279 2021-06-21 22:25:58.049863 moabb-0.4.6/moabb/analysis/plotting.py
--rw-r--r--   0        0        0     8503 2022-04-07 12:26:21.899180 moabb-0.4.6/moabb/analysis/results.py
--rw-r--r--   0        0        0    17750 2022-04-07 10:18:18.255273 moabb-0.4.6/moabb/datasets/Lee2019.py
--rw-r--r--   0        0        0     7394 2022-04-07 10:18:18.255534 moabb-0.4.6/moabb/datasets/Weibo2014.py
--rw-r--r--   0        0        0     4858 2022-04-07 10:18:18.255747 moabb-0.4.6/moabb/datasets/Zhou2016.py
--rw-r--r--   0        0        0     1247 2022-04-07 12:26:21.899425 moabb-0.4.6/moabb/datasets/__init__.py
--rw-r--r--   0        0        0     2176 2021-06-21 22:26:02.038274 moabb-0.4.6/moabb/datasets/alex_mi.py
--rw-r--r--   0        0        0     7150 2021-10-20 01:55:47.554979 moabb-0.4.6/moabb/datasets/base.py
--rw-r--r--   0        0        0    17737 2022-04-07 10:18:18.256224 moabb-0.4.6/moabb/datasets/bbci_eeg_fnirs.py
--rw-r--r--   0        0        0    40324 2021-06-21 22:26:05.637816 moabb-0.4.6/moabb/datasets/bnci.py
--rw-r--r--   0        0        0    28297 2022-04-07 12:26:21.899708 moabb-0.4.6/moabb/datasets/braininvaders.py
--rw-r--r--   0        0        0     8197 2021-06-21 22:26:01.748928 moabb-0.4.6/moabb/datasets/download-tqdm.py
--rw-r--r--   0        0        0     8632 2022-04-07 10:18:18.256483 moabb-0.4.6/moabb/datasets/download.py
--rw-r--r--   0        0        0     7224 2021-06-21 22:26:06.146523 moabb-0.4.6/moabb/datasets/epfl.py
--rw-r--r--   0        0        0     2642 2021-09-03 14:11:20.362598 moabb-0.4.6/moabb/datasets/fake.py
--rw-r--r--   0        0        0     5055 2021-06-21 22:26:05.346069 moabb-0.4.6/moabb/datasets/gigadb.py
--rw-r--r--   0        0        0    14291 2022-04-07 10:18:18.256667 moabb-0.4.6/moabb/datasets/huebner_llp.py
--rw-r--r--   0        0        0     3906 2021-08-19 14:10:27.000975 moabb-0.4.6/moabb/datasets/mpi_mi.py
--rw-r--r--   0        0        0     7350 2021-06-21 22:26:01.563245 moabb-0.4.6/moabb/datasets/neiry.py
--rw-r--r--   0        0        0     6403 2022-04-07 10:18:18.256921 moabb-0.4.6/moabb/datasets/physionet_mi.py
--rw-r--r--   0        0        0     4062 2022-04-07 10:18:18.257190 moabb-0.4.6/moabb/datasets/schirrmeister2017.py
--rw-r--r--   0        0        0     7925 2022-04-07 10:18:18.258051 moabb-0.4.6/moabb/datasets/sosulski2019.py
--rw-r--r--   0        0        0     3349 2021-06-21 22:26:05.241783 moabb-0.4.6/moabb/datasets/ssvep_exo.py
--rw-r--r--   0        0        0    20352 2022-04-07 10:18:18.258569 moabb-0.4.6/moabb/datasets/ssvep_mamem.py
--rw-r--r--   0        0        0     3550 2021-06-21 22:26:01.110228 moabb-0.4.6/moabb/datasets/ssvep_nakanishi.py
--rw-r--r--   0        0        0     7144 2021-06-21 22:26:06.837533 moabb-0.4.6/moabb/datasets/ssvep_wang.py
--rw-r--r--   0        0        0     5886 2021-06-21 22:26:06.355646 moabb-0.4.6/moabb/datasets/upper_limb.py
--rw-r--r--   0        0        0     4305 2021-06-21 22:26:05.488263 moabb-0.4.6/moabb/datasets/utils.py
--rw-r--r--   0        0        0      428 2021-06-21 22:25:59.756120 moabb-0.4.6/moabb/evaluations/__init__.py
--rw-r--r--   0        0        0     6951 2021-10-20 01:55:47.557214 moabb-0.4.6/moabb/evaluations/base.py
--rw-r--r--   0        0        0    21963 2022-04-07 10:18:18.259092 moabb-0.4.6/moabb/evaluations/evaluations.py
--rw-r--r--   0        0        0      449 2021-06-21 22:26:17.306490 moabb-0.4.6/moabb/paradigms/__init__.py
--rw-r--r--   0        0        0     8835 2021-10-20 01:55:47.557947 moabb-0.4.6/moabb/paradigms/base.py
--rw-r--r--   0        0        0    13072 2021-10-20 01:55:47.558454 moabb-0.4.6/moabb/paradigms/motor_imagery.py
--rw-r--r--   0        0        0     9543 2021-09-03 14:11:20.366170 moabb-0.4.6/moabb/paradigms/p300.py
--rw-r--r--   0        0        0     9217 2021-06-21 22:26:18.689036 moabb-0.4.6/moabb/paradigms/ssvep.py
--rw-r--r--   0        0        0      379 2021-10-20 01:55:47.558893 moabb-0.4.6/moabb/pipelines/__init__.py
--rw-r--r--   0        0        0    18794 2021-10-20 01:55:47.559923 moabb-0.4.6/moabb/pipelines/classification.py
--rw-r--r--   0        0        0     2187 2021-06-21 22:26:09.920011 moabb-0.4.6/moabb/pipelines/csp.py
--rw-r--r--   0        0        0     2011 2021-06-21 22:26:10.090218 moabb-0.4.6/moabb/pipelines/features.py
--rw-r--r--   0        0        0     6085 2021-10-20 01:55:47.560495 moabb-0.4.6/moabb/pipelines/utils.py
--rwxr-xr-x   0        0        0     6325 2021-06-21 22:25:57.654125 moabb-0.4.6/moabb/run.py
--rw-r--r--   0        0        0      299 2021-06-21 22:26:07.653722 moabb-0.4.6/moabb/tests/__init__.py
--rw-r--r--   0        0        0     5064 2021-06-21 22:26:07.343044 moabb-0.4.6/moabb/tests/analysis.py
--rw-r--r--   0        0        0     2059 2021-06-21 22:26:07.536361 moabb-0.4.6/moabb/tests/datasets.py
--rw-r--r--   0        0        0     4603 2021-06-21 22:26:07.441337 moabb-0.4.6/moabb/tests/download.py
--rw-r--r--   0        0        0     7885 2022-04-07 12:26:21.899978 moabb-0.4.6/moabb/tests/evaluations.py
--rw-r--r--   0        0        0    17586 2021-09-03 14:11:20.367146 moabb-0.4.6/moabb/tests/paradigms.py
--rw-r--r--   0        0        0      260 2021-06-21 22:26:09.341348 moabb-0.4.6/moabb/tests/test_pipelines/LogVar.yml
--rw-r--r--   0        0        0      216 2021-06-21 22:26:09.235324 moabb-0.4.6/moabb/tests/test_pipelines/SSVEP_CCA.yml
--rw-r--r--   0        0        0     2509 2022-04-07 10:18:18.259497 moabb-0.4.6/moabb/tests/util_tests.py
--rw-r--r--   0        0        0     1850 2021-09-03 14:11:20.367758 moabb-0.4.6/moabb/utils.py
--rw-r--r--   0        0        0     1223 2022-04-07 12:26:21.900165 moabb-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    11985 2022-04-07 12:27:14.977795 moabb-0.4.6/setup.py
--rw-r--r--   0        0        0    11923 2022-04-07 12:27:14.978654 moabb-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1524 2022-02-02 13:27:15.071351 moabb-0.5.0/LICENSE
+-rw-r--r--   0        0        0    12450 2023-03-20 21:52:28.967817 moabb-0.5.0/README.md
+-rw-r--r--   0        0        0      134 2023-05-23 01:53:37.595092 moabb-0.5.0/moabb/__init__.py
+-rw-r--r--   0        0        0     2317 2023-04-19 06:19:41.753656 moabb-0.5.0/moabb/analysis/__init__.py
+-rw-r--r--   0        0        0    10920 2023-01-03 09:13:10.073480 moabb-0.5.0/moabb/analysis/meta_analysis.py
+-rw-r--r--   0        0        0    11242 2023-04-19 06:19:41.754275 moabb-0.5.0/moabb/analysis/plotting.py
+-rw-r--r--   0        0        0     9288 2023-03-29 08:14:20.701682 moabb-0.5.0/moabb/analysis/results.py
+-rw-r--r--   0        0        0    10931 2023-05-23 01:53:37.595674 moabb-0.5.0/moabb/benchmark.py
+-rw-r--r--   0        0        0    19272 2023-01-03 12:39:59.580480 moabb-0.5.0/moabb/datasets/Lee2019.py
+-rw-r--r--   0        0        0     7939 2023-01-03 12:39:59.580825 moabb-0.5.0/moabb/datasets/Weibo2014.py
+-rw-r--r--   0        0        0     5399 2023-01-03 12:39:59.581147 moabb-0.5.0/moabb/datasets/Zhou2016.py
+-rw-r--r--   0        0        0     1429 2023-04-27 09:08:18.918671 moabb-0.5.0/moabb/datasets/__init__.py
+-rw-r--r--   0        0        0     2755 2023-01-03 12:39:59.581549 moabb-0.5.0/moabb/datasets/alex_mi.py
+-rw-r--r--   0        0        0     7150 2023-01-03 09:13:10.077816 moabb-0.5.0/moabb/datasets/base.py
+-rw-r--r--   0        0        0    18974 2023-01-03 12:39:59.581935 moabb-0.5.0/moabb/datasets/bbci_eeg_fnirs.py
+-rw-r--r--   0        0        0    45166 2023-01-04 00:54:30.444628 moabb-0.5.0/moabb/datasets/bnci.py
+-rw-r--r--   0        0        0    39027 2023-05-23 01:53:37.596347 moabb-0.5.0/moabb/datasets/braininvaders.py
+-rw-r--r--   0        0        0     8870 2023-01-04 00:54:30.445344 moabb-0.5.0/moabb/datasets/download.py
+-rw-r--r--   0        0        0     7765 2023-03-05 07:49:33.884584 moabb-0.5.0/moabb/datasets/epfl.py
+-rw-r--r--   0        0        0     4783 2023-04-27 09:08:18.920982 moabb-0.5.0/moabb/datasets/fake.py
+-rw-r--r--   0        0        0     5639 2023-01-03 12:39:59.583526 moabb-0.5.0/moabb/datasets/gigadb.py
+-rw-r--r--   0        0        0    15036 2023-04-27 09:08:18.921676 moabb-0.5.0/moabb/datasets/huebner_llp.py
+-rw-r--r--   0        0        0     4495 2023-01-03 12:39:59.583824 moabb-0.5.0/moabb/datasets/mpi_mi.py
+-rw-r--r--   0        0        0     8083 2023-01-31 12:28:02.804185 moabb-0.5.0/moabb/datasets/neiry.py
+-rw-r--r--   0        0        0     7007 2023-01-03 12:39:59.584454 moabb-0.5.0/moabb/datasets/physionet_mi.py
+-rw-r--r--   0        0        0     4710 2023-01-03 12:39:59.584791 moabb-0.5.0/moabb/datasets/schirrmeister2017.py
+-rw-r--r--   0        0        0     8573 2023-04-27 09:08:18.921907 moabb-0.5.0/moabb/datasets/sosulski2019.py
+-rw-r--r--   0        0        0     3952 2023-03-05 07:49:33.886813 moabb-0.5.0/moabb/datasets/ssvep_exo.py
+-rw-r--r--   0        0        0    22134 2023-01-31 12:28:02.804547 moabb-0.5.0/moabb/datasets/ssvep_mamem.py
+-rw-r--r--   0        0        0     4179 2023-01-03 12:39:59.585795 moabb-0.5.0/moabb/datasets/ssvep_nakanishi.py
+-rw-r--r--   0        0        0     7748 2023-01-03 12:39:59.586141 moabb-0.5.0/moabb/datasets/ssvep_wang.py
+-rw-r--r--   0        0        0     6480 2023-01-03 12:39:59.586478 moabb-0.5.0/moabb/datasets/upper_limb.py
+-rw-r--r--   0        0        0     4305 2023-01-03 09:13:10.088168 moabb-0.5.0/moabb/datasets/utils.py
+-rw-r--r--   0        0        0      428 2023-01-03 09:13:10.088435 moabb-0.5.0/moabb/evaluations/__init__.py
+-rw-r--r--   0        0        0     7251 2023-01-31 12:28:02.804914 moabb-0.5.0/moabb/evaluations/base.py
+-rw-r--r--   0        0        0    30271 2023-03-29 08:14:20.702636 moabb-0.5.0/moabb/evaluations/evaluations.py
+-rw-r--r--   0        0        0      449 2022-02-02 13:27:15.099488 moabb-0.5.0/moabb/paradigms/__init__.py
+-rw-r--r--   0        0        0    10533 2023-05-19 13:25:19.708410 moabb-0.5.0/moabb/paradigms/base.py
+-rw-r--r--   0        0        0    13284 2023-03-20 21:52:18.340752 moabb-0.5.0/moabb/paradigms/motor_imagery.py
+-rw-r--r--   0        0        0    11687 2023-05-19 13:25:19.708765 moabb-0.5.0/moabb/paradigms/p300.py
+-rw-r--r--   0        0        0     9280 2023-01-03 09:13:10.090603 moabb-0.5.0/moabb/paradigms/ssvep.py
+-rw-r--r--   0        0        0     1180 2023-05-19 13:25:19.710062 moabb-0.5.0/moabb/pipelines/__init__.py
+-rw-r--r--   0        0        0    23799 2023-05-23 01:53:37.596942 moabb-0.5.0/moabb/pipelines/classification.py
+-rw-r--r--   0        0        0     2187 2023-01-03 09:13:10.092407 moabb-0.5.0/moabb/pipelines/csp.py
+-rw-r--r--   0        0        0    25436 2023-05-23 01:53:37.597821 moabb-0.5.0/moabb/pipelines/deep_learning.py
+-rw-r--r--   0        0        0     3724 2023-05-19 13:25:19.710824 moabb-0.5.0/moabb/pipelines/features.py
+-rw-r--r--   0        0        0    11973 2023-03-29 08:14:20.703034 moabb-0.5.0/moabb/pipelines/utils.py
+-rw-r--r--   0        0        0     6052 2023-03-05 07:49:33.892949 moabb-0.5.0/moabb/pipelines/utils_deep_model.py
+-rw-r--r--   0        0        0     6095 2023-04-27 09:08:18.922140 moabb-0.5.0/moabb/pipelines/utils_pytorch.py
+-rw-r--r--   0        0        0     3214 2023-03-20 21:52:18.341944 moabb-0.5.0/moabb/run.py
+-rw-r--r--   0        0        0     3823 2023-01-24 15:26:14.317791 moabb-0.5.0/moabb/tests/None/GridSearch_CrossSession/FakeDataset/1/C/Grid_Search_CrossSession.pkl
+-rw-r--r--   0        0        0     3823 2023-01-24 15:26:15.021255 moabb-0.5.0/moabb/tests/None/GridSearch_CrossSession/FakeDataset/2/C/Grid_Search_CrossSession.pkl
+-rw-r--r--   0        0        0     3823 2023-01-24 15:26:16.180064 moabb-0.5.0/moabb/tests/None/GridSearch_CrossSubject/FakeDataset/C/Grid_Search_CrossSubject.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:17.199118 moabb-0.5.0/moabb/tests/None/GridSearch_WithinSession/FakeDataset/subject1/session_0/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:17.800564 moabb-0.5.0/moabb/tests/None/GridSearch_WithinSession/FakeDataset/subject1/session_1/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:18.013718 moabb-0.5.0/moabb/tests/None/GridSearch_WithinSession/FakeDataset/subject2/session_0/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:18.111500 moabb-0.5.0/moabb/tests/None/GridSearch_WithinSession/FakeDataset/subject2/session_1/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0      439 2023-05-19 13:25:19.711115 moabb-0.5.0/moabb/tests/__init__.py
+-rw-r--r--   0        0        0     7320 2023-04-19 06:19:41.758459 moabb-0.5.0/moabb/tests/analysis.py
+-rw-r--r--   0        0        0     1595 2023-01-03 09:13:10.095459 moabb-0.5.0/moabb/tests/benchmark.py
+-rw-r--r--   0        0        0     1628 2023-05-19 13:25:19.711291 moabb-0.5.0/moabb/tests/classification.py
+-rw-r--r--   0        0        0     2704 2023-04-27 09:08:18.922341 moabb-0.5.0/moabb/tests/datasets.py
+-rw-r--r--   0        0        0     4603 2023-01-03 09:13:10.096132 moabb-0.5.0/moabb/tests/download.py
+-rw-r--r--   0        0        0     9970 2023-03-29 08:14:20.704307 moabb-0.5.0/moabb/tests/evaluations.py
+-rw-r--r--   0        0        0    23023 2023-05-19 13:25:19.711653 moabb-0.5.0/moabb/tests/paradigms.py
+-rw-r--r--   0        0        0     3823 2023-01-24 16:40:17.724302 moabb-0.5.0/moabb/tests/res_test/GridSearch_CrossSession/FakeDataset/1/C/Grid_Search_CrossSession.pkl
+-rw-r--r--   0        0        0     3823 2023-01-24 16:40:18.705183 moabb-0.5.0/moabb/tests/res_test/GridSearch_CrossSession/FakeDataset/2/C/Grid_Search_CrossSession.pkl
+-rw-r--r--   0        0        0     3823 2023-01-24 16:40:20.327325 moabb-0.5.0/moabb/tests/res_test/GridSearch_CrossSubject/FakeDataset/C/Grid_Search_CrossSubject.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:18.703819 moabb-0.5.0/moabb/tests/res_test/GridSearch_WithinSession/FakeDataset/subject1/session_0/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:19.309606 moabb-0.5.0/moabb/tests/res_test/GridSearch_WithinSession/FakeDataset/subject1/session_1/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:19.501713 moabb-0.5.0/moabb/tests/res_test/GridSearch_WithinSession/FakeDataset/subject2/session_0/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0     4447 2023-01-24 15:26:19.607097 moabb-0.5.0/moabb/tests/res_test/GridSearch_WithinSession/FakeDataset/subject2/session_1/C/Grid_Search_WithinSession.pkl
+-rw-r--r--   0        0        0      357 2023-01-31 12:28:02.806198 moabb-0.5.0/moabb/tests/test_pipelines/CSP.yml
+-rw-r--r--   0        0        0      260 2021-06-21 22:56:45.336965 moabb-0.5.0/moabb/tests/test_pipelines/LogVar.yml
+-rw-r--r--   0        0        0      216 2022-02-02 13:27:15.108179 moabb-0.5.0/moabb/tests/test_pipelines/SSVEP_CCA.yml
+-rw-r--r--   0        0        0     5131 2023-04-19 06:19:41.758897 moabb-0.5.0/moabb/tests/util_braindecode.py
+-rw-r--r--   0        0        0     3847 2023-03-23 11:26:36.931808 moabb-0.5.0/moabb/tests/util_tests.py
+-rw-r--r--   0        0        0     4097 2023-04-19 06:19:41.759994 moabb-0.5.0/moabb/utils.py
+-rw-r--r--   0        0        0     1768 2023-05-23 01:53:37.600172 moabb-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    15097 1970-01-01 00:00:00.000000 moabb-0.5.0/setup.py
+-rw-r--r--   0        0        0    13824 1970-01-01 00:00:00.000000 moabb-0.5.0/PKG-INFO
```

### Comparing `moabb-0.4.6/LICENSE` & `moabb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moabb-0.4.6/README.md` & `moabb-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 This document is a hub to give you some information about the project. Jump straight to
 one of the sections below, or just scroll down to find out more.
 
 - [What are we doing? (And why?)](#what-are-we-doing)
 - [Installation](#installation)
 - [Running](#running)
 - [Supported datasets](#supported-datasets)
-- [Who are we? n](#who-are-we)
+- [Who are we?](#who-are-we)
 - [Get in touch](#contact-us)
 - [Documentation][link_moabb_docs]
 - [Architecture and main concepts](#architecture-and-main-concepts)
 - [Citing MOABB and related publications](#citing-moabb-and-related-publications)
 
 ## What are we doing?
 
@@ -61,16 +61,16 @@
 
 ### The solution
 
 The Mother of all BCI Benchmarks allows to:
 
 - Build a comprehensive benchmark of popular BCI algorithms applied on an extensive list
   of freely available EEG datasets.
-- The code will be made available on github, serving as a reference point for the future
-  algorithmic developments.
+- The code is available on GitHub, serving as a reference point for the future algorithmic
+  developments.
 - Algorithms can be ranked and promoted on a website, providing a clear picture of the
   different solutions available in the field.
 
 This project will be successful when we read in an abstract “ … the proposed method
 obtained a score of 89% on the MOABB (Mother of All BCI Benchmarks), outperforming the
 state of the art by 5% ...”.
 
@@ -83,15 +83,15 @@
 See [Troubleshooting](#Troubleshooting) section if you have a problem.
 
 ### Manual installation
 
 You could fork or clone the repository and go to the downloaded directory, then run:
 
 1. install `poetry` (only once per machine):\
-   `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -`\
+   `curl -sSL https://install.python-poetry.org | python3 -`\
    or [checkout installation instruction](https://python-poetry.org/docs/#installation) or
    use [conda forge version](https://anaconda.org/conda-forge/poetry)
 1. (Optional, skip if not sure) Disable automatic environment creation:\
    `poetry config virtualenvs.create false`
 1. install all dependencies in one command (have to be run in the project directory):\
    `poetry install`
 
@@ -116,25 +116,81 @@
 ### Use MOABB
 
 First, you could take a look at our [tutorials](./tutorials) that cover the most important
 concepts and use cases. Also, we have a several [examples](./examples/) available.
 
 You might be interested in [MOABB documentation][link_moabb_docs]
 
+### Moabb and docker
+
+Moabb has a default image to run the benchmark. You have two options to download this
+image: build from scratch or pull from the docker hub. **We recommend pulling from the
+docker hub**.
+
+If this were your first time using docker, you would need to **install the docker** and
+**login** on docker hub. We recommend the
+[official](https://docs.docker.com/desktop/install/linux-install/) docker documentation
+for this step, it is essential to follow the instructions.
+
+After installing docker, you can pull the image from the docker hub:
+
+```bash
+docker pull baristimunha/moabb
+# rename the tag to moabb
+docker tag baristimunha/moabb moabb
+```
+
+If you want to build the image from scratch, you can use the following command at the
+root. You may have to login with the API key in the
+[NGC Catalog](https://catalog.ngc.nvidia.com/) to run this command.
+
+```bash
+bash docker/create_docker.sh
+```
+
+With the image downloaded or rebuilt from scratch, you will have an image called `moabb`.
+To run the default benchmark, still at the root of the project, and you can use the
+following command:
+
+```bash
+mkdir dataset
+mkdir results
+mkdir output
+bash docker/run_docker.sh PATH_TO_ROOT_FOLDER
+```
+
+An example of the command is:
+
+```bash
+cd /home/user/project/moabb
+mkdir dataset
+mkdir results
+mkdir output
+bash docker/run_docker.sh /home/user/project/moabb
+```
+
+Note: It is important to use an absolute path for the root folder to run, but you can
+modify the run_docker.sh script to save in another path beyond the root of the project. By
+default, the script will save the results in the project's root in the folder `results`,
+the datasets in the folder `dataset` and the output in the folder `output`.
+
 ### Troubleshooting
 
 Currently pip install moabb fails when pip version < 21, e.g. with 20.0.2 due to an `idna`
 package conflict. Newer pip versions resolve this conflict automatically. To fix this you
 can upgrade your pip version using: `pip install -U pip` before installing `moabb`.
 
 ## Supported datasets
 
 The list of supported datasets can be found here :
 https://neurotechx.github.io/moabb/datasets.html
 
+Detailed information regarding datasets (electrodes, trials, sessions) are indicated on
+the wiki: https://github.com/NeuroTechX/moabb/wiki/Datasets-Support
+
 ### Submit a new dataset
 
 you can submit a new dataset by mentioning it to this
 [issue](https://github.com/NeuroTechX/moabb/issues/1). The datasets currently on our radar
 can be seen [here] (https://github.com/NeuroTechX/moabb/wiki/Datasets-Support)
 
 ## Who are we?
@@ -169,21 +225,21 @@
 Please note that it's very important to us that we maintain a positive and supportive
 environment for everyone who wants to participate. When you join us we ask that you follow
 our [code of conduct](CODE_OF_CONDUCT.md) in all interactions both on and offline.
 
 ## Contact us
 
 If you want to report a problem or suggest an enhancement, we'd love for you to
-[open an issue](../../issues) at this github repository because then we can get right on
+[open an issue](../../issues) at this GitHub repository because then we can get right on
 it.
 
 For a less formal discussion or exchanging ideas, you can also reach us on the [Gitter
 channel][link_gitter] or join our weekly office hours! This an open video meeting
 happening on a [regular basis](https://github.com/NeuroTechX/moabb/issues/191), please ask
-the link on the gitter channel. We are also on [NeuroTechX slack #moabb
+the link on the gitter channel. We are also on [NeuroTechX Slack #moabb
 channel][link_neurotechx_signup].
 
 ## Architecture and Main Concepts
 
 <p align="center">
   <img alt="banner" src="/images/architecture.png/" width="400">
 </p>
@@ -251,11 +307,11 @@
 BCI algorithms applied on an extensive list of freely available EEG datasets.
 
 [link_alex_b]: http://alexandre.barachant.org/
 [link_vinay]: https://ei.is.tuebingen.mpg.de/~vjayaram
 [link_neurotechx]: http://neurotechx.com/
 [link_sylvain]: https://sylvchev.github.io/
 [link_neurotechx_signup]: https://neurotechx.com/
-[link_gitter]: https://gitter.im/moabb_dev/community
+[link_gitter]: https://app.gitter.im/#/room/#moabb_dev_community:gitter.im
 [link_moabb_docs]: https://neurotechx.github.io/moabb/
 [link_arxiv]: https://arxiv.org/abs/1805.06427
 [link_jne]: http://iopscience.iop.org/article/10.1088/1741-2552/aadea0/meta
```

### Comparing `moabb-0.4.6/moabb/analysis/__init__.py` & `moabb-0.5.0/moabb/analysis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from datetime import datetime
 
 from moabb.analysis import plotting as plt
 from moabb.analysis.meta_analysis import (  # noqa: E501
     compute_dataset_statistics,
     find_significant_differences,
 )
+from moabb.analysis.plotting import codecarbon_plot  # noqa: F401
 from moabb.analysis.results import Results  # noqa: F401
 
 
 log = logging.getLogger(__name__)
 
 
 def analyze(results, out_path, name="analysis", plot=False):
     """Analyze results.
 
     Given a results dataframe, generates a folder with
     results and a dataframe of the exact data used to generate those results,
-    aswell as introspection to return information on the computer
+    as well as introspection to return information on the computer
 
     parameters
     ----------
     out_path: location to store analysis folder
 
     results: Dataframe generated from Results object
 
@@ -40,16 +41,14 @@
     elif not os.path.isdir(out_path):
         raise IOError("Given directory does not exist")
     else:
         analysis_path = os.path.join(out_path, name)
 
     unique_ids = [plt._simplify_names(x) for x in results.pipeline.unique()]
     simplify = True
-    print(unique_ids)
-    print(set(unique_ids))
     if len(unique_ids) != len(set(unique_ids)):
         log.warning("Pipeline names are too similar, turning off name shortening")
         simplify = False
 
     os.makedirs(analysis_path, exist_ok=True)
     # TODO: no good cross-platform way of recording CPU info?
     with open(os.path.join(analysis_path, "info.txt"), "a") as f:
```

### Comparing `moabb-0.4.6/moabb/analysis/meta_analysis.py` & `moabb-0.5.0/moabb/analysis/meta_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 
     Returns
     -------
     df: DataFrame
         Aggregated results, samples are index, columns are pipelines,
         and values are scores
     """
-    return df.groupby(["pipeline", "dataset", "subject"]).mean().reset_index()
+    return (
+        df.groupby(["pipeline", "dataset", "subject"])
+        .mean(numeric_only=True)
+        .reset_index()
+    )
 
 
 def compute_pvals_wilcoxon(df, order=None):
     """Compute Wilcoxon rank-sum test on agregated results
 
     Returns kxk matrix of p-values computed via the Wilcoxon rank-sum test,
     order defines the order of rows and columns
```

### Comparing `moabb-0.4.6/moabb/analysis/plotting.py` & `moabb-0.5.0/moabb/analysis/plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,15 +41,20 @@
     -------
     fig: Figure
         Pyplot handle
     color_dict: dict
         Dictionary with the facecolor
     """
     data = collapse_session_scores(data)
-    data["dataset"] = data["dataset"].apply(_simplify_names)
+    unique_ids = data["dataset"].apply(_simplify_names)
+    if len(unique_ids) != len(set(unique_ids)):
+        log.warning("Dataset names are too similar, turning off name shortening")
+    else:
+        data["dataset"] = unique_ids
+
     if pipelines is not None:
         data = data[data.pipeline.isin(pipelines)]
     fig = plt.figure(figsize=(8.5, 11))
     ax = fig.add_subplot(111)
     # markers = ['o', '8', 's', 'p', '+', 'x', 'D', 'd', '>', '<', '^']
     sea.stripplot(
         data=data,
@@ -67,14 +72,65 @@
     ax.set_title("Scores per dataset and algorithm")
     handles, labels = ax.get_legend_handles_labels()
     color_dict = {lb: h.get_facecolor()[0] for lb, h in zip(labels, handles)}
     plt.tight_layout()
     return fig, color_dict
 
 
+def codecarbon_plot(data, order_list=None, pipelines=None, country=""):
+    """Plot code carbon consume for the results from the benchmark
+
+    Parameters
+    ----------
+    data: output of Results.to_dataframe()
+        results on datasets
+    order_list: list of str | None
+        order of pipelines to include in this plot
+    pipelines: list of str | None
+        pipelines to include in this plot
+    country: str
+        country to include in the title
+    pipelines: list of str | None
+        pipelines to include in this plot
+
+    Returns
+    -------
+    fig: Figure
+        Pyplot handle
+    """
+    data = collapse_session_scores(data)
+    unique_ids = data["dataset"].apply(_simplify_names)
+    if len(unique_ids) != len(set(unique_ids)):
+        log.warning("Dataset names are too similar, turning off name shortening")
+    else:
+        data["dataset"] = unique_ids
+
+    if pipelines is not None:
+        data = data[data.pipeline.isin(pipelines)]
+
+    data = data.rename(columns={"carbon emission": "carbon_emission"})
+
+    fig = sea.catplot(
+        kind="bar",
+        data=data,
+        x="dataset",
+        y="carbon_emission",
+        hue="pipeline",
+        palette=PIPELINE_PALETTE,
+        height=8.5,
+        hue_order=order_list,
+    ).set(title=r"$CO_2$ emission per dataset and algorithm" + country)
+    fig.set(yscale="log")
+    fig.tight_layout()
+    fig.set_ylabels(r"$CO_2$ emission (Log Scale)")
+    fig.set_xlabels("Dataset")
+
+    return fig
+
+
 def paired_plot(data, alg1, alg2):
     """Generate a figure with a paired plot
 
     Parameters
     ----------
     data: DataFrame
         dataframe obtained from evaluation
@@ -198,22 +254,30 @@
     assert alg1 in stats_df.pipe1.unique()
     assert alg2 in stats_df.pipe1.unique()
     df_fw = stats_df.loc[(stats_df.pipe1 == alg1) & (stats_df.pipe2 == alg2)]
     df_fw = df_fw.sort_values(by="pipe1")
     df_bk = stats_df.loc[(stats_df.pipe1 == alg2) & (stats_df.pipe2 == alg1)]
     df_bk = df_bk.sort_values(by="pipe1")
     dsets = df_fw.dataset.unique()
+    simplify = True
+    unique_ids = [_simplify_names(x) for x in dsets]
+    if len(unique_ids) != len(set(unique_ids)):
+        log.warning("Dataset names are too similar, turning off name shortening")
+        simplify = False
     ci = []
     fig = plt.figure()
     gs = gridspec.GridSpec(1, 5)
     sig_ind = []
     pvals = []
     ax = fig.add_subplot(gs[0, :-1])
     ax.set_yticks(np.arange(len(dsets) + 1))
-    ax.set_yticklabels(["Meta-effect"] + [_simplify_names(d) for d in dsets])
+    if simplify:
+        ax.set_yticklabels(["Meta-effect"] + [d for d in unique_ids])
+    else:
+        ax.set_yticklabels(["Meta-effect"] + [d for d in dsets])
     pval_ax = fig.add_subplot(gs[0, -1], sharey=ax)
     plt.setp(pval_ax.get_yticklabels(), visible=False)
     _min = 0
     _max = 0
     for ind, d in enumerate(dsets):
         nsub = float(df_fw.loc[df_fw.dataset == d, "nsub"])
         t_dof = nsub - 1
```

### Comparing `moabb-0.4.6/moabb/analysis/results.py` & `moabb-0.5.0/moabb/analysis/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,36 @@
 import numpy as np
 import pandas as pd
 from mne import get_config, set_config
 from mne.datasets.utils import _get_path
 from sklearn.base import BaseEstimator
 
 
+try:
+    from codecarbon import EmissionsTracker  # noqa
+
+    _carbonfootprint = True
+except ImportError:
+    _carbonfootprint = False
+
+
 def get_string_rep(obj):
     if issubclass(type(obj), BaseEstimator):
         str_repr = repr(obj.get_params())
     else:
         str_repr = repr(obj)
     if "<lambda> at " in str_repr:
         warnings.warn(
             "You are probably using a classifier with a lambda function"
             " as an attribute. Lambda functions can only be identified"
             " by memory address which MOABB does not consider. To avoid"
             " issues you can use named functions defined using the def"
             " keyword instead.",
             RuntimeWarning,
+            stacklevel=2,
         )
     str_no_addresses = re.sub("0x[a-z0-9]*", "0x__", str_repr)
     return str_no_addresses.replace("\n", "").encode("utf8")
 
 
 def get_digest(obj):
     """Return hash of an object repr.
@@ -98,28 +107,35 @@
 
         if not osp.isfile(self.filepath):
             with h5py.File(self.filepath, "w") as f:
                 f.attrs["create_time"] = np.string_(
                     "{:%Y-%m-%d, %H:%M}".format(datetime.now())
                 )
 
-    def add(self, results, pipelines):
+    def add(self, results, pipelines):  # noqa: C901
         """add results"""
 
         def to_list(res):
             if type(res) is dict:
                 return [res]
             elif type(res) is not list:
                 raise ValueError(
                     "Results are given as neither dict nor"
                     "list but {}".format(type(res).__name__)
                 )
             else:
                 return res
 
+        col_names = ["score", "time", "samples"]
+        if _carbonfootprint:
+            n_cols = 4
+            col_names.append("carbon_emission")
+        else:
+            n_cols = 3
+
         with h5py.File(self.filepath, "r+") as f:
             for name, data_dict in results.items():
                 digest = get_digest(pipelines[name])
                 if digest not in f.keys():
                     # create pipeline main group if nonexistant
                     f.create_group(digest)
 
@@ -135,20 +151,22 @@
                     # create dataset subgroup if nonexistant
                     dset = ppline_grp.create_group(dname)
                     dset.attrs["n_subj"] = len(d1["dataset"].subject_list)
                     dset.attrs["n_sessions"] = d1["dataset"].n_sessions
                     dt = h5py.special_dtype(vlen=str)
                     dset.create_dataset("id", (0, 2), dtype=dt, maxshape=(None, 2))
                     dset.create_dataset(
-                        "data", (0, 3 + n_add_cols), maxshape=(None, 3 + n_add_cols)
+                        "data",
+                        (0, n_cols + n_add_cols),
+                        maxshape=(None, n_cols + n_add_cols),
                     )
                     dset.attrs["channels"] = d1["n_channels"]
                     dset.attrs.create(
                         "columns",
-                        ["score", "time", "samples", *self.additional_columns],
+                        col_names + self.additional_columns,
                         dtype=dt,
                     )
                 dset = ppline_grp[dname]
                 for d in dlist:
                     # add id and scores to group
                     length = len(dset["id"]) + 1
                     dset["id"].resize(length, 0)
@@ -158,29 +176,37 @@
                         add_cols = [d[ac] for ac in self.additional_columns]
                     except KeyError:
                         raise ValueError(
                             f"Additional columns: {self.additional_columns} "
                             f"were specified in the evaluation, but results"
                             f" contain only these keys: {d.keys()}."
                         ) from None
+                    cols = [d["score"], d["time"], d["n_samples"]]
+                    if _carbonfootprint:
+                        if isinstance(d["carbon_emission"], tuple):
+                            cols.append(*d["carbon_emission"])
+                        else:
+                            cols.append(d["carbon_emission"])
                     dset["data"][-1, :] = np.asarray(
-                        [d["score"], d["time"], d["n_samples"], *add_cols]
+                        [
+                            *cols,
+                            *add_cols,
+                        ]
                     )
 
     def to_dataframe(self, pipelines=None):
         df_list = []
 
         # get the list of pipeline hash
         digests = []
         if pipelines is not None:
             digests = [get_digest(pipelines[name]) for name in pipelines]
 
         with h5py.File(self.filepath, "r") as f:
             for digest, p_group in f.items():
-
                 # skip if not in pipeline list
                 if (pipelines is not None) & (digest not in digests):
                     continue
 
                 name = p_group.attrs["name"]
                 for dname, dset in p_group.items():
                     array = np.array(dset["data"])
```

### Comparing `moabb-0.4.6/moabb/datasets/Lee2019.py` & `moabb-0.5.0/moabb/datasets/Lee2019.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,24 +146,14 @@
         stim_chan = np.zeros(len(raw))
         for i_sample, id_class in zip(event_times_in_samples, event_id):
             stim_chan[i_sample] += id_class
         stim_raw = self._make_raw_array(
             stim_chan[:, None], ["STI 014"], "stim", sfreq, verbose="WARNING"
         )
 
-        # Add events
-        event_arr = [
-            event_times_in_samples,
-            [0] * len(event_times_in_samples),
-            event_id,
-        ]
-        raw.info["events"] = [
-            dict(list=np.array(event_arr).T, channels=None),
-        ]
-
         # Add EMG and stim channels
         raw = raw.add_channels([emg_raw, stim_raw])
         return raw
 
     def _get_single_rest_run(self, data, prefix):
         sfreq = data["fs"].item()
         raw = self._make_raw_array(
@@ -235,14 +225,23 @@
 
         return subject_paths
 
 
 class Lee2019_MI(Lee2019):
     """BMI/OpenBMI dataset for MI.
 
+    .. admonition:: Dataset summary
+
+
+        ==========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name          #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ==========  =======  =======  ==========  =================  ============  ===============  ===========
+        Lee2019_MI       55       62           2                100  4s            1000Hz                     2
+        ==========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from Lee et al 2019 [1]_.
 
     **Dataset Description**
 
     EEG signals were recorded with a sampling rate of 1,000 Hz and
     collected with 62 Ag/AgCl electrodes. The EEG amplifier used
     in the experiment was a BrainAmp (Brain Products; Munich,
@@ -296,14 +295,23 @@
 
     __init__ = partialmethod(Lee2019.__init__, "MI")
 
 
 class Lee2019_ERP(Lee2019):
     """BMI/OpenBMI dataset for P300.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Name           #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Lee2019_ERP       54       62  6900 NT / 1380 T   1s               1000Hz                     2
+        ===========  =======  =======  =================  ===============  ===============  ===========
+
     Dataset from Lee et al 2019 [1]_.
 
     **Dataset Description**
 
     EEG signals were recorded with a sampling rate of 1,000 Hz and
     collected with 62 Ag/AgCl electrodes. The EEG amplifier used
     in the experiment was a BrainAmp (Brain Products; Munich,
@@ -331,15 +339,15 @@
     one sequence consisted of 12 stimulus flashes. A maximum
     of five sequences (i.e., 60 flashes) was allotted without prolonged
     inter-sequence intervals for each target character. After the end
     of five sequences, 4.5 s were given to the user for identifying, locating,
     and gazing at the next target character. The participant
     was instructed to attend to the target symbol by counting the
     number of times each target character had been flashed.
-        In the training session, subjects were asked to copy-spell
+    In the training session, subjects were asked to copy-spell
     a given sentence, "NEURAL NETWORKS AND DEEP LEARNING"
     (33 characters including spaces) by gazing at the target character
     on the screen. The training session was performed in the offline
     condition, and no feedback was provided to the subject during
     the EEG recording. In the test session, subjects were instructed to
     copy-spell "PATTERN RECOGNITION MACHINE LEARNING"
     (36 characters including spaces), and the real-time EEG data were
@@ -377,14 +385,23 @@
 
     __init__ = partialmethod(Lee2019.__init__, "ERP")
 
 
 class Lee2019_SSVEP(Lee2019):
     """BMI/OpenBMI dataset for SSVEP.
 
+    .. admonition:: Dataset summary
+
+
+        =============  =======  =======  ==========  =================  ===============  ===============  ===========
+        Name             #Subj    #Chan    #Classes    #Trials / class  Trials length    Sampling rate      #Sessions
+        =============  =======  =======  ==========  =================  ===============  ===============  ===========
+        Lee2019_SSVEP       24       16           4                 25  1s               1000Hz                     1
+        =============  =======  =======  ==========  =================  ===============  ===============  ===========
+
     Dataset from Lee et al 2019 [1]_.
 
     **Dataset Description**
 
     EEG signals were recorded with a sampling rate of 1,000 Hz and
     collected with 62 Ag/AgCl electrodes. The EEG amplifier used
     in the experiment was a BrainAmp (Brain Products; Munich,
```

### Comparing `moabb-0.4.6/moabb/datasets/Weibo2014.py` & `moabb-0.5.0/moabb/datasets/Weibo2014.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import logging
 import os
 import shutil
 
 import mne
 import numpy as np
-from mne.datasets.utils import _get_path
 from pooch import Unzip, retrieve
 from scipy.io import loadmat
 
 from .base import BaseDataset
+from .download import get_dataset_path
 
 
 log = logging.getLogger(__name__)
 
 FILES = []
 FILES.append("https://dataverse.harvard.edu/api/access/datafile/2499178")
 FILES.append("https://dataverse.harvard.edu/api/access/datafile/2499182")
@@ -60,14 +60,23 @@
             get_subjects(list(range(8, 11)), file3_subj, 2)
     return os.path.join(base_path, "subject_{}.mat".format(subject))
 
 
 class Weibo2014(BaseDataset):
     """Motor Imagery dataset from Weibo et al 2014.
 
+    .. admonition:: Dataset summary
+
+
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name         #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Weibo2014       10       60           7                 80  4s            200Hz                      1
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from the article *Evaluation of EEG oscillatory patterns and
     cognitive process during simple and compound limb motor imagery* [1]_.
 
     It contains data recorded on 10 subjects, with 60 electrodes.
 
     This dataset was used to investigate the differences of the EEG patterns
     between simple limb motor imagery and compound limb motor
@@ -168,13 +177,12 @@
         return {"session_0": {"run_0": raw}}
 
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
         if subject not in self.subject_list:
             raise (ValueError("Invalid subject number"))
-        key = "MNE_DATASETS_WEIBO2014_PATH"
-        path = _get_path(path, key, "Weibo 2014")
+        path = get_dataset_path("WEIBO", path)
         basepath = os.path.join(path, "MNE-weibo-2014")
         if not os.path.isdir(basepath):
             os.makedirs(basepath)
         return eeg_data_path(basepath, subject)
```

### Comparing `moabb-0.4.6/moabb/datasets/Zhou2016.py` & `moabb-0.5.0/moabb/datasets/Zhou2016.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import os
 import shutil
 import zipfile as z
 
 import numpy as np
 from mne.channels import make_standard_montage
-from mne.datasets.utils import _get_path
 from mne.io import read_raw_cnt
 from pooch import retrieve
 
 from .base import BaseDataset
+from .download import get_dataset_path
 
 
 DATA_PATH = "https://ndownloader.figshare.com/files/3662952"
 
 
 def local_data_path(base_path, subject):
     if not os.path.isdir(os.path.join(base_path, "subject_{}".format(subject))):
@@ -46,14 +46,23 @@
         for y in ["1", "2", "3"]
     ]
 
 
 class Zhou2016(BaseDataset):
     """Motor Imagery dataset from Zhou et al 2016.
 
+    .. admonition:: Dataset summary
+
+
+        ========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name        #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ========  =======  =======  ==========  =================  ============  ===============  ===========
+        Zhou2016        4       14           3                160  5s            250Hz                      3
+        ========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from the article *A Fully Automated Trial Selection Method for
     Optimization of Motor Imagery Based Brain-Computer Interface* [1]_.
     This dataset contains data recorded on 4 subjects performing 3 type of
     motor imagery: left hand, right hand and feet.
 
     Every subject went through three sessions, each of which contained two
     consecutive runs with several minutes inter-run breaks, and each run
@@ -110,13 +119,12 @@
         return out
 
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
         if subject not in self.subject_list:
             raise (ValueError("Invalid subject number"))
-        key = "MNE_DATASETS_ZHOU2016_PATH"
-        path = _get_path(path, key, "Zhou 2016")
+        path = get_dataset_path("ZHOU", path)
         basepath = os.path.join(path, "MNE-zhou-2016")
         if not os.path.isdir(basepath):
             os.makedirs(basepath)
         return local_data_path(basepath, subject)
```

### Comparing `moabb-0.4.6/moabb/datasets/__init__.py` & `moabb-0.5.0/moabb/datasets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 """
 A dataset handle and abstract low level access to the data. the dataset will
 takes data stored locally, in the format in which they have been downloaded,
 and will convert them into a MNE raw object. There are options to pool all the
 different recording sessions per subject or to evaluate them separately.
+
+See https://github.com/NeuroTechX/moabb/wiki/Datasets-Support for detail
+on datasets (electrodes, number of trials, sessions, etc.)
 """
 # flake8: noqa
 from .alex_mi import AlexMI
 from .bbci_eeg_fnirs import Shin2017A, Shin2017B
 from .bnci import (
     BNCI2014001,
     BNCI2014002,
     BNCI2014004,
     BNCI2014008,
     BNCI2014009,
     BNCI2015001,
     BNCI2015003,
     BNCI2015004,
 )
-from .braininvaders import bi2012, bi2013a, bi2014a, bi2014b, bi2015a, bi2015b
+from .braininvaders import (
+    VirtualReality,
+    bi2012,
+    bi2013a,
+    bi2014a,
+    bi2014b,
+    bi2015a,
+    bi2015b,
+)
 from .epfl import EPFLP300
 from .gigadb import Cho2017
 from .huebner_llp import Huebner2017, Huebner2018
 from .Lee2019 import Lee2019_ERP, Lee2019_MI, Lee2019_SSVEP
 from .mpi_mi import MunichMI
 from .neiry import DemonsP300
 from .physionet_mi import PhysionetMI
```

### Comparing `moabb-0.4.6/moabb/datasets/alex_mi.py` & `moabb-0.5.0/moabb/datasets/alex_mi.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 
 ALEX_URL = "https://zenodo.org/record/806023/files/"
 
 
 class AlexMI(BaseDataset):
     """Alex Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ======  =======  =======  ==========  =================  ============  ===============  ===========
+        Name      #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ======  =======  =======  ==========  =================  ============  ===============  ===========
+        AlexMI        8       16           3                 20  3s            512Hz                      1
+        ======  =======  =======  ==========  =================  ============  ===============  ===========
+
     Motor imagery dataset from the PhD dissertation of A. Barachant [1]_.
 
     This Dataset contains EEG recordings from 8 subjects, performing 2 task of
     motor imagination (right hand, feet or rest). Data have been recorded at
     512Hz with 16 wet electrodes (Fpz, F7, F3, Fz, F4, F8, T7, C3, Cz, C4, T8,
     P7, P3, Pz, P4, P8) with a g.tec g.USBamp EEG amplifier.
```

### Comparing `moabb-0.4.6/moabb/datasets/base.py` & `moabb-0.5.0/moabb/datasets/base.py`

 * *Files identical despite different names*

### Comparing `moabb-0.4.6/moabb/datasets/bbci_eeg_fnirs.py` & `moabb-0.5.0/moabb/datasets/bbci_eeg_fnirs.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,18 +181,29 @@
         else:
             return eeg_data_path(op.join(path, "MNE-eegfnirs-data"), subject, self.accept)
 
 
 class Shin2017A(Shin2017):
     """Motor Imagey Dataset from Shin et al 2017
 
+    .. admonition:: Dataset summary
+
+
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name         #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Shin2017A       29       30           2                 30  10s           200Hz                      3
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from [1]_.
 
-    You should accept the licence term [2]_ to download this dataset, using::
-        Shin2017A(accept=True)
+
+    .. caution::
+       You should accept the licence term [2]_ to download this dataset, using:
+       ``Shin2017A(accept=True)``
 
     **Data Acquisition**
 
     EEG and NIRS data was collected in an ordinary bright room. EEG data was
     recorded by a multichannel BrainAmp EEG amplifier with thirty active
     electrodes (Brain Products GmbH, Gilching, Germany) with linked mastoids
     reference at 1000 Hz sampling rate. The EEG amplifier was also used to
@@ -275,32 +286,43 @@
     References
     ----------
 
     .. [1] Shin, J., von Lühmann, A., Blankertz, B., Kim, D.W., Jeong, J.,
            Hwang, H.J. and Müller, K.R., 2017. Open access dataset for EEG+NIRS
            single-trial classification. IEEE Transactions on Neural Systems
            and Rehabilitation Engineering, 25(10), pp.1735-1745.
+
     .. [2] GNU General Public License, Version 3
            `<https://www.gnu.org/licenses/gpl-3.0.txt>`_
     """
 
     def __init__(self, accept=False):
         super().__init__(
             fnirs=False, motor_imagery=True, mental_arithmetic=False, accept=accept
         )
         self.code = "Shin2017A"
 
 
 class Shin2017B(Shin2017):
     """Mental Arithmetic Dataset from Shin et al 2017
 
+    .. admonition:: Dataset summary
+
+
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name         #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Shin2017B       29       30           2                 30  10s           200Hz                      3
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from [1]_.
 
-    You should accept the licence term [2]_ to download this dataset, using::
-        Shin2017A(accept=True)
+    .. caution::
+        You should accept the licence term [2]_ to download this dataset, using:
+        ``Shin2017B(accept=True)``
 
     **Data Acquisition**
 
     EEG and NIRS data was collected in an ordinary bright room. EEG data was
     recorded by a multichannel BrainAmp EEG amplifier with thirty active
     electrodes (Brain Products GmbH, Gilching, Germany) with linked mastoids
     reference at 1000 Hz sampling rate. The EEG amplifier was also used to
@@ -377,14 +399,15 @@
 
     References
     ----------
     .. [1] Shin, J., von Lühmann, A., Blankertz, B., Kim, D.W., Jeong, J.,
            Hwang, H.J. and Müller, K.R., 2017. Open access dataset for EEG+NIRS
            single-trial classification. IEEE Transactions on Neural Systems
            and Rehabilitation Engineering, 25(10), pp.1735-1745.
+
     .. [2] GNU General Public License, Version 3
            `<https://www.gnu.org/licenses/gpl-3.0.txt>`_
     """
 
     def __init__(self, accept=False):
         super().__init__(
             fnirs=False, motor_imagery=False, mental_arithmetic=True, accept=accept
```

### Comparing `moabb-0.4.6/moabb/datasets/bnci.py` & `moabb-0.5.0/moabb/datasets/bnci.py`

 * *Files 16% similar despite different names*

```diff
@@ -235,14 +235,17 @@
     filename = data_path(url, path, force_update, update_path)[0]
 
     data = loadmat(filename, struct_as_record=False, squeeze_me=True)["data"]
     sess = []
     event_id = {}
     for run in data:
         raw, ev = _convert_run_p300_sl(run, verbose=verbose)
+        # Raw EEG data are scaled by a factor 10.
+        # See https://github.com/NeuroTechX/moabb/issues/275
+        raw._data[:16, :] /= 10.0
         sess.append(raw)
         event_id.update(ev)
 
     sessions = {}
     for i, sessi in enumerate(sess):
         sessions["session_" + str(i)] = {"run_0": sessi}
 
@@ -673,14 +676,23 @@
             force_update=force_update,
         )
 
 
 class BNCI2014001(MNEBNCI):
     """BNCI 2014-001 Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name           #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        BNCI2014001       10       22           4                144  4s            250Hz                      2
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset IIa from BCI Competition 4 [1]_.
 
     **Dataset Description**
 
     This data set consists of EEG data from 9 subjects.  The cue-based BCI
     paradigm consisted of four different motor imagery tasks, namely the imag-
     ination of movement of the left hand (class 1), right hand (class 2), both
@@ -728,14 +740,23 @@
             doi="10.3389/fnins.2012.00055",
         )
 
 
 class BNCI2014002(MNEBNCI):
     """BNCI 2014-002 Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name           #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        BNCI2014002       15       15           2                 80  5s            512Hz                      1
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Motor Imagery Dataset from [1]_.
 
     **Dataset description**
 
     The session consisted of eight runs, five of them for training and three
     with feedback for validation.  One run was composed of 20 trials.  Taken
     together, we recorded 50 trials per class for training and 30 trials per
@@ -782,14 +803,23 @@
             doi="10.1515/bmt-2014-0117",
         )
 
 
 class BNCI2014004(MNEBNCI):
     """BNCI 2014-004 Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name           #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        BNCI2014004       10        3           2                360  4.5s          250Hz                      5
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset B from BCI Competition 2008.
 
     **Dataset description**
 
     This data set consists of EEG data from 9 subjects of a study published in
     [1]_. The subjects were right-handed, had normal or corrected-to-normal
     vision and were paid for participating in the experiments.
@@ -856,14 +886,23 @@
             doi="10.1109/TNSRE.2007.906956",
         )
 
 
 class BNCI2014008(MNEBNCI):
     """BNCI 2014-008 P300 dataset
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Name           #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        BNCI2014008        8        8  3500 NT / 700 T    1s               256Hz                      1
+        ===========  =======  =======  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     **Dataset description**
 
     This dataset represents a complete record of P300 evoked potentials
     using a paradigm originally described by Farwell and Donchin [2]_.
     In these sessions, 8 users with amyotrophic lateral sclerosis (ALS)
@@ -918,14 +957,23 @@
             doi="10.3389/fnhum.2013.00732",
         )
 
 
 class BNCI2014009(MNEBNCI):
     """BNCI 2014-009 P300 dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Name           #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        BNCI2014009       10       16  1440 NT / 288 T    0.8s             256Hz                      3
+        ===========  =======  =======  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     **Dataset description**
 
     This dataset presents a complete record of P300 evoked potentials
     using two different paradigms: a paradigm based on the P300 Speller in
     overt attention condition and a paradigm based used in covert attention
@@ -972,14 +1020,23 @@
             doi="10.1088/1741-2560/11/3/035008",
         )
 
 
 class BNCI2015001(MNEBNCI):
     """BNCI 2015-001 Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name           #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        BNCI2015001       13       13           2                200  5s            512Hz                      2
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from [1]_.
 
     **Dataset description**
 
     We acquired the EEG from three Laplacian derivations, 3.5 cm (center-to-
     center) around the electrode positions (according to International 10-20
     System of Electrode Placement) C3 (FC3, C5, CP3 and C1), Cz (FCz, C1, CPz
@@ -1020,14 +1077,23 @@
             doi="10.1109/tnsre.2012.2189584",
         )
 
 
 class BNCI2015003(MNEBNCI):
     """BNCI 2015-003 P300 dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Name           #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        BNCI2015003       10        8  1500 NT / 300 T    0.8s             256Hz                      1
+        ===========  =======  =======  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     **Dataset description**
 
     This dataset contains recordings from 10 subjects performing a visual P300
     task for spelling. Results were published in [1]_. Sampling frequency was
     256 Hz and there were 8 electrodes ('Fz', 'Cz', 'P3', 'Pz', 'P4', 'PO7',
@@ -1055,14 +1121,23 @@
             doi="10.1016/j.neulet.2009.06.045",
         )
 
 
 class BNCI2015004(MNEBNCI):
     """BNCI 2015-004 Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name           #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        BNCI2015004       10       30           5                 80  7s            256Hz                      2
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from [1]_.
 
     **Dataset description**
 
     We provide EEG data recorded from nine users with disability (spinal cord
     injury and stroke) on two different days (sessions).  Users performed,
     follow- ing a cue-guided experimental paradigm, five distinct mental tasks
```

### Comparing `moabb-0.4.6/moabb/datasets/braininvaders.py` & `moabb-0.5.0/moabb/datasets/braininvaders.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 import os.path as osp
 import shutil
 import zipfile as z
 from distutils.dir_util import copy_tree
 
 import mne
 import numpy as np
+import pandas as pd
 import yaml
 from mne.channels import make_standard_montage
 from scipy.io import loadmat
 
 from moabb.datasets import download as dl
 from moabb.datasets.base import BaseDataset
 
 
 BI2012a_URL = "https://zenodo.org/record/2649069/files/"
 BI2013a_URL = "https://zenodo.org/record/2669187/files/"
 BI2014a_URL = "https://zenodo.org/record/3266223/files/"
 BI2014b_URL = "https://zenodo.org/record/3267302/files/"
 BI2015a_URL = "https://zenodo.org/record/3266930/files/"
 BI2015b_URL = "https://zenodo.org/record/3268762/files/"
+VIRTUALREALITY_URL = "https://zenodo.org/record/2605205/files/"
 
 
 def _bi_get_subject_data(ds, subject):  # noqa: C901
     file_path_list = ds.data_path(subject)
 
     sessions = {}
 
@@ -37,14 +39,17 @@
         ]:
             session_name = "session_1"
         elif ds.code == "Brain Invaders 2013a":
             session_number = file_path.split(os.sep)[-2].replace("Session", "")
             session_name = "session_" + session_number
         elif ds.code == "Brain Invaders 2015a":
             session_name = f'session_{file_path.split("_")[-1][1:2]}'
+        elif ds.code == "P300-VR":
+            session_name = file_path.split(".")[0].split("_")[-1]
+
         if session_name not in sessions.keys():
             sessions[session_name] = {}
 
         if ds.code == "Brain Invaders 2012":
             condition = file_path.split("/")[-1].split(".")[0].split(os.sep)[-1]
             run_name = "run_" + condition
             # fmt: off
@@ -141,30 +146,84 @@
             stim = D[-1, :]
             idx_target = (stim >= 60) & (stim <= 85)
             idx_nontarget = (stim >= 20) & (stim <= 45)
             stim[idx_target] = 2
             stim[idx_nontarget] = 1
             X = np.concatenate([S, stim[None, :]])
             sfreq = 512
+        elif ds.code == "Virtual Reality dataset":
+            data = loadmat(os.path.join(file_path, os.listdir(file_path)[0]))["data"]
+
+            chnames = [
+                "Fp1",
+                "Fp2",
+                "Fc5",
+                "Fz",
+                "Fc6",
+                "T7",
+                "Cz",
+                "T8",
+                "P7",
+                "P3",
+                "Pz",
+                "P4",
+                "P8",
+                "O1",
+                "Oz",
+                "O2",
+                "stim",
+            ]
+
+            S = data[:, 1:17]
+            stim = 2 * data[:, 18] + 1 * data[:, 19]
+            chtypes = ["eeg"] * 16 + ["stim"]
+            X = np.concatenate([S, stim[:, None]], axis=1).T
+
+            sfreq = 512
 
         info = mne.create_info(
             ch_names=chnames,
             sfreq=sfreq,
             ch_types=chtypes,
             verbose=False,
         )
-        raw = mne.io.RawArray(data=X, info=info, verbose=False)
-        raw.set_montage(make_standard_montage("standard_1020"))
 
-        if ds.code == "Brain Invaders 2012":
-            # get rid of the Fz channel (it is the ground)
-            raw.info["bads"] = ["Fz"]
-            raw.pick_types(eeg=True, stim=True)
+        if not ds.code == "Virtual Reality dataset":
+            raw = mne.io.RawArray(data=X, info=info, verbose=False)
+            raw.set_montage(make_standard_montage("standard_1020"))
+
+            if ds.code == "Brain Invaders 2012":
+                # get rid of the Fz channel (it is the ground)
+                raw.info["bads"] = ["Fz"]
+                raw.pick_types(eeg=True, stim=True)
+
+            sessions[session_name][run_name] = raw
+        else:
+            idx_blockStart = np.where(data[:, 20] > 0)[0]
+            idx_repetEndin = np.where(data[:, 21] > 0)[0]
+
+            sessions[session_name] = {}
+            for bi, idx_bi in enumerate(idx_blockStart):
+                start = idx_bi
+                end = idx_repetEndin[4::5][bi]
+                Xbi = X[:, start:end]
+
+                idx_repetEndin_local = (
+                    idx_repetEndin[bi * 5 : (bi * 5 + 5)] - idx_blockStart[bi]
+                )
+                idx_repetEndin_local = np.concatenate([[0], idx_repetEndin_local])
+                for j in range(5):
+                    start = idx_repetEndin_local[j]
+                    end = idx_repetEndin_local[j + 1]
+                    Xbij = Xbi[:, start:end]
+                    raw = mne.io.RawArray(data=Xbij, info=info, verbose=False)
+                    sessions[session_name][
+                        "block_" + str(bi + 1) + "-repetition_" + str(j + 1)
+                    ] = raw
 
-        sessions[session_name][run_name] = raw
     return sessions
 
 
 def _bi_data_path(  # noqa: C901
     ds, subject, path=None, force_update=False, update_path=None, verbose=None
 ):
     if subject not in ds.subject_list:
@@ -325,45 +384,59 @@
             osp.join(
                 path_folder,
                 f"group_{(subject+1)//2:02}",
                 f"group_{(subject+1)//2:02}_s{i}",
             )
             for i in range(1, 5)
         ]
+    elif ds.code == "Virtual Reality dataset":
+        subject_paths = []
+        url = "{:s}subject_{:02d}_{:s}.mat".format(
+            VIRTUALREALITY_URL,
+            subject,
+            "VR" if ds.virtual_reality else ds.personal_computer,
+        )
+        file_path = dl.data_path(url, "VIRTUALREALITY")
+        subject_paths.append(file_path)
 
     return subject_paths
 
 
 class bi2012(BaseDataset):
     """P300 dataset bi2012 from a "Brain Invaders" experiment
 
+    .. admonition:: Dataset summary
+        ================ ======= ======= ================ =============== =============== ===========
+         Name             #Subj   #Chan   #Trials/class    Trials length   Sampling Rate   #Sessions
+        ================ ======= ======= ================ =============== =============== ===========
+         bi2013a           25      16     6140 NT / 128 T       1s              512Hz          2
+        ================ ======= ======= ================ =============== =============== ===========
+
     Dataset following the setup from [1]_ carried-out at University of
     Grenoble Alpes.
 
-    **Dataset Description**
-
     This dataset contains electroencephalographic (EEG) recordings of 25 subjects testing
     the Brain Invaders, a visual P300 Brain-Computer Interface inspired by the famous vintage
     video game Space Invaders (Taito, Tokyo, Japan). The visual P300 is an event-related
     potential elicited by a visual stimulation, peaking 240-600 ms after stimulus onset. EEG
     data were recorded by 16 electrodes in an experiment that took place in the GIPSA-lab,
     Grenoble, France, in 2012). A full description of the experiment is available in [1]_.
 
-    **Authors**
+    :Principal Investigator: B.Sc. Gijsbrecht Franciscus Petrus Van Veen
+
+    :Technical Supervisors: Ph.D. Alexandre Barachant, Eng. Anton Andreev, Eng. Grégoire Cattan,
+                            Eng. Pedro. L. C. Rodrigues
 
-    Principal Investigator: B.Sc. Gijsbrecht Franciscus Petrus Van Veen
-    Technical Supervisors: Ph.D. Alexandre Barachant, Eng. Anton Andreev, Eng. Grégoire Cattan,
-                           Eng. Pedro. L. C. Rodrigues
-    Scientific Supervisor: Ph.D. Marco Congedo
+    :Scientific Supervisor: Ph.D. Marco Congedo
 
-    **ID of the dataset**
-    BI.EEG.2012-GIPSA
+    :ID of the dataset: BI.EEG.2012-GIPSA
 
     Notes
     -----
+
     .. versionadded:: 0.4.6
 
     References
     ----------
 
     .. [1] Van Veen, G., Barachant, A., Andreev, A., Cattan, G., Rodrigues, P. C., &
            Congedo, M. (2019). Building Brain Invaders: EEG data of an experimental validation.
@@ -393,19 +466,26 @@
     ):
         return _bi_data_path(self, subject, path, force_update, update_path, verbose)
 
 
 class bi2013a(BaseDataset):
     """P300 dataset bi2013a from a "Brain Invaders" experiment
 
+    .. admonition:: Dataset summary
+
+
+        =======  =======  =======  =================  ===============  ===============  =================
+        Name       #Subj    #Chan  #Trials / class    Trials length    Sampling rate    #Sessions
+        =======  =======  =======  =================  ===============  ===============  =================
+        bi2013a       24       16  3200 NT / 640 T    1s               512Hz            (1-7)8 s|(8-24)1s
+        =======  =======  =======  =================  ===============  ===============  =================
+
     Dataset following the setup from [1]_ carried-out at University of
     Grenoble Alpes.
 
-    **Dataset Description**
-
     This dataset concerns an experiment carried out at GIPSA-lab
     (University of Grenoble Alpes, CNRS, Grenoble-INP) in 2013.
     The recordings concerned 24 subjects in total. Subjects 1 to 7 participated
     to eight sessions, run in different days, subject 8 to 24 participated to
     one session. Each session consisted in two runs, one in a Non-Adaptive
     (classical) and one in an Adaptive (calibration-less) mode of operation.
     The order of the runs was randomized for each session. In both runs there
@@ -437,31 +517,31 @@
     * Digital Filter: no
     * Electrodes:  16 wet Silver/Silver Chloride electrodes positioned at
       FP1, FP2, F5, AFz, F6, T7, Cz, T8, P7, P3, Pz, P4, P8, O1, Oz, O2
       according to the 10/20 international system.
     * Reference: left ear-lobe.
     * Ground: N/A.
 
-    **Authors**
-
-    Principal Investigators: Erwan Vaineau, Dr. Alexandre Barachant
-    Scientific Supervisor :  Dr. Marco Congedo
-    Technical Supervisor : Anton Andreev
+    :Principal Investigators: Erwan Vaineau, Dr. Alexandre Barachant
+    :Scientific Supervisor:  Dr. Marco Congedo
+    :Technical Supervisor: Anton Andreev
 
     References
     ----------
 
     .. [1] Vaineau, E., Barachant, A., Andreev, A., Rodrigues, P. C.,
            Cattan, G. & Congedo, M. (2019). Brain invaders adaptive
            versus non-adaptive P300 brain-computer interface dataset.
            arXiv preprint arXiv:1904.09111.
+
     .. [2] Barachant A, Congedo M (2014) A Plug & Play P300 BCI using
            Information Geometry.
            arXiv:1409.0107.
-    .. [7] Congedo M, Goyat M, Tarrin N, Ionescu G, Rivet B,Varnet L, Rivet B,
+
+    .. [3] Congedo M, Goyat M, Tarrin N, Ionescu G, Rivet B,Varnet L, Rivet B,
            Phlypo R, Jrad N, Acquadro M, Jutten C (2011) “Brain Invaders”: a
            prototype of an open-source P300-based video game working with the
            OpenViBE platform. Proc. IBCI Conf., Graz, Austria, 280-283.
     """
 
     def __init__(self, NonAdaptive=True, Adaptive=False, Training=True, Online=False):
         super().__init__(
@@ -488,33 +568,37 @@
     ):
         return _bi_data_path(self, subject, path, force_update, update_path, verbose)
 
 
 class bi2014a(BaseDataset):
     """P300 dataset bi2014a from a "Brain Invaders" experiment
 
-    **Dataset Description**
+    .. admonition:: Dataset summary
+        ================ ======= ======= ================ =============== =============== ===========
+         Name             #Subj   #Chan   #Trials/class    Trials length   Sampling Rate   #Sessions
+        ================ ======= ======= ================ =============== =============== ===========
+         bi2014a           71      16        5 NT x 1 T         1s              512Hz       up to 3
+        ================ ======= ======= ================ =============== =============== ===========
 
     This dataset contains electroencephalographic (EEG) recordings of 71 subjects
     playing to a visual P300 Brain-Computer Interface (BCI) videogame named Brain Invaders.
     The interface uses the oddball paradigm on a grid of 36 symbols (1 Target, 35 Non-Target)
     that are flashed pseudo-randomly to elicit the P300 response. EEG data were recorded
     using 16 active dry electrodes with up to three game sessions. The experiment took place
     at GIPSA-lab, Grenoble, France, in 2014. A full description of the experiment is available
     at [1]_. The ID of this dataset is bi2014a.
 
-    **Authors**
-
-    Investigators: Eng. Louis Korczowski, B. Sc. Ekaterina Ostaschenko
-    Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
-                       M. Sc. Violette Gautheret
-    Scientific Supervisor: Ph.D. Marco Congedo
+    :Investigators: Eng. Louis Korczowski, B. Sc. Ekaterina Ostaschenko
+    :Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
+                        M. Sc. Violette Gautheret
+    :Scientific Supervisor: Ph.D. Marco Congedo
 
     Notes
     -----
+
     .. versionadded:: 0.4.6
 
     References
     ----------
 
     .. [1] Korczowski, L., Ostaschenko, E., Andreev, A., Cattan, G., Rodrigues, P. L. C.,
            Gautheret, V., & Congedo, M. (2019). Brain Invaders calibration-less P300-based
@@ -542,34 +626,38 @@
     ):
         return _bi_data_path(self, subject, path, force_update, update_path, verbose)
 
 
 class bi2014b(BaseDataset):
     """P300 dataset bi2014b from a "Brain Invaders" experiment
 
-    **Dataset Description**
+    .. admonition:: Dataset summary
+        ================ ======= ======= ================ =============== =============== ===========
+         Name             #Subj   #Chan   #Trials/class    Trials length   Sampling Rate   #Sessions
+        ================ ======= ======= ================ =============== =============== ===========
+         bi2014b           38      32        5 NT x 1 T         1s              512Hz           3
+        ================ ======= ======= ================ =============== =============== ===========
 
     This dataset contains electroencephalographic (EEG) recordings of 38 subjects playing in
     pair (19 pairs) to the multi-user version of a visual P300-based Brain-Computer Interface (BCI)
     named Brain Invaders. The interface uses the oddball paradigm on a grid of 36 symbols (1 Target,
     35 Non-Target) that are flashed pseudo-randomly to elicit a P300 response, an evoked-potential
     appearing about 300ms after stimulation onset. EEG data were recorded using 32 active wet
     electrodes per subjects (total: 64 electrodes) during three randomized conditions
     (Solo1, Solo2, Collaboration). The experiment took place at GIPSA-lab, Grenoble, France, in 2014.
     A full description of the experiment is available at [1]_. The ID of this dataset is bi2014b.
 
-    **Authors**
-
-    Investigators: Eng. Louis Korczowski, B. Sc. Ekaterina Ostaschenko
-    Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
-                       M. Sc. Violette Gautheret
-    Scientific Supervisor: Ph.D. Marco Congedo
+    :Investigators: Eng. Louis Korczowski, B. Sc. Ekaterina Ostaschenko
+    :Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
+                        M. Sc. Violette Gautheret
+    :Scientific Supervisor: Ph.D. Marco Congedo
 
     Notes
     -----
+
     .. versionadded:: 0.4.6
 
     References
     ----------
 
     .. [1] Korczowski, L., Ostaschenko, E., Andreev, A., Cattan, G., Rodrigues, P. L. C.,
            Gautheret, V., & Congedo, M. (2019). Brain Invaders Solo versus Collaboration:
@@ -597,35 +685,39 @@
     ):
         return _bi_data_path(self, subject, path, force_update, update_path, verbose)
 
 
 class bi2015a(BaseDataset):
     """P300 dataset bi2015a from a "Brain Invaders" experiment
 
-    **Dataset Description**
+    .. admonition:: Dataset summary
+        ================ ======= ======= ================ =============== =============== ===========
+         Name             #Subj   #Chan   #Trials/class    Trials length   Sampling Rate   #Sessions
+        ================ ======= ======= ================ =============== =============== ===========
+         bi2015a           50      32        5 NT x 1 T         1s              512Hz           3
+        ================ ======= ======= ================ =============== =============== ===========
 
     This dataset contains electroencephalographic (EEG) recordings
     of 43 subjects playing to a visual P300 Brain-Computer Interface (BCI)
     videogame named Brain Invaders. The interface uses the oddball paradigm
     on a grid of 36 symbols (1 Target, 35 Non-Target) that are flashed
     pseudo-randomly to elicit the P300 response. EEG data were recorded using
     32 active wet electrodes with three conditions: flash duration 50ms, 80ms
     or 110ms. The experiment took place at GIPSA-lab, Grenoble, France, in 2015.
     A full description of the experiment is available at [1]_. The ID of this
     dataset is bi2015a.
 
-    **Authors**
-
-    Investigators: Eng. Louis Korczowski, B. Sc. Martine Cederhout
-    Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
-                       M. Sc. Violette Gautheret
-    Scientific Supervisor: Ph.D. Marco Congedo
+    :Investigators: Eng. Louis Korczowski, B. Sc. Martine Cederhout
+    :Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
+                        M. Sc. Violette Gautheret
+    :Scientific Supervisor: Ph.D. Marco Congedo
 
     Notes
     -----
+
     .. versionadded:: 0.4.6
 
     References
     ----------
 
     .. [1] Korczowski, L., Cederhout, M., Andreev, A., Cattan, G., Rodrigues, P. L. C.,
            Gautheret, V., & Congedo, M. (2019). Brain Invaders calibration-less P300-based
@@ -653,38 +745,42 @@
     ):
         return _bi_data_path(self, subject, path, force_update, update_path, verbose)
 
 
 class bi2015b(BaseDataset):
     """P300 dataset bi2015b from a "Brain Invaders" experiment
 
-    **Dataset Description**
+       .. admonition:: Dataset summary
+        ================ ======= ======= ================ =============== =============== ===========
+         Name             #Subj   #Chan   #Trials/class    Trials length   Sampling Rate   #Sessions
+        ================ ======= ======= ================ =============== =============== ===========
+         bi2015b           44      32        5 NT x 1 T         1s              512Hz           2
+        ================ ======= ======= ================ =============== =============== ===========
 
     This dataset contains electroencephalographic (EEG) recordings
     of 44 subjects playing in pair to the multi-user version of a visual
     P300 Brain-Computer Interface (BCI) named Brain Invaders. The interface
     uses the oddball paradigm on a grid of 36 symbols (1 or 2 Target,
     35 or 34 Non-Target) that are flashed pseudo-randomly to elicit the
     P300 response. EEG data were recorded using 32 active wet electrodes
     per subjects (total: 64 electrodes) during four randomised conditions
     (Cooperation 1-Target, Cooperation 2-Targets, Competition 1-Target,
     Competition 2-Targets). The experiment took place at GIPSA-lab, Grenoble,
     France, in 2015. A full description of the experiment is available at
     A full description of the experiment is available at [1]_. The ID of this
     dataset is bi2015a.
 
-    **Authors**
-
-    Investigators: Eng. Louis Korczowski, B. Sc. Martine Cederhout
-    Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
-                       M. Sc. Violette Gautheret
-    Scientific Supervisor: Ph.D. Marco Congedo
+    :Investigators: Eng. Louis Korczowski, B. Sc. Martine Cederhout
+    :Technical Support: Eng. Anton Andreev, Eng. Grégoire Cattan, Eng. Pedro. L. C. Rodrigues,
+                        M. Sc. Violette Gautheret
+    :Scientific Supervisor: Ph.D. Marco Congedo
 
     Notes
     -----
+
     .. versionadded:: 0.4.6
 
     References
     ----------
 
     .. [1] Korczowski, L., Cederhout, M., Andreev, A., Cattan, G., Rodrigues, P. L. C.,
            Gautheret, V., & Congedo, M. (2019). Brain Invaders Cooperative versus Competitive:
@@ -707,7 +803,139 @@
         """return data for a single subject"""
         return _bi_get_subject_data(self, subject)
 
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
         return _bi_data_path(self, subject, path, force_update, update_path, verbose)
+
+
+class VirtualReality(BaseDataset):
+    """Dataset of an EEG-based BCI experiment in Virtual Reality using P300
+
+    .. admonition:: Dataset summary
+        ================ ======= ======= ================ =============== =============== ===========
+         Name             #Subj   #Chan   #Trials/class    Trials length   Sampling Rate   #Sessions
+        ================ ======= ======= ================ =============== =============== ===========
+         VirtualReality   24      16      600 NT / 120 T   1s              512Hz           2
+        ================ ======= ======= ================ =============== =============== ===========
+
+
+    We describe the experimental procedures for a dataset that we have made publicly
+    available at https://doi.org/10.5281/zenodo.2605204 in mat (Mathworks, Natick, USA)
+    and csv formats [1]_. This dataset contains electroencephalographic recordings on 21
+    subjects doing a visual P300 experiment on non-VR (PC display) and VR (virtual
+    reality). The visual P300 is an event-related potential elicited by a visual
+    stimulation, peaking 240-600 ms after stimulus onset. The experiment was designed
+    in order to compare the use of a P300-based brain-computer interface on a PC and
+    with a virtual reality headset, concerning the physiological, subjective and
+    performance aspects. The brain-computer interface is based on electroencephalography
+    (EEG). EEG data were recorded thanks to 16 electrodes. The virtual reality headset
+    consisted of a passive head-mounted display, that is, a head-mounted display which
+    does not include any electronics at the exception of a smartphone. A full description
+    of the experiment is available at https://hal.archives-ouvertes.fr/hal-02078533.
+
+    Parameters
+    ----------
+    virtual_reality: bool (default False)
+        if True, return runs corresponding to P300 experiment on virtual reality.
+    screen_display: bool (default True)
+        if True, return runs corresponding to P300 experiment on personal computer.
+
+    Notes
+    -----
+    .. versionadded:: 0.5.0
+
+    References
+    ----------
+    .. [1] G. Cattan, A. Andreev, P. L. C. Rodrigues, and M. Congedo (2019).
+            Dataset of an EEG-based BCI experiment in Virtual Reality and
+            on a Personal Computer. Research Report, GIPSA-lab; IHMTEK.
+            https://doi.org/10.5281/zenodo.2605204
+
+    .. versionadded:: 0.5.0
+    """
+
+    def __init__(self, virtual_reality=False, screen_display=True):
+        super().__init__(
+            subjects=list(range(1, 20 + 1)),
+            sessions_per_subject=1,
+            events=dict(Target=2, NonTarget=1),
+            code="P300-VR",
+            interval=[0, 1.0],
+            paradigm="p300",
+            doi="https://doi.org/10.5281/zenodo.2605204",
+        )
+
+        self.virtual_reality = virtual_reality
+        self.personal_computer = screen_display
+
+    def _get_single_subject_data(self, subject):
+        """return data for a single subject"""
+        return _bi_get_subject_data(self, subject)
+
+    def data_path(
+        self, subject, path=None, force_update=False, update_path=None, verbose=None
+    ):
+        return _bi_data_path(self, subject, path, force_update, update_path, verbose)
+
+    def get_block_repetition(self, paradigm, subjects, block_list, repetition_list):
+        """Select data for all provided subjects, blocks and repetitions.
+        Each subject has 5 blocks of 12 repetitions.
+
+        The returned data is a dictionary with the folowing structure::
+
+            data = {'subject_id' :
+                        {'session_id':
+                            {'run_id': raw}
+                        }
+                    }
+
+        See also
+        --------
+        BaseDataset.get_data
+
+        Parameters
+        ----------
+        subjects: List of int
+            List of subject number
+        block_list: List of int
+            List of block number (from 1 to 5)
+        repetition_list: List of int
+            List of repetition number inside a block (from 1 to 12)
+
+        Returns
+        -------
+        data: Dict
+            dict containing the raw data
+        """
+        X, labels, meta = paradigm.get_data(self, subjects)
+        X_select = []
+        labels_select = []
+        meta_select = []
+        for block in block_list:
+            for repetition in repetition_list:
+                X_select.append(
+                    X[
+                        meta["run"]
+                        == "block_" + str(block) + "-repetition_" + str(repetition)
+                    ]
+                )
+                labels_select.append(
+                    labels[
+                        meta["run"]
+                        == "block_" + str(block) + "-repetition_" + str(repetition)
+                    ]
+                )
+                meta_select.append(
+                    meta[
+                        meta["run"]
+                        == "block_" + str(block) + "-repetition_" + str(repetition)
+                    ]
+                )
+        X_select = np.concatenate(X_select)
+        labels_select = np.concatenate(labels_select)
+        meta_select = np.concatenate(meta_select)
+        df = pd.DataFrame(meta_select, columns=meta.columns)
+        meta_select = df
+
+        return X_select, labels_select, meta_select
```

### Comparing `moabb-0.4.6/moabb/datasets/download-tqdm.py` & `moabb-0.5.0/moabb/datasets/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,170 @@
 # Author: Alexandre Barachant <alexandre.barachant@gmail.com>
+#         Sylvain Chevallier <sylvain.chevallier@uvsq.fr>
 # License: BSD Style.
 
 import json
 import os
 import os.path as osp
+from pathlib import Path
 
 import requests
 from mne import get_config, set_config
-from mne.datasets.utils import _do_path_update, _get_path
-from mne.utils import _fetch_file, _url_to_local_path, verbose
-from pooch import file_hash, retrieve, FTPDownloader, HTTPDownloader, SFTPDownloader
+from mne.datasets.utils import _get_path
+from mne.utils import _url_to_local_path, verbose
+from pooch import file_hash, retrieve
 from requests.exceptions import HTTPError
 
 
+def get_dataset_path(sign, path):
+    """Returns the dataset path allowing for changes in MNE_DATA
+     config
+
+    Parameters
+    ----------
+    sign : str
+        Signifier of dataset
+    path : None | str
+        Location of where to look for the data storing location.
+        If None, the environment variable or config parameter
+        ``MNE_DATASETS_(signifier)_PATH`` is used. If it doesn't exist, the
+        "~/mne_data" directory is used. If the dataset
+        is not found under the given path, the data
+        will be automatically downloaded to the specified folder.
+
+    Returns
+    -------
+        path : None | str
+        Location of where to look for the data storing location
+    """
+    sign = sign.upper()
+    key = "MNE_DATASETS_{:s}_PATH".format(sign)
+    if get_config(key) is None:
+        if get_config("MNE_DATA") is None:
+            path_def = Path.home() / "mne_data"
+            print(
+                "MNE_DATA is not already configured. It will be set to "
+                "default location in the home directory - "
+                + str(path_def)
+                + "\nAll datasets will be downloaded to this location, if anything is "
+                "already downloaded, please move manually to this location"
+            )
+            if not path_def.is_dir():
+                path_def.mkdir(parents=True)
+            set_config("MNE_DATA", str(Path.home() / "mne_data"))
+        set_config(key, get_config("MNE_DATA"))
+    return _get_path(path, key, sign)
+
+
 @verbose
 def data_path(url, sign, path=None, force_update=False, update_path=True, verbose=None):
-    """Get path to local copy of given dataset URL.
+    """Get path to local copy of given dataset URL. **Deprecated**
 
     This is a low-level function useful for getting a local copy of a
-    remote dataset
+    remote dataset. It is deprecated in favor of data_dl.
 
     Parameters
     ----------
     url : str
         Path to remote location of data
     sign : str
         Signifier of dataset
     path : None | str
-        Location of where to look for the BNCI data storing location.
+        Location of where to look for the data storing location.
         If None, the environment variable or config parameter
         ``MNE_DATASETS_(signifier)_PATH`` is used. If it doesn't exist, the
         "~/mne_data" directory is used. If the dataset
         is not found under the given path, the data
         will be automatically downloaded to the specified folder.
     force_update : bool
         Force update of the dataset even if a local copy exists.
-    update_path : bool | None
-        If True, set the MNE_DATASETS_(signifier)_PATH in mne-python
-        config to the given path. If None, the user is prompted.
+    update_path : bool | None, **Deprecated**
+        Unused, kept for compatibility purpose.
     verbose : bool, str, int, or None
         If not None, override default verbose level (see :func:`mne.verbose`).
 
     Returns
     -------
     path : list of str
         Local path to the given data file. This path is contained inside a list
         of length one, for compatibility.
 
     """  # noqa: E501
-    sign = sign.upper()
-    key = "MNE_DATASETS_{:s}_PATH".format(sign)
+    path = get_dataset_path(sign, path)
     key_dest = "MNE-{:s}-data".format(sign.lower())
-    if get_config(key) is None:
-        set_config(key, osp.join(osp.expanduser("~"), "mne_data"))
-    path = _get_path(path, key, sign)
     destination = _url_to_local_path(url, osp.join(path, key_dest))
     # Fetch the file
     if not osp.isfile(destination) or force_update:
         if osp.isfile(destination):
             os.remove(destination)
         if not osp.isdir(osp.dirname(destination)):
             os.makedirs(osp.dirname(destination))
-        _fetch_file(url, destination, print_destination=False)
-
-    # Offer to update the path
-    _do_path_update(path, update_path, key, sign)
+        retrieve(url, None, path=destination)
     return destination
 
 
 @verbose
-def data_dl(url, sign, path=None, force_update=False, update_path=True, verbose=None):
+def data_dl(url, sign, path=None, force_update=False, verbose=None):
     """Download file from url to specified path
 
     This function should replace data_path as the MNE will not support the download
     of dataset anymore. This version is using Pooch.
-    Beware that now, all the file are stored directly in
 
     Parameters
     ----------
     url : str
         Path to remote location of data
     sign : str
         Signifier of dataset
     path : None | str
-        Location of where to look for the BNCI data storing location.
+        Location of where to look for the data storing location.
         If None, the environment variable or config parameter
         ``MNE_DATASETS_(signifier)_PATH`` is used. If it doesn't exist, the
         "~/mne_data" directory is used. If the dataset
         is not found under the given path, the data
         will be automatically downloaded to the specified folder.
     force_update : bool
         Force update of the dataset even if a local copy exists.
-    update_path : bool | None
-        If True, set the MNE_DATASETS_(signifier)_PATH in mne-python
-        config to the given path. If None, the user is prompted.
     verbose : bool, str, int, or None
         If not None, override default verbose level (see :func:`mne.verbose`).
 
     Returns
     -------
     path : list of str
         Local path to the given data file. This path is contained inside a list
         of length one, for compatibility.
     """
-    sign = sign.upper()
-    key = "MNE_DATASETS_{:s}_PATH".format(sign)
+    path = Path(get_dataset_path(sign, path))
     key_dest = "MNE-{:s}-data".format(sign.lower())
-    if get_config(key) is None:
-        set_config(key, osp.join(osp.expanduser("~"), "mne_data"))
-    path = _get_path(path, key, sign)
-    destination = _url_to_local_path(url, osp.join(path, key_dest))
-    protocol = url.split(':')[0].lower()
-    if protocol in ['http', 'https']:
-        dl = HTTPDownloader(progressbar=True)
-    elif protocol == 'ftp':
-        dl = FTPDownloader(progressbar=True)
-    elif protocol == 'sftp':
-        dl = SFTPDownloader(progressbar=True)
-    else:
-        dl = None
+    destination = _url_to_local_path(url, path / key_dest)
+    destination = str(path) + destination.split(str(path))[1]
+    table = {ord(c): "-" for c in ':*?"<>|'}
+    destination = Path(str(path) + destination.split(str(path))[1].translate(table))
 
     # Fetch the file
-    if not osp.isfile(destination) or force_update:
-        if osp.isfile(destination):
-            os.remove(destination)
-        if not osp.isdir(osp.dirname(destination)):
-            os.makedirs(osp.dirname(destination))
+    if not destination.is_file() or force_update:
+        if destination.is_file():
+            destination.unlink()
+        if not destination.parent.is_dir():
+            destination.parent.mkdir(parents=True)
         known_hash = None
     else:
-        known_hash = file_hash(destination)
+        known_hash = file_hash(str(destination))
     dlpath = retrieve(
-        url, known_hash, fname=osp.basename(url), path=osp.dirname(destination), downloader=dl,
+        url,
+        known_hash,
+        fname=Path(url).name,
+        path=str(destination.parent),
+        progressbar=True,
     )
-
-    # Offer to update the path
-    if update_path:
-        _do_path_update(path, update_path, key, sign)
-
     return dlpath
 
 
 # This function is from https://github.com/cognoma/figshare (BSD-3-Clause)
-def issue_request(method, url, headers, data=None, binary=False):
+def fs_issue_request(method, url, headers, data=None, binary=False):
     """Wrapper for HTTP request
 
     Parameters
     ----------
     method : str
         HTTP method. One of GET, PUT, POST or DELETE
     url : str
@@ -196,19 +215,20 @@
     response : dict
         HTTP request response as a python dict
     """
     fsurl = "https://api.figshare.com/v2"
     if version is None:
         url = fsurl + "/articles/{}/files".format(article_id)
         headers = {"Content-Type": "application/json"}
-        response = issue_request("GET", url, headers=headers)
+        response = fs_issue_request("GET", url, headers=headers)
         return response
     else:
         url = fsurl + "/articles/{}/versions/{}".format(article_id, version)
-        request = issue_request("GET", url, headers=headers)
+        headers = {"Content-Type": "application/json"}
+        request = fs_issue_request("GET", url, headers=headers)
         return request["files"]
 
 
 def fs_get_file_hash(filelist):
     """Returns a dict associating figshare file id to MD5 hash
 
     Parameters
```

### Comparing `moabb-0.4.6/moabb/datasets/epfl.py` & `moabb-0.5.0/moabb/datasets/epfl.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 
 EPFLP300_URL = "http://documents.epfl.ch/groups/m/mm/mmspg/www/BCI/p300/"
 
 
 class EPFLP300(BaseDataset):
     """P300 dataset from Hoffmann et al 2008.
 
+    .. admonition:: Dataset summary
+
+
+        ========  =======  =======  =================  ===============  ===============  ===========
+        Name        #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ========  =======  =======  =================  ===============  ===============  ===========
+        EPFLP300        8       32  2753 NT / 551 T    1s               2048Hz                     4
+        ========  =======  =======  =================  ===============  ===============  ===========
+
     Dataset from the paper [1]_.
 
     **Dataset Description**
 
     In the present work a six-choice P300 paradigm is tested using a population
     of five disabled and four able-bodied subjects. Six different images were
     flashed in random order with a stimulus interval of 400 ms. Users were
@@ -69,15 +78,14 @@
             code="EPFL P300 dataset",
             interval=[0, 1],
             paradigm="p300",
             doi="10.1016/j.jneumeth.2007.03.005",
         )
 
     def _get_single_run_data(self, file_path):
-
         # data from the .mat
         data = loadmat(file_path)
         signals = data["data"]
         stimuli = data["stimuli"].squeeze()
         events = data["events"]
         target = data["target"][0][0]
 
@@ -144,29 +152,27 @@
     def _get_single_subject_data(self, subject):
         """return data for a single subject"""
 
         file_path_list = self.data_path(subject)
         sessions = {}
 
         for file_path in sorted(file_path_list):
-
             session_name = "session_" + file_path.split(os.sep)[-2].replace("session", "")
 
             if session_name not in sessions.keys():
                 sessions[session_name] = {}
 
             run_name = "run_" + str(len(sessions[session_name]) + 1)
             sessions[session_name][run_name] = self._get_single_run_data(file_path)
 
         return sessions
 
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
-
         if subject not in self.subject_list:
             raise (ValueError("Invalid subject number"))
 
         # check if has the .zip
         url = "{:s}subject{:d}.zip".format(EPFLP300_URL, subject)
         path_zip = dl.data_dl(url, "EPFLP300")
         path_folder = path_zip.strip("subject{:d}.zip".format(subject))
```

### Comparing `moabb-0.4.6/moabb/datasets/gigadb.py` & `moabb-0.5.0/moabb/datasets/gigadb.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,23 @@
 log = logging.getLogger(__name__)
 GIGA_URL = "ftp://parrot.genomics.cn/gigadb/pub/10.5524/100001_101000/100295/mat_data/"
 
 
 class Cho2017(BaseDataset):
     """Motor Imagery dataset from Cho et al 2017.
 
+    .. admonition:: Dataset summary
+
+
+        =======  =======  =======  ==========  =================  ============  ===============  ===========
+        Name       #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        =======  =======  =======  ==========  =================  ============  ===============  ===========
+        Cho2017       53       64           2                100  3s            512Hz                      1
+        =======  =======  =======  ==========  =================  ============  ===============  ===========
+
     Dataset from the paper [1]_.
 
     **Dataset Description**
 
     We conducted a BCI experiment for motor imagery movement (MI movement)
     of the left and right hands with 52 subjects (19 females, mean age ± SD
     age = 24.8 ± 3.86 years); Each subject took part in the same experiment,
```

### Comparing `moabb-0.4.6/moabb/datasets/huebner_llp.py` & `moabb-0.5.0/moabb/datasets/huebner_llp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import glob
-import os
 import re
 import zipfile
 from abc import ABC
+from pathlib import Path
 
 import mne
 import numpy as np
 
 from moabb.datasets import download as dl
 from moabb.datasets.base import BaseDataset
 
@@ -17,15 +16,14 @@
 OPTICAL_MARKER_CODE = 500
 
 
 class _BaseVisualMatrixSpellerDataset(BaseDataset, ABC):
     def __init__(
         self, src_url, n_subjects, raw_slice_offset, use_blocks_as_sessions=True, **kwargs
     ):
-
         self.n_channels = 31  # all channels except 5 times x_* CH and EOGvu
         if kwargs["interval"] is None:
             # "Epochs were windowed to [−200, 700] ms relative to the stimulus onset [...]."
             kwargs["interval"] = [-0.2, 0.7]
 
         super().__init__(
             events=dict(Target=10002, NonTarget=10001),
@@ -36,23 +34,24 @@
 
         self.raw_slice_offset = 2_000 if raw_slice_offset is None else raw_slice_offset
         self._src_url = src_url
         self.use_blocks_as_sessions = use_blocks_as_sessions
 
     @staticmethod
     def _filename_trial_info_extraction(vhdr_file_path):
-        vhdr_file_name = os.path.basename(vhdr_file_path)
+        vhdr_file_path = Path(vhdr_file_path)
+        vhdr_file_name = vhdr_file_path.name
         run_file_pattern = "^matrixSpeller_Block([0-9]+)_Run([0-9]+)\\.vhdr$"
         vhdr_file_patter_match = re.match(run_file_pattern, vhdr_file_name)
 
         if not vhdr_file_patter_match:
             # TODO: raise a wild exception?
             print(vhdr_file_path)
 
-        session_name = os.path.basename(os.path.dirname(vhdr_file_path))
+        session_name = vhdr_file_path.parent.name
         block_idx = vhdr_file_patter_match.group(1)
         run_idx = vhdr_file_patter_match.group(2)
         return session_name, block_idx, run_idx
 
     def _get_single_subject_data(self, subject):
         subject_data_vhdr_files = self.data_path(subject)
         sessions = dict()
@@ -80,49 +79,47 @@
 
         return sessions
 
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
         url = f"{self._src_url}subject{subject:02d}.zip"
-        data_archive_path = dl.data_dl(url, "llp")
-        data_dir_extracted_path = os.path.dirname(data_archive_path)
-        # else:
-        #     raise ValueError(f'URL or data path must be given but both are None.')
-
-        subject_dir_path = os.path.join(data_dir_extracted_path, f"subject{subject:02d}")
-
-        data_extracted = os.path.isdir(subject_dir_path)
-        if not data_extracted:
-            # print('unzip', path_to_data_archive)  # TODO logging? check verbose
-            zipfile_path = glob.glob(
-                os.path.join(data_dir_extracted_path, data_archive_path, "*.zip")
-            )[0]
+        zipfile_path = Path(dl.data_dl(url, "llp"))
+        zipfile_extracted_path = zipfile_path.parent
+
+        subject_dir_path = zipfile_extracted_path / f"subject{subject:02d}"
+
+        if not subject_dir_path.is_dir():
             _BaseVisualMatrixSpellerDataset._extract_data(
-                data_dir_extracted_path, zipfile_path
+                zipfile_extracted_path, zipfile_path
             )
 
-        run_glob_pattern = os.path.join(
-            data_dir_extracted_path,
-            f"subject{subject:02d}",
-            "matrixSpeller_Block*_Run*.vhdr",
-        )
-        subject_paths = glob.glob(run_glob_pattern)
+        subject_paths = zipfile_extracted_path / f"subject{subject:02d}"
+        subject_paths = subject_paths.glob("matrixSpeller_Block*_Run*.vhdr")
+        subject_paths = [str(p) for p in subject_paths]
         return sorted(subject_paths)
 
     @staticmethod
     def _extract_data(data_dir_extracted_path, data_archive_path):
         zip_ref = zipfile.ZipFile(data_archive_path, "r")
         zip_ref.extractall(data_dir_extracted_path)
 
 
 class Huebner2017(_BaseVisualMatrixSpellerDataset):
     """
     Learning from label proportions for a visual matrix speller (ERP) dataset from Hübner et al 2017 [1]_.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Name           #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Huebner2017       13       31                     0.9s             1000Hz                     1
+        ===========  =======  =======  =================  ===============  ===============  ===========
 
     **Dataset description**
 
     The subjects were asked to spell the sentence: “Franzy jagt im komplett verwahrlosten Taxi quer durch Freiburg”.
     The sentence was chosen because it contains each letter used in German at least once. Each subject spelled this
     sentence three times. The stimulus onset asynchrony (SOA) was 250 ms (corresponding to 15 frames on the LCD screen
     utilized) while the stimulus duration was 100 ms (corresponding to 6 frames on the LCD screen utilized). For each
@@ -174,14 +171,25 @@
         )
 
 
 class Huebner2018(_BaseVisualMatrixSpellerDataset):
     """
     Mixture of LLP and EM for a visual matrix speller (ERP) dataset from Hübner et al 2018 [1]_.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Name           #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ===========  =======  =======  =================  ===============  ===============  ===========
+        Huebner2018       12       31                     0.9s             1000Hz                     1
+        ===========  =======  =======  =================  ===============  ===============  ===========
+
+    **Dataset description**
+
     Within a single session, a subject was asked to spell the beginning of a sentence in each of three blocks.The text
     consists of the 35 symbols “Franzy jagt im Taxi quer durch das ”. Each block, one of the three decoding
     algorithms (EM, LLP, MIX) was used in order to guess the attended symbol. The order of the blocks was
     pseudo-randomized over subjects, such that each possible order of the three decoding algorithms was used twice.
     This randomization should reduce systematic biases by order effects or temporal effects, e.g., due to fatigue or
     task-learning.
```

### Comparing `moabb-0.4.6/moabb/datasets/mpi_mi.py` & `moabb-0.5.0/moabb/datasets/mpi_mi.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 
 DOWNLOAD_URL = "https://zenodo.org/record/1217449/files/"
 
 
 class MunichMI(BaseDataset):
     """Munich Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name        #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ========  =======  =======  ==========  =================  ============  ===============  ===========
+        MunichMI       10      128           2                150  7s            500Hz                      1
+        ========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Motor imagery dataset from Grosse-Wentrup et al. 2009 [1]_.
 
     A trial started with the central display of a white fixation cross. After 3
     s, a white arrow was superimposed on the fixation cross, either pointing to
     the left or the right.
     Subjects were instructed to perform haptic motor imagery of the
     left or the right hand during display of the arrow, as indicated by the
```

### Comparing `moabb-0.4.6/moabb/datasets/neiry.py` & `moabb-0.5.0/moabb/datasets/neiry.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 from . import download as dl
 from .base import BaseDataset
 
 
 class DemonsP300(BaseDataset):
     """Visual P300 dataset recorded in Virtual Reality (VR) game Raccoons versus Demons.
 
+    .. admonition:: Dataset summary
+
+
+        ==========  =======  =======  =================  ===============  ===============  ===========
+        Name          #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        ==========  =======  =======  =================  ===============  ===============  ===========
+        DemonsP300       60        8  935 NT / 50 T      1s               500Hz                      1
+        ==========  =======  =======  =================  ===============  ===============  ===========
+
+    .. danger::
+
+       This dataset contains major unresolved issues and could removed in the near futur. Use it in a benchmark
+       at your own risk. See https://github.com/NeuroTechX/moabb/issues/216
+
     **Dataset Description**
 
     We publish dataset of visual P300 BCI performed in Virtual Reality (VR) game Raccoons versus
     Demons (RvD). Data contains reach labels incorporating information about stimulus chosen enabling us
     to estimate model’s confidence at each stimulus prediction stage.
     `target` channel contains standard P300 target/non-target labels,
     while `mult_target` channel contains multiclass labels (numbers of activated stimuli).
@@ -71,26 +85,26 @@
 
     _ms_in_sec = 1000
     _hdf_path = "p300dataset"
     _ds_folder_name = "demons"
 
     _act_dtype = np.dtype(
         [
-            ("id", np.int),
-            ("target", np.int),
-            ("is_train", np.bool),
-            ("prediction", np.int),
-            ("sessions", np.object),  # list of `_session_dtype`
+            ("id", int),
+            ("target", int),
+            ("is_train", bool),
+            ("prediction", int),
+            ("sessions", object),  # list of `_session_dtype`
         ]
     )
     _session_dtype = np.dtype(
         [
-            ("eeg", np.object),
-            ("starts", np.object),
-            ("stimuli", np.object),
+            ("eeg", object),
+            ("starts", object),
+            ("stimuli", object),
         ]
     )
 
     def __init__(self):
         super().__init__(
             subjects=list(range(60)),
             sessions_per_subject=1,
@@ -147,15 +161,15 @@
         for i, act in enumerate(record):
             # target and stims are increased by 1
             # because the channel is filled with zeros by default
             target = act["target"] + 1
             run_data = []
             for eeg, starts, stims in act["sessions"]:
                 starts = starts * self.sampling_rate / self._ms_in_sec
-                starts = starts.round().astype(np.int)
+                starts = starts.round().astype(int)
                 stims = stims + 1
                 stims_channel = np.zeros(eeg.shape[1])
                 target_channel = np.zeros(eeg.shape[1])
 
                 for start, stimul in zip(starts, stims):
                     stims_channel[start] = stimul
                     target_channel[start] = 1 if stimul == target else 2
```

### Comparing `moabb-0.4.6/moabb/datasets/physionet_mi.py` & `moabb-0.5.0/moabb/datasets/physionet_mi.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 
 BASE_URL = "https://physionet.org/files/eegmmidb/1.0.0/"
 
 
 class PhysionetMI(BaseDataset):
     """Physionet Motor Imagery dataset.
 
+    .. admonition:: Dataset summary
+
+
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name           #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+        PhysionetMI      109       64           4                 23  3s            160Hz                      1
+        ===========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Physionet MI dataset: https://physionet.org/pn4/eegmmidb/
 
     This data set consists of over 1500 one- and two-minute EEG recordings,
     obtained from 109 volunteers [2]_.
 
     Subjects performed different motor/imagery tasks while 64-channel EEG were
     recorded using the BCI2000 system (http://www.bci2000.org) [1]_.
```

### Comparing `moabb-0.4.6/moabb/datasets/sosulski2019.py` & `moabb-0.5.0/moabb/datasets/sosulski2019.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,26 @@
     "https://freidok.uni-freiburg.de/fedora/objects/freidok:154576/datastreams"
 )
 
 
 class Sosulski2019(BaseDataset):
     """P300 dataset from initial spot study.
 
-    Dataset [1], study on spatial transfer between SOAs [2], actual paradigm / online optimization [3].
+    Dataset [1]_, study on spatial transfer between SOAs [2]_, actual paradigm / online optimization [3]_.
 
-    **Dataset Description**
+    .. admonition:: Dataset summary
 
+
+        =============  =======  =======  =================  ===============  ===============  ===========
+        Name             #Subj    #Chan  #Trials / class    Trials length    Sampling rate      #Sessions
+        =============  =======  =======  =================  ===============  ===============  ===========
+        Sosulski2019       13       32   75 NT / 15 T                        1000Hz                     1
+        =============  =======  =======  =================  ===============  ===============  ===========
+
+    **Dataset description**
     This dataset contains multiple small trials of an auditory oddball paradigm. The paradigm presented two different
     sinusoidal tones. A low-pitched (500 Hz, 40 ms duration) non-target tone and a high-pitched (1000 Hz,
     40 ms duration) target tone. Subjects were instructed to attend to the high-pitched target tones and ignore the
     low-pitched tones.
 
     One trial (= one file) consisted of 90 tones, 15 targets and 75 non-targets. The order was pseudo-randomized in a
     way that at least two non-target tones occur between two target tones. Additionally, if you split the 90 tones of
@@ -45,28 +53,38 @@
     recording, the cap was prepared such that impedances on all electrodes were around 20 kOhm. The EEG signal was
     recorded at 1000 Hz.
 
     The data contains 31 scalp channels, one EOG channel and five miscellaneous non-EEG signal channels. However,
     only scalp EEG and the EOG channel is available in all subjects. The markers in the marker file indicate the
     onset of target tones (21) and non-target tones (1).
 
-    WARNING: Note that this wrapper currently only loads the second part of the experiment and uses pseudo-sessions
-    to achieve the functionality to handle different conditions in MOABB. As a result, the statistical testing
-    features of MOABB cannot be used for this dataset.
+    .. caution::
+
+       Note that this wrapper currently only loads the second part of the experiment and uses pseudo-sessions
+       to achieve the functionality to handle different conditions in MOABB. As a result, the statistical testing
+       features of MOABB cannot be used for this dataset.
 
     References
     ----------
 
     .. [1] Sosulski, J., Tangermann, M.: Electroencephalogram signals recorded from 13 healthy subjects during an
-    auditory oddball paradigm under different stimulus onset asynchrony conditions. Dataset. DOI: 10.6094/UNIFR/154576
+           auditory oddball paradigm under different stimulus onset asynchrony conditions.
+           Dataset. DOI: 10.6094/UNIFR/154576
+
     .. [2] Sosulski, J., Tangermann, M.: Spatial filters for auditory evoked potentials transfer between different
-    experimental conditions. Graz BCI Conference. 2019.
-    .. [3] Sosulski, J., Hübner, D., Klein, A., Tangermann, M.:  Online Optimization of Stimulation Speed in an Auditory Brain-Computer Interface under Time Constraints. arXiv preprint. 2021.
+           experimental conditions. Graz BCI Conference. 2019.
+
+    .. [3] Sosulski, J., Hübner, D., Klein, A., Tangermann, M.:  Online Optimization of Stimulation Speed in
+           an Auditory Brain-Computer Interface under Time Constraints. arXiv preprint. 2021.
+
+    Notes
+    -----
 
     .. versionadded:: 0.4.5
+
     """
 
     def __init__(
         self,
         use_soas_as_sessions=True,
         load_soa_60=False,
         reject_non_iid=False,
@@ -149,15 +167,14 @@
             sessions[session_name][run_name] = self._get_single_run_data(file_path)
 
         return sessions
 
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
-
         if subject not in self.subject_list:
             raise (ValueError("Invalid subject number"))
 
         # check if has the .zip
         file_number = Sosulski2019._map_subject_to_filenumber(subject)
         url = f"{SPOT_PILOT_P300_URL}/FILE{file_number}/content"
         path_zip = dl.data_dl(url, "spot")
```

### Comparing `moabb-0.4.6/moabb/datasets/ssvep_mamem.py` & `moabb-0.5.0/moabb/datasets/ssvep_mamem.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         else:
             s = s + (current - previous)
             c = c + 1
         previous = timestamps[i]
     sampleB = samples[i - 1]
     freqs.append(s // c)
     t_start.append(sampleA)
-    freqs = np.array(freqs, dtype=np.int) * 2
+    freqs = np.array(freqs, dtype=int) * 2
     freqs = 1000 // freqs
     t_start = np.array(t_start)
 
     if labels is None:
         freqs_labels = {6: 1, 7: 2, 8: 3, 9: 4, 11: 5}
         for f, t in zip(freqs, t_start):
             eeg[-1, t] = freqs_labels[f]
@@ -104,32 +104,32 @@
         sessions = {}
 
         for fpath in fnames:
             fnamed = fsn[osp.basename(fpath)]
             if fnamed[4] == "x":
                 continue
             session_name = "session_0"
-            if self.code == "SSVEP MAMEM3":
+            if self.code == "MAMEM3_SSVEP":
                 repetition = len(fnamed) - 10
                 run_name = f"run_{(ord(fnamed[4])-97)*2 + repetition}"
             else:
                 run_name = f"run_{ord(fnamed[4])-97}"
 
-            if self.code == "SSVEP MAMEM3":
+            if self.code == "MAMEM3_SSVEP":
                 m = loadmat(fpath)
                 ch_names = [e[0] for e in m["info"][0, 0][9][0]]
                 sfreq = 128
                 montage = make_standard_montage("standard_1020")
                 eeg = m["eeg"]
             else:
                 m = loadmat(fpath, squeeze_me=True)
                 ch_names = [f"E{i + 1}" for i in range(0, 256)]
                 ch_names.append("stim")
                 sfreq = 250
-                if self.code == "SSVEP MAMEM2":
+                if self.code == "MAMEM2_SSVEP":
                     labels = m["labels"]
                 else:
                     labels = None
                 eeg = mamem_event(m["eeg"], m["DIN_1"], labels=labels)
                 montage = make_standard_montage("GSN-HydroCel-256")
             ch_types = ["eeg"] * (len(ch_names) - 1) + ["stim"]
             info = create_info(ch_names, sfreq, ch_types)
@@ -146,15 +146,15 @@
     def data_path(
         self, subject, path=None, force_update=False, update_path=None, verbose=None
     ):
         if subject not in self.subject_list:
             raise (ValueError("Invalid subject number"))
 
         sub = f"{subject:02d}"
-        sign = self.code.split()[1]
+        sign = self.code.split("_")[0]
         key_dest = f"MNE-{sign.lower():s}-data"
         path = osp.join(get_dataset_path(sign, path), key_dest)
 
         filelist = fs_get_file_list(self.figshare_id)
         reg = fs_get_file_hash(filelist)
         fsn = fs_get_file_id(filelist)
         gb = pooch.create(path=path, base_url=MAMEM_URL, registry=reg)
@@ -165,14 +165,23 @@
                 spath.append(gb.fetch(fsn[f]))
         return spath
 
 
 class MAMEM1(BaseMAMEM):
     """SSVEP MAMEM 1 dataset
 
+    .. admonition:: Dataset summary
+
+
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+        Name      #Subj    #Chan    #Classes  #Trials / class    Trials length    Sampling rate      #Sessions
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+        MAMEM1       10      256           5  12-15              3s               250Hz                      1
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     EEG signals with 256 channels captured from 11 subjects executing a
     SSVEP-based experimental protocol. Five different frequencies
     (6.66, 7.50, 8.57, 10.00 and 12.00 Hz) have been used for the visual
     stimulation,and the EGI 300 Geodesic EEG System (GES 300), using a
     stimulation, HydroCel Geodesic Sensor Net (HCGSN) and a sampling rate of
@@ -267,23 +276,32 @@
     """
 
     def __init__(self):
         super().__init__(
             events={"6.66": 1, "7.50": 2, "8.57": 3, "10.00": 4, "12.00": 5},
             sessions_per_subject=1,
             # 5 runs per sessions, except 3 for S001, S003, S008, 4 for S004
-            code="SSVEP MAMEM1",
+            code="MAMEM1_SSVEP",
             doi="https://arxiv.org/abs/1602.00904",
             figshare_id=2068677,
         )
 
 
 class MAMEM2(BaseMAMEM):
     """SSVEP MAMEM 2 dataset
 
+    .. admonition:: Dataset summary
+
+
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+        Name      #Subj    #Chan    #Classes  #Trials / class    Trials length    Sampling rate      #Sessions
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+        MAMEM2       10      256           5  20-30              3s               250Hz                      1
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     EEG signals with 256 channels captured from 11 subjects executing a
     SSVEP-based experimental protocol. Five different frequencies
     (6.66, 7.50, 8.57, 10.00 and 12.00 Hz) have been used for the visual
     stimulation,and the EGI 300 Geodesic EEG System (GES 300), using a
     stimulation, HydroCel Geodesic Sensor Net (HCGSN) and a sampling rate of
@@ -351,23 +369,32 @@
            `<https://figshare.com/articles/dataset/MAMEM_EEG_SSVEP_Dataset_II_256_channels_11_subjects_5_frequencies_presented_simultaneously_/3153409?file=4911931>`_  # noqa: E501
     """
 
     def __init__(self):
         super().__init__(
             events={"6.66": 1, "7.50": 2, "8.57": 3, "10.00": 4, "12.00": 5},
             sessions_per_subject=1,
-            code="SSVEP MAMEM2",
+            code="MAMEM2_SSVEP",
             doi="https://arxiv.org/abs/1602.00904",
             figshare_id=3153409,
         )
 
 
 class MAMEM3(BaseMAMEM):
     """SSVEP MAMEM 3 dataset
 
+    .. admonition:: Dataset summary
+
+
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+        Name      #Subj    #Chan    #Classes  #Trials / class    Trials length    Sampling rate      #Sessions
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+        MAMEM3       10       14           4  20-30              3s               128Hz                      1
+        ======  =======  =======  ==========  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     EEG signals with 14 channels captured from 11 subjects executing a
     SSVEP-based experimental protocol. Five different frequencies
     (6.66, 7.50, 8.57, 10.00 and 12.00 Hz) have been used for the visual
     stimulation, and the Emotiv EPOC, using 14 wireless channels has been used
     for capturing the signals.
@@ -450,11 +477,11 @@
                 "6.66": 33029,
                 "7.50": 33028,
                 "8.57": 33027,
                 "10.00": 33026,
                 "12.00": 33025,
             },
             sessions_per_subject=1,
-            code="SSVEP MAMEM3",
+            code="MAMEM3_SSVEP",
             doi="https://arxiv.org/abs/1602.00904",
             figshare_id=3413851,
         )
```

### Comparing `moabb-0.4.6/moabb/datasets/ssvep_nakanishi.py` & `moabb-0.5.0/moabb/datasets/ssvep_nakanishi.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 
 NAKAHISHI_URL = "https://github.com/mnakanishi/12JFPM_SSVEP/raw/master/data/"
 
 
 class Nakanishi2015(BaseDataset):
     """SSVEP Nakanishi 2015 dataset
 
+    .. admonition:: Dataset summary
+
+
+        =============  =======  =======  ==========  =================  ===============  ===============  ===========
+        Name             #Subj    #Chan    #Classes    #Trials / class  Trials length    Sampling rate      #Sessions
+        =============  =======  =======  ==========  =================  ===============  ===============  ===========
+        Nakanishi2015        9        8          12                 15  4.15s            256Hz                      1
+        =============  =======  =======  ==========  =================  ===============  ===============  ===========
+
     This dataset contains 12-class joint frequency-phase modulated steady-state
     visual evoked potentials (SSVEPs) acquired from 10 subjects used to
     estimate an online performance of brain-computer interface (BCI) in the
     reference study [1]_.
 
     references
     ----------
@@ -50,15 +59,15 @@
                 "10.25": 7,
                 "12.25": 8,
                 "14.25": 9,
                 "10.75": 10,
                 "12.75": 11,
                 "14.75": 12,
             },
-            code="SSVEP Nakanishi",
+            code="Nakanishi_SSVEP",
             interval=[0.15, 4.3],
             paradigm="ssvep",
             doi="doi.org/10.1371/journal.pone.0140703",
         )
 
     def _get_single_subject_data(self, subject):
         """Return the data of a single subject"""
```

### Comparing `moabb-0.4.6/moabb/datasets/ssvep_wang.py` & `moabb-0.5.0/moabb/datasets/ssvep_wang.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 WANG_URL = "ftp://sccn.ucsd.edu/pub/ssvep_benchmark_dataset/"
 # WANG_URL = "http://www.thubci.com/uploads/down/"
 
 
 class Wang2016(BaseDataset):
     """SSVEP Wang 2016 dataset
 
+    .. admonition:: Dataset summary
+
+
+        ========  =======  =======  ==========  =================  ===============  ===============  ===========
+        Name        #Subj    #Chan    #Classes    #Trials / class  Trials length    Sampling rate      #Sessions
+        ========  =======  =======  ==========  =================  ===============  ===============  ===========
+        Wang2016       32       62          40                  6  5s               250Hz                      1
+        ========  =======  =======  ==========  =================  ===============  ===============  ===========
+
     Dataset from [1]_.
 
     This dataset gathered SSVEP-BCI recordings of 35 healthy subjects (17
     females, aged 17-34 years, mean age: 22 years) focusing on 40 characters
     flickering at different frequencies (8-15.8 Hz with an interval of 0.2 Hz).
     For each subject, the experiment consisted of 6 blocks. Each block
     contained 40 trials corresponding to all 40 characters indicated in a
@@ -100,15 +109,15 @@
     # fmt: on
 
     def __init__(self):
         super().__init__(
             subjects=list(range(1, 35)),
             sessions_per_subject=1,
             events=self._events,
-            code="SSVEP Wang",
+            code="Wang_SSVEP",
             interval=[0.5, 5.5],
             paradigm="ssvep",
             doi="doi://10.1109/TNSRE.2016.2627556",
         )
 
     def _get_single_subject_data(self, subject):
         """Return the data of a single subject"""
```

### Comparing `moabb-0.4.6/moabb/datasets/upper_limb.py` & `moabb-0.5.0/moabb/datasets/upper_limb.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 UPPER_LIMB_URL = "https://zenodo.org/record/834976/files/"
 
 
 class Ofner2017(BaseDataset):
     """Motor Imagery ataset from Ofner et al 2017.
 
+    .. admonition:: Dataset summary
+
+
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Name         #Subj    #Chan    #Classes    #Trials / class  Trials len    Sampling rate      #Sessions
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+        Ofner2017       15       61           7                 60  3s            512Hz                      1
+        =========  =======  =======  ==========  =================  ============  ===============  ===========
+
     Upper limb Motor imagery dataset from the paper [1]_.
 
     **Dataset description**
 
     We recruited 15 healthy subjects aged between 22 and 40 years with a mean
     age of 27 years (standard deviation 5 years). Nine subjects were female,
     and all the subjects except s1 were right-handed.
```

### Comparing `moabb-0.4.6/moabb/datasets/utils.py` & `moabb-0.5.0/moabb/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `moabb-0.4.6/moabb/evaluations/base.py` & `moabb-0.5.0/moabb/evaluations/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         Suffix for the results file.
     hdf5_path: str
         Specific path for storing the results.
     additional_columns: None
         Adding information to results.
     return_epochs: bool, default=False
         use MNE epoch to train pipelines.
+    return_raws: bool, default=False
+        use MNE raw to train pipelines.
     mne_labels: bool, default=False
         if returning MNE epoch, use original dataset label if True
     """
 
     def __init__(
         self,
         paradigm,
@@ -52,21 +54,23 @@
         n_jobs=1,
         overwrite=False,
         error_score="raise",
         suffix="",
         hdf5_path=None,
         additional_columns=None,
         return_epochs=False,
+        return_raws=False,
         mne_labels=False,
     ):
         self.random_state = random_state
         self.n_jobs = n_jobs
         self.error_score = error_score
         self.hdf5_path = hdf5_path
         self.return_epochs = return_epochs
+        self.return_raws = return_raws
         self.mne_labels = mne_labels
 
         # check paradigm
         if not isinstance(paradigm, BaseParadigm):
             raise (ValueError("paradigm must be an Paradigm instance"))
         self.paradigm = paradigm
 
@@ -118,24 +122,26 @@
             type(self.paradigm),
             overwrite=overwrite,
             suffix=suffix,
             hdf5_path=self.hdf5_path,
             additional_columns=additional_columns,
         )
 
-    def process(self, pipelines):
+    def process(self, pipelines, param_grid=None):
         """Runs all pipelines on all datasets.
 
         This function will apply all provided pipelines and return a dataframe
         containing the results of the evaluation.
 
         Parameters
         ----------
         pipelines : dict of pipeline instance.
             A dict containing the sklearn pipeline to evaluate.
+        param_grid : dict of str
+            The key of the dictionary must be the same as the associated pipeline.
 
         Returns
         -------
         results: pd.DataFrame
             A dataframe containing the results.
 
         """
@@ -146,15 +152,15 @@
 
         for _, pipeline in pipelines.items():
             if not (isinstance(pipeline, BaseEstimator)):
                 raise (ValueError("pipelines must only contains Pipelines " "instance"))
 
         for dataset in self.datasets:
             log.info("Processing dataset: {}".format(dataset.code))
-            results = self.evaluate(dataset, pipelines)
+            results = self.evaluate(dataset, pipelines, param_grid)
             for res in results:
                 self.push_result(res, pipelines)
 
         return self.results.to_dataframe(pipelines=pipelines)
 
     def push_result(self, res, pipelines):
         message = "{} | ".format(res["pipeline"])
@@ -165,15 +171,15 @@
         log.info(message)
         self.results.add({res["pipeline"]: res}, pipelines=pipelines)
 
     def get_results(self):
         return self.results.to_dataframe()
 
     @abstractmethod
-    def evaluate(self, dataset, pipelines):
+    def evaluate(self, dataset, pipelines, param_grid):
         """Evaluate results on a single dataset.
 
         This method return a generator. each results item is a dict with
         the following convension::
 
             res = {'time': Duration of the training ,
                    'dataset': dataset id,
```

### Comparing `moabb-0.4.6/moabb/paradigms/base.py` & `moabb-0.5.0/moabb/paradigms/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import logging
-from abc import ABCMeta, abstractmethod, abstractproperty
+from abc import ABCMeta, abstractmethod
 
 import mne
 import numpy as np
 import pandas as pd
 
 
 log = logging.getLogger(__name__)
 
 
 class BaseParadigm(metaclass=ABCMeta):
     """Base Paradigm."""
 
+    @abstractmethod
     def __init__(self):
         pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def scoring(self):
         """Property that defines scoring metric (e.g. ROC-AUC or accuracy
         or f-score), given as a sklearn-compatible string or a compatible
         sklearn scorer.
 
         """
         pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def datasets(self):
         """Property that define the list of compatible datasets"""
         pass
 
     @abstractmethod
     def is_valid(self, dataset):
         """Verify the dataset is compatible with the paradigm.
@@ -47,28 +50,32 @@
             The dataset to verify.
         """
         pass
 
     def prepare_process(self, dataset):
         """Prepare processing of raw files
 
-        This function allows to set parameter of the paradigm class prior to
-        the preprocessing (process_raw). Does nothing by default and could be
-        overloaded if needed.
-
-        Parameters
-        ----------
-
-        dataset : dataset instance
-            The dataset corresponding to the raw file. mainly use to access
-            dataset specific information.
+                This function allows to set parameter of the paradigm class prior to
+                the preprocessing (process_raw). Does nothing by default and could be
+                overloaded if needed.
+
+                Parameters
+                ----------
+
+                dataset : dataset instance
+                    The dataset corresponding to the raw file. mainly use to access
+                    dataset specific i
+        nformation.
         """
-        pass
+        if dataset is not None:
+            pass
 
-    def process_raw(self, raw, dataset, return_epochs=False):  # noqa: C901
+    def process_raw(  # noqa: C901
+        self, raw, dataset, return_epochs=False, return_raws=False
+    ):
         """
         Process one raw data file.
 
         This function apply the preprocessing and eventual epoching on the
         individual run, and return the data, labels and a dataframe with
         metadata.
 
@@ -81,41 +88,49 @@
             the raw EEG data.
         dataset : dataset instance
             The dataset corresponding to the raw file. mainly use to access
             dataset specific information.
         return_epochs: boolean
             This flag specifies whether to return only the data array or the
             complete processed mne.Epochs
+        return_raws: boolean
+            To return raw files and events, to ensure compatibility with braindecode.
+            Mutually exclusive with return_epochs
 
         returns
         -------
         X : Union[np.ndarray, mne.Epochs]
             the data that will be used as features for the model
             Note: if return_epochs=True,  this is mne.Epochs
             if return_epochs=False, this is np.ndarray
         labels: np.ndarray
             the labels for training / evaluating the model
         metadata: pd.DataFrame
             A dataframe containing the metadata
 
         """
+
+        if return_epochs and return_raws:
+            message = "Select only return_epochs or return_raws, not both"
+            raise ValueError(message)
+
         # get events id
         event_id = self.used_events(dataset)
 
         # find the events, first check stim_channels then annotations
         stim_channels = mne.utils._get_stim_channel(None, raw.info, raise_error=False)
         if len(stim_channels) > 0:
             events = mne.find_events(raw, shortest_event=0, verbose=False)
         else:
             try:
                 events, _ = mne.events_from_annotations(
                     raw, event_id=event_id, verbose=False
                 )
             except ValueError:
-                log.warning("No matching annotations in {}".format(raw.filenames))
+                log.warning(f"No matching annotations in {raw.filenames}")
                 return
 
         # picks channels
         if self.channels is None:
             picks = mne.pick_types(raw.info, eeg=True, stim=False)
         else:
             picks = mne.pick_channels(
@@ -125,80 +140,89 @@
         # pick events, based on event_id
         try:
             events = mne.pick_events(events, include=list(event_id.values()))
         except RuntimeError:
             # skip raw if no event found
             return
 
-        # get interval
-        tmin = self.tmin + dataset.interval[0]
-        if self.tmax is None:
-            tmax = dataset.interval[1]
+        if return_raws:
+            raw = raw.pick(picks)
         else:
-            tmax = self.tmax + dataset.interval[0]
+            # get interval
+            tmin = self.tmin + dataset.interval[0]
+            if self.tmax is None:
+                tmax = dataset.interval[1]
+            else:
+                tmax = self.tmax + dataset.interval[0]
 
-        X = []
-        for bandpass in self.filters:
-            fmin, fmax = bandpass
-            # filter data
-            raw_f = raw.copy().filter(
-                fmin, fmax, method="iir", picks=picks, verbose=False
-            )
-            # epoch data
-            baseline = self.baseline
-            if baseline is not None:
-                baseline = (
-                    self.baseline[0] + dataset.interval[0],
-                    self.baseline[1] + dataset.interval[0],
+            X = []
+            for bandpass in self.filters:
+                fmin, fmax = bandpass
+                # filter data
+                raw_f = raw.copy().filter(
+                    fmin, fmax, method="iir", picks=picks, verbose=False
                 )
-                bmin = baseline[0] if baseline[0] < tmin else tmin
-                bmax = baseline[1] if baseline[1] > tmax else tmax
-            else:
-                bmin = tmin
-                bmax = tmax
-            epochs = mne.Epochs(
-                raw_f,
-                events,
-                event_id=event_id,
-                tmin=bmin,
-                tmax=bmax,
-                proj=False,
-                baseline=baseline,
-                preload=True,
-                verbose=False,
-                picks=picks,
-                event_repeated="drop",
-                on_missing="ignore",
-            )
-            if bmin < tmin or bmax > tmax:
-                epochs.crop(tmin=tmin, tmax=tmax)
-            if self.resample is not None:
-                epochs = epochs.resample(self.resample)
-            # rescale to work with uV
-            if return_epochs:
-                X.append(epochs)
-            else:
-                X.append(dataset.unit_factor * epochs.get_data())
+                # epoch data
+                baseline = self.baseline
+                if baseline is not None:
+                    baseline = (
+                        self.baseline[0] + dataset.interval[0],
+                        self.baseline[1] + dataset.interval[0],
+                    )
+                    bmin = baseline[0] if baseline[0] < tmin else tmin
+                    bmax = baseline[1] if baseline[1] > tmax else tmax
+                else:
+                    bmin = tmin
+                    bmax = tmax
+                epochs = mne.Epochs(
+                    raw_f,
+                    events,
+                    event_id=event_id,
+                    tmin=bmin,
+                    tmax=bmax,
+                    proj=False,
+                    baseline=baseline,
+                    preload=True,
+                    verbose=False,
+                    picks=picks,
+                    event_repeated="drop",
+                    on_missing="ignore",
+                )
+                if bmin < tmin or bmax > tmax:
+                    epochs.crop(tmin=tmin, tmax=tmax)
+                if self.resample is not None:
+                    epochs = epochs.resample(self.resample)
+                # rescale to work with uV
+                if return_epochs:
+                    X.append(epochs)
+                else:
+                    X.append(dataset.unit_factor * epochs.get_data())
+
+            # overwrite events in case epochs have been dropped:
+            # (assuming all filters produce the same number of epochs...)
+            events = epochs.events
 
         inv_events = {k: v for v, k in event_id.items()}
-        labels = np.array([inv_events[e] for e in epochs.events[:, -1]])
+        labels = np.array([inv_events[e] for e in events[:, -1]])
 
         if return_epochs:
             X = mne.concatenate_epochs(X)
+        elif return_raws:
+            X = raw
         elif len(self.filters) == 1:
             # if only one band, return a 3D array
             X = X[0]
         else:
             # otherwise return a 4D
             X = np.array(X).transpose((1, 2, 3, 0))
 
         metadata = pd.DataFrame(index=range(len(labels)))
         return X, labels, metadata
 
-    def get_data(self, dataset, subjects=None, return_epochs=False):
+    def get_data(self, dataset, subjects=None, return_epochs=False, return_raws=False):
         """
         Return the data for a list of subject.
 
         return the data, labels and a dataframe with metadata. the dataframe
         will contain at least the following columns
 
         - subject : the subject indice
@@ -210,55 +234,71 @@
         dataset:
             A dataset instance.
         subjects: List of int
             List of subject number
         return_epochs: boolean
             This flag specifies whether to return only the data array or the
             complete processed mne.Epochs
+        return_raws: boolean
+            To return raw files and events, to ensure compatibility with braindecode.
+            Mutually exclusive with return_epochs
 
         returns
         -------
         X : Union[np.ndarray, mne.Epochs]
             the data that will be used as features for the model
             Note: if return_epochs=True,  this is mne.Epochs
             if return_epochs=False, this is np.ndarray
         labels: np.ndarray
             the labels for training / evaluating the model
         metadata: pd.DataFrame
             A dataframe containing the metadata.
         """
 
         if not self.is_valid(dataset):
-            message = "Dataset {} is not valid for paradigm".format(dataset.code)
+            message = f"Dataset {dataset.code} is not valid for paradigm"
             raise AssertionError(message)
 
+        if return_epochs and return_raws:
+            message = "Select only return_epochs or return_raws, not both"
+            raise ValueError(message)
+
         data = dataset.get_data(subjects)
         self.prepare_process(dataset)
 
-        X = [] if return_epochs else np.array([])
+        X = [] if (return_epochs or return_raws) else np.array([])
         labels = []
         metadata = []
         for subject, sessions in data.items():
             for session, runs in sessions.items():
                 for run, raw in runs.items():
-                    proc = self.process_raw(raw, dataset, return_epochs=return_epochs)
+                    proc = self.process_raw(raw, dataset, return_epochs, return_raws)
 
                     if proc is None:
                         # this mean the run did not contain any selected event
                         # go to next
                         continue
 
                     x, lbs, met = proc
                     met["subject"] = subject
                     met["session"] = session
                     met["run"] = run
                     metadata.append(met)
 
                     # grow X and labels in a memory efficient way. can be slow
                     if return_epochs:
+                        x.metadata = (
+                            met.copy()
+                            if len(self.filters) == 1
+                            else pd.concat(
+                                [met.copy()] * len(self.filters), ignore_index=True
+                            )
+                        )
+                        X.append(x)
+                    elif return_raws:
                         X.append(x)
                     else:
                         X = np.append(X, x, axis=0) if len(X) else x
                     labels = np.append(labels, lbs, axis=0)
 
         metadata = pd.concat(metadata, ignore_index=True)
         if return_epochs:
```

### Comparing `moabb-0.4.6/moabb/paradigms/motor_imagery.py` & `moabb-0.5.0/moabb/paradigms/motor_imagery.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     events: List of str | None (default None)
         event to use for epoching. If None, default to all events defined in
         the dataset.
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -106,15 +106,15 @@
 
     @property
     def scoring(self):
         return "accuracy"
 
 
 class SinglePass(BaseMotorImagery):
-    """Single Bandpass filter motot Imagery.
+    """Single Bandpass filter motor Imagery.
 
     Motor imagery paradigm with only one bandpass filter (default 8 to 32 Hz)
 
     Parameters
     ----------
     fmin: float (default 8)
         cutoff frequency (Hz) for the high pass filter
@@ -125,20 +125,20 @@
     events: List of str | None (default None)
         event to use for epoching. If None, default to all events defined in
         the dataset.
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -318,20 +318,20 @@
 
     fmax: float (default 32)
         cutoff frequency (Hz) for the low pass filter
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -342,43 +342,45 @@
         list of channel to select. If None, use all EEG channels available in
         the dataset.
 
     resample: float | None (default None)
         If not None, resample the eeg data with the sampling rate provided.
     """
 
-    def __init__(self, n_classes=2, **kwargs):
+    def __init__(self, n_classes=None, **kwargs):
         super().__init__(**kwargs)
         self.n_classes = n_classes
 
         if self.events is None:
             log.warning("Choosing from all possible events")
-        else:
+        elif self.n_classes is not None:
             assert n_classes <= len(self.events), "More classes than events specified"
 
     def is_valid(self, dataset):
         ret = True
         if not dataset.paradigm == "imagery":
             ret = False
-        if self.events is None:
+        elif self.n_classes is None and self.events is None:
+            pass
+        elif self.events is None:
             if not len(dataset.event_id) >= self.n_classes:
                 ret = False
         else:
             overlap = len(set(self.events) & set(dataset.event_id.keys()))
-            if not overlap >= self.n_classes:
+            if self.n_classes is not None and not overlap >= self.n_classes:
                 ret = False
         return ret
 
     def used_events(self, dataset):
         out = {}
         if self.events is None:
             for k, v in dataset.event_id.items():
                 out[k] = v
-                if len(out) == self.n_classes:
-                    break
+            if self.n_classes is None:
+                self.n_classes = len(out)
         else:
             for event in self.events:
                 if event in dataset.event_id.keys():
                     out[event] = dataset.event_id[event]
                 if len(out) == self.n_classes:
                     break
         if len(out) < self.n_classes:
@@ -413,7 +415,10 @@
 
 class FakeImageryParadigm(LeftRightImagery):
     """Fake Imagery for left hand/right hand classification."""
 
     @property
     def datasets(self):
         return [FakeDataset(["left_hand", "right_hand"], paradigm="imagery")]
+
+    def is_valid(self, dataset):
+        return True
```

### Comparing `moabb-0.4.6/moabb/paradigms/p300.py` & `moabb-0.5.0/moabb/paradigms/p300.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     events: List of str | None (default None)
         event to use for epoching. If None, default to all events defined in
         the dataset.
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -94,101 +94,158 @@
         # we should verify list of channels, somehow
         return ret
 
     @abc.abstractmethod
     def used_events(self, dataset):
         pass
 
-    def process_raw(self, raw, dataset, return_epochs=False):  # noqa: C901
+    def process_raw(  # noqa: C901
+        self, raw, dataset, return_epochs=False, return_raws=False
+    ):
+        """
+        Process one raw data file.
+
+        This function apply the preprocessing and eventual epoching on the
+        individual run, and return the data, labels and a dataframe with
+        metadata.
+
+        metadata is a dataframe with as many row as the length of the data
+        and labels.
+
+        Parameters
+        ----------
+        raw: mne.Raw instance
+            the raw EEG data.
+        dataset : dataset instance
+            The dataset corresponding to the raw file. mainly use to access
+            dataset specific information.
+        return_epochs: boolean
+            This flag specifies whether to return only the data array or the
+            complete processed mne.Epochs
+        return_raws: boolean
+            To return raw files and events, to ensure compatibility with braindecode.
+            Mutually exclusive with return_epochs
+
+        returns
+        -------
+        X : Union[np.ndarray, mne.Epochs]
+            the data that will be used as features for the model
+            Note: if return_epochs=True,  this is mne.Epochs
+            if return_epochs=False, this is np.ndarray
+        labels: np.ndarray
+            the labels for training / evaluating the model
+        metadata: pd.DataFrame
+            A dataframe containing the metadata
+
+        """
+
+        if return_epochs and return_raws:
+            message = "Select only return_epochs or return_raws, not both"
+            raise ValueError(message)
+
+        # get events id
+        event_id = self.used_events(dataset)
+
         # find the events, first check stim_channels then annotations
         stim_channels = mne.utils._get_stim_channel(None, raw.info, raise_error=False)
         if len(stim_channels) > 0:
             events = mne.find_events(raw, shortest_event=0, verbose=False)
         else:
-            events, _ = mne.events_from_annotations(raw, verbose=False)
+            try:
+                events, _ = mne.events_from_annotations(
+                    raw, event_id=event_id, verbose=False
+                )
+            except ValueError:
+                log.warning(f"No matching annotations in {raw.filenames}")
+                return
 
         # picks channels
-        channels = () if self.channels is None else self.channels
-        picks = mne.pick_types(raw.info, eeg=True, stim=False, include=channels)
         if self.channels is None:
             picks = mne.pick_types(raw.info, eeg=True, stim=False)
         else:
             picks = mne.pick_channels(
-                raw.info["ch_names"], include=channels, ordered=True
+                raw.info["ch_names"], include=self.channels, ordered=True
             )
 
-        # get event id
-        event_id = self.used_events(dataset)
-
         # pick events, based on event_id
         try:
             if type(event_id["Target"]) is list and type(event_id["NonTarget"]) == list:
                 event_id_new = dict(Target=1, NonTarget=0)
                 events = mne.merge_events(events, event_id["Target"], 1)
                 events = mne.merge_events(events, event_id["NonTarget"], 0)
                 event_id = event_id_new
             events = mne.pick_events(events, include=list(event_id.values()))
         except RuntimeError:
             # skip raw if no event found
             return
 
-        # get interval
-        tmin = self.tmin + dataset.interval[0]
-        if self.tmax is None:
-            tmax = dataset.interval[1]
+        if return_raws:
+            raw = raw.pick(picks)
         else:
-            tmax = self.tmax + dataset.interval[0]
+            # get interval
+            tmin = self.tmin + dataset.interval[0]
+            if self.tmax is None:
+                tmax = dataset.interval[1]
+            else:
+                tmax = self.tmax + dataset.interval[0]
 
-        X = []
-        for bandpass in self.filters:
-            fmin, fmax = bandpass
-            # filter data
-            raw_f = raw.copy().filter(
-                fmin, fmax, method="iir", picks=picks, verbose=False
-            )
-            # epoch data
-            baseline = self.baseline
-            if baseline is not None:
-                baseline = (
-                    self.baseline[0] + dataset.interval[0],
-                    self.baseline[1] + dataset.interval[0],
+            X = []
+            for bandpass in self.filters:
+                fmin, fmax = bandpass
+                # filter data
+                raw_f = raw.copy().filter(
+                    fmin, fmax, method="iir", picks=picks, verbose=False
                 )
-                bmin = baseline[0] if baseline[0] < tmin else tmin
-                bmax = baseline[1] if baseline[1] > tmax else tmax
-            else:
-                bmin = tmin
-                bmax = tmax
-            epochs = mne.Epochs(
-                raw_f,
-                events,
-                event_id=event_id,
-                tmin=bmin,
-                tmax=bmax,
-                proj=False,
-                baseline=baseline,
-                preload=True,
-                verbose=False,
-                picks=picks,
-                on_missing="ignore",
-            )
-            if bmin < tmin or bmax > tmax:
-                epochs.crop(tmin=tmin, tmax=tmax)
-            if self.resample is not None:
-                epochs = epochs.resample(self.resample)
-            # rescale to work with uV
-            if return_epochs:
-                X.append(epochs)
-            else:
-                X.append(dataset.unit_factor * epochs.get_data())
+                # epoch data
+                baseline = self.baseline
+                if baseline is not None:
+                    baseline = (
+                        self.baseline[0] + dataset.interval[0],
+                        self.baseline[1] + dataset.interval[0],
+                    )
+                    bmin = baseline[0] if baseline[0] < tmin else tmin
+                    bmax = baseline[1] if baseline[1] > tmax else tmax
+                else:
+                    bmin = tmin
+                    bmax = tmax
+                epochs = mne.Epochs(
+                    raw_f,
+                    events,
+                    event_id=event_id,
+                    tmin=bmin,
+                    tmax=bmax,
+                    proj=False,
+                    baseline=baseline,
+                    preload=True,
+                    verbose=False,
+                    picks=picks,
+                    event_repeated="drop",
+                    on_missing="ignore",
+                )
+                if bmin < tmin or bmax > tmax:
+                    epochs.crop(tmin=tmin, tmax=tmax)
+                if self.resample is not None:
+                    epochs = epochs.resample(self.resample)
+                # rescale to work with uV
+                if return_epochs:
+                    X.append(epochs)
+                else:
+                    X.append(dataset.unit_factor * epochs.get_data())
+
+            # overwrite events in case epochs have been dropped:
+            # (assuming all filters produce the same number of epochs...)
+            events = epochs.events
 
         inv_events = {k: v for v, k in event_id.items()}
-        labels = np.array([inv_events[e] for e in epochs.events[:, -1]])
+        labels = np.array([inv_events[e] for e in events[:, -1]])
 
         if return_epochs:
             X = mne.concatenate_epochs(X)
+        elif return_raws:
+            X = raw
         elif len(self.filters) == 1:
             # if only one band, return a 3D array
             X = X[0]
         else:
             # otherwise return a 4D
             X = np.array(X).transpose((1, 2, 3, 0))
 
@@ -226,20 +283,20 @@
     events: List of str | None (default None)
         event to use for epoching. If None, default to all events defined in
         the dataset.
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -283,7 +340,10 @@
 
 class FakeP300Paradigm(P300):
     """Fake P300 for Target/NonTarget classification."""
 
     @property
     def datasets(self):
         return [FakeDataset(["Target", "NonTarget"], paradigm="p300")]
+
+    def is_valid(self, dataset):
+        return True
```

### Comparing `moabb-0.4.6/moabb/paradigms/ssvep.py` & `moabb-0.5.0/moabb/paradigms/ssvep.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 
     n_classes: int or None (default None)
         Number of classes each dataset must have. All dataset classes if None.
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -173,20 +173,20 @@
 
     n_classes: int or None (default None)
         Number of classes each dataset must have. All dataset classes if None
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -226,20 +226,20 @@
 
     n_classes: int or None (default 2)
         Number of classes each dataset must have. All dataset classes if None
 
     tmin: float (default 0.0)
         Start time (in second) of the epoch, relative to the dataset specific
         task interval e.g. tmin = 1 would mean the epoch will start 1 second
-        after the begining of the task as defined by the dataset.
+        after the beginning of the task as defined by the dataset.
 
     tmax: float | None, (default None)
-        End time (in second) of the epoch, relative to the begining of the
+        End time (in second) of the epoch, relative to the beginning of the
         dataset specific task interval. tmax = 5 would mean the epoch will end
-        5 second after the begining of the task as defined in the dataset. If
+        5 second after the beginning of the task as defined in the dataset. If
         None, use the dataset value.
 
     baseline: None | tuple of length 2
             The time interval to consider as “baseline” when applying baseline
             correction. If None, do not apply baseline correction.
             If a tuple (a, b), the interval is between a and b (in seconds),
             including the endpoints.
@@ -260,7 +260,10 @@
 
 class FakeSSVEPParadigm(BaseSSVEP):
     """Fake SSVEP classification."""
 
     @property
     def datasets(self):
         return [FakeDataset(event_list=["13", "15"], paradigm="ssvep")]
+
+    def is_valid(self, dataset):
+        return True
```

### Comparing `moabb-0.4.6/moabb/pipelines/classification.py` & `moabb-0.5.0/moabb/pipelines/classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import scipy.linalg as linalg
+from joblib import Parallel, delayed
 from pyriemann.estimation import Covariances
+from pyriemann.utils.covariance import covariances
 from pyriemann.utils.mean import mean_covariance
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.cross_decomposition import CCA
 from sklearn.utils.validation import check_is_fitted
 
 from .utils import filterbank
 
@@ -13,14 +15,29 @@
     """Classifier based on Canonical Correlation Analysis for SSVEP
 
     A CCA is computed from the set of training signals and some pure
     sinusoids to act as reference.
     Classification is made by taking the frequency with the max correlation,
     as proposed in [1]_.
 
+    Parameters
+    ----------
+    interval : list of lenght 2
+        List of form [tmin, tmax]. With tmin and tmax as defined in the SSVEP
+        paradigm :meth:`moabb.paradigms.SSVEP`
+
+    freqs : dict with n_classes keys
+        Frequencies corresponding to the SSVEP stimulation frequencies.
+        They are used to identify SSVEP classes presents in the data.
+
+    n_harmonics: int
+        Number of stimulation frequency's harmonics to be used in the genration
+        of the CCA reference signal.
+
+
     References
     ----------
 
     .. [1] Bin, G., Gao, X., Yan, Z., Hong, B., & Gao, S. (2009). An online
            multi-channel SSVEP-based brain-computer interface using a
            canonical correlation analysis method. Journal of neural
            engineering, 6(4), 046002.
@@ -64,15 +81,15 @@
         y = []
         for x in X:
             corr_f = {}
             for f in self.freqs:
                 if f.replace(".", "", 1).isnumeric():
                     S_x, S_y = self.cca.fit_transform(x.T, self.Yf[f].T)
                     corr_f[f] = np.corrcoef(S_x.T, S_y.T)[0, 1]
-            y.append(self.one_hot[max(corr_f, key=lambda k: corr_f[k])])
+            y.append(self.one_hot[max(corr_f, key=corr_f.get)])
         return y
 
     def predict_proba(self, X):
         """Probabilty could be computed from the correlation coefficient"""
         P = np.zeros(shape=(len(X), len(self.freqs)))
         for i, x in enumerate(X):
             for j, f in enumerate(self.freqs):
@@ -154,15 +171,18 @@
           "Enhancing detection of SSVEPs for a high-speed brain speller using
           task-related component analysis",
           IEEE Trans. Biomed. Eng, 65(1):104-112, 2018.
 
     Code based on the Matlab implementation from authors of [1]_
     (https://github.com/mnakanishi/TRCA-SSVEP).
 
-        .. versionadded:: 0.4.4
+
+    Notes
+    -----
+    .. versionadded:: 0.4.4
     """
 
     def __init__(
         self,
         interval,
         freqs,
         n_fbands=5,
@@ -507,7 +527,140 @@
             # Fusion for the filterbank analysis
             rho = np.dot(normalized_coefs, corr_array)
 
             rho /= sum(rho)
             y_pred[trial_n] = rho
 
         return y_pred
+
+
+def _whitening(X):
+    """utility function to whiten EEG signal
+
+    Parameters
+    ----------
+    X: ndarray of shape (n_channels, n_samples)
+    """
+    n_channels, n_samples = X.shape
+    X_white = X.copy()
+
+    X_white = X_white - np.mean(X_white, axis=1, keepdims=True)
+    C = covariances(X_white.reshape((1, n_channels, n_samples)), estimator="sch")[
+        0
+    ]  # Shrunk covariance matrix
+    eig_val, eig_vec = linalg.eigh(C)
+    V = (np.abs(eig_val) ** -0.5)[:, np.newaxis] * eig_vec.T
+    X_white = V @ X_white
+    return X_white
+
+
+class SSVEP_MsetCCA(BaseEstimator, ClassifierMixin):
+    """Classifier based on MsetCCA for SSVEP
+
+     The MsetCCA method learns multiple linear transforms to extract
+     SSVEP common features from multiple sets of EEG data. These are then used
+     to compute the reference signal used in CCA [1]_.
+
+    Parameters
+    ----------
+    freqs : dict with n_classes keys
+        Frequencies corresponding to the SSVEP stimulation frequencies.
+        They are used to identify SSVEP classes presents in the data.
+
+    n_filters: int
+        Number of multisets spatial filters used per sample data.
+        It corresponds to the number of eigen vectors taken the solution of the
+        MAXVAR objective function as formulated in Eq.5 in [1]_.
+
+
+    References
+    ----------
+
+    .. [1] Zhang, Y.U., Zhou, G., Jin, J., Wang, X. and Cichocki, A. (2014). Frequency
+           recognition in SSVEP-based BCI using multiset canonical correlation analysis.
+           International journal of neural systems, 24(04), p.1450013.
+           https://doi.org/10.1142/S0129065714500130
+
+    Notes
+    -----
+    .. versionadded:: 0.5.0
+    """
+
+    def __init__(self, freqs, n_filters=1, n_jobs=1):
+        self.n_jobs = n_jobs
+        self.n_filters = n_filters
+        self.freqs = freqs
+        self.cca = CCA(n_components=1)
+
+    def fit(self, X, y, sample_weight=None):
+        """
+        Compute the optimized reference signal at each stimulus frequency
+        """
+        self.classes_ = np.unique(y)
+        self.one_hot = {}
+        for i, k in enumerate(self.classes_):
+            self.one_hot[k] = i
+        n_trials, n_channels, n_times = X.shape
+
+        # Whiten signal in parallel
+        if self.n_jobs == 1:
+            X_white = [_whitening(X_i) for X_i in X]
+        else:
+            X_white = Parallel(n_jobs=self.n_jobs)(delayed(_whitening)(X_i) for X_i in X)
+        X_white = np.stack(X_white, axis=0)
+
+        Y = X_white.transpose(2, 0, 1).reshape(-1, n_times)
+        # R = np.cov(Y)
+        # or more similar to the article:
+        R = Y @ Y.T
+        # S = np.diag(np.diag(R)) # This does not match the definition in the article
+        # S exactly as defined in the article
+        mask = np.kron(
+            np.eye(n_trials), np.ones((n_channels, n_channels))
+        )  # block diagonal mask
+        S = R * mask
+
+        # Get W
+        _, tempW = linalg.eigh(
+            R - S, S, subset_by_index=[R.shape[1] - self.n_filters, R.shape[1] - 1]
+        )
+        W = np.reshape(tempW, (n_trials, n_channels, self.n_filters))
+
+        # Normalise W
+        W = W / np.linalg.norm(W, axis=0, keepdims=True)
+
+        Z = W.transpose((0, 2, 1)) @ X_white
+
+        # Get Ym
+        self.Ym = dict()
+        for m_class in self.classes_:
+            self.Ym[m_class] = Z[y == m_class].transpose(2, 0, 1).reshape(-1, n_times)
+
+        return self
+
+    def predict(self, X):
+        """Predict is made by taking the maximum correlation coefficient"""
+
+        # Check is fit had been called
+        check_is_fitted(self)
+
+        y = []
+        for x in X:
+            corr_f = {}
+            for f in self.classes_:
+                S_x, S_y = self.cca.fit_transform(x.T, self.Ym[f].T)
+                corr_f[f] = np.corrcoef(S_x.T, S_y.T)[0, 1]
+            y.append(self.one_hot[max(corr_f, key=corr_f.get)])
+        return y
+
+    def predict_proba(self, X):
+        """Probabilty could be computed from the correlation coefficient"""
+
+        # Check is fit had been called
+        check_is_fitted(self)
+
+        P = np.zeros(shape=(len(X), len(self.classes_)))
+        for i, x in enumerate(X):
+            for j, f in enumerate(self.classes_):
+                S_x, S_y = self.cca.fit_transform(x.T, self.Ym[f].T)
+                P[i, j] = np.corrcoef(S_x.T, S_y.T)[0, 1]
+        return P / np.resize(P.sum(axis=1), P.T.shape).T
```

### Comparing `moabb-0.4.6/moabb/pipelines/csp.py` & `moabb-0.5.0/moabb/pipelines/csp.py`

 * *Files identical despite different names*

### Comparing `moabb-0.4.6/moabb/tests/download.py` & `moabb-0.5.0/moabb/tests/download.py`

 * *Files identical despite different names*

### Comparing `moabb-0.4.6/moabb/tests/evaluations.py` & `moabb-0.5.0/moabb/tests/evaluations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 import os
 import os.path as osp
 import platform
 import unittest
 import warnings
 from collections import OrderedDict
 
+import joblib
 import numpy as np
 import sklearn.base
 from pyriemann.estimation import Covariances
 from pyriemann.spatialfilters import CSP
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA
+from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import make_pipeline
 
 from moabb.analysis.results import get_string_rep
 from moabb.datasets.fake import FakeDataset
 from moabb.evaluations import evaluations as ev
 from moabb.paradigms.motor_imagery import FakeImageryParadigm
 
 
+try:
+    from codecarbon import EmissionsTracker  # noqa
+
+    _carbonfootprint = True
+except ImportError:
+    _carbonfootprint = False
+
+
 pipelines = OrderedDict()
 pipelines["C"] = make_pipeline(Covariances("oas"), CSP(8), LDA())
 dataset = FakeDataset(["left_hand", "right_hand"], n_subjects=2)
 if not osp.isdir(osp.join(osp.expanduser("~"), "mne_data")):
     os.makedirs(osp.join(osp.expanduser("~"), "mne_data"))
 
 
@@ -38,34 +48,104 @@
     stuff on. To test the scoring and train/test we need to also have data and
     run it. Putting this on the future docket...
 
     """
 
     def setUp(self):
         self.eval = ev.WithinSessionEvaluation(
-            paradigm=FakeImageryParadigm(), datasets=[dataset]
+            paradigm=FakeImageryParadigm(),
+            datasets=[dataset],
+            hdf5_path="res_test",
         )
 
     def test_mne_labels(self):
         kwargs = dict(paradigm=FakeImageryParadigm(), datasets=[dataset])
         epochs = dict(return_epochs=False, mne_labels=True)
         self.assertRaises(ValueError, ev.WithinSessionEvaluation, **epochs, **kwargs)
 
     def tearDown(self):
         path = self.eval.results.filepath
         if os.path.isfile(path):
             os.remove(path)
 
     def test_eval_results(self):
-        results = [r for r in self.eval.evaluate(dataset, pipelines)]
+        results = [r for r in self.eval.evaluate(dataset, pipelines, param_grid=None)]
 
-        # We should get 4 results, 2 session 2 subject
+        # We should get 4 results, 2 sessions 2 subjects
         self.assertEqual(len(results), 4)
-        # We should have 8 columns in the results data frame
-        self.assertEqual(len(results[0].keys()), 8)
+        # We should have 9 columns in the results data frame
+        self.assertEqual(len(results[0].keys()), 9 if _carbonfootprint else 8)
+
+    def test_eval_grid_search(self):
+        gs_param = {
+            "Within": os.path.join(
+                "res_test",
+                "GridSearch_WithinSession",
+                str(dataset.code),
+                "subject1",
+                "session_0",
+                "C",
+                "Grid_Search_WithinSession.pkl",
+            ),
+            "CrossSess": os.path.join(
+                "res_test",
+                "GridSearch_CrossSession",
+                str(dataset.code),
+                "1",
+                "C",
+                "Grid_Search_CrossSession.pkl",
+            ),
+            "CrossSubj": os.path.join(
+                "res_test",
+                "GridSearch_CrossSubject",
+                str(dataset.code),
+                "C",
+                "Grid_Search_CrossSubject.pkl",
+            ),
+        }
+        if isinstance(self.eval, ev.WithinSessionEvaluation):
+            respath = gs_param["Within"]
+        elif isinstance(self.eval, ev.CrossSessionEvaluation):
+            respath = gs_param["CrossSess"]
+        elif isinstance(self.eval, ev.CrossSubjectEvaluation):
+            respath = gs_param["CrossSubj"]
+
+        # Test grid search
+        param_grid = {"C": {"csp__metric": ["euclid", "riemann"]}}
+        results = [
+            r for r in self.eval.evaluate(dataset, pipelines, param_grid=param_grid)
+        ]
+
+        # We should get 4 results, 2 sessions 2 subjects
+        self.assertEqual(len(results), 4)
+        # We should have 9 columns in the results data frame
+        self.assertEqual(len(results[0].keys()), 9 if _carbonfootprint else 8)
+        # We should check for selected parameters with joblib
+        self.assertTrue(os.path.isfile(respath))
+        res = joblib.load(respath)
+        self.assertIsInstance(res, GridSearchCV)
+
+    def test_lambda_warning(self):
+        def explicit_kernel(x):
+            return x**3
+
+        c1 = DummyClassifier(kernel=lambda x: x**2)
+        c2 = DummyClassifier(kernel=lambda x: 5 * x)
+
+        c3 = DummyClassifier(kernel=explicit_kernel)
+
+        self.assertFalse(repr(c1) == repr(c2))
+        if platform.system() != "Windows":
+            with self.assertWarns(RuntimeWarning):
+                self.assertTrue(get_string_rep(c1) == get_string_rep(c2))
+
+        # I do not know an elegant way to check for no warnings
+        with warnings.catch_warnings(record=True) as w:
+            get_string_rep(c3)
+            self.assertTrue(len(w) == 0)
 
 
 class Test_WithinSessLearningCurve(unittest.TestCase):
     """
     Some tests for the learning curve evaluation.
 
     TODO if we ever extend dataset metadata, e.g. including y for example, we could get rid of a
@@ -76,15 +156,17 @@
     def test_correct_results_integrity(self):
         learning_curve_eval = ev.WithinSessionEvaluation(
             paradigm=FakeImageryParadigm(),
             datasets=[dataset],
             data_size={"policy": "ratio", "value": np.array([0.2, 0.5])},
             n_perms=np.array([2, 2]),
         )
-        results = [r for r in learning_curve_eval.evaluate(dataset, pipelines)]
+        results = [
+            r for r in learning_curve_eval.evaluate(dataset, pipelines, param_grid=None)
+        ]
         keys = results[0].keys()
         self.assertEqual(len(keys), 10)  # 8 + 2 new for learning curve
         self.assertTrue("permutation" in keys)
         self.assertTrue("data_size" in keys)
 
     def test_all_policies_work(self):
         kwargs = dict(paradigm=FakeImageryParadigm(), datasets=[dataset], n_perms=[2, 2])
@@ -100,29 +182,31 @@
             ev.WithinSessionEvaluation,
             **dict(data_size={"policy": "does_not_exist", "value": [0.2, 0.5]}, **kwargs),
         )
 
     def test_data_sanity(self):
         # need this helper to iterate over the generator
         def run_evaluation(eval, dataset, pipelines):
-            list(eval.evaluate(dataset, pipelines))
+            list(eval.evaluate(dataset, pipelines, param_grid=None))
 
         # E.g. if number of samples too high -> expect error
         kwargs = dict(paradigm=FakeImageryParadigm(), datasets=[dataset], n_perms=[2, 2])
         should_work = ev.WithinSessionEvaluation(
             data_size={"policy": "per_class", "value": [5, 10]}, **kwargs
         )
         too_many_samples = ev.WithinSessionEvaluation(
             data_size={"policy": "per_class", "value": [5, 100000]}, **kwargs
         )
         # This one should run
         run_evaluation(should_work, dataset, pipelines)
         self.assertRaises(
             ValueError, run_evaluation, too_many_samples, dataset, pipelines
         )
+
+    def test_eval_grid_search(self):
         pass
 
     def test_datasize_parameters(self):
         # Fail if not values are not correctly ordered
         kwargs = dict(paradigm=FakeImageryParadigm(), datasets=[dataset])
         decreasing_datasize = dict(
             data_size={"policy": "per_class", "value": [5, 4]}, n_perms=[2, 1], **kwargs
@@ -156,15 +240,17 @@
         self.assertRaises(ValueError, self.eval.process, pipelines)
         # TODO Add custom evaluation that actually returns additional info
 
 
 class Test_CrossSubj(Test_WithinSess):
     def setUp(self):
         self.eval = ev.CrossSubjectEvaluation(
-            paradigm=FakeImageryParadigm(), datasets=[dataset]
+            paradigm=FakeImageryParadigm(),
+            datasets=[dataset],
+            hdf5_path="res_test",
         )
 
     def test_compatible_dataset(self):
         # raise
         ds = FakeDataset(["left_hand", "right_hand"], n_subjects=1)
         self.assertFalse(self.eval.is_valid(dataset=ds))
 
@@ -172,47 +258,23 @@
         ds = FakeDataset(["left_hand", "right_hand"], n_subjects=2)
         self.assertTrue(self.eval.is_valid(dataset=ds))
 
 
 class Test_CrossSess(Test_WithinSess):
     def setUp(self):
         self.eval = ev.CrossSessionEvaluation(
-            paradigm=FakeImageryParadigm(), datasets=[dataset]
+            paradigm=FakeImageryParadigm(),
+            datasets=[dataset],
+            hdf5_path="res_test",
         )
 
     def test_compatible_dataset(self):
         ds = FakeDataset(["left_hand", "right_hand"], n_sessions=1)
         self.assertFalse(self.eval.is_valid(ds))
 
         # do not raise
         ds = FakeDataset(["left_hand", "right_hand"], n_sessions=2)
         self.assertTrue(self.eval.is_valid(dataset=ds))
 
 
-class Test_LambdaWarning(Test_WithinSess):
-    def setUp(self):
-        self.eval = ev.WithinSessionEvaluation(
-            paradigm=FakeImageryParadigm(), datasets=[dataset]
-        )
-
-    def test_lambda_warning(self):
-        def explicit_kernel(x):
-            return x ** 3
-
-        c1 = DummyClassifier(kernel=lambda x: x ** 2)
-        c2 = DummyClassifier(kernel=lambda x: 5 * x)
-
-        c3 = DummyClassifier(kernel=explicit_kernel)
-
-        self.assertFalse(repr(c1) == repr(c2))
-        if platform.system() != "Windows":
-            with self.assertWarns(RuntimeWarning):
-                self.assertTrue(get_string_rep(c1) == get_string_rep(c2))
-
-        # I do not know an elegant way to check for no warnings
-        with warnings.catch_warnings(record=True) as w:
-            get_string_rep(c3)
-            self.assertTrue(len(w) == 0)
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `moabb-0.4.6/moabb/tests/paradigms.py` & `moabb-0.5.0/moabb/tests/paradigms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import unittest
 
 import numpy as np
 from mne import BaseEpochs
+from mne.io import BaseRaw
 
 from moabb.datasets.fake import FakeDataset
 from moabb.paradigms import (
     P300,
     SSVEP,
     BaseMotorImagery,
     BaseP300,
@@ -46,14 +47,27 @@
         # we should have only one subject in the metadata
         self.assertEqual(np.unique(metadata.subject), 1)
         # we should have two sessions in the metadata
         self.assertEqual(len(np.unique(metadata.session)), 2)
         # should return epochs
         epochs, _, _ = paradigm.get_data(dataset, subjects=[1], return_epochs=True)
         self.assertIsInstance(epochs, BaseEpochs)
+        # should return raws
+        raws, _, _ = paradigm.get_data(dataset, subjects=[1], return_raws=True)
+        for raw in raws:
+            self.assertIsInstance(raw, BaseRaw)
+        # should raise error
+        self.assertRaises(
+            ValueError,
+            paradigm.get_data,
+            dataset,
+            subjects=[1],
+            return_epochs=True,
+            return_raws=True,
+        )
 
     def test_BaseImagery_channel_order(self):
         """test if paradigm return correct channel order, see issue #227"""
         datasetA = FakeDataset(paradigm="imagery", channels=["C3", "Cz", "C4"])
         datasetB = FakeDataset(paradigm="imagery", channels=["Cz", "C4", "C3"])
         paradigm = SimpleMotorImagery(channels=["C4", "C3", "Cz"])
 
@@ -92,14 +106,41 @@
 
     def test_BaseImagery_noevent(self):
         # Assert error if events from paradigm and dataset dont overlap
         paradigm = SimpleMotorImagery(events=["left_hand", "right_hand"])
         dataset = FakeDataset(paradigm="imagery")
         self.assertRaises(AssertionError, paradigm.get_data, dataset)
 
+    def test_BaseImagery_droppedevent(self):
+        dataset = FakeDataset(paradigm="imagery")
+        tmax = dataset.interval[1]
+        # with regular windows, all epochs should be valid:
+        paradigm1 = SimpleMotorImagery(tmax=tmax)
+        # with large windows, some epochs will have to be dropped:
+        paradigm2 = SimpleMotorImagery(tmax=10 * tmax)
+        # with epochs:
+        epochs1, labels1, metadata1 = paradigm1.get_data(dataset, return_epochs=True)
+        epochs2, labels2, metadata2 = paradigm2.get_data(dataset, return_epochs=True)
+        self.assertEqual(len(epochs1), len(labels1), len(metadata1))
+        self.assertEqual(len(epochs2), len(labels2), len(metadata2))
+        self.assertGreater(len(epochs1), len(epochs2))
+        # with np.array:
+        X1, labels1, metadata1 = paradigm1.get_data(dataset)
+        X2, labels2, metadata2 = paradigm2.get_data(dataset)
+        self.assertEqual(len(X1), len(labels1), len(metadata1))
+        self.assertEqual(len(X2), len(labels2), len(metadata2))
+        self.assertGreater(len(X1), len(X2))
+
+    def test_BaseImagery_epochsmetadata(self):
+        dataset = FakeDataset(paradigm="imagery")
+        paradigm = SimpleMotorImagery()
+        epochs, _, metadata = paradigm.get_data(dataset, return_epochs=True)
+        # does not work with multiple filters:
+        self.assertTrue(metadata.equals(epochs.metadata))
+
     def test_LeftRightImagery_paradigm(self):
         # with a good dataset
         paradigm = LeftRightImagery()
         dataset = FakeDataset(event_list=["left_hand", "right_hand"], paradigm="imagery")
         X, labels, metadata = paradigm.get_data(dataset, subjects=[1])
 
         self.assertEqual(len(np.unique(labels)), 2)
@@ -174,14 +215,27 @@
         # we should have only one subject in the metadata
         self.assertEqual(np.unique(metadata.subject), 1)
         # we should have two sessions in the metadata
         self.assertEqual(len(np.unique(metadata.session)), 2)
         # should return epochs
         epochs, _, _ = paradigm.get_data(dataset, subjects=[1], return_epochs=True)
         self.assertIsInstance(epochs, BaseEpochs)
+        # should return raws
+        raws, _, _ = paradigm.get_data(dataset, subjects=[1], return_raws=True)
+        for raw in raws:
+            self.assertIsInstance(raw, BaseRaw)
+        # should raise error
+        self.assertRaises(
+            ValueError,
+            paradigm.get_data,
+            dataset,
+            subjects=[1],
+            return_epochs=True,
+            return_raws=True,
+        )
 
     def test_BaseP300_channel_order(self):
         """test if paradigm return correct channel order, see issue #227"""
         datasetA = FakeDataset(
             paradigm="p300",
             channels=["C3", "Cz", "C4"],
             event_list=["Target", "NonTarget"],
@@ -222,14 +276,41 @@
         # add something on the event channel
         raw._data[-1] *= 10
         self.assertIsNone(paradigm.process_raw(raw, dataset))
         # zeros it out
         raw._data[-1] *= 0
         self.assertIsNone(paradigm.process_raw(raw, dataset))
 
+    def test_BaseP300_droppedevent(self):
+        dataset = FakeDataset(paradigm="p300", event_list=["Target", "NonTarget"])
+        tmax = dataset.interval[1]
+        # with regular windows, all epochs should be valid:
+        paradigm1 = SimpleP300(tmax=tmax)
+        # with large windows, some epochs will have to be dropped:
+        paradigm2 = SimpleP300(tmax=10 * tmax)
+        # with epochs:
+        epochs1, labels1, metadata1 = paradigm1.get_data(dataset, return_epochs=True)
+        epochs2, labels2, metadata2 = paradigm2.get_data(dataset, return_epochs=True)
+        self.assertEqual(len(epochs1), len(labels1), len(metadata1))
+        self.assertEqual(len(epochs2), len(labels2), len(metadata2))
+        self.assertGreater(len(epochs1), len(epochs2))
+        # with np.array:
+        X1, labels1, metadata1 = paradigm1.get_data(dataset)
+        X2, labels2, metadata2 = paradigm2.get_data(dataset)
+        self.assertEqual(len(X1), len(labels1), len(metadata1))
+        self.assertEqual(len(X2), len(labels2), len(metadata2))
+        self.assertGreater(len(X1), len(X2))
+
+    def test_BaseP300_epochsmetadata(self):
+        dataset = FakeDataset(paradigm="p300", event_list=["Target", "NonTarget"])
+        paradigm = SimpleP300()
+        epochs, _, metadata = paradigm.get_data(dataset, return_epochs=True)
+        # does not work with multiple filters:
+        self.assertTrue(metadata.equals(epochs.metadata))
+
     def test_P300_specifyevent(self):
         # we cant pass event to this class
         self.assertRaises(ValueError, P300, events=["a"])
 
     def test_P300_wrongevent(self):
         # does not accept dataset with bad event
         paradigm = P300()
@@ -267,14 +348,27 @@
         # Only one subject in the metadata
         self.assertEqual(np.unique(metadata.subject), 1)
         # we should have two sessions in the metadata, n_classes = 2 as default
         self.assertEqual(len(np.unique(metadata.session)), 2)
         # should return epochs
         epochs, _, _ = paradigm.get_data(dataset, subjects=[1], return_epochs=True)
         self.assertIsInstance(epochs, BaseEpochs)
+        # should return raws
+        raws, _, _ = paradigm.get_data(dataset, subjects=[1], return_raws=True)
+        for raw in raws:
+            self.assertIsInstance(raw, BaseRaw)
+        # should raise error
+        self.assertRaises(
+            ValueError,
+            paradigm.get_data,
+            dataset,
+            subjects=[1],
+            return_epochs=True,
+            return_raws=True,
+        )
 
     def test_BaseSSVEP_channel_order(self):
         """test if paradigm return correct channel order, see issue #227"""
         datasetA = FakeDataset(paradigm="ssvep", channels=["C3", "Cz", "C4"])
         datasetB = FakeDataset(paradigm="ssvep", channels=["Cz", "C4", "C3"])
         paradigm = BaseSSVEP(channels=["C4", "C3", "Cz"])
 
@@ -323,14 +417,41 @@
         paradigm = BaseSSVEP(n_classes=4)
         dataset = FakeDataset(event_list=["13", "15"], paradigm="ssvep")
         self.assertRaises(ValueError, paradigm.get_data, dataset)
 
     def test_BaseSSVEP_moreclassesthanevent(self):
         self.assertRaises(AssertionError, BaseSSVEP, n_classes=3, events=["13.", "14."])
 
+    def test_BaseSSVEP_droppedevent(self):
+        dataset = FakeDataset(paradigm="ssvep")
+        tmax = dataset.interval[1]
+        # with regular windows, all epochs should be valid:
+        paradigm1 = BaseSSVEP(tmax=tmax)
+        # with large windows, some epochs will have to be dropped:
+        paradigm2 = BaseSSVEP(tmax=10 * tmax)
+        # with epochs:
+        epochs1, labels1, metadata1 = paradigm1.get_data(dataset, return_epochs=True)
+        epochs2, labels2, metadata2 = paradigm2.get_data(dataset, return_epochs=True)
+        self.assertEqual(len(epochs1), len(labels1), len(metadata1))
+        self.assertEqual(len(epochs2), len(labels2), len(metadata2))
+        self.assertGreater(len(epochs1), len(epochs2))
+        # with np.array:
+        X1, labels1, metadata1 = paradigm1.get_data(dataset)
+        X2, labels2, metadata2 = paradigm2.get_data(dataset)
+        self.assertEqual(len(X1), len(labels1), len(metadata1))
+        self.assertEqual(len(X2), len(labels2), len(metadata2))
+        self.assertGreater(len(X1), len(X2))
+
+    def test_BaseSSVEP_epochsmetadata(self):
+        dataset = FakeDataset(paradigm="ssvep")
+        paradigm = BaseSSVEP()
+        epochs, _, metadata = paradigm.get_data(dataset, return_epochs=True)
+        # does not work with multiple filters:
+        self.assertTrue(metadata.equals(epochs.metadata))
+
     def test_SSVEP_noevent(self):
         # Assert error if events from paradigm and dataset dont overlap
         paradigm = SSVEP(events=["11", "12"], n_classes=2)
         dataset = FakeDataset(event_list=["13", "14"], paradigm="ssvep")
         self.assertRaises(AssertionError, paradigm.get_data, dataset)
 
     def test_SSVEP_paradigm(self):
```

### Comparing `moabb-0.4.6/pyproject.toml` & `moabb-0.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,76 @@
 [tool.poetry]
 name = "moabb"
-version = "0.4.6"
+version = "0.5.0"
 description = "Mother of All BCI Benchmarks"
 authors = ["Alexandre Barachant", "Vinay Jayaram"]
-maintainers = ["Sylvain Chevallier <sylvain.chevallier@uvsq.fr>"]
+maintainers = ["Sylvain Chevallier <sylvain.chevallier@universite-paris-saclay.fr>"]
 readme = "README.md"
 repository = "https://github.com/NeuroTechX/moabb"
-documentation = "http://moabb.neurotechx.com/docs/index.html"
+documentation = "https://neurotechx.github.io/moabb"
 keywords = ["eeg", "datasets", "reproducibility", "bci", "benchmark"]
 license = "BSD-3-Clause"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-numpy = "^1.19.0"
-scipy = "^1.5"
-mne = ">=0.19"
-pandas = "^1.0"
-h5py = "^3.0"
-scikit-learn = "^1.0"
-pyriemann = ">=0.2.6"
-matplotlib = "^3.0"
-seaborn = ">=0.9"
-PyYAML = "^5.0"
-pooch = "^1.6"
-requests = "^2.15.1"
-coverage = "^5.5"
-tqdm = "^4.62"
-
-[tool.poetry.dev-dependencies]
-Sphinx = "^3.3"
-sphinx-gallery = "^0.8.2"
-sphinx-bootstrap-theme = "^0.8"
-numpydoc = "^1.1.0"
-m2r2 = "^0.2.7"
-mistune = "<2"
-pre-commit = "^2.11.1"
+python = ">=3.8, <3.11"
+numpy = "^1.22"
+scipy = "^1.9.3"
+mne = "^1.3.0"
+pandas = "^1.5.2"
+h5py = "^3.7.0"
+scikit-learn = "^1.2.0"
+matplotlib = "^3.6.2"
+seaborn = "^0.12.1"
+pyriemann = "^0.3"
+PyYAML = "^6.0"
+pooch = "^1.6.0"
+requests = "^2.28.1"
+tqdm = "^4.64.1"
+coverage = "^7.0.1"
+memory-profiler = "^0.61.0"
+
+[tool.poetry.group.carbonemission]
+optional = true
+
+[tool.poetry.group.carbonemission.dependencies]
+codecarbon = "^2.1.4" # for carbon emission
+
+[tool.poetry.group.deeplearning]
+optional = true
+
+[tool.poetry.group.deeplearning.dependencies]
+tensorflow = "^2.10"
+keras = ">=1.11.0"
+scikeras = "^0.10.0"
+braindecode = "^0.7"
+torch = "^1.13.1"
+libclang = "^15.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^5.3.0"
+sphinx-gallery = "^0.11.1"
+sphinx-bootstrap-theme = "^0.8.1"
+pydata-sphinx-theme = "^0.13.2"
+numpydoc = "^1.5.0"
+pre-commit = "^2.21.0"
+m2r2 = "^0.3.0"
 tdlda = {git = "https://github.com/jsosulski/tdlda.git", rev = "0.1.0"}
+sphinx-design = "^0.3.0"
+sphinx-rtd-theme = "^1.2.0"
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 90
-target-version = ["py36"]
+target-version = ["py38"]
 
 [tool.isort]
 src_paths = ["moabb"]
 profile = "black"
 line_length = 90
 lines_after_imports = 2
```

### Comparing `moabb-0.4.6/setup.py` & `moabb-0.5.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,43 +7,59 @@
  'moabb.datasets',
  'moabb.evaluations',
  'moabb.paradigms',
  'moabb.pipelines',
  'moabb.tests']
 
 package_data = \
-{'': ['*'], 'moabb.tests': ['test_pipelines/*']}
+{'': ['*'],
+ 'moabb.tests': ['None/GridSearch_CrossSession/FakeDataset/1/C/*',
+                 'None/GridSearch_CrossSession/FakeDataset/2/C/*',
+                 'None/GridSearch_CrossSubject/FakeDataset/C/*',
+                 'None/GridSearch_WithinSession/FakeDataset/subject1/session_0/C/*',
+                 'None/GridSearch_WithinSession/FakeDataset/subject1/session_1/C/*',
+                 'None/GridSearch_WithinSession/FakeDataset/subject2/session_0/C/*',
+                 'None/GridSearch_WithinSession/FakeDataset/subject2/session_1/C/*',
+                 'res_test/GridSearch_CrossSession/FakeDataset/1/C/*',
+                 'res_test/GridSearch_CrossSession/FakeDataset/2/C/*',
+                 'res_test/GridSearch_CrossSubject/FakeDataset/C/*',
+                 'res_test/GridSearch_WithinSession/FakeDataset/subject1/session_0/C/*',
+                 'res_test/GridSearch_WithinSession/FakeDataset/subject1/session_1/C/*',
+                 'res_test/GridSearch_WithinSession/FakeDataset/subject2/session_0/C/*',
+                 'res_test/GridSearch_WithinSession/FakeDataset/subject2/session_1/C/*',
+                 'test_pipelines/*']}
 
 install_requires = \
-['PyYAML>=5.0,<6.0',
- 'coverage>=5.5,<6.0',
- 'h5py>=3.0,<4.0',
- 'matplotlib>=3.0,<4.0',
- 'mne>=0.19',
- 'numpy>=1.19.0,<2.0.0',
- 'pandas>=1.0,<2.0',
- 'pooch>=1.6,<2.0',
- 'pyriemann>=0.2.6',
- 'requests>=2.15.1,<3.0.0',
- 'scikit-learn>=1.0,<2.0',
- 'scipy>=1.5,<2.0',
- 'seaborn>=0.9',
- 'tqdm>=4.62,<5.0']
+['PyYAML>=6.0,<7.0',
+ 'coverage>=7.0.1,<8.0.0',
+ 'h5py>=3.7.0,<4.0.0',
+ 'matplotlib>=3.6.2,<4.0.0',
+ 'memory-profiler>=0.61.0,<0.62.0',
+ 'mne>=1.3.0,<2.0.0',
+ 'numpy>=1.22,<2.0',
+ 'pandas>=1.5.2,<2.0.0',
+ 'pooch>=1.6.0,<2.0.0',
+ 'pyriemann>=0.3,<0.4',
+ 'requests>=2.28.1,<3.0.0',
+ 'scikit-learn>=1.2.0,<2.0.0',
+ 'scipy>=1.9.3,<2.0.0',
+ 'seaborn>=0.12.1,<0.13.0',
+ 'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'moabb',
-    'version': '0.4.6',
+    'version': '0.5.0',
     'description': 'Mother of All BCI Benchmarks',
-    'long_description': '# Mother of all BCI Benchmarks\n\n<p align=center>\n  <img alt="banner" src="/images/M.png/">\n</p>\n<p align=center>\n  Build a comprehensive benchmark of popular Brain-Computer Interface (BCI) algorithms applied on an extensive list of freely available EEG datasets.\n</p>\n\n## Disclaimer\n\n**This is an open science project that may evolve depending on the need of the\ncommunity.**\n\n[![Build Status](https://github.com/NeuroTechX/moabb/workflows/Test/badge.svg)](https://github.com/NeuroTechX/moabb/actions?query=branch%3Amaster)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI](https://img.shields.io/pypi/v/moabb?color=blue&style=plastic)](https://img.shields.io/pypi/v/moabb)\n[![Downloads](https://pepy.tech/badge/moabb)](https://pepy.tech/project/moabb)\n\n## Welcome!\n\nFirst and foremost, Welcome! :tada: Willkommen! :confetti_ball: Bienvenue!\n:balloon::balloon::balloon:\n\nThank you for visiting the Mother of all BCI Benchmark repository.\n\nThis document is a hub to give you some information about the project. Jump straight to\none of the sections below, or just scroll down to find out more.\n\n- [What are we doing? (And why?)](#what-are-we-doing)\n- [Installation](#installation)\n- [Running](#running)\n- [Supported datasets](#supported-datasets)\n- [Who are we? n](#who-are-we)\n- [Get in touch](#contact-us)\n- [Documentation][link_moabb_docs]\n- [Architecture and main concepts](#architecture-and-main-concepts)\n- [Citing MOABB and related publications](#citing-moabb-and-related-publications)\n\n## What are we doing?\n\n### The problem\n\n[Brain-Computer Interfaces](https://en.wikipedia.org/wiki/Brain%E2%80%93computer_interface)\nallow to interact with a computer using brain signals. In this project, we focus mostly on\nelectroencephalographic signals\n([EEG](https://en.wikipedia.org/wiki/Electroencephalography)), that is a very active\nresearch domain, with worldwide scientific contributions. Still:\n\n- Reproducible Research in BCI has a long way to go.\n- While many BCI datasets are made freely available, researchers do not publish code, and\n  reproducing results required to benchmark new algorithms turns out to be trickier than\n  it should be.\n- Performances can be significantly impacted by parameters of the preprocessing steps,\n  toolboxes used and implementation “tricks” that are almost never reported in the\n  literature.\n\nAs a result, there is no comprehensive benchmark of BCI algorithms, and newcomers are\nspending a tremendous amount of time browsing literature to find out what algorithm works\nbest and on which dataset.\n\n### The solution\n\nThe Mother of all BCI Benchmarks allows to:\n\n- Build a comprehensive benchmark of popular BCI algorithms applied on an extensive list\n  of freely available EEG datasets.\n- The code will be made available on github, serving as a reference point for the future\n  algorithmic developments.\n- Algorithms can be ranked and promoted on a website, providing a clear picture of the\n  different solutions available in the field.\n\nThis project will be successful when we read in an abstract “ … the proposed method\nobtained a score of 89% on the MOABB (Mother of All BCI Benchmarks), outperforming the\nstate of the art by 5% ...”.\n\n## Installation\n\n### Pip installation\n\nTo use MOABB, you could simply do: \\\n`pip install MOABB` \\\nSee [Troubleshooting](#Troubleshooting) section if you have a problem.\n\n### Manual installation\n\nYou could fork or clone the repository and go to the downloaded directory, then run:\n\n1. install `poetry` (only once per machine):\\\n   `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -`\\\n   or [checkout installation instruction](https://python-poetry.org/docs/#installation) or\n   use [conda forge version](https://anaconda.org/conda-forge/poetry)\n1. (Optional, skip if not sure) Disable automatic environment creation:\\\n   `poetry config virtualenvs.create false`\n1. install all dependencies in one command (have to be run in the project directory):\\\n   `poetry install`\n\nSee [contributors\' guidelines](CONTRIBUTING.md) for detailed explanation.\n\n### Requirements we use\n\nSee `pyproject.toml` file for full list of dependencies\n\n## Running\n\n### Verify Installation\n\nTo ensure it is running correctly, you can also run\n\n```\npython -m unittest moabb.tests\n```\n\nonce it is installed.\n\n### Use MOABB\n\nFirst, you could take a look at our [tutorials](./tutorials) that cover the most important\nconcepts and use cases. Also, we have a several [examples](./examples/) available.\n\nYou might be interested in [MOABB documentation][link_moabb_docs]\n\n### Troubleshooting\n\nCurrently pip install moabb fails when pip version < 21, e.g. with 20.0.2 due to an `idna`\npackage conflict. Newer pip versions resolve this conflict automatically. To fix this you\ncan upgrade your pip version using: `pip install -U pip` before installing `moabb`.\n\n## Supported datasets\n\nThe list of supported datasets can be found here :\nhttps://neurotechx.github.io/moabb/datasets.html\n\n### Submit a new dataset\n\nyou can submit a new dataset by mentioning it to this\n[issue](https://github.com/NeuroTechX/moabb/issues/1). The datasets currently on our radar\ncan be seen [here] (https://github.com/NeuroTechX/moabb/wiki/Datasets-Support)\n\n## Who are we?\n\nThe founders of the Mother of all BCI Benchmarks are [Alexander Barachant][link_alex_b]\nand [Vinay Jayaram][link_vinay]. This project is under the umbrella of\n[NeuroTechX][link_neurotechx], the international community for NeuroTech enthusiasts. The\nproject is currently maintained by [Sylvain Chevallier][link_sylvain].\n\n### What do we need?\n\n**You**! In whatever way you can help.\n\nWe need expertise in programming, user experience, software sustainability, documentation\nand technical writing and project management.\n\nWe\'d love your feedback along the way.\n\nOur primary goal is to build a comprehensive benchmark of popular BCI algorithms applied\non an extensive list of freely available EEG datasets, and we\'re excited to support the\nprofessional development of any and all of our contributors. If you\'re looking to learn to\ncode, try out working collaboratively, or translate your skills to the digital domain,\nwe\'re here to help.\n\n### Get involved\n\nIf you think you can help in any of the areas listed above (and we bet you can) or in any\nof the many areas that we haven\'t yet thought of (and here we\'re _sure_ you can) then\nplease check out our [contributors\' guidelines](CONTRIBUTING.md) and our\n[roadmap](ROADMAP.md).\n\nPlease note that it\'s very important to us that we maintain a positive and supportive\nenvironment for everyone who wants to participate. When you join us we ask that you follow\nour [code of conduct](CODE_OF_CONDUCT.md) in all interactions both on and offline.\n\n## Contact us\n\nIf you want to report a problem or suggest an enhancement, we\'d love for you to\n[open an issue](../../issues) at this github repository because then we can get right on\nit.\n\nFor a less formal discussion or exchanging ideas, you can also reach us on the [Gitter\nchannel][link_gitter] or join our weekly office hours! This an open video meeting\nhappening on a [regular basis](https://github.com/NeuroTechX/moabb/issues/191), please ask\nthe link on the gitter channel. We are also on [NeuroTechX slack #moabb\nchannel][link_neurotechx_signup].\n\n## Architecture and Main Concepts\n\n<p align="center">\n  <img alt="banner" src="/images/architecture.png/" width="400">\n</p>\nThere are 4 main concepts in the MOABB: the datasets, the paradigm, the evaluation, and the pipelines. In addition, we offer statistical and visualization utilities to simplify the workflow.\n\n### Datasets\n\nA dataset handles and abstracts low-level access to the data. The dataset will read data\nstored locally, in the format in which they have been downloaded, and will convert them\ninto a MNE raw object. There are options to pool all the different recording sessions per\nsubject or to evaluate them separately.\n\n### Paradigm\n\nA paradigm defines how the raw data will be converted to trials ready to be processed by a\ndecoding algorithm. This is a function of the paradigm used, i.e. in motor imagery one can\nhave two-class, multi-class, or continuous paradigms; similarly, different preprocessing\nis necessary for ERP vs ERD paradigms.\n\n### Evaluations\n\nAn evaluation defines how we go from trials per subject and session to a generalization\nstatistic (AUC score, f-score, accuracy, etc) -- it can be either within-recording-session\naccuracy, across-session within-subject accuracy, across-subject accuracy, or other\ntransfer learning settings.\n\n### Pipelines\n\nPipeline defines all steps required by an algorithm to obtain predictions. Pipelines are\ntypically a chain of sklearn compatible transformers and end with a sklearn compatible\nestimator. See\n[Pipelines](http://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html)\nfor more info.\n\n### Statistics and visualization\n\nOnce an evaluation has been run, the raw results are returned as a DataFrame. This can be\nfurther processed via the following commands to generate some basic visualization and\nstatistical comparisons:\n\n```\nfrom moabb.analysis import analyze\n\nresults = evaluation.process(pipeline_dict)\nanalyze(results)\n```\n\n## Citing MOABB and related publications\n\nTo cite MOABB, you could use the following paper:\n\n> Vinay Jayaram and Alexandre Barachant.\n> ["MOABB: trustworthy algorithm benchmarking for BCIs."](http://iopscience.iop.org/article/10.1088/1741-2552/aadea0/meta)\n> Journal of neural engineering 15.6 (2018): 066011.\n> [DOI](https://doi.org/10.1088/1741-2552/aadea0)\n\nIf you publish a paper using MOABB, please contact us on [gitter][link_gitter] or open an\nissue, and we will add your paper to the\n[dedicated wiki page](https://github.com/NeuroTechX/moabb/wiki/MOABB-bibliography).\n\n## Thank You\n\nThank you so much (Danke schön! Merci beaucoup!) for visiting the project and we do hope\nthat you\'ll join us on this amazing journey to build a comprehensive benchmark of popular\nBCI algorithms applied on an extensive list of freely available EEG datasets.\n\n[link_alex_b]: http://alexandre.barachant.org/\n[link_vinay]: https://ei.is.tuebingen.mpg.de/~vjayaram\n[link_neurotechx]: http://neurotechx.com/\n[link_sylvain]: https://sylvchev.github.io/\n[link_neurotechx_signup]: https://neurotechx.com/\n[link_gitter]: https://gitter.im/moabb_dev/community\n[link_moabb_docs]: https://neurotechx.github.io/moabb/\n[link_arxiv]: https://arxiv.org/abs/1805.06427\n[link_jne]: http://iopscience.iop.org/article/10.1088/1741-2552/aadea0/meta\n',
+    'long_description': '# Mother of all BCI Benchmarks\n\n<p align=center>\n  <img alt="banner" src="/images/M.png/">\n</p>\n<p align=center>\n  Build a comprehensive benchmark of popular Brain-Computer Interface (BCI) algorithms applied on an extensive list of freely available EEG datasets.\n</p>\n\n## Disclaimer\n\n**This is an open science project that may evolve depending on the need of the\ncommunity.**\n\n[![Build Status](https://github.com/NeuroTechX/moabb/workflows/Test/badge.svg)](https://github.com/NeuroTechX/moabb/actions?query=branch%3Amaster)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI](https://img.shields.io/pypi/v/moabb?color=blue&style=plastic)](https://img.shields.io/pypi/v/moabb)\n[![Downloads](https://pepy.tech/badge/moabb)](https://pepy.tech/project/moabb)\n\n## Welcome!\n\nFirst and foremost, Welcome! :tada: Willkommen! :confetti_ball: Bienvenue!\n:balloon::balloon::balloon:\n\nThank you for visiting the Mother of all BCI Benchmark repository.\n\nThis document is a hub to give you some information about the project. Jump straight to\none of the sections below, or just scroll down to find out more.\n\n- [What are we doing? (And why?)](#what-are-we-doing)\n- [Installation](#installation)\n- [Running](#running)\n- [Supported datasets](#supported-datasets)\n- [Who are we?](#who-are-we)\n- [Get in touch](#contact-us)\n- [Documentation][link_moabb_docs]\n- [Architecture and main concepts](#architecture-and-main-concepts)\n- [Citing MOABB and related publications](#citing-moabb-and-related-publications)\n\n## What are we doing?\n\n### The problem\n\n[Brain-Computer Interfaces](https://en.wikipedia.org/wiki/Brain%E2%80%93computer_interface)\nallow to interact with a computer using brain signals. In this project, we focus mostly on\nelectroencephalographic signals\n([EEG](https://en.wikipedia.org/wiki/Electroencephalography)), that is a very active\nresearch domain, with worldwide scientific contributions. Still:\n\n- Reproducible Research in BCI has a long way to go.\n- While many BCI datasets are made freely available, researchers do not publish code, and\n  reproducing results required to benchmark new algorithms turns out to be trickier than\n  it should be.\n- Performances can be significantly impacted by parameters of the preprocessing steps,\n  toolboxes used and implementation “tricks” that are almost never reported in the\n  literature.\n\nAs a result, there is no comprehensive benchmark of BCI algorithms, and newcomers are\nspending a tremendous amount of time browsing literature to find out what algorithm works\nbest and on which dataset.\n\n### The solution\n\nThe Mother of all BCI Benchmarks allows to:\n\n- Build a comprehensive benchmark of popular BCI algorithms applied on an extensive list\n  of freely available EEG datasets.\n- The code is available on GitHub, serving as a reference point for the future algorithmic\n  developments.\n- Algorithms can be ranked and promoted on a website, providing a clear picture of the\n  different solutions available in the field.\n\nThis project will be successful when we read in an abstract “ … the proposed method\nobtained a score of 89% on the MOABB (Mother of All BCI Benchmarks), outperforming the\nstate of the art by 5% ...”.\n\n## Installation\n\n### Pip installation\n\nTo use MOABB, you could simply do: \\\n`pip install MOABB` \\\nSee [Troubleshooting](#Troubleshooting) section if you have a problem.\n\n### Manual installation\n\nYou could fork or clone the repository and go to the downloaded directory, then run:\n\n1. install `poetry` (only once per machine):\\\n   `curl -sSL https://install.python-poetry.org | python3 -`\\\n   or [checkout installation instruction](https://python-poetry.org/docs/#installation) or\n   use [conda forge version](https://anaconda.org/conda-forge/poetry)\n1. (Optional, skip if not sure) Disable automatic environment creation:\\\n   `poetry config virtualenvs.create false`\n1. install all dependencies in one command (have to be run in the project directory):\\\n   `poetry install`\n\nSee [contributors\' guidelines](CONTRIBUTING.md) for detailed explanation.\n\n### Requirements we use\n\nSee `pyproject.toml` file for full list of dependencies\n\n## Running\n\n### Verify Installation\n\nTo ensure it is running correctly, you can also run\n\n```\npython -m unittest moabb.tests\n```\n\nonce it is installed.\n\n### Use MOABB\n\nFirst, you could take a look at our [tutorials](./tutorials) that cover the most important\nconcepts and use cases. Also, we have a several [examples](./examples/) available.\n\nYou might be interested in [MOABB documentation][link_moabb_docs]\n\n### Moabb and docker\n\nMoabb has a default image to run the benchmark. You have two options to download this\nimage: build from scratch or pull from the docker hub. **We recommend pulling from the\ndocker hub**.\n\nIf this were your first time using docker, you would need to **install the docker** and\n**login** on docker hub. We recommend the\n[official](https://docs.docker.com/desktop/install/linux-install/) docker documentation\nfor this step, it is essential to follow the instructions.\n\nAfter installing docker, you can pull the image from the docker hub:\n\n```bash\ndocker pull baristimunha/moabb\n# rename the tag to moabb\ndocker tag baristimunha/moabb moabb\n```\n\nIf you want to build the image from scratch, you can use the following command at the\nroot. You may have to login with the API key in the\n[NGC Catalog](https://catalog.ngc.nvidia.com/) to run this command.\n\n```bash\nbash docker/create_docker.sh\n```\n\nWith the image downloaded or rebuilt from scratch, you will have an image called `moabb`.\nTo run the default benchmark, still at the root of the project, and you can use the\nfollowing command:\n\n```bash\nmkdir dataset\nmkdir results\nmkdir output\nbash docker/run_docker.sh PATH_TO_ROOT_FOLDER\n```\n\nAn example of the command is:\n\n```bash\ncd /home/user/project/moabb\nmkdir dataset\nmkdir results\nmkdir output\nbash docker/run_docker.sh /home/user/project/moabb\n```\n\nNote: It is important to use an absolute path for the root folder to run, but you can\nmodify the run_docker.sh script to save in another path beyond the root of the project. By\ndefault, the script will save the results in the project\'s root in the folder `results`,\nthe datasets in the folder `dataset` and the output in the folder `output`.\n\n### Troubleshooting\n\nCurrently pip install moabb fails when pip version < 21, e.g. with 20.0.2 due to an `idna`\npackage conflict. Newer pip versions resolve this conflict automatically. To fix this you\ncan upgrade your pip version using: `pip install -U pip` before installing `moabb`.\n\n## Supported datasets\n\nThe list of supported datasets can be found here :\nhttps://neurotechx.github.io/moabb/datasets.html\n\nDetailed information regarding datasets (electrodes, trials, sessions) are indicated on\nthe wiki: https://github.com/NeuroTechX/moabb/wiki/Datasets-Support\n\n### Submit a new dataset\n\nyou can submit a new dataset by mentioning it to this\n[issue](https://github.com/NeuroTechX/moabb/issues/1). The datasets currently on our radar\ncan be seen [here] (https://github.com/NeuroTechX/moabb/wiki/Datasets-Support)\n\n## Who are we?\n\nThe founders of the Mother of all BCI Benchmarks are [Alexander Barachant][link_alex_b]\nand [Vinay Jayaram][link_vinay]. This project is under the umbrella of\n[NeuroTechX][link_neurotechx], the international community for NeuroTech enthusiasts. The\nproject is currently maintained by [Sylvain Chevallier][link_sylvain].\n\n### What do we need?\n\n**You**! In whatever way you can help.\n\nWe need expertise in programming, user experience, software sustainability, documentation\nand technical writing and project management.\n\nWe\'d love your feedback along the way.\n\nOur primary goal is to build a comprehensive benchmark of popular BCI algorithms applied\non an extensive list of freely available EEG datasets, and we\'re excited to support the\nprofessional development of any and all of our contributors. If you\'re looking to learn to\ncode, try out working collaboratively, or translate your skills to the digital domain,\nwe\'re here to help.\n\n### Get involved\n\nIf you think you can help in any of the areas listed above (and we bet you can) or in any\nof the many areas that we haven\'t yet thought of (and here we\'re _sure_ you can) then\nplease check out our [contributors\' guidelines](CONTRIBUTING.md) and our\n[roadmap](ROADMAP.md).\n\nPlease note that it\'s very important to us that we maintain a positive and supportive\nenvironment for everyone who wants to participate. When you join us we ask that you follow\nour [code of conduct](CODE_OF_CONDUCT.md) in all interactions both on and offline.\n\n## Contact us\n\nIf you want to report a problem or suggest an enhancement, we\'d love for you to\n[open an issue](../../issues) at this GitHub repository because then we can get right on\nit.\n\nFor a less formal discussion or exchanging ideas, you can also reach us on the [Gitter\nchannel][link_gitter] or join our weekly office hours! This an open video meeting\nhappening on a [regular basis](https://github.com/NeuroTechX/moabb/issues/191), please ask\nthe link on the gitter channel. We are also on [NeuroTechX Slack #moabb\nchannel][link_neurotechx_signup].\n\n## Architecture and Main Concepts\n\n<p align="center">\n  <img alt="banner" src="/images/architecture.png/" width="400">\n</p>\nThere are 4 main concepts in the MOABB: the datasets, the paradigm, the evaluation, and the pipelines. In addition, we offer statistical and visualization utilities to simplify the workflow.\n\n### Datasets\n\nA dataset handles and abstracts low-level access to the data. The dataset will read data\nstored locally, in the format in which they have been downloaded, and will convert them\ninto a MNE raw object. There are options to pool all the different recording sessions per\nsubject or to evaluate them separately.\n\n### Paradigm\n\nA paradigm defines how the raw data will be converted to trials ready to be processed by a\ndecoding algorithm. This is a function of the paradigm used, i.e. in motor imagery one can\nhave two-class, multi-class, or continuous paradigms; similarly, different preprocessing\nis necessary for ERP vs ERD paradigms.\n\n### Evaluations\n\nAn evaluation defines how we go from trials per subject and session to a generalization\nstatistic (AUC score, f-score, accuracy, etc) -- it can be either within-recording-session\naccuracy, across-session within-subject accuracy, across-subject accuracy, or other\ntransfer learning settings.\n\n### Pipelines\n\nPipeline defines all steps required by an algorithm to obtain predictions. Pipelines are\ntypically a chain of sklearn compatible transformers and end with a sklearn compatible\nestimator. See\n[Pipelines](http://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html)\nfor more info.\n\n### Statistics and visualization\n\nOnce an evaluation has been run, the raw results are returned as a DataFrame. This can be\nfurther processed via the following commands to generate some basic visualization and\nstatistical comparisons:\n\n```\nfrom moabb.analysis import analyze\n\nresults = evaluation.process(pipeline_dict)\nanalyze(results)\n```\n\n## Citing MOABB and related publications\n\nTo cite MOABB, you could use the following paper:\n\n> Vinay Jayaram and Alexandre Barachant.\n> ["MOABB: trustworthy algorithm benchmarking for BCIs."](http://iopscience.iop.org/article/10.1088/1741-2552/aadea0/meta)\n> Journal of neural engineering 15.6 (2018): 066011.\n> [DOI](https://doi.org/10.1088/1741-2552/aadea0)\n\nIf you publish a paper using MOABB, please contact us on [gitter][link_gitter] or open an\nissue, and we will add your paper to the\n[dedicated wiki page](https://github.com/NeuroTechX/moabb/wiki/MOABB-bibliography).\n\n## Thank You\n\nThank you so much (Danke schön! Merci beaucoup!) for visiting the project and we do hope\nthat you\'ll join us on this amazing journey to build a comprehensive benchmark of popular\nBCI algorithms applied on an extensive list of freely available EEG datasets.\n\n[link_alex_b]: http://alexandre.barachant.org/\n[link_vinay]: https://ei.is.tuebingen.mpg.de/~vjayaram\n[link_neurotechx]: http://neurotechx.com/\n[link_sylvain]: https://sylvchev.github.io/\n[link_neurotechx_signup]: https://neurotechx.com/\n[link_gitter]: https://app.gitter.im/#/room/#moabb_dev_community:gitter.im\n[link_moabb_docs]: https://neurotechx.github.io/moabb/\n[link_arxiv]: https://arxiv.org/abs/1805.06427\n[link_jne]: http://iopscience.iop.org/article/10.1088/1741-2552/aadea0/meta\n',
     'author': 'Alexandre Barachant',
-    'author_email': None,
+    'author_email': 'None',
     'maintainer': 'Sylvain Chevallier',
-    'maintainer_email': 'sylvain.chevallier@uvsq.fr',
+    'maintainer_email': 'sylvain.chevallier@universite-paris-saclay.fr',
     'url': 'https://github.com/NeuroTechX/moabb',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `moabb-0.4.6/PKG-INFO` & `moabb-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: moabb
-Version: 0.4.6
+Version: 0.5.0
 Summary: Mother of All BCI Benchmarks
 Home-page: https://github.com/NeuroTechX/moabb
 License: BSD-3-Clause
 Keywords: eeg,datasets,reproducibility,bci,benchmark
 Author: Alexandre Barachant
 Maintainer: Sylvain Chevallier
-Maintainer-email: sylvain.chevallier@uvsq.fr
-Requires-Python: >=3.7,<4.0
+Maintainer-email: sylvain.chevallier@universite-paris-saclay.fr
+Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyYAML (>=5.0,<6.0)
-Requires-Dist: coverage (>=5.5,<6.0)
-Requires-Dist: h5py (>=3.0,<4.0)
-Requires-Dist: matplotlib (>=3.0,<4.0)
-Requires-Dist: mne (>=0.19)
-Requires-Dist: numpy (>=1.19.0,<2.0.0)
-Requires-Dist: pandas (>=1.0,<2.0)
-Requires-Dist: pooch (>=1.6,<2.0)
-Requires-Dist: pyriemann (>=0.2.6)
-Requires-Dist: requests (>=2.15.1,<3.0.0)
-Requires-Dist: scikit-learn (>=1.0,<2.0)
-Requires-Dist: scipy (>=1.5,<2.0)
-Requires-Dist: seaborn (>=0.9)
-Requires-Dist: tqdm (>=4.62,<5.0)
-Project-URL: Documentation, http://moabb.neurotechx.com/docs/index.html
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: coverage (>=7.0.1,<8.0.0)
+Requires-Dist: h5py (>=3.7.0,<4.0.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: memory-profiler (>=0.61.0,<0.62.0)
+Requires-Dist: mne (>=1.3.0,<2.0.0)
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pooch (>=1.6.0,<2.0.0)
+Requires-Dist: pyriemann (>=0.3,<0.4)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Documentation, https://neurotechx.github.io/moabb
 Project-URL: Repository, https://github.com/NeuroTechX/moabb
 Description-Content-Type: text/markdown
 
 # Mother of all BCI Benchmarks
 
 <p align=center>
   <img alt="banner" src="/images/M.png/">
@@ -62,15 +62,15 @@
 This document is a hub to give you some information about the project. Jump straight to
 one of the sections below, or just scroll down to find out more.
 
 - [What are we doing? (And why?)](#what-are-we-doing)
 - [Installation](#installation)
 - [Running](#running)
 - [Supported datasets](#supported-datasets)
-- [Who are we? n](#who-are-we)
+- [Who are we?](#who-are-we)
 - [Get in touch](#contact-us)
 - [Documentation][link_moabb_docs]
 - [Architecture and main concepts](#architecture-and-main-concepts)
 - [Citing MOABB and related publications](#citing-moabb-and-related-publications)
 
 ## What are we doing?
 
@@ -96,16 +96,16 @@
 
 ### The solution
 
 The Mother of all BCI Benchmarks allows to:
 
 - Build a comprehensive benchmark of popular BCI algorithms applied on an extensive list
   of freely available EEG datasets.
-- The code will be made available on github, serving as a reference point for the future
-  algorithmic developments.
+- The code is available on GitHub, serving as a reference point for the future algorithmic
+  developments.
 - Algorithms can be ranked and promoted on a website, providing a clear picture of the
   different solutions available in the field.
 
 This project will be successful when we read in an abstract “ … the proposed method
 obtained a score of 89% on the MOABB (Mother of All BCI Benchmarks), outperforming the
 state of the art by 5% ...”.
 
@@ -118,15 +118,15 @@
 See [Troubleshooting](#Troubleshooting) section if you have a problem.
 
 ### Manual installation
 
 You could fork or clone the repository and go to the downloaded directory, then run:
 
 1. install `poetry` (only once per machine):\
-   `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -`\
+   `curl -sSL https://install.python-poetry.org | python3 -`\
    or [checkout installation instruction](https://python-poetry.org/docs/#installation) or
    use [conda forge version](https://anaconda.org/conda-forge/poetry)
 1. (Optional, skip if not sure) Disable automatic environment creation:\
    `poetry config virtualenvs.create false`
 1. install all dependencies in one command (have to be run in the project directory):\
    `poetry install`
 
@@ -151,25 +151,81 @@
 ### Use MOABB
 
 First, you could take a look at our [tutorials](./tutorials) that cover the most important
 concepts and use cases. Also, we have a several [examples](./examples/) available.
 
 You might be interested in [MOABB documentation][link_moabb_docs]
 
+### Moabb and docker
+
+Moabb has a default image to run the benchmark. You have two options to download this
+image: build from scratch or pull from the docker hub. **We recommend pulling from the
+docker hub**.
+
+If this were your first time using docker, you would need to **install the docker** and
+**login** on docker hub. We recommend the
+[official](https://docs.docker.com/desktop/install/linux-install/) docker documentation
+for this step, it is essential to follow the instructions.
+
+After installing docker, you can pull the image from the docker hub:
+
+```bash
+docker pull baristimunha/moabb
+# rename the tag to moabb
+docker tag baristimunha/moabb moabb
+```
+
+If you want to build the image from scratch, you can use the following command at the
+root. You may have to login with the API key in the
+[NGC Catalog](https://catalog.ngc.nvidia.com/) to run this command.
+
+```bash
+bash docker/create_docker.sh
+```
+
+With the image downloaded or rebuilt from scratch, you will have an image called `moabb`.
+To run the default benchmark, still at the root of the project, and you can use the
+following command:
+
+```bash
+mkdir dataset
+mkdir results
+mkdir output
+bash docker/run_docker.sh PATH_TO_ROOT_FOLDER
+```
+
+An example of the command is:
+
+```bash
+cd /home/user/project/moabb
+mkdir dataset
+mkdir results
+mkdir output
+bash docker/run_docker.sh /home/user/project/moabb
+```
+
+Note: It is important to use an absolute path for the root folder to run, but you can
+modify the run_docker.sh script to save in another path beyond the root of the project. By
+default, the script will save the results in the project's root in the folder `results`,
+the datasets in the folder `dataset` and the output in the folder `output`.
+
 ### Troubleshooting
 
 Currently pip install moabb fails when pip version < 21, e.g. with 20.0.2 due to an `idna`
 package conflict. Newer pip versions resolve this conflict automatically. To fix this you
 can upgrade your pip version using: `pip install -U pip` before installing `moabb`.
 
 ## Supported datasets
 
 The list of supported datasets can be found here :
 https://neurotechx.github.io/moabb/datasets.html
 
+Detailed information regarding datasets (electrodes, trials, sessions) are indicated on
+the wiki: https://github.com/NeuroTechX/moabb/wiki/Datasets-Support
+
 ### Submit a new dataset
 
 you can submit a new dataset by mentioning it to this
 [issue](https://github.com/NeuroTechX/moabb/issues/1). The datasets currently on our radar
 can be seen [here] (https://github.com/NeuroTechX/moabb/wiki/Datasets-Support)
 
 ## Who are we?
@@ -204,21 +260,21 @@
 Please note that it's very important to us that we maintain a positive and supportive
 environment for everyone who wants to participate. When you join us we ask that you follow
 our [code of conduct](CODE_OF_CONDUCT.md) in all interactions both on and offline.
 
 ## Contact us
 
 If you want to report a problem or suggest an enhancement, we'd love for you to
-[open an issue](../../issues) at this github repository because then we can get right on
+[open an issue](../../issues) at this GitHub repository because then we can get right on
 it.
 
 For a less formal discussion or exchanging ideas, you can also reach us on the [Gitter
 channel][link_gitter] or join our weekly office hours! This an open video meeting
 happening on a [regular basis](https://github.com/NeuroTechX/moabb/issues/191), please ask
-the link on the gitter channel. We are also on [NeuroTechX slack #moabb
+the link on the gitter channel. We are also on [NeuroTechX Slack #moabb
 channel][link_neurotechx_signup].
 
 ## Architecture and Main Concepts
 
 <p align="center">
   <img alt="banner" src="/images/architecture.png/" width="400">
 </p>
@@ -286,12 +342,12 @@
 BCI algorithms applied on an extensive list of freely available EEG datasets.
 
 [link_alex_b]: http://alexandre.barachant.org/
 [link_vinay]: https://ei.is.tuebingen.mpg.de/~vjayaram
 [link_neurotechx]: http://neurotechx.com/
 [link_sylvain]: https://sylvchev.github.io/
 [link_neurotechx_signup]: https://neurotechx.com/
-[link_gitter]: https://gitter.im/moabb_dev/community
+[link_gitter]: https://app.gitter.im/#/room/#moabb_dev_community:gitter.im
 [link_moabb_docs]: https://neurotechx.github.io/moabb/
 [link_arxiv]: https://arxiv.org/abs/1805.06427
 [link_jne]: http://iopscience.iop.org/article/10.1088/1741-2552/aadea0/meta
```

