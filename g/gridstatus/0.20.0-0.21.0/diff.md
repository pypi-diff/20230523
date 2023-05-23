# Comparing `tmp/gridstatus-0.20.0.tar.gz` & `tmp/gridstatus-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-3u3dc75r/gridstatus-0.20.0.tar", last modified: Fri Mar 24 21:00:15 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-g5585lv9/gridstatus-0.21.0.tar", last modified: Tue May 23 00:38:18 2023, max compression
```

## Comparing `gridstatus-0.20.0.tar` & `gridstatus-0.21.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-24 21:00:03.000000 gridstatus-0.20.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4443 2023-03-24 21:00:15.000000 gridstatus-0.20.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1995 2023-03-24 21:00:03.000000 gridstatus-0.20.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/docs/
--rw-r--r--   0 root         (0) root         (0)     4290 2023-03-24 21:00:03.000000 gridstatus-0.20.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-03-24 21:00:03.000000 gridstatus-0.20.0/docs/update_docs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus/
--rw-r--r--   0 root         (0) root         (0)      869 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/base.py
--rw-r--r--   0 root         (0) root         (0)    29736 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/caiso.py
--rw-r--r--   0 root         (0) root         (0)    11362 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/decorators.py
--rw-r--r--   0 root         (0) root         (0)    34371 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/ercot.py
--rw-r--r--   0 root         (0) root         (0)    22751 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/isone.py
--rw-r--r--   0 root         (0) root         (0)     5067 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/lmp_config.py
--rw-r--r--   0 root         (0) root         (0)      108 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/logging.py
--rw-r--r--   0 root         (0) root         (0)    10952 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/miso.py
--rw-r--r--   0 root         (0) root         (0)    24798 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/nyiso.py
--rw-r--r--   0 root         (0) root         (0)    21563 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/pjm.py
--rw-r--r--   0 root         (0) root         (0)    28516 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/spp.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9830 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/base_test_iso.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/decorators.py
--rw-r--r--   0 root         (0) root         (0)     5808 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_caiso.py
--rw-r--r--   0 root         (0) root         (0)     7391 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_ercot.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_gridstatus.py
--rw-r--r--   0 root         (0) root         (0)      215 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_interconnection_queue.py
--rw-r--r--   0 root         (0) root         (0)     2454 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_isone.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_lmp_config.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_miso.py
--rw-r--r--   0 root         (0) root         (0)     6115 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_nyiso.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_pjm.py
--rw-r--r--   0 root         (0) root         (0)     1079 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_save_to.py
--rw-r--r--   0 root         (0) root         (0)     9422 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_spp.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)       92 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_version.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/tests/test_viz.py
--rw-r--r--   0 root         (0) root         (0)     8117 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/version.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-03-24 21:00:03.000000 gridstatus-0.20.0/gridstatus/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4443 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      573 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-24 21:00:15.000000 gridstatus-0.20.0/gridstatus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3065 2023-03-24 21:00:03.000000 gridstatus-0.20.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 21:00:15.000000 gridstatus-0.20.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 21:00:15.000000 gridstatus-0.20.0/utils/ercot/
--rw-r--r--   0 root         (0) root         (0)     2481 2023-03-24 21:00:03.000000 gridstatus-0.20.0/utils/ercot/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-23 00:38:04.000000 gridstatus-0.21.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-05-23 00:38:18.000000 gridstatus-0.21.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-05-23 00:38:04.000000 gridstatus-0.21.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-05-23 00:38:04.000000 gridstatus-0.21.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-23 00:38:04.000000 gridstatus-0.21.0/docs/update_docs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus/
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/base.py
+-rw-r--r--   0 root         (0) root         (0)    45618 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/caiso.py
+-rw-r--r--   0 root         (0) root         (0)    12502 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     5567 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/eia.py
+-rw-r--r--   0 root         (0) root         (0)    35728 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/ercot.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/gs_logging.py
+-rw-r--r--   0 root         (0) root         (0)    23024 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/isone.py
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/lmp_config.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/miso.py
+-rw-r--r--   0 root         (0) root         (0)    26181 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/nyiso.py
+-rw-r--r--   0 root         (0) root         (0)    21566 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/pjm.py
+-rw-r--r--   0 root         (0) root         (0)    33028 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/spp.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12735 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/base_test_iso.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     9418 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_caiso.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_eia.py
+-rw-r--r--   0 root         (0) root         (0)     9292 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_ercot.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_gridstatus.py
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_interconnection_queue.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_isone.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_lmp_config.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_miso.py
+-rw-r--r--   0 root         (0) root         (0)     7599 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_nyiso.py
+-rw-r--r--   0 root         (0) root         (0)    11196 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_pjm.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_save_to.py
+-rw-r--r--   0 root         (0) root         (0)    11968 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_spp.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/tests/test_viz.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/version.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-05-23 00:38:04.000000 gridstatus-0.21.0/gridstatus/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      590 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-23 00:38:18.000000 gridstatus-0.21.0/gridstatus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3091 2023-05-23 00:38:04.000000 gridstatus-0.21.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 00:38:18.000000 gridstatus-0.21.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:38:18.000000 gridstatus-0.21.0/utils/ercot/
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-05-23 00:38:04.000000 gridstatus-0.21.0/utils/ercot/README.md
```

### Comparing `gridstatus-0.20.0/LICENSE` & `gridstatus-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/PKG-INFO` & `gridstatus-0.21.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatus
-Version: 0.20.0
+Version: 0.21.0
 Summary: API to access energy data
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -34,38 +34,38 @@
 License-File: LICENSE
 
 <p align="center">
 <img width=75% src="/gridstatus-header.png" alt="gridstatus logo" />
 </p>
 
 <p align="center">
-    <a href="https://github.com/kmax12/gridstatus/actions?query=branch%3Amain+workflow%3ATests" target="_blank">
+    <!-- disable until tests more reliable -->
+    <!-- <a href="https://github.com/kmax12/gridstatus/actions?query=branch%3Amain+workflow%3ATests" target="_blank">
         <img src="https://github.com/kmax12/gridstatus/workflows/Tests/badge.svg?branch=main" alt="Tests" />
-    </a>
+    </a> -->
     <a href="https://codecov.io/gh/kmax12/gridstatus" target="_blank">
         <img src="https://codecov.io/gh/kmax12/gridstatus/branch/main/graph/badge.svg" alt="Code Coverage"//>
     </a>
     <a href="https://badge.fury.io/py/gridstatus" target="_blank">
         <img src="https://badge.fury.io/py/gridstatus.svg?maxAge=2592000" alt="PyPI version">
     </a>
 </p>
 
 `gridstatus` is a Python library that provides a uniform API for accessing electricity supply, demand, and pricing data for the major Independent System Operators (ISOs) in the United States. It currently supports data from CAISO, SPP, ISONE, MISO, Ercot, NYISO, and PJM.
 
-
 ## GridStatus.io
 
 To preview some the data this library provide access to, visit [GridStatus.io](https://www.gridstatus.io/).
 
 ## Community
 
-* Need Help? Post a [GitHub issue](https://github.com/kmax12/gridstatus/issues) 
-* Want to chat? Join our [Slack](https://join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
-* Want to stay updated? Follow us on Twitter [@grid_status](https://twitter.com/grid_status)
-* Want to contribute? Read our [Contributing Guide](CONTRIBUTING.md)
+- Need Help? Post a [GitHub issue](https://github.com/kmax12/gridstatus/issues)
+- Want to chat? Join our [Slack](https://join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
+- Want to stay updated? Follow us on Twitter [@grid_status](https://twitter.com/grid_status)
+- Want to contribute? Read our [Contributing Guide](CONTRIBUTING.md)
 
 ## Installation
 
 `gridstatus` supports python 3.8+. Install with pip
 
 ```
 python -m pip install gridstatus
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gridstatus Version: 0.20.0 Summary: API to access
+Metadata-Version: 2.1 Name: gridstatus Version: 0.21.0 Summary: API to access
 energy data Author-email: Max Kanter
 gmail.com> Maintainer-email: Max Kanter
 gmail.com> License: Copyright 2022 James Max Kanter Redistribution and use in
 source and binary forms, with or without modification, are permitted provided
 that the following conditions are met: 1. Redistributions of source code must
 retain the above copyright notice, this list of conditions and the following
 disclaimer. 2. Redistributions in binary form must reproduce the above
@@ -27,26 +27,26 @@
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: <4,>=3.8 Description-
 Content-Type: text/markdown Provides-Extra: test Provides-Extra: dev Provides-
 Extra: docs License-File: LICENSE
                                [gridstatus logo]
-                                   [Tests] >
+                                        >
  [PyPI_version]
 `gridstatus` is a Python library that provides a uniform API for accessing
 electricity supply, demand, and pricing data for the major Independent System
 Operators (ISOs) in the United States. It currently supports data from CAISO,
 SPP, ISONE, MISO, Ercot, NYISO, and PJM. ## GridStatus.io To preview some the
 data this library provide access to, visit [GridStatus.io](https://
-www.gridstatus.io/). ## Community * Need Help? Post a [GitHub issue](https://
-github.com/kmax12/gridstatus/issues) * Want to chat? Join our [Slack](https://
+www.gridstatus.io/). ## Community - Need Help? Post a [GitHub issue](https://
+github.com/kmax12/gridstatus/issues) - Want to chat? Join our [Slack](https://
 join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
-* Want to stay updated? Follow us on Twitter [@grid_status](https://
-twitter.com/grid_status) * Want to contribute? Read our [Contributing Guide]
+- Want to stay updated? Follow us on Twitter [@grid_status](https://
+twitter.com/grid_status) - Want to contribute? Read our [Contributing Guide]
 (CONTRIBUTING.md) ## Installation `gridstatus` supports python 3.8+. Install
 with pip ``` python -m pip install gridstatus ``` Upgrade using the following
 command ``` python -m pip install --upgrade gridstatus ``` ## Documentation and
 Examples To learn more, visit the [documentation](https://docs.gridstatus.io/
 ) and view [example notebooks](https://docs.gridstatus.io/en/latest/Examples/
 index.html). ## Get Help We'd love to answer any usage or data access
 questions! Please let us know by posting a GitHub issue.
```

### Comparing `gridstatus-0.20.0/README.md` & `gridstatus-0.21.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 <p align="center">
 <img width=75% src="/gridstatus-header.png" alt="gridstatus logo" />
 </p>
 
 <p align="center">
-    <a href="https://github.com/kmax12/gridstatus/actions?query=branch%3Amain+workflow%3ATests" target="_blank">
+    <!-- disable until tests more reliable -->
+    <!-- <a href="https://github.com/kmax12/gridstatus/actions?query=branch%3Amain+workflow%3ATests" target="_blank">
         <img src="https://github.com/kmax12/gridstatus/workflows/Tests/badge.svg?branch=main" alt="Tests" />
-    </a>
+    </a> -->
     <a href="https://codecov.io/gh/kmax12/gridstatus" target="_blank">
         <img src="https://codecov.io/gh/kmax12/gridstatus/branch/main/graph/badge.svg" alt="Code Coverage"//>
     </a>
     <a href="https://badge.fury.io/py/gridstatus" target="_blank">
         <img src="https://badge.fury.io/py/gridstatus.svg?maxAge=2592000" alt="PyPI version">
     </a>
 </p>
 
 `gridstatus` is a Python library that provides a uniform API for accessing electricity supply, demand, and pricing data for the major Independent System Operators (ISOs) in the United States. It currently supports data from CAISO, SPP, ISONE, MISO, Ercot, NYISO, and PJM.
 
-
 ## GridStatus.io
 
 To preview some the data this library provide access to, visit [GridStatus.io](https://www.gridstatus.io/).
 
 ## Community
 
-* Need Help? Post a [GitHub issue](https://github.com/kmax12/gridstatus/issues) 
-* Want to chat? Join our [Slack](https://join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
-* Want to stay updated? Follow us on Twitter [@grid_status](https://twitter.com/grid_status)
-* Want to contribute? Read our [Contributing Guide](CONTRIBUTING.md)
+- Need Help? Post a [GitHub issue](https://github.com/kmax12/gridstatus/issues)
+- Want to chat? Join our [Slack](https://join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
+- Want to stay updated? Follow us on Twitter [@grid_status](https://twitter.com/grid_status)
+- Want to contribute? Read our [Contributing Guide](CONTRIBUTING.md)
 
 ## Installation
 
 `gridstatus` supports python 3.8+. Install with pip
 
 ```
 python -m pip install gridstatus
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
                                [gridstatus logo]
-                                   [Tests] >
+                                        >
  [PyPI_version]
 `gridstatus` is a Python library that provides a uniform API for accessing
 electricity supply, demand, and pricing data for the major Independent System
 Operators (ISOs) in the United States. It currently supports data from CAISO,
 SPP, ISONE, MISO, Ercot, NYISO, and PJM. ## GridStatus.io To preview some the
 data this library provide access to, visit [GridStatus.io](https://
-www.gridstatus.io/). ## Community * Need Help? Post a [GitHub issue](https://
-github.com/kmax12/gridstatus/issues) * Want to chat? Join our [Slack](https://
+www.gridstatus.io/). ## Community - Need Help? Post a [GitHub issue](https://
+github.com/kmax12/gridstatus/issues) - Want to chat? Join our [Slack](https://
 join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
-* Want to stay updated? Follow us on Twitter [@grid_status](https://
-twitter.com/grid_status) * Want to contribute? Read our [Contributing Guide]
+- Want to stay updated? Follow us on Twitter [@grid_status](https://
+twitter.com/grid_status) - Want to contribute? Read our [Contributing Guide]
 (CONTRIBUTING.md) ## Installation `gridstatus` supports python 3.8+. Install
 with pip ``` python -m pip install gridstatus ``` Upgrade using the following
 command ``` python -m pip install --upgrade gridstatus ``` ## Documentation and
 Examples To learn more, visit the [documentation](https://docs.gridstatus.io/
 ) and view [example notebooks](https://docs.gridstatus.io/en/latest/Examples/
 index.html). ## Get Help We'd love to answer any usage or data access
 questions! Please let us know by posting a GitHub issue.
```

### Comparing `gridstatus-0.20.0/docs/conf.py` & `gridstatus-0.21.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/docs/update_docs.py` & `gridstatus-0.21.0/docs/update_docs.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/gridstatus/__init__.py` & `gridstatus-0.21.0/gridstatus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from gridstatus.nyiso import NYISO
 from gridstatus.caiso import CAISO
 from gridstatus.ercot import Ercot
 from gridstatus.isone import ISONE
 from gridstatus.miso import MISO
 from gridstatus.spp import SPP
 from gridstatus.pjm import PJM
+from gridstatus.eia import EIA
 
 all_isos = [NYISO, CAISO, Ercot, ISONE, MISO, SPP, PJM]
 
 
 __all__ = [
     "NYISO",
     "CAISO",
```

### Comparing `gridstatus-0.20.0/gridstatus/base.py` & `gridstatus-0.21.0/gridstatus/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
 import requests
 
-from gridstatus.logging import log
+from gridstatus.gs_logging import log
 
 # TODO: this is needed to make SPP request work. restrict only to SPP
 requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS = "ALL:@SECLEVEL=1"
 
 # not supported exception
```

### Comparing `gridstatus-0.20.0/gridstatus/caiso.py` & `gridstatus-0.21.0/gridstatus/nyiso.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,301 +1,239 @@
-import io
-import time
-from contextlib import redirect_stderr
-from zipfile import ZipFile
-
 import pandas as pd
-import requests
-import tabula
 
+import gridstatus
 from gridstatus import utils
-from gridstatus.base import GridStatus, ISOBase, Markets, NotSupported
+from gridstatus.base import (
+    GridStatus,
+    InterconnectionQueueStatus,
+    ISOBase,
+    Markets,
+)
 from gridstatus.decorators import support_date_range
+from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
-from gridstatus.logging import log
-
-_BASE = "https://www.caiso.com/outlook/SP"
-_HISTORY_BASE = "https://www.caiso.com/outlook/SP/History"
-
-
-class CAISO(ISOBase):
-    """California Independent System Operator (CAISO)"""
-
-    name = "California ISO"
-    iso_id = "caiso"
-    default_timezone = "US/Pacific"
-
-    status_homepage = "https://www.caiso.com/TodaysOutlook/Pages/default.aspx"
-    interconnection_homepage = "https://rimspub.caiso.com/rimsui/logon.do"
-
-    # Markets PRC_INTVL_LMP, PRC_RTPD_LMP, PRC_LMP
-    markets = [
-        Markets.REAL_TIME_5_MIN,
-        Markets.REAL_TIME_15_MIN,
-        Markets.DAY_AHEAD_HOURLY,
-    ]
-
-    trading_hub_locations = [
-        "TH_NP15_GEN-APND",
-        "TH_SP15_GEN-APND",
-        "TH_ZP26_GEN-APND",
-    ]
-
-    def _current_day(self):
-        # get current date from stats api
-        return self.get_status(date="latest").time.date()
 
-    def get_stats(self, verbose=False):
-        stats_url = _BASE + "/stats.txt"
-        r = self._get_json(stats_url, verbose=verbose)
-        return r
-
-    def get_status(self, date="latest", verbose=False) -> str:
-        """Get Current Status of the Grid. Only date="latest" is supported
-
-        Known possible values: Normal, Restricted Maintenance Operations, Flex Alert
-        """
+ZONE = "zone"
+GENERATOR = "generator"
+"""NYISO offers LMP data at two locational granularities: \
+    load zone and point of generator interconnection"""
+
+
+class NYISO(ISOBase):
+    """New York Independent System Operator (NYISO)"""
+
+    name = "New York ISO"
+    iso_id = "nyiso"
+    default_timezone = "US/Eastern"
+    markets = [Markets.REAL_TIME_5_MIN, Markets.DAY_AHEAD_HOURLY]
+    status_homepage = "https://www.nyiso.com/system-conditions"
+    interconnection_homepage = "https://www.nyiso.com/interconnections"
 
+    @support_date_range(frequency="MONTH_START")
+    def get_status(self, date, end=None, verbose=False):
         if date == "latest":
-            # todo is it possible for this to return more than one element?
-            r = self.get_stats(verbose=verbose)
-
-            time = pd.to_datetime(r["slotDate"]).tz_localize("US/Pacific")
-            # can only store one value for status so we concat them together
-            status = ", ".join(r["gridstatus"])
-            reserves = r["Current_reserve"]
-
-            return GridStatus(time=time, status=status, reserves=reserves, iso=self)
-        else:
-            raise NotSupported()
+            latest = self._latest_from_today(self.get_status)
+            return GridStatus(
+                time=latest["time"],
+                status=latest["status"],
+                reserves=None,
+                iso=self,
+                notes=latest["notes"],
+            )
 
-    @support_date_range(frequency="1D")
-    def get_fuel_mix(self, date, start=None, end=None, verbose=False):
-        """Get fuel mix in 5 minute intervals for a provided day
+        status_df = self._download_nyiso_archive(
+            date=date,
+            end=end,
+            dataset_name="RealTimeEvents",
+            verbose=verbose,
+        )
 
-        Arguments:
-            date (datetime.date, str): "latest", "today", or an object
-                that can be parsed as a datetime for the day to return data.
+        status_df = status_df.rename(
+            columns={"Message": "Status"},
+        )
 
-            start (datetime.date, str): start of date range to return.
-                alias for `date` parameter.
-                Only specify one of `date` or `start`.
-
-            end (datetime.date, str): "today" or an object that can be parsed
-                as a datetime for the day to return data.
-                Only used if requesting a range of dates.
+        def _parse_status(row):
+            STATE_CHANGE = "**State Change. System now operating in "
 
-            verbose (bool, optional): print verbose output. Defaults to False.
+            row["Notes"] = None
+            if row["Status"] == "Start of day system state is NORMAL":
+                row["Notes"] = [row["Status"]]
+                row["Status"] = "Normal"
+            elif STATE_CHANGE in row["Status"]:
+                row["Notes"] = [row["Status"]]
+
+                row["Status"] = row["Status"][
+                    row["Status"].index(STATE_CHANGE)
+                    + len(STATE_CHANGE) : -len(" state.**")
+                ].capitalize()
+
+            return row
+
+        status_df = status_df.apply(_parse_status, axis=1)
+        status_df = status_df[["Time", "Status", "Notes"]]
+        return status_df
+
+    @support_date_range(frequency="MONTH_START")
+    def get_fuel_mix(self, date, end=None, verbose=False):
+        # note: this is simlar datastructure to pjm
 
-        Returns:
-            pandas.DataFrame: A DataFrame with columns - 'Time' and columns \
-                for each fuel type.
-        """
         if date == "latest":
-            mix = self.get_fuel_mix("today", verbose=verbose)
-            return mix.tail(1).reset_index(drop=True)
-
-        return self._get_historical_fuel_mix(date, verbose=verbose)
-
-    def _get_historical_fuel_mix(self, date, verbose=False):
-        df = _get_historical("fuelsource", date, verbose=verbose)
+            return (
+                self.get_fuel_mix(date="today", verbose=verbose)
+                .tail(1)
+                .reset_index(drop=True)
+            )
 
-        # rename some inconsistent columns names to standardize across dates
-        df = df.rename(
-            columns={
-                "Small hydro": "Small Hydro",
-                "Natural gas": "Natural Gas",
-                "Large hydro": "Large Hydro",
-            },
+        mix_df = self._download_nyiso_archive(
+            date=date,
+            end=end,
+            dataset_name="rtfuelmix",
+            verbose=verbose,
         )
 
-        # when day light savings time switches, there are na rows
-        df = df.dropna()
+        mix_df = mix_df.pivot_table(
+            index=["Time"],
+            columns="Fuel Category",
+            values="Gen MW",
+            aggfunc="first",
+        ).reset_index()
 
-        return df
+        mix_df.columns.name = None
 
-    @support_date_range(frequency="1D")
-    def get_load(self, date, end=None, verbose=False):
-        """Return load at a previous date in 5 minute intervals"""
+        return mix_df
 
-        if date == "latest":
-            # todo call today
-            load_url = _BASE + "/demand.csv"
-            df = pd.read_csv(load_url)
-
-            # get last non null row
-            data = df[~df["Current demand"].isnull()].iloc[-1]
-
-            return {
-                "time": _make_timestamp(data["Time"], self._current_day()),
-                "load": data["Current demand"],
-            }
-
-        return self._get_historical_load(date, verbose=verbose)
-
-    def _get_historical_load(self, date, verbose=False):
-        df = _get_historical("demand", date, verbose=verbose)
-
-        df = df[["Time", "Interval Start", "Interval End", "Current demand"]]
-        df = df.rename(columns={"Current demand": "Load"})
-        df = df.dropna(subset=["Load"])
-        return df
+    @support_date_range(frequency="MONTH_START")
+    def get_load(self, date, end=None, verbose=False):
+        """Returns load at a previous date in 5 minute intervals for
+          each zone and total load
 
-    @support_date_range(frequency="31D")
-    def get_load_forecast(self, date, end=None, sleep=4, verbose=False):
-        """Returns load forecast for a previous date in 1 hour intervals
+        Parameters:
+            date (str): Date to get load for. Can be "latest", "today", or
+              a date in the format YYYY-MM-DD
+            end (str): End date for date range. Optional.
+            verbose (bool): Whether to print verbose output. Optional.
 
-        Arguments:
-            date (datetime.date, pd.Timestamp, str): day to return.
-                If string, format should be YYYYMMDD e.g 20200623
-
-            sleep (int): number of seconds to sleep before returning to avoid
-                hitting rate limit in regular usage. Defaults to 5 seconds.
+        Returns:
+            pandas.DataFrame: Load data for NYISO and each zone
 
         """
+        if date == "latest":
+            return self._latest_from_today(self.get_load)
 
-        start, end = _caiso_handle_start_end(date, end)
-
-        url = (
-            "http://oasis.caiso.com/oasisapi/SingleZip?"
-            + "resultformat=6&queryname=SLD_FCST&version=1&market_run_id=DAM"
-            + f"&startdatetime={start}&enddatetime={end}"
+        data = self._download_nyiso_archive(
+            date=date,
+            end=end,
+            dataset_name="pal",
+            verbose=verbose,
         )
 
-        df = _get_oasis(url, verbose=verbose, sleep=sleep).rename(
-            columns={"MW": "Load Forecast"},
+        # pivot table
+        df = data.pivot_table(
+            index=["Time"],
+            columns="Name",
+            values="Load",
+            aggfunc="first",
         )
 
-        # returns many areas, we only want one overall iso
-        df = df[df["TAC_AREA_NAME"] == "CA ISO-TAC"]
-
-        df = df.sort_values("Time")
+        df.insert(0, "Load", df.sum(axis=1))
 
-        # todo - what is the actual time of the forecast?
-        df["Forecast Time"] = df["Time"].iloc[0]
-
-        df = df[
-            [
-                "Forecast Time",
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Load Forecast",
-            ]
-        ]
+        df.reset_index(inplace=True)
+        # drop NA loads
+        # data = data.dropna(subset=["Load"])
 
         return df
 
-    def get_pnodes(self):
-        url = "http://oasis.caiso.com/oasisapi/SingleZip?resultformat=6&queryname=ATL_PNODE_MAP&version=1&startdatetime=20220801T07:00-0000&enddatetime=20220802T07:00-0000&pnode_id=ALL"  # noqa
-        df = pd.read_csv(url, compression="zip").rename(
+    @support_date_range(frequency="MONTH_START")
+    def get_load_forecast(self, date, end=None, verbose=False):
+        """Get load forecast for a date in 1 hour intervals"""
+        date = utils._handle_date(date, self.default_timezone)
+
+        # todo optimize this to accept a date range
+        data = self._download_nyiso_archive(
+            date,
+            end=end,
+            dataset_name="isolf",
+            verbose=verbose,
+        )
+
+        data = data[
+            ["Time", "Interval Start", "Interval End", "File Date", "NYISO"]
+        ].rename(
             columns={
-                "APNODE_ID": "Aggregate PNode ID",
-                "PNODE_ID": "PNode ID",
+                "File Date": "Forecast Time",
+                "NYISO": "Load Forecast",
+                "Time": "Time",
             },
         )
-        return df
+
+        return data
 
     @lmp_config(
         supports={
-            Markets.DAY_AHEAD_HOURLY: ["latest", "today", "historical"],
-            Markets.REAL_TIME_15_MIN: ["latest", "today", "historical"],
             Markets.REAL_TIME_5_MIN: ["latest", "today", "historical"],
+            Markets.DAY_AHEAD_HOURLY: ["latest", "today", "historical"],
         },
     )
-    @support_date_range(frequency="31D")
+    @support_date_range(frequency="MONTH_START")
     def get_lmp(
         self,
         date,
-        market: str,
-        locations: list = None,
-        sleep: int = 5,
         end=None,
+        market: str = None,
+        locations: list = None,
+        location_type: str = None,
         verbose=False,
     ):
-        """Get LMP pricing starting at supplied date for a list of locations.
-
-        Arguments:
-            date (datetime.date, str): date to return data
-
-            market: market to return from. supports:
-
-            locations (list): list of locations to get data from.
-                If no locations are provided, defaults to NP15, SP15, and ZP26,
-                which are the trading hub locations. For a list of locations,
-                call ``CAISO.get_pnodes()``
-
-            sleep (int): number of seconds to sleep before returning to
-                avoid hitting rate limit in regular usage. Defaults to 5 seconds.
-
-        Returns:
-            pandas.DataFrame: A DataFrame of pricing data
+        """
+        Supported Markets:
+            - ``REAL_TIME_5_MIN``
+            - ``DAY_AHEAD_HOURLY``
+
+        Supported Location Types:
+            - ``zone``
+            - ``generator``
         """
         if date == "latest":
-            return self._latest_lmp_from_today(market=market, locations=locations)
+            return self._latest_lmp_from_today(
+                market=market,
+                locations=locations,
+                location_type=location_type,
+                verbose=verbose,
+            )
 
         if locations is None:
-            locations = self.trading_hub_locations
-
-        assert isinstance(locations, list), "locations must be a list"
+            locations = "ALL"
 
-        # todo make sure defaults to local timezone
-        start, end = _caiso_handle_start_end(date, end)
+        if location_type is None:
+            location_type = ZONE
 
-        if market == Markets.DAY_AHEAD_HOURLY:
-            query_name = "PRC_LMP"
-            market_run_id = "DAM"
-            version = 12
-            PRICE_COL = "MW"
-        elif market == Markets.REAL_TIME_15_MIN:
-            query_name = "PRC_RTPD_LMP"
-            market_run_id = "RTPD"
-            version = 3
-            PRICE_COL = "PRC"
-        elif market == Markets.REAL_TIME_5_MIN:
-            query_name = "PRC_INTVL_LMP"
-            market_run_id = "RTM"
-            version = 3
-            PRICE_COL = "VALUE"
-        else:
-            raise RuntimeError("LMP Market is not supported")
-
-        nodes_str = ",".join(locations)
-        url = f"http://oasis.caiso.com/oasisapi/SingleZip?resultformat=6&queryname={query_name}&version={version}&startdatetime={start}&enddatetime={end}&market_run_id={market_run_id}&node={nodes_str}"  # noqa
-
-        df = _get_oasis(
-            url,
+        marketname = self._set_marketname(market)
+        location_type = self._set_location_type(location_type)
+        filename = marketname + f"_{location_type}"
+
+        df = self._download_nyiso_archive(
+            date=date,
+            end=end,
+            dataset_name=marketname,
+            filename=filename,
             verbose=verbose,
-            sleep=sleep,
         )
 
-        df = df.pivot_table(
-            index=["Time", "Interval Start", "Interval End", "NODE"],
-            columns="LMP_TYPE",
-            values=PRICE_COL,
-            aggfunc="first",
-        )
+        columns = {
+            "Name": "Location",
+            "LBMP ($/MWHr)": "LMP",
+            "Marginal Cost Losses ($/MWHr)": "Loss",
+            "Marginal Cost Congestion ($/MWHr)": "Congestion",
+        }
 
-        df = df.reset_index().rename(
-            columns={
-                "NODE": "Location",
-                "LMP": "LMP",
-                "MCE": "Energy",
-                "MCC": "Congestion",
-                "MCL": "Loss",
-            },
-        )
+        df = df.rename(columns=columns)
 
+        df["Energy"] = df["LMP"] - (df["Loss"] - df["Congestion"])
         df["Market"] = market.value
-        df["Location Type"] = None
-
-        df.loc[
-            df["Location"].isin(self.trading_hub_locations),
-            "Location Type",
-        ] = "Trading Hub"
+        df["Location Type"] = "Zone" if location_type == ZONE else "Generator"
 
         df = df[
             [
                 "Time",
                 "Interval Start",
                 "Interval End",
                 "Market",
@@ -304,661 +242,591 @@
                 "LMP",
                 "Energy",
                 "Congestion",
                 "Loss",
             ]
         ]
 
-        data = utils.filter_lmp_locations(df, locations)
+        df = utils.filter_lmp_locations(df, locations)
 
-        # clean up pivot name in header
-        data.columns.name = None
-
-        return data
-
-    @support_date_range(frequency="1D")
-    def get_storage(self, date, verbose=False):
-        """Return storage charging or discharging for today in 5 minute intervals
-
-        Negative means charging, positive means discharging
-
-        Arguments:
-            date (datetime.date, str): date to return data
-        """
-        if date == "latest":
-            return self._latest_from_today(self.get_storage)
-
-        df = _get_historical("storage", date, verbose=verbose)
-
-        df = df.rename(
-            columns={
-                "Total batteries": "Supply",
-                "Stand-alone batteries": "Stand-alone Batteries",
-                "Hybrid batteries": "Hybrid Batteries",
-            },
-        )
-        df = df[
-            [
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Supply",
-                "Stand-alone Batteries",
-                "Hybrid Batteries",
-            ]
-        ]
         return df
 
-    @support_date_range(frequency="31D")
-    def get_gas_prices(
-        self,
-        date,
-        end=None,
-        fuel_region_id="ALL",
-        sleep=4,
-        verbose=False,
-    ):
-        """Return gas prices at a previous date
-
-        Arguments:
-            date (datetime.date, str): date to return data
-
-            end (datetime.date, str): last date of range to return data.
-                If None, returns only date. Defaults to None.
+    def get_interconnection_queue(self, verbose=False):
+        """Return NYISO interconnection queue
 
-            fuel_region_id(str, or list): single fuel region id or list of fuel
-                region ids to return data for. Defaults to ALL, which returns
-                all fuel regions.
+        Additional Non-NYISO queue info: https://www3.dps.ny.gov/W/PSCWeb.nsf/All/286D2C179E9A5A8385257FBF003F1F7E?OpenDocument
 
         Returns:
-            pandas.DataFrame: A DataFrame of gas prices
-        """
+            pandas.DataFrame: Interconnection queue containing, active, withdrawn, \
+                and completed project
 
-        start, end = _caiso_handle_start_end(date, end)
+        """  # noqa
 
-        if isinstance(fuel_region_id, list):
-            fuel_region_id = ",".join(fuel_region_id)
+        # 3 sheets - ['Interconnection Queue', 'Withdrawn', 'In Service']
+        # harded coded for now. perhaps this url can be parsed from the html here:
+        url = "https://www.nyiso.com/documents/20142/1407078/NYISO-Interconnection-Queue.xlsx"  # noqa
 
-        url = f"http://oasis.caiso.com/oasisapi/SingleZip?resultformat=6&queryname=PRC_FUEL&version=1&FUEL_REGION_ID={fuel_region_id}&startdatetime={start}&enddatetime={end}"  # noqa
+        msg = f"Downloading interconnection queue from {url}"
+        log(msg, verbose)
 
-        df = _get_oasis(url, verbose=verbose, sleep=sleep).rename(
-            columns={
-                "FUEL_REGION_ID": "Fuel Region Id",
-                "PRC": "Price",
-            },
+        all_sheets = pd.read_excel(
+            url,
+            sheet_name=["Interconnection Queue", "Withdrawn"],
         )
-        df = (
-            df.sort_values("Time")
-            .sort_values(
-                ["Fuel Region Id", "Time"],
+
+        # Drop extra rows at bottom
+        active = (
+            all_sheets["Interconnection Queue"]
+            .dropna(
+                subset=["Queue Pos.", "Project Name"],
             )
-            .reset_index(drop=True)
+            .copy()
         )
 
-        df = df[
-            [
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Fuel Region Id",
-                "Price",
-            ]
-        ]
-        return df
+        active["Status"] = InterconnectionQueueStatus.ACTIVE.value
 
-    @support_date_range(frequency="31D")
-    def get_ghg_allowance(
-        self,
-        date,
-        end=None,
-        sleep=4,
-        verbose=False,
-    ):
-        """Return ghg allowance at a previous date
+        withdrawn = all_sheets["Withdrawn"]
+        withdrawn["Status"] = InterconnectionQueueStatus.WITHDRAWN.value
+        # assume it was withdrawn when last updated
+        withdrawn["Withdrawn Date"] = withdrawn["Last Update"]
+        withdrawn["Withdrawal Comment"] = None
+        withdrawn = withdrawn.rename(columns={"Utility ": "Utility"})
 
-        Arguments:
-            date (datetime.date, str): date to return data
-
-            end (datetime.date, str): last date of range to return data.
-                If None, returns only date. Defaults to None.
-        """
-
-        start, end = _caiso_handle_start_end(date, end)
-
-        url = f"http://oasis.caiso.com/oasisapi/SingleZip?resultformat=6&queryname=PRC_GHG_ALLOWANCE&version=1&startdatetime={start}&enddatetime={end}"  # noqa
-
-        df = _get_oasis(url, verbose=verbose, sleep=sleep).rename(
-            columns={
-                "GHG_PRC_IDX": "GHG Allowance Price",
-            },
-        )
+        # make completed look like the other two sheets
+        completed = pd.read_excel(url, sheet_name="In Service", header=[0, 1])
+        completed.insert(15, "SGIA Tender Date", None)
+        completed.insert(16, "CY Complete Date", None)
+        completed.insert(17, "Proposed Initial-Sync Date", None)
 
-        df = df[
-            [
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "GHG Allowance Price",
-            ]
-        ]
+        completed["Status"] = InterconnectionQueueStatus.COMPLETED.value
 
-        return df
+        if (
+            "SGIA Tender Date" in active.columns
+            and "SGIA Tender Date" not in completed.columns
+        ):
+            active = active.drop(columns=["SGIA Tender Date"])
+        completed.columns = active.columns
 
-    def get_interconnection_queue(self, verbose=False):
-        url = "http://www.caiso.com/PublishedDocuments/PublicQueueReport.xlsx"
+        # the spreadsheet doesnt have a date, so make it null
+        completed["Proposed  In-Service"] = None
+        completed["Proposed COD"] = None
+        # assume it was finished when last updated
+        completed["Actual Completion Date"] = completed["Last Updated Date"]
 
-        msg = f"Downloading interconnection queue from {url}"
-        log(msg, verbose)
+        queue = pd.concat([active, withdrawn, completed])
 
-        sheets = pd.read_excel(url, skiprows=3, sheet_name=None)
+        # fix extra space in column name
 
-        # remove legend at the bottom
-        queued_projects = sheets["Grid GenerationQueue"][:-8]
-        completed_projects = sheets["Completed Generation Projects"][:-2]
-        withdrawn_projects = sheets["Withdrawn Generation Projects"][:-2].rename(
-            columns={"Project Name - Confidential": "Project Name"},
+        queue["Type/ Fuel"] = queue["Type/ Fuel"].map(
+            {
+                "S": "Solar",
+                "ES": "Energy Storage",
+                "W": "Wind",
+                "AC": "AC Transmission",
+                "DC": "DC Transmission",
+                "CT": "Combustion Turbine",
+                "CC": "Combined Cycle",
+                "M": "Methane",
+                #    "CR": "",
+                "H": "Hydro",
+                "L": "Load",
+                "ST": "Steam Turbine",
+                "CC-NG": "Natural Gas",
+                "FC": "Fuel Cell",
+                "PS": "Pumped Storage",
+                "NU": "Nuclear",
+                "D": "Dual Fuel",
+                #    "C": "",
+                "NG": "Natural Gas",
+                "Wo": "Wood",
+                "F": "Flywheel",
+                #    "CW": "",
+                "CC-D": "Combined Cycle - Dual Fuel",
+                "SW": "=Solid Waste",
+                #    "CR=CSR - ES + Solar": "",
+                "CT-NG": "Combustion Turbine - Natural Gas",
+                "DC/AC": "DC/AC Transmission",
+                "CT-D": "Combustion Turbine - Dual Fuel",
+                "CS-NG": "Steam Turbine & Combustion Turbine-  Natural Gas",
+                "ST-NG": "Steam Turbine - Natural Gas",
+            },
         )
 
-        queue = pd.concat(
-            [queued_projects, completed_projects, withdrawn_projects],
+        queue["Capacity (MW)"] = (
+            queue[["SP (MW)", "WP (MW)"]]
+            .replace(
+                "TBD",
+                0,
+            )
+            .replace(" ", 0)
+            .fillna(0)
+            .astype(float)
+            .max(axis=1)
         )
 
-        queue = queue.rename(
-            columns={
-                "Interconnection Request\nReceive Date": (
-                    "Interconnection Request Receive Date"
-                ),
-                "Actual\nOn-line Date": "Actual On-line Date",
-                "Current\nOn-line Date": "Current On-line Date",
-                "Interconnection Agreement \nStatus": (
-                    "Interconnection Agreement Status"
-                ),
-                "Study\nProcess": "Study Process",
-                "Proposed\nOn-line Date\n(as filed with IR)": (
-                    "Proposed On-line Date (as filed with IR)"
-                ),
-                "System Impact Study or \nPhase I Cluster Study": (
-                    "System Impact Study or Phase I Cluster Study"
-                ),
-                "Facilities Study (FAS) or \nPhase II Cluster Study": (
-                    "Facilities Study (FAS) or Phase II Cluster Study"
-                ),
-                "Optional Study\n(OS)": "Optional Study (OS)",
-            },
+        queue["Date of IR"] = pd.to_datetime(queue["Date of IR"])
+        queue["Proposed COD"] = pd.to_datetime(
+            queue["Proposed COD"],
+            errors="coerce",
         )
-
-        type_columns = ["Type-1", "Type-2", "Type-3"]
-        queue["Generation Type"] = queue[type_columns].apply(
-            lambda x: " + ".join(x.dropna()),
-            axis=1,
+        queue["Proposed  In-Service"] = pd.to_datetime(
+            queue["Proposed  In-Service"],
+            errors="coerce",
+        )
+        queue["Proposed Initial-Sync Date"] = pd.to_datetime(
+            queue["Proposed Initial-Sync Date"],
+            errors="coerce",
         )
 
+        # TODO handle other 2 sheets
+        # TODO they publish past queues,
+        # but not sure what data is in them that is relevant
+
         rename = {
-            "Queue Position": "Queue ID",
+            "Queue Pos.": "Queue ID",
             "Project Name": "Project Name",
-            "Generation Type": "Generation Type",
-            "Queue Date": "Queue Date",
             "County": "County",
             "State": "State",
-            "Application Status": "Status",
-            "Current On-line Date": "Proposed Completion Date",
-            "Actual On-line Date": "Actual Completion Date",
-            "Reason for Withdrawal": "Withdrawal Comment",
-            "Withdrawn Date": "Withdrawn Date",
+            "Owner/Developer": "Interconnecting Entity",
             "Utility": "Transmission Owner",
-            "Station or Transmission Line": "Interconnection Location",
-            "Net MWs to Grid": "Capacity (MW)",
+            "Interconnection Point": "Interconnection Location",
+            "Status": "Status",
+            "Date of IR": "Queue Date",
+            "Proposed COD": "Proposed Completion Date",
+            "Type/ Fuel": "Generation Type",
+            "Capacity (MW)": "Capacity (MW)",
+            "SP (MW)": "Summer Capacity (MW)",
+            "WP (MW)": "Winter Capacity (MW)",
         }
 
         extra_columns = [
-            "Type-1",
-            "Type-2",
-            "Type-3",
-            "Fuel-1",
-            "Fuel-2",
-            "Fuel-3",
-            "MW-1",
-            "MW-2",
-            "MW-3",
-            "Interconnection Request Receive Date",
-            "Interconnection Agreement Status",
-            "Study Process",
-            "Proposed On-line Date (as filed with IR)",
-            "System Impact Study or Phase I Cluster Study",
-            "Facilities Study (FAS) or Phase II Cluster Study",
-            "Optional Study (OS)",
-            "Full Capacity, Partial or Energy Only (FC/P/EO)",
-            "Off-Peak Deliverability and Economic Only",
-            "Feasibility Study or Supplemental Review",
+            "Proposed  In-Service",
+            "Proposed Initial-Sync Date",
+            "Last Updated Date",
+            "Z",
+            "S",
+            "Availability of Studies",
+            "SGIA Tender Date",
         ]
 
-        missing = [
-            "Interconnecting Entity",
-            "Summer Capacity (MW)",
-            "Winter Capacity (MW)",
-        ]
-
-        queue = utils.format_interconnection_df(
-            queue=queue,
-            rename=rename,
-            extra=extra_columns,
-            missing=missing,
-        )
+        queue = utils.format_interconnection_df(queue, rename, extra_columns)
 
         return queue
 
-    @support_date_range(frequency="1D")
-    def get_curtailment(self, date, verbose=False):
-        """Return curtailment data for a given date
-
-        Notes:
-            * requires java to be installed in order to run
-            * Data available from June 30, 2016 to present
+    def get_generators(self, verbose=False):
+        """Get a list of generators in NYISO
 
+        When possible return capacity and fuel type information
 
         Arguments:
-            date (datetime.date, str): date to return data
+            verbose (bool, optional): print out requested url. Defaults to False.
 
-            end (datetime.date, str): last date of range to return data.
-                If None, returns only date. Defaults to None.
+        Returns:
+            pandas.DataFrame: a DataFrame of generators and locations
 
-            verbose: print out url being fetched. Defaults to False.
+            **Possible Columns**
 
-        Returns:
-            pandas.DataFrame: A DataFrame of curtailment data
+            * Generator Name
+            * PTID
+            * Subzone
+            * Zone
+            * Latitude
+            * Longitude
+            * Owner, Operator, and / or Billing Organization
+            * Station Unit
+            * Town
+            * County
+            * State
+            * In-Service Date
+            * Name Plate Rating (V) MW
+            * 2022 CRIS MW Summer
+            * 2022 CRIS MW Winter
+            * 2022 Capability MW Summer
+            * 2022 Capability MW Winter
+            * Is Dual Fuel
+            * Unit Type
+            * Fuel Type 1
+            * Fuel Type 2
+            * 2021 Net Energy GWh
+            * Notes
+            * Generator Type
         """
 
-        # http://www.caiso.com/Documents/Wind_SolarReal-TimeDispatchCurtailmentReport02dec_2020.pdf
+        url = "http://mis.nyiso.com/public/csv/generator/generator.csv"
 
-        date_strs = [
-            date.strftime("%b%d_%Y"),
-            date.strftime(
-                "%d%b_%Y",
-            ).lower(),
-            date.strftime("-%b%d_%Y"),
-        ]
+        msg = f"Requesting {url}"
+        log(msg, verbose)
 
-        # handle specfic case where dec 02, 2021 has wrong year in file name
-        if date_strs[0] == "Dec02_2021":
-            date_strs = ["02dec_2020"]
-        if date_strs[0] == "Dec02_2020":
-            # this correct, so make sure we don't try the
-            # other file since 2021 is published wrong
-            date_strs = ["Dec02_2020"]
-
-        # todo handle not always just 4th pge
-
-        pdf = None
-        for date_str in date_strs:
-            url = f"http://www.caiso.com/Documents/Wind_SolarReal-TimeDispatchCurtailmentReport{date_str}.pdf"  # noqa: E501
+        df = pd.read_csv(url)
 
-            msg = f"Fetching URL: {url}"
-            log(msg, verbose)
+        # need to be updated once a year. approximately around end of april
+        # find it here: https://www.nyiso.com/gold-book-resources
+        capacity_url_2022 = "https://www.nyiso.com/documents/20142/30338270/2022-NYCA-Generators.xlsx/f0526021-37fd-2c27-94ee-14d0f31878c1"  # noqa
 
-            r = requests.get(url)
-            if b"404 - Page Not Found" in r.content:
-                continue
-            pdf = io.BytesIO(r.content)
-            break
+        msg = f"Requesting {url}"
+        log(msg, verbose)
 
-        if pdf is None:
-            raise ValueError(
-                "Could not find curtailment PDF for {}".format(date),
-            )
+        generators = pd.read_excel(
+            capacity_url_2022,
+            sheet_name=[
+                "Table III-2a",
+                "Table III-2b",
+            ],
+            skiprows=3,
+            header=[0, 1, 2, 3, 4],
+        )
 
-        with io.StringIO() as buf, redirect_stderr(buf):
-            try:
-                tables = tabula.read_pdf(pdf, pages="all")
-            except Exception:
-                print(buf.getvalue())
-                raise RuntimeError("Problem Reading PDF")
-
-        index_curtailment_table = list(
-            map(lambda df: "FUEL TYPE" in df.columns, tables),
-        ).index(True)
-        tables = tables[index_curtailment_table:]
-        if len(tables) == 0:
-            raise ValueError("No tables found")
-        elif len(tables) == 1:
-            df = tables[0]
-        else:
-            # this is case where there was a continuation of the
-            # curtailment table
-            # on a second page. there is no header,
-            # make parsed header of extra table the first row
-
-            def _handle_extra_table(extra_table):
-                extra_table = pd.concat(
-                    [
-                        extra_table.columns.to_frame().T.replace("Unnamed: 0", None),
-                        extra_table,
-                    ],
-                )
-                extra_table.columns = tables[0].columns
+        generators["Table III-2a"]["Generator Type"] = "Market Generator"
+        generators["Table III-2b"]["Generator Type"] = "Non-Market Generator"
 
-                return extra_table
+        # combined both sheets
+        generators = pd.concat(generators.values())
+
+        # manually transcribed column names
+        generators.columns = [
+            "LINE REF. NO.",
+            "Owner, Operator, and / or Billing Organization",
+            "Station Unit",
+            "Zone",
+            "PTID",
+            "Town",
+            "County",
+            "State",
+            "In-Service Date",
+            "Name Plate Rating (V) MW",
+            "2022 CRIS MW Summer",
+            "2022 CRIS MW Winter",
+            "2022 Capability MW Summer",
+            "2022 Capability MW Winter",
+            "Is Dual Fuel",
+            "Unit Type",
+            "Fuel Type 1",
+            "Fuel Type 2",
+            "2021 Net Energy GWh",
+            "Notes",
+            "Generator Type",
+        ]
+        generators = generators.dropna(subset=["PTID"])
 
-            extra_tables = [tables[0]] + [_handle_extra_table(t) for t in tables[1:]]
+        generators["PTID"] = generators["PTID"].astype(int)
 
-            df = pd.concat(extra_tables).reset_index()
+        # in other data
+        generators = generators.drop(columns=["Zone", "LINE REF. NO."])
 
-        rename = {
-            "DATE": "Date",
-            "HOU\rR": "Hour",
-            "HOUR": "Hour",
-            "CURT TYPE": "Curtailment Type",
-            "REASON": "Curtailment Reason",
-            "FUEL TYPE": "Fuel Type",
-            "CURTAILED MWH": "Curtailment (MWh)",
-            "CURTAILED\rMWH": "Curtailment (MWh)",
-            "CURTAILED MW": "Curtailment (MW)",
-            "CURTAILED\rMW": "Curtailment (MW)",
-        }
-
-        df = df.rename(columns=rename)
+        combined = pd.merge(df, generators, on=["PTID"], how="left")
 
-        # convert from hour ending to hour beginning
-        df["Hour"] = df["Hour"].astype(int) - 1
+        unit_type_map = {
+            "CC": "Combined Cycle",
+            "CG": "Cogeneration",
+            "CT": "Combustion Turbine Portion (CC)",
+            "CW": "Waste Heat Only (CC)",
+            "ES": "Energy Storage",
+            "FC": "Fuel Cell",
+            "GT": "Combustion Turbine",
+            "HY": "Conventional Hydro",
+            "IC": "Internal Combustion",
+            "JE": "Jet Engine",
+            "NB": "Steam (BWR Nuclear)",
+            "NP": "Steam (PWR Nuclear)",
+            "PS": "Pumped Storage Hydro",
+            "PV": "Photovoltaic",
+            "ST": "Steam Turbine (Fossil)",
+            "WT": "Wind Turbine",
+        }
+        combined["Unit Type"] = combined["Unit Type"].map(unit_type_map)
 
-        df["Time"] = df["Hour"].apply(
-            lambda x, date=date: date + pd.Timedelta(hours=x),
+        fuel_type_map = {
+            "BAT": "Battery",
+            "BUT": "Butane",
+            "FO2": "No. 2 Fuel Oil",
+            "FO4": "No. 4 Fuel Oil",
+            "FO6": "No. 6 Fuel Oil",
+            "FW": "Fly Wheel",
+            "JF": "Jet Fuel",
+            "KER": "Kerosene",
+            "MTE": "Methane (Bio Gas)",
+            "NG": "Natural Gas",
+            "OT": "Other (Describe In Footnote)",
+            "REF": "Refuse (Solid Waste)",
+            "SUN": "Sunlight",
+            "UR": "Uranium",
+            "WAT": "Water",
+            "WD": "Wood and/or Wood Waste",
+            "WND": "Wind",
+        }
+        combined["Fuel Type 1"] = combined["Fuel Type 1"].map(
+            fuel_type_map,
         )
-
-        df["Interval Start"] = df["Time"]
-        df["Interval End"] = df["Time"] + pd.Timedelta(hours=1)
-
-        df = df.drop(columns=["Date", "Hour"])
-
-        df["Fuel Type"] = df["Fuel Type"].map(
-            {
-                "SOLR": "Solar",
-                "WIND": "Wind",
-            },
+        combined["Fuel Type 2"] = combined["Fuel Type 2"].map(
+            fuel_type_map,
         )
 
-        df = df[
-            [
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Curtailment Type",
-                "Curtailment Reason",
-                "Fuel Type",
-                "Curtailment (MWh)",
-                "Curtailment (MW)",
-            ]
-        ]
+        combined["Is Dual Fuel"] = combined["Is Dual Fuel"] == "YES"
 
-        return df
+        state_code_map = {
+            36: "New York",
+            42: "Pennsylvania",
+            25: "Massachusetts",
+            34: "New Jersey",
+        }
+        combined["State"] = combined["State"].map(state_code_map)
 
-    @support_date_range(frequency="1D")
-    def get_as_prices(self, date, end=None, sleep=4, verbose=False):
-        """Return AS prices for a given date for each region
+        # todo map county codes to names. info on first sheet of excel
 
-        Arguments:
-            date (datetime.date, str): date to return data
+        return combined
 
-            end (datetime.date, str): last date of range to return data.
-                If None, returns only date. Defaults to None.
+    def get_loads(self, verbose=False):
+        """Get a list of loads in NYISO
 
-            verbose (bool, optional): print out url being fetched. Defaults to False.
+        Arguments:
+            verbose (bool, optional): print out requested url. Defaults to False.
 
         Returns:
-            pandas.DataFrame: A DataFrame of AS prices
+            pandas.DataFrame: a DataFrame of loads and locations
         """
 
-        start, end = _caiso_handle_start_end(date, end)
-
-        url = f"http://oasis.caiso.com/oasisapi/SingleZip?resultformat=6&queryname=PRC_AS&version=12&startdatetime={start}&enddatetime={end}&market_run_id=DAM&anc_type=ALL&anc_region=ALL"  # noqa
+        url = "http://mis.nyiso.com/public/csv/load/load.csv"
 
-        df = _get_oasis(url=url, verbose=verbose, sleep=sleep).rename(
-            columns={
-                "ANC_REGION": "Region",
-                "MARKET_RUN_ID": "Market",
-            },
-        )
+        msg = f"Requesting {url}"
+        log(msg, verbose)
 
-        as_type_map = {
-            "NR": "Non-Spinning Reserves",
-            "RD": "Regulation Down",
-            "RMD": "Regulation Mileage Down",
-            "RMU": "Regulation Mileage Up",
-            "RU": "Regulation Up",
-            "SR": "Spinning Reserves",
-        }
-        df["ANC_TYPE"] = df["ANC_TYPE"].map(as_type_map)
+        df = pd.read_csv(url)
 
-        df = df.pivot_table(
-            index=[
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Region",
-                "Market",
-            ],
-            columns="ANC_TYPE",
-            values="MW",
-        ).reset_index()
-
-        df = df.fillna(0)
+        return df
 
-        df.columns.name = None
+    def _set_marketname(self, market: Markets) -> str:
+        if market == Markets.REAL_TIME_5_MIN:
+            marketname = "realtime"
+        elif market == Markets.DAY_AHEAD_HOURLY:
+            marketname = "damlbmp"
+        else:
+            raise RuntimeError("LMP Market is not supported")
+        return marketname
 
-        return df
+    def _set_location_type(self, location_type: str) -> str:
+        location_types = [ZONE, GENERATOR]
+        if location_type == ZONE:
+            return ZONE
+        elif location_type == GENERATOR:
+            return "gen"
+        else:
+            raise ValueError(
+                f"Invalid location type. Expected one of: {location_types}",
+            )
 
-    @support_date_range(frequency="31D")
-    def get_as_procurement(
+    def _download_nyiso_archive(
         self,
         date,
         end=None,
-        market="DAM",
-        sleep=4,
+        dataset_name=None,
+        filename=None,
         verbose=False,
     ):
-        """Get ancillary services procurement data from CAISO.
+        """Download a dataset from NYISO's archive
 
         Arguments:
-            date (datetime.date, str): date to return data
-
-            end (datetime.date, str): last date of range to return data.
-                If None, returns only date. Defaults to None.
-
-            market: DAM or RTM. Defaults to DAM.
+            date (str or datetime): the date to download.
+                if end is provided, this is the start date
+            end (str or datetime):
+                the end date to download. if provided, date is the start date
+            dataset_name (str):
+                the name of the dataset to download
+            filename (str): the name of the file to download.
+                if not provided, dataset_name is used
+            verbose (bool): print out requested url
 
         Returns:
-            pandas.DataFrame: A DataFrame of ancillary services data
-        """
-        assert market in ["DAM", "RTM"], "market must be DAM or RTM"
-
-        start, end = _caiso_handle_start_end(date, end)
-
-        url = f"http://oasis.caiso.com/oasisapi/SingleZip?resultformat=6&queryname=AS_RESULTS&version=1&startdatetime={start}&enddatetime={end}&market_run_id={market}&anc_type=ALL&anc_region=ALL"  # noqa
-
-        df = _get_oasis(url=url, verbose=verbose, sleep=sleep).rename(
-            columns={
-                "ANC_REGION": "Region",
-                "MARKET_RUN_ID": "Market",
-            },
-        )
-
-        as_type_map = {
-            "NR": "Non-Spinning Reserves",
-            "RD": "Regulation Down",
-            "RMD": "Regulation Mileage Down",
-            "RMU": "Regulation Mileage Up",
-            "RU": "Regulation Up",
-            "SR": "Spinning Reserves",
-        }
-        df["ANC_TYPE"] = df["ANC_TYPE"].map(as_type_map)
-
-        result_type_map = {
-            "AS_BUY_MW": "Procured (MW)",
-            "AS_SELF_MW": "Self-Provided (MW)",
-            "AS_MW": "Total (MW)",
-            "AS_COST": "Total Cost",
-        }
-        df["RESULT_TYPE"] = df["RESULT_TYPE"].map(result_type_map)
-
-        df["column"] = df["ANC_TYPE"] + " " + df["RESULT_TYPE"]
-
-        df = df.pivot_table(
-            index=[
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Region",
-                "Market",
-            ],
-            columns="column",
-            values="MW",
-        ).reset_index()
-
-        df.columns.name = None
-
-        return df
-
-
-def _make_timestamp(time_str, today, timezone="US/Pacific"):
-    hour, minute = map(int, time_str.split(":"))
-    return pd.Timestamp(
-        year=today.year,
-        month=today.month,
-        day=today.day,
-        hour=hour,
-        minute=minute,
-        tz=timezone,
-    )
+            pandas.DataFrame: the downloaded data
 
+        """
+        if filename is None:
+            filename = dataset_name
 
-def _get_historical(file, date, verbose=False):
-    try:
-        date_str = date.strftime("%Y%m%d")
-        url = _HISTORY_BASE + "/%s/%s.csv" % (date_str, file)
-        msg = f"Fetching URL: {url}"
-        log(msg, verbose)
-    except Exception:
-        # fallback if today and no historical file yet
-        if utils.is_today(date, CAISO.default_timezone):
-            url = _BASE + "/%s.csv" % file
-            msg = f"Fetching URL: {url}"
+        date = gridstatus.utils._handle_date(date)
+        month = date.strftime("%Y%m01")
+        day = date.strftime("%Y%m%d")
+
+        # the last 7 days of file are hosted directly as csv
+        # todo this can probably be optimized to down single csv if
+        # a range and all files are in the last 7 days
+        if end is None and date > pd.Timestamp.now(
+            tz=self.default_timezone,
+        ).normalize() - pd.DateOffset(days=7):
+            csv_filename = f"{day}{filename}.csv"
+            csv_url = f"http://mis.nyiso.com/public/csv/{dataset_name}/{csv_filename}"
+            msg = f"Requesting {csv_url}"
             log(msg, verbose)
 
-    df = pd.read_csv(url)
-
-    # sometimes there are extra rows at the end, so this lets us ignore them
-    df = df.dropna(subset=["Time"])
-
-    df["Time"] = df["Time"].apply(
-        _make_timestamp,
-        today=date,
-        timezone="US/Pacific",
-    )
-
-    # sometimes returns midnight, which is technically the next day
-    # to be careful, let's check if that is the case before dropping
-    if df.iloc[-1]["Time"].hour == 0:
-        df = df.iloc[:-1]
-
-    # insert interval start/end columns
-    df.insert(1, "Interval Start", df["Time"])
-
-    # be careful if this is ever not 5 minutes
-    df.insert(2, "Interval End", df["Time"] + pd.Timedelta(minutes=5))
+            df = pd.read_csv(csv_url)
+            df = _handle_time(df, dataset_name)
+            df["File Date"] = date.normalize()
+        else:
+            zip_url = f"http://mis.nyiso.com/public/csv/{dataset_name}/{month}{filename}_csv.zip"  # noqa: E501
+            z = utils.get_zip_folder(zip_url, verbose=verbose)
 
-    return df
+            all_dfs = []
+            if end is None:
+                date_range = [date]
+            else:
+                date_range = pd.date_range(
+                    date.date(),
+                    end.date(),
+                    freq="1D",
+                    inclusive="both",
+                )
 
+            for d in date_range:
+                d = gridstatus.utils._handle_date(d)
+                month = d.strftime("%Y%m01")
+                day = d.strftime("%Y%m%d")
+
+                csv_filename = f"{day}{filename}.csv"
+                if csv_filename not in z.namelist():
+                    msg = f"{csv_filename} not found in {zip_url}"
+                    log(msg, verbose)
+                    continue
+                df = pd.read_csv(z.open(csv_filename))
+                df["File Date"] = d.normalize()
 
-def _get_oasis(url, verbose=False, sleep=4):
+                df = _handle_time(df, dataset_name)
+                all_dfs.append(df)
 
-    msg = f"Fetching URL: {url}"
-    log(msg, verbose)
+            df = pd.concat(all_dfs)
 
-    retry_num = 0
-    while retry_num < 3:
-        r = requests.get(url)
+        return df
 
-        if r.status_code == 200:
-            break
+    def get_capacity_prices(self, date=None, verbose=False):
+        """Pull the most recent capacity market report's market clearing prices
 
-        retry_num += 1
-        print(f"Failed to get data from CAISO. Error: {r.status_code}")
-        print(f"Retrying {retry_num}...")
-        time.sleep(5)
+        Arguments:
+            date (pandas.Timestamp): date that will be used to pull latest capacity
+                report (will refer to month and year)
 
-    z = ZipFile(io.BytesIO(r.content))
+            verbose (bool, optional): print out requested url. Defaults to False.
 
-    df = pd.read_csv(
-        z.open(z.namelist()[0]),
-    )
+        Returns:
+            a DataFrame of monthly capacity prices (all three auctions) for \
+                each of the four capacity localities within NYISO
+        """
+        if date is None:
+            date = pd.Timestamp.now(tz=self.default_timezone)
+        else:
+            date = utils._handle_date(date, tz=self.default_timezone)
 
-    if "INTERVALSTARTTIME_GMT" in df.columns:
-        df["INTERVALSTARTTIME_GMT"] = pd.to_datetime(
-            df["INTERVALSTARTTIME_GMT"],
-            utc=True,
-        ).dt.tz_convert(CAISO.default_timezone)
-
-        df["INTERVALENDTIME_GMT"] = pd.to_datetime(
-            df["INTERVALENDTIME_GMT"],
-            utc=True,
-        ).dt.tz_convert(CAISO.default_timezone)
+        if date.year == 2014:
+            year_code = 1410927
+        elif date.year == 2015:
+            year_code = 1410895
+        elif date.year == 2016:
+            year_code = 1410901
+        if date.year == 2017:
+            year_code = 1410883
+        if date.year == 2018:
+            year_code = 1410889
+        if date.year == 2019:
+            year_code = 4266869
+        elif date.year == 2020:
+            year_code = 10106066
+        elif date.year == 2021:
+            year_code = 18170164
+        elif date.year == 2022:
+            year_code = 27447313
+        elif date.year == 2023:
+            year_code = 35397361
+        else:
+            raise ValueError(
+                "Year not currently supported. Please file an issue.",
+            )
 
-        df.rename(
-            columns={
-                "INTERVALSTARTTIME_GMT": "Interval Start",
-                "INTERVALENDTIME_GMT": "Interval End",
-            },
-            inplace=True,
+            # todo: it looks like the "27447313" component of the base URL changes
+            # every year but I'm not sure what the link between that and the year
+            # is...
+        capacity_market_base_url = (
+            f"https://www.nyiso.com/documents/20142/{year_code}/ICAP-Market-Report"
         )
 
-        df.insert(0, "Time", df["Interval Start"])
-
-    # avoid rate limiting
-    time.sleep(5)
-
-    return df
-
-
-#  get Ancillary Services
-
+        url = f"{capacity_market_base_url}-{date.month_name()}-{date.year}.xlsx"
+        msg = f"Requesting {url}"
+        log(msg, verbose)
 
-def _caiso_handle_start_end(date, end):
-    start = date.tz_convert("UTC")
+        df = pd.read_excel(url, sheet_name="MCP Table", header=[0, 1])
 
-    if end:
-        end = end
-        end = end.tz_convert("UTC")
+        df.rename(columns={"Unnamed: 0_level_0": "", "Date": ""}, inplace=True)
+        df.set_index("", inplace=True)
+        return df.dropna(how="any", axis="columns")
+
+
+dataset_interval_map = {
+    # (time_type, interval_duration_minutes)
+    # load
+    "pal": ("instantaneous", None),
+    # fuel mix
+    "rtfuelmix": ("instantaneous", None),
+    # load forecast
+    "isolf": ("start", 60),
+    # dam lmp
+    "damlbmp": ("start", 60),
+    # rt lmp
+    "realtime": ("end", 5),
+    # real time events
+    "RealTimeEvents": ("instantaneous", None),
+}
+
+
+def _handle_time(df, dataset_name):
+    time_type, interval_duration_minutes = dataset_interval_map[dataset_name]
+
+    if "Time Stamp" in df.columns:
+        time_stamp_col = "Time Stamp"
+    elif "Timestamp" in df.columns:
+        time_stamp_col = "Timestamp"
+
+    def time_to_datetime(s, dst="infer"):
+        return pd.to_datetime(s).dt.tz_localize(
+            NYISO.default_timezone,
+            ambiguous=dst,
+        )
+
+    if "Time Zone" in df.columns:
+        dst = df["Time Zone"] == "EDT"
+        df[time_stamp_col] = time_to_datetime(
+            df[time_stamp_col],
+            dst,
+        )
+
+    elif "Name" in df.columns:
+        # once we group by name, the time series for each group is no longer ambiguous
+        df[time_stamp_col] = df.groupby("Name", group_keys=False)[time_stamp_col].apply(
+            time_to_datetime,
+            "infer",
+        )
     else:
-        end = start + pd.DateOffset(1)
-
-    start = start.strftime("%Y%m%dT%H:%M-0000")
-    end = end.strftime("%Y%m%dT%H:%M-0000")
-
-    return start, end
-
-
-if __name__ == "__main__":
-    import gridstatus
+        df[time_stamp_col] = time_to_datetime(
+            df[time_stamp_col],
+            "infer",
+        )
+
+    df = df.rename(columns={time_stamp_col: "Time"})
+
+    if time_type != "instantaneous":
+        interval_duration = pd.Timedelta(minutes=interval_duration_minutes)
+        if time_type == "start":
+            df["Interval Start"] = df["Time"]
+            df["Interval End"] = df["Interval Start"] + interval_duration
+        elif time_type == "end":
+            df["Interval Start"] = df["Time"] - interval_duration
+            df["Interval End"] = df["Time"]
+            df["Time"] = df["Interval Start"]
+
+        utils.move_cols_to_front(
+            df,
+            ["Time", "Interval Start", "Interval End"],
+        )
 
-    print("asd")
-    iso = gridstatus.CAISO()
+    return df
 
-    df = iso.get_curtailment(
-        start="2016-06-30",
-        end="today",
-        save_to="caiso_curtailment_2/",
-        verbose=True,
-    )
 
-    # check if any files are missing
-    import glob
+"""
+pricing data
 
-    files = glob.glob("caiso_curtailment/*.csv")
-    dates = (
-        pd.Series(
-            [pd.to_datetime(f[-12:-4]) for f in files],
-        )
-        .sort_values()
-        .to_frame()
-        .set_index(0, drop=False)
-    )
-    diffs = dates.diff()[0].dt.days
-    miss = diffs[diffs > 1]
+https://www.nyiso.com/en/energy-market-operational-data
+"""
```

### Comparing `gridstatus-0.20.0/gridstatus/decorators.py` & `gridstatus-0.21.0/gridstatus/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,20 @@
                 os.makedirs(save_to, exist_ok=True)
 
             error = "ignore"
             errors = []
             if "error" in args_dict:
                 error = args_dict.pop("error")
 
+            # if date is a tuple, then change to start and end
+            if "date" in args_dict and isinstance(args_dict["date"], tuple):
+                args_dict["start"] = args_dict["date"][0]
+                args_dict["end"] = args_dict["date"][1]
+                del args_dict["date"]
+
             if "date" in args_dict and "start" in args_dict:
                 raise ValueError(
                     "Cannot supply both 'date' and 'start' to function {}".format(
                         f,
                     ),
                 )
 
@@ -56,79 +62,100 @@
             if "start" in args_dict:
                 args_dict["date"] = args_dict["start"]
                 del args_dict["start"]
 
             if args_dict["date"] == "latest":
                 return f(*args, **kwargs)
 
-            if (
-                isinstance(args_dict["date"], str)
-                and args_dict["date"].lower() == "today"
-            ):
-                args_dict["date"] = pd.Timestamp.now(
-                    tz=args_dict["self"].default_timezone,
-                ).date()
-
             args_dict["date"] = gridstatus.utils._handle_date(
                 args_dict["date"],
                 args_dict["self"].default_timezone,
             )
 
             # no date range handling required
             if "end" not in args_dict:
                 df = f(**args_dict)
                 _handle_save_to(df, save_to, args_dict, f)
                 return df
-            else:
-                if (
-                    isinstance(args_dict["end"], str)
-                    and args_dict["end"].lower() == "today"
-                ):
-                    # add one day since end is exclusive
-                    args_dict["end"] = pd.Timestamp.now(
-                        tz=args_dict["self"].default_timezone,
-                    ).date() + pd.DateOffset(days=1)
 
-                args_dict["end"] = gridstatus.utils._handle_date(
-                    args_dict["end"],
-                    args_dict["self"].default_timezone,
-                )
+            if (
+                isinstance(args_dict["end"], str)
+                and args_dict["end"].lower() == "today"
+            ):
+                # add one day since end is exclusive
+                args_dict["end"] = pd.Timestamp.now(
+                    tz=args_dict["self"].default_timezone,
+                ).date() + pd.DateOffset(days=1)
 
-                assert (
-                    args_dict["end"] > args_dict["date"]
-                ), "End date {} must be after start date {}".format(
-                    args_dict["end"],
-                    args_dict["date"],
-                )
+            args_dict["end"] = gridstatus.utils._handle_date(
+                args_dict["end"],
+                args_dict["self"].default_timezone,
+            )
+
+            assert (
+                args_dict["end"] > args_dict["date"]
+            ), "End date {} must be after start date {}".format(
+                args_dict["end"],
+                args_dict["date"],
+            )
 
             # use .date() to remove timezone info, which doesnt matter
             # if just a date
 
+            # if frequency is callable, then use it to get the frequency
+            frequency = self.frequency
+            if callable(frequency):
+                frequency = self.frequency(args_dict)
+
             # Note: this may create a split that will end up
             # being unnecessary after running update dates below.
             # that is because after adding new dates, it's possible that two
             # ranges could be added.
             # Unnecessary optimization right now to include
             # logic to handle this
+
+            # if certain frequency, we need to handle first interval
+            # specially so pd.date_range works
+            prepend = []
+            if frequency == "DAY_START":
+                frequency = "1D"
+                next_day_start = args_dict["date"].ceil("1D")
+                if (
+                    next_day_start < args_dict["end"]
+                    and next_day_start != args_dict["date"]
+                ):
+                    prepend = [args_dict["date"]]
+                    args_dict["date"] = args_dict["date"].ceil("1D")
+            elif frequency == "MONTH_START":
+                frequency = "1M"
+                next_month_start = (
+                    args_dict["date"] + pd.offsets.MonthBegin(1)
+                ).normalize()
+                if (
+                    next_month_start < args_dict["end"]
+                    and next_month_start != args_dict["date"]
+                ):
+                    prepend = [args_dict["date"]]
+                    args_dict["date"] = next_month_start
+
             dates = pd.date_range(
-                args_dict["date"].date(),
-                args_dict["end"].date(),
-                freq=self.frequency,
+                args_dict["date"],
+                args_dict["end"],
+                freq=frequency,
                 inclusive="neither",
             )
-            dates = [args_dict["date"]] + dates.tolist() + [args_dict["end"]]
+            dates = prepend + [args_dict["date"]] + dates.tolist() + [args_dict["end"]]
 
             dates = [
                 gridstatus.utils._handle_date(
                     d,
                     args_dict["self"].default_timezone,
                 )
                 for d in dates
             ]
-
             # sometime api have restrictions/optimizations based on date ranges
             # update_dates allows for the caller to insert this logic
             if self.update_dates is not None:
                 dates = self.update_dates(dates, args_dict)
 
             start_date = dates[0]
 
@@ -151,15 +178,15 @@
                     if start_date is None:
                         start_date = end_date
                         continue
 
                     args_dict["date"] = start_date
 
                     # no need for end if we are querying for just 1 day
-                    if self.frequency != "1D":
+                    if frequency != "1D":
                         args_dict["end"] = end_date
 
                     try:
                         df = f(**args_dict)
                     except Exception as e:
                         if error == "raise":
                             raise e
```

### Comparing `gridstatus-0.20.0/gridstatus/ercot.py` & `gridstatus-0.21.0/gridstatus/ercot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import io
 from dataclasses import dataclass
 from zipfile import ZipFile
 
 import pandas as pd
 import requests
+import tqdm
 
 from gridstatus import utils
 from gridstatus.base import (
     GridStatus,
     InterconnectionQueueStatus,
     ISOBase,
     Markets,
     NotSupported,
 )
 from gridstatus.decorators import ercot_update_dates, support_date_range
+from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
-from gridstatus.logging import log
 
-LOCATION_TYPE_HUB = "HUB"
-LOCATION_TYPE_NODE = "NODE"
-LOCATION_TYPE_ZONE = "ZONE"
+LOCATION_TYPE_HUB = "Trading Hub"
+LOCATION_TYPE_RESOURCE_NODE = "Resource Node"
+LOCATION_TYPE_ZONE = "Load Zone"
 
 """
 Report Type IDs
 """
 # DAM Clearing Prices for Capacity
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP4-188-CD
 DAM_CLEARING_PRICES_FOR_CAPACITY_RTID = 12329
@@ -36,14 +37,18 @@
 # https://www.ercot.com/mp/data-products/data-product-details?id=PG7-200-ER
 GIS_REPORT_RTID = 15933
 
 # Historical RTM Load Zone and Hub Prices
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP6-785-ER
 HISTORICAL_RTM_LOAD_ZONE_AND_HUB_PRICES_RTID = 13061
 
+# Historical DAM Load Zone and Hub Prices
+# https://www.ercot.com/mp/data-products/data-product-details?id=NP4-180-ER
+HISTORICAL_DAM_LOAD_ZONE_AND_HUB_PRICES_RTID = 13060
+
 # Settlement Points List and Electrical Buses Mapping
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP4-160-SG
 SETTLEMENT_POINTS_LIST_AND_ELECTRICAL_BUSES_MAPPING_RTID = 10008
 
 # Settlement Point Prices at Resource Nodes, Hubs and Load Zones
 # https://www.ercot.com/mp/data-products/data-product-details?id=NP6-905-CD
 SETTLEMENT_POINT_PRICES_AT_RESOURCE_NODES_HUBS_AND_LOAD_ZONES_RTID = 12301
@@ -91,27 +96,29 @@
     markets = [
         Markets.REAL_TIME_15_MIN,
         Markets.DAY_AHEAD_HOURLY,
     ]
 
     location_types = [
         LOCATION_TYPE_HUB,
-        LOCATION_TYPE_NODE,
         LOCATION_TYPE_ZONE,
+        LOCATION_TYPE_RESOURCE_NODE,
     ]
 
     BASE = "https://www.ercot.com/api/1/services/read/dashboards"
     ACTUAL_LOADS_URL_FORMAT = "https://www.ercot.com/content/cdr/html/{timestamp}_actual_loads_of_forecast_zones.html"  # noqa
     LOAD_HISTORICAL_MAX_DAYS = 14
     AS_PRICES_HISTORICAL_MAX_DAYS = 30
 
     @dataclass
     class Document:
         url: str
         publish_date: pd.Timestamp
+        constructed_name: str
+        friendly_name: str
 
     def get_status(self, date, verbose=False):
         """Returns status of grid"""
         if date != "latest":
             raise NotSupported()
 
         r = self._get_json(self.BASE + "/daily-prc.json", verbose=verbose)
@@ -137,80 +144,85 @@
             notes=notes,
         )
 
     def get_fuel_mix(self, date, verbose=False):
         """Get fuel mix 5 minute intervals
 
         Arguments:
-            date (datetime.date, str): "latest", "today".
-                historical data currently not supported
+            date (datetime.date, str): "latest", "today",
+                and yesterday's date are supported.
 
             verbose(bool): print verbose output. Defaults to False.
 
         Returns:
             pandas.DataFrame: A DataFrame with columns; Time and columns for each fuel \
-                type (solar and wind)
+                type
         """
 
-        if date == "latest":
-            df = self.get_fuel_mix("today")
-            return df.tail(1).reset_index(drop=True)
-
-        # todo: can also support yesterday
-        elif utils.is_today(date, tz=self.default_timezone):
-            date = utils._handle_date(date, tz=self.default_timezone)
-            url = self.BASE + "/fuel-mix.json"
-            r = self._get_json(url, verbose=verbose)
-
-            today_str = date.strftime("%Y-%m-%d")
-            mix = (
-                pd.DataFrame(r["data"][today_str])
+        if date != "latest":
+            date_parsed = utils._handle_date(date, tz=self.default_timezone)
+            check_yesterday = date_parsed + pd.DateOffset(days=1)
+            if not (
+                utils.is_today(date, tz=self.default_timezone)
+                or utils.is_today(check_yesterday, tz=self.default_timezone)
+            ):
+                raise NotSupported()
+
+        url = self.BASE + "/fuel-mix.json"
+        data = self._get_json(url, verbose=verbose)
+
+        dfs = []
+        for day in data["data"].keys():
+            df = (
+                pd.DataFrame(data["data"][day])
                 .applymap(
                     lambda x: x["gen"],
                     na_action="ignore",
                 )
                 .T
             )
-            mix.index.name = "Interval End"
-            mix = mix.reset_index()
+            dfs.append(df)
 
-            mix["Interval End"] = pd.to_datetime(mix["Interval End"]).dt.tz_localize(
-                self.default_timezone,
-                ambiguous="infer",
-            )
+        mix = pd.concat(dfs)
+        mix.index.name = "Time"
+        mix = mix.reset_index()
+
+        mix["Time"] = pd.to_datetime(mix["Time"]).dt.tz_localize(
+            self.default_timezone,
+            ambiguous="infer",
+        )
+
+        # most timestamps are a few seconds off round 5 minute ticks
+        # round to nearest minute
+        mix["Time"] = mix["Time"].round("min")
 
-            # most timestamps are a few seconds off round 5 minute ticks
-            # round to nearest minute
-            mix["Interval End"] = mix["Interval End"].round("min")
-            mix["Interval Start"] = mix["Interval End"] - pd.Timedelta(minutes=5)
-            mix["Time"] = mix["Interval Start"]
-
-            mix = mix[
-                [
-                    "Time",
-                    "Interval Start",
-                    "Interval End",
-                    "Coal and Lignite",
-                    "Hydro",
-                    "Nuclear",
-                    "Power Storage",
-                    "Solar",
-                    "Wind",
-                    "Natural Gas",
-                    "Other",
-                ]
+        mix = mix[
+            [
+                "Time",
+                "Coal and Lignite",
+                "Hydro",
+                "Nuclear",
+                "Power Storage",
+                "Solar",
+                "Wind",
+                "Natural Gas",
+                "Other",
             ]
+        ]
 
+        if date == "latest":
             return mix
 
-        else:
-            raise NotSupported()
+        # return where date_parsed matches mix["Time"]
 
-    @support_date_range("1D")
-    def get_load(self, date, verbose=False):
+        return mix[mix["Time"].dt.date == date_parsed.date()].reset_index(drop=True)
+
+    @support_date_range("DAY_START")
+    def get_load(self, date, end=None, verbose=False):
+        """Get load for a date"""
         if date == "latest":
             today_load = self.get_load("today", verbose=verbose)
             latest = today_load.iloc[-1]
             return {"load": latest["Load"], "time": latest["Time"]}
 
         elif utils.is_today(date, tz=self.default_timezone):
             df = self._get_todays_outlook_non_forecast(date, verbose=verbose)
@@ -331,34 +343,78 @@
                 "Forecast Time",
                 "Load Forecast",
             ]
         ]
 
         return doc
 
-    def get_rtm_spp(self, year):
+    def get_rtm_spp(self, year, verbose=False):
         """Get Historical RTM Settlement Point Prices(SPPs)
             for each of the Hubs and Load Zones
 
         Arguments:
             year(int): year to get data for
+                Starting 2011, returns data for the entire year
 
         Source:
             https://www.ercot.com/mp/data-products/data-product-details?id=NP6-785-ER
         """  # noqa
         doc_info = self._get_document(
             report_type_id=HISTORICAL_RTM_LOAD_ZONE_AND_HUB_PRICES_RTID,
             constructed_name_contains=f"{year}.zip",
-            verbose=True,
+            verbose=verbose,
         )
 
-        x = utils.get_zip_file(doc_info.url)
+        x = utils.get_zip_file(doc_info.url, verbose=verbose)
         all_sheets = pd.read_excel(x, sheet_name=None)
         df = pd.concat(all_sheets.values())
-        return df
+
+        # fix parsing error where no data is present
+        # should only be 1 row per year
+        count = df[["Delivery Hour", "Delivery Interval"]].isnull().all(axis=1).sum()
+        if count == 1:
+            df = df.dropna(
+                subset=["Delivery Hour", "Delivery Interval"],
+                how="all",
+            )
+        elif count > 1:
+            raise ValueError(
+                "Parsing error, more than expected null rows found",
+            )
+
+        df["Delivery Interval"] = df["Delivery Interval"].astype("Int64")
+        df = self.parse_doc(df, verbose=verbose)
+        df["Market"] = Markets.REAL_TIME_15_MIN.value
+        return self._finalize_spp_df(df, verbose=verbose)
+
+    def get_dam_spp(self, year, verbose=False):
+        """Get Historical DAM Settlement Point Prices(SPPs)
+        for each of the Hubs and Load Zones
+
+        Arguments:
+            year(int): year to get data for.
+                Starting 2011, returns data for the entire year
+
+
+        Source:
+            https://www.ercot.com/mp/data-products/data-product-details?id=NP4-180-ER
+        """
+        doc_info = self._get_document(
+            report_type_id=HISTORICAL_DAM_LOAD_ZONE_AND_HUB_PRICES_RTID,
+            constructed_name_contains=f"{year}.zip",
+            verbose=verbose,
+        )
+
+        x = utils.get_zip_file(doc_info.url, verbose=verbose)
+        all_sheets = pd.read_excel(x, sheet_name=None)
+        df = pd.concat(all_sheets.values())
+        # filter where DSTFlag == 10
+        df = self.parse_doc(df, verbose=verbose)
+        df["Market"] = Markets.DAY_AHEAD_HOURLY.value
+        return self._finalize_spp_df(df, verbose=verbose)
 
     def get_interconnection_queue(self, verbose=False):
         """
         Get interconnection queue for ERCOT
 
         Monthly historical data available here:
             http://mis.ercot.com/misapp/GetReports.do?reportTypeId=15933&reportTitle=GIS%20Report&showHTMLView=&mimicKey
@@ -497,22 +553,22 @@
 
     @lmp_config(
         supports={
             Markets.REAL_TIME_15_MIN: ["latest", "today", "historical"],
             Markets.DAY_AHEAD_HOURLY: ["latest", "today", "historical"],
         },
     )
-    @support_date_range(frequency="1D")
+    @support_date_range(frequency="DAY_START")
     def get_spp(
         self,
         date,
         end=None,
         market: str = None,
         locations: list = "ALL",
-        location_type: str = LOCATION_TYPE_ZONE,
+        location_type: str = "ALL",
         verbose=False,
     ):
         """Get SPP data for ERCOT
 
         Supported Markets:
             - ``REAL_TIME_15_MIN``
             - ``DAY_AHEAD_HOURLY``
@@ -521,31 +577,102 @@
             - ``zone``
             - ``hub``
             - ``node``
         """
         if market == Markets.REAL_TIME_15_MIN:
             df = self._get_spp_rtm15(
                 date,
-                location_type,
                 verbose,
             )
-            settlement_point_field = "SettlementPointName"
         elif market == Markets.DAY_AHEAD_HOURLY:
-            df = self._get_spp_dam(date, location_type, verbose)
-            settlement_point_field = "SettlementPoint"
-        else:
-            raise NotSupported(
-                f"Market {market} not supported for ERCOT",
-            )
-        return Ercot._finalize_spp_df(df, settlement_point_field, locations)
+            df = self._get_spp_dam(date, verbose)
+
+        return self._finalize_spp_df(
+            df,
+            locations=locations,
+            location_type=location_type,
+            verbose=verbose,
+        )
+
+    def _finalize_spp_df(self, df, locations=None, location_type=None, verbose=False):
+        df = df.rename(
+            columns={
+                "SettlementPoint": "Location",
+                "Settlement Point": "Location",
+                "SettlementPointName": "Location",
+                "Settlement Point Name": "Location",
+            },
+        )
+
+        mapping_df = self._get_settlement_point_mapping(verbose=verbose)
+        resource_node = mapping_df["RESOURCE_NODE"].dropna().unique()
+
+        # if df[df.duplicated()].shape[0] > 0:
+        #     import pdb
+        #     pdb.set_trace()
+
+        # Create boolean masks for each location type
+        is_hub = df["Location"].str.startswith("HB_")
+        is_load_zone = df["Location"].str.startswith("LZ_")
+        is_resource_node = df["Location"].isin(resource_node)
+
+        # Assign location types based on the boolean masks
+        df.loc[is_hub, "Location Type"] = LOCATION_TYPE_HUB
+        df.loc[is_load_zone, "Location Type"] = LOCATION_TYPE_ZONE
+        df.loc[is_resource_node, "Location Type"] = LOCATION_TYPE_RESOURCE_NODE
+
+        # If a location type is not found, default to LOCATION_TYPE_RESOURCE_NODE
+        df["Location Type"].fillna(LOCATION_TYPE_RESOURCE_NODE, inplace=True)
+
+        df = df.rename(
+            columns={
+                "SettlementPointPrice": "SPP",
+                "Settlement Point Price": "SPP",
+            },
+        )
+
+        df = df[
+            [
+                "Time",
+                "Interval Start",
+                "Interval End",
+                "Location",
+                "Location Type",
+                "Market",
+                "SPP",
+            ]
+        ]
+
+        # todo figure out why
+        # when you get rid of SettlementPointType some
+        # rows are duplicated
+        # For example, SettlementPointType LZ and LZEW
+        df = df.drop_duplicates(
+            subset=[
+                "Time",
+                "Interval Start",
+                "Interval End",
+                "Location",
+            ],
+        )
+
+        df = utils.filter_lmp_locations(
+            df=df,
+            locations=locations,
+            location_type=location_type,
+        )
+
+        df = df.sort_values(by="Interval Start")
+        df = df.reset_index(drop=True)
+
+        return df
 
     def _get_spp_dam(
         self,
         date,
-        location_type: str = None,
         verbose=False,
     ):
         """Get day-ahead hourly Market SPP data for ERCOT"""
         if date == "latest":
             raise ValueError(
                 "DAM is released daily, so use date='today' instead",
             )
@@ -563,101 +690,69 @@
         msg = f"Fetching {doc_info.url}"
         log(msg, verbose)
 
         df = self.read_doc(doc_info, verbose=verbose)
 
         # fetch mapping
         df["Market"] = Markets.DAY_AHEAD_HOURLY.value
-        df["Location Type"] = self._get_location_type_name(location_type)
-
-        mapping_df = self._get_settlement_point_mapping(verbose=verbose)
-        df = self._filter_by_location_type(df, mapping_df, location_type)
 
         return df
 
-    @staticmethod
-    def _finalize_spp_df(df, settlement_point_field, locations):
-        """
-        Finalizes DataFrame by:
-        - filtering by locations list
-        - renaming and ordering columns
-        - and resetting the index
-
-        Arguments:
-            df (pandas.DataFrame): DataFrame with SPP data
-            settlement_point_field (str): Field name of
-                settlement point to rename to "Location"
-        """
-        df = df.rename(
-            columns={
-                "SettlementPointPrice": "SPP",
-                settlement_point_field: "Location",
-            },
-        )
-        df = utils.filter_lmp_locations(df, locations)
-        df = df[
-            [
-                "Time",
-                "Interval Start",
-                "Interval End",
-                "Location",
-                "Location Type",
-                "Market",
-                "SPP",
-            ]
-        ]
-        df = df.sort_values(by="Interval Start")
-        df = df.reset_index(drop=True)
-        return df
-
     def _get_spp_rtm15(
         self,
         date,
-        location_type: str = None,
         verbose=False,
     ):
         """Get Real-time 15-minute Market SPP data for ERCOT
 
         https://www.ercot.com/mp/data-products/data-product-details?id=NP6-905-CD
         """
-        today = pd.Timestamp.now(tz=self.default_timezone).normalize()
+        query_date = date
         if date == "latest":
-            publish_date = today
-        else:
-            publish_date = utils._handle_date(date, self.default_timezone)
+            query_date = utils._handle_date("today", self.default_timezone)
         # returns list of Document(url=,publish_date=)
-        docs = self._get_documents(
+
+        query_date_str = f"SPPHLZNP6905_{query_date.strftime('%Y%m%d')}"
+        all_docs = self._get_documents(
             report_type_id=SETTLEMENT_POINT_PRICES_AT_RESOURCE_NODES_HUBS_AND_LOAD_ZONES_RTID,
-            date=publish_date,
-            constructed_name_contains="csv.zip",
+            extension="csv",
             verbose=verbose,
         )
+
+        # look at file name to determine the
+        # date/interval the file represents
+        docs = []
+        for doc in all_docs:
+            if query_date_str + "_0000" in doc.constructed_name:
+                continue
+
+            if (
+                query_date_str in doc.constructed_name
+                or f"SPPHLZNP6905_{(query_date + pd.Timedelta(days=1)).strftime('%Y%m%d')}_0000"  # noqa: E501
+                in doc.constructed_name
+            ):
+                docs.append(doc)
+
         if date == "latest":
             # just pluck out the latest document based on publish_date
             docs = [max(docs, key=lambda x: x.publish_date)]
         if len(docs) == 0:
             raise ValueError(f"Could not fetch SPP data for {date}")
 
         all_dfs = []
-        for doc_info in docs:
+        for doc_info in tqdm.tqdm(docs, disable=not verbose):
             doc_url = doc_info.url
-
             msg = f"Fetching {doc_url}"
             log(msg, verbose)
             df = self.read_doc(doc_info, verbose=verbose)
             all_dfs.append(df)
+
         df = pd.concat(all_dfs).reset_index(drop=True)
-        df.drop
 
         df["Market"] = Markets.REAL_TIME_15_MIN.value
-        df["Location Type"] = self._get_location_type_name(location_type)
-        # Additional filter as the document may contain the last 15 minutes of yesterday
-        df = df[df["Interval Start"].dt.date == publish_date.date()]
-        df = self._filter_by_settlement_point_type(df, location_type)
-
         return df
 
     @support_date_range(frequency="1Y", update_dates=ercot_update_dates)
     def get_as_prices(
         self,
         date,
         end=None,
@@ -686,15 +781,14 @@
         if (
             date.date()
             >= (
                 pd.Timestamp.now(tz=self.default_timezone)
                 - pd.DateOffset(days=self.AS_PRICES_HISTORICAL_MAX_DAYS)
             ).date()
         ):
-
             return self._get_as_prices_recent(date, end=end)
         elif not end:
             end = date
 
         doc_info = self._get_document(
             report_type_id=HISTORICAL_DAM_CLEARING_PRICES_FOR_CAPACITY_RTID,
             constructed_name_contains=f"{date.year}.zip",
@@ -730,15 +824,15 @@
             .reset_index(drop=True)
         )
 
         print(data)
 
         return data
 
-    @support_date_range("1D")
+    @support_date_range("DAY_START")
     def _get_as_prices_recent(self, date, verbose=False):
         """Get ancillary service clearing prices in hourly intervals in Day
             Ahead Market. This function is can return the last 31 days
             of ancillary pricing.
 
         Arguments:
             date (datetime.date, str): date of delivery for AS services
@@ -842,14 +936,15 @@
         return max(documents, key=lambda x: x.publish_date)
 
     def _get_documents(
         self,
         report_type_id,
         date=None,
         constructed_name_contains=None,
+        extension=None,
         verbose=False,
     ) -> list:
         """Searches by Report Type ID, filtering for date and/or constructed name
 
         Returns:
             list of Document with URL and Publish Date
         """
@@ -866,27 +961,32 @@
             publish_date = pd.Timestamp(doc["Document"]["PublishDate"]).tz_convert(
                 self.default_timezone,
             )
 
             if date:
                 match = match and publish_date.date() == date.date()
 
+            if extension:
+                match = match and doc["Document"]["FriendlyName"].endswith(extension)
+
             if constructed_name_contains:
                 match = (
                     match
                     and constructed_name_contains in doc["Document"]["ConstructedName"]
                 )
 
             if match:
                 doc_id = doc["Document"]["DocID"]
                 url = f"https://www.ercot.com/misdownload/servlets/mirDownload?doclookupId={doc_id}"  # noqa
                 matches.append(
                     self.Document(
                         url=url,
                         publish_date=publish_date,
+                        constructed_name=doc["Document"]["ConstructedName"],
+                        friendly_name=doc["Document"]["FriendlyName"],
                     ),
                 )
 
         return matches
 
     def _handle_json_data(self, df, columns):
         df["Time"] = (
@@ -911,42 +1011,14 @@
         cols_to_keep = [
             "Time",
             "Interval Start",
             "Interval End",
         ] + list(columns.keys())
         return df[cols_to_keep].rename(columns=columns)
 
-    def _filter_by_settlement_point_type(self, df, location_type):
-        """Filter by settlement point type"""
-        norm_location_type = location_type.upper()
-        if norm_location_type == LOCATION_TYPE_NODE:
-            df = df[
-                df["SettlementPointType"].isin(
-                    RESOURCE_NODE_SETTLEMENT_TYPES,
-                )
-            ]
-        elif norm_location_type == LOCATION_TYPE_ZONE:
-            df = df[df["SettlementPointType"].isin(LOAD_ZONE_SETTLEMENT_TYPES)]
-        elif norm_location_type == LOCATION_TYPE_HUB:
-            df = df[df["SettlementPointType"].isin(HUB_SETTLEMENT_TYPES)]
-        else:
-            raise ValueError(f"Invalid location_type: {location_type}")
-        return df
-
-    def _get_location_type_name(self, location_type):
-        norm_location_type = location_type.upper()
-        if norm_location_type == LOCATION_TYPE_NODE:
-            return "Node"
-        elif norm_location_type == LOCATION_TYPE_ZONE:
-            return "Zone"
-        elif norm_location_type == LOCATION_TYPE_HUB:
-            return "Hub"
-        else:
-            raise ValueError(f"Invalid location_type: {location_type}")
-
     def _get_settlement_point_mapping(self, verbose=False):
         """Get DataFrame whose columns can help us filter out values"""
 
         doc_info = self._get_document(
             report_type_id=SETTLEMENT_POINTS_LIST_AND_ELECTRICAL_BUSES_MAPPING_RTID,
             verbose=verbose,
         )
@@ -960,101 +1032,93 @@
         names = z.namelist()
         settlement_points_file = [
             name for name in names if "Settlement_Points" in name
         ][0]
         df = pd.read_csv(z.open(settlement_points_file))
         return df
 
-    def _filter_by_location_type(self, df, mapping_df, location_type):
-        """Filter by location type"""
-        norm_location_type = location_type.upper()
-        if norm_location_type == LOCATION_TYPE_NODE:
-            valid_values = mapping_df["RESOURCE_NODE"].unique()
-        elif norm_location_type == LOCATION_TYPE_ZONE:
-            valid_values = mapping_df["SETTLEMENT_LOAD_ZONE"].unique()
-        elif norm_location_type == LOCATION_TYPE_HUB:
-            valid_values = mapping_df["HUB"].unique()
-        else:
-            raise ValueError(f"Invalid location_type: {location_type}")
-
-        return df[df["SettlementPoint"].isin(valid_values)]
-
     def read_doc(self, doc, verbose=False):
         doc = pd.read_csv(doc.url, compression="zip")
+        return self.parse_doc(doc, verbose=verbose)
 
+    def parse_doc(self, doc, verbose=False):
         # files sometimes have different naming conventions
         # a more elegant solution would be nice
         doc.rename(
             columns={
                 "Delivery Date": "DeliveryDate",
                 "Hour Ending": "HourEnding",
                 "Repeated Hour Flag": "DSTFlag",
                 "DeliveryHour": "HourEnding",
+                "Delivery Hour": "HourEnding",
+                "Delivery Interval": "DeliveryInterval",
                 # fix whitespace in column name
                 "DSTFlag    ": "DSTFlag",
             },
             inplace=True,
         )
 
         original_cols = doc.columns.tolist()
 
         # i think DeliveryInterval only shows up
         # in 15 minute data along with DeliveryHour
         if "DeliveryInterval" in original_cols:
             interval_length = pd.Timedelta(minutes=15)
-            doc["Interval End"] = (
+
+            doc["HourBeginning"] = doc["HourEnding"] - 1
+
+            doc["Interval Start"] = (
                 pd.to_datetime(doc["DeliveryDate"])
-                + doc["HourEnding"].astype("timedelta64[h]")
-                + (doc["DeliveryInterval"] * interval_length)
+                + doc["HourBeginning"].astype("timedelta64[h]")
+                + ((doc["DeliveryInterval"] - 1) * interval_length)
             )
 
         else:
             interval_length = pd.Timedelta(hours=1)
-            doc["Interval End"] = pd.to_datetime(doc["DeliveryDate"]) + (
-                doc["HourEnding"].str.split(":").str[0].astype(int)
-            ).astype("timedelta64[h]")
-
-            # if there is a DST skip, add an hour to the previous row
-            # for example, data has 2022-03-13 02:00:00,
-            # but that should be 2022-03-13 03:00:00
-            dst_skip_hour = doc[doc["Interval End"].diff() == pd.Timedelta(hours=2)]
-            for i in dst_skip_hour.index:
-                doc.loc[i - 1, "Interval End"] = doc.loc[
-                    i - 1,
-                    "Interval End",
-                ] + pd.DateOffset(
-                    hours=1,
-                )  # noqa
+            doc["HourBeginning"] = (
+                doc["HourEnding"]
+                .astype(str)
+                .str.split(
+                    ":",
+                )
+                .str[0]
+                .astype(int)
+                - 1
+            )
+            doc["Interval Start"] = pd.to_datetime(doc["DeliveryDate"]) + doc[
+                "HourBeginning"
+            ].astype("timedelta64[h]")
 
-        doc["Interval End"] = doc["Interval End"].dt.tz_localize(
+        doc["Interval Start"] = doc["Interval Start"].dt.tz_localize(
             self.default_timezone,
             ambiguous=doc["DSTFlag"] == "Y",
         )
 
-        doc["Interval Start"] = doc["Interval End"] - interval_length
+        doc["Interval End"] = doc["Interval Start"] + interval_length
+
         doc["Time"] = doc["Interval Start"]
 
         cols_to_keep = [
             "Time",
             "Interval Start",
             "Interval End",
         ] + original_cols
 
         # todo try to clean up this logic
         doc = doc[cols_to_keep]
-        doc.drop(
+        doc = doc.drop(
             columns=[
                 "DeliveryDate",
                 "HourEnding",
                 "DSTFlag",
             ],
-            inplace=True,
         )
         if "DeliveryInterval" in doc.columns:
-            doc.drop(columns=["DeliveryInterval"], inplace=True)
+            doc = doc.drop(columns=["DeliveryInterval"])
 
         return doc
 
 
 if __name__ == "__main__":
     iso = Ercot()
-    iso.get_fuel_mix("latest")
+
+    df = iso.get_rtm_spp(2011)
```

### Comparing `gridstatus-0.20.0/gridstatus/isone.py` & `gridstatus-0.21.0/gridstatus/isone.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     GridStatus,
     InterconnectionQueueStatus,
     ISOBase,
     Markets,
     NotSupported,
 )
 from gridstatus.decorators import support_date_range
+from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
-from gridstatus.logging import log
 
 
 class ISONE(ISOBase):
     """ISO New England (ISONE)"""
 
     name = "ISO New England"
     iso_id = "isone"
@@ -99,15 +99,15 @@
     #     # todo has marginal flag
     #     mix_df = mix_df.set_index("FuelCategory")[
     #         ["GenMw"]].T.reset_index(drop=True)
     #     mix_df.insert(0, "Time", time)
     #     mix_df.columns.name = None
     #     return mix_df
 
-    @support_date_range(frequency="1D")
+    @support_date_range(frequency="DAY_START")
     def get_fuel_mix(self, date, end=None, verbose=False):
         """Return fuel mix at a previous date
 
         Provided at frequent, but irregular intervals by ISONE
         """
         if date == "latest":
             return (
@@ -136,51 +136,29 @@
             index="Date",
             columns="Fuel Category",
             values="Gen Mw",
             aggfunc="first",
         ).reset_index()
         mix_df.columns.name = None
 
-        # assume interval end. unclear based on data
-        mix_df = mix_df.rename(columns={"Date": "Interval End"})
+        # assume instant in time, unclear if this is correct
+        mix_df = mix_df.rename(columns={"Date": "Time"})
 
         mix_df = mix_df.fillna(0)
 
-        mix_df["Interval Start"] = (
-            mix_df["Interval End"] - mix_df["Interval End"].diff()
-        )
-
-        # add midnight to first row of Interval Start
-        mix_df.loc[0, "Interval Start"] = mix_df["Interval Start"].min().normalize()
-
-        # if historical data, add row at end to go to midnight of next day
-        # todo manually verified works, but add test for this
-        if not utils.is_today(date, self.default_timezone):
-            new_row = pd.DataFrame(
-                {
-                    "Interval Start": [mix_df["Interval End"].max()],
-                    "Interval End": [
-                        mix_df["Interval End"].max().normalize() + pd.Timedelta(days=1),
-                    ],
-                },
-            )
-            mix_df = pd.concat([mix_df, new_row], ignore_index=True).ffill()
-
-        mix_df["Time"] = mix_df["Interval Start"]
-
         # move time columns front
         mix_df = utils.move_cols_to_front(
             mix_df,
-            ["Time", "Interval Start", "Interval End"],
+            ["Time"],
         )
 
         return mix_df
 
-    @support_date_range(frequency="1D")
-    def get_load(self, date, verbose=False):
+    @support_date_range(frequency="DAY_START")
+    def get_load(self, date, end=None, verbose=False):
         """Return load at a previous date in 5 minute intervals"""
         # todo document the earliest supported date
         # supports a start and end date
         if date == "latest":
             return self._latest_from_today(self.get_load)
 
         date_str = date.strftime("%Y%m%d")
@@ -200,57 +178,40 @@
         df["Interval Start"] = df["Time"]
         df["Interval End"] = df["Time"] + pd.Timedelta(minutes=5)
 
         df = df[["Time", "Interval Start", "Interval End", "Load"]]
 
         return df
 
-    @support_date_range(frequency="1D")
-    def get_load_forecast(self, date, end=None, verbose=False):
-        """Return forecast at a previous date"""
-        start_str = date.strftime("%m/%d/%Y")
-        end_str = (date + pd.Timedelta(days=1)).strftime("%m/%d/%Y")
-        data = {
-            "_nstmp_startDate": start_str,
-            "_nstmp_endDate": end_str,
-            "_nstmp_twodays": True,
-            "_nstmp_twodaysCheckbox": False,
-            "_nstmp_requestType": "systemload",
-            "_nstmp_forecast": True,
-            "_nstmp_actual": False,
-            "_nstmp_cleared": False,
-            "_nstmp_priorDay": False,
-            "_nstmp_inclPumpLoad": True,
-            "_nstmp_inclBtmPv": True,
-        }
-
-        data = _make_wsclient_request(
-            url="https://www.iso-ne.com/ws/wsclient",
-            data=data,
+    @support_date_range(frequency="DAY_START")
+    def get_btm_solar(self, date, end=None, verbose=False):
+        """Return BTM solar at a previous date in 5 minute intervals"""
+        df = self._get_system_load(
+            date,
+            end=date,
+            series="actual",
             verbose=verbose,
         )
 
-        data = pd.DataFrame(data[0]["data"]["forecast"])
+        df["BTM Solar"] = df["NativeLoadBtmPv"] - df["Load"]
 
-        # must convert this way rather than use pd.to_datetime
-        # to handle DST transitions
-        data["BeginDate"] = data["BeginDate"].apply(
-            lambda x: pd.Timestamp(x).tz_convert(ISONE.default_timezone),
-        )
+        df["Interval Start"] = df["Time"]
+        df["Interval End"] = df["Time"] + pd.Timedelta(minutes=5)
 
-        data["CreationDate"] = data["BeginDate"].apply(
-            lambda x: pd.Timestamp(x).tz_convert(ISONE.default_timezone),
-        )
+        return df[["Time", "Interval Start", "Interval End", "BTM Solar"]]
 
-        df = data[["CreationDate", "BeginDate", "Mw"]].rename(
-            columns={
-                "CreationDate": "Forecast Time",
-                "BeginDate": "Time",
-                "Mw": "Load Forecast",
-            },
+    @support_date_range(frequency="DAY_START")
+    def get_load_forecast(self, date, end=None, verbose=False):
+        """Return forecast at a previous date"""
+
+        df = self._get_system_load(
+            date,
+            end=date + pd.Timedelta(days=1),
+            series="forecast",
+            verbose=verbose,
         )
 
         df["Interval Start"] = df["Time"]
         df["Interval End"] = df["Time"] + pd.Timedelta(hours=1)
 
         df = df[
             [
@@ -311,15 +272,15 @@
     @lmp_config(
         supports={
             Markets.REAL_TIME_5_MIN: ["latest", "today", "historical"],
             Markets.REAL_TIME_HOURLY: ["latest", "today", "historical"],
             Markets.DAY_AHEAD_HOURLY: ["today", "historical"],
         },
     )
-    @support_date_range(frequency="1D")
+    @support_date_range(frequency="DAY_START")
     def get_lmp(
         self,
         date,
         end=None,
         market: str = None,
         locations: list = None,
         include_id=False,
@@ -633,14 +594,68 @@
         queue = queue.sort_values(
             "Queue ID",
             ascending=False,
         ).reset_index(drop=True)
 
         return queue
 
+    def _get_system_load(self, date, end, series, verbose=False):
+        start_str = date.strftime("%m/%d/%Y")
+        end_str = end.strftime("%m/%d/%Y")
+        params = {
+            "_nstmp_startDate": start_str,
+            "_nstmp_endDate": end_str,
+            "_nstmp_twodays": True,
+            "_nstmp_twodaysCheckbox": False,
+            "_nstmp_requestType": "systemload",
+            "_nstmp_forecast": True,
+            "_nstmp_actual": True,
+            "_nstmp_cleared": True,
+            "_nstmp_priorDay": False,
+            "_nstmp_inclPumpLoad": True,
+            "_nstmp_inclBtmPv": True,
+        }
+
+        raw_data = _make_wsclient_request(
+            url="https://www.iso-ne.com/ws/wsclient",
+            data=params,
+            verbose=verbose,
+        )
+
+        data = pd.DataFrame(raw_data[0]["data"][series])
+
+        # must convert this way rather than use pd.to_datetime
+        # to handle DST transitions
+        data["BeginDate"] = data["BeginDate"].apply(
+            lambda x: pd.Timestamp(x).tz_convert(ISONE.default_timezone),
+        )
+
+        # for times earlier this creation date is after the forecasted interval
+        # for all historical data
+        if "CreationDate" in data.columns:
+            data["CreationDate"] = data["CreationDate"].apply(
+                lambda x: pd.Timestamp(x).tz_convert(ISONE.default_timezone),
+            )
+        if series == "actual":
+            mw_rename = "Load"
+        elif series == "forecast":
+            mw_rename = "Load Forecast"
+        else:
+            raise ValueError(f"Unrecognized series: {series}")
+
+        data = data.rename(
+            columns={
+                "BeginDate": "Time",
+                "Mw": mw_rename,
+                "CreationDate": "Forecast Time",
+            },
+        )
+
+        return data
+
 
 def _make_request(url, skiprows, verbose):
     attempt = 0
     while attempt < 3:
         with requests.Session() as s:
             # make first get request to get cookies set
             s.get(
```

### Comparing `gridstatus-0.20.0/gridstatus/lmp_config.py` & `gridstatus-0.21.0/gridstatus/lmp_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 
     @staticmethod
     def _parse_date(date, tz):
         """Parse date to pd.Timestamp,
         to be used later on for validation"""
         from gridstatus.utils import _handle_date
 
+        # if date range tuple, just validate start
+        if isinstance(date, tuple):
+            date = date[0]
+
         if date == "latest":
             return _handle_date("today", tz=tz)
         elif (
             isinstance(date, str)
             or isinstance(date, pd.Timestamp)
             or isinstance(date, datetime.date)
         ):
@@ -84,19 +88,14 @@
 
         tz = instance.default_timezone
         date_value = self._parse_date(date, tz=tz)
         market_value = Markets(market)
 
         self._check_support(date, date_value, market_value, tz)
 
-        if date != "latest":
-            if "date" in arguments:
-                arguments["date"] = date_value
-            elif "start" in arguments:
-                arguments["start"] = date_value
         arguments["market"] = market_value
 
         return bound_args
 
     def _check_support(self, orig_date, date, market, tz):
         if market not in self.supports:
             raise NotSupported(f"{market} not supported")
```

### Comparing `gridstatus-0.20.0/gridstatus/miso.py` & `gridstatus-0.21.0/gridstatus/miso.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
 import pandas as pd
 import requests
 
 from gridstatus import utils
 from gridstatus.base import ISOBase, Markets, NotSupported
+from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
-from gridstatus.logging import log
 
 
 class MISO(ISOBase):
     """Midcontinent Independent System Operator (MISO)"""
 
     BASE = "https://api.misoenergy.org/MISORTWDDataBroker/DataBrokerServices.asmx"
 
@@ -139,15 +139,21 @@
         )
 
         df["Forecast Time"] = date
 
         df = add_interval_end(df, 60)
 
         df = df[
-            ["Time", "Interval Start", "Interval End", "Forecast Time", "LoadForecast"]
+            [
+                "Time",
+                "Interval Start",
+                "Interval End",
+                "Forecast Time",
+                "LoadForecast",
+            ]
         ].rename(
             columns={"LoadForecast": "Load Forecast"},
         )
 
         return df
 
     def _get_load_and_forecast_data(self, verbose=False):
```

### Comparing `gridstatus-0.20.0/gridstatus/nyiso.py` & `gridstatus-0.21.0/gridstatus/pjm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,805 +1,688 @@
 import io
-from zipfile import ZipFile
+import math
+import warnings
 
 import pandas as pd
 import requests
+import tqdm
 
-import gridstatus
 from gridstatus import utils
-from gridstatus.base import (
-    GridStatus,
-    InterconnectionQueueStatus,
-    ISOBase,
-    Markets,
+from gridstatus.base import ISOBase, Markets, NotSupported
+from gridstatus.decorators import (
+    _get_pjm_archive_date,
+    pjm_update_dates,
+    support_date_range,
 )
-from gridstatus.decorators import support_date_range
+from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
-from gridstatus.logging import log
-
-ZONE = "zone"
-GENERATOR = "generator"
-"""NYISO offers LMP data at two locational granularities: \
-    load zone and point of generator interconnection"""
 
 
-class NYISO(ISOBase):
-    """New York Independent System Operator (NYISO)"""
+class PJM(ISOBase):
+    """PJM"""
 
-    name = "New York ISO"
-    iso_id = "nyiso"
+    name = "PJM"
+    iso_id = "pjm"
     default_timezone = "US/Eastern"
-    markets = [Markets.REAL_TIME_5_MIN, Markets.DAY_AHEAD_HOURLY]
-    status_homepage = "https://www.nyiso.com/system-conditions"
-    interconnection_homepage = "https://www.nyiso.com/interconnections"
-
-    @support_date_range(frequency="MS")
-    def get_status(self, date, end=None, verbose=False):
-        if date == "latest":
-            latest = self._latest_from_today(self.get_status)
-            return GridStatus(
-                time=latest["time"],
-                status=latest["status"],
-                reserves=None,
-                iso=self,
-                notes=latest["notes"],
-            )
-
-        status_df = self._download_nyiso_archive(
-            date=date,
-            end=end,
-            dataset_name="RealTimeEvents",
-            verbose=verbose,
-        )
-
-        status_df = status_df.rename(
-            columns={"Message": "Status"},
-        )
-
-        def _parse_status(row):
-            STATE_CHANGE = "**State Change. System now operating in "
-
-            row["Notes"] = None
-            if row["Status"] == "Start of day system state is NORMAL":
-                row["Notes"] = [row["Status"]]
-                row["Status"] = "Normal"
-            elif STATE_CHANGE in row["Status"]:
-                row["Notes"] = [row["Status"]]
-
-                row["Status"] = row["Status"][
-                    row["Status"].index(STATE_CHANGE)
-                    + len(STATE_CHANGE) : -len(" state.**")
-                ].capitalize()
 
-            return row
+    interconnection_homepage = (
+        "https://www.pjm.com/planning/services-requests/interconnection-queues.aspx"
+    )
 
-        status_df = status_df.apply(_parse_status, axis=1)
-        status_df = status_df[["Time", "Status", "Notes"]]
-        return status_df
+    location_types = [
+        "ZONE",
+        "LOAD",
+        "GEN",
+        "AGGREGATE",
+        "INTERFACE",
+        "EXT",
+        "HUB",
+        "EHV",
+        "TIE",
+        "RESIDUAL_METERED_EDC",
+    ]
+
+    hub_node_ids = [
+        "51217",
+        "116013751",
+        "35010337",
+        "34497151",
+        "34497127",
+        "34497125",
+        "33092315",
+        "33092313",
+        "33092311",
+        "4669664",
+        "51288",
+        "51287",
+    ]
+
+    zone_node_ids = [
+        "1",
+        "3",
+        "51291",
+        "51292",
+        "51293",
+        "51295",
+        "51296",
+        "51297",
+        "51298",
+        "51299",
+        "51300",
+        "51301",
+        "7633629",
+        "8394954",
+        "8445784",
+        "33092371",
+        "34508503",
+        "34964545",
+        "37737283",
+        "116013753",
+        "124076095",
+        "970242670",
+        "1709725933",
+    ]
+
+    markets = [
+        Markets.REAL_TIME_5_MIN,
+        Markets.REAL_TIME_HOURLY,
+        Markets.DAY_AHEAD_HOURLY,
+    ]
 
-    @support_date_range(frequency="MS")
+    @support_date_range(frequency="365D")
     def get_fuel_mix(self, date, end=None, verbose=False):
-        # note: this is simlar datastructure to pjm
+        """Get fuel mix for a date or date range  in hourly intervals"""
 
         if date == "latest":
-            return (
-                self.get_fuel_mix(date="today", verbose=verbose)
-                .tail(1)
-                .reset_index(drop=True)
-            )
+            mix = self.get_fuel_mix("today")
+            return mix.tail(1).reset_index(drop=True)
+
+        # earliest date available appears to be 1/1/2016
+        data = {
+            "fields": "datetime_beginning_utc,fuel_type,is_renewable,mw",
+            "sort": "datetime_beginning_utc",
+            "order": "Asc",
+        }
 
-        mix_df = self._download_nyiso_archive(
-            date=date,
+        mix_df = self._get_pjm_json(
+            "gen_by_fuel",
+            start=date,
             end=end,
-            dataset_name="rtfuelmix",
-            verbose=verbose,
+            params=data,
+            interval_duration_min=60,
         )
 
         mix_df = mix_df.pivot_table(
             index=["Time", "Interval Start", "Interval End"],
-            columns="Fuel Category",
-            values="Gen MW",
+            columns="fuel_type",
+            values="mw",
             aggfunc="first",
         ).reset_index()
 
         mix_df.columns.name = None
 
         return mix_df
 
-    @support_date_range(frequency="MS")
+    @support_date_range(frequency="30D")
     def get_load(self, date, end=None, verbose=False):
-        """Returns load at a previous date in 5 minute intervals"""
+        """Returns load at a previous date at 5 minute intervals
+
+        Arguments:
+            date (datetime.date, str): date to get load for. must be in last 30 days
+
+        Returns:
+            pd.DataFrame: Load data time series. Columns: Time, Load, and all areas
+
+            * Load columns represent PJM-wide load
+            * Returns data for the following areas: AE, AEP, APS, ATSI,
+            BC, COMED, DAYTON, DEOK, DOM, DPL, DUQ, EKPC, JC,
+            ME, PE, PEP, PJM MID ATLANTIC REGION, PJM RTO,
+            PJM SOUTHERN REGION, PJM WESTERN REGION, PL, PN, PS, RECO
+        """
+
         if date == "latest":
-            return self._latest_from_today(self.get_load)
+            return self._latest_from_today(self.get_load, verbose=verbose)
+
+        # more hourly historical load here: https://dataminer2.pjm.com/feed/hrl_load_metered/definition
 
-        data = self._download_nyiso_archive(
-            date=date,
+        # todo can support a load area
+        data = {
+            "order": "Asc",
+            "sort": "datetime_beginning_utc",
+            "isActiveMetadata": "true",
+            "fields": "area,datetime_beginning_utc,instantaneous_load",
+        }
+        load = self._get_pjm_json(
+            "inst_load",
+            # one minute earlier to hand off by a few seconds seconds
+            start=date - pd.Timedelta(minutes=1),
             end=end,
-            dataset_name="pal",
+            params=data,
             verbose=verbose,
         )
 
-        # drop NA loads
-        data = data.dropna(subset=["Load"])
+        # pivot on area
+        load = load.pivot_table(
+            index=["Time", "Interval Start"],
+            columns="area",
+            values="instantaneous_load",
+            aggfunc="first",
+        ).reset_index()
+
+        # round to nearest minute
+        load["Interval Start"] = load["Interval Start"].dt.round("1min")
+        load["Time"] = load["Interval Start"]
+
+        load["Interval End"] = load["Interval Start"] + pd.Timedelta(minutes=5)
 
-        # TODO load by zone
-        load = (
-            data.groupby(["Time", "Interval Start", "Interval End"])["Load"]
-            .sum()
-            .reset_index()
+        load.columns.name = None
+
+        # set Load column name to match return column of other ISOs
+        load["Load"] = load["PJM RTO"]
+
+        load = utils.move_cols_to_front(
+            load,
+            ["Time", "Interval Start", "Interval End", "Load"],
         )
 
         return load
 
-    @support_date_range(frequency="MS")
-    def get_load_forecast(self, date, end=None, verbose=False):
-        """Get load forecast for a date in 1 hour intervals"""
-        date = utils._handle_date(date, self.default_timezone)
-
-        # todo optimize this to accept a date range
-        data = self._download_nyiso_archive(
-            date,
-            end=end,
-            dataset_name="isolf",
+    def get_load_forecast(self, date, verbose=False):
+        """Get forecast for today in hourly intervals.
+
+        Updates every Every half hour on the quarter E.g. 1:15 and 1:45
+
+        """
+
+        if not utils.is_today(date, self.default_timezone):
+            raise NotSupported()
+
+        # todo: should we use the UTC field instead of EPT?
+        params = {
+            "fields": (
+                "evaluated_at_datetime_utc,forecast_area,forecast_datetime_beginning_utc,forecast_datetime_ending_utc,forecast_load_mw"
+            ),
+            "forecast_area": "RTO_COMBINED",
+        }
+        data = self._get_pjm_json(
+            "load_frcstd_7_day",
+            start=None,
+            params=params,
             verbose=verbose,
         )
-
-        data = data[
-            ["Time", "Interval Start", "Interval End", "File Date", "NYISO"]
-        ].rename(
+        data = data.rename(
             columns={
-                "File Date": "Forecast Time",
-                "NYISO": "Load Forecast",
-                "Time": "Time",
+                "evaluated_at_datetime_utc": "Forecast Time",
+                "forecast_load_mw": "Load Forecast",
+                "forecast_datetime_beginning_utc": "Interval Start",
+                "forecast_datetime_ending_utc": "Interval End",
             },
         )
 
+        data.drop("forecast_area", axis=1, inplace=True)
+
+        data["Forecast Time"] = pd.to_datetime(
+            data["Forecast Time"],
+            utc=True,
+        ).dt.tz_convert(
+            self.default_timezone,
+        )
+
+        data["Interval Start"] = pd.to_datetime(
+            data["Interval Start"],
+            utc=True,
+        ).dt.tz_convert(
+            self.default_timezone,
+        )
+
+        data["Interval End"] = pd.to_datetime(
+            data["Interval End"],
+            utc=True,
+        ).dt.tz_convert(
+            self.default_timezone,
+        )
+
+        data["Time"] = data["Interval Start"]
+
+        data = data[
+            [
+                "Time",
+                "Interval Start",
+                "Interval End",
+                "Forecast Time",
+                "Load Forecast",
+            ]
+        ]
         return data
 
+    # todo https://dataminer2.pjm.com/feed/load_frcstd_hist/definition
+    # def get_historical_forecast(self, date):
+    # pass
+
+    def get_pnode_ids(self):
+        data = {
+            "fields": "effective_date,pnode_id,pnode_name,pnode_subtype,pnode_type\
+                ,termination_date,voltage_level,zone",
+            "termination_date": "12/31/9999exact",
+        }
+        nodes = self._get_pjm_json("pnode", start=None, params=data)
+
+        # only keep most recent effective date for each id
+        # return sorted by pnode_id
+        nodes = (
+            nodes.sort_values("effective_date", ascending=False)
+            .drop_duplicates(
+                "pnode_id",
+            )
+            .sort_values("pnode_id")
+            .reset_index(drop=True)
+        )
+        return nodes
+
     @lmp_config(
         supports={
             Markets.REAL_TIME_5_MIN: ["latest", "today", "historical"],
-            Markets.DAY_AHEAD_HOURLY: ["latest", "today", "historical"],
+            Markets.REAL_TIME_HOURLY: ["today", "historical"],
+            Markets.DAY_AHEAD_HOURLY: ["today", "historical"],
         },
     )
-    @support_date_range(frequency="MS")
+    @support_date_range(frequency="365D", update_dates=pjm_update_dates)
     def get_lmp(
         self,
         date,
+        market: str,
         end=None,
-        market: str = None,
-        locations: list = None,
-        location_type: str = None,
+        locations="hubs",
+        location_type=None,
         verbose=False,
     ):
-        """
-        Supported Markets:
-            - ``REAL_TIME_5_MIN``
-            - ``DAY_AHEAD_HOURLY``
-
-        Supported Location Types:
-            - ``zone``
-            - ``generator``
+        """Returns LMP at a previous date
+
+        Notes:
+            * If start date is prior to the PJM archive date, all data
+            must be downloaded before location filtering can be performed
+            due to limitations of PJM API. The archive date is
+            186 days (~6 months) before today for the 5 minute real time
+            market and 731 days (~2 years) before today for the Hourly
+            Real Time and Day Ahead Hourly markets. Node type filter can be
+            performed for Real Time Hourly and Day Ahead Hourly markets.
+
+            * If location_type is provided, it is filtered after data
+            is retrieved for Real Time 5 Minute market regardless of the
+            date. This is due to PJM api limitations
+
+        Arguments:
+            date (datetime.date, str): date to get LMPs for
+
+            end (datetime.date, str): end date to get LMPs for
+
+            market (str):  Supported Markets:
+                REAL_TIME_5_MIN, REAL_TIME_HOURLY, DAY_AHEAD_HOURLY
+
+            locations (list, optional):  list of pnodeid to get LMPs for.
+                Defaults to "hubs". Use get_pnode_ids() to get
+                a list of possible pnode ids. If "all", will
+                return data from all p nodes (warning there are
+                over 10,000 unique pnodes, so expect millions or billions of rows!)
+
+            location_type (str, optional):  If specified,
+                will only return data for nodes of this type.
+                Defaults to None. Possible location types are: 'ZONE',
+                'LOAD', 'GEN', 'AGGREGATE', 'INTERFACE', 'EXT',
+                'HUB', 'EHV', 'TIE', 'RESIDUAL_METERED_EDC'.
+
         """
         if date == "latest":
             return self._latest_lmp_from_today(
                 market=market,
                 locations=locations,
                 location_type=location_type,
                 verbose=verbose,
             )
 
-        if locations is None:
-            locations = "ALL"
+        if locations == "hubs":
+            locations = self.hub_node_ids
 
-        if location_type is None:
-            location_type = ZONE
+        params = {}
 
-        marketname = self._set_marketname(market)
-        location_type = self._set_location_type(location_type)
-        filename = marketname + f"_{location_type}"
+        if market == Markets.REAL_TIME_5_MIN:
+            market_endpoint = "rt_fivemin_hrl_lmps"
+            market_type = "rt"
+            interval_duration_min = 5
+        elif market == Markets.REAL_TIME_HOURLY:
+            # todo implemlement location type filter
+            market_endpoint = "rt_hrl_lmps"
+            market_type = "rt"
+            interval_duration_min = 60
+        elif market == Markets.DAY_AHEAD_HOURLY:
+            # todo implemlement location type filter
+            market_endpoint = "da_hrl_lmps"
+            market_type = "da"
+            interval_duration_min = 60
+        else:
+            raise ValueError(
+                (
+                    "market must be one of REAL_TIME_5_MIN, REAL_TIME_HOURLY,"
+                    " DAY_AHEAD_HOURLY"
+                ),
+            )
 
-        df = self._download_nyiso_archive(
-            date=date,
-            end=end,
-            dataset_name=marketname,
-            filename=filename,
-            verbose=verbose,
-        )
+        if location_type:
+            location_type = location_type.upper()
+            if location_type not in self.location_types:
+                raise ValueError(
+                    f"location_type must be one of {self.location_types}",
+                )
 
-        columns = {
-            "Name": "Location",
-            "LBMP ($/MWHr)": "LMP",
-            "Marginal Cost Losses ($/MWHr)": "Loss",
-            "Marginal Cost Congestion ($/MWHr)": "Congestion",
-        }
+            if market == Markets.REAL_TIME_5_MIN:
+                warnings.warn(
+                    (
+                        "When using Real Time 5 Minute market, location_type filter"
+                        " will happen after all data is downloaded"
+                    ),
+                )
+            else:
+                params["type"] = f"*{location_type}*"
+
+            if locations is not None:
+                locations = None
 
-        df = df.rename(columns=columns)
+        if date >= _get_pjm_archive_date(market):
+            # after archive date, filtering allowed
+            params["fields"] = (
+                f"congestion_price_{market_type},datetime_beginning_ept,datetime_beginning_utc,equipment,marginal_loss_price_{market_type},pnode_id,pnode_name,row_is_current,system_energy_price_{market_type},total_lmp_{market_type},type,version_nbr,voltage,zone",
+            )
+
+            if locations and locations != "ALL":
+                params["pnode_id"] = ";".join(map(str, locations))
+
+        elif locations is not None:
+            warnings.warn(
+                (
+                    "Querying before archive date, so filtering by location will happen"
+                    " after all data is downloaded"
+                ),
+            )
+
+        try:
+            data = self._get_pjm_json(
+                market_endpoint,
+                start=date,
+                end=end,
+                params=params,
+                verbose=verbose,
+                interval_duration_min=interval_duration_min,
+            )
+        except RuntimeError as e:
+            if "No data found" not in str(e):
+                raise e
+
+            if market_endpoint == "rt_fivemin_hrl_lmps":
+                market_endpoint = "rt_unverified_fivemin_lmps"
+                params[
+                    "fields"
+                ] = "congestion_price_rt,datetime_beginning_ept,datetime_beginning_utc,marginal_loss_price_rt,occ_check,pnode_id,pnode_name,ref_caseid_used_multi_interval,total_lmp_rt,type"  # noqa: E501
+
+            data = self._get_pjm_json(
+                market_endpoint,
+                start=date,
+                end=end,
+                params=params,
+                verbose=verbose,
+                interval_duration_min=interval_duration_min,
+            )
+
+            data["system_energy_price_rt"] = (
+                data["total_lmp_rt"]
+                - data["congestion_price_rt"]
+                - data["marginal_loss_price_rt"]
+            )
+
+        data = data.rename(
+            columns={
+                "pnode_id": "Location",
+                "pnode_name": "Location Name",
+                "type": "Location Type",
+                f"total_lmp_{market_type}": "LMP",
+                f"system_energy_price_{market_type}": "Energy",
+                f"congestion_price_{market_type}": "Congestion",
+                f"marginal_loss_price_{market_type}": "Loss",
+            },
+        )
 
-        df["Energy"] = df["LMP"] - (df["Loss"] - df["Congestion"])
-        df["Market"] = market.value
-        df["Location Type"] = "Zone" if location_type == ZONE else "Generator"
+        data["Market"] = market.value
 
-        df = df[
+        data = data[
             [
                 "Time",
                 "Interval Start",
                 "Interval End",
                 "Market",
                 "Location",
+                "Location Name",
                 "Location Type",
                 "LMP",
                 "Energy",
                 "Congestion",
                 "Loss",
             ]
         ]
 
-        df = utils.filter_lmp_locations(df, locations)
-
-        return df
-
-    def get_interconnection_queue(self, verbose=False):
-        """Return NYISO interconnection queue
-
-        Additional Non-NYISO queue info: https://www3.dps.ny.gov/W/PSCWeb.nsf/All/286D2C179E9A5A8385257FBF003F1F7E?OpenDocument
-
-        Returns:
-            pandas.DataFrame: Interconnection queue containing, active, withdrawn, \
-                and completed project
-
-        """  # noqa
-
-        # 3 sheets - ['Interconnection Queue', 'Withdrawn', 'In Service']
-        # harded coded for now. perhaps this url can be parsed from the html here:
-        url = "https://www.nyiso.com/documents/20142/1407078/NYISO-Interconnection-Queue.xlsx"  # noqa
-
-        msg = f"Downloading interconnection queue from {url}"
-        log(msg, verbose)
-
-        all_sheets = pd.read_excel(
-            url,
-            sheet_name=["Interconnection Queue", "Withdrawn"],
-        )
-
-        # Drop extra rows at bottom
-        active = (
-            all_sheets["Interconnection Queue"]
-            .dropna(
-                subset=["Queue Pos.", "Project Name"],
-            )
-            .copy()
-        )
-
-        active["Status"] = InterconnectionQueueStatus.ACTIVE.value
-
-        withdrawn = all_sheets["Withdrawn"]
-        withdrawn["Status"] = InterconnectionQueueStatus.WITHDRAWN.value
-        # assume it was withdrawn when last updated
-        withdrawn["Withdrawn Date"] = withdrawn["Last Update"]
-        withdrawn["Withdrawal Comment"] = None
-        withdrawn = withdrawn.rename(columns={"Utility ": "Utility"})
-
-        # make completed look like the other two sheets
-        completed = pd.read_excel(url, sheet_name="In Service", header=[0, 1])
-        completed.insert(15, "SGIA Tender Date", None)
-        completed.insert(16, "CY Complete Date", None)
-        completed.insert(17, "Proposed Initial-Sync Date", None)
-
-        completed["Status"] = InterconnectionQueueStatus.COMPLETED.value
-
-        if (
-            "SGIA Tender Date" in active.columns
-            and "SGIA Tender Date" not in completed.columns
-        ):
-            active = active.drop(columns=["SGIA Tender Date"])
-        completed.columns = active.columns
-
-        # the spreadsheet doesnt have a date, so make it null
-        completed["Proposed  In-Service"] = None
-        completed["Proposed COD"] = None
-        # assume it was finished when last updated
-        completed["Actual Completion Date"] = completed["Last Updated Date"]
-
-        queue = pd.concat([active, withdrawn, completed])
-
-        # fix extra space in column name
-
-        queue["Type/ Fuel"] = queue["Type/ Fuel"].map(
-            {
-                "S": "Solar",
-                "ES": "Energy Storage",
-                "W": "Wind",
-                "AC": "AC Transmission",
-                "DC": "DC Transmission",
-                "CT": "Combustion Turbine",
-                "CC": "Combined Cycle",
-                "M": "Methane",
-                #    "CR": "",
-                "H": "Hydro",
-                "L": "Load",
-                "ST": "Steam Turbine",
-                "CC-NG": "Natural Gas",
-                "FC": "Fuel Cell",
-                "PS": "Pumped Storage",
-                "NU": "Nuclear",
-                "D": "Dual Fuel",
-                #    "C": "",
-                "NG": "Natural Gas",
-                "Wo": "Wood",
-                "F": "Flywheel",
-                #    "CW": "",
-                "CC-D": "Combined Cycle - Dual Fuel",
-                "SW": "=Solid Waste",
-                #    "CR=CSR - ES + Solar": "",
-                "CT-NG": "Combustion Turbine - Natural Gas",
-                "DC/AC": "DC/AC Transmission",
-                "CT-D": "Combustion Turbine - Dual Fuel",
-                "CS-NG": "Steam Turbine & Combustion Turbine-  Natural Gas",
-                "ST-NG": "Steam Turbine - Natural Gas",
-            },
-        )
-
-        queue["Capacity (MW)"] = (
-            queue[["SP (MW)", "WP (MW)"]]
-            .replace(
-                "TBD",
-                0,
-            )
-            .replace(" ", 0)
-            .fillna(0)
-            .astype(float)
-            .max(axis=1)
-        )
-
-        queue["Date of IR"] = pd.to_datetime(queue["Date of IR"])
-        queue["Proposed COD"] = pd.to_datetime(
-            queue["Proposed COD"],
-            errors="coerce",
-        )
-        queue["Proposed  In-Service"] = pd.to_datetime(
-            queue["Proposed  In-Service"],
-            errors="coerce",
-        )
-        queue["Proposed Initial-Sync Date"] = pd.to_datetime(
-            queue["Proposed Initial-Sync Date"],
-            errors="coerce",
-        )
-
-        # TODO handle other 2 sheets
-        # TODO they publish past queues,
-        # but not sure what data is in them that is relevant
-
-        rename = {
-            "Queue Pos.": "Queue ID",
-            "Project Name": "Project Name",
-            "County": "County",
-            "State": "State",
-            "Owner/Developer": "Interconnecting Entity",
-            "Utility": "Transmission Owner",
-            "Interconnection Point": "Interconnection Location",
-            "Status": "Status",
-            "Date of IR": "Queue Date",
-            "Proposed COD": "Proposed Completion Date",
-            "Type/ Fuel": "Generation Type",
-            "Capacity (MW)": "Capacity (MW)",
-            "SP (MW)": "Summer Capacity (MW)",
-            "WP (MW)": "Winter Capacity (MW)",
-        }
-
-        extra_columns = [
-            "Proposed  In-Service",
-            "Proposed Initial-Sync Date",
-            "Last Updated Date",
-            "Z",
-            "S",
-            "Availability of Studies",
-            "SGIA Tender Date",
-        ]
-
-        queue = utils.format_interconnection_df(queue, rename, extra_columns)
-
-        return queue
-
-    def get_generators(self, verbose=False):
-        """Get a list of generators in NYISO
-
-        When possible return capacity and fuel type information
-
-        Arguments:
-            verbose (bool, optional): print out requested url. Defaults to False.
-
-        Returns:
-            pandas.DataFrame: a DataFrame of generators and locations
-
-            **Possible Columns**
-
-            * Generator Name
-            * PTID
-            * Subzone
-            * Zone
-            * Latitude
-            * Longitude
-            * Owner, Operator, and / or Billing Organization
-            * Station Unit
-            * Town
-            * County
-            * State
-            * In-Service Date
-            * Name Plate Rating (V) MW
-            * 2022 CRIS MW Summer
-            * 2022 CRIS MW Winter
-            * 2022 Capability MW Summer
-            * 2022 Capability MW Winter
-            * Is Dual Fuel
-            * Unit Type
-            * Fuel Type 1
-            * Fuel Type 2
-            * 2021 Net Energy GWh
-            * Notes
-            * Generator Type
-        """
-
-        url = "http://mis.nyiso.com/public/csv/generator/generator.csv"
-
-        msg = f"Requesting {url}"
-        log(msg, verbose)
-
-        df = pd.read_csv(url)
-
-        # need to be updated once a year. approximately around end of april
-        # find it here: https://www.nyiso.com/gold-book-resources
-        capacity_url_2022 = "https://www.nyiso.com/documents/20142/30338270/2022-NYCA-Generators.xlsx/f0526021-37fd-2c27-94ee-14d0f31878c1"  # noqa
-
-        msg = f"Requesting {url}"
-        log(msg, verbose)
-
-        generators = pd.read_excel(
-            capacity_url_2022,
-            sheet_name=[
-                "Table III-2a",
-                "Table III-2b",
-            ],
-            skiprows=3,
-            header=[0, 1, 2, 3, 4],
-        )
-
-        generators["Table III-2a"]["Generator Type"] = "Market Generator"
-        generators["Table III-2b"]["Generator Type"] = "Non-Market Generator"
-
-        # combined both sheets
-        generators = pd.concat(generators.values())
-
-        # manually transcribed column names
-        generators.columns = [
-            "LINE REF. NO.",
-            "Owner, Operator, and / or Billing Organization",
-            "Station Unit",
-            "Zone",
-            "PTID",
-            "Town",
-            "County",
-            "State",
-            "In-Service Date",
-            "Name Plate Rating (V) MW",
-            "2022 CRIS MW Summer",
-            "2022 CRIS MW Winter",
-            "2022 Capability MW Summer",
-            "2022 Capability MW Winter",
-            "Is Dual Fuel",
-            "Unit Type",
-            "Fuel Type 1",
-            "Fuel Type 2",
-            "2021 Net Energy GWh",
-            "Notes",
-            "Generator Type",
-        ]
-        generators = generators.dropna(subset=["PTID"])
-
-        generators["PTID"] = generators["PTID"].astype(int)
-
-        # in other data
-        generators = generators.drop(columns=["Zone", "LINE REF. NO."])
-
-        combined = pd.merge(df, generators, on=["PTID"], how="left")
+        # API cannot filter location type for rt 5 min
+        if location_type and market == Markets.REAL_TIME_5_MIN:
+            data = data[data["Location Type"] == location_type]
+
+        if locations is not None and locations != "ALL":
+            data = utils.filter_lmp_locations(
+                data,
+                map(int, locations),
+            )
 
-        unit_type_map = {
-            "CC": "Combined Cycle",
-            "CG": "Cogeneration",
-            "CT": "Combustion Turbine Portion (CC)",
-            "CW": "Waste Heat Only (CC)",
-            "ES": "Energy Storage",
-            "FC": "Fuel Cell",
-            "GT": "Combustion Turbine",
-            "HY": "Conventional Hydro",
-            "IC": "Internal Combustion",
-            "JE": "Jet Engine",
-            "NB": "Steam (BWR Nuclear)",
-            "NP": "Steam (PWR Nuclear)",
-            "PS": "Pumped Storage Hydro",
-            "PV": "Photovoltaic",
-            "ST": "Steam Turbine (Fossil)",
-            "WT": "Wind Turbine",
-        }
-        combined["Unit Type"] = combined["Unit Type"].map(unit_type_map)
+        data = data.sort_values("Interval Start")
 
-        fuel_type_map = {
-            "BAT": "Battery",
-            "BUT": "Butane",
-            "FO2": "No. 2 Fuel Oil",
-            "FO4": "No. 4 Fuel Oil",
-            "FO6": "No. 6 Fuel Oil",
-            "FW": "Fly Wheel",
-            "JF": "Jet Fuel",
-            "KER": "Kerosene",
-            "MTE": "Methane (Bio Gas)",
-            "NG": "Natural Gas",
-            "OT": "Other (Describe In Footnote)",
-            "REF": "Refuse (Solid Waste)",
-            "SUN": "Sunlight",
-            "UR": "Uranium",
-            "WAT": "Water",
-            "WD": "Wood and/or Wood Waste",
-            "WND": "Wind",
-        }
-        combined["Fuel Type 1"] = combined["Fuel Type 1"].map(
-            fuel_type_map,
-        )
-        combined["Fuel Type 2"] = combined["Fuel Type 2"].map(
-            fuel_type_map,
-        )
-
-        combined["Is Dual Fuel"] = combined["Is Dual Fuel"] == "YES"
+        return data
 
-        state_code_map = {
-            36: "New York",
-            42: "Pennsylvania",
-            25: "Massachusetts",
-            34: "New Jersey",
+    def _get_pjm_json(
+        self,
+        endpoint,
+        start,
+        params,
+        end=None,
+        start_row=1,
+        row_count=100000,
+        interval_duration_min=None,
+        verbose=False,
+    ):
+        default_params = {
+            "startRow": start_row,
+            "rowCount": row_count,
         }
-        combined["State"] = combined["State"].map(state_code_map)
 
-        # todo map county codes to names. info on first sheet of excel
+        # update final params with default params
+        final_params = params.copy()
+        final_params.update(default_params)
 
-        return combined
-
-    def get_loads(self, verbose=False):
-        """Get a list of loads in NYISO
-
-        Arguments:
-            verbose (bool, optional): print out requested url. Defaults to False.
+        if start is not None:
+            start = utils._handle_date(start)
 
-        Returns:
-            pandas.DataFrame: a DataFrame of loads and locations
-        """
+            if end:
+                end = utils._handle_date(end)
+            else:
+                end = start + pd.DateOffset(days=1)
 
-        url = "http://mis.nyiso.com/public/csv/load/load.csv"
+            final_params["datetime_beginning_ept"] = (
+                start.strftime("%m/%d/%Y %H:%M") + "to" + end.strftime("%m/%d/%Y %H:%M")
+            )
 
-        msg = f"Requesting {url}"
+        msg = f"Retrieving data from {endpoint} with params {final_params}"
         log(msg, verbose)
 
-        df = pd.read_csv(url)
-
-        return df
+        api_key = self._get_key()
+        r = self._get_json(
+            "https://api.pjm.com/api/v1/" + endpoint,
+            params=final_params,
+            headers={"Ocp-Apim-Subscription-Key": api_key},
+        )
+
+        if "errors" in r:
+            raise RuntimeError(r["errors"])
+
+        # todo should this be a warning?
+        if r["totalRows"] == 0:
+            raise RuntimeError("No data found for query")
+
+        df = pd.DataFrame(r["items"])
+
+        num_pages = math.ceil(r["totalRows"] / row_count)
+        if num_pages > 1:
+            to_add = [df]
+            for page in tqdm.tqdm(range(1, num_pages), initial=1, total=num_pages):
+                next_url = [x for x in r["links"] if x["rel"] == "next"][0]["href"]
+                r = self._get_json(
+                    next_url,
+                    headers={
+                        "Ocp-Apim-Subscription-Key": api_key,
+                    },
+                )
+                to_add.append(pd.DataFrame(r["items"]))
 
-    def _set_marketname(self, market: Markets) -> str:
-        if market == Markets.REAL_TIME_5_MIN:
-            marketname = "realtime"
-        elif market == Markets.DAY_AHEAD_HOURLY:
-            marketname = "damlbmp"
-        else:
-            raise RuntimeError("LMP Market is not supported")
-        return marketname
+            df = pd.concat(to_add)
 
-    def _set_location_type(self, location_type: str) -> str:
-        location_types = [ZONE, GENERATOR]
-        if location_type == ZONE:
-            return ZONE
-        elif location_type == GENERATOR:
-            return "gen"
-        else:
-            raise ValueError(
-                f"Invalid location type. Expected one of: {location_types}",
+        if "datetime_beginning_utc" in df.columns:
+            df["Interval Start"] = (
+                pd.to_datetime(df["datetime_beginning_utc"])
+                .dt.tz_localize(
+                    "UTC",
+                )
+                .dt.tz_convert(self.default_timezone)
             )
 
-    def _download_nyiso_archive(
-        self,
-        date,
-        end=None,
-        dataset_name=None,
-        filename=None,
-        verbose=False,
-    ):
-        if filename is None:
-            filename = dataset_name
-
-        date = gridstatus.utils._handle_date(date)
-        month = date.strftime("%Y%m01")
-        day = date.strftime("%Y%m%d")
-
-        csv_filename = f"{day}{filename}.csv"
-        csv_url = f"http://mis.nyiso.com/public/csv/{dataset_name}/{csv_filename}"
-        zip_url = (
-            f"http://mis.nyiso.com/public/csv/{dataset_name}/{month}{filename}_csv.zip"
-        )
-
-        # the last 7 days of file are hosted directly as csv
-        if end is None and date > pd.Timestamp.now(
-            tz=self.default_timezone,
-        ).normalize() - pd.DateOffset(days=7):
-            msg = f"Requesting {csv_url}"
-            log(msg, verbose)
-
-            df = pd.read_csv(csv_url)
-            df = _handle_time(df, dataset_name)
-            df["File Date"] = date.normalize()
-        else:
-
-            msg = f"Requesting {zip_url}"
-            log(msg, verbose)
+            # drop datetime_beginning_utc
+            df = df.drop(columns=["datetime_beginning_utc"])
 
-            r = requests.get(zip_url)
-            z = ZipFile(io.BytesIO(r.content))
-
-            all_dfs = []
-            if end is None:
-                date_range = [date]
-            else:
-                date_range = pd.date_range(
-                    date,
-                    end,
-                    freq="1D",
-                    inclusive="left",
+            # PJM API is inclusive of end,
+            # so we need to drop where end timestamp is included
+            df = df[
+                df["Interval Start"].dt.strftime(
+                    "%Y-%m-%d %H:%M",
                 )
+                != end.strftime("%Y-%m-%d %H:%M")
+            ]
 
-            for d in date_range:
-                d = gridstatus.utils._handle_date(d)
-                month = d.strftime("%Y%m01")
-                day = d.strftime("%Y%m%d")
-
-                csv_filename = f"{day}{filename}.csv"
-                df = pd.read_csv(z.open(csv_filename))
-                df["File Date"] = d.normalize()
+            if "datetime_ending_utc" in df.columns:
+                df["Interval End"] = (
+                    pd.to_datetime(df["datetime_ending_utc"])
+                    .dt.tz_localize(
+                        "UTC",
+                    )
+                    .dt.tz_convert(self.default_timezone)
+                )
 
-                df = _handle_time(df, dataset_name)
-                all_dfs.append(df)
+                # drop datetime_ending_utc
+                df = df.drop(columns=["datetime_ending_utc"])
+            elif interval_duration_min:
+                df["Interval End"] = df["Interval Start"] + pd.Timedelta(
+                    minutes=interval_duration_min,
+                )
 
-            df = pd.concat(all_dfs)
+        if "Interval Start" in df.columns:
+            df["Time"] = df["Interval Start"]
 
         return df
 
-    def get_capacity_prices(self, date=None, verbose=False):
-        """Pull the most recent capacity market report's market clearing prices
-
-        Arguments:
-            date (pandas.Timestamp): date that will be used to pull latest capacity
-                report (will refer to month and year)
-
-            verbose (bool, optional): print out requested url. Defaults to False.
-
-        Returns:
-            a DataFrame of monthly capacity prices (all three auctions) for \
-                each of the four capacity localities within NYISO
-        """
-        if date is None:
-            date = pd.Timestamp.now(tz=self.default_timezone)
-        else:
-            date = utils._handle_date(date, tz=self.default_timezone)
-
-        if date.year == 2014:
-            year_code = 1410927
-        elif date.year == 2015:
-            year_code = 1410895
-        elif date.year == 2016:
-            year_code = 1410901
-        if date.year == 2017:
-            year_code = 1410883
-        if date.year == 2018:
-            year_code = 1410889
-        if date.year == 2019:
-            year_code = 4266869
-        elif date.year == 2020:
-            year_code = 10106066
-        elif date.year == 2021:
-            year_code = 18170164
-        elif date.year == 2022:
-            year_code = 27447313
-        elif date.year == 2023:
-            year_code = 35397361
-        else:
-            raise ValueError(
-                "Year not currently supported. Please file an issue.",
-            )
-
-            # todo: it looks like the "27447313" component of the base URL changes
-            # every year but I'm not sure what the link between that and the year
-            # is...
-        capacity_market_base_url = (
-            f"https://www.nyiso.com/documents/20142/{year_code}/ICAP-Market-Report"
+    def get_interconnection_queue(self, verbose=False):
+        r = requests.post(
+            "https://services.pjm.com/PJMPlanningApi/api/Queue/ExportToXls",
+            headers={
+                # unclear if this key changes. obtained from https://www.pjm.com/dist/interconnectionqueues.71b76ed30033b3ff06bd.js
+                "api-subscription-key": "E29477D0-70E0-4825-89B0-43F460BF9AB4",
+                "Host": "services.pjm.com",
+                "Origin": "https://www.pjm.com",
+                "Referer": "https://www.pjm.com/",
+            },
         )
+        queue = pd.read_excel(io.BytesIO(r.content))
 
-        url = f"{capacity_market_base_url}-{date.month_name()}-{date.year}.xlsx"
-        msg = f"Requesting {url}"
-        log(msg, verbose)
-
-        df = pd.read_excel(url, sheet_name="MCP Table", header=[0, 1])
+        queue["Capacity (MW)"] = queue[["MFO", "MW In Service"]].min(axis=1)
 
-        df.rename(columns={"Unnamed: 0_level_0": "", "Date": ""}, inplace=True)
-        df.set_index("", inplace=True)
-        return df.dropna(how="any", axis="columns")
-
-
-dataset_interval_map = {
-    # (time_type, interval_duration_minutes)
-    # load
-    "pal": ("start", 5),
-    # fuel mix
-    "rtfuelmix": ("end", 5),
-    # load forecast
-    "isolf": ("start", 60),
-    # dam lmp
-    "damlbmp": ("start", 60),
-    # rt lmp
-    "realtime": ("end", 5),
-    # real time events
-    "RealTimeEvents": ("instantaneous", None),
-}
-
-
-def _handle_time(df, dataset_name):
+        rename = {
+            "Queue Number": "Queue ID",
+            "Name": "Project Name",
+            "County": "County",
+            "State": "State",
+            "Transmission Owner": "Transmission Owner",
+            "Queue Date": "Queue Date",
+            "Withdrawal Date": "Withdrawn Date",
+            "Withdrawn Remarks": "Withdrawal Comment",
+            "Status": "Status",
+            "Revised In Service Date": "Proposed Completion Date",
+            "Actual In Service Date": "Actual Completion Date",
+            "Fuel": "Generation Type",
+            "MW Capacity": "Summer Capacity (MW)",
+            "MW Energy": "Winter Capacity (MW)",
+        }
 
-    time_type, interval_duration_minutes = dataset_interval_map[dataset_name]
+        extra = [
+            "MW In Service",
+            "Commercial Name",
+            "Initial Study",
+            "Feasibility Study",
+            "Feasibility Study Status",
+            "System Impact Study",
+            "System Impact Study Status",
+            "Facilities Study",
+            "Facilities Study Status",
+            "Interim Interconnection Service Agreement",
+            "Interim/Interconnection Service Agreement Status",
+            "Wholesale Market Participation Agreement",
+            "Construction Service Agreement",
+            "Construction Service Agreement Status",
+            "Upgrade Construction Service Agreement",
+            "Upgrade Construction Service Agreement Status",
+            "Backfeed Date",
+            "Long-Term Firm Service Start Date",
+            "Long-Term Firm Service End Date",
+            "Test Energy Date",
+        ]
 
-    if "Time Stamp" in df.columns:
-        time_stamp_col = "Time Stamp"
-    elif "Timestamp" in df.columns:
-        time_stamp_col = "Timestamp"
+        missing = ["Interconnecting Entity", "Interconnection Location"]
 
-    def time_to_datetime(s, dst="infer"):
-        return pd.to_datetime(s).dt.tz_localize(
-            NYISO.default_timezone,
-            ambiguous=dst,
+        queue = utils.format_interconnection_df(
+            queue,
+            rename,
+            extra=extra,
+            missing=missing,
         )
 
-    if "Time Zone" in df.columns:
-        dst = df["Time Zone"] == "EDT"
-        df[time_stamp_col] = time_to_datetime(
-            df[time_stamp_col],
-            dst,
-        )
+        return queue
 
-    elif "Name" in df.columns:
-        # once we group by name, the time series for each group is no longer ambiguous
-        df[time_stamp_col] = df.groupby("Name", group_keys=False)[time_stamp_col].apply(
-            time_to_datetime,
-            "infer",
-        )
-    else:
-        df[time_stamp_col] = time_to_datetime(
-            df[time_stamp_col],
-            "infer",
+    def _get_key(self):
+        settings = self._get_json(
+            "https://dataminer2.pjm.com/config/settings.json",
         )
 
-    df = df.rename(columns={time_stamp_col: "Time"})
-
-    if time_type != "instantaneous":
-        interval_duration = pd.Timedelta(minutes=interval_duration_minutes)
-        if time_type == "start":
-            df["Interval Start"] = df["Time"]
-            df["Interval End"] = df["Time"] + interval_duration
-        elif time_type == "end":
-            df["Interval End"] = df["Time"]
-            df["Interval Start"] = df["Time"] - interval_duration
+        return settings["subscriptionKey"]
 
-        utils.move_cols_to_front(
-            df,
-            ["Time", "Interval Start", "Interval End"],
-        )
 
-    return df
+"""
+import gridstatus
+iso = gridstatus.PJM()
+nodes = iso.get_pnode_ids()
+zones = nodes[nodes["pnode_subtype"] == "ZONE"]
+zone_ids = zones["pnode_id"].tolist()
+iso.get_historical_lmp("Oct 1, 2022", "DAY_AHEAD_HOURLY", locations=zone_ids)
+pnode_id
+"""
 
 
-"""
-pricing data
+if __name__ == "__main__":
+    import gridstatus
 
-https://www.nyiso.com/en/energy-market-operational-data
-"""
+    for i in gridstatus.all_isos:
+        print("\n" + i.name + "\n")
+        for c in i().get_interconnection_queue().columns:
+            print(c.replace("\n", " "))
+
+        i().get_interconnection_queue().to_csv(
+            f"debug/queue/{i.iso_id}-queue.csv",
+            index=None,
+        )
```

### Comparing `gridstatus-0.20.0/gridstatus/spp.py` & `gridstatus-0.21.0/gridstatus/spp.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     GridStatus,
     InterconnectionQueueStatus,
     ISOBase,
     Markets,
     NotSupported,
 )
 from gridstatus.decorators import support_date_range
+from gridstatus.gs_logging import log
 from gridstatus.lmp_config import lmp_config
-from gridstatus.logging import log
 
 FS_RTBM_LMP_BY_LOCATION = "rtbm-lmp-by-location"
 FS_DAM_LMP_BY_LOCATION = "da-lmp-by-location"
 MARKETPLACE_BASE_URL = "https://marketplace.spp.org"
 FILE_BROWSER_API_URL = "https://marketplace.spp.org/file-browser-api/"
 
 LOCATION_TYPE_HUB = "HUB"
@@ -89,60 +89,49 @@
         if date != "latest":
             raise NotSupported()
 
         url = "https://www.spp.org/markets-operations/current-grid-conditions/"
         html_text = requests.get(url).content.decode("UTF-8")
         return self._get_status_from_html(html_text)
 
-    def get_fuel_mix(self, date, verbose=False):
+    def get_fuel_mix(self, date, detailed=False, verbose=False):
         """Get fuel mix
 
         Args:
             date: supports today and latest
+            detailed: if True, breaks out self scheduled and market scheduled
 
         Note:
             if today, returns last 2 hours of data. maybe include previous day
 
         Returns:
             pd.DataFrame: fuel mix
 
         """
         if date == "latest":
-            return (
-                self.get_fuel_mix("today", verbose=verbose)
-                .tail(1)
-                .reset_index(drop=True)
-            )
+            return self.get_fuel_mix(
+                "today",
+                detailed=detailed,
+                verbose=verbose,
+            ).reset_index(drop=True)
 
         if not utils.is_today(date, self.default_timezone):
             # https://marketplace.spp.org/pages/generation-mix-historical
             # many years of historical 5 minute data
             raise NotSupported
 
-        url = "https://marketplace.spp.org/chart-api/gen-mix/asChart"
-        r = self._get_json(url, verbose=verbose)["response"]
-
-        data = {"Timestamp": r["labels"]}
-        data.update((d["label"], d["data"]) for d in r["datasets"])
-
-        historical_mix = pd.DataFrame(data)
-
-        historical_mix["Timestamp"] = pd.to_datetime(
-            historical_mix["Timestamp"],
-        ).dt.tz_convert(
-            self.default_timezone,
-        )
-
-        historical_mix.rename(
-            columns={"Timestamp": "Time"},
-            inplace=True,
+        url = "https://marketplace.spp.org/file-browser-api/download/generation-mix-historical?path=%2FGenMix2Hour.csv"  # noqa
+        df_raw = pd.read_csv(url)
+        historical_mix = process_gen_mix(df_raw, detailed=detailed)
+
+        historical_mix = historical_mix.drop(
+            columns=["Short Term Load Forecast", "Average Actual Load"],
+            errors="ignore",
         )
 
-        historical_mix = add_interval(historical_mix, interval_min=5)
-
         return historical_mix
 
     def get_load(self, date, verbose=False):
         """Returns load for last 24hrs in 5 minute intervals"""
 
         if date == "latest":
             return self._latest_from_today(self.get_load)
@@ -213,14 +202,109 @@
         current_day_forecast = add_interval(
             current_day_forecast,
             interval_min=60,
         )
 
         return current_day_forecast
 
+    def _process_ver_curtailments(self, df):
+        df = df.rename(
+            columns={
+                "GMTIntervalEnding": "Interval End",
+                "WindRedispatchCurtailments": "Wind Redispatch Curtailments",
+                "WindManualCurtailments": "Wind Manual Curtailments",
+                "WindCurtailedForEnergy": "Wind Curtailed For Energy",
+                "SolarRedispatchCurtailments": "Solar Redispatch Curtailments",
+                "SolarManualCurtailments": "Solar Manual Curtailments",
+                "SolarCurtailedForEnergy": "Solar Curtailed For Energy",
+            },
+        )
+
+        df["Interval End"] = pd.to_datetime(df["Interval End"], utc=True).dt.tz_convert(
+            self.default_timezone,
+        )
+
+        df["Interval Start"] = df["Interval End"] - pd.Timedelta(minutes=5)
+
+        df["Time"] = df["Interval Start"]
+
+        cols = [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "Wind Redispatch Curtailments",
+            "Wind Manual Curtailments",
+            "Wind Curtailed For Energy",
+            "Solar Redispatch Curtailments",
+            "Solar Manual Curtailments",
+            "Solar Curtailed For Energy",
+        ]
+
+        # historical data doesnt have all columns
+        for c in cols:
+            if c not in df.columns:
+                df[c] = pd.NA
+
+        df = df[cols]
+
+        return df
+
+    @support_date_range("DAY_START")
+    def get_ver_curtailments(self, date, end=None, verbose=False):
+        """Get VER Curtailments
+
+        Supports recent data. For historical annual data use get_ver_curtailments_annual
+
+        Args:
+            date: start date
+            end: end date
+
+
+        """
+        url = f"https://marketplace.spp.org/file-browser-api/download/ver-curtailments?path=%2F{date.strftime('%Y')}%2F{date.strftime('%m')}%2FVER-Curtailments-{date.strftime('%Y%m%d')}.csv"  # noqa
+
+        msg = f"Downloading {url}"
+        log(msg, verbose)
+        df = pd.read_csv(url)
+
+        return self._process_ver_curtailments(df)
+
+    def get_ver_curtailments_annual(self, year, verbose=True):
+        """Get VER Curtailments for a year. Starting 2014.
+        Recent data use get_ver_curtailments
+
+        Args:
+            year: year to get data for
+            verbose: print url
+
+        Returns:
+            pd.DataFrame: VER Curtailments
+        """
+        url = f"https://marketplace.spp.org/file-browser-api/download/ver-curtailments?path=%2F{year}%2F{year}.zip"  # noqa
+        z = utils.get_zip_folder(url, verbose=verbose)
+
+        # iterate through all files in zip
+        # find the one that end with .csv
+        # read that csv
+        all_dfs = []
+        for f in z.filelist:
+            if f.filename.endswith(".csv"):
+                df = pd.read_csv(z.open(f.filename))
+                all_dfs.append(df)
+
+        df = pd.concat(all_dfs)
+
+        df = self._process_ver_curtailments(df)
+
+        df = df[~df["Interval Start"].isnull()]
+
+        df = df.sort_values("Time")
+
+        return df
+
     def _get_load_and_forecast(self, verbose=False):
         url = "https://marketplace.spp.org/chart-api/load-forecast/asChart"
 
         msg = f"Getting load and forecast from {url}"
         log(msg, verbose)
 
         r = self._get_json(url)["response"]
@@ -335,15 +419,15 @@
 
     @lmp_config(
         supports={
             Markets.REAL_TIME_5_MIN: ["latest", "today", "historical"],
             Markets.DAY_AHEAD_HOURLY: ["latest", "today", "historical"],
         },
     )
-    @support_date_range(frequency="1D")
+    @support_date_range(frequency="DAY_START")
     def get_lmp(
         self,
         date,
         end=None,
         market: str = None,
         locations: list = "ALL",
         location_type: str = LOCATION_TYPE_HUB,
@@ -880,14 +964,76 @@
 
         return (
             status,
             notes,
         )
 
 
+def process_gen_mix(df, detailed=False):
+    """Parse SPP generation mix data from
+    https://marketplace.spp.org/pages/generation-mix-historical
+
+    Args:
+        df (pd.DataFrame): raw data
+        detailed (bool): whether to combine market and self columns
+
+    Returns:
+        pd.DataFrame: processed data
+    """
+    new_df = df.copy()
+
+    # remove whitespace from column names
+    new_df.columns = new_df.columns.str.strip()
+
+    # rename columns to standardize
+    new_df = new_df.rename(
+        columns={
+            "GMTTime": "Time",
+            "GMT MKT Interval": "Time",
+            "Gas Self": "Natural Gas Self",
+            # rename below is based on documenation
+            "Load": "Short Term Load Forecast",
+        },
+    )
+
+    # parse time
+    new_df["Time"] = pd.to_datetime(new_df["Time"], utc=True).dt.tz_convert(
+        SPP.default_timezone,
+    )
+
+    # combine market and self columns
+    columns_to_combine = [
+        "Coal",
+        "Diesel Fuel Oil",
+        "Hydro",
+        "Natural Gas",
+        "Nuclear",
+        "Solar",
+        "Waste Disposal Services",
+        "Wind",
+        "Waste Heat",
+        "Other",
+    ]
+
+    if not detailed:
+        for col in columns_to_combine:
+            market_col = f"{col} Market"
+            self_col = f"{col} Self"
+
+            if market_col not in new_df.columns or self_col not in new_df.columns:
+                continue
+
+            new_df[col] = new_df[market_col] + new_df[self_col]
+            new_df = new_df.drop([market_col, self_col], axis=1)
+
+    new_df = add_interval(new_df, 5)
+
+    return new_df
+
+
 def add_interval(df, interval_min):
     """Adds Interval Start and Interval End columns to df"""
     df["Interval Start"] = df["Time"]
     df["Interval End"] = df["Interval Start"] + pd.Timedelta(minutes=interval_min)
 
     df = utils.move_cols_to_front(
         df,
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/base_test_iso.py` & `gridstatus-0.21.0/gridstatus/tests/base_test_iso.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import pytest
 from pandas.core.dtypes.common import is_numeric_dtype
 
+import gridstatus
 from gridstatus.base import GridStatus, _interconnection_columns
 
 
 class BaseTestISO:
-
     iso = None
 
     def test_init(self):
         assert self.iso is not None
 
     """get_fuel_mix"""
 
@@ -76,21 +76,48 @@
 
         df = self.iso.get_fuel_mix(date=start.date(), end=end.date())
         self._check_fuel_mix(df)
 
         # make sure right number of days are returned
         assert df["Time"].dt.day.nunique() == num_days
 
+    def test_range_two_days_with_day_start_endpoint(self):
+        yesterday = gridstatus.utils._handle_date(
+            "today",
+            self.iso.default_timezone,
+        ) - pd.Timedelta(days=1)
+        yesterday = yesterday.replace(hour=1, minute=0, second=0, microsecond=0)
+        start = yesterday - pd.Timedelta(hours=3)
+
+        # add one minute since pjm is exclusive of end date
+        # and does not include the whole day like other isos
+        df = self.iso.get_fuel_mix(start=start, end=yesterday + pd.Timedelta(minutes=1))
+
+        assert df["Time"].max() >= yesterday.replace(hour=0, minute=0, second=0)
+        assert df["Time"].min() <= start
+
+        self._check_fuel_mix(df)
+
+    def test_start_end_same_day(self):
+        yesterday = gridstatus.utils._handle_date(
+            "today",
+            self.iso.default_timezone,
+        ) - pd.Timedelta(days=1)
+        start = yesterday.replace(hour=0, minute=5, second=0, microsecond=0)
+        end = yesterday.replace(hour=6, minute=5, second=0, microsecond=0)
+        df = self.iso.get_fuel_mix(start=start, end=end)
+        # ignore last row, since it is sometime midnight of next day
+        assert df["Time"].iloc[:-1].dt.date.unique().tolist() == [yesterday.date()]
+        self._check_fuel_mix(df)
+
     def test_get_fuel_mix_latest(self):
         df = self.iso.get_fuel_mix("latest")
         assert isinstance(df, pd.DataFrame)
-        assert len(df) == 1
         assert isinstance(df.Time.iloc[0], pd.Timestamp)
         assert df.index.name is None
-        assert df.index.tolist() == [0]
         self._check_fuel_mix(df)
 
     def test_get_fuel_mix_today(self):
         df = self.iso.get_fuel_mix("today")
         self._check_fuel_mix(df)
 
     """get_interconnection_queue"""
@@ -101,14 +128,31 @@
         assert isinstance(queue, pd.DataFrame)
         assert queue.shape[0] > 0
         assert set(_interconnection_columns).issubset(queue.columns)
 
     """get_lmp"""
 
     # @pytest.mark.parametrize in ISO
+    def test_lmp_date_range(self, market=None):
+        today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
+        three_days_ago = today - pd.Timedelta(days=3)
+        df_1 = self.iso.get_lmp(
+            start=three_days_ago,
+            end=today,
+            market=market,
+        )
+        df_2 = self.iso.get_lmp(
+            date=(three_days_ago, today),
+            market=market,
+        )
+
+        self._check_lmp_columns(df_1, market)
+        assert df_1.equals(df_2)
+
+    # @pytest.mark.parametrize in ISO
     def test_get_lmp_historical(self, market=None):
         date_str = "2022-07-22"
         if market is not None:
             hist = self.iso.get_lmp(date_str, market=market)
             assert isinstance(hist, pd.DataFrame)
             self._check_lmp_columns(hist, market)
 
@@ -125,24 +169,29 @@
             df = self.iso.get_lmp("today", market=market)
             assert isinstance(df, pd.DataFrame)
             self._check_lmp_columns(df, market)
 
     """get_load"""
 
     def test_get_load_historical_with_date_range(self):
-        num_days = 7
+        num_days = 4
         end = pd.Timestamp.now(
             tz=self.iso.default_timezone,
         ) + pd.Timedelta(days=1)
         start = end - pd.Timedelta(days=num_days)
+
         data = self.iso.get_load(date=start.date(), end=end.date())
         self._check_load(data)
         # make sure right number of days are returned
         assert data["Time"].dt.day.nunique() == num_days
 
+        data_tuple = self.iso.get_load(date=(start.date(), end.date()))
+
+        assert data_tuple.equals(data)
+
     def test_get_load_historical(self):
         # pick a test date 2 weeks back
         test_date = (pd.Timestamp.now() - pd.Timedelta(days=14)).date()
 
         # date string works
         date_str = test_date.strftime("%Y%m%d")
         df = self.iso.get_load(date_str)
@@ -170,16 +219,16 @@
         assert is_numeric_dtype(type(load["load"]))
         today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
         assert load["time"].date() == today
 
     def test_get_load_today(self):
         df = self.iso.get_load("today")
         self._check_load(df)
-        today = pd.Timestamp.now(tz=self.iso.default_timezone)
-        assert (df["Time"].dt.date == today.date()).all()
+        today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
+        assert (df["Time"].dt.date == today).all()
         return df
 
     """get_load_forecast"""
 
     def test_get_load_forecast_historical(self):
         test_date = (pd.Timestamp.now() - pd.Timedelta(days=14)).date()
         forecast = self.iso.get_load_forecast(date=test_date)
@@ -216,40 +265,65 @@
 
     def test_get_storage_today(self):
         storage = self.iso.get_storage("today")
         self._check_storage(storage)
 
     """other"""
 
-    def _check_ordered_by_time(self, df):
+    def _check_ordered_by_time(self, df, col):
         assert isinstance(df, pd.DataFrame)
         assert df.shape[0] > 0
-        assert df["Interval Start"].is_monotonic_increasing
+        assert df[col].is_monotonic_increasing
 
-    def _check_time_columns(self, df):
+    def _check_time_columns(self, df, instant_or_interval="interval"):
         assert isinstance(df, pd.DataFrame)
-        time_cols = ["Time", "Interval Start", "Interval End"]
+
+        if instant_or_interval == "interval":
+            time_cols = ["Time", "Interval Start", "Interval End"]
+            ordered_by_col = "Interval Start"
+        elif instant_or_interval == "instant":
+            time_cols = ["Time"]
+            ordered_by_col = "Time"
+            assert "Interval Start" not in df.columns
+            assert "Interval End" not in df.columns
+        else:
+            raise ValueError(
+                "instant_or_interval must be 'interval' or 'instant'",
+            )
 
         assert time_cols == df.columns[: len(time_cols)].tolist()
         # check all time cols are localized timestamps
         for col in time_cols:
             assert isinstance(df.loc[0][col], pd.Timestamp)
             assert df.loc[0][col].tz is not None
 
-        self._check_ordered_by_time(df)
+        self._check_ordered_by_time(df, ordered_by_col)
 
     def _check_fuel_mix(self, df):
         assert isinstance(df, pd.DataFrame)
         assert df.columns.name is None
-        self._check_time_columns(df)
+
+        time_type = "interval"
+        if self.iso.iso_id in ["nyiso", "isone", "ercot"]:
+            time_type = "instant"
+        elif self.iso.iso_id in ["caiso", "spp", "miso", "pjm"]:
+            time_type = "interval"
+        else:
+            raise ValueError("Unknown ISO ID")
+        self._check_time_columns(df, instant_or_interval=time_type)
 
     def _check_load(self, df):
         assert isinstance(df, pd.DataFrame)
         assert df.shape[0] >= 0
-        self._check_time_columns(df)
+
+        if self.iso.iso_id in ["nyiso"]:
+            time_type = "instant"
+        elif self.iso.iso_id in ["caiso", "isone", "spp", "miso", "pjm", "ercot"]:
+            time_type = "interval"
+        self._check_time_columns(df, instant_or_interval=time_type)
         assert "Load" in df.columns
         assert is_numeric_dtype(df["Load"])
 
     def _check_forecast(self, df):
         assert set(df.columns) == set(
             [
                 "Time",
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_ercot.py` & `gridstatus-0.21.0/gridstatus/tests/test_nyiso.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,238 +1,256 @@
 import pandas as pd
 import pytest
 
 import gridstatus
-from gridstatus import Ercot, Markets, NotSupported
+from gridstatus import NYISO, Markets
 from gridstatus.tests.base_test_iso import BaseTestISO
+from gridstatus.tests.decorators import with_markets
 
 
-class TestErcot(BaseTestISO):
-    iso = Ercot()
+class TestNYISO(BaseTestISO):
+    iso = NYISO()
 
-    def test_get_as_prices(self):
-        as_cols = [
-            "Time",
-            "Interval Start",
-            "Interval End",
-            "Market",
-            "Non-Spinning Reserves",
-            "Regulation Down",
-            "Regulation Up",
-            "Responsive Reserves",
-        ]
+    """"get_capacity_prices"""
 
-        # today
-        today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
+    def test_get_capacity_prices(self):
+        # test 2022, 2023, and today
+        df = self.iso.get_capacity_prices(date="Dec 1, 2022", verbose=True)
+        assert not df.empty, "DataFrame came back empty"
 
-        df = self.iso.get_as_prices(today)
-        assert df.shape[0] >= 0
-        assert df.columns.tolist() == as_cols
-        assert df["Time"].unique()[0].date() == today
+        df = self.iso.get_capacity_prices(date="Jan 1, 2023", verbose=True)
+        assert not df.empty, "DataFrame came back empty"
 
-        date = today - pd.Timedelta(days=3)
-        df = self.iso.get_as_prices(date)
-        assert df.shape[0] >= 0
-        assert df.columns.tolist() == as_cols
-        assert df["Time"].unique()[0].date() == date
+        df = self.iso.get_capacity_prices(date="today", verbose=True)
+        assert not df.empty, "DataFrame came back empty"
 
-        date = pd.Timestamp(2022, 11, 8).date()
-        df = self.iso.get_as_prices(date, end="today")
-        assert df.shape[0] >= 0
-        assert df.columns.tolist() == as_cols
-        assert df.Time.min().date() == date
-        assert df.Time.max().date() == today
+    """get_fuel_mix"""
 
-        date = today - pd.DateOffset(days=365)
-        df = self.iso.get_as_prices(date)
+    def test_get_fuel_mix_date_range(self):
+        df = self.iso.get_fuel_mix(start="Aug 1, 2022", end="Oct 22, 2022")
         assert df.shape[0] >= 0
-        assert df.columns.tolist() == as_cols
-        assert df.Time.min().date() == date.date()
 
-        df = self.iso.get_as_prices(date, end=today)
+    def test_range_two_days_across_month(self):
+        today = gridstatus.utils._handle_date("today", self.iso.default_timezone)
+        first_day_of_month = today.replace(day=1, hour=5, minute=0, second=0)
+        last_day_of_prev_month = first_day_of_month - pd.Timedelta(days=1)
+        df = self.iso.get_fuel_mix(start=last_day_of_prev_month, end=first_day_of_month)
+
+        assert df["Time"].max() >= first_day_of_month
+        assert df["Time"].min() <= last_day_of_prev_month
+        assert df["Time"].dt.date.nunique() == 3  # 2 days + 1 day for midnight
+        self._check_fuel_mix(df)
+
+    """get_generators"""
 
-        for check_date in pd.date_range(date, today, freq="D", inclusive="left"):
-            temp = df.loc[df.Time.dt.date == check_date.date()].copy()
-            assert temp.shape[0] > 0
-
-        date = pd.Timestamp(2022, 11, 8).date()
-        end = pd.Timestamp(2022, 11, 30).date()
-        df = self.iso.get_as_prices(date, end=end)
+    # todo
+    @pytest.mark.skip(reason="Needs to be updated to 2023 data")
+    def test_get_generators(self):
+        df = self.iso.get_generators()
+        columns = [
+            "Generator Name",
+            "PTID",
+            "Subzone",
+            "Zone",
+            "Latitude",
+            "Longitude",
+        ]
+        assert set(df.columns).issuperset(set(columns))
         assert df.shape[0] >= 0
-        assert df.columns.tolist() == as_cols
-        assert max(df.Time).date() == end
-        assert min(df.Time).date() == date
 
-    """get_fuel_mix"""
+    """get_load"""
 
-    def test_get_fuel_mix(self):
-        # today
-        cols = [
+    def test_get_load_contains_zones(self):
+        df = self.iso.get_load("today")
+        nyiso_load_cols = [
             "Time",
-            "Interval Start",
-            "Interval End",
-            "Coal and Lignite",
-            "Hydro",
-            "Nuclear",
-            "Power Storage",
-            "Solar",
-            "Wind",
-            "Natural Gas",
-            "Other",
+            "Load",
+            "CAPITL",
+            "CENTRL",
+            "DUNWOD",
+            "GENESE",
+            "HUD VL",
+            "LONGIL",
+            "MHK VL",
+            "MILLWD",
+            "N.Y.C.",
+            "NORTH",
+            "WEST",
         ]
-        df = self.iso.get_fuel_mix("today")
-        self._check_fuel_mix(df)
-        assert df.shape[0] >= 0
-        assert df.columns.tolist() == cols
+        assert df.columns.tolist() == nyiso_load_cols
 
-        # latest
-        df = self.iso.get_fuel_mix("latest")
-        self._check_fuel_mix(df)
+    def test_get_load_month_range(self):
+        df = self.iso.get_load(start="2023-04-01", end="2023-05-16")
         assert df.shape[0] >= 0
-        assert df.columns.tolist() == cols
-
-    @pytest.mark.skip(reason="Not Applicable")
-    def test_get_fuel_mix_date_or_start(self):
-        pass
-
-    def test_get_fuel_mix_historical(self):
-        with pytest.raises(NotSupported):
-            super().test_get_fuel_mix_historical()
-
-    @pytest.mark.skip(reason="Not Applicable")
-    def test_get_fuel_mix_historical_with_date_range(self):
-        pass
 
     """get_lmp"""
 
-    @pytest.mark.skip(reason="Not Applicable")
-    def test_get_lmp_historical(self, markets=None):
-        pass
-
-    def test_get_load_3_days_ago(self):
-        today = pd.Timestamp.now(tz=self.iso.default_timezone).date()
-        three_days_ago = today - pd.Timedelta(days=3)
-        df = self.iso.get_load(three_days_ago)
-        self._check_load(df)
-        assert df["Time"].unique()[0].date() == three_days_ago
-
-    """get_load_forecast"""
-
-    def test_get_load_forecast_historical(self):
-        with pytest.raises(NotSupported):
-            super().test_get_load_forecast_historical()
-
-    @pytest.mark.skip(reason="Not Applicable")
-    def test_get_load_forecast_historical_with_date_range(self):
-        pass
-
-    """get_spp"""
+    @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
+    )
+    def test_lmp_date_range(self, market):
+        super().test_lmp_date_range(market=market)
+
+    @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
+        Markets.REAL_TIME_5_MIN,
+    )
+    def test_get_lmp_historical(self, market):
+        super().test_get_lmp_historical(market=market)
+
+    @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
+        Markets.REAL_TIME_5_MIN,
+    )
+    def test_get_lmp_today(self, market):
+        super().test_get_lmp_today(market=market)
+
+    @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
+        Markets.REAL_TIME_5_MIN,
+    )
+    def test_get_lmp_latest(self, market):
+        super().test_get_lmp_latest(market=market)
+
+    def test_get_lmp_historical_with_range(self):
+        start = "2021-12-01"
+        end = "2022-2-02"
+        df = self.iso.get_lmp(
+            start=start,
+            end=end,
+            market=Markets.REAL_TIME_5_MIN,
+        )
+        assert df.shape[0] >= 0
 
-    def test_get_spp_dam_latest_day_ahead_hourly_zone_should_raise_exception(self):
-        with pytest.raises(ValueError):
-            self.iso.get_spp(
-                date="latest",
-                market=Markets.DAY_AHEAD_HOURLY,
-                location_type="zone",
-            )
+    def test_get_lmp_location_type_parameter(self):
+        date = "2022-06-09"
 
-    def test_get_spp_dam_today_day_ahead_hourly_hub(self):
-        df = self.iso.get_spp(
-            date="today",
+        df_zone = self.iso.get_lmp(
+            date=date,
             market=Markets.DAY_AHEAD_HOURLY,
-            location_type="hub",
+            location_type="zone",
         )
-        self._check_ercot_spp(df, Markets.DAY_AHEAD_HOURLY, "Hub")
-
-    def test_get_spp_dam_today_day_ahead_hourly_node(self):
-        df = self.iso.get_spp(
-            date="today",
+        assert (df_zone["Location Type"] == "Zone").all()
+        df_gen = self.iso.get_lmp(
+            date=date,
             market=Markets.DAY_AHEAD_HOURLY,
-            location_type="node",
+            location_type="generator",
         )
-        self._check_ercot_spp(df, Markets.DAY_AHEAD_HOURLY, "Node")
+        assert (df_gen["Location Type"] == "Generator").all()
 
-    def test_get_spp_dam_today_day_ahead_hourly_zone(self):
-        df = self.iso.get_spp(
+        df_zone = self.iso.get_lmp(
             date="today",
             market=Markets.DAY_AHEAD_HOURLY,
             location_type="zone",
         )
-        self._check_ercot_spp(df, Markets.DAY_AHEAD_HOURLY, "Zone")
-
-    @pytest.mark.skip(reason="takes too long to run")
-    def test_get_spp_rtm_historical(self):
-        rtm = gridstatus.Ercot().get_rtm_spp(2020)
-        assert isinstance(rtm, pd.DataFrame)
-        assert len(rtm) > 0
-
-    @pytest.mark.slow
-    def test_get_spp_today_real_time_15_minutes_zone(self):
-        df = self.iso.get_spp(
+        assert (df_zone["Location Type"] == "Zone").all()
+        df_gen = self.iso.get_lmp(
             date="today",
-            market=Markets.REAL_TIME_15_MIN,
-            location_type="zone",
+            market=Markets.DAY_AHEAD_HOURLY,
+            location_type="generator",
         )
-        self._check_ercot_spp(df, Markets.REAL_TIME_15_MIN, "Zone")
+        assert (df_gen["Location Type"] == "Generator").all()
 
-    def test_get_spp_two_days_ago_day_ahead_hourly_zone(self):
-        two_days_ago = pd.Timestamp.now(
-            tz=self.iso.default_timezone,
-        ).date() - pd.Timedelta(
-            days=2,
-        )
-        df = self.iso.get_spp(
-            date=two_days_ago,
+        df_zone = self.iso.get_lmp(
+            date="latest",
             market=Markets.DAY_AHEAD_HOURLY,
             location_type="zone",
         )
-        self._check_ercot_spp(df, Markets.DAY_AHEAD_HOURLY, "Zone")
-
-    @pytest.mark.slow
-    def test_get_spp_two_days_ago_real_time_15_minutes_zone(self):
-        two_days_ago = pd.Timestamp.now(
-            tz=self.iso.default_timezone,
-        ).date() - pd.Timedelta(
-            days=2,
-        )
-        df = self.iso.get_spp(
-            date=two_days_ago,
-            market=Markets.REAL_TIME_15_MIN,
-            location_type="zone",
+        assert (df_zone["Location Type"] == "Zone").all()
+        df_gen = self.iso.get_lmp(
+            date="latest",
+            market=Markets.DAY_AHEAD_HOURLY,
+            location_type="generator",
         )
-        self._check_ercot_spp(df, Markets.REAL_TIME_15_MIN, "Zone")
+        assert (df_gen["Location Type"] == "Generator").all()
+
+        with pytest.raises(ValueError):
+            self.iso.get_lmp(
+                date="latest",
+                market=Markets.DAY_AHEAD_HOURLY,
+                location_type="dummy",
+            )
+
+    """get_loads"""
+
+    def test_get_loads(self):
+        df = self.iso.get_loads()
+        columns = [
+            "Load Name",
+            "PTID",
+            "Subzone",
+            "Zone",
+        ]
+        assert set(df.columns) == set(columns)
+        assert df.shape[0] >= 0
+
+    """get_status"""
+
+    def test_get_status_historical_status(self):
+        date = "20220609"
+        status = self.iso.get_status(date)
+        self._check_status(status)
+
+        start = "2022-05-01"
+        end = "2022-10-02"
+        status = self.iso.get_status(start=start, end=end)
+        self._check_status(status)
 
     """get_storage"""
 
     def test_get_storage_historical(self):
         with pytest.raises(NotImplementedError):
             super().test_get_storage_historical()
 
     def test_get_storage_today(self):
         with pytest.raises(NotImplementedError):
             super().test_get_storage_today()
 
+    def test_various_edt_to_est(self):
+        # number of rows hardcoded based on when this test was written. should stay same
+
+        date = "Nov 7, 2021"
+
+        df = self.iso.get_status(date=date)
+        assert df.shape[0] >= 1
+
+        df = self.iso.get_fuel_mix(date=date)
+        assert df.shape[0] >= 307
+
+        df = self.iso.get_load_forecast(date=date)
+        assert df.shape[0] >= 145
+        df = self.iso.get_lmp(date=date, market=Markets.REAL_TIME_5_MIN)
+        assert df.shape[0] >= 4605
+        df = self.iso.get_lmp(date=date, market=Markets.DAY_AHEAD_HOURLY)
+        assert df.shape[0] >= 375
+
+        df = self.iso.get_load(date=date)
+        assert df.shape[0] >= 307
+
+    def test_various_est_to_edt(self):
+        # number of rows hardcoded based on when this test was written. should stay same
+
+        date = "March 14, 2021"
+
+        df = self.iso.get_status(date=date)
+        assert df.shape[0] >= 5
+
+        df = self.iso.get_lmp(date=date, market=Markets.REAL_TIME_5_MIN)
+        assert df.shape[0] >= 4215
+
+        df = self.iso.get_lmp(date=date, market=Markets.DAY_AHEAD_HOURLY)
+        assert df.shape[0] >= 345
+
+        df = self.iso.get_load_forecast(date=date)
+        assert df.shape[0] >= 143
+
+        df = self.iso.get_fuel_mix(date=date)
+        assert df.shape[0] >= 281
+
+        df = self.iso.get_load(date=date)
+        assert df.shape[0] >= 281
+
     @staticmethod
-    def _check_ercot_spp(df, market, location_type):
-        """Common checks for SPP data:
-        - Columns
-        - One Market
-        - One Location Type
-        """
-        cols = [
-            "Time",
-            "Interval Start",
-            "Interval End",
-            "Location",
-            "Location Type",
-            "Market",
-            "SPP",
-        ]
-        assert df.shape[0] >= 0
-        assert df.columns.tolist() == cols
-        markets = df["Market"].unique()
-        assert len(markets) == 1
-        assert markets[0] == market.value
-
-        location_types = df["Location Type"].unique()
-        assert len(location_types) == 1
-        assert location_types[0] == location_type
+    def _check_status(df):
+        assert set(df.columns) == set(
+            ["Time", "Status", "Notes"],
+        )
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_gridstatus.py` & `gridstatus-0.21.0/gridstatus/tests/test_gridstatus.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_isone.py` & `gridstatus-0.21.0/gridstatus/tests/test_isone.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,18 +25,53 @@
         # nov 7 is a known data where nan values are returned
         assert not data.isna().any().any()
 
     @pytest.mark.parametrize("date", DST_BOUNDARIES)
     def test_get_fuel_mix(self, date):
         self.iso.get_fuel_mix(date=date, verbose=VERBOSE)
 
+    """get_btm_solar"""
+
+    def test_get_btm_solar(self):
+        df = self.iso.get_btm_solar(date="today", verbose=VERBOSE)
+
+        assert df.columns.tolist() == [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "BTM Solar",
+        ]
+        self._check_time_columns(df, "interval")
+
+    def test_get_btm_solar_range(self):
+        df = self.iso.get_btm_solar(
+            date=("April 12, 2023", "April 14, 2023"),
+            verbose=VERBOSE,
+        )
+
+        assert df.shape[0] == df.drop_duplicates().shape[0]
+
+        assert df.columns.tolist() == [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "BTM Solar",
+        ]
+        self._check_time_columns(df, "interval")
+
     """get_lmp"""
 
     @with_markets(
         Markets.DAY_AHEAD_HOURLY,
+    )
+    def test_lmp_date_range(self, market):
+        super().test_lmp_date_range(market=market)
+
+    @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
         Markets.REAL_TIME_5_MIN,
         Markets.REAL_TIME_HOURLY,
     )
     def test_get_lmp_historical(self, market):
         super().test_get_lmp_historical(market=market)
 
     @with_markets(
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_lmp_config.py` & `gridstatus-0.21.0/gridstatus/tests/test_lmp_config.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_miso.py` & `gridstatus-0.21.0/gridstatus/tests/test_miso.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,32 @@
         with pytest.raises(NotSupported):
             super().test_get_fuel_mix_historical()
 
     @pytest.mark.skip(reason="Not Applicable")
     def test_get_fuel_mix_historical_with_date_range(self):
         pass
 
+    @pytest.mark.skip(reason="Not Applicable")
+    def test_range_two_days_with_day_start_endpoint(self):
+        pass
+
+    @pytest.mark.skip(reason="Not Applicable")
+    def test_start_end_same_day(self):
+        pass
+
     def test_get_fuel_mix_today(self):
         with pytest.raises(NotSupported):
             super().test_get_fuel_mix_today()
 
     """get_lmp"""
 
+    @pytest.mark.skip(reason="Not Applicable")
+    def test_lmp_date_range(self, markets=None):
+        pass
+
     @with_markets(
         Markets.REAL_TIME_5_MIN,
         Markets.DAY_AHEAD_HOURLY,
     )
     def test_get_lmp_historical(self, market):
         with pytest.raises(NotSupported):
             super().test_get_lmp_historical(market)
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_pjm.py` & `gridstatus-0.21.0/gridstatus/tests/test_pjm.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
         assert len(df["Time"]) == 23  # 23 hours due to shift forwards in time
         assert (df["Time"].dt.strftime("%Y-%m-%d") == date).all()
 
     """get_lmp"""
 
     @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
+    )
+    def test_lmp_date_range(self, market):
+        super().test_lmp_date_range(market=market)
+
+    @with_markets(
         # Markets.REAL_TIME_5_MIN, # TODO reenable, but too slow
         Markets.REAL_TIME_HOURLY,
         Markets.DAY_AHEAD_HOURLY,
     )
     def test_get_lmp_historical(self, market):
         super().test_get_lmp_historical(market=market)
 
@@ -347,15 +353,15 @@
             market=m,
         )
         assert isinstance(hist, pd.DataFrame)
         self._check_lmp_columns(hist, m)
 
         # all standard
         # move a few days back to avoid late published data
-        end = pd.Timestamp.now() - pd.DateOffset(days=4)
+        end = pd.Timestamp.now().normalize() - pd.DateOffset(days=4)
         start = end - pd.DateOffset(days=1)
 
         hist = self.iso.get_lmp(
             start=start,
             end=end,
             location_type="hub",
             market=m,
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_save_to.py` & `gridstatus-0.21.0/gridstatus/tests/test_save_to.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_spp.py` & `gridstatus-0.21.0/gridstatus/tests/test_spp.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,22 +23,67 @@
         with pytest.raises(NotSupported):
             super().test_get_fuel_mix_historical()
 
     @pytest.mark.skip(reason="Not Applicable")
     def test_get_fuel_mix_historical_with_date_range(self):
         pass
 
+    @pytest.mark.skip(reason="Not Applicable")
+    def test_range_two_days_with_day_start_endpoint(self):
+        pass
+
+    @pytest.mark.skip(reason="Not Applicable")
+    def test_start_end_same_day(self):
+        pass
+
     def test_get_fuel_mix_central_time(self):
         fm = self.iso.get_fuel_mix(date="latest")
         assert fm.Time.iloc[0].tz.zone == self.iso.default_timezone
 
+    def test_get_fuel_mix_self_market(self):
+        fm = self.iso.get_fuel_mix(date="latest", detailed=True)
+
+        cols = [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "Coal Market",
+            "Coal Self",
+            "Diesel Fuel Oil Market",
+            "Diesel Fuel Oil Self",
+            "Hydro Market",
+            "Hydro Self",
+            "Natural Gas Market",
+            "Natural Gas Self",
+            "Nuclear Market",
+            "Nuclear Self",
+            "Solar Market",
+            "Solar Self",
+            "Waste Disposal Services Market",
+            "Waste Disposal Services Self",
+            "Wind Market",
+            "Wind Self",
+            "Waste Heat Market",
+            "Waste Heat Self",
+            "Other Market",
+            "Other Self",
+        ]
+
+        assert fm.columns.tolist() == cols
+
     """get_lmp"""
 
     @with_markets(
         Markets.DAY_AHEAD_HOURLY,
+    )
+    def test_lmp_date_range(self, market):
+        super().test_lmp_date_range(market=market)
+
+    @with_markets(
+        Markets.DAY_AHEAD_HOURLY,
         Markets.REAL_TIME_5_MIN,
     )
     def test_get_lmp_historical(self, market):
         super().test_get_lmp_historical(market=market)
 
     @with_markets(
         Markets.DAY_AHEAD_HOURLY,
@@ -107,15 +152,15 @@
         assert location_types[0] == location_type
 
     @pytest.mark.parametrize(
         "date,market,location_type",
         [
             ("latest", Markets.REAL_TIME_15_MIN, "Interface"),
             (
-                pd.Timestamp.now() - pd.Timedelta(days=2),
+                pd.Timestamp.now().normalize() - pd.Timedelta(days=2),
                 Markets.REAL_TIME_15_MIN,
                 "Interface",
             ),
         ],
     )
     def test_get_lmp_unsupported_raises_not_supported(
         self,
@@ -292,7 +337,42 @@
             status = self.iso._get_status_from_html(
                 contents,
                 year_hint=year_hint,
             )
         except Exception as e:
             raise Exception(f"Error parsing {filename}: {e}")
         return status
+
+    """ get_ver_curtailment """
+
+    def _check_ver_curtailments(self, df):
+        assert isinstance(df, pd.DataFrame)
+
+        assert df.columns.tolist() == [
+            "Time",
+            "Interval Start",
+            "Interval End",
+            "Wind Redispatch Curtailments",
+            "Wind Manual Curtailments",
+            "Wind Curtailed For Energy",
+            "Solar Redispatch Curtailments",
+            "Solar Manual Curtailments",
+            "Solar Curtailed For Energy",
+        ]
+
+    def test_get_ver_curtailments_historical(self):
+        two_days_ago = pd.Timestamp.now() - pd.Timedelta(days=2)
+        start = two_days_ago - pd.Timedelta(days=2)
+        df = self.iso.get_ver_curtailments(start=start, end=two_days_ago)
+
+        assert df["Interval Start"].min().date() == start.date()
+        assert df["Interval Start"].max().date() == two_days_ago.date()
+        self._check_ver_curtailments(df)
+
+    def test_get_get_ver_curtailments_annual(self):
+        year = 2020
+        df = self.iso.get_ver_curtailments_annual(year=year)
+
+        assert df["Interval Start"].min().date() == pd.Timestamp(f"{year}-01-01").date()
+        assert df["Interval Start"].max().date() == pd.Timestamp(f"{year}-12-31").date()
+
+        self._check_ver_curtailments(df)
```

### Comparing `gridstatus-0.20.0/gridstatus/tests/test_viz.py` & `gridstatus-0.21.0/gridstatus/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/gridstatus/utils.py` & `gridstatus-0.21.0/gridstatus/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import requests
 import tqdm
 
 import gridstatus
 from gridstatus.base import Markets, NotSupported, _interconnection_columns
 from gridstatus.caiso import CAISO
 from gridstatus.ercot import Ercot
+from gridstatus.gs_logging import log
 from gridstatus.isone import ISONE
 from gridstatus.lmp_config import lmp_config
 from gridstatus.miso import MISO
 from gridstatus.nyiso import NYISO
 from gridstatus.pjm import PJM
 from gridstatus.spp import SPP
 
@@ -98,16 +99,20 @@
 def _handle_date(date, tz=None):
     if date == "today":
         date = pd.Timestamp.now(tz=tz).normalize()
 
     if not isinstance(date, pd.Timestamp):
         date = pd.to_datetime(date)
 
-    if tz and date.tzinfo is None:
-        date = date.tz_localize(tz)
+    if tz:
+        if date.tzinfo is None:
+            date = date.tz_localize(tz)
+        else:
+            # todo see if this triggers in tests
+            date = date.tz_convert(tz)
 
     return date
 
 
 LMP_METHOD_NAMES = ["get_lmp", "get_spp"]
 
 
@@ -160,36 +165,54 @@
     )
 
     transposed = transposed.sort_index().applymap(convert_bool_to_emoji)
 
     return transposed.to_markdown() + "\n"
 
 
-def filter_lmp_locations(df, locations):
+# todo require locations and location_type arguments
+
+
+def filter_lmp_locations(df, locations=None, location_type=None):
     """
     Filters DataFrame by locations, which can be a list, "ALL" or None
 
     Arguments:
         df (pandas.DataFrame): DataFrame to filter
         locations: "ALL" or list of locations to filter "Location" column by
     """
-    if locations == "ALL" or locations is None:
-        return df
+    if location_type != "ALL" and location_type is not None:
+        if isinstance(location_type, str):
+            location_type = [location_type]
+
+        df = df[df["Location Type"].isin(location_type)]
 
-    return df[df["Location"].isin(locations)]
+    if locations != "ALL" and locations is not None:
+        df = df[df["Location"].isin(locations)]
 
+    return df
 
-def get_zip_file(url):
+
+def get_zip_file(url, verbose=False):
     # todo add retry logic
     # todo does this need to be a with statement?
+    log(f"Downloading {url}", verbose=verbose)
     r = requests.get(url)
     z = ZipFile(io.BytesIO(r.content))
     return z.open(z.namelist()[0])
 
 
+def get_zip_folder(zip_url, verbose=False):
+    msg = f"Requesting {zip_url}"
+    log(msg, verbose)
+    r = requests.get(zip_url)
+    z = ZipFile(io.BytesIO(r.content))
+    return z
+
+
 def is_today(date, tz):
     return _handle_date(date, tz=tz).date() == pd.Timestamp.now(tz=tz).date()
 
 
 def is_within_last_days(date, days, tz):
     """Returns whether date is within N days"""
     now = pd.Timestamp.now(tz=tz).date()
@@ -242,18 +265,19 @@
     dfs = []
     for f in tqdm.tqdm(all_files, disable=not verbose):
         df = pd.read_csv(f, parse_dates=True)
         dfs.append(df)
 
     data = pd.concat(dfs).reset_index(drop=True)
 
-    if "Time" in data.columns:
-        data["Time"] = pd.to_datetime(data["Time"], utc=True)
-        if time_zone:
-            data["Time"] = data["Time"].dt.tz_convert(time_zone)
+    for time_col in ["Time", "Interval Start", "Interval End"]:
+        if time_col in data.columns:
+            data[time_col] = pd.to_datetime(data[time_col], utc=True)
+            if time_zone:
+                data[time_col] = data[time_col].dt.tz_convert(time_zone)
 
     # todo make sure dates get parsed
     # todo make sure rows are sorted by time
 
     return data
```

### Comparing `gridstatus-0.20.0/gridstatus/viz.py` & `gridstatus-0.21.0/gridstatus/viz.py`

 * *Files identical despite different names*

### Comparing `gridstatus-0.20.0/gridstatus.egg-info/PKG-INFO` & `gridstatus-0.21.0/gridstatus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatus
-Version: 0.20.0
+Version: 0.21.0
 Summary: API to access energy data
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -34,38 +34,38 @@
 License-File: LICENSE
 
 <p align="center">
 <img width=75% src="/gridstatus-header.png" alt="gridstatus logo" />
 </p>
 
 <p align="center">
-    <a href="https://github.com/kmax12/gridstatus/actions?query=branch%3Amain+workflow%3ATests" target="_blank">
+    <!-- disable until tests more reliable -->
+    <!-- <a href="https://github.com/kmax12/gridstatus/actions?query=branch%3Amain+workflow%3ATests" target="_blank">
         <img src="https://github.com/kmax12/gridstatus/workflows/Tests/badge.svg?branch=main" alt="Tests" />
-    </a>
+    </a> -->
     <a href="https://codecov.io/gh/kmax12/gridstatus" target="_blank">
         <img src="https://codecov.io/gh/kmax12/gridstatus/branch/main/graph/badge.svg" alt="Code Coverage"//>
     </a>
     <a href="https://badge.fury.io/py/gridstatus" target="_blank">
         <img src="https://badge.fury.io/py/gridstatus.svg?maxAge=2592000" alt="PyPI version">
     </a>
 </p>
 
 `gridstatus` is a Python library that provides a uniform API for accessing electricity supply, demand, and pricing data for the major Independent System Operators (ISOs) in the United States. It currently supports data from CAISO, SPP, ISONE, MISO, Ercot, NYISO, and PJM.
 
-
 ## GridStatus.io
 
 To preview some the data this library provide access to, visit [GridStatus.io](https://www.gridstatus.io/).
 
 ## Community
 
-* Need Help? Post a [GitHub issue](https://github.com/kmax12/gridstatus/issues) 
-* Want to chat? Join our [Slack](https://join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
-* Want to stay updated? Follow us on Twitter [@grid_status](https://twitter.com/grid_status)
-* Want to contribute? Read our [Contributing Guide](CONTRIBUTING.md)
+- Need Help? Post a [GitHub issue](https://github.com/kmax12/gridstatus/issues)
+- Want to chat? Join our [Slack](https://join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
+- Want to stay updated? Follow us on Twitter [@grid_status](https://twitter.com/grid_status)
+- Want to contribute? Read our [Contributing Guide](CONTRIBUTING.md)
 
 ## Installation
 
 `gridstatus` supports python 3.8+. Install with pip
 
 ```
 python -m pip install gridstatus
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gridstatus Version: 0.20.0 Summary: API to access
+Metadata-Version: 2.1 Name: gridstatus Version: 0.21.0 Summary: API to access
 energy data Author-email: Max Kanter
 gmail.com> Maintainer-email: Max Kanter
 gmail.com> License: Copyright 2022 James Max Kanter Redistribution and use in
 source and binary forms, with or without modification, are permitted provided
 that the following conditions are met: 1. Redistributions of source code must
 retain the above copyright notice, this list of conditions and the following
 disclaimer. 2. Redistributions in binary form must reproduce the above
@@ -27,26 +27,26 @@
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: <4,>=3.8 Description-
 Content-Type: text/markdown Provides-Extra: test Provides-Extra: dev Provides-
 Extra: docs License-File: LICENSE
                                [gridstatus logo]
-                                   [Tests] >
+                                        >
  [PyPI_version]
 `gridstatus` is a Python library that provides a uniform API for accessing
 electricity supply, demand, and pricing data for the major Independent System
 Operators (ISOs) in the United States. It currently supports data from CAISO,
 SPP, ISONE, MISO, Ercot, NYISO, and PJM. ## GridStatus.io To preview some the
 data this library provide access to, visit [GridStatus.io](https://
-www.gridstatus.io/). ## Community * Need Help? Post a [GitHub issue](https://
-github.com/kmax12/gridstatus/issues) * Want to chat? Join our [Slack](https://
+www.gridstatus.io/). ## Community - Need Help? Post a [GitHub issue](https://
+github.com/kmax12/gridstatus/issues) - Want to chat? Join our [Slack](https://
 join.slack.com/t/gridstatus/shared_invite/zt-1jk6vlzt2-Lzz4pdpjkJYVUJkynOiIvQ)
-* Want to stay updated? Follow us on Twitter [@grid_status](https://
-twitter.com/grid_status) * Want to contribute? Read our [Contributing Guide]
+- Want to stay updated? Follow us on Twitter [@grid_status](https://
+twitter.com/grid_status) - Want to contribute? Read our [Contributing Guide]
 (CONTRIBUTING.md) ## Installation `gridstatus` supports python 3.8+. Install
 with pip ``` python -m pip install gridstatus ``` Upgrade using the following
 command ``` python -m pip install --upgrade gridstatus ``` ## Documentation and
 Examples To learn more, visit the [documentation](https://docs.gridstatus.io/
 ) and view [example notebooks](https://docs.gridstatus.io/en/latest/Examples/
 index.html). ## Get Help We'd love to answer any usage or data access
 questions! Please let us know by posting a GitHub issue.
```

### Comparing `gridstatus-0.20.0/gridstatus.egg-info/SOURCES.txt` & `gridstatus-0.21.0/gridstatus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 pyproject.toml
 docs/conf.py
 docs/update_docs.py
 gridstatus/__init__.py
 gridstatus/base.py
 gridstatus/caiso.py
 gridstatus/decorators.py
+gridstatus/eia.py
 gridstatus/ercot.py
+gridstatus/gs_logging.py
 gridstatus/isone.py
 gridstatus/lmp_config.py
-gridstatus/logging.py
 gridstatus/miso.py
 gridstatus/nyiso.py
 gridstatus/pjm.py
 gridstatus/spp.py
 gridstatus/test.py
 gridstatus/utils.py
 gridstatus/version.py
@@ -25,14 +26,15 @@
 gridstatus.egg-info/requires.txt
 gridstatus.egg-info/top_level.txt
 gridstatus/tests/__init__.py
 gridstatus/tests/base_test_iso.py
 gridstatus/tests/conftest.py
 gridstatus/tests/decorators.py
 gridstatus/tests/test_caiso.py
+gridstatus/tests/test_eia.py
 gridstatus/tests/test_ercot.py
 gridstatus/tests/test_gridstatus.py
 gridstatus/tests/test_interconnection_queue.py
 gridstatus/tests/test_isone.py
 gridstatus/tests/test_lmp_config.py
 gridstatus/tests/test_logger.py
 gridstatus/tests/test_miso.py
```

### Comparing `gridstatus-0.20.0/gridstatus.egg-info/requires.txt` & `gridstatus-0.21.0/gridstatus.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 beautifulsoup4>=4.8.13
 tabulate>=0.8.10
 tqdm>=4.64.1
 openpyxl>=3.1.0
 tabula-py>=2.5.1
 lxml>=4.9.1
 plotly>=5.11.0
+termcolor>=2.2.0
 
 [dev]
 ruff==0.0.202
 black[jupyter]==22.12.0
 pre-commit==2.21.0
 
 [docs]
```

### Comparing `gridstatus-0.20.0/pyproject.toml` & `gridstatus-0.21.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "beautifulsoup4 >= 4.8.13",
     "tabulate >= 0.8.10",
     "tqdm >= 4.64.1",
     "openpyxl >= 3.1.0",
     "tabula-py >= 2.5.1",
     "lxml >= 4.9.1",
     "plotly >= 5.11.0",
+    "termcolor >= 2.2.0",
 ]
 
 [project.urls]
 "Source Code"= "https://github.com/kmax12/gridstatus/"
 "Changes" = "https://github.com/kmax12/gridstatus/blob/main/CHANGELOG.md"
 "Issue Tracker" = "https://github.com/kmax12/gridstatus/issues"
```

### Comparing `gridstatus-0.20.0/utils/ercot/README.md` & `gridstatus-0.21.0/utils/ercot/README.md`

 * *Files identical despite different names*

