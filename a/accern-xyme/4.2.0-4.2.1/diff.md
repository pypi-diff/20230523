# Comparing `tmp/accern_xyme-4.2.0.tar.gz` & `tmp/accern_xyme-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accern_xyme-4.2.0.tar", last modified: Thu Jul 21 16:08:38 2022, max compression
+gzip compressed data, was "accern_xyme-4.2.1.tar", last modified: Tue May 23 09:25:43 2023, max compression
```

## Comparing `accern_xyme-4.2.0.tar` & `accern_xyme-4.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.170978 accern_xyme-4.2.0/
--rw-r--r--   0 josuakrause   (503) staff       (20)     1079 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/LICENSE
--rw-r--r--   0 josuakrause   (503) staff       (20)       35 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/MANIFEST.in
--rw-r--r--   0 josuakrause   (503) staff       (20)     1598 2022-07-21 16:08:38.171049 accern_xyme-4.2.0/PKG-INFO
--rw-r--r--   0 josuakrause   (503) staff       (20)      874 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/README.rst
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.166897 accern_xyme-4.2.0/packages/
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.167012 accern_xyme-4.2.0/packages/python/
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.168925 accern_xyme-4.2.0/packages/python/accern_xyme/
--rw-r--r--   0 josuakrause   (503) staff       (20)      280 2022-07-21 15:48:09.000000 accern_xyme-4.2.0/packages/python/accern_xyme/__init__.py
--rw-r--r--   0 josuakrause   (503) staff       (20)     1087 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/__main__.py
--rw-r--r--   0 josuakrause   (503) staff       (20)   110626 2022-07-21 15:48:09.000000 accern_xyme-4.2.0/packages/python/accern_xyme/accern_xyme.py
--rw-r--r--   0 josuakrause   (503) staff       (20)        0 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/py.typed
--rw-r--r--   0 josuakrause   (503) staff       (20)    11301 2022-04-22 13:40:55.000000 accern_xyme-4.2.0/packages/python/accern_xyme/types.py
--rw-r--r--   0 josuakrause   (503) staff       (20)    17611 2022-07-21 15:48:09.000000 accern_xyme-4.2.0/packages/python/accern_xyme/util.py
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.169988 accern_xyme-4.2.0/packages/python/accern_xyme/v2/
--rw-r--r--   0 josuakrause   (503) staff       (20)       36 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v2/__init__.py
--rw-r--r--   0 josuakrause   (503) staff       (20)   101344 2022-07-21 15:48:09.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v2/legacy.py
--rw-r--r--   0 josuakrause   (503) staff       (20)     3611 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v2/util.py
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.170837 accern_xyme-4.2.0/packages/python/accern_xyme/v3/
--rw-r--r--   0 josuakrause   (503) staff       (20)       41 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v3/__init__.py
--rw-r--r--   0 josuakrause   (503) staff       (20)    90939 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v3/accern_xyme.py
--rw-r--r--   0 josuakrause   (503) staff       (20)     7581 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v3/types.py
--rw-r--r--   0 josuakrause   (503) staff       (20)    13310 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/packages/python/accern_xyme/v3/util.py
-drwxr-xr-x   0 josuakrause   (503) staff       (20)        0 2022-07-21 16:08:38.169526 accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/
--rw-r--r--   0 josuakrause   (503) staff       (20)     1598 2022-07-21 16:08:38.000000 accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/PKG-INFO
--rw-r--r--   0 josuakrause   (503) staff       (20)      827 2022-07-21 16:08:38.000000 accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/SOURCES.txt
--rw-r--r--   0 josuakrause   (503) staff       (20)        1 2022-07-21 16:08:38.000000 accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/dependency_links.txt
--rw-r--r--   0 josuakrause   (503) staff       (20)      174 2022-07-21 16:08:38.000000 accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/requires.txt
--rw-r--r--   0 josuakrause   (503) staff       (20)       12 2022-07-21 16:08:38.000000 accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/top_level.txt
--rw-r--r--   0 josuakrause   (503) staff       (20)     1168 2022-07-21 16:08:38.171365 accern_xyme-4.2.0/setup.cfg
--rw-r--r--   0 josuakrause   (503) staff       (20)      115 2022-01-11 03:16:58.000000 accern_xyme-4.2.0/setup.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.900720 accern_xyme-4.2.1/
+-rw-r--r--   0 shaunak    (501) staff       (20)     1079 2020-09-03 14:18:00.000000 accern_xyme-4.2.1/LICENSE
+-rw-r--r--   0 shaunak    (501) staff       (20)       35 2020-09-03 14:18:00.000000 accern_xyme-4.2.1/MANIFEST.in
+-rw-r--r--   0 shaunak    (501) staff       (20)     1653 2023-05-23 09:25:43.900885 accern_xyme-4.2.1/PKG-INFO
+-rw-r--r--   0 shaunak    (501) staff       (20)      929 2022-10-26 17:37:21.000000 accern_xyme-4.2.1/README.rst
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.884321 accern_xyme-4.2.1/packages/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.884716 accern_xyme-4.2.1/packages/python/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.891156 accern_xyme-4.2.1/packages/python/accern_xyme/
+-rw-r--r--   0 shaunak    (501) staff       (20)      280 2022-09-21 12:21:43.000000 accern_xyme-4.2.1/packages/python/accern_xyme/__init__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     1087 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/__main__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)   116150 2023-05-23 09:23:01.000000 accern_xyme-4.2.1/packages/python/accern_xyme/accern_xyme.py
+-rw-r--r--   0 shaunak    (501) staff       (20)        0 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/py.typed
+-rw-r--r--   0 shaunak    (501) staff       (20)    11609 2023-05-23 09:23:01.000000 accern_xyme-4.2.1/packages/python/accern_xyme/types.py
+-rw-r--r--   0 shaunak    (501) staff       (20)    17611 2022-09-13 13:43:15.000000 accern_xyme-4.2.1/packages/python/accern_xyme/util.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.896698 accern_xyme-4.2.1/packages/python/accern_xyme/v2/
+-rw-r--r--   0 shaunak    (501) staff       (20)       36 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v2/__init__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)   101344 2022-09-13 13:43:15.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v2/legacy.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     3611 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v2/util.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.899771 accern_xyme-4.2.1/packages/python/accern_xyme/v3/
+-rw-r--r--   0 shaunak    (501) staff       (20)       41 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v3/__init__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)    90939 2021-09-07 08:25:52.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v3/accern_xyme.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     7581 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v3/types.py
+-rw-r--r--   0 shaunak    (501) staff       (20)    13310 2021-05-06 11:02:37.000000 accern_xyme-4.2.1/packages/python/accern_xyme/v3/util.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-05-23 09:25:43.894102 accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/
+-rw-r--r--   0 shaunak    (501) staff       (20)     1653 2023-05-23 09:25:43.000000 accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/PKG-INFO
+-rw-r--r--   0 shaunak    (501) staff       (20)      827 2023-05-23 09:25:43.000000 accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)        1 2023-05-23 09:25:43.000000 accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)      174 2023-05-23 09:25:43.000000 accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/requires.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)       12 2023-05-23 09:25:43.000000 accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/top_level.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)     1168 2023-05-23 09:25:43.901852 accern_xyme-4.2.1/setup.cfg
+-rw-r--r--   0 shaunak    (501) staff       (20)      115 2021-03-12 08:04:24.000000 accern_xyme-4.2.1/setup.py
```

### Comparing `accern_xyme-4.2.0/LICENSE` & `accern_xyme-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/PKG-INFO` & `accern_xyme-4.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accern_xyme
-Version: 4.2.0
+Version: 4.2.1
 Summary: AccernXYME is a library for easily accessing XYME via python.
 Home-page: https://github.com/Accern/accern-xyme
 Author: Accern Corp.
 Author-email: josua.krause@accern.com
 License: MIT
 Keywords: XYME AI machine learning client
 Classifier: Development Status :: 4 - Beta
@@ -19,18 +19,18 @@
 License-File: LICENSE
 
 Accern-XYME
 ===========
 
 *accern\_xyme* is a python/typescript library for accessing XYME functionality.
 
-|CircleCI|
+|GHAction|
 
-.. |CircleCI| image:: https://circleci.com/gh/Accern/accern-xyme.svg?style=svg
-   :target: https://circleci.com/gh/Accern/accern-xyme
+.. |GHAction| image:: https://github.com/Accern/accern-xyme/actions/workflows/python-app.yaml/badge.svg
+   :target: https://github.com/Accern/accern-xyme/actions/workflows/python-app.yaml/
 
 Python Usage
 ------------
 
 You can install *accern\_xyme* with pip:
 
 .. code:: sh
```

### Comparing `accern_xyme-4.2.0/README.rst` & `accern_xyme-4.2.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Accern-XYME
 ===========
 
 *accern\_xyme* is a python/typescript library for accessing XYME functionality.
 
-|CircleCI|
+|GHAction|
 
-.. |CircleCI| image:: https://circleci.com/gh/Accern/accern-xyme.svg?style=svg
-   :target: https://circleci.com/gh/Accern/accern-xyme
+.. |GHAction| image:: https://github.com/Accern/accern-xyme/actions/workflows/python-app.yaml/badge.svg
+   :target: https://github.com/Accern/accern-xyme/actions/workflows/python-app.yaml/
 
 Python Usage
 ------------
 
 You can install *accern\_xyme* with pip:
 
 .. code:: sh
```

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/__main__.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/__main__.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/accern_xyme.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/accern_xyme.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,6911 +5,7256 @@
 00000040: 7479 7069 6e67 2069 6d70 6f72 7420 280a  typing import (.
 00000050: 2020 2020 416e 792c 0a20 2020 2043 616c      Any,.    Cal
 00000060: 6c61 626c 652c 0a20 2020 2063 6173 742c  lable,.    cast,
 00000070: 0a20 2020 2044 6963 742c 0a20 2020 2049  .    Dict,.    I
 00000080: 4f2c 0a20 2020 2049 7465 7261 626c 652c  O,.    Iterable,
 00000090: 0a20 2020 2049 7465 7261 746f 722c 0a20  .    Iterator,. 
 000000a0: 2020 204c 6973 742c 0a20 2020 204f 7074     List,.    Opt
-000000b0: 696f 6e61 6c2c 0a20 2020 206f 7665 726c  ional,.    overl
-000000c0: 6f61 642c 0a20 2020 2053 6574 2c0a 2020  oad,.    Set,.  
-000000d0: 2020 5465 7874 494f 2c0a 2020 2020 5475    TextIO,.    Tu
-000000e0: 706c 652c 0a20 2020 2054 5950 455f 4348  ple,.    TYPE_CH
-000000f0: 4543 4b49 4e47 2c0a 2020 2020 556e 696f  ECKING,.    Unio
-00000100: 6e2c 0a29 0a69 6d70 6f72 7420 696f 0a69  n,.).import io.i
-00000110: 6d70 6f72 7420 6f73 0a69 6d70 6f72 7420  mport os.import 
-00000120: 7069 636b 6c65 0a69 6d70 6f72 7420 7379  pickle.import sy
-00000130: 730a 696d 706f 7274 206a 736f 6e0a 696d  s.import json.im
-00000140: 706f 7274 2074 696d 650a 696d 706f 7274  port time.import
-00000150: 2077 6561 6b72 6566 0a69 6d70 6f72 7420   weakref.import 
-00000160: 696e 7370 6563 740a 696d 706f 7274 2074  inspect.import t
-00000170: 6578 7477 7261 700a 696d 706f 7274 2074  extwrap.import t
-00000180: 6872 6561 6469 6e67 0a69 6d70 6f72 7420  hreading.import 
-00000190: 636f 6e74 6578 746c 6962 0a66 726f 6d20  contextlib.from 
-000001a0: 696f 2069 6d70 6f72 7420 4279 7465 7349  io import BytesI
-000001b0: 4f2c 2053 7472 696e 6749 4f0a 6672 6f6d  O, StringIO.from
-000001c0: 2075 726c 6c69 622e 7061 7273 6520 696d   urllib.parse im
-000001d0: 706f 7274 2075 726c 7061 7273 652c 2075  port urlparse, u
-000001e0: 726c 756e 7061 7273 650a 6672 6f6d 2070  rlunparse.from p
-000001f0: 6174 686c 6962 2069 6d70 6f72 7420 506f  athlib import Po
-00000200: 7369 7850 6174 682c 2050 7572 6550 6174  sixPath, PurePat
-00000210: 680a 6672 6f6d 2067 7261 7068 7669 7a2e  h.from graphviz.
-00000220: 6261 636b 656e 6420 696d 706f 7274 2045  backend import E
-00000230: 7865 6375 7461 626c 654e 6f74 466f 756e  xecutableNotFoun
-00000240: 640a 696d 706f 7274 2070 616e 6461 7320  d.import pandas 
-00000250: 6173 2070 640a 696d 706f 7274 2072 6571  as pd.import req
-00000260: 7565 7374 730a 6672 6f6d 2072 6571 7565  uests.from reque
-00000270: 7374 7320 696d 706f 7274 2052 6573 706f  sts import Respo
-00000280: 6e73 650a 6672 6f6d 2072 6571 7565 7374  nse.from request
-00000290: 732e 6578 6365 7074 696f 6e73 2069 6d70  s.exceptions imp
-000002a0: 6f72 7420 4854 5450 4572 726f 722c 2052  ort HTTPError, R
-000002b0: 6571 7565 7374 4578 6365 7074 696f 6e0a  equestException.
-000002c0: 6672 6f6d 2074 7970 696e 675f 6578 7465  from typing_exte
-000002d0: 6e73 696f 6e73 2069 6d70 6f72 7420 4c69  nsions import Li
-000002e0: 7465 7261 6c0a 696d 706f 7274 2071 7569  teral.import qui
-000002f0: 636b 5f73 6572 7665 720a 0a66 726f 6d20  ck_server..from 
-00000300: 2e75 7469 6c20 696d 706f 7274 2028 0a20  .util import (. 
-00000310: 2020 2061 7379 6e63 5f63 6f6d 7075 7465     async_compute
-00000320: 2c0a 2020 2020 4279 7465 5265 7370 6f6e  ,.    ByteRespon
-00000330: 7365 2c0a 2020 2020 636f 6d70 7574 655f  se,.    compute_
-00000340: 7061 7261 6c6c 656c 2c0a 2020 2020 636f  parallel,.    co
-00000350: 6e74 656e 745f 746f 5f63 7376 5f62 7974  ntent_to_csv_byt
-00000360: 6573 2c0a 2020 2020 6466 5f74 6f5f 6373  es,.    df_to_cs
-00000370: 765f 6279 7465 732c 0a20 2020 2067 6574  v_bytes,.    get
-00000380: 5f61 6765 2c0a 2020 2020 6765 745f 6669  _age,.    get_fi
-00000390: 6c65 5f68 6173 682c 0a20 2020 2067 6574  le_hash,.    get
-000003a0: 5f66 696c 655f 7570 6c6f 6164 5f63 6875  _file_upload_chu
-000003b0: 6e6b 5f73 697a 652c 0a20 2020 2067 6574  nk_size,.    get
-000003c0: 5f6d 6178 5f72 6574 7279 2c0a 2020 2020  _max_retry,.    
-000003d0: 6765 745f 7072 6f67 7265 7373 5f62 6172  get_progress_bar
-000003e0: 2c0a 2020 2020 6765 745f 7265 7472 795f  ,.    get_retry_
-000003f0: 736c 6565 702c 0a20 2020 2068 6173 5f67  sleep,.    has_g
-00000400: 7261 7068 5f65 6173 792c 0a20 2020 2069  raph_easy,.    i
-00000410: 6e74 6572 7072 6574 5f63 7479 7065 2c0a  nterpret_ctype,.
-00000420: 2020 2020 6973 5f6a 7570 7974 6572 2c0a      is_jupyter,.
-00000430: 2020 2020 6d61 7962 655f 6a73 6f6e 5f6c      maybe_json_l
-00000440: 6f61 6473 2c0a 2020 2020 6d65 7267 655f  oads,.    merge_
-00000450: 6374 7970 652c 0a20 2020 2073 6166 655f  ctype,.    safe_
-00000460: 6f70 745f 6e75 6d2c 0a20 2020 2053 6572  opt_num,.    Ser
-00000470: 7665 7253 6964 6545 7272 6f72 2c0a 2020  verSideError,.  
-00000480: 2020 746f 5f62 6f6f 6c2c 0a29 0a66 726f    to_bool,.).fro
-00000490: 6d20 2e74 7970 6573 2069 6d70 6f72 7420  m .types import 
-000004a0: 280a 2020 2020 416c 6c6f 7765 6443 7573  (.    AllowedCus
-000004b0: 746f 6d49 6d70 6f72 7473 2c0a 2020 2020  tomImports,.    
-000004c0: 4261 7365 4461 6744 6566 2c0a 2020 2020  BaseDagDef,.    
-000004d0: 426c 6f62 4465 7461 696c 732c 0a20 2020  BlobDetails,.   
-000004e0: 2042 6c6f 6246 696c 6573 5265 7370 6f6e   BlobFilesRespon
-000004f0: 7365 2c0a 2020 2020 426c 6f62 496e 6974  se,.    BlobInit
-00000500: 2c0a 2020 2020 426c 6f62 4f77 6e65 722c  ,.    BlobOwner,
-00000510: 0a20 2020 2042 6c6f 6254 7970 6552 6573  .    BlobTypeRes
-00000520: 706f 6e73 652c 0a20 2020 2042 6c6f 6255  ponse,.    BlobU
-00000530: 5249 5265 7370 6f6e 7365 2c0a 2020 2020  RIResponse,.    
-00000540: 4361 6368 6553 7461 7473 2c0a 2020 2020  CacheStats,.    
-00000550: 436f 7079 426c 6f62 2c0a 2020 2020 4461  CopyBlob,.    Da
-00000560: 6743 7265 6174 652c 0a20 2020 2044 6167  gCreate,.    Dag
-00000570: 4465 662c 0a20 2020 2044 6167 4475 7052  Def,.    DagDupR
-00000580: 6573 706f 6e73 652c 0a20 2020 2044 6167  esponse,.    Dag
-00000590: 496e 666f 2c0a 2020 2020 4461 6749 6e69  Info,.    DagIni
-000005a0: 742c 0a20 2020 2044 6167 4c69 7374 2c0a  t,.    DagList,.
-000005b0: 2020 2020 4461 6750 7265 7474 794e 6f64      DagPrettyNod
-000005c0: 652c 0a20 2020 2044 6167 5265 6c6f 6164  e,.    DagReload
-000005d0: 2c0a 2020 2020 4461 6753 7461 7475 732c  ,.    DagStatus,
-000005e0: 0a20 2020 2044 656c 6574 6542 6c6f 6252  .    DeleteBlobR
-000005f0: 6573 706f 6e73 652c 0a20 2020 2044 796e  esponse,.    Dyn
-00000600: 616d 6963 5265 7375 6c74 732c 0a20 2020  amicResults,.   
-00000610: 2044 796e 616d 6963 5374 6174 7573 5265   DynamicStatusRe
-00000620: 7370 6f6e 7365 2c0a 2020 2020 4553 5175  sponse,.    ESQu
-00000630: 6572 7952 6573 706f 6e73 652c 0a20 2020  eryResponse,.   
-00000640: 2046 696c 654d 6170 2c0a 2020 2020 466c   FileMap,.    Fl
-00000650: 7573 6841 6c6c 5175 6575 6573 5265 7370  ushAllQueuesResp
-00000660: 6f6e 7365 2c0a 2020 2020 496e 4375 7273  onse,.    InCurs
-00000670: 6f72 732c 0a20 2020 2049 6e73 7461 6e63  ors,.    Instanc
-00000680: 6553 7461 7475 732c 0a20 2020 204a 534f  eStatus,.    JSO
-00000690: 4e42 6c6f 6241 7070 656e 6452 6573 706f  NBlobAppendRespo
-000006a0: 6e73 652c 0a20 2020 204b 6166 6b61 4772  nse,.    KafkaGr
-000006b0: 6f75 702c 0a20 2020 204b 6166 6b61 4d65  oup,.    KafkaMe
-000006c0: 7373 6167 652c 0a20 2020 204b 6166 6b61  ssage,.    Kafka
-000006d0: 4f66 6673 6574 732c 0a20 2020 204b 6166  Offsets,.    Kaf
-000006e0: 6b61 5468 726f 7567 6870 7574 2c0a 2020  kaThroughput,.  
-000006f0: 2020 4b61 666b 6154 6f70 6963 4e61 6d65    KafkaTopicName
-00000700: 732c 0a20 2020 204b 6166 6b61 546f 7069  s,.    KafkaTopi
-00000710: 6373 2c0a 2020 2020 4b6e 6f77 6e42 6c6f  cs,.    KnownBlo
-00000720: 6273 2c0a 2020 2020 4d69 6e69 6d61 6c51  bs,.    MinimalQ
-00000730: 7565 7565 5374 6174 7352 6573 706f 6e73  ueueStatsRespons
-00000740: 652c 0a20 2020 204d 6f64 656c 496e 666f  e,.    ModelInfo
-00000750: 2c0a 2020 2020 4d6f 6465 6c50 6172 616d  ,.    ModelParam
-00000760: 7352 6573 706f 6e73 652c 0a20 2020 204d  sResponse,.    M
-00000770: 6f64 656c 5265 6c65 6173 6552 6573 706f  odelReleaseRespo
-00000780: 6e73 652c 0a20 2020 204d 6f64 656c 5665  nse,.    ModelVe
-00000790: 7273 696f 6e52 6573 706f 6e73 652c 0a20  rsionResponse,. 
-000007a0: 2020 204e 616d 6573 7061 6365 4c69 7374     NamespaceList
-000007b0: 2c0a 2020 2020 4e61 6d65 7370 6163 6555  ,.    NamespaceU
-000007c0: 7064 6174 6553 6574 7469 6e67 732c 0a20  pdateSettings,. 
-000007d0: 2020 204e 6f64 6543 6875 6e6b 2c0a 2020     NodeChunk,.  
-000007e0: 2020 4e6f 6465 4375 7374 6f6d 436f 6465    NodeCustomCode
-000007f0: 2c0a 2020 2020 4e6f 6465 4375 7374 6f6d  ,.    NodeCustom
-00000800: 496d 706f 7274 732c 0a20 2020 204e 6f64  Imports,.    Nod
-00000810: 6544 6566 2c0a 2020 2020 4e6f 6465 4465  eDef,.    NodeDe
-00000820: 6649 6e66 6f2c 0a20 2020 204e 6f64 6549  fInfo,.    NodeI
-00000830: 6e66 6f2c 0a20 2020 204e 6f64 6553 7461  nfo,.    NodeSta
-00000840: 7465 2c0a 2020 2020 4e6f 6465 5374 6174  te,.    NodeStat
-00000850: 7573 2c0a 2020 2020 4e6f 6465 5469 6d69  us,.    NodeTimi
-00000860: 6e67 2c0a 2020 2020 4e6f 6465 5479 7065  ng,.    NodeType
-00000870: 5265 7370 6f6e 7365 2c0a 2020 2020 4e6f  Response,.    No
-00000880: 6465 5479 7065 732c 0a20 2020 204e 6f64  deTypes,.    Nod
-00000890: 6555 7365 7243 6f6c 756d 6e73 5265 7370  eUserColumnsResp
-000008a0: 6f6e 7365 2c0a 2020 2020 5072 6574 7479  onse,.    Pretty
-000008b0: 5265 7370 6f6e 7365 2c0a 2020 2020 5075  Response,.    Pu
-000008c0: 744e 6f64 6542 6c6f 622c 0a20 2020 2051  tNodeBlob,.    Q
-000008d0: 7565 7565 4d6f 6465 2c0a 2020 2020 5175  ueueMode,.    Qu
-000008e0: 6575 6553 7461 7473 5265 7370 6f6e 7365  eueStatsResponse
-000008f0: 2c0a 2020 2020 5175 6575 6553 7461 7475  ,.    QueueStatu
-00000900: 732c 0a20 2020 2052 6561 644e 6f64 652c  s,.    ReadNode,
-00000910: 0a20 2020 2053 3343 6f6e 6669 672c 0a20  .    S3Config,. 
-00000920: 2020 2053 6574 4e61 6d65 6453 6563 7265     SetNamedSecre
-00000930: 742c 0a20 2020 2053 6574 7469 6e67 734f  t,.    SettingsO
-00000940: 626a 2c0a 2020 2020 5461 736b 5374 6174  bj,.    TaskStat
-00000950: 7573 2c0a 2020 2020 5469 6d69 6e67 2c0a  us,.    Timing,.
-00000960: 2020 2020 5469 6d69 6e67 5265 7375 6c74      TimingResult
-00000970: 2c0a 2020 2020 5469 6d69 6e67 732c 0a20  ,.    Timings,. 
-00000980: 2020 2054 7269 746f 6e4d 6f64 656c 7352     TritonModelsR
-00000990: 6573 706f 6e73 652c 0a20 2020 2055 5249  esponse,.    URI
-000009a0: 5072 6566 6978 2c0a 2020 2020 5570 6c6f  Prefix,.    Uplo
-000009b0: 6164 4669 6c65 7352 6573 706f 6e73 652c  adFilesResponse,
-000009c0: 0a20 2020 2055 5549 4452 6573 706f 6e73  .    UUIDRespons
-000009d0: 652c 0a20 2020 2056 6572 7369 6f6e 5265  e,.    VersionRe
-000009e0: 7370 6f6e 7365 2c0a 2020 2020 576f 726b  sponse,.    Work
-000009f0: 6572 5363 616c 652c 0a29 0a0a 6966 2054  erScale,.)..if T
-00000a00: 5950 455f 4348 4543 4b49 4e47 3a0a 2020  YPE_CHECKING:.  
-00000a10: 2020 5756 4420 3d20 7765 616b 7265 662e    WVD = weakref.
-00000a20: 5765 616b 5661 6c75 6544 6963 7469 6f6e  WeakValueDiction
-00000a30: 6172 795b 7374 722c 2027 4461 6748 616e  ary[str, 'DagHan
-00000a40: 646c 6527 5d0a 656c 7365 3a0a 2020 2020  dle'].else:.    
-00000a50: 5756 4420 3d20 7765 616b 7265 662e 5765  WVD = weakref.We
-00000a60: 616b 5661 6c75 6544 6963 7469 6f6e 6172  akValueDictionar
-00000a70: 790a 0a0a 4150 495f 5645 5253 494f 4e20  y...API_VERSION 
-00000a80: 3d20 350a 4d49 4e5f 4150 495f 5645 5253  = 5.MIN_API_VERS
-00000a90: 494f 4e20 3d20 340a 4445 4641 554c 545f  ION = 4.DEFAULT_
-00000aa0: 5552 4c20 3d20 2268 7474 703a 2f2f 6c6f  URL = "http://lo
-00000ab0: 6361 6c68 6f73 743a 3830 3830 220a 4445  calhost:8080".DE
-00000ac0: 4641 554c 545f 4e41 4d45 5350 4143 4520  FAULT_NAMESPACE 
-00000ad0: 3d20 2264 6566 6175 6c74 220a 0a0a 4d45  = "default"...ME
-00000ae0: 5448 4f44 5f44 454c 4554 4520 3d20 2244  THOD_DELETE = "D
-00000af0: 454c 4554 4522 0a4d 4554 484f 445f 4649  ELETE".METHOD_FI
-00000b00: 4c45 203d 2022 4649 4c45 220a 4d45 5448  LE = "FILE".METH
-00000b10: 4f44 5f47 4554 203d 2022 4745 5422 0a4d  OD_GET = "GET".M
-00000b20: 4554 484f 445f 4c4f 4e47 504f 5354 203d  ETHOD_LONGPOST =
-00000b30: 2022 4c4f 4e47 504f 5354 220a 4d45 5448   "LONGPOST".METH
-00000b40: 4f44 5f50 4f53 5420 3d20 2250 4f53 5422  OD_POST = "POST"
-00000b50: 0a4d 4554 484f 445f 5055 5420 3d20 2250  .METHOD_PUT = "P
-00000b60: 5554 220a 0a50 5245 4649 5820 3d20 222f  UT"..PREFIX = "/
-00000b70: 7879 6d65 220a 0a49 4e50 5554 5f43 5356  xyme"..INPUT_CSV
-00000b80: 5f45 5854 203d 2022 2e63 7376 220a 494e  _EXT = ".csv".IN
-00000b90: 5055 545f 5453 565f 4558 5420 3d20 222e  PUT_TSV_EXT = ".
-00000ba0: 7473 7622 0a49 4e50 5554 5f5a 4950 5f45  tsv".INPUT_ZIP_E
-00000bb0: 5854 203d 2022 2e7a 6970 220a 494e 5055  XT = ".zip".INPU
-00000bc0: 545f 4558 5420 3d20 5b49 4e50 5554 5f5a  T_EXT = [INPUT_Z
-00000bd0: 4950 5f45 5854 2c20 494e 5055 545f 4353  IP_EXT, INPUT_CS
-00000be0: 565f 4558 542c 2049 4e50 5554 5f54 5356  V_EXT, INPUT_TSV
-00000bf0: 5f45 5854 5d0a 0a0a 4655 4e43 203d 2043  _EXT]...FUNC = C
-00000c00: 616c 6c61 626c 655b 2e2e 2e2c 2041 6e79  allable[..., Any
-00000c10: 5d0a 4355 5354 4f4d 5f4e 4f44 455f 5459  ].CUSTOM_NODE_TY
-00000c20: 5045 5320 3d20 7b0a 2020 2020 2263 7573  PES = {.    "cus
-00000c30: 746f 6d5f 6461 7461 222c 0a20 2020 2022  tom_data",.    "
-00000c40: 6375 7374 6f6d 5f6a 736f 6e22 2c0a 2020  custom_json",.  
-00000c50: 2020 2263 7573 746f 6d5f 6a73 6f6e 5f74    "custom_json_t
-00000c60: 6f5f 6461 7461 222c 0a20 2020 2022 6375  o_data",.    "cu
-00000c70: 7374 6f6d 5f6a 736f 6e5f 6a6f 696e 5f64  stom_json_join_d
-00000c80: 6174 6122 2c0a 7d0a 4e4f 5f52 4554 5259  ata",.}.NO_RETRY
-00000c90: 3a20 4c69 7374 5b73 7472 5d20 3d20 5b5d  : List[str] = []
-00000ca0: 2020 2320 5b4d 4554 484f 445f 504f 5354    # [METHOD_POST
-00000cb0: 2c20 4d45 5448 4f44 5f46 494c 455d 0a0a  , METHOD_FILE]..
-00000cc0: 0a63 6c61 7373 2041 6363 6573 7344 656e  .class AccessDen
-00000cd0: 6965 6428 4578 6365 7074 696f 6e29 3a0a  ied(Exception):.
-00000ce0: 2020 2020 7061 7373 0a0a 2320 2a2a 2a20      pass..# *** 
-00000cf0: 4163 6365 7373 4465 6e69 6564 202a 2a2a  AccessDenied ***
-00000d00: 0a0a 0a63 6c61 7373 204c 6567 6163 7956  ...class LegacyV
-00000d10: 6572 7369 6f6e 2845 7863 6570 7469 6f6e  ersion(Exception
-00000d20: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00000d30: 745f 5f28 7365 6c66 2c20 6170 695f 7665  t__(self, api_ve
-00000d40: 7273 696f 6e3a 2069 6e74 2920 2d3e 204e  rsion: int) -> N
-00000d50: 6f6e 653a 0a20 2020 2020 2020 2073 7570  one:.        sup
-00000d60: 6572 2829 2e5f 5f69 6e69 745f 5f28 6622  er().__init__(f"
-00000d70: 6578 7065 6374 6564 207b 4150 495f 5645  expected {API_VE
-00000d80: 5253 494f 4e7d 2067 6f74 207b 6170 695f  RSION} got {api_
-00000d90: 7665 7273 696f 6e7d 2229 0a20 2020 2020  version}").     
-00000da0: 2020 2073 656c 662e 5f61 7069 5f76 6572     self._api_ver
-00000db0: 7369 6f6e 203d 2061 7069 5f76 6572 7369  sion = api_versi
-00000dc0: 6f6e 0a0a 2020 2020 6465 6620 6765 745f  on..    def get_
-00000dd0: 6170 695f 7665 7273 696f 6e28 7365 6c66  api_version(self
-00000de0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00000df0: 2020 7265 7475 726e 2073 656c 662e 5f61    return self._a
-00000e00: 7069 5f76 6572 7369 6f6e 0a0a 2320 2a2a  pi_version..# **
-00000e10: 2a20 4c65 6761 6379 5665 7273 696f 6e20  * LegacyVersion 
-00000e20: 2a2a 2a0a 0a0a 636c 6173 7320 5859 4d45  ***...class XYME
-00000e30: 436c 6965 6e74 3a0a 2020 2020 6465 6620  Client:.    def 
-00000e40: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00000e50: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00000e60: 2020 2020 2020 2020 7572 6c3a 2073 7472          url: str
-00000e70: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
-00000e80: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-00000e90: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
-00000ea0: 6e61 6d65 7370 6163 653a 2073 7472 2920  namespace: str) 
-00000eb0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00000ec0: 2073 656c 662e 5f75 726c 203d 2075 726c   self._url = url
-00000ed0: 2e72 7374 7269 7028 222f 2229 0a20 2020  .rstrip("/").   
-00000ee0: 2020 2020 2069 6620 746f 6b65 6e20 6973       if token is
-00000ef0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00000f00: 2020 2074 6f6b 656e 203d 206f 732e 656e     token = os.en
-00000f10: 7669 726f 6e2e 6765 7428 2258 594d 455f  viron.get("XYME_
-00000f20: 5345 5256 4552 5f54 4f4b 454e 2229 0a20  SERVER_TOKEN"). 
-00000f30: 2020 2020 2020 2073 656c 662e 5f74 6f6b         self._tok
-00000f40: 656e 203d 2074 6f6b 656e 0a20 2020 2020  en = token.     
-00000f50: 2020 2073 656c 662e 5f6e 616d 6573 7061     self._namespa
-00000f60: 6365 203d 206e 616d 6573 7061 6365 0a20  ce = namespace. 
-00000f70: 2020 2020 2020 2073 656c 662e 5f6c 6173         self._las
-00000f80: 745f 6163 7469 6f6e 203d 2074 696d 652e  t_action = time.
-00000f90: 6d6f 6e6f 746f 6e69 6328 290a 2020 2020  monotonic().    
-00000fa0: 2020 2020 7365 6c66 2e5f 6175 746f 5f72      self._auto_r
-00000fb0: 6566 7265 7368 203d 2054 7275 650a 2020  efresh = True.  
-00000fc0: 2020 2020 2020 7365 6c66 2e5f 6461 675f        self._dag_
-00000fd0: 6361 6368 653a 2057 5644 203d 2077 6561  cache: WVD = wea
-00000fe0: 6b72 6566 2e57 6561 6b56 616c 7565 4469  kref.WeakValueDi
-00000ff0: 6374 696f 6e61 7279 2829 0a20 2020 2020  ctionary().     
-00001000: 2020 2073 656c 662e 5f6e 6f64 655f 6465     self._node_de
-00001010: 6673 3a20 4f70 7469 6f6e 616c 5b44 6963  fs: Optional[Dic
-00001020: 745b 7374 722c 204e 6f64 6544 6566 496e  t[str, NodeDefIn
-00001030: 666f 5d5d 203d 204e 6f6e 650a 0a20 2020  fo]] = None..   
-00001040: 2020 2020 2064 6566 2067 6574 5f76 6572       def get_ver
-00001050: 7369 6f6e 2829 202d 3e20 5475 706c 655b  sion() -> Tuple[
-00001060: 696e 742c 2069 6e74 5d3a 0a20 2020 2020  int, int]:.     
-00001070: 2020 2020 2020 2073 6572 7665 725f 7665         server_ve
-00001080: 7273 696f 6e20 3d20 7365 6c66 2e67 6574  rsion = self.get
-00001090: 5f73 6572 7665 725f 7665 7273 696f 6e28  _server_version(
-000010a0: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
-000010b0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-000010c0: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 696e 7428 7365 7276 6572 5f76 6572 7369  int(server_versi
-000010f0: 6f6e 5b22 6170 695f 7665 7273 696f 6e22  on["api_version"
-00001100: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00001110: 2020 2020 2020 2020 696e 7428 7365 7276          int(serv
-00001120: 6572 5f76 6572 7369 6f6e 2e67 6574 2822  er_version.get("
-00001130: 6170 695f 7665 7273 696f 6e5f 6d69 6e6f  api_version_mino
-00001140: 7222 2c20 3029 292c 0a20 2020 2020 2020  r", 0)),.       
-00001150: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00001160: 2020 2020 2020 2065 7863 6570 7420 2856         except (V
-00001170: 616c 7565 4572 726f 722c 204b 6579 4572  alueError, KeyEr
-00001180: 726f 7229 2061 7320 653a 0a20 2020 2020  ror) as e:.     
-00001190: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000011a0: 204c 6567 6163 7956 6572 7369 6f6e 2831   LegacyVersion(1
-000011b0: 2920 6672 6f6d 2065 0a0a 2020 2020 2020  ) from e..      
-000011c0: 2020 6170 695f 7665 7273 696f 6e2c 2061    api_version, a
-000011d0: 7069 5f76 6572 7369 6f6e 5f6d 696e 6f72  pi_version_minor
-000011e0: 203d 2067 6574 5f76 6572 7369 6f6e 2829   = get_version()
-000011f0: 0a20 2020 2020 2020 2069 6620 6170 695f  .        if api_
-00001200: 7665 7273 696f 6e20 3c20 4d49 4e5f 4150  version < MIN_AP
-00001210: 495f 5645 5253 494f 4e3a 0a20 2020 2020  I_VERSION:.     
-00001220: 2020 2020 2020 2072 6169 7365 204c 6567         raise Leg
-00001230: 6163 7956 6572 7369 6f6e 2861 7069 5f76  acyVersion(api_v
-00001240: 6572 7369 6f6e 290a 2020 2020 2020 2020  ersion).        
-00001250: 7365 6c66 2e5f 6170 695f 7665 7273 696f  self._api_versio
-00001260: 6e20 3d20 6170 695f 7665 7273 696f 6e0a  n = api_version.
-00001270: 2020 2020 2020 2020 7365 6c66 2e5f 6170          self._ap
-00001280: 695f 7665 7273 696f 6e5f 6d69 6e6f 7220  i_version_minor 
-00001290: 3d20 6170 695f 7665 7273 696f 6e5f 6d69  = api_version_mi
-000012a0: 6e6f 720a 0a20 2020 2064 6566 2067 6574  nor..    def get
-000012b0: 5f61 7069 5f76 6572 7369 6f6e 2873 656c  _api_version(sel
-000012c0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-000012d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000012e0: 6170 695f 7665 7273 696f 6e0a 0a20 2020  api_version..   
-000012f0: 2064 6566 2067 6574 5f61 7069 5f76 6572   def get_api_ver
-00001300: 7369 6f6e 5f6d 696e 6f72 2873 656c 6629  sion_minor(self)
-00001310: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00001320: 2072 6574 7572 6e20 7365 6c66 2e5f 6170   return self._ap
-00001330: 695f 7665 7273 696f 6e5f 6d69 6e6f 720a  i_version_minor.
-00001340: 0a20 2020 2064 6566 2068 6173 5f76 6572  .    def has_ver
-00001350: 7369 6f6e 2873 656c 662c 206d 616a 6f72  sion(self, major
-00001360: 3a20 696e 742c 206d 696e 6f72 3a20 696e  : int, minor: in
-00001370: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
-00001380: 2020 2020 6966 2073 656c 662e 5f61 7069      if self._api
-00001390: 5f76 6572 7369 6f6e 203e 206d 616a 6f72  _version > major
-000013a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000013b0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-000013c0: 2020 7265 7475 726e 2073 656c 662e 5f61    return self._a
-000013d0: 7069 5f76 6572 7369 6f6e 203d 3d20 6d61  pi_version == ma
-000013e0: 6a6f 7220 616e 6420 7365 6c66 2e5f 6170  jor and self._ap
-000013f0: 695f 7665 7273 696f 6e5f 6d69 6e6f 7220  i_version_minor 
-00001400: 3e3d 206d 696e 6f72 0a0a 2020 2020 6465  >= minor..    de
-00001410: 6620 7365 745f 6175 746f 5f72 6566 7265  f set_auto_refre
-00001420: 7368 2873 656c 662c 2069 735f 6175 746f  sh(self, is_auto
-00001430: 5f72 6566 7265 7368 3a20 626f 6f6c 2920  _refresh: bool) 
-00001440: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00001450: 2073 656c 662e 5f61 7574 6f5f 7265 6672   self._auto_refr
-00001460: 6573 6820 3d20 6973 5f61 7574 6f5f 7265  esh = is_auto_re
-00001470: 6672 6573 680a 0a20 2020 2064 6566 2069  fresh..    def i
-00001480: 735f 6175 746f 5f72 6566 7265 7368 2873  s_auto_refresh(s
-00001490: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-000014a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000014b0: 662e 5f61 7574 6f5f 7265 6672 6573 680a  f._auto_refresh.
-000014c0: 0a20 2020 2064 6566 2072 6566 7265 7368  .    def refresh
-000014d0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000014e0: 2020 2020 2020 2020 7365 6c66 2e5f 6e6f          self._no
-000014f0: 6465 5f64 6566 7320 3d20 4e6f 6e65 0a0a  de_defs = None..
-00001500: 2020 2020 6465 6620 5f6d 6179 6265 5f72      def _maybe_r
-00001510: 6566 7265 7368 2873 656c 6629 202d 3e20  efresh(self) -> 
-00001520: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-00001530: 2073 656c 662e 6973 5f61 7574 6f5f 7265   self.is_auto_re
-00001540: 6672 6573 6828 293a 0a20 2020 2020 2020  fresh():.       
-00001550: 2020 2020 2073 656c 662e 7265 6672 6573       self.refres
-00001560: 6828 290a 0a20 2020 2023 2046 4958 4d45  h()..    # FIXME
-00001570: 3a20 446f 2077 6520 7374 696c 6c20 6e65  : Do we still ne
-00001580: 6564 2074 6869 733f 0a20 2020 2040 636f  ed this?.    @co
-00001590: 6e74 6578 746c 6962 2e63 6f6e 7465 7874  ntextlib.context
-000015a0: 6d61 6e61 6765 720a 2020 2020 6465 6620  manager.    def 
-000015b0: 6275 6c6b 5f6f 7065 7261 7469 6f6e 2873  bulk_operation(s
-000015c0: 656c 6629 202d 3e20 4974 6572 6174 6f72  elf) -> Iterator
-000015d0: 5b62 6f6f 6c5d 3a0a 2020 2020 2020 2020  [bool]:.        
-000015e0: 6f6c 645f 7265 6672 6573 6820 3d20 7365  old_refresh = se
-000015f0: 6c66 2e69 735f 6175 746f 5f72 6566 7265  lf.is_auto_refre
-00001600: 7368 2829 0a20 2020 2020 2020 2074 7279  sh().        try
-00001610: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00001620: 6c66 2e73 6574 5f61 7574 6f5f 7265 6672  lf.set_auto_refr
-00001630: 6573 6828 4661 6c73 6529 0a20 2020 2020  esh(False).     
-00001640: 2020 2020 2020 2079 6965 6c64 206f 6c64         yield old
-00001650: 5f72 6566 7265 7368 0a20 2020 2020 2020  _refresh.       
-00001660: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-00001670: 2020 2020 2020 7365 6c66 2e73 6574 5f61        self.set_a
-00001680: 7574 6f5f 7265 6672 6573 6828 6f6c 645f  uto_refresh(old_
-00001690: 7265 6672 6573 6829 0a0a 2020 2020 6465  refresh)..    de
-000016a0: 6620 5f72 6177 5f72 6571 7565 7374 5f62  f _raw_request_b
-000016b0: 7974 6573 280a 2020 2020 2020 2020 2020  ytes(.          
-000016c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000016d0: 2020 2020 6d65 7468 6f64 3a20 7374 722c      method: str,
-000016e0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-000016f0: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-00001700: 2020 2020 6172 6773 3a20 4469 6374 5b73      args: Dict[s
-00001710: 7472 2c20 416e 795d 2c0a 2020 2020 2020  tr, Any],.      
-00001720: 2020 2020 2020 6669 6c65 733a 204f 7074        files: Opt
-00001730: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-00001740: 4279 7465 7349 4f5d 5d20 3d20 4e6f 6e65  BytesIO]] = None
-00001750: 2c0a 2020 2020 2020 2020 2020 2020 6164  ,.            ad
-00001760: 645f 7072 6566 6978 3a20 626f 6f6c 203d  d_prefix: bool =
-00001770: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-00001780: 2020 2061 6464 5f6e 616d 6573 7061 6365     add_namespace
-00001790: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-000017a0: 2020 2020 2020 2020 2020 2061 7069 5f76             api_v
-000017b0: 6572 7369 6f6e 3a20 4f70 7469 6f6e 616c  ersion: Optional
-000017c0: 5b69 6e74 5d20 3d20 4e6f 6e65 2920 2d3e  [int] = None) ->
-000017d0: 2054 7570 6c65 5b42 7974 6573 494f 2c20   Tuple[BytesIO, 
-000017e0: 7374 725d 3a0a 2020 2020 2020 2020 6669  str]:.        fi
-000017f0: 6c65 5f72 6573 6574 7320 3d20 7b7d 0a20  le_resets = {}. 
-00001800: 2020 2020 2020 2063 616e 5f72 6573 6574         can_reset
-00001810: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00001820: 6966 2066 696c 6573 2069 7320 6e6f 7420  if files is not 
-00001830: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00001840: 2020 666f 7220 2866 6e61 6d65 2c20 6662    for (fname, fb
-00001850: 7566 6629 2069 6e20 6669 6c65 732e 6974  uff) in files.it
-00001860: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00001870: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-00001880: 7228 6662 7566 662c 2022 7365 656b 2229  r(fbuff, "seek")
-00001890: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000018a0: 2020 2020 2020 6669 6c65 5f72 6573 6574        file_reset
-000018b0: 735b 666e 616d 655d 203d 2066 6275 6666  s[fname] = fbuff
-000018c0: 2e73 6565 6b28 302c 2069 6f2e 5345 454b  .seek(0, io.SEEK
-000018d0: 5f43 5552 290a 2020 2020 2020 2020 2020  _CUR).          
-000018e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001900: 6361 6e5f 7265 7365 7420 3d20 4661 6c73  can_reset = Fals
-00001910: 650a 0a20 2020 2020 2020 2064 6566 2072  e..        def r
-00001920: 6573 6574 5f66 696c 6573 2829 202d 3e20  eset_files() -> 
-00001930: 626f 6f6c 3a0a 2020 2020 2020 2020 2020  bool:.          
-00001940: 2020 6966 2066 696c 6573 2069 7320 4e6f    if files is No
-00001950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00001960: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00001970: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00001980: 6f74 2063 616e 5f72 6573 6574 3a0a 2020  ot can_reset:.  
-00001990: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000019a0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-000019b0: 2020 2020 2020 2066 6f72 2028 666e 616d         for (fnam
-000019c0: 652c 2070 6f73 2920 696e 2066 696c 655f  e, pos) in file_
-000019d0: 7265 7365 7473 2e69 7465 6d73 2829 3a0a  resets.items():.
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 6669 6c65 735b 666e 616d 655d 2e73 6565  files[fname].see
-00001a00: 6b28 706f 732c 2069 6f2e 5345 454b 5f53  k(pos, io.SEEK_S
-00001a10: 4554 290a 2020 2020 2020 2020 2020 2020  ET).            
-00001a20: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
-00001a30: 2020 2020 2072 6574 7279 203d 2030 0a20       retry = 0. 
-00001a40: 2020 2020 2020 206d 6178 5f72 6574 7279         max_retry
-00001a50: 203d 2067 6574 5f6d 6178 5f72 6574 7279   = get_max_retry
-00001a60: 2829 0a20 2020 2020 2020 2077 6869 6c65  ().        while
-00001a70: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
-00001a80: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00001a90: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2072 6574 7572 6e20 7365 6c66 2e5f 6661   return self._fa
-00001ac0: 6c6c 6962 6c65 5f72 6177 5f72 6571 7565  llible_raw_reque
-00001ad0: 7374 5f62 7974 6573 280a 2020 2020 2020  st_bytes(.      
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2020 6d65 7468 6f64 2c0a 2020 2020 2020    method,.      
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 7061 7468 2c0a 2020 2020 2020 2020    path,.        
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 6172 6773 2c0a 2020 2020 2020 2020 2020  args,.          
-00001b40: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00001b50: 6c65 732c 0a20 2020 2020 2020 2020 2020  les,.           
-00001b60: 2020 2020 2020 2020 2020 2020 2061 6464               add
-00001b70: 5f70 7265 6669 782c 0a20 2020 2020 2020  _prefix,.       
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2061 6464 5f6e 616d 6573 7061 6365 2c0a   add_namespace,.
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 2020 2020 2020 2020 6170 695f 7665 7273          api_vers
-00001bc0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-00001bd0: 2020 2020 2065 7863 6570 7420 4854 5450       except HTTP
-00001be0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 6966 2065 2e72 6573 706f 6e73 652e 7374  if e.response.st
-00001c10: 6174 7573 5f63 6f64 6520 696e 2028 3430  atus_code in (40
-00001c20: 332c 2034 3034 2c20 3530 3029 3a0a 2020  3, 404, 500):.  
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c40: 2020 2020 2020 7265 7472 7920 3d20 6d61        retry = ma
-00001c50: 785f 7265 7472 790a 2020 2020 2020 2020  x_retry.        
-00001c60: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00001c70: 6520 650a 2020 2020 2020 2020 2020 2020  e e.            
-00001c80: 6578 6365 7074 2052 6571 7565 7374 4578  except RequestEx
-00001c90: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
-00001ca0: 2020 2020 2020 2020 2069 6620 7265 7472           if retr
-00001cb0: 7920 3e3d 206d 6178 5f72 6574 7279 3a0a  y >= max_retry:.
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 2020 2020 7261 6973 650a 2020 2020 2020      raise.      
-00001ce0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00001cf0: 2072 6573 6574 5f66 696c 6573 2829 3a0a   reset_files():.
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 7261 6973 650a 2020 2020 2020      raise.      
-00001d20: 2020 2020 2020 2020 2020 6966 206d 6574            if met
-00001d30: 686f 6420 696e 204e 4f5f 5245 5452 593a  hod in NO_RETRY:
-00001d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d50: 2020 2020 2072 6169 7365 0a20 2020 2020       raise.     
-00001d60: 2020 2020 2020 2020 2020 2074 696d 652e             time.
-00001d70: 736c 6565 7028 6765 745f 7265 7472 795f  sleep(get_retry_
-00001d80: 736c 6565 7028 2929 0a20 2020 2020 2020  sleep()).       
-00001d90: 2020 2020 2072 6574 7279 202b 3d20 310a       retry += 1.
-00001da0: 0a20 2020 2064 6566 205f 7261 775f 7265  .    def _raw_re
-00001db0: 7175 6573 745f 7374 7228 0a20 2020 2020  quest_str(.     
-00001dc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00001dd0: 2020 2020 2020 2020 206d 6574 686f 643a           method:
-00001de0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00001df0: 2020 7061 7468 3a20 7374 722c 0a20 2020    path: str,.   
-00001e00: 2020 2020 2020 2020 2061 7267 733a 2044           args: D
-00001e10: 6963 745b 7374 722c 2041 6e79 5d2c 0a20  ict[str, Any],. 
-00001e20: 2020 2020 2020 2020 2020 2061 6464 5f70             add_p
-00001e30: 7265 6669 783a 2062 6f6f 6c20 3d20 5472  refix: bool = Tr
-00001e40: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001e50: 6164 645f 6e61 6d65 7370 6163 653a 2062  add_namespace: b
-00001e60: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-00001e70: 2020 2020 2020 2020 6170 695f 7665 7273          api_vers
-00001e80: 696f 6e3a 204f 7074 696f 6e61 6c5b 696e  ion: Optional[in
-00001e90: 745d 203d 204e 6f6e 6529 202d 3e20 5465  t] = None) -> Te
-00001ea0: 7874 494f 3a0a 2020 2020 2020 2020 7265  xtIO:.        re
-00001eb0: 7472 7920 3d20 300a 2020 2020 2020 2020  try = 0.        
-00001ec0: 6d61 785f 7265 7472 7920 3d20 6765 745f  max_retry = get_
-00001ed0: 6d61 785f 7265 7472 7928 290a 2020 2020  max_retry().    
-00001ee0: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
-00001ef0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00001f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00001f20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001f30: 2073 656c 662e 5f66 616c 6c69 626c 655f   self._fallible_
-00001f40: 7261 775f 7265 7175 6573 745f 7374 7228  raw_request_str(
-00001f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f60: 2020 2020 2020 2020 206d 6574 686f 642c           method,
-00001f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f80: 2020 2020 2020 2020 2070 6174 682c 0a20           path,. 
-00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 2020 2020 2020 2061 7267 732c 0a20 2020         args,.   
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 2061 6464 5f70 7265 6669 782c       add_prefix,
-00001fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001fe0: 2020 2020 2020 2020 2061 6464 5f6e 616d           add_nam
-00001ff0: 6573 7061 6365 2c0a 2020 2020 2020 2020  espace,.        
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 6170 695f 7665 7273 696f 6e29 0a20 2020  api_version).   
-00002020: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00002030: 6570 7420 4854 5450 4572 726f 7220 6173  ept HTTPError as
-00002040: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-00002050: 2020 2020 2020 2020 6966 2065 2e72 6573          if e.res
-00002060: 706f 6e73 652e 7374 6174 7573 5f63 6f64  ponse.status_cod
-00002070: 6520 696e 2028 3430 332c 2034 3034 2c20  e in (403, 404, 
-00002080: 3530 3029 3a0a 2020 2020 2020 2020 2020  500):.          
-00002090: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000020a0: 7472 7920 3d20 6d61 785f 7265 7472 790a  try = max_retry.
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2020 7261 6973 6520 650a 2020 2020      raise e.    
-000020d0: 2020 2020 2020 2020 6578 6365 7074 2052          except R
-000020e0: 6571 7565 7374 4578 6365 7074 696f 6e3a  equestException:
-000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002100: 2069 6620 6d65 7468 6f64 2069 6e20 4e4f   if method in NO
-00002110: 5f52 4554 5259 3a0a 2020 2020 2020 2020  _RETRY:.        
-00002120: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00002130: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00002140: 2020 6966 2072 6574 7279 203e 3d20 6d61    if retry >= ma
-00002150: 785f 7265 7472 793a 0a20 2020 2020 2020  x_retry:.       
-00002160: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00002170: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00002180: 2020 2074 696d 652e 736c 6565 7028 6765     time.sleep(ge
-00002190: 745f 7265 7472 795f 736c 6565 7028 2929  t_retry_sleep())
-000021a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000021b0: 7279 202b 3d20 310a 0a20 2020 2064 6566  ry += 1..    def
-000021c0: 205f 7261 775f 7265 7175 6573 745f 6a73   _raw_request_js
-000021d0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-000021e0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-000021f0: 2020 6d65 7468 6f64 3a20 7374 722c 0a20    method: str,. 
-00002200: 2020 2020 2020 2020 2020 2070 6174 683a             path:
-00002210: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00002220: 2020 6172 6773 3a20 4469 6374 5b73 7472    args: Dict[str
-00002230: 2c20 416e 795d 2c0a 2020 2020 2020 2020  , Any],.        
-00002240: 2020 2020 6164 645f 7072 6566 6978 3a20      add_prefix: 
-00002250: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-00002260: 2020 2020 2020 2020 2061 6464 5f6e 616d           add_nam
-00002270: 6573 7061 6365 3a20 626f 6f6c 203d 2054  espace: bool = T
-00002280: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00002290: 2066 696c 6573 3a20 4f70 7469 6f6e 616c   files: Optional
-000022a0: 5b44 6963 745b 7374 722c 2049 4f5b 6279  [Dict[str, IO[by
-000022b0: 7465 735d 5d5d 203d 204e 6f6e 652c 0a20  tes]]] = None,. 
-000022c0: 2020 2020 2020 2020 2020 2061 7069 5f76             api_v
-000022d0: 6572 7369 6f6e 3a20 4f70 7469 6f6e 616c  ersion: Optional
-000022e0: 5b69 6e74 5d20 3d20 4e6f 6e65 2920 2d3e  [int] = None) ->
-000022f0: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
-00002300: 0a20 2020 2020 2020 2066 696c 655f 7265  .        file_re
-00002310: 7365 7473 203d 207b 7d0a 2020 2020 2020  sets = {}.      
-00002320: 2020 6361 6e5f 7265 7365 7420 3d20 5472    can_reset = Tr
-00002330: 7565 0a20 2020 2020 2020 2069 6620 6669  ue.        if fi
-00002340: 6c65 7320 6973 206e 6f74 204e 6f6e 653a  les is not None:
-00002350: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00002360: 2028 666e 616d 652c 2066 6275 6666 2920   (fname, fbuff) 
-00002370: 696e 2066 696c 6573 2e69 7465 6d73 2829  in files.items()
-00002380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002390: 2020 6966 2068 6173 6174 7472 2866 6275    if hasattr(fbu
-000023a0: 6666 2c20 2273 6565 6b22 293a 0a20 2020  ff, "seek"):.   
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2066 696c 655f 7265 7365 7473 5b66 6e61   file_resets[fna
-000023d0: 6d65 5d20 3d20 6662 7566 662e 7365 656b  me] = fbuff.seek
-000023e0: 2830 2c20 696f 2e53 4545 4b5f 4355 5229  (0, io.SEEK_CUR)
-000023f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002400: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002410: 2020 2020 2020 2020 2020 2063 616e 5f72             can_r
-00002420: 6573 6574 203d 2046 616c 7365 0a0a 2020  eset = False..  
-00002430: 2020 2020 2020 6465 6620 7265 7365 745f        def reset_
-00002440: 6669 6c65 7328 2920 2d3e 2062 6f6f 6c3a  files() -> bool:
-00002450: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002460: 6669 6c65 7320 6973 204e 6f6e 653a 0a20  files is None:. 
-00002470: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002480: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00002490: 2020 2020 2020 2069 6620 6e6f 7420 6361         if not ca
-000024a0: 6e5f 7265 7365 743a 0a20 2020 2020 2020  n_reset:.       
-000024b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000024c0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-000024d0: 2020 666f 7220 2866 6e61 6d65 2c20 706f    for (fname, po
-000024e0: 7329 2069 6e20 6669 6c65 5f72 6573 6574  s) in file_reset
-000024f0: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-00002500: 2020 2020 2020 2020 2020 2066 696c 6573             files
-00002510: 5b66 6e61 6d65 5d2e 7365 656b 2870 6f73  [fname].seek(pos
-00002520: 2c20 696f 2e53 4545 4b5f 5345 5429 0a20  , io.SEEK_SET). 
-00002530: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002540: 6e20 5472 7565 0a0a 2020 2020 2020 2020  n True..        
-00002550: 7265 7472 7920 3d20 300a 2020 2020 2020  retry = 0.      
-00002560: 2020 6d61 785f 7265 7472 7920 3d20 6765    max_retry = ge
-00002570: 745f 6d61 785f 7265 7472 7928 290a 2020  t_max_retry().  
-00002580: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00002590: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-000025a0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-000025b0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000025c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000025d0: 726e 2073 656c 662e 5f66 616c 6c69 626c  rn self._fallibl
-000025e0: 655f 7261 775f 7265 7175 6573 745f 6a73  e_raw_request_js
-000025f0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00002600: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-00002610: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
-00002620: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00002630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002640: 2020 2020 2020 2020 2020 6172 6773 2c0a            args,.
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 2020 2020 6164 645f 7072 6566          add_pref
-00002670: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
-00002680: 2020 2020 2020 2020 2020 2020 6164 645f              add_
-00002690: 6e61 6d65 7370 6163 652c 0a20 2020 2020  namespace,.     
-000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026b0: 2020 2066 696c 6573 2c0a 2020 2020 2020     files,.      
-000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026d0: 2020 6170 695f 7665 7273 696f 6e29 0a20    api_version). 
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000026f0: 7863 6570 7420 4854 5450 4572 726f 7220  xcept HTTPError 
-00002700: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00002710: 2020 2020 2020 2020 2020 6966 2065 2e72            if e.r
-00002720: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
-00002730: 6f64 6520 696e 2028 3430 332c 2034 3034  ode in (403, 404
-00002740: 2c20 3530 3029 3a0a 2020 2020 2020 2020  , 500):.        
-00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 7265 7472 7920 3d20 6d61 785f 7265 7472  retry = max_retr
-00002770: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00002780: 2020 2020 2020 7261 6973 6520 650a 2020        raise e.  
-00002790: 2020 2020 2020 2020 2020 6578 6365 7074            except
-000027a0: 2052 6571 7565 7374 4578 6365 7074 696f   RequestExceptio
-000027b0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-000027c0: 2020 2069 6620 7265 7472 7920 3e3d 206d     if retry >= m
-000027d0: 6178 5f72 6574 7279 3a0a 2020 2020 2020  ax_retry:.      
-000027e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000027f0: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
-00002800: 2020 2020 6966 206e 6f74 2072 6573 6574      if not reset
-00002810: 5f66 696c 6573 2829 3a0a 2020 2020 2020  _files():.      
-00002820: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00002830: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
-00002840: 2020 2020 6966 206d 6574 686f 6420 696e      if method in
-00002850: 204e 4f5f 5245 5452 593a 0a20 2020 2020   NO_RETRY:.     
-00002860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002870: 6169 7365 0a20 2020 2020 2020 2020 2020  aise.           
-00002880: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00002890: 6765 745f 7265 7472 795f 736c 6565 7028  get_retry_sleep(
-000028a0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-000028b0: 6574 7279 202b 3d20 310a 0a20 2020 2064  etry += 1..    d
-000028c0: 6566 205f 6661 6c6c 6962 6c65 5f72 6177  ef _fallible_raw
-000028d0: 5f72 6571 7565 7374 5f62 7974 6573 280a  _request_bytes(.
-000028e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000028f0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-00002900: 7468 6f64 3a20 7374 722c 0a20 2020 2020  thod: str,.     
-00002910: 2020 2020 2020 2070 6174 683a 2073 7472         path: str
-00002920: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-00002930: 6773 3a20 4469 6374 5b73 7472 2c20 416e  gs: Dict[str, An
-00002940: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
-00002950: 6669 6c65 733a 204f 7074 696f 6e61 6c5b  files: Optional[
-00002960: 4469 6374 5b73 7472 2c20 4279 7465 7349  Dict[str, BytesI
-00002970: 4f5d 5d2c 0a20 2020 2020 2020 2020 2020  O]],.           
-00002980: 2061 6464 5f70 7265 6669 783a 2062 6f6f   add_prefix: boo
-00002990: 6c2c 0a20 2020 2020 2020 2020 2020 2061  l,.            a
-000029a0: 6464 5f6e 616d 6573 7061 6365 3a20 626f  dd_namespace: bo
-000029b0: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
-000029c0: 6170 695f 7665 7273 696f 6e3a 204f 7074  api_version: Opt
-000029d0: 696f 6e61 6c5b 696e 745d 2920 2d3e 2054  ional[int]) -> T
-000029e0: 7570 6c65 5b42 7974 6573 494f 2c20 7374  uple[BytesIO, st
-000029f0: 725d 3a0a 2020 2020 2020 2020 7072 6566  r]:.        pref
-00002a00: 6978 203d 2022 220a 2020 2020 2020 2020  ix = "".        
-00002a10: 6966 2061 6464 5f70 7265 6669 783a 0a20  if add_prefix:. 
-00002a20: 2020 2020 2020 2020 2020 2069 6620 6170             if ap
-00002a30: 695f 7665 7273 696f 6e20 6973 204e 6f6e  i_version is Non
-00002a40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002a50: 2020 2061 7069 5f76 6572 7369 6f6e 203d     api_version =
-00002a60: 2073 656c 662e 5f61 7069 5f76 6572 7369   self._api_versi
-00002a70: 6f6e 0a20 2020 2020 2020 2020 2020 2070  on.            p
-00002a80: 7265 6669 7820 3d20 6622 7b50 5245 4649  refix = f"{PREFI
-00002a90: 587d 2f76 7b61 7069 5f76 6572 7369 6f6e  X}/v{api_version
-00002aa0: 7d22 0a20 2020 2020 2020 2075 726c 203d  }".        url =
-00002ab0: 2066 227b 7365 6c66 2e5f 7572 6c7d 7b70   f"{self._url}{p
-00002ac0: 7265 6669 787d 7b70 6174 687d 220a 2020  refix}{path}".  
-00002ad0: 2020 2020 2020 6865 6164 6572 7320 3d20        headers = 
-00002ae0: 7b0a 2020 2020 2020 2020 2020 2020 2261  {.            "a
-00002af0: 7574 686f 7269 7a61 7469 6f6e 223a 2073  uthorization": s
-00002b00: 656c 662e 5f74 6f6b 656e 2c0a 2020 2020  elf._token,.    
-00002b10: 2020 2020 7d0a 2020 2020 2020 2020 6966      }.        if
-00002b20: 2061 6464 5f6e 616d 6573 7061 6365 3a0a   add_namespace:.
-00002b30: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00002b40: 5b22 6e61 6d65 7370 6163 6522 5d20 3d20  ["namespace"] = 
-00002b50: 7365 6c66 2e5f 6e61 6d65 7370 6163 650a  self._namespace.
-00002b60: 0a20 2020 2020 2020 2064 6566 2063 6865  .        def che
-00002b70: 636b 5f65 7272 6f72 2872 6571 3a20 5265  ck_error(req: Re
-00002b80: 7370 6f6e 7365 2920 2d3e 204e 6f6e 653a  sponse) -> None:
-00002b90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002ba0: 7265 712e 7374 6174 7573 5f63 6f64 6520  req.status_code 
-00002bb0: 3d3d 2034 3033 3a0a 2020 2020 2020 2020  == 403:.        
-00002bc0: 2020 2020 2020 2020 7261 6973 6520 4163          raise Ac
-00002bd0: 6365 7373 4465 6e69 6564 2872 6571 2e74  cessDenied(req.t
-00002be0: 6578 7429 0a20 2020 2020 2020 2020 2020  ext).           
-00002bf0: 2072 6571 2e72 6169 7365 5f66 6f72 5f73   req.raise_for_s
-00002c00: 7461 7475 7328 290a 2020 2020 2020 2020  tatus().        
-00002c10: 2020 2020 2320 4e4f 5445 3a20 6e6f 2063      # NOTE: no c
-00002c20: 6f6e 7465 6e74 2074 7970 6520 6368 6563  ontent type chec
-00002c30: 6b20 2d2d 2077 696c 6c20 6265 2068 616e  k -- will be han
-00002c40: 646c 6564 2062 7920 696e 7465 7270 7265  dled by interpre
-00002c50: 745f 6374 7970 650a 0a20 2020 2020 2020  t_ctype..       
-00002c60: 2069 6620 6d65 7468 6f64 203d 3d20 4d45   if method == ME
-00002c70: 5448 4f44 5f47 4554 3a0a 2020 2020 2020  THOD_GET:.      
-00002c80: 2020 2020 2020 7265 7120 3d20 7265 7175        req = requ
-00002c90: 6573 7473 2e67 6574 2875 726c 2c20 7061  ests.get(url, pa
-00002ca0: 7261 6d73 3d61 7267 732c 2068 6561 6465  rams=args, heade
-00002cb0: 7273 3d68 6561 6465 7273 290a 2020 2020  rs=headers).    
-00002cc0: 2020 2020 2020 2020 6368 6563 6b5f 6572          check_er
-00002cd0: 726f 7228 7265 7129 0a20 2020 2020 2020  ror(req).       
-00002ce0: 2020 2020 2072 6574 7572 6e20 4279 7465       return Byte
-00002cf0: 7349 4f28 7265 712e 636f 6e74 656e 7429  sIO(req.content)
-00002d00: 2c20 7265 712e 6865 6164 6572 735b 2263  , req.headers["c
-00002d10: 6f6e 7465 6e74 2d74 7970 6522 5d0a 2020  ontent-type"].  
-00002d20: 2020 2020 2020 6966 206d 6574 686f 6420        if method 
-00002d30: 3d3d 204d 4554 484f 445f 504f 5354 3a0a  == METHOD_POST:.
-00002d40: 2020 2020 2020 2020 2020 2020 7265 7120              req 
-00002d50: 3d20 7265 7175 6573 7473 2e70 6f73 7428  = requests.post(
-00002d60: 7572 6c2c 206a 736f 6e3d 6172 6773 2c20  url, json=args, 
-00002d70: 6865 6164 6572 733d 6865 6164 6572 7329  headers=headers)
-00002d80: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-00002d90: 636b 5f65 7272 6f72 2872 6571 290a 2020  ck_error(req).  
-00002da0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002db0: 2042 7974 6573 494f 2872 6571 2e63 6f6e   BytesIO(req.con
-00002dc0: 7465 6e74 292c 2072 6571 2e68 6561 6465  tent), req.heade
-00002dd0: 7273 5b22 636f 6e74 656e 742d 7479 7065  rs["content-type
-00002de0: 225d 0a20 2020 2020 2020 2069 6620 6d65  "].        if me
-00002df0: 7468 6f64 203d 3d20 4d45 5448 4f44 5f46  thod == METHOD_F
-00002e00: 494c 453a 0a20 2020 2020 2020 2020 2020  ILE:.           
-00002e10: 2069 6620 6669 6c65 7320 6973 204e 6f6e   if files is Non
-00002e20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002e30: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00002e40: 726f 7228 6622 6669 6c65 206d 6574 686f  ror(f"file metho
-00002e50: 6420 6d75 7374 2068 6176 6520 6669 6c65  d must have file
-00002e60: 733a 207b 6669 6c65 737d 2229 0a20 2020  s: {files}").   
-00002e70: 2020 2020 2020 2020 2072 6571 203d 2072           req = r
-00002e80: 6571 7565 7374 732e 706f 7374 280a 2020  equests.post(.  
-00002e90: 2020 2020 2020 2020 2020 2020 2020 7572                ur
-00002ea0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-00002eb0: 2020 2064 6174 613d 6172 6773 2c0a 2020     data=args,.  
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00002ed0: 6c65 733d 7b0a 2020 2020 2020 2020 2020  les={.          
-00002ee0: 2020 2020 2020 2020 2020 6b65 793a 2028            key: (
-00002ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f00: 2020 2020 2020 2020 2067 6574 6174 7472           getattr
-00002f10: 2876 616c 7565 2c20 226e 616d 6522 2c20  (value, "name", 
-00002f20: 6b65 7929 2c0a 2020 2020 2020 2020 2020  key),.          
-00002f30: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00002f40: 6c75 652c 0a20 2020 2020 2020 2020 2020  lue,.           
-00002f50: 2020 2020 2020 2020 2020 2020 2022 6170               "ap
-00002f60: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-00002f70: 7374 7265 616d 222c 0a20 2020 2020 2020  stream",.       
-00002f80: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
-00002f90: 6f72 2028 6b65 792c 2076 616c 7565 2920  or (key, value) 
-00002fa0: 696e 2066 696c 6573 2e69 7465 6d73 2829  in files.items()
-00002fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002fc0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00002fd0: 2020 2020 6865 6164 6572 733d 6865 6164      headers=head
-00002fe0: 6572 7329 0a20 2020 2020 2020 2020 2020  ers).           
-00002ff0: 2063 6865 636b 5f65 7272 6f72 2872 6571   check_error(req
-00003000: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00003010: 7475 726e 2042 7974 6573 494f 2872 6571  turn BytesIO(req
-00003020: 2e63 6f6e 7465 6e74 292c 2072 6571 2e68  .content), req.h
-00003030: 6561 6465 7273 5b22 636f 6e74 656e 742d  eaders["content-
-00003040: 7479 7065 225d 0a20 2020 2020 2020 2072  type"].        r
-00003050: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00003060: 6622 756e 6b6e 6f77 6e20 6d65 7468 6f64  f"unknown method
-00003070: 207b 6d65 7468 6f64 7d22 290a 0a20 2020   {method}")..   
-00003080: 2064 6566 205f 6661 6c6c 6962 6c65 5f72   def _fallible_r
-00003090: 6177 5f72 6571 7565 7374 5f73 7472 280a  aw_request_str(.
-000030a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000030b0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-000030c0: 7468 6f64 3a20 7374 722c 0a20 2020 2020  thod: str,.     
-000030d0: 2020 2020 2020 2070 6174 683a 2073 7472         path: str
-000030e0: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-000030f0: 6773 3a20 4469 6374 5b73 7472 2c20 416e  gs: Dict[str, An
-00003100: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
-00003110: 6164 645f 7072 6566 6978 3a20 626f 6f6c  add_prefix: bool
-00003120: 2c0a 2020 2020 2020 2020 2020 2020 6164  ,.            ad
-00003130: 645f 6e61 6d65 7370 6163 653a 2062 6f6f  d_namespace: boo
-00003140: 6c2c 0a20 2020 2020 2020 2020 2020 2061  l,.            a
-00003150: 7069 5f76 6572 7369 6f6e 3a20 4f70 7469  pi_version: Opti
-00003160: 6f6e 616c 5b69 6e74 5d29 202d 3e20 5465  onal[int]) -> Te
-00003170: 7874 494f 3a0a 2020 2020 2020 2020 7072  xtIO:.        pr
-00003180: 6566 6978 203d 2022 220a 2020 2020 2020  efix = "".      
-00003190: 2020 6966 2061 6464 5f70 7265 6669 783a    if add_prefix:
-000031a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000031b0: 6170 695f 7665 7273 696f 6e20 6973 204e  api_version is N
-000031c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000031d0: 2020 2020 2061 7069 5f76 6572 7369 6f6e       api_version
-000031e0: 203d 2073 656c 662e 5f61 7069 5f76 6572   = self._api_ver
-000031f0: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
-00003200: 2070 7265 6669 7820 3d20 6622 7b50 5245   prefix = f"{PRE
-00003210: 4649 587d 2f76 7b61 7069 5f76 6572 7369  FIX}/v{api_versi
-00003220: 6f6e 7d22 0a20 2020 2020 2020 2075 726c  on}".        url
-00003230: 203d 2066 227b 7365 6c66 2e5f 7572 6c7d   = f"{self._url}
-00003240: 7b70 7265 6669 787d 7b70 6174 687d 220a  {prefix}{path}".
-00003250: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
-00003260: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00003270: 2261 7574 686f 7269 7a61 7469 6f6e 223a  "authorization":
-00003280: 2073 656c 662e 5f74 6f6b 656e 2c0a 2020   self._token,.  
-00003290: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000032a0: 6966 2061 6464 5f6e 616d 6573 7061 6365  if add_namespace
-000032b0: 3a0a 2020 2020 2020 2020 2020 2020 6172  :.            ar
-000032c0: 6773 5b22 6e61 6d65 7370 6163 6522 5d20  gs["namespace"] 
-000032d0: 3d20 7365 6c66 2e5f 6e61 6d65 7370 6163  = self._namespac
-000032e0: 650a 0a20 2020 2020 2020 2064 6566 2063  e..        def c
-000032f0: 6865 636b 5f65 7272 6f72 2872 6571 3a20  heck_error(req: 
-00003300: 5265 7370 6f6e 7365 2920 2d3e 204e 6f6e  Response) -> Non
-00003310: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00003320: 6620 7265 712e 7374 6174 7573 5f63 6f64  f req.status_cod
-00003330: 6520 3d3d 2034 3033 3a0a 2020 2020 2020  e == 403:.      
-00003340: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00003350: 4163 6365 7373 4465 6e69 6564 2872 6571  AccessDenied(req
-00003360: 2e74 6578 7429 0a20 2020 2020 2020 2020  .text).         
-00003370: 2020 2072 6571 2e72 6169 7365 5f66 6f72     req.raise_for
-00003380: 5f73 7461 7475 7328 290a 2020 2020 2020  _status().      
-00003390: 2020 2020 2020 6966 2072 6571 2e68 6561        if req.hea
-000033a0: 6465 7273 5b22 636f 6e74 656e 742d 7479  ders["content-ty
-000033b0: 7065 225d 203d 3d20 2261 7070 6c69 6361  pe"] == "applica
-000033c0: 7469 6f6e 2f70 726f 626c 656d 2b6a 736f  tion/problem+jso
-000033d0: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
-000033e0: 2020 2020 7261 6973 6520 5365 7276 6572      raise Server
-000033f0: 5369 6465 4572 726f 7228 6a73 6f6e 2e6c  SideError(json.l
-00003400: 6f61 6473 2872 6571 2e74 6578 7429 5b22  oads(req.text)["
-00003410: 6572 724d 6573 7361 6765 225d 290a 0a20  errMessage"]).. 
-00003420: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
-00003430: 203d 3d20 4d45 5448 4f44 5f47 4554 3a0a   == METHOD_GET:.
-00003440: 2020 2020 2020 2020 2020 2020 7265 7120              req 
-00003450: 3d20 7265 7175 6573 7473 2e67 6574 2875  = requests.get(u
-00003460: 726c 2c20 7061 7261 6d73 3d61 7267 732c  rl, params=args,
-00003470: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
-00003480: 290a 2020 2020 2020 2020 2020 2020 6368  ).            ch
-00003490: 6563 6b5f 6572 726f 7228 7265 7129 0a20  eck_error(req). 
-000034a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000034b0: 6e20 5374 7269 6e67 494f 2872 6571 2e74  n StringIO(req.t
-000034c0: 6578 7429 0a20 2020 2020 2020 2069 6620  ext).        if 
-000034d0: 6d65 7468 6f64 203d 3d20 4d45 5448 4f44  method == METHOD
-000034e0: 5f50 4f53 543a 0a20 2020 2020 2020 2020  _POST:.         
-000034f0: 2020 2072 6571 203d 2072 6571 7565 7374     req = request
-00003500: 732e 706f 7374 2875 726c 2c20 6a73 6f6e  s.post(url, json
-00003510: 3d61 7267 732c 2068 6561 6465 7273 3d68  =args, headers=h
-00003520: 6561 6465 7273 290a 2020 2020 2020 2020  eaders).        
-00003530: 2020 2020 6368 6563 6b5f 6572 726f 7228      check_error(
-00003540: 7265 7129 0a20 2020 2020 2020 2020 2020  req).           
-00003550: 2072 6574 7572 6e20 5374 7269 6e67 494f   return StringIO
-00003560: 2872 6571 2e74 6578 7429 0a20 2020 2020  (req.text).     
-00003570: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00003580: 726f 7228 6622 756e 6b6e 6f77 6e20 6d65  ror(f"unknown me
-00003590: 7468 6f64 207b 6d65 7468 6f64 7d22 290a  thod {method}").
-000035a0: 0a20 2020 2064 6566 205f 6661 6c6c 6962  .    def _fallib
-000035b0: 6c65 5f72 6177 5f72 6571 7565 7374 5f6a  le_raw_request_j
-000035c0: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
-000035d0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-000035e0: 2020 206d 6574 686f 643a 2073 7472 2c0a     method: str,.
-000035f0: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00003600: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-00003610: 2020 2061 7267 733a 2044 6963 745b 7374     args: Dict[st
-00003620: 722c 2041 6e79 5d2c 0a20 2020 2020 2020  r, Any],.       
-00003630: 2020 2020 2061 6464 5f70 7265 6669 783a       add_prefix:
-00003640: 2062 6f6f 6c2c 0a20 2020 2020 2020 2020   bool,.         
-00003650: 2020 2061 6464 5f6e 616d 6573 7061 6365     add_namespace
-00003660: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
-00003670: 2020 2020 6669 6c65 733a 204f 7074 696f      files: Optio
-00003680: 6e61 6c5b 4469 6374 5b73 7472 2c20 494f  nal[Dict[str, IO
-00003690: 5b62 7974 6573 5d5d 5d2c 0a20 2020 2020  [bytes]]],.     
-000036a0: 2020 2020 2020 2061 7069 5f76 6572 7369         api_versi
-000036b0: 6f6e 3a20 4f70 7469 6f6e 616c 5b69 6e74  on: Optional[int
-000036c0: 5d29 202d 3e20 4469 6374 5b73 7472 2c20  ]) -> Dict[str, 
-000036d0: 416e 795d 3a0a 2020 2020 2020 2020 7072  Any]:.        pr
-000036e0: 6566 6978 203d 2022 220a 2020 2020 2020  efix = "".      
-000036f0: 2020 6966 2061 6464 5f70 7265 6669 783a    if add_prefix:
-00003700: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003710: 6170 695f 7665 7273 696f 6e20 6973 204e  api_version is N
-00003720: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00003730: 2020 2020 2061 7069 5f76 6572 7369 6f6e       api_version
-00003740: 203d 2073 656c 662e 5f61 7069 5f76 6572   = self._api_ver
-00003750: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
-00003760: 2070 7265 6669 7820 3d20 6622 7b50 5245   prefix = f"{PRE
-00003770: 4649 587d 2f76 7b61 7069 5f76 6572 7369  FIX}/v{api_versi
-00003780: 6f6e 7d22 0a20 2020 2020 2020 2075 726c  on}".        url
-00003790: 203d 2066 227b 7365 6c66 2e5f 7572 6c7d   = f"{self._url}
-000037a0: 7b70 7265 6669 787d 7b70 6174 687d 220a  {prefix}{path}".
-000037b0: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
-000037c0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-000037d0: 2261 7574 686f 7269 7a61 7469 6f6e 223a  "authorization":
-000037e0: 2073 656c 662e 5f74 6f6b 656e 2c0a 2020   self._token,.  
-000037f0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00003800: 6966 2061 6464 5f6e 616d 6573 7061 6365  if add_namespace
-00003810: 3a0a 2020 2020 2020 2020 2020 2020 6172  :.            ar
-00003820: 6773 5b22 6e61 6d65 7370 6163 6522 5d20  gs["namespace"] 
-00003830: 3d20 7365 6c66 2e5f 6e61 6d65 7370 6163  = self._namespac
-00003840: 650a 2020 2020 2020 2020 6966 206d 6574  e.        if met
-00003850: 686f 6420 213d 204d 4554 484f 445f 4649  hod != METHOD_FI
-00003860: 4c45 2061 6e64 2066 696c 6573 2069 7320  LE and files is 
-00003870: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00003880: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00003890: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-000038a0: 2020 2020 2020 2020 6622 6669 6c65 7320          f"files 
-000038b0: 6172 6520 6f6e 6c79 2061 6c6c 6f77 2066  are only allow f
-000038c0: 6f72 2070 6f73 7420 2867 6f74 207b 6d65  or post (got {me
-000038d0: 7468 6f64 7d29 3a20 7b66 696c 6573 7d22  thod}): {files}"
-000038e0: 290a 2020 2020 2020 2020 7265 7120 3d20  ).        req = 
-000038f0: 4e6f 6e65 0a0a 2020 2020 2020 2020 6465  None..        de
-00003900: 6620 6368 6563 6b5f 6572 726f 7228 7265  f check_error(re
-00003910: 713a 2052 6573 706f 6e73 6529 202d 3e20  q: Response) -> 
-00003920: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003930: 2020 6966 2072 6571 2e73 7461 7475 735f    if req.status_
-00003940: 636f 6465 203d 3d20 3430 333a 0a20 2020  code == 403:.   
-00003950: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00003960: 7365 2041 6363 6573 7344 656e 6965 6428  se AccessDenied(
-00003970: 7265 712e 7465 7874 290a 2020 2020 2020  req.text).      
-00003980: 2020 2020 2020 7265 712e 7261 6973 655f        req.raise_
-00003990: 666f 725f 7374 6174 7573 2829 0a20 2020  for_status().   
-000039a0: 2020 2020 2020 2020 2069 6620 7265 712e           if req.
-000039b0: 6865 6164 6572 735b 2263 6f6e 7465 6e74  headers["content
-000039c0: 2d74 7970 6522 5d20 3d3d 2022 6170 706c  -type"] == "appl
-000039d0: 6963 6174 696f 6e2f 7072 6f62 6c65 6d2b  ication/problem+
-000039e0: 6a73 6f6e 223a 0a20 2020 2020 2020 2020  json":.         
-000039f0: 2020 2020 2020 2072 6169 7365 2053 6572         raise Ser
-00003a00: 7665 7253 6964 6545 7272 6f72 286a 736f  verSideError(jso
-00003a10: 6e2e 6c6f 6164 7328 7265 712e 7465 7874  n.loads(req.text
-00003a20: 295b 2265 7272 4d65 7373 6167 6522 5d29  )["errMessage"])
-00003a30: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
-00003a40: 2020 2020 2020 2020 2020 2069 6620 6d65             if me
-00003a50: 7468 6f64 203d 3d20 4d45 5448 4f44 5f47  thod == METHOD_G
-00003a60: 4554 3a0a 2020 2020 2020 2020 2020 2020  ET:.            
-00003a70: 2020 2020 7265 7120 3d20 7265 7175 6573      req = reques
-00003a80: 7473 2e67 6574 2875 726c 2c20 7061 7261  ts.get(url, para
-00003a90: 6d73 3d61 7267 732c 2068 6561 6465 7273  ms=args, headers
-00003aa0: 3d68 6561 6465 7273 290a 2020 2020 2020  =headers).      
-00003ab0: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
-00003ac0: 6572 726f 7228 7265 7129 0a20 2020 2020  error(req).     
-00003ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003ae0: 6e20 6a73 6f6e 2e6c 6f61 6473 2872 6571  n json.loads(req
-00003af0: 2e74 6578 7429 0a20 2020 2020 2020 2020  .text).         
-00003b00: 2020 2069 6620 6d65 7468 6f64 203d 3d20     if method == 
-00003b10: 4d45 5448 4f44 5f46 494c 453a 0a20 2020  METHOD_FILE:.   
-00003b20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003b30: 6669 6c65 7320 6973 204e 6f6e 653a 0a20  files is None:. 
-00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00003b60: 726f 7228 6622 6669 6c65 206d 6574 686f  ror(f"file metho
-00003b70: 6420 6d75 7374 2068 6176 6520 6669 6c65  d must have file
-00003b80: 733a 207b 6669 6c65 737d 2229 0a20 2020  s: {files}").   
-00003b90: 2020 2020 2020 2020 2020 2020 2072 6571               req
-00003ba0: 203d 2072 6571 7565 7374 732e 706f 7374   = requests.post
-00003bb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00003bc0: 2020 2020 2020 7572 6c2c 0a20 2020 2020        url,.     
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00003be0: 6174 613d 6172 6773 2c0a 2020 2020 2020  ata=args,.      
-00003bf0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00003c00: 6c65 733d 7b0a 2020 2020 2020 2020 2020  les={.          
-00003c10: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
-00003c20: 793a 2028 0a20 2020 2020 2020 2020 2020  y: (.           
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c40: 2067 6574 6174 7472 2876 616c 7565 2c20   getattr(value, 
-00003c50: 226e 616d 6522 2c20 6b65 7929 2c0a 2020  "name", key),.  
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c70: 2020 2020 2020 2020 2020 7661 6c75 652c            value,
-00003c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c90: 2020 2020 2020 2020 2020 2020 2022 6170               "ap
-00003ca0: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-00003cb0: 7374 7265 616d 222c 0a20 2020 2020 2020  stream",.       
-00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 2029 2066 6f72 2028 6b65 792c 2076 616c   ) for (key, val
-00003ce0: 7565 2920 696e 2066 696c 6573 2e69 7465  ue) in files.ite
-00003cf0: 6d73 2829 0a20 2020 2020 2020 2020 2020  ms().           
-00003d00: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 6865 6164 6572 733d 6865 6164 6572 7329  headers=headers)
-00003d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d40: 2063 6865 636b 5f65 7272 6f72 2872 6571   check_error(req
-00003d50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003d60: 2020 7265 7475 726e 206a 736f 6e2e 6c6f    return json.lo
-00003d70: 6164 7328 7265 712e 7465 7874 290a 2020  ads(req.text).  
-00003d80: 2020 2020 2020 2020 2020 6966 206d 6574            if met
-00003d90: 686f 6420 3d3d 204d 4554 484f 445f 504f  hod == METHOD_PO
-00003da0: 5354 3a0a 2020 2020 2020 2020 2020 2020  ST:.            
-00003db0: 2020 2020 7265 7120 3d20 7265 7175 6573      req = reques
-00003dc0: 7473 2e70 6f73 7428 7572 6c2c 206a 736f  ts.post(url, jso
-00003dd0: 6e3d 6172 6773 2c20 6865 6164 6572 733d  n=args, headers=
-00003de0: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
-00003df0: 2020 2020 2020 2020 2063 6865 636b 5f65           check_e
-00003e00: 7272 6f72 2872 6571 290a 2020 2020 2020  rror(req).      
-00003e10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003e20: 206a 736f 6e2e 6c6f 6164 7328 7265 712e   json.loads(req.
-00003e30: 7465 7874 290a 2020 2020 2020 2020 2020  text).          
-00003e40: 2020 6966 206d 6574 686f 6420 3d3d 204d    if method == M
-00003e50: 4554 484f 445f 5055 543a 0a20 2020 2020  ETHOD_PUT:.     
-00003e60: 2020 2020 2020 2020 2020 2072 6571 203d             req =
-00003e70: 2072 6571 7565 7374 732e 7075 7428 7572   requests.put(ur
-00003e80: 6c2c 206a 736f 6e3d 6172 6773 2c20 6865  l, json=args, he
-00003e90: 6164 6572 733d 6865 6164 6572 7329 0a20  aders=headers). 
-00003ea0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003eb0: 6865 636b 5f65 7272 6f72 2872 6571 290a  heck_error(req).
-00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ed0: 7265 7475 726e 206a 736f 6e2e 6c6f 6164  return json.load
-00003ee0: 7328 7265 712e 7465 7874 290a 2020 2020  s(req.text).    
-00003ef0: 2020 2020 2020 2020 6966 206d 6574 686f          if metho
-00003f00: 6420 3d3d 204d 4554 484f 445f 4445 4c45  d == METHOD_DELE
-00003f10: 5445 3a0a 2020 2020 2020 2020 2020 2020  TE:.            
-00003f20: 2020 2020 7265 7120 3d20 7265 7175 6573      req = reques
-00003f30: 7473 2e64 656c 6574 6528 7572 6c2c 206a  ts.delete(url, j
-00003f40: 736f 6e3d 6172 6773 2c20 6865 6164 6572  son=args, header
-00003f50: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
-00003f60: 2020 2020 2020 2020 2020 2063 6865 636b             check
-00003f70: 5f65 7272 6f72 2872 6571 290a 2020 2020  _error(req).    
-00003f80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003f90: 726e 206a 736f 6e2e 6c6f 6164 7328 7265  rn json.loads(re
-00003fa0: 712e 7465 7874 290a 2020 2020 2020 2020  q.text).        
-00003fb0: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
-00003fc0: 204d 4554 484f 445f 4c4f 4e47 504f 5354   METHOD_LONGPOST
-00003fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003fe0: 2020 6172 6773 5b22 746f 6b65 6e22 5d20    args["token"] 
-00003ff0: 3d20 7365 6c66 2e5f 746f 6b65 6e0a 2020  = self._token.  
-00004000: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00004010: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00004020: 2020 2020 2020 2072 6573 203d 2071 7569         res = qui
-00004030: 636b 5f73 6572 7665 722e 776f 726b 6572  ck_server.worker
-00004040: 5f72 6571 7565 7374 2875 726c 2c20 6172  _request(url, ar
-00004050: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
-00004060: 2020 2020 2020 2020 6966 2022 6572 724d          if "errM
-00004070: 6573 7361 6765 2220 696e 2072 6573 3a0a  essage" in res:.
-00004080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004090: 2020 2020 2020 2020 7261 6973 6520 5365          raise Se
-000040a0: 7276 6572 5369 6465 4572 726f 7228 7265  rverSideError(re
-000040b0: 735b 2265 7272 4d65 7373 6167 6522 5d29  s["errMessage"])
-000040c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040d0: 2020 2020 2072 6574 7572 6e20 7265 730a       return res.
-000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040f0: 6578 6365 7074 2071 7569 636b 5f73 6572  except quick_ser
-00004100: 7665 722e 576f 726b 6572 4572 726f 7220  ver.WorkerError 
-00004110: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00004120: 2020 2020 2020 2020 2020 6966 2065 2e67            if e.g
-00004130: 6574 5f73 7461 7475 735f 636f 6465 2829  et_status_code()
-00004140: 203d 3d20 3430 333a 0a20 2020 2020 2020   == 403:.       
-00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2072 6169 7365 2041 6363 6573 7344 656e   raise AccessDen
-00004170: 6965 6428 652e 6172 6773 2920 6672 6f6d  ied(e.args) from
-00004180: 2065 0a20 2020 2020 2020 2020 2020 2020   e.             
-00004190: 2020 2020 2020 2072 6169 7365 2065 0a20         raise e. 
-000041a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000041b0: 2056 616c 7565 4572 726f 7228 6622 756e   ValueError(f"un
-000041c0: 6b6e 6f77 6e20 6d65 7468 6f64 207b 6d65  known method {me
-000041d0: 7468 6f64 7d22 290a 2020 2020 2020 2020  thod}").        
-000041e0: 6578 6365 7074 206a 736f 6e2e 6465 636f  except json.deco
-000041f0: 6465 722e 4a53 4f4e 4465 636f 6465 4572  der.JSONDecodeEr
-00004200: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-00004210: 2020 2020 2020 6966 2072 6571 2069 7320        if req is 
-00004220: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00004230: 2020 2020 2020 7261 6973 650a 2020 2020        raise.    
-00004240: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00004250: 6c75 6545 7272 6f72 2872 6571 2e74 6578  lueError(req.tex
-00004260: 7429 2066 726f 6d20 650a 0a20 2020 2064  t) from e..    d
-00004270: 6566 2072 6571 7565 7374 5f62 7974 6573  ef request_bytes
-00004280: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00004290: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-000042a0: 6d65 7468 6f64 3a20 7374 722c 0a20 2020  method: str,.   
-000042b0: 2020 2020 2020 2020 2070 6174 683a 2073           path: s
-000042c0: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-000042d0: 6172 6773 3a20 4469 6374 5b73 7472 2c20  args: Dict[str, 
-000042e0: 416e 795d 2c0a 2020 2020 2020 2020 2020  Any],.          
-000042f0: 2020 6669 6c65 733a 204f 7074 696f 6e61    files: Optiona
-00004300: 6c5b 4469 6374 5b73 7472 2c20 4279 7465  l[Dict[str, Byte
-00004310: 7349 4f5d 5d20 3d20 4e6f 6e65 2c0a 2020  sIO]] = None,.  
-00004320: 2020 2020 2020 2020 2020 6164 645f 7072            add_pr
-00004330: 6566 6978 3a20 626f 6f6c 203d 2054 7275  efix: bool = Tru
-00004340: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
-00004350: 6464 5f6e 616d 6573 7061 6365 3a20 626f  dd_namespace: bo
-00004360: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-00004370: 2020 2020 2020 2061 7069 5f76 6572 7369         api_versi
-00004380: 6f6e 3a20 4f70 7469 6f6e 616c 5b69 6e74  on: Optional[int
-00004390: 5d20 3d20 4e6f 6e65 2920 2d3e 2054 7570  ] = None) -> Tup
-000043a0: 6c65 5b42 7974 6573 494f 2c20 7374 725d  le[BytesIO, str]
-000043b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000043c0: 2073 656c 662e 5f72 6177 5f72 6571 7565   self._raw_reque
-000043d0: 7374 5f62 7974 6573 280a 2020 2020 2020  st_bytes(.      
-000043e0: 2020 2020 2020 6d65 7468 6f64 2c20 7061        method, pa
-000043f0: 7468 2c20 6172 6773 2c20 6669 6c65 732c  th, args, files,
-00004400: 2061 6464 5f70 7265 6669 782c 2061 6464   add_prefix, add
-00004410: 5f6e 616d 6573 7061 6365 2c20 6170 695f  _namespace, api_
-00004420: 7665 7273 696f 6e29 0a0a 2020 2020 6465  version)..    de
-00004430: 6620 7265 7175 6573 745f 6a73 6f6e 280a  f request_json(.
-00004440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004450: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-00004460: 7468 6f64 3a20 7374 722c 0a20 2020 2020  thod: str,.     
-00004470: 2020 2020 2020 2070 6174 683a 2073 7472         path: str
-00004480: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-00004490: 6773 3a20 4469 6374 5b73 7472 2c20 416e  gs: Dict[str, An
-000044a0: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
-000044b0: 6164 645f 7072 6566 6978 3a20 626f 6f6c  add_prefix: bool
-000044c0: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-000044d0: 2020 2020 2061 6464 5f6e 616d 6573 7061       add_namespa
-000044e0: 6365 3a20 626f 6f6c 203d 2054 7275 652c  ce: bool = True,
-000044f0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00004500: 6573 3a20 4f70 7469 6f6e 616c 5b44 6963  es: Optional[Dic
-00004510: 745b 7374 722c 2049 4f5b 6279 7465 735d  t[str, IO[bytes]
-00004520: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00004530: 2020 2020 2020 2061 7069 5f76 6572 7369         api_versi
-00004540: 6f6e 3a20 4f70 7469 6f6e 616c 5b69 6e74  on: Optional[int
-00004550: 5d20 3d20 4e6f 6e65 2920 2d3e 2044 6963  ] = None) -> Dic
-00004560: 745b 7374 722c 2041 6e79 5d3a 0a20 2020  t[str, Any]:.   
-00004570: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00004580: 2e5f 7261 775f 7265 7175 6573 745f 6a73  ._raw_request_js
-00004590: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-000045a0: 6d65 7468 6f64 2c20 7061 7468 2c20 6172  method, path, ar
-000045b0: 6773 2c20 6164 645f 7072 6566 6978 2c20  gs, add_prefix, 
-000045c0: 6164 645f 6e61 6d65 7370 6163 652c 2066  add_namespace, f
-000045d0: 696c 6573 2c20 6170 695f 7665 7273 696f  iles, api_versio
-000045e0: 6e29 0a0a 2020 2020 6465 6620 6765 745f  n)..    def get_
-000045f0: 7365 7276 6572 5f76 6572 7369 6f6e 2873  server_version(s
-00004600: 656c 6629 202d 3e20 5665 7273 696f 6e52  elf) -> VersionR
-00004610: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00004620: 2072 6574 7572 6e20 6361 7374 2856 6572   return cast(Ver
-00004630: 7369 6f6e 5265 7370 6f6e 7365 2c20 7365  sionResponse, se
-00004640: 6c66 2e72 6571 7565 7374 5f6a 736f 6e28  lf.request_json(
-00004650: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00004660: 484f 445f 4745 542c 0a20 2020 2020 2020  HOD_GET,.       
-00004670: 2020 2020 2066 227b 5052 4546 4958 7d2f       f"{PREFIX}/
-00004680: 767b 4150 495f 5645 5253 494f 4e7d 2f76  v{API_VERSION}/v
-00004690: 6572 7369 6f6e 222c 0a20 2020 2020 2020  ersion",.       
-000046a0: 2020 2020 207b 7d2c 0a20 2020 2020 2020       {},.       
-000046b0: 2020 2020 2061 6464 5f70 7265 6669 783d       add_prefix=
-000046c0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-000046d0: 2020 2061 6464 5f6e 616d 6573 7061 6365     add_namespace
-000046e0: 3d46 616c 7365 2929 0a0a 2020 2020 6465  =False))..    de
-000046f0: 6620 6765 745f 7665 7273 696f 6e5f 6f76  f get_version_ov
-00004700: 6572 7269 6465 2873 656c 6629 202d 3e20  erride(self) -> 
-00004710: 4469 6374 5b73 7472 2c20 4c69 7374 5b4f  Dict[str, List[O
-00004720: 7074 696f 6e61 6c5b 7374 725d 5d5d 3a0a  ptional[str]]]:.
-00004730: 2020 2020 2020 2020 7365 7276 6572 5f76          server_v
-00004740: 6572 7369 6f6e 203d 2073 656c 662e 6765  ersion = self.ge
-00004750: 745f 7365 7276 6572 5f76 6572 7369 6f6e  t_server_version
-00004760: 2829 0a20 2020 2020 2020 2069 6d67 5f72  ().        img_r
-00004770: 6570 6f20 3d20 7365 7276 6572 5f76 6572  epo = server_ver
-00004780: 7369 6f6e 5b22 696d 6167 655f 7265 706f  sion["image_repo
-00004790: 225d 0a20 2020 2020 2020 2069 6d67 5f74  "].        img_t
-000047a0: 6167 203d 2073 6572 7665 725f 7665 7273  ag = server_vers
-000047b0: 696f 6e5b 2269 6d61 6765 5f74 6167 225d  ion["image_tag"]
-000047c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000047d0: 7b0a 2020 2020 2020 2020 2020 2020 2276  {.            "v
-000047e0: 6572 7369 6f6e 223a 205b 696d 675f 7265  ersion": [img_re
-000047f0: 706f 2c20 696d 675f 7461 675d 2c0a 2020  po, img_tag],.  
-00004800: 2020 2020 2020 7d0a 0a20 2020 2064 6566        }..    def
-00004810: 2067 6574 5f6e 616d 6573 7061 6365 7328   get_namespaces(
-00004820: 7365 6c66 2920 2d3e 204c 6973 745b 7374  self) -> List[st
-00004830: 725d 3a0a 2020 2020 2020 2020 7265 7475  r]:.        retu
-00004840: 726e 2063 6173 7428 4e61 6d65 7370 6163  rn cast(Namespac
-00004850: 654c 6973 742c 2073 656c 662e 7265 7175  eList, self.requ
-00004860: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-00004870: 2020 2020 2020 4d45 5448 4f44 5f47 4554        METHOD_GET
-00004880: 2c20 222f 6e61 6d65 7370 6163 6573 222c  , "/namespaces",
-00004890: 207b 7d29 295b 226e 616d 6573 7061 6365   {}))["namespace
-000048a0: 7322 5d0a 0a20 2020 2064 6566 2067 6574  s"]..    def get
-000048b0: 5f64 6167 7328 7365 6c66 2920 2d3e 204c  _dags(self) -> L
-000048c0: 6973 745b 7374 725d 3a0a 2020 2020 2020  ist[str]:.      
-000048d0: 2020 7265 7475 726e 205b 0a20 2020 2020    return [.     
-000048e0: 2020 2020 2020 2072 6573 5b22 6461 6722         res["dag"
-000048f0: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00004900: 7220 7265 7320 696e 2073 656c 662e 6765  r res in self.ge
-00004910: 745f 6461 675f 7469 6d65 7328 7265 7472  t_dag_times(retr
-00004920: 6965 7665 5f74 696d 6573 3d46 616c 7365  ieve_times=False
-00004930: 295b 315d 0a20 2020 2020 2020 205d 0a0a  )[1].        ]..
-00004940: 2020 2020 6465 6620 6765 745f 6461 675f      def get_dag_
-00004950: 6167 6573 2873 656c 6629 202d 3e20 4c69  ages(self) -> Li
-00004960: 7374 5b44 6963 745b 7374 722c 204f 7074  st[Dict[str, Opt
-00004970: 696f 6e61 6c5b 7374 725d 5d5d 3a0a 2020  ional[str]]]:.  
-00004980: 2020 2020 2020 6375 725f 7469 6d65 2c20        cur_time, 
-00004990: 6461 6773 203d 2073 656c 662e 6765 745f  dags = self.get_
-000049a0: 6461 675f 7469 6d65 7328 7265 7472 6965  dag_times(retrie
-000049b0: 7665 5f74 696d 6573 3d54 7275 6529 0a20  ve_times=True). 
-000049c0: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
-000049d0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000049f0: 6f6e 6669 675f 6572 726f 7222 3a20 6461  onfig_error": da
-00004a00: 675f 7374 6174 7573 5b22 636f 6e66 6967  g_status["config
-00004a10: 5f65 7272 6f72 225d 2c0a 2020 2020 2020  _error"],.      
-00004a20: 2020 2020 2020 2020 2020 2263 7265 6174            "creat
-00004a30: 6564 223a 2067 6574 5f61 6765 2863 7572  ed": get_age(cur
-00004a40: 5f74 696d 652c 2064 6167 5f73 7461 7475  _time, dag_statu
-00004a50: 735b 2263 7265 6174 6564 225d 292c 0a20  s["created"]),. 
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004a70: 6461 6722 3a20 6461 675f 7374 6174 7573  dag": dag_status
-00004a80: 5b22 6461 6722 5d2c 0a20 2020 2020 2020  ["dag"],.       
-00004a90: 2020 2020 2020 2020 2022 6465 6c65 7465           "delete
-00004aa0: 6422 3a20 6765 745f 6167 6528 6375 725f  d": get_age(cur_
-00004ab0: 7469 6d65 2c20 6461 675f 7374 6174 7573  time, dag_status
-00004ac0: 5b22 6465 6c65 7465 6422 5d29 2c0a 2020  ["deleted"]),.  
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00004ae0: 6174 6573 7422 3a20 6765 745f 6167 6528  atest": get_age(
-00004af0: 6375 725f 7469 6d65 2c20 6461 675f 7374  cur_time, dag_st
-00004b00: 6174 7573 5b22 6c61 7465 7374 225d 292c  atus["latest"]),
-00004b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b20: 2022 6f6c 6465 7374 223a 2067 6574 5f61   "oldest": get_a
-00004b30: 6765 2863 7572 5f74 696d 652c 2064 6167  ge(cur_time, dag
-00004b40: 5f73 7461 7475 735b 226f 6c64 6573 7422  _status["oldest"
-00004b50: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00004b60: 7d0a 2020 2020 2020 2020 2020 2020 666f  }.            fo
-00004b70: 7220 6461 675f 7374 6174 7573 2069 6e20  r dag_status in 
-00004b80: 736f 7274 6564 2864 6167 732c 206b 6579  sorted(dags, key
-00004b90: 3d6c 616d 6264 6120 656c 3a20 280a 2020  =lambda el: (.  
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00004bb0: 5b22 636f 6e66 6967 5f65 7272 6f72 225d  ["config_error"]
-00004bc0: 2069 7320 4e6f 6e65 2c0a 2020 2020 2020   is None,.      
-00004bd0: 2020 2020 2020 2020 2020 7361 6665 5f6f            safe_o
-00004be0: 7074 5f6e 756d 2865 6c5b 226f 6c64 6573  pt_num(el["oldes
-00004bf0: 7422 5d29 2c0a 2020 2020 2020 2020 2020  t"]),.          
-00004c00: 2020 2020 2020 7361 6665 5f6f 7074 5f6e        safe_opt_n
-00004c10: 756d 2865 6c5b 226c 6174 6573 7422 5d29  um(el["latest"])
-00004c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004c30: 2020 656c 5b22 6461 6722 5d29 290a 2020    el["dag"])).  
-00004c40: 2020 2020 2020 5d0a 0a20 2020 2064 6566        ]..    def
-00004c50: 2067 6574 5f64 6167 5f74 696d 6573 2873   get_dag_times(s
-00004c60: 656c 662c 2072 6574 7269 6576 655f 7469  elf, retrieve_ti
-00004c70: 6d65 733a 2062 6f6f 6c20 3d20 5472 7565  mes: bool = True
-00004c80: 2920 2d3e 2054 7570 6c65 5b0a 2020 2020  ) -> Tuple[.    
-00004c90: 2020 2020 2020 2020 666c 6f61 742c 204c          float, L
-00004ca0: 6973 745b 4461 6753 7461 7475 735d 5d3a  ist[DagStatus]]:
-00004cb0: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
-00004cc0: 6173 7428 4461 674c 6973 742c 2073 656c  ast(DagList, sel
-00004cd0: 662e 7265 7175 6573 745f 6a73 6f6e 280a  f.request_json(.
-00004ce0: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
-00004cf0: 4f44 5f47 4554 2c20 222f 6461 6773 222c  OD_GET, "/dags",
-00004d00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004d10: 2020 2022 7265 7472 6965 7665 5f74 696d     "retrieve_tim
-00004d20: 6573 223a 2069 6e74 2872 6574 7269 6576  es": int(retriev
-00004d30: 655f 7469 6d65 7329 2c0a 2020 2020 2020  e_times),.      
-00004d40: 2020 2020 2020 7d29 290a 2020 2020 2020        })).      
-00004d50: 2020 7265 7475 726e 2072 6573 5b22 6375    return res["cu
-00004d60: 725f 7469 6d65 225d 2c20 7265 735b 2264  r_time"], res["d
-00004d70: 6167 7322 5d0a 0a20 2020 2064 6566 2067  ags"]..    def g
-00004d80: 6574 5f64 6167 2873 656c 662c 2064 6167  et_dag(self, dag
-00004d90: 5f75 7269 3a20 7374 7229 202d 3e20 2744  _uri: str) -> 'D
-00004da0: 6167 4861 6e64 6c65 273a 0a20 2020 2020  agHandle':.     
-00004db0: 2020 2072 6573 203d 2073 656c 662e 5f64     res = self._d
-00004dc0: 6167 5f63 6163 6865 2e67 6574 2864 6167  ag_cache.get(dag
-00004dd0: 5f75 7269 290a 2020 2020 2020 2020 6966  _uri).        if
-00004de0: 2072 6573 2069 7320 6e6f 7420 4e6f 6e65   res is not None
-00004df0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00004e00: 7475 726e 2072 6573 0a20 2020 2020 2020  turn res.       
-00004e10: 2072 6573 203d 2044 6167 4861 6e64 6c65   res = DagHandle
-00004e20: 2873 656c 662c 2064 6167 5f75 7269 290a  (self, dag_uri).
-00004e30: 2020 2020 2020 2020 7365 6c66 2e5f 6461          self._da
-00004e40: 675f 6361 6368 655b 6461 675f 7572 695d  g_cache[dag_uri]
-00004e50: 203d 2072 6573 0a20 2020 2020 2020 2072   = res.        r
-00004e60: 6574 7572 6e20 7265 730a 0a20 2020 2064  eturn res..    d
-00004e70: 6566 2067 6574 5f62 6c6f 625f 6861 6e64  ef get_blob_hand
-00004e80: 6c65 2873 656c 662c 2075 7269 3a20 7374  le(self, uri: st
-00004e90: 722c 2069 735f 6675 6c6c 3a20 626f 6f6c  r, is_full: bool
-00004ea0: 203d 2046 616c 7365 2920 2d3e 2027 426c   = False) -> 'Bl
-00004eb0: 6f62 4861 6e64 6c65 273a 0a20 2020 2020  obHandle':.     
-00004ec0: 2020 2072 6574 7572 6e20 426c 6f62 4861     return BlobHa
-00004ed0: 6e64 6c65 2873 656c 662c 2075 7269 2c20  ndle(self, uri, 
-00004ee0: 6973 5f66 756c 6c3d 6973 5f66 756c 6c29  is_full=is_full)
-00004ef0: 0a0a 2020 2020 6465 6620 6765 745f 6e6f  ..    def get_no
-00004f00: 6465 5f64 6566 7328 7365 6c66 2920 2d3e  de_defs(self) ->
-00004f10: 2044 6963 745b 7374 722c 204e 6f64 6544   Dict[str, NodeD
-00004f20: 6566 496e 666f 5d3a 0a20 2020 2020 2020  efInfo]:.       
-00004f30: 2073 656c 662e 5f6d 6179 6265 5f72 6566   self._maybe_ref
-00004f40: 7265 7368 2829 0a20 2020 2020 2020 2069  resh().        i
-00004f50: 6620 7365 6c66 2e5f 6e6f 6465 5f64 6566  f self._node_def
-00004f60: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00004f70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004f80: 6e20 7365 6c66 2e5f 6e6f 6465 5f64 6566  n self._node_def
-00004f90: 730a 2020 2020 2020 2020 7265 7320 3d20  s.        res = 
-00004fa0: 6361 7374 284e 6f64 6554 7970 6573 2c20  cast(NodeTypes, 
-00004fb0: 7365 6c66 2e72 6571 7565 7374 5f6a 736f  self.request_jso
-00004fc0: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-00004fd0: 4554 484f 445f 4745 542c 2022 2f6e 6f64  ETHOD_GET, "/nod
-00004fe0: 655f 7479 7065 7322 2c20 7b7d 2c20 6164  e_types", {}, ad
-00004ff0: 645f 6e61 6d65 7370 6163 653d 4661 6c73  d_namespace=Fals
-00005000: 6529 295b 2269 6e66 6f22 5d0a 2020 2020  e))["info"].    
-00005010: 2020 2020 7365 6c66 2e5f 6e6f 6465 5f64      self._node_d
-00005020: 6566 7320 3d20 7265 730a 2020 2020 2020  efs = res.      
-00005030: 2020 7265 7475 726e 2072 6573 0a0a 2020    return res..  
-00005040: 2020 6465 6620 6372 6561 7465 5f6e 6577    def create_new
-00005050: 5f62 6c6f 6228 7365 6c66 2c20 626c 6f62  _blob(self, blob
-00005060: 5f74 7970 653a 2073 7472 2920 2d3e 2073  _type: str) -> s
-00005070: 7472 3a0a 2020 2020 2020 2020 7265 7475  tr:.        retu
-00005080: 726e 2063 6173 7428 426c 6f62 496e 6974  rn cast(BlobInit
-00005090: 2c20 7365 6c66 2e72 6571 7565 7374 5f6a  , self.request_j
-000050a0: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
-000050b0: 204d 4554 484f 445f 504f 5354 2c20 222f   METHOD_POST, "/
-000050c0: 626c 6f62 5f69 6e69 7422 2c20 7b0a 2020  blob_init", {.  
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000050e0: 7970 6522 3a20 626c 6f62 5f74 7970 652c  ype": blob_type,
-000050f0: 0a20 2020 2020 2020 2020 2020 207d 2c20  .            }, 
-00005100: 6164 645f 6e61 6d65 7370 6163 653d 4661  add_namespace=Fa
-00005110: 6c73 6529 295b 2262 6c6f 6222 5d0a 0a20  lse))["blob"].. 
-00005120: 2020 2064 6566 2067 6574 5f62 6c6f 625f     def get_blob_
-00005130: 6f77 6e65 7228 7365 6c66 2c20 626c 6f62  owner(self, blob
-00005140: 5f75 7269 3a20 7374 7229 202d 3e20 426c  _uri: str) -> Bl
-00005150: 6f62 4f77 6e65 723a 0a20 2020 2020 2020  obOwner:.       
-00005160: 2072 6574 7572 6e20 6361 7374 2842 6c6f   return cast(Blo
-00005170: 624f 776e 6572 2c20 7365 6c66 2e72 6571  bOwner, self.req
-00005180: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-00005190: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
-000051a0: 542c 2022 2f62 6c6f 625f 6f77 6e65 7222  T, "/blob_owner"
-000051b0: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
-000051c0: 2020 2020 2262 6c6f 6222 3a20 626c 6f62      "blob": blob
-000051d0: 5f75 7269 2c0a 2020 2020 2020 2020 2020  _uri,.          
-000051e0: 2020 7d29 290a 0a20 2020 2064 6566 2073    }))..    def s
-000051f0: 6574 5f62 6c6f 625f 6f77 6e65 7228 0a20  et_blob_owner(. 
-00005200: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00005210: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
-00005220: 625f 7572 693a 2073 7472 2c0a 2020 2020  b_uri: str,.    
-00005230: 2020 2020 2020 2020 6461 675f 6964 3a20          dag_id: 
-00005240: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00005250: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00005260: 2020 6e6f 6465 5f69 643a 204f 7074 696f    node_id: Optio
-00005270: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00005280: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-00005290: 6572 6e61 6c5f 6f77 6e65 723a 2062 6f6f  ernal_owner: boo
-000052a0: 6c20 3d20 4661 6c73 6529 202d 3e20 426c  l = False) -> Bl
-000052b0: 6f62 4f77 6e65 723a 0a20 2020 2020 2020  obOwner:.       
-000052c0: 2072 6574 7572 6e20 6361 7374 2842 6c6f   return cast(Blo
-000052d0: 624f 776e 6572 2c20 7365 6c66 2e72 6571  bOwner, self.req
-000052e0: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-000052f0: 2020 2020 2020 204d 4554 484f 445f 5055         METHOD_PU
-00005300: 542c 2022 2f62 6c6f 625f 6f77 6e65 7222  T, "/blob_owner"
-00005310: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
-00005320: 2020 2020 2262 6c6f 6222 3a20 626c 6f62      "blob": blob
-00005330: 5f75 7269 2c0a 2020 2020 2020 2020 2020  _uri,.          
-00005340: 2020 2020 2020 226f 776e 6572 5f64 6167        "owner_dag
-00005350: 223a 2064 6167 5f69 642c 0a20 2020 2020  ": dag_id,.     
-00005360: 2020 2020 2020 2020 2020 2022 6f77 6e65             "owne
-00005370: 725f 6e6f 6465 223a 206e 6f64 655f 6964  r_node": node_id
-00005380: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005390: 2020 2265 7874 6572 6e61 6c5f 6f77 6e65    "external_owne
-000053a0: 7222 3a20 6578 7465 726e 616c 5f6f 776e  r": external_own
-000053b0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000053c0: 7d29 290a 0a20 2020 2064 6566 2063 7265  }))..    def cre
-000053d0: 6174 655f 6e65 775f 6461 6728 0a20 2020  ate_new_dag(.   
-000053e0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-000053f0: 2020 2020 2020 2020 2020 2075 7365 726e             usern
-00005400: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-00005410: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00005420: 2020 2020 2020 2064 6167 6e61 6d65 3a20         dagname: 
-00005430: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00005440: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00005450: 2020 696e 6465 783a 204f 7074 696f 6e61    index: Optiona
-00005460: 6c5b 696e 745d 203d 204e 6f6e 6529 202d  l[int] = None) -
-00005470: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
-00005480: 6574 7572 6e20 6361 7374 2844 6167 496e  eturn cast(DagIn
-00005490: 6974 2c20 7365 6c66 2e72 6571 7565 7374  it, self.request
-000054a0: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
-000054b0: 2020 204d 4554 484f 445f 504f 5354 2c20     METHOD_POST, 
-000054c0: 222f 6461 675f 696e 6974 222c 207b 0a20  "/dag_init", {. 
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000054e0: 7573 6572 223a 2075 7365 726e 616d 652c  user": username,
-000054f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005500: 2022 6e61 6d65 223a 2064 6167 6e61 6d65   "name": dagname
-00005510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005520: 2020 2269 6e64 6578 223a 2069 6e64 6578    "index": index
-00005530: 2c0a 2020 2020 2020 2020 2020 2020 7d29  ,.            })
-00005540: 295b 2264 6167 225d 0a0a 2020 2020 6465  )["dag"]..    de
-00005550: 6620 6765 745f 626c 6f62 5f74 7970 6528  f get_blob_type(
-00005560: 7365 6c66 2c20 626c 6f62 5f75 7269 3a20  self, blob_uri: 
-00005570: 7374 7229 202d 3e20 426c 6f62 5479 7065  str) -> BlobType
-00005580: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00005590: 2020 7265 7475 726e 2063 6173 7428 426c    return cast(Bl
-000055a0: 6f62 5479 7065 5265 7370 6f6e 7365 2c20  obTypeResponse, 
-000055b0: 7365 6c66 2e72 6571 7565 7374 5f6a 736f  self.request_jso
-000055c0: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-000055d0: 4554 484f 445f 4745 542c 2022 2f62 6c6f  ETHOD_GET, "/blo
-000055e0: 625f 7479 7065 222c 207b 0a20 2020 2020  b_type", {.     
-000055f0: 2020 2020 2020 2020 2020 2022 626c 6f62             "blob
-00005600: 5f75 7269 223a 2062 6c6f 625f 7572 692c  _uri": blob_uri,
-00005610: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00005620: 2020 2020 2020 2020 2929 0a0a 2020 2020          ))..    
-00005630: 6465 6620 6765 745f 6373 765f 626c 6f62  def get_csv_blob
-00005640: 2873 656c 662c 2062 6c6f 625f 7572 693a  (self, blob_uri:
-00005650: 2073 7472 2920 2d3e 2027 4353 5642 6c6f   str) -> 'CSVBlo
-00005660: 6248 616e 646c 6527 3a0a 2020 2020 2020  bHandle':.      
-00005670: 2020 626c 6f62 5f74 7970 6520 3d20 7365    blob_type = se
-00005680: 6c66 2e67 6574 5f62 6c6f 625f 7479 7065  lf.get_blob_type
-00005690: 2862 6c6f 625f 7572 6929 0a20 2020 2020  (blob_uri).     
-000056a0: 2020 2069 6620 6e6f 7420 626c 6f62 5f74     if not blob_t
-000056b0: 7970 655b 2269 735f 6373 7622 5d3a 0a20  ype["is_csv"]:. 
-000056c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000056d0: 2056 616c 7565 4572 726f 7228 6622 626c   ValueError(f"bl
-000056e0: 6f62 3a20 7b62 6c6f 625f 7572 697d 2069  ob: {blob_uri} i
-000056f0: 7320 6e6f 7420 6373 7620 7479 7065 2229  s not csv type")
-00005700: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005710: 4353 5642 6c6f 6248 616e 646c 6528 7365  CSVBlobHandle(se
-00005720: 6c66 2c20 626c 6f62 5f75 7269 2c20 6973  lf, blob_uri, is
-00005730: 5f66 756c 6c3d 4661 6c73 6529 0a0a 2020  _full=False)..  
-00005740: 2020 6465 6620 6765 745f 746f 7263 685f    def get_torch_
-00005750: 626c 6f62 2873 656c 662c 2062 6c6f 625f  blob(self, blob_
-00005760: 7572 693a 2073 7472 2920 2d3e 2027 546f  uri: str) -> 'To
-00005770: 7263 6842 6c6f 6248 616e 646c 6527 3a0a  rchBlobHandle':.
-00005780: 2020 2020 2020 2020 626c 6f62 5f74 7970          blob_typ
-00005790: 6520 3d20 7365 6c66 2e67 6574 5f62 6c6f  e = self.get_blo
-000057a0: 625f 7479 7065 2862 6c6f 625f 7572 6929  b_type(blob_uri)
-000057b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000057c0: 626c 6f62 5f74 7970 655b 2269 735f 746f  blob_type["is_to
-000057d0: 7263 6822 5d3a 0a20 2020 2020 2020 2020  rch"]:.         
-000057e0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000057f0: 726f 7228 6622 626c 6f62 3a20 7b62 6c6f  ror(f"blob: {blo
-00005800: 625f 7572 697d 2069 7320 6e6f 7420 746f  b_uri} is not to
-00005810: 7263 6820 7479 7065 2229 0a20 2020 2020  rch type").     
-00005820: 2020 2072 6574 7572 6e20 546f 7263 6842     return TorchB
-00005830: 6c6f 6248 616e 646c 6528 7365 6c66 2c20  lobHandle(self, 
-00005840: 626c 6f62 5f75 7269 2c20 6973 5f66 756c  blob_uri, is_ful
-00005850: 6c3d 4661 6c73 6529 0a0a 2020 2020 6465  l=False)..    de
-00005860: 6620 6765 745f 6375 7374 6f6d 5f63 6f64  f get_custom_cod
-00005870: 655f 626c 6f62 2873 656c 662c 2062 6c6f  e_blob(self, blo
-00005880: 625f 7572 693a 2073 7472 2920 2d3e 2027  b_uri: str) -> '
-00005890: 4375 7374 6f6d 436f 6465 426c 6f62 4861  CustomCodeBlobHa
-000058a0: 6e64 6c65 273a 0a20 2020 2020 2020 2062  ndle':.        b
-000058b0: 6c6f 625f 7479 7065 203d 2073 656c 662e  lob_type = self.
-000058c0: 6765 745f 626c 6f62 5f74 7970 6528 626c  get_blob_type(bl
-000058d0: 6f62 5f75 7269 290a 2020 2020 2020 2020  ob_uri).        
-000058e0: 6966 206e 6f74 2062 6c6f 625f 7479 7065  if not blob_type
-000058f0: 5b22 6973 5f63 7573 746f 6d5f 636f 6465  ["is_custom_code
-00005900: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00005910: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00005920: 2866 2262 6c6f 623a 207b 626c 6f62 5f75  (f"blob: {blob_u
-00005930: 7269 7d20 6973 206e 6f74 2063 7573 746f  ri} is not custo
-00005940: 6d20 636f 6465 2074 7970 6522 290a 2020  m code type").  
-00005950: 2020 2020 2020 7265 7475 726e 2043 7573        return Cus
-00005960: 746f 6d43 6f64 6542 6c6f 6248 616e 646c  tomCodeBlobHandl
-00005970: 6528 7365 6c66 2c20 626c 6f62 5f75 7269  e(self, blob_uri
-00005980: 2c20 6973 5f66 756c 6c3d 4661 6c73 6529  , is_full=False)
-00005990: 0a0a 2020 2020 6465 6620 6765 745f 6a73  ..    def get_js
-000059a0: 6f6e 5f62 6c6f 6228 7365 6c66 2c20 626c  on_blob(self, bl
-000059b0: 6f62 5f75 7269 3a20 7374 7229 202d 3e20  ob_uri: str) -> 
-000059c0: 274a 534f 4e42 6c6f 6248 616e 646c 6527  'JSONBlobHandle'
-000059d0: 3a0a 2020 2020 2020 2020 626c 6f62 5f74  :.        blob_t
-000059e0: 7970 6520 3d20 7365 6c66 2e67 6574 5f62  ype = self.get_b
-000059f0: 6c6f 625f 7479 7065 2862 6c6f 625f 7572  lob_type(blob_ur
-00005a00: 6929 0a20 2020 2020 2020 2069 6620 6e6f  i).        if no
-00005a10: 7420 626c 6f62 5f74 7970 655b 2269 735f  t blob_type["is_
-00005a20: 6a73 6f6e 225d 3a0a 2020 2020 2020 2020  json"]:.        
-00005a30: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00005a40: 7272 6f72 2866 2262 6c6f 623a 207b 626c  rror(f"blob: {bl
-00005a50: 6f62 5f75 7269 7d20 6973 206e 6f74 206a  ob_uri} is not j
-00005a60: 736f 6e20 7479 7065 2229 0a20 2020 2020  son type").     
-00005a70: 2020 2072 6574 7572 6e20 4a53 4f4e 426c     return JSONBl
-00005a80: 6f62 4861 6e64 6c65 2873 656c 662c 2062  obHandle(self, b
-00005a90: 6c6f 625f 7572 692c 2069 735f 6675 6c6c  lob_uri, is_full
-00005aa0: 3d46 616c 7365 290a 0a20 2020 2064 6566  =False)..    def
-00005ab0: 2064 7570 6c69 6361 7465 5f64 6167 280a   duplicate_dag(.
-00005ac0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005ad0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00005ae0: 675f 7572 693a 2073 7472 2c0a 2020 2020  g_uri: str,.    
-00005af0: 2020 2020 2020 2020 6465 7374 5f75 7269          dest_uri
-00005b00: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00005b10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00005b20: 2020 2020 636f 7079 5f6e 6f6e 6f77 6e65      copy_nonowne
-00005b30: 645f 626c 6f62 733a 204f 7074 696f 6e61  d_blobs: Optiona
-00005b40: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
-00005b50: 2020 2020 2020 2020 2020 2020 7265 7461              reta
-00005b60: 696e 5f6e 6f6e 6f77 6e65 645f 626c 6f62  in_nonowned_blob
-00005b70: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-00005b80: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
-00005b90: 6e69 6e67 735f 696f 3a20 4f70 7469 6f6e  nings_io: Option
-00005ba0: 616c 5b49 4f5b 416e 795d 5d20 3d20 7379  al[IO[Any]] = sy
-00005bb0: 732e 7374 6465 7272 2920 2d3e 2073 7472  s.stderr) -> str
-00005bc0: 3a0a 2020 2020 2020 2020 6966 2063 6f70  :.        if cop
-00005bd0: 795f 6e6f 6e6f 776e 6564 5f62 6c6f 6273  y_nonowned_blobs
-00005be0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005bf0: 2020 2020 2020 636f 7079 5f6e 6f6e 6f77        copy_nonow
-00005c00: 6e65 645f 626c 6f62 7320 3d20 6e6f 7420  ned_blobs = not 
-00005c10: 7265 7461 696e 5f6e 6f6e 6f77 6e65 645f  retain_nonowned_
-00005c20: 626c 6f62 730a 2020 2020 2020 2020 656c  blobs.        el
-00005c30: 6966 2077 6172 6e69 6e67 735f 696f 2069  if warnings_io i
-00005c40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00005c50: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00005c60: 5f69 6f2e 7772 6974 6528 0a20 2020 2020  _io.write(.     
-00005c70: 2020 2020 2020 2020 2020 2022 636f 7079             "copy
-00005c80: 5f6e 6f6e 6f77 6e65 645f 626c 6f62 7320  _nonowned_blobs 
-00005c90: 6973 2064 6570 7265 6361 7465 643b 2022  is deprecated; "
-00005ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cb0: 2022 7573 6520 7265 7461 696e 5f6e 6f6e   "use retain_non
-00005cc0: 6f77 6e65 645f 626c 6f62 7320 696e 7374  owned_blobs inst
-00005cd0: 6561 645c 6e22 290a 2020 2020 2020 2020  ead\n").        
-00005ce0: 2020 2020 7761 726e 696e 6773 5f69 6f2e      warnings_io.
-00005cf0: 666c 7573 6828 290a 2020 2020 2020 2020  flush().        
-00005d00: 2320 4649 584d 453a 2021 2121 7879 6d65  # FIXME: !!!xyme
-00005d10: 2d62 6163 6b65 6e64 2062 7567 2121 210a  -backend bug!!!.
-00005d20: 2020 2020 2020 2020 636f 7079 5f6e 6f6e          copy_non
-00005d30: 6f77 6e65 645f 626c 6f62 7320 3d20 6e6f  owned_blobs = no
-00005d40: 7420 636f 7079 5f6e 6f6e 6f77 6e65 645f  t copy_nonowned_
-00005d50: 626c 6f62 730a 2020 2020 2020 2020 6172  blobs.        ar
-00005d60: 6773 203d 207b 0a20 2020 2020 2020 2020  gs = {.         
-00005d70: 2020 2022 6461 6722 3a20 6461 675f 7572     "dag": dag_ur
-00005d80: 692c 0a20 2020 2020 2020 2020 2020 2022  i,.            "
-00005d90: 636f 7079 5f6e 6f6e 6f77 6e65 645f 626c  copy_nonowned_bl
-00005da0: 6f62 7322 3a20 636f 7079 5f6e 6f6e 6f77  obs": copy_nonow
-00005db0: 6e65 645f 626c 6f62 732c 0a20 2020 2020  ned_blobs,.     
-00005dc0: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
-00005dd0: 6465 7374 5f75 7269 2069 7320 6e6f 7420  dest_uri is not 
-00005de0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00005df0: 2020 6172 6773 5b22 6465 7374 225d 203d    args["dest"] =
-00005e00: 2064 6573 745f 7572 690a 2020 2020 2020   dest_uri.      
-00005e10: 2020 7265 7475 726e 2063 6173 7428 4461    return cast(Da
-00005e20: 6744 7570 5265 7370 6f6e 7365 2c20 7365  gDupResponse, se
-00005e30: 6c66 2e72 6571 7565 7374 5f6a 736f 6e28  lf.request_json(
-00005e40: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00005e50: 484f 445f 504f 5354 2c20 222f 6461 675f  HOD_POST, "/dag_
-00005e60: 6475 7022 2c20 6172 6773 2929 5b22 6461  dup", args))["da
-00005e70: 6722 5d0a 0a20 2020 2064 6566 2073 6574  g"]..    def set
-00005e80: 5f64 6167 280a 2020 2020 2020 2020 2020  _dag(.          
-00005e90: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00005ea0: 2020 2020 6461 675f 7572 693a 2073 7472      dag_uri: str
-00005eb0: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
-00005ec0: 6673 3a20 4261 7365 4461 6744 6566 2c0a  fs: BaseDagDef,.
-00005ed0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-00005ee0: 696e 6773 5f69 6f3a 204f 7074 696f 6e61  ings_io: Optiona
-00005ef0: 6c5b 494f 5b41 6e79 5d5d 203d 2073 7973  l[IO[Any]] = sys
-00005f00: 2e73 7464 6572 7229 202d 3e20 2744 6167  .stderr) -> 'Dag
-00005f10: 4861 6e64 6c65 273a 0a20 2020 2020 2020  Handle':.       
-00005f20: 2064 6167 5f63 7265 6174 6520 3d20 6361   dag_create = ca
-00005f30: 7374 2844 6167 4372 6561 7465 2c20 7365  st(DagCreate, se
-00005f40: 6c66 2e72 6571 7565 7374 5f6a 736f 6e28  lf.request_json(
-00005f50: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00005f60: 484f 445f 504f 5354 2c20 222f 6461 675f  HOD_POST, "/dag_
-00005f70: 6372 6561 7465 222c 207b 0a20 2020 2020  create", {.     
-00005f80: 2020 2020 2020 2020 2020 2022 6461 6722             "dag"
-00005f90: 3a20 6461 675f 7572 692c 0a20 2020 2020  : dag_uri,.     
-00005fa0: 2020 2020 2020 2020 2020 2022 6465 6673             "defs
-00005fb0: 223a 2064 6566 732c 0a20 2020 2020 2020  ": defs,.       
-00005fc0: 2020 2020 207d 2929 0a20 2020 2020 2020       })).       
-00005fd0: 2064 6167 5f75 7269 203d 2064 6167 5f63   dag_uri = dag_c
-00005fe0: 7265 6174 655b 2264 6167 225d 0a20 2020  reate["dag"].   
-00005ff0: 2020 2020 2069 6620 7761 726e 696e 6773       if warnings
-00006000: 5f69 6f20 6973 206e 6f74 204e 6f6e 653a  _io is not None:
-00006010: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
-00006020: 6e69 6e67 7320 3d20 6461 675f 6372 6561  nings = dag_crea
-00006030: 7465 5b22 7761 726e 696e 6773 225d 0a20  te["warnings"]. 
-00006040: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00006050: 6e28 7761 726e 696e 6773 2920 3e20 313a  n(warnings) > 1:
-00006060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006070: 2077 6172 6e69 6e67 735f 696f 2e77 7269   warnings_io.wri
-00006080: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00006090: 2020 2020 2020 2020 6622 7b6c 656e 2877          f"{len(w
-000060a0: 6172 6e69 6e67 7329 7d20 7761 726e 696e  arnings)} warnin
-000060b0: 6773 2077 6869 6c65 2022 0a20 2020 2020  gs while ".     
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000060d0: 2273 6574 7469 6e67 2064 6167 207b 6461  "setting dag {da
-000060e0: 675f 7572 697d 3a5c 6e22 290a 2020 2020  g_uri}:\n").    
-000060f0: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
-00006100: 2877 6172 6e69 6e67 7329 203d 3d20 313a  (warnings) == 1:
-00006110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006120: 2077 6172 6e69 6e67 735f 696f 2e77 7269   warnings_io.wri
-00006130: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00006140: 2020 2020 2020 2020 6622 5761 726e 696e          f"Warnin
-00006150: 6720 7768 696c 6520 7365 7474 696e 6720  g while setting 
-00006160: 6461 6720 7b64 6167 5f75 7269 7d3a 5c6e  dag {dag_uri}:\n
-00006170: 2229 0a20 2020 2020 2020 2020 2020 2066  ").            f
-00006180: 6f72 2077 6172 6e20 696e 2077 6172 6e69  or warn in warni
-00006190: 6e67 733a 0a20 2020 2020 2020 2020 2020  ngs:.           
-000061a0: 2020 2020 2077 6172 6e69 6e67 735f 696f       warnings_io
-000061b0: 2e77 7269 7465 2866 227b 7761 726e 7d5c  .write(f"{warn}\
-000061c0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-000061d0: 6966 2077 6172 6e69 6e67 733a 0a20 2020  if warnings:.   
-000061e0: 2020 2020 2020 2020 2020 2020 2077 6172               war
-000061f0: 6e69 6e67 735f 696f 2e66 6c75 7368 2829  nings_io.flush()
-00006200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006210: 7365 6c66 2e67 6574 5f64 6167 2864 6167  self.get_dag(dag
-00006220: 5f75 7269 290a 0a20 2020 2064 6566 2073  _uri)..    def s
-00006230: 6574 5f73 6574 7469 6e67 7328 0a20 2020  et_settings(.   
-00006240: 2020 2020 2020 2020 2073 656c 662c 2063           self, c
-00006250: 6f6e 6669 675f 746f 6b65 6e3a 2073 7472  onfig_token: str
-00006260: 2c20 7365 7474 696e 6773 3a20 5365 7474  , settings: Sett
-00006270: 696e 6773 4f62 6a29 202d 3e20 5365 7474  ingsObj) -> Sett
-00006280: 696e 6773 4f62 6a3a 0a20 2020 2020 2020  ingsObj:.       
-00006290: 2072 6574 7572 6e20 6361 7374 284e 616d   return cast(Nam
-000062a0: 6573 7061 6365 5570 6461 7465 5365 7474  espaceUpdateSett
-000062b0: 696e 6773 2c20 7365 6c66 2e72 6571 7565  ings, self.reque
-000062c0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-000062d0: 2020 2020 204d 4554 484f 445f 504f 5354       METHOD_POST
-000062e0: 2c20 222f 7365 7474 696e 6773 222c 207b  , "/settings", {
-000062f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006300: 2022 7365 7474 696e 6773 223a 2073 6574   "settings": set
-00006310: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-00006320: 2020 2020 2020 2022 636f 6e66 6967 5f74         "config_t
-00006330: 6f6b 656e 223a 2063 6f6e 6669 675f 746f  oken": config_to
-00006340: 6b65 6e2c 0a20 2020 2020 2020 2020 2020  ken,.           
-00006350: 207d 2929 5b22 7365 7474 696e 6773 225d   }))["settings"]
-00006360: 0a0a 2020 2020 6465 6620 6765 745f 7365  ..    def get_se
-00006370: 7474 696e 6773 2873 656c 6629 202d 3e20  ttings(self) -> 
-00006380: 5365 7474 696e 6773 4f62 6a3a 0a20 2020  SettingsObj:.   
-00006390: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
-000063a0: 284e 616d 6573 7061 6365 5570 6461 7465  (NamespaceUpdate
-000063b0: 5365 7474 696e 6773 2c20 7365 6c66 2e72  Settings, self.r
-000063c0: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
-000063d0: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-000063e0: 4745 542c 2022 2f73 6574 7469 6e67 7322  GET, "/settings"
-000063f0: 2c20 7b7d 2929 5b22 7365 7474 696e 6773  , {}))["settings
-00006400: 225d 0a0a 2020 2020 6465 6620 6765 745f  "]..    def get_
-00006410: 616c 6c6f 7765 645f 6375 7374 6f6d 5f69  allowed_custom_i
-00006420: 6d70 6f72 7473 2873 656c 6629 202d 3e20  mports(self) -> 
-00006430: 416c 6c6f 7765 6443 7573 746f 6d49 6d70  AllowedCustomImp
-00006440: 6f72 7473 3a0a 2020 2020 2020 2020 7265  orts:.        re
-00006450: 7475 726e 2063 6173 7428 416c 6c6f 7765  turn cast(Allowe
-00006460: 6443 7573 746f 6d49 6d70 6f72 7473 2c20  dCustomImports, 
-00006470: 7365 6c66 2e72 6571 7565 7374 5f6a 736f  self.request_jso
-00006480: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-00006490: 4554 484f 445f 4745 542c 2022 2f61 6c6c  ETHOD_GET, "/all
-000064a0: 6f77 6564 5f63 7573 746f 6d5f 696d 706f  owed_custom_impo
-000064b0: 7274 7322 2c20 7b7d 2c20 6164 645f 6e61  rts", {}, add_na
-000064c0: 6d65 7370 6163 653d 4661 6c73 6529 290a  mespace=False)).
-000064d0: 0a20 2020 2040 6f76 6572 6c6f 6164 0a20  .    @overload. 
-000064e0: 2020 2064 6566 2063 6865 636b 5f71 7565     def check_que
-000064f0: 7565 5f73 7461 7473 2820 2023 2070 796c  ue_stats(  # pyl
-00006500: 696e 743a 2064 6973 6162 6c65 3d6e 6f2d  int: disable=no-
-00006510: 7365 6c66 2d75 7365 0a20 2020 2020 2020  self-use.       
-00006520: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00006530: 2020 2020 2020 2064 6167 3a20 4f70 7469         dag: Opti
-00006540: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
-00006550: 2020 2020 2020 206d 696e 696d 616c 3a20         minimal: 
-00006560: 4c69 7465 7261 6c5b 5472 7565 5d29 202d  Literal[True]) -
-00006570: 3e20 4d69 6e69 6d61 6c51 7565 7565 5374  > MinimalQueueSt
-00006580: 6174 7352 6573 706f 6e73 653a 0a20 2020  atsResponse:.   
-00006590: 2020 2020 202e 2e2e 0a0a 2020 2020 406f       .....    @o
-000065a0: 7665 726c 6f61 640a 2020 2020 6465 6620  verload.    def 
-000065b0: 6368 6563 6b5f 7175 6575 655f 7374 6174  check_queue_stat
-000065c0: 7328 2020 2320 7079 6c69 6e74 3a20 6469  s(  # pylint: di
-000065d0: 7361 626c 653d 6e6f 2d73 656c 662d 7573  sable=no-self-us
-000065e0: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-000065f0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00006600: 6461 673a 204f 7074 696f 6e61 6c5b 7374  dag: Optional[st
-00006610: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
-00006620: 6d69 6e69 6d61 6c3a 204c 6974 6572 616c  minimal: Literal
-00006630: 5b46 616c 7365 5d29 202d 3e20 5175 6575  [False]) -> Queu
-00006640: 6553 7461 7473 5265 7370 6f6e 7365 3a0a  eStatsResponse:.
-00006650: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
-00006660: 2040 6f76 6572 6c6f 6164 0a20 2020 2064   @overload.    d
-00006670: 6566 2063 6865 636b 5f71 7565 7565 5f73  ef check_queue_s
-00006680: 7461 7473 2820 2023 2070 796c 696e 743a  tats(  # pylint:
-00006690: 2064 6973 6162 6c65 3d6e 6f2d 7365 6c66   disable=no-self
-000066a0: 2d75 7365 0a20 2020 2020 2020 2020 2020  -use.           
-000066b0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-000066c0: 2020 2064 6167 3a20 4f70 7469 6f6e 616c     dag: Optional
-000066d0: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
-000066e0: 2020 206d 696e 696d 616c 3a20 626f 6f6c     minimal: bool
-000066f0: 2920 2d3e 2055 6e69 6f6e 5b0a 2020 2020  ) -> Union[.    
-00006700: 2020 2020 2020 2020 2020 2020 4d69 6e69              Mini
-00006710: 6d61 6c51 7565 7565 5374 6174 7352 6573  malQueueStatsRes
-00006720: 706f 6e73 652c 2051 7565 7565 5374 6174  ponse, QueueStat
-00006730: 7352 6573 706f 6e73 655d 3a0a 2020 2020  sResponse]:.    
-00006740: 2020 2020 2e2e 2e0a 0a20 2020 2064 6566      .....    def
-00006750: 2063 6865 636b 5f71 7565 7565 5f73 7461   check_queue_sta
-00006760: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-00006770: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00006780: 2020 6461 673a 204f 7074 696f 6e61 6c5b    dag: Optional[
-00006790: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-000067a0: 2020 2020 2020 2020 206d 696e 696d 616c           minimal
-000067b0: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-000067c0: 2d3e 2055 6e69 6f6e 5b0a 2020 2020 2020  -> Union[.      
-000067d0: 2020 2020 2020 2020 2020 4d69 6e69 6d61            Minima
-000067e0: 6c51 7565 7565 5374 6174 7352 6573 706f  lQueueStatsRespo
-000067f0: 6e73 652c 2051 7565 7565 5374 6174 7352  nse, QueueStatsR
-00006800: 6573 706f 6e73 655d 3a0a 2020 2020 2020  esponse]:.      
-00006810: 2020 6966 206d 696e 696d 616c 3a0a 2020    if minimal:.  
-00006820: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006830: 2063 6173 7428 4d69 6e69 6d61 6c51 7565   cast(MinimalQue
-00006840: 7565 5374 6174 7352 6573 706f 6e73 652c  ueStatsResponse,
-00006850: 2073 656c 662e 7265 7175 6573 745f 6a73   self.request_js
-00006860: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00006870: 2020 2020 4d45 5448 4f44 5f47 4554 2c20      METHOD_GET, 
-00006880: 222f 7175 6575 655f 7374 6174 7322 2c20  "/queue_stats", 
-00006890: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000068a0: 2020 2020 2020 2264 6167 223a 2064 6167        "dag": dag
-000068b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000068c0: 2020 2020 2020 226d 696e 696d 616c 223a        "minimal":
-000068d0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000068e0: 2020 2020 2020 207d 2929 0a20 2020 2020         })).     
-000068f0: 2020 2072 6574 7572 6e20 6361 7374 2851     return cast(Q
-00006900: 7565 7565 5374 6174 7352 6573 706f 6e73  ueueStatsRespons
-00006910: 652c 2073 656c 662e 7265 7175 6573 745f  e, self.request_
-00006920: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
-00006930: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
-00006940: 7175 6575 655f 7374 6174 7322 2c20 7b0a  queue_stats", {.
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2264 6167 223a 2064 6167 2c0a 2020 2020  "dag": dag,.    
-00006970: 2020 2020 2020 2020 2020 2020 226d 696e              "min
-00006980: 696d 616c 223a 2046 616c 7365 2c0a 2020  imal": False,.  
-00006990: 2020 2020 2020 2020 2020 7d29 290a 0a20            })).. 
-000069a0: 2020 2064 6566 2067 6574 5f69 6e73 7461     def get_insta
-000069b0: 6e63 655f 7374 6174 7573 280a 2020 2020  nce_status(.    
-000069c0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000069d0: 2020 2020 2020 2020 2020 6461 675f 7572            dag_ur
-000069e0: 693a 204f 7074 696f 6e61 6c5b 7374 725d  i: Optional[str]
-000069f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00006a00: 2020 2020 206e 6f64 655f 6964 3a20 4f70       node_id: Op
-00006a10: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00006a20: 6e65 2920 2d3e 2044 6963 745b 496e 7374  ne) -> Dict[Inst
-00006a30: 616e 6365 5374 6174 7573 2c20 696e 745d  anceStatus, int]
-00006a40: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00006a50: 2063 6173 7428 4469 6374 5b49 6e73 7461   cast(Dict[Insta
-00006a60: 6e63 6553 7461 7475 732c 2069 6e74 5d2c  nceStatus, int],
-00006a70: 2073 656c 662e 7265 7175 6573 745f 6a73   self.request_js
-00006a80: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00006a90: 4d45 5448 4f44 5f47 4554 2c20 222f 696e  METHOD_GET, "/in
-00006aa0: 7374 616e 6365 5f73 7461 7475 7322 2c20  stance_status", 
-00006ab0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00006ac0: 2020 2264 6167 223a 2064 6167 5f75 7269    "dag": dag_uri
-00006ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006ae0: 2020 226e 6f64 6522 3a20 6e6f 6465 5f69    "node": node_i
-00006af0: 642c 0a20 2020 2020 2020 2020 2020 207d  d,.            }
-00006b00: 2929 0a0a 2020 2020 6465 6620 6765 745f  ))..    def get_
-00006b10: 7175 6575 655f 6d6f 6465 2873 656c 6629  queue_mode(self)
-00006b20: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00006b30: 2072 6574 7572 6e20 6361 7374 2851 7565   return cast(Que
-00006b40: 7565 4d6f 6465 2c20 7365 6c66 2e72 6571  ueMode, self.req
-00006b50: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-00006b60: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
-00006b70: 542c 2022 2f71 7565 7565 5f6d 6f64 6522  T, "/queue_mode"
-00006b80: 2c20 7b7d 2c20 6164 645f 6e61 6d65 7370  , {}, add_namesp
-00006b90: 6163 653d 4661 6c73 6529 295b 226d 6f64  ace=False))["mod
-00006ba0: 6522 5d0a 0a20 2020 2064 6566 2073 6574  e"]..    def set
-00006bb0: 5f71 7565 7565 5f6d 6f64 6528 7365 6c66  _queue_mode(self
-00006bc0: 2c20 6d6f 6465 3a20 7374 7229 202d 3e20  , mode: str) -> 
-00006bd0: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
-00006be0: 7572 6e20 6361 7374 2851 7565 7565 4d6f  urn cast(QueueMo
-00006bf0: 6465 2c20 7365 6c66 2e72 6571 7565 7374  de, self.request
-00006c00: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
-00006c10: 2020 204d 4554 484f 445f 5055 542c 2022     METHOD_PUT, "
-00006c20: 2f71 7565 7565 5f6d 6f64 6522 2c20 7b0a  /queue_mode", {.
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 226d 6f64 6522 3a20 6d6f 6465 2c0a 2020  "mode": mode,.  
-00006c50: 2020 2020 2020 2020 2020 7d2c 2061 6464            }, add
-00006c60: 5f6e 616d 6573 7061 6365 3d46 616c 7365  _namespace=False
-00006c70: 2929 5b22 6d6f 6465 225d 0a0a 2020 2020  ))["mode"]..    
-00006c80: 6465 6620 666c 7573 685f 616c 6c5f 7175  def flush_all_qu
-00006c90: 6575 655f 6461 7461 2873 656c 6629 202d  eue_data(self) -
-00006ca0: 3e20 4e6f 6e65 3a0a 0a20 2020 2020 2020  > None:..       
-00006cb0: 2064 6566 2064 6f5f 666c 7573 6828 2920   def do_flush() 
-00006cc0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00006cd0: 2020 2020 2072 6573 203d 2063 6173 7428       res = cast(
-00006ce0: 466c 7573 6841 6c6c 5175 6575 6573 5265  FlushAllQueuesRe
-00006cf0: 7370 6f6e 7365 2c20 7365 6c66 2e72 6571  sponse, self.req
-00006d00: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-00006d10: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
-00006d20: 445f 504f 5354 2c20 222f 666c 7573 685f  D_POST, "/flush_
-00006d30: 616c 6c5f 7175 6575 6573 222c 207b 7d2c  all_queues", {},
-00006d40: 2061 6464 5f6e 616d 6573 7061 6365 3d46   add_namespace=F
-00006d50: 616c 7365 2929 0a20 2020 2020 2020 2020  alse)).         
-00006d60: 2020 2072 6574 7572 6e20 626f 6f6c 2872     return bool(r
-00006d70: 6573 5b22 7375 6363 6573 7322 5d29 0a0a  es["success"])..
-00006d80: 2020 2020 2020 2020 7768 696c 6520 646f          while do
-00006d90: 5f66 6c75 7368 2829 3a20 2023 2077 6520  _flush():  # we 
-00006da0: 666c 7573 6820 756e 7469 6c20 7468 6572  flush until ther
-00006db0: 6520 6973 206e 6f74 6869 6e67 2074 6f20  e is nothing to 
-00006dc0: 666c 7573 6820 616e 796d 6f72 650a 2020  flush anymore.  
-00006dd0: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00006de0: 6c65 6570 2831 2e30 290a 0a20 2020 2064  leep(1.0)..    d
-00006df0: 6566 2067 6574 5f63 6163 6865 5f73 7461  ef get_cache_sta
-00006e00: 7473 2873 656c 6629 202d 3e20 4361 6368  ts(self) -> Cach
-00006e10: 6553 7461 7473 3a0a 2020 2020 2020 2020  eStats:.        
-00006e20: 7265 7475 726e 2063 6173 7428 4361 6368  return cast(Cach
-00006e30: 6553 7461 7473 2c20 7365 6c66 2e72 6571  eStats, self.req
-00006e40: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-00006e50: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
-00006e60: 542c 2022 2f63 6163 6865 5f73 7461 7473  T, "/cache_stats
-00006e70: 222c 207b 7d2c 2061 6464 5f6e 616d 6573  ", {}, add_names
-00006e80: 7061 6365 3d46 616c 7365 2929 0a0a 2020  pace=False))..  
-00006e90: 2020 6465 6620 7265 7365 745f 6361 6368    def reset_cach
-00006ea0: 6528 7365 6c66 2920 2d3e 2043 6163 6865  e(self) -> Cache
-00006eb0: 5374 6174 733a 0a20 2020 2020 2020 2072  Stats:.        r
-00006ec0: 6574 7572 6e20 6361 7374 2843 6163 6865  eturn cast(Cache
-00006ed0: 5374 6174 732c 2073 656c 662e 7265 7175  Stats, self.requ
-00006ee0: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-00006ef0: 2020 2020 2020 4d45 5448 4f44 5f50 4f53        METHOD_POS
-00006f00: 542c 2022 2f63 6163 6865 5f72 6573 6574  T, "/cache_reset
-00006f10: 222c 207b 7d2c 2061 6464 5f6e 616d 6573  ", {}, add_names
-00006f20: 7061 6365 3d46 616c 7365 2929 0a0a 2020  pace=False))..  
-00006f30: 2020 6465 6620 6372 6561 7465 5f6b 6166    def create_kaf
-00006f40: 6b61 5f65 7272 6f72 5f74 6f70 6963 2873  ka_error_topic(s
-00006f50: 656c 6629 202d 3e20 4b61 666b 6154 6f70  elf) -> KafkaTop
-00006f60: 6963 733a 0a20 2020 2020 2020 2072 6574  ics:.        ret
-00006f70: 7572 6e20 6361 7374 284b 6166 6b61 546f  urn cast(KafkaTo
-00006f80: 7069 6373 2c20 7365 6c66 2e72 6571 7565  pics, self.reque
-00006f90: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-00006fa0: 2020 2020 204d 4554 484f 445f 504f 5354       METHOD_POST
-00006fb0: 2c20 222f 6b61 666b 615f 746f 7069 6373  , "/kafka_topics
-00006fc0: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
-00006fd0: 2020 2020 2022 6e75 6d5f 7061 7274 6974       "num_partit
-00006fe0: 696f 6e73 223a 2031 2c0a 2020 2020 2020  ions": 1,.      
-00006ff0: 2020 2020 2020 7d29 290a 0a20 2020 2064        }))..    d
-00007000: 6566 2067 6574 5f6b 6166 6b61 5f65 7272  ef get_kafka_err
-00007010: 6f72 5f74 6f70 6963 2873 656c 6629 202d  or_topic(self) -
-00007020: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
-00007030: 6573 203d 2063 6173 7428 4b61 666b 6154  es = cast(KafkaT
-00007040: 6f70 6963 4e61 6d65 732c 2073 656c 662e  opicNames, self.
-00007050: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
-00007060: 2020 2020 2020 2020 2020 4d45 5448 4f44            METHOD
-00007070: 5f47 4554 2c20 222f 6b61 666b 615f 746f  _GET, "/kafka_to
-00007080: 7069 635f 6e61 6d65 7322 2c20 7b7d 2929  pic_names", {}))
-00007090: 5b22 6572 726f 7222 5d0a 2020 2020 2020  ["error"].      
-000070a0: 2020 6173 7365 7274 2072 6573 2069 7320    assert res is 
-000070b0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-000070c0: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
-000070d0: 2064 6566 2064 656c 6574 655f 6b61 666b   def delete_kafk
-000070e0: 615f 6572 726f 725f 746f 7069 6328 7365  a_error_topic(se
-000070f0: 6c66 2920 2d3e 204b 6166 6b61 546f 7069  lf) -> KafkaTopi
-00007100: 6373 3a0a 2020 2020 2020 2020 7265 7475  cs:.        retu
-00007110: 726e 2063 6173 7428 4b61 666b 6154 6f70  rn cast(KafkaTop
-00007120: 6963 732c 2073 656c 662e 7265 7175 6573  ics, self.reques
-00007130: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
-00007140: 2020 2020 4d45 5448 4f44 5f50 4f53 542c      METHOD_POST,
-00007150: 2022 2f6b 6166 6b61 5f74 6f70 6963 7322   "/kafka_topics"
-00007160: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
-00007170: 2020 2020 226e 756d 5f70 6172 7469 7469      "num_partiti
-00007180: 6f6e 7322 3a20 302c 0a20 2020 2020 2020  ons": 0,.       
-00007190: 2020 2020 207d 2929 0a0a 2020 2020 6465       }))..    de
-000071a0: 6620 7265 6164 5f6b 6166 6b61 5f65 7272  f read_kafka_err
-000071b0: 6f72 7328 7365 6c66 2c20 6f66 6673 6574  ors(self, offset
-000071c0: 3a20 7374 7220 3d20 2263 7572 7265 6e74  : str = "current
-000071d0: 2229 202d 3e20 4c69 7374 5b73 7472 5d3a  ") -> List[str]:
-000071e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000071f0: 6361 7374 284c 6973 745b 7374 725d 2c20  cast(List[str], 
-00007200: 7365 6c66 2e72 6571 7565 7374 5f6a 736f  self.request_jso
-00007210: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-00007220: 4554 484f 445f 4745 542c 2022 2f6b 6166  ETHOD_GET, "/kaf
-00007230: 6b61 5f6d 7367 222c 207b 0a20 2020 2020  ka_msg", {.     
-00007240: 2020 2020 2020 2020 2020 2022 6f66 6673             "offs
-00007250: 6574 223a 206f 6666 7365 742c 0a20 2020  et": offset,.   
-00007260: 2020 2020 2020 2020 207d 2929 0a0a 2020           }))..  
-00007270: 2020 6465 6620 6765 745f 6e61 6d65 645f    def get_named_
-00007280: 7365 6372 6574 7328 0a20 2020 2020 2020  secrets(.       
-00007290: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000072a0: 2020 2020 2020 2063 6f6e 6669 675f 746f         config_to
-000072b0: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-000072c0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-000072d0: 2020 2020 2020 2073 686f 775f 7661 6c75         show_valu
-000072e0: 6573 3a20 626f 6f6c 203d 2046 616c 7365  es: bool = False
-000072f0: 2920 2d3e 2044 6963 745b 7374 722c 204f  ) -> Dict[str, O
-00007300: 7074 696f 6e61 6c5b 7374 725d 5d3a 0a20  ptional[str]]:. 
-00007310: 2020 2020 2020 2069 6620 7368 6f77 5f76         if show_v
-00007320: 616c 7565 7320 616e 6420 636f 6e66 6967  alues and config
-00007330: 5f74 6f6b 656e 2069 7320 4e6f 6e65 3a0a  _token is None:.
-00007340: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00007350: 6520 5661 6c75 6545 7272 6f72 2822 636f  e ValueError("co
-00007360: 6e66 6967 5f74 6f6b 656e 206d 7573 7420  nfig_token must 
-00007370: 6265 2073 6574 2074 6f20 7368 6f77 5f76  be set to show_v
-00007380: 616c 7565 7322 290a 2020 2020 2020 2020  alues").        
-00007390: 7265 7475 726e 2063 6173 7428 4469 6374  return cast(Dict
-000073a0: 5b73 7472 2c20 4f70 7469 6f6e 616c 5b73  [str, Optional[s
-000073b0: 7472 5d5d 2c20 7365 6c66 2e72 6571 7565  tr]], self.reque
-000073c0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-000073d0: 2020 2020 204d 4554 484f 445f 4745 542c       METHOD_GET,
-000073e0: 2022 2f6e 616d 6564 5f73 6563 7265 7473   "/named_secrets
-000073f0: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
-00007400: 2020 2020 2022 7368 6f77 223a 2069 6e74       "show": int
-00007410: 2862 6f6f 6c28 7368 6f77 5f76 616c 7565  (bool(show_value
-00007420: 7329 292c 0a20 2020 2020 2020 2020 2020  s)),.           
-00007430: 2020 2020 2022 636f 6e66 6967 5f74 6f6b       "config_tok
-00007440: 656e 223a 2063 6f6e 6669 675f 746f 6b65  en": config_toke
-00007450: 6e2c 0a20 2020 2020 2020 2020 2020 207d  n,.            }
-00007460: 2929 0a0a 2020 2020 6465 6620 7365 745f  ))..    def set_
-00007470: 6e61 6d65 645f 7365 6372 6574 280a 2020  named_secret(.  
-00007480: 2020 2020 2020 2020 2020 7365 6c66 2c20            self, 
-00007490: 636f 6e66 6967 5f74 6f6b 656e 3a20 7374  config_token: st
-000074a0: 722c 206b 6579 3a20 7374 722c 2076 616c  r, key: str, val
-000074b0: 7565 3a20 7374 7229 202d 3e20 626f 6f6c  ue: str) -> bool
-000074c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000074d0: 2063 6173 7428 5365 744e 616d 6564 5365   cast(SetNamedSe
-000074e0: 6372 6574 2c20 7365 6c66 2e72 6571 7565  cret, self.reque
-000074f0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-00007500: 2020 2020 204d 4554 484f 445f 5055 542c       METHOD_PUT,
-00007510: 2022 2f6e 616d 6564 5f73 6563 7265 7473   "/named_secrets
-00007520: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
-00007530: 2020 2020 2022 6b65 7922 3a20 6b65 792c       "key": key,
-00007540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007550: 2022 7661 6c75 6522 3a20 7661 6c75 652c   "value": value,
-00007560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007570: 2022 636f 6e66 6967 5f74 6f6b 656e 223a   "config_token":
-00007580: 2063 6f6e 6669 675f 746f 6b65 6e2c 0a20   config_token,. 
-00007590: 2020 2020 2020 2020 2020 207d 2929 5b22             }))["
-000075a0: 7265 706c 6163 6564 225d 0a0a 2020 2020  replaced"]..    
-000075b0: 6465 6620 6765 745f 6572 726f 725f 6c6f  def get_error_lo
-000075c0: 6773 2873 656c 6629 202d 3e20 7374 723a  gs(self) -> str:
-000075d0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000075e0: 6c66 2e5f 7261 775f 7265 7175 6573 745f  lf._raw_request_
-000075f0: 7374 7228 4d45 5448 4f44 5f47 4554 2c20  str(METHOD_GET, 
-00007600: 222f 6572 726f 725f 6c6f 6773 222c 207b  "/error_logs", {
-00007610: 7d29 2061 7320 6669 6e3a 0a20 2020 2020  }) as fin:.     
-00007620: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00007630: 6e2e 7265 6164 2829 0a0a 2020 2020 6465  n.read()..    de
-00007640: 6620 6765 745f 6b6e 6f77 6e5f 626c 6f62  f get_known_blob
-00007650: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
-00007660: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00007670: 2062 6c6f 625f 7479 7065 3a20 4f70 7469   blob_type: Opti
-00007680: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00007690: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
-000076a0: 6e6e 6563 746f 723a 204f 7074 696f 6e61  nnector: Optiona
-000076b0: 6c5b 7374 725d 203d 204e 6f6e 6529 202d  l[str] = None) -
-000076c0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-000076d0: 2020 2020 2072 6574 7572 6e20 5b0a 2020       return [.  
-000076e0: 2020 2020 2020 2020 2020 7265 735b 305d            res[0]
-000076f0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00007700: 2072 6573 2069 6e20 7365 6c66 2e67 6574   res in self.get
-00007710: 5f6b 6e6f 776e 5f62 6c6f 625f 7469 6d65  _known_blob_time
-00007720: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00007730: 2020 2072 6574 7269 6576 655f 7469 6d65     retrieve_time
-00007740: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-00007750: 2020 2020 2020 2020 2062 6c6f 625f 7479           blob_ty
-00007760: 7065 3d62 6c6f 625f 7479 7065 2c0a 2020  pe=blob_type,.  
-00007770: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00007780: 6e6e 6563 746f 723d 636f 6e6e 6563 746f  nnector=connecto
-00007790: 7229 5b31 5d0a 2020 2020 2020 2020 5d0a  r)[1].        ].
-000077a0: 0a20 2020 2064 6566 2067 6574 5f6b 6e6f  .    def get_kno
-000077b0: 776e 5f62 6c6f 625f 6167 6573 280a 2020  wn_blob_ages(.  
-000077c0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-000077d0: 2020 2020 2020 2020 2020 2020 626c 6f62              blob
-000077e0: 5f74 7970 653a 204f 7074 696f 6e61 6c5b  _type: Optional[
-000077f0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00007800: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
-00007810: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
-00007820: 5d20 3d20 4e6f 6e65 2920 2d3e 204c 6973  ] = None) -> Lis
-00007830: 745b 5475 706c 655b 7374 722c 2073 7472  t[Tuple[str, str
-00007840: 5d5d 3a0a 2020 2020 2020 2020 6375 725f  ]]:.        cur_
-00007850: 7469 6d65 2c20 626c 6f62 7320 3d20 7365  time, blobs = se
-00007860: 6c66 2e67 6574 5f6b 6e6f 776e 5f62 6c6f  lf.get_known_blo
-00007870: 625f 7469 6d65 7328 0a20 2020 2020 2020  b_times(.       
-00007880: 2020 2020 2072 6574 7269 6576 655f 7469       retrieve_ti
-00007890: 6d65 733d 5472 7565 2c20 626c 6f62 5f74  mes=True, blob_t
-000078a0: 7970 653d 626c 6f62 5f74 7970 652c 2063  ype=blob_type, c
-000078b0: 6f6e 6e65 6374 6f72 3d63 6f6e 6e65 6374  onnector=connect
-000078c0: 6f72 290a 2020 2020 2020 2020 7265 7475  or).        retu
-000078d0: 726e 205b 0a20 2020 2020 2020 2020 2020  rn [.           
-000078e0: 2028 626c 6f62 5f69 642c 2067 6574 5f61   (blob_id, get_a
-000078f0: 6765 2863 7572 5f74 696d 652c 2062 6c6f  ge(cur_time, blo
-00007900: 625f 7469 6d65 2929 0a20 2020 2020 2020  b_time)).       
-00007910: 2020 2020 2066 6f72 2028 626c 6f62 5f69       for (blob_i
-00007920: 642c 2062 6c6f 625f 7469 6d65 2920 696e  d, blob_time) in
-00007930: 2073 6f72 7465 6428 626c 6f62 732c 206b   sorted(blobs, k
-00007940: 6579 3d6c 616d 6264 6120 656c 3a20 280a  ey=lambda el: (.
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 7361 6665 5f6f 7074 5f6e 756d 2865 6c5b  safe_opt_num(el[
-00007970: 315d 292c 2065 6c5b 305d 2929 0a20 2020  1]), el[0])).   
-00007980: 2020 2020 205d 0a0a 2020 2020 6465 6620       ]..    def 
-00007990: 6765 745f 6b6e 6f77 6e5f 626c 6f62 5f74  get_known_blob_t
-000079a0: 696d 6573 280a 2020 2020 2020 2020 2020  imes(.          
-000079b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000079c0: 2020 2020 7265 7472 6965 7665 5f74 696d      retrieve_tim
-000079d0: 6573 3a20 626f 6f6c 2c0a 2020 2020 2020  es: bool,.      
-000079e0: 2020 2020 2020 626c 6f62 5f74 7970 653a        blob_type:
-000079f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00007a00: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00007a10: 2020 2063 6f6e 6e65 6374 6f72 3a20 4f70     connector: Op
-00007a20: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00007a30: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00007a40: 2920 2d3e 2054 7570 6c65 5b66 6c6f 6174  ) -> Tuple[float
-00007a50: 2c20 4c69 7374 5b54 7570 6c65 5b73 7472  , List[Tuple[str
-00007a60: 2c20 4f70 7469 6f6e 616c 5b66 6c6f 6174  , Optional[float
-00007a70: 5d5d 5d5d 3a0a 2020 2020 2020 2020 6f62  ]]]]:.        ob
-00007a80: 6a3a 2044 6963 745b 7374 722c 2055 6e69  j: Dict[str, Uni
-00007a90: 6f6e 5b69 6e74 2c20 7374 725d 5d20 3d20  on[int, str]] = 
-00007aa0: 7b0a 2020 2020 2020 2020 2020 2020 2272  {.            "r
-00007ab0: 6574 7269 6576 655f 7469 6d65 7322 3a20  etrieve_times": 
-00007ac0: 696e 7428 7265 7472 6965 7665 5f74 696d  int(retrieve_tim
-00007ad0: 6573 292c 0a20 2020 2020 2020 207d 0a20  es),.        }. 
-00007ae0: 2020 2020 2020 2069 6620 626c 6f62 5f74         if blob_t
-00007af0: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-00007b00: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
-00007b10: 5b22 626c 6f62 5f74 7970 6522 5d20 3d20  ["blob_type"] = 
-00007b20: 626c 6f62 5f74 7970 650a 2020 2020 2020  blob_type.      
-00007b30: 2020 6966 2063 6f6e 6e65 6374 6f72 2069    if connector i
-00007b40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00007b50: 2020 2020 2020 2020 6f62 6a5b 2263 6f6e          obj["con
-00007b60: 6e65 6374 6f72 225d 203d 2063 6f6e 6e65  nector"] = conne
-00007b70: 6374 6f72 0a20 2020 2020 2020 2072 6573  ctor.        res
-00007b80: 203d 2063 6173 7428 4b6e 6f77 6e42 6c6f   = cast(KnownBlo
-00007b90: 6273 2c20 7365 6c66 2e72 6571 7565 7374  bs, self.request
-00007ba0: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
-00007bb0: 2020 204d 4554 484f 445f 4745 542c 2022     METHOD_GET, "
-00007bc0: 2f6b 6e6f 776e 5f62 6c6f 6273 222c 206f  /known_blobs", o
-00007bd0: 626a 2929 0a20 2020 2020 2020 2072 6574  bj)).        ret
-00007be0: 7572 6e20 7265 735b 2263 7572 5f74 696d  urn res["cur_tim
-00007bf0: 6522 5d2c 2072 6573 5b22 626c 6f62 7322  e"], res["blobs"
-00007c00: 5d0a 0a20 2020 2064 6566 2067 6574 5f74  ]..    def get_t
-00007c10: 7269 746f 6e5f 6d6f 6465 6c73 2873 656c  riton_models(sel
-00007c20: 6629 202d 3e20 4c69 7374 5b73 7472 5d3a  f) -> List[str]:
-00007c30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007c40: 6361 7374 2854 7269 746f 6e4d 6f64 656c  cast(TritonModel
-00007c50: 7352 6573 706f 6e73 652c 2073 656c 662e  sResponse, self.
-00007c60: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
-00007c70: 2020 2020 2020 2020 2020 4d45 5448 4f44            METHOD
-00007c80: 5f47 4554 2c20 222f 696e 6665 7265 6e63  _GET, "/inferenc
-00007c90: 655f 6d6f 6465 6c73 222c 207b 7d29 295b  e_models", {}))[
-00007ca0: 226d 6f64 656c 7322 5d0a 0a20 2020 2040  "models"]..    @
-00007cb0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-00007cc0: 2064 6566 2072 6561 645f 6476 6328 0a20   def read_dvc(. 
-00007cd0: 2020 2020 2020 2020 2020 2070 6174 683a             path:
-00007ce0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00007cf0: 2020 7265 706f 3a20 7374 722c 0a20 2020    repo: str,.   
-00007d00: 2020 2020 2020 2020 2072 6576 3a20 4f70           rev: Op
-00007d10: 7469 6f6e 616c 5b73 7472 5d20 3d20 2248  tional[str] = "H
-00007d20: 4541 4422 2c0a 2020 2020 2020 2020 2020  EAD",.          
-00007d30: 2020 7761 726e 696e 6773 5f69 6f3a 204f    warnings_io: O
-00007d40: 7074 696f 6e61 6c5b 494f 5b41 6e79 5d5d  ptional[IO[Any]]
-00007d50: 203d 2073 7973 2e73 7464 6572 7229 202d   = sys.stderr) -
-00007d60: 3e20 416e 793a 0a20 2020 2020 2020 2022  > Any:.        "
-00007d70: 2222 5265 6164 696e 6720 6476 6320 6669  ""Reading dvc fi
-00007d80: 6c65 2063 6f6e 7465 6e74 2066 726f 6d20  le content from 
-00007d90: 6769 7420 7472 6163 6b65 6420 4456 4320  git tracked DVC 
-00007da0: 7072 6f6a 6563 742e 0a0a 2020 2020 2020  project...      
-00007db0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00007dc0: 2020 2020 7061 7468 2028 7374 7229 3a0a      path (str):.
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 4669 6c65 2070 6174 6820 746f 2072 6561  File path to rea
-00007df0: 642c 2072 656c 6174 6976 6520 746f 2074  d, relative to t
-00007e00: 6865 2072 6f6f 7420 6f66 2074 6865 2072  he root of the r
-00007e10: 6570 6f2e 0a20 2020 2020 2020 2020 2020  epo..           
-00007e20: 2072 6570 6f20 2873 7472 293a 0a20 2020   repo (str):.   
-00007e30: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-00007e40: 6369 6669 6573 2074 6865 206c 6f63 6174  cifies the locat
-00007e50: 696f 6e20 6f66 2074 6865 2044 5643 2070  ion of the DVC p
-00007e60: 726f 6a65 6374 2e20 4974 2063 616e 2062  roject. It can b
-00007e70: 6520 610a 2020 2020 2020 2020 2020 2020  e a.            
-00007e80: 2020 2020 6769 7468 7562 2055 524c 206f      github URL o
-00007e90: 7220 6120 6669 6c65 2073 7973 7465 6d20  r a file system 
-00007ea0: 7061 7468 2e0a 2020 2020 2020 2020 2020  path..          
-00007eb0: 2020 7265 7620 2873 7472 293a 0a20 2020    rev (str):.   
-00007ec0: 2020 2020 2020 2020 2020 2020 2047 6974               Git
-00007ed0: 2063 6f6d 6d69 7420 2861 6e79 2072 6576   commit (any rev
-00007ee0: 6973 696f 6e20 7375 6368 2061 7320 6120  ision such as a 
-00007ef0: 6272 616e 6368 206f 7220 7461 6720 6e61  branch or tag na
-00007f00: 6d65 2c20 6f72 2061 0a20 2020 2020 2020  me, or a.       
-00007f10: 2020 2020 2020 2020 2063 6f6d 6d69 7420           commit 
-00007f20: 6861 7368 292e 2049 6620 7265 706f 2069  hash). If repo i
-00007f30: 7320 6e6f 7420 6120 4769 7420 7265 706f  s not a Git repo
-00007f40: 2c20 7468 6973 206f 7074 696f 6e20 6973  , this option is
-00007f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007f60: 2069 676e 6f72 6564 2e20 4465 6661 756c   ignored. Defaul
-00007f70: 743a 2048 4541 442e 0a20 2020 2020 2020  t: HEAD..       
-00007f80: 2020 2020 2077 6172 6e69 6e67 735f 696f       warnings_io
-00007f90: 2028 6f70 7469 6f6e 616c 2049 4f29 3a0a   (optional IO):.
-00007fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fb0: 494f 2073 7472 6561 6d20 7768 6572 6520  IO stream where 
-00007fc0: 7468 6520 7761 726e 696e 6720 7769 6c6c  the warning will
-00007fd0: 2062 6520 7072 696e 7465 6420 746f 0a0a   be printed to..
-00007fe0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00007ff0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-00008000: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
-00008010: 6669 6c65 2e0a 2020 2020 2020 2020 2222  file..        ""
-00008020: 220a 2020 2020 2020 2020 6672 6f6d 202e  ".        from .
-00008030: 7574 696c 2069 6d70 6f72 7420 6861 735f  util import has_
-00008040: 6476 630a 0a20 2020 2020 2020 2069 6620  dvc..        if 
-00008050: 6e6f 7420 6861 735f 6476 6328 293a 0a20  not has_dvc():. 
-00008060: 2020 2020 2020 2020 2020 2069 6620 7761             if wa
-00008070: 726e 696e 6773 5f69 6f20 6973 206e 6f74  rnings_io is not
-00008080: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008090: 2020 2020 2020 2077 6172 6e69 6e67 735f         warnings_
-000080a0: 696f 2e77 7269 7465 280a 2020 2020 2020  io.write(.      
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2250                "P
-000080c0: 6c65 6173 6520 696e 7374 616c 6c20 6476  lease install dv
-000080d0: 6320 6874 7470 733a 2f2f 6476 632e 6f72  c https://dvc.or
-000080e0: 672f 646f 632f 696e 7374 616c 6c22 290a  g/doc/install").
-000080f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008100: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-00008110: 2069 6d70 6f72 7420 6476 632e 6170 690a   import dvc.api.
-00008120: 0a20 2020 2020 2020 2072 6573 203d 2064  .        res = d
-00008130: 7663 2e61 7069 2e72 6561 6428 7061 7468  vc.api.read(path
-00008140: 2c20 7265 706f 3d72 6570 6f2c 2072 6576  , repo=repo, rev
-00008150: 3d72 6576 2c20 6d6f 6465 3d22 7222 290a  =rev, mode="r").
-00008160: 2020 2020 2020 2020 6d61 7962 655f 7061          maybe_pa
-00008170: 7273 6520 3d20 6d61 7962 655f 6a73 6f6e  rse = maybe_json
-00008180: 5f6c 6f61 6473 2872 6573 290a 2020 2020  _loads(res).    
-00008190: 2020 2020 6966 206d 6179 6265 5f70 6172      if maybe_par
-000081a0: 7365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  se is not None:.
-000081b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000081c0: 726e 206d 6179 6265 5f70 6172 7365 0a20  rn maybe_parse. 
-000081d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000081e0: 730a 0a20 2020 2040 7374 6174 6963 6d65  s..    @staticme
-000081f0: 7468 6f64 0a20 2020 2064 6566 2067 6574  thod.    def get
-00008200: 5f65 6e76 5f73 7472 286b 6579 3a20 7374  _env_str(key: st
-00008210: 722c 2064 6566 6175 6c74 3a20 4f70 7469  r, default: Opti
-00008220: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00008230: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00008240: 2020 7265 7320 3d20 6f73 2e67 6574 656e    res = os.geten
-00008250: 7628 6b65 792c 2064 6566 6175 6c74 3d64  v(key, default=d
-00008260: 6566 6175 6c74 290a 2020 2020 2020 2020  efault).        
-00008270: 6966 2072 6573 2069 7320 4e6f 6e65 3a0a  if res is None:.
-00008280: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008290: 6520 5661 6c75 6545 7272 6f72 2866 2265  e ValueError(f"e
-000082a0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000082b0: 626c 6520 7b6b 6579 7d20 6973 206e 6f74  ble {key} is not
-000082c0: 2073 6574 2229 0a20 2020 2020 2020 2072   set").        r
-000082d0: 6574 7572 6e20 6622 7b72 6573 7d22 0a0a  eturn f"{res}"..
-000082e0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-000082f0: 640a 2020 2020 6465 6620 6765 745f 656e  d.    def get_en
-00008300: 765f 696e 7428 6b65 793a 2073 7472 2c20  v_int(key: str, 
-00008310: 6465 6661 756c 743a 204f 7074 696f 6e61  default: Optiona
-00008320: 6c5b 696e 745d 203d 204e 6f6e 6529 202d  l[int] = None) -
-00008330: 3e20 696e 743a 0a20 2020 2020 2020 2072  > int:.        r
-00008340: 6573 203d 206f 732e 6765 7465 6e76 286b  es = os.getenv(k
-00008350: 6579 2c20 6465 6661 756c 743d 6465 6661  ey, default=defa
-00008360: 756c 7429 0a20 2020 2020 2020 2069 6620  ult).        if 
-00008370: 7265 7320 6973 204e 6f6e 653a 0a20 2020  res is None:.   
-00008380: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00008390: 616c 7565 4572 726f 7228 6622 656e 7669  alueError(f"envi
-000083a0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-000083b0: 207b 6b65 797d 2069 7320 6e6f 7420 7365   {key} is not se
-000083c0: 7422 290a 2020 2020 2020 2020 7265 7475  t").        retu
-000083d0: 726e 2069 6e74 2872 6573 290a 0a20 2020  rn int(res)..   
-000083e0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-000083f0: 2020 2064 6566 2067 6574 5f65 6e76 5f62     def get_env_b
-00008400: 6f6f 6c28 6b65 793a 2073 7472 2c20 6465  ool(key: str, de
-00008410: 6661 756c 743a 204f 7074 696f 6e61 6c5b  fault: Optional[
-00008420: 626f 6f6c 5d20 3d20 4e6f 6e65 2920 2d3e  bool] = None) ->
-00008430: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
-00008440: 6573 203d 206f 732e 6765 7465 6e76 286b  es = os.getenv(k
-00008450: 6579 2c20 6465 6661 756c 743d 6465 6661  ey, default=defa
-00008460: 756c 7429 0a20 2020 2020 2020 2069 6620  ult).        if 
-00008470: 7265 7320 6973 204e 6f6e 653a 0a20 2020  res is None:.   
-00008480: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00008490: 616c 7565 4572 726f 7228 6622 656e 7669  alueError(f"envi
-000084a0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-000084b0: 207b 6b65 797d 2069 7320 6e6f 7420 7365   {key} is not se
-000084c0: 7422 290a 2020 2020 2020 2020 7265 7475  t").        retu
-000084d0: 726e 2074 6f5f 626f 6f6c 2872 6573 290a  rn to_bool(res).
-000084e0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-000084f0: 6f64 0a20 2020 2064 6566 206c 6f61 645f  od.    def load_
-00008500: 6a73 6f6e 286a 736f 6e5f 7061 7468 3a20  json(json_path: 
-00008510: 7374 7229 202d 3e20 4469 6374 5b73 7472  str) -> Dict[str
-00008520: 2c20 416e 795d 3a0a 2020 2020 2020 2020  , Any]:.        
-00008530: 7769 7468 206f 7065 6e28 6a73 6f6e 5f70  with open(json_p
-00008540: 6174 682c 2022 7222 2920 6173 2066 696e  ath, "r") as fin
-00008550: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00008560: 7475 726e 206a 736f 6e2e 6c6f 6164 2866  turn json.load(f
-00008570: 696e 290a 0a20 2020 2040 636c 6173 736d  in)..    @classm
-00008580: 6574 686f 640a 2020 2020 6465 6620 6c6f  ethod.    def lo
-00008590: 6164 5f73 335f 636f 6e66 6967 2863 6c73  ad_s3_config(cls
-000085a0: 2c20 636f 6e66 6967 5f70 6174 683a 2073  , config_path: s
-000085b0: 7472 2920 2d3e 2053 3343 6f6e 6669 673a  tr) -> S3Config:
-000085c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000085d0: 6361 7374 2853 3343 6f6e 6669 672c 2063  cast(S3Config, c
-000085e0: 6c73 2e6c 6f61 645f 6a73 6f6e 2863 6f6e  ls.load_json(con
-000085f0: 6669 675f 7061 7468 2929 0a0a 2020 2020  fig_path))..    
-00008600: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00008610: 2064 6566 2064 6f77 6e6c 6f61 645f 7333   def download_s3
-00008620: 5f66 726f 6d5f 6669 6c65 280a 2020 2020  _from_file(.    
-00008630: 2020 2020 2020 2020 636c 732c 2064 6573          cls, des
-00008640: 745f 7061 7468 3a20 4c69 7374 5b73 7472  t_path: List[str
-00008650: 5d2c 2063 6f6e 6669 675f 7061 7468 3a20  ], config_path: 
-00008660: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
-00008670: 2020 2020 2020 636c 732e 646f 776e 6c6f        cls.downlo
-00008680: 6164 5f73 3328 6465 7374 5f70 6174 682c  ad_s3(dest_path,
-00008690: 2063 6c73 2e6c 6f61 645f 7333 5f63 6f6e   cls.load_s3_con
-000086a0: 6669 6728 636f 6e66 6967 5f70 6174 6829  fig(config_path)
-000086b0: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
-000086c0: 7468 6f64 0a20 2020 2064 6566 2064 6f77  thod.    def dow
-000086d0: 6e6c 6f61 645f 7333 2864 6573 745f 7061  nload_s3(dest_pa
-000086e0: 7468 3a20 4c69 7374 5b73 7472 5d2c 2063  th: List[str], c
-000086f0: 6f6e 6669 673a 2053 3343 6f6e 6669 6729  onfig: S3Config)
-00008700: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00008710: 2020 696d 706f 7274 2062 6f74 6f33 0a0a    import boto3..
-00008720: 2020 2020 2020 2020 7333 203d 2062 6f74          s3 = bot
-00008730: 6f33 2e63 6c69 656e 7428 0a20 2020 2020  o3.client(.     
-00008740: 2020 2020 2020 2022 7333 222c 0a20 2020         "s3",.   
-00008750: 2020 2020 2020 2020 2061 7773 5f61 6363           aws_acc
-00008760: 6573 735f 6b65 795f 6964 3d63 6f6e 6669  ess_key_id=confi
-00008770: 675b 2261 6363 6572 6e5f 6177 735f 6b65  g["accern_aws_ke
-00008780: 7922 5d2c 0a20 2020 2020 2020 2020 2020  y"],.           
-00008790: 2061 7773 5f73 6563 7265 745f 6163 6365   aws_secret_acce
-000087a0: 7373 5f6b 6579 3d63 6f6e 6669 675b 2261  ss_key=config["a
-000087b0: 6363 6572 6e5f 6177 735f 6163 6365 7373  ccern_aws_access
-000087c0: 5f6b 6579 225d 290a 2020 2020 2020 2020  _key"]).        
-000087d0: 6173 7365 7274 206c 656e 2864 6573 745f  assert len(dest_
-000087e0: 7061 7468 2920 3d3d 206c 656e 2863 6f6e  path) == len(con
-000087f0: 6669 675b 226d 6f64 656c 5f64 6f77 6e6c  fig["model_downl
-00008800: 6f61 645f 7061 7468 225d 290a 2020 2020  oad_path"]).    
-00008810: 2020 2020 666f 7220 2864 6573 742c 2070      for (dest, p
-00008820: 6174 6829 2069 6e20 7a69 7028 6465 7374  ath) in zip(dest
-00008830: 5f70 6174 682c 2063 6f6e 6669 675b 226d  _path, config["m
-00008840: 6f64 656c 5f64 6f77 6e6c 6f61 645f 7061  odel_download_pa
-00008850: 7468 225d 293a 0a20 2020 2020 2020 2020  th"]):.         
-00008860: 2020 2073 332e 646f 776e 6c6f 6164 5f66     s3.download_f
-00008870: 696c 6528 636f 6e66 6967 5b22 6d6f 6465  ile(config["mode
-00008880: 6c5f 646f 776e 6c6f 6164 5f62 7563 6b65  l_download_bucke
-00008890: 7422 5d2c 2070 6174 682c 2064 6573 7429  t"], path, dest)
-000088a0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-000088b0: 6f64 0a20 2020 2064 6566 2075 706c 6f61  od.    def uploa
-000088c0: 645f 7333 5f66 726f 6d5f 6669 6c65 280a  d_s3_from_file(.
-000088d0: 2020 2020 2020 2020 2020 2020 636c 732c              cls,
-000088e0: 2073 6f75 7263 655f 7061 7468 3a20 4c69   source_path: Li
-000088f0: 7374 5b73 7472 5d2c 2063 6f6e 6669 675f  st[str], config_
-00008900: 7061 7468 3a20 7374 7229 202d 3e20 4e6f  path: str) -> No
-00008910: 6e65 3a0a 2020 2020 2020 2020 636c 732e  ne:.        cls.
-00008920: 7570 6c6f 6164 5f73 3328 736f 7572 6365  upload_s3(source
-00008930: 5f70 6174 682c 2063 6c73 2e6c 6f61 645f  _path, cls.load_
-00008940: 7333 5f63 6f6e 6669 6728 636f 6e66 6967  s3_config(config
-00008950: 5f70 6174 6829 290a 0a20 2020 2040 7374  _path))..    @st
-00008960: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00008970: 6566 2075 706c 6f61 645f 7333 2873 6f75  ef upload_s3(sou
-00008980: 7263 655f 7061 7468 3a20 4c69 7374 5b73  rce_path: List[s
-00008990: 7472 5d2c 2063 6f6e 6669 673a 2053 3343  tr], config: S3C
-000089a0: 6f6e 6669 6729 202d 3e20 4e6f 6e65 3a0a  onfig) -> None:.
-000089b0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
-000089c0: 6f74 6f33 0a0a 2020 2020 2020 2020 7333  oto3..        s3
-000089d0: 203d 2062 6f74 6f33 2e63 6c69 656e 7428   = boto3.client(
-000089e0: 0a20 2020 2020 2020 2020 2020 2022 7333  .            "s3
-000089f0: 222c 0a20 2020 2020 2020 2020 2020 2061  ",.            a
-00008a00: 7773 5f61 6363 6573 735f 6b65 795f 6964  ws_access_key_id
-00008a10: 3d63 6f6e 6669 675b 2261 6363 6572 6e5f  =config["accern_
-00008a20: 6177 735f 6b65 7922 5d2c 0a20 2020 2020  aws_key"],.     
-00008a30: 2020 2020 2020 2061 7773 5f73 6563 7265         aws_secre
-00008a40: 745f 6163 6365 7373 5f6b 6579 3d63 6f6e  t_access_key=con
-00008a50: 6669 675b 2261 6363 6572 6e5f 6177 735f  fig["accern_aws_
-00008a60: 6163 6365 7373 5f6b 6579 225d 290a 2020  access_key"]).  
-00008a70: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
-00008a80: 2873 6f75 7263 655f 7061 7468 2920 3d3d  (source_path) ==
-00008a90: 206c 656e 2863 6f6e 6669 675b 226d 6f64   len(config["mod
-00008aa0: 656c 5f64 6f77 6e6c 6f61 645f 7061 7468  el_download_path
-00008ab0: 225d 290a 2020 2020 2020 2020 666f 7220  "]).        for 
-00008ac0: 2873 6f75 7263 652c 2070 6174 6829 2069  (source, path) i
-00008ad0: 6e20 7a69 7028 736f 7572 6365 5f70 6174  n zip(source_pat
-00008ae0: 682c 2063 6f6e 6669 675b 226d 6f64 656c  h, config["model
-00008af0: 5f64 6f77 6e6c 6f61 645f 7061 7468 225d  _download_path"]
-00008b00: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00008b10: 332e 7570 6c6f 6164 5f66 696c 6528 736f  3.upload_file(so
-00008b20: 7572 6365 2c20 636f 6e66 6967 5b22 6d6f  urce, config["mo
-00008b30: 6465 6c5f 646f 776e 6c6f 6164 5f62 7563  del_download_buc
-00008b40: 6b65 7422 5d2c 2070 6174 6829 0a0a 2020  ket"], path)..  
-00008b50: 2020 6465 6620 6765 745f 7575 6964 2873    def get_uuid(s
-00008b60: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-00008b70: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
-00008b80: 2855 5549 4452 6573 706f 6e73 652c 2073  (UUIDResponse, s
-00008b90: 656c 662e 7265 7175 6573 745f 6a73 6f6e  elf.request_json
-00008ba0: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-00008bb0: 5448 4f44 5f47 4554 2c20 222f 7575 6964  THOD_GET, "/uuid
-00008bc0: 222c 207b 7d29 295b 2275 7569 6422 5d0a  ", {}))["uuid"].
-00008bd0: 0a20 2020 2064 6566 2064 656c 6574 655f  .    def delete_
-00008be0: 626c 6f62 7328 7365 6c66 2c20 626c 6f62  blobs(self, blob
-00008bf0: 5f75 7269 733a 204c 6973 745b 7374 725d  _uris: List[str]
-00008c00: 2920 2d3e 2044 656c 6574 6542 6c6f 6252  ) -> DeleteBlobR
-00008c10: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00008c20: 2072 6574 7572 6e20 6361 7374 2844 656c   return cast(Del
-00008c30: 6574 6542 6c6f 6252 6573 706f 6e73 652c  eteBlobResponse,
-00008c40: 2073 656c 662e 7265 7175 6573 745f 6a73   self.request_js
-00008c50: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00008c60: 4d45 5448 4f44 5f44 454c 4554 452c 2022  METHOD_DELETE, "
-00008c70: 2f62 6c6f 6222 2c20 7b0a 2020 2020 2020  /blob", {.      
-00008c80: 2020 2020 2020 2020 2020 2262 6c6f 625f            "blob_
-00008c90: 7572 6973 223a 2062 6c6f 625f 7572 6973  uris": blob_uris
-00008ca0: 2c0a 2020 2020 2020 2020 2020 2020 7d2c  ,.            },
-00008cb0: 0a20 2020 2020 2020 2029 290a 0a23 202a  .        ))..# *
-00008cc0: 2a2a 2058 594d 4543 6c69 656e 7420 2a2a  ** XYMEClient **
-00008cd0: 2a0a 0a0a 636c 6173 7320 4461 6748 616e  *...class DagHan
-00008ce0: 646c 653a 0a20 2020 2064 6566 205f 5f69  dle:.    def __i
-00008cf0: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-00008d00: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00008d10: 2020 2020 2063 6c69 656e 743a 2058 594d       client: XYM
-00008d20: 4543 6c69 656e 742c 0a20 2020 2020 2020  EClient,.       
-00008d30: 2020 2020 2064 6167 5f75 7269 3a20 7374       dag_uri: st
-00008d40: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-00008d50: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
-00008d60: 203d 2063 6c69 656e 740a 2020 2020 2020   = client.      
-00008d70: 2020 7365 6c66 2e5f 6461 675f 7572 6920    self._dag_uri 
-00008d80: 3d20 6461 675f 7572 690a 2020 2020 2020  = dag_uri.      
-00008d90: 2020 7365 6c66 2e5f 6e61 6d65 3a20 4f70    self._name: Op
-00008da0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00008db0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-00008dc0: 5f63 6f6d 7061 6e79 3a20 4f70 7469 6f6e  _company: Option
-00008dd0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
-00008de0: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
-00008df0: 7465 5f75 7269 3a20 4f70 7469 6f6e 616c  te_uri: Optional
-00008e00: 5b73 7472 5d20 3d20 4e6f 6e65 0a20 2020  [str] = None.   
-00008e10: 2020 2020 2073 656c 662e 5f75 7269 5f70       self._uri_p
-00008e20: 7265 6669 783a 204f 7074 696f 6e61 6c5b  refix: Optional[
-00008e30: 5552 4950 7265 6669 785d 203d 204e 6f6e  URIPrefix] = Non
-00008e40: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00008e50: 6973 5f68 6967 685f 7072 696f 7269 7479  is_high_priority
-00008e60: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-00008e70: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00008e80: 7365 6c66 2e5f 7175 6575 655f 6d6e 673a  self._queue_mng:
-00008e90: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00008ea0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00008eb0: 6c66 2e5f 7665 7273 696f 6e5f 6f76 6572  lf._version_over
-00008ec0: 7269 6465 3a20 4f70 7469 6f6e 616c 5b73  ride: Optional[s
-00008ed0: 7472 5d20 3d20 4e6f 6e65 0a20 2020 2020  tr] = None.     
-00008ee0: 2020 2073 656c 662e 5f6e 6f64 6573 3a20     self._nodes: 
-00008ef0: 4469 6374 5b73 7472 2c20 4e6f 6465 4861  Dict[str, NodeHa
-00008f00: 6e64 6c65 5d20 3d20 7b7d 0a20 2020 2020  ndle] = {}.     
-00008f10: 2020 2073 656c 662e 5f6e 6f64 655f 6c6f     self._node_lo
-00008f20: 6f6b 7570 3a20 4469 6374 5b73 7472 2c20  okup: Dict[str, 
-00008f30: 7374 725d 203d 207b 7d0a 2020 2020 2020  str] = {}.      
-00008f40: 2020 7365 6c66 2e5f 6479 6e61 6d69 635f    self._dynamic_
-00008f50: 6572 726f 723a 204f 7074 696f 6e61 6c5b  error: Optional[
-00008f60: 7374 725d 203d 204e 6f6e 650a 2020 2020  str] = None.    
-00008f70: 2020 2020 7365 6c66 2e5f 696e 733a 204f      self._ins: O
-00008f80: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-00008f90: 5d5d 203d 204e 6f6e 650a 2020 2020 2020  ]] = None.      
-00008fa0: 2020 7365 6c66 2e5f 6f75 7473 3a20 4f70    self._outs: Op
-00008fb0: 7469 6f6e 616c 5b4c 6973 745b 5475 706c  tional[List[Tupl
-00008fc0: 655b 7374 722c 2073 7472 5d5d 5d20 3d20  e[str, str]]] = 
-00008fd0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7265  None..    def re
-00008fe0: 6672 6573 6828 7365 6c66 2920 2d3e 204e  fresh(self) -> N
-00008ff0: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
-00009000: 662e 5f6e 616d 6520 3d20 4e6f 6e65 0a20  f._name = None. 
-00009010: 2020 2020 2020 2073 656c 662e 5f63 6f6d         self._com
-00009020: 7061 6e79 203d 204e 6f6e 650a 2020 2020  pany = None.    
-00009030: 2020 2020 7365 6c66 2e5f 7374 6174 655f      self._state_
-00009040: 7572 6920 3d20 4e6f 6e65 0a20 2020 2020  uri = None.     
-00009050: 2020 2073 656c 662e 5f75 7269 5f70 7265     self._uri_pre
-00009060: 6669 7820 3d20 4e6f 6e65 0a20 2020 2020  fix = None.     
-00009070: 2020 2073 656c 662e 5f69 735f 6869 6768     self._is_high
-00009080: 5f70 7269 6f72 6974 7920 3d20 4e6f 6e65  _priority = None
-00009090: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
-000090a0: 7565 7565 5f6d 6e67 203d 204e 6f6e 650a  ueue_mng = None.
-000090b0: 2020 2020 2020 2020 7365 6c66 2e5f 7665          self._ve
-000090c0: 7273 696f 6e5f 6f76 6572 7269 6465 203d  rsion_override =
-000090d0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-000090e0: 6c66 2e5f 696e 7320 3d20 4e6f 6e65 0a20  lf._ins = None. 
-000090f0: 2020 2020 2020 2073 656c 662e 5f6f 7574         self._out
-00009100: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
-00009110: 2023 204e 4f54 453a 2077 6520 646f 6e27   # NOTE: we don'
-00009120: 7420 7265 7365 7420 6e6f 6465 730a 0a20  t reset nodes.. 
-00009130: 2020 2064 6566 205f 6d61 7962 655f 7265     def _maybe_re
-00009140: 6672 6573 6828 7365 6c66 2920 2d3e 204e  fresh(self) -> N
-00009150: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-00009160: 7365 6c66 2e5f 636c 6965 6e74 2e69 735f  self._client.is_
-00009170: 6175 746f 5f72 6566 7265 7368 2829 3a0a  auto_refresh():.
-00009180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009190: 2e72 6566 7265 7368 2829 0a0a 2020 2020  .refresh()..    
-000091a0: 6465 6620 5f6d 6179 6265 5f66 6574 6368  def _maybe_fetch
-000091b0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000091c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000091d0: 5f6e 616d 6520 6973 204e 6f6e 653a 0a20  _name is None:. 
-000091e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000091f0: 5f66 6574 6368 5f69 6e66 6f28 290a 0a20  _fetch_info().. 
-00009200: 2020 2064 6566 2067 6574 5f69 6e66 6f28     def get_info(
-00009210: 7365 6c66 2920 2d3e 2044 6167 496e 666f  self) -> DagInfo
-00009220: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00009230: 2063 6173 7428 4461 6749 6e66 6f2c 2073   cast(DagInfo, s
-00009240: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
-00009250: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-00009260: 2020 2020 2020 4d45 5448 4f44 5f47 4554        METHOD_GET
-00009270: 2c20 222f 6461 675f 696e 666f 222c 207b  , "/dag_info", {
-00009280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009290: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
-000092a0: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
-000092b0: 2020 2020 7d29 290a 0a20 2020 2064 6566      }))..    def
-000092c0: 205f 6665 7463 685f 696e 666f 2873 656c   _fetch_info(sel
-000092d0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-000092e0: 2020 2020 696e 666f 203d 2073 656c 662e      info = self.
-000092f0: 6765 745f 696e 666f 2829 0a20 2020 2020  get_info().     
-00009300: 2020 2073 656c 662e 5f6e 616d 6520 3d20     self._name = 
-00009310: 696e 666f 5b22 6e61 6d65 225d 0a20 2020  info["name"].   
-00009320: 2020 2020 2073 656c 662e 5f63 6f6d 7061       self._compa
-00009330: 6e79 203d 2069 6e66 6f5b 2263 6f6d 7061  ny = info["compa
-00009340: 6e79 225d 0a20 2020 2020 2020 2073 656c  ny"].        sel
-00009350: 662e 5f73 7461 7465 5f75 7269 203d 2069  f._state_uri = i
-00009360: 6e66 6f5b 2273 7461 7465 5f75 7269 225d  nfo["state_uri"]
-00009370: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
-00009380: 7269 5f70 7265 6669 7820 3d20 696e 666f  ri_prefix = info
-00009390: 5b22 7572 695f 7072 6566 6978 225d 0a20  ["uri_prefix"]. 
-000093a0: 2020 2020 2020 2073 656c 662e 5f69 735f         self._is_
-000093b0: 6869 6768 5f70 7269 6f72 6974 7920 3d20  high_priority = 
-000093c0: 696e 666f 5b22 6869 6768 5f70 7269 6f72  info["high_prior
-000093d0: 6974 7922 5d0a 2020 2020 2020 2020 7365  ity"].        se
-000093e0: 6c66 2e5f 7175 6575 655f 6d6e 6720 3d20  lf._queue_mng = 
-000093f0: 696e 666f 5b22 7175 6575 655f 6d6e 6722  info["queue_mng"
-00009400: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
-00009410: 7665 7273 696f 6e5f 6f76 6572 7269 6465  version_override
-00009420: 203d 2069 6e66 6f5b 2276 6572 7369 6f6e   = info["version
-00009430: 5f6f 7665 7272 6964 6522 5d0a 2020 2020  _override"].    
-00009440: 2020 2020 7365 6c66 2e5f 696e 7320 3d20      self._ins = 
-00009450: 696e 666f 5b22 696e 7322 5d0a 2020 2020  info["ins"].    
-00009460: 2020 2020 7365 6c66 2e5f 6f75 7473 203d      self._outs =
-00009470: 205b 2865 6c5b 305d 2c20 656c 5b31 5d29   [(el[0], el[1])
-00009480: 2066 6f72 2065 6c20 696e 2069 6e66 6f5b   for el in info[
-00009490: 226f 7574 7322 5d5d 0a20 2020 2020 2020  "outs"]].       
-000094a0: 206f 6c64 5f6e 6f64 6573 203d 207b 7d20   old_nodes = {} 
-000094b0: 6966 2073 656c 662e 5f6e 6f64 6573 2069  if self._nodes i
-000094c0: 7320 4e6f 6e65 2065 6c73 6520 7365 6c66  s None else self
-000094d0: 2e5f 6e6f 6465 730a 2020 2020 2020 2020  ._nodes.        
-000094e0: 7365 6c66 2e5f 6e6f 6465 7320 3d20 7b0a  self._nodes = {.
-000094f0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-00009500: 5b22 6964 225d 3a20 4e6f 6465 4861 6e64  ["id"]: NodeHand
-00009510: 6c65 2e66 726f 6d5f 6e6f 6465 5f69 6e66  le.from_node_inf
-00009520: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
-00009530: 2020 2073 656c 662e 5f63 6c69 656e 742c     self._client,
-00009540: 2073 656c 662c 206e 6f64 652c 206f 6c64   self, node, old
-00009550: 5f6e 6f64 6573 2e67 6574 286e 6f64 655b  _nodes.get(node[
-00009560: 2269 6422 5d29 290a 2020 2020 2020 2020  "id"])).        
-00009570: 2020 2020 666f 7220 6e6f 6465 2069 6e20      for node in 
-00009580: 696e 666f 5b22 6e6f 6465 7322 5d0a 2020  info["nodes"].  
-00009590: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000095a0: 7365 6c66 2e5f 6e6f 6465 5f6c 6f6f 6b75  self._node_looku
-000095b0: 7020 3d20 7b0a 2020 2020 2020 2020 2020  p = {.          
-000095c0: 2020 6e6f 6465 5b22 6e61 6d65 225d 3a20    node["name"]: 
-000095d0: 6e6f 6465 5b22 6964 225d 0a20 2020 2020  node["id"].     
-000095e0: 2020 2020 2020 2066 6f72 206e 6f64 6520         for node 
-000095f0: 696e 2069 6e66 6f5b 226e 6f64 6573 225d  in info["nodes"]
-00009600: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00009610: 6e6f 6465 5b22 6e61 6d65 225d 2069 7320  node["name"] is 
-00009620: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-00009630: 207d 0a0a 2020 2020 6465 6620 6765 745f   }..    def get_
-00009640: 6e6f 6465 7328 7365 6c66 2920 2d3e 204c  nodes(self) -> L
-00009650: 6973 745b 7374 725d 3a0a 2020 2020 2020  ist[str]:.      
-00009660: 2020 7365 6c66 2e5f 6d61 7962 655f 7265    self._maybe_re
-00009670: 6672 6573 6828 290a 2020 2020 2020 2020  fresh().        
-00009680: 7365 6c66 2e5f 6d61 7962 655f 6665 7463  self._maybe_fetc
-00009690: 6828 290a 2020 2020 2020 2020 7265 7475  h().        retu
-000096a0: 726e 206c 6973 7428 7365 6c66 2e5f 6e6f  rn list(self._no
-000096b0: 6465 732e 6b65 7973 2829 290a 0a20 2020  des.keys())..   
-000096c0: 2064 6566 2067 6574 5f6e 6f64 6528 7365   def get_node(se
-000096d0: 6c66 2c20 6e6f 6465 5f6e 616d 653a 2073  lf, node_name: s
-000096e0: 7472 2920 2d3e 2027 4e6f 6465 4861 6e64  tr) -> 'NodeHand
-000096f0: 6c65 273a 0a20 2020 2020 2020 2073 656c  le':.        sel
-00009700: 662e 5f6d 6179 6265 5f72 6566 7265 7368  f._maybe_refresh
-00009710: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00009720: 5f6d 6179 6265 5f66 6574 6368 2829 0a20  _maybe_fetch(). 
-00009730: 2020 2020 2020 206e 6f64 655f 6964 203d         node_id =
-00009740: 2073 656c 662e 5f6e 6f64 655f 6c6f 6f6b   self._node_look
-00009750: 7570 2e67 6574 286e 6f64 655f 6e61 6d65  up.get(node_name
-00009760: 2c20 6e6f 6465 5f6e 616d 6529 0a20 2020  , node_name).   
-00009770: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009780: 2e5f 6e6f 6465 735b 6e6f 6465 5f69 645d  ._nodes[node_id]
-00009790: 0a0a 2020 2020 6465 6620 6765 745f 7572  ..    def get_ur
-000097a0: 6928 7365 6c66 2920 2d3e 2073 7472 3a0a  i(self) -> str:.
-000097b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000097c0: 656c 662e 5f64 6167 5f75 7269 0a0a 2020  elf._dag_uri..  
-000097d0: 2020 6465 6620 6765 745f 6e61 6d65 2873    def get_name(s
-000097e0: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-000097f0: 2020 2020 2073 656c 662e 5f6d 6179 6265       self._maybe
-00009800: 5f72 6566 7265 7368 2829 0a20 2020 2020  _refresh().     
-00009810: 2020 2073 656c 662e 5f6d 6179 6265 5f66     self._maybe_f
-00009820: 6574 6368 2829 0a20 2020 2020 2020 2061  etch().        a
-00009830: 7373 6572 7420 7365 6c66 2e5f 6e61 6d65  ssert self._name
-00009840: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00009850: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009860: 2e5f 6e61 6d65 0a0a 2020 2020 6465 6620  ._name..    def 
-00009870: 6765 745f 636f 6d70 616e 7928 7365 6c66  get_company(self
-00009880: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00009890: 2020 7365 6c66 2e5f 6d61 7962 655f 7265    self._maybe_re
-000098a0: 6672 6573 6828 290a 2020 2020 2020 2020  fresh().        
-000098b0: 7365 6c66 2e5f 6d61 7962 655f 6665 7463  self._maybe_fetc
-000098c0: 6828 290a 2020 2020 2020 2020 6173 7365  h().        asse
-000098d0: 7274 2073 656c 662e 5f63 6f6d 7061 6e79  rt self._company
-000098e0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-000098f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009900: 2e5f 636f 6d70 616e 790a 0a20 2020 2064  ._company..    d
-00009910: 6566 2067 6574 5f73 7461 7465 5f75 7269  ef get_state_uri
-00009920: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-00009930: 2020 2020 2020 2073 656c 662e 5f6d 6179         self._may
-00009940: 6265 5f72 6566 7265 7368 2829 0a20 2020  be_refresh().   
-00009950: 2020 2020 2073 656c 662e 5f6d 6179 6265       self._maybe
-00009960: 5f66 6574 6368 2829 0a20 2020 2020 2020  _fetch().       
-00009970: 2061 7373 6572 7420 7365 6c66 2e5f 7374   assert self._st
-00009980: 6174 655f 7572 6920 6973 206e 6f74 204e  ate_uri is not N
-00009990: 6f6e 650a 2020 2020 2020 2020 7265 7475  one.        retu
-000099a0: 726e 2073 656c 662e 5f73 7461 7465 5f75  rn self._state_u
-000099b0: 7269 0a0a 2020 2020 6465 6620 6765 745f  ri..    def get_
-000099c0: 7665 7273 696f 6e5f 6f76 6572 7269 6465  version_override
-000099d0: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-000099e0: 616c 5b73 7472 5d3a 0a20 2020 2020 2020  al[str]:.       
-000099f0: 2073 656c 662e 5f6d 6179 6265 5f72 6566   self._maybe_ref
-00009a00: 7265 7368 2829 0a20 2020 2020 2020 2073  resh().        s
-00009a10: 656c 662e 5f6d 6179 6265 5f66 6574 6368  elf._maybe_fetch
-00009a20: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
-00009a30: 7420 7365 6c66 2e5f 7665 7273 696f 6e5f  t self._version_
-00009a40: 6f76 6572 7269 6465 2069 7320 6e6f 7420  override is not 
-00009a50: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
-00009a60: 7572 6e20 7365 6c66 2e5f 7665 7273 696f  urn self._versio
-00009a70: 6e5f 6f76 6572 7269 6465 0a0a 2020 2020  n_override..    
-00009a80: 6465 6620 6765 745f 7572 695f 7072 6566  def get_uri_pref
-00009a90: 6978 2873 656c 6629 202d 3e20 5552 4950  ix(self) -> URIP
-00009aa0: 7265 6669 783a 0a20 2020 2020 2020 2073  refix:.        s
-00009ab0: 656c 662e 5f6d 6179 6265 5f72 6566 7265  elf._maybe_refre
-00009ac0: 7368 2829 0a20 2020 2020 2020 2073 656c  sh().        sel
-00009ad0: 662e 5f6d 6179 6265 5f66 6574 6368 2829  f._maybe_fetch()
-00009ae0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00009af0: 7365 6c66 2e5f 7572 695f 7072 6566 6978  self._uri_prefix
-00009b00: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00009b10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009b20: 2e5f 7572 695f 7072 6566 6978 0a0a 2020  ._uri_prefix..  
-00009b30: 2020 6465 6620 6765 745f 7469 6d69 6e67    def get_timing
-00009b40: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00009b50: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00009b60: 626c 6163 6b6c 6973 743a 204f 7074 696f  blacklist: Optio
-00009b70: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
-00009b80: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00009b90: 2020 2029 202d 3e20 5469 6d69 6e67 5265     ) -> TimingRe
-00009ba0: 7375 6c74 3a0a 2020 2020 2020 2020 626c  sult:.        bl
-00009bb0: 6973 7420 3d20 5b5d 2069 6620 626c 6163  ist = [] if blac
-00009bc0: 6b6c 6973 7420 6973 204e 6f6e 6520 656c  klist is None el
-00009bd0: 7365 2062 6c61 636b 6c69 7374 0a20 2020  se blacklist.   
-00009be0: 2020 2020 206e 6f64 655f 7469 6d69 6e67       node_timing
-00009bf0: 3a20 4469 6374 5b73 7472 2c20 4e6f 6465  : Dict[str, Node
-00009c00: 5469 6d69 6e67 5d20 3d20 7b7d 0a20 2020  Timing] = {}.   
-00009c10: 2020 2020 206e 6f64 6573 203d 2073 656c       nodes = sel
-00009c20: 662e 6765 745f 6e6f 6465 7328 290a 0a20  f.get_nodes().. 
-00009c30: 2020 2020 2020 2064 6566 2067 6574 5f66         def get_f
-00009c40: 696c 7465 7264 5f74 696d 6573 280a 2020  ilterd_times(.  
-00009c50: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00009c60: 6465 5f74 696d 653a 204c 6973 745b 5469  de_time: List[Ti
-00009c70: 6d69 6e67 5d29 202d 3e20 5475 706c 655b  ming]) -> Tuple[
-00009c80: 666c 6f61 742c 2066 6c6f 6174 2c20 4c69  float, float, Li
-00009c90: 7374 5b54 696d 696e 675d 5d3a 0a20 2020  st[Timing]]:.   
-00009ca0: 2020 2020 2020 2020 2066 6e73 203d 205b           fns = [
-00009cb0: 5d0a 2020 2020 2020 2020 2020 2020 6e6f  ].            no
-00009cc0: 6465 5f74 6f74 616c 203d 2030 2e30 0a20  de_total = 0.0. 
-00009cd0: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
-00009ce0: 616c 7565 2069 6e20 6e6f 6465 5f74 696d  alue in node_tim
-00009cf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009d00: 2020 2069 6620 7661 6c75 655b 226e 616d     if value["nam
-00009d10: 6522 5d20 6e6f 7420 696e 2062 6c69 7374  e"] not in blist
-00009d20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009d30: 2020 2020 2020 666e 732e 6170 7065 6e64        fns.append
-00009d40: 2876 616c 7565 290a 2020 2020 2020 2020  (value).        
-00009d50: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-00009d60: 5f74 6f74 616c 202b 3d20 7661 6c75 655b  _total += value[
-00009d70: 2274 6f74 616c 225d 0a20 2020 2020 2020  "total"].       
-00009d80: 2020 2020 2069 6620 6e6f 7420 666e 733a       if not fns:
-00009d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009da0: 2072 6574 7572 6e20 2830 2c20 302c 2066   return (0, 0, f
-00009db0: 6e73 290a 2020 2020 2020 2020 2020 2020  ns).            
-00009dc0: 7265 7475 726e 2028 6e6f 6465 5f74 6f74  return (node_tot
-00009dd0: 616c 2c20 6e6f 6465 5f74 6f74 616c 202f  al, node_total /
-00009de0: 206c 656e 2866 6e73 292c 2066 6e73 290a   len(fns), fns).
-00009df0: 0a20 2020 2020 2020 2064 6167 5f74 6f74  .        dag_tot
-00009e00: 616c 203d 2030 2e30 0a20 2020 2020 2020  al = 0.0.       
-00009e10: 2066 6f72 206e 6f64 6520 696e 206e 6f64   for node in nod
-00009e20: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00009e30: 6e6f 6465 5f67 6574 203d 2073 656c 662e  node_get = self.
-00009e40: 6765 745f 6e6f 6465 286e 6f64 6529 0a20  get_node(node). 
-00009e50: 2020 2020 2020 2020 2020 206e 6f64 655f             node_
-00009e60: 7469 6d65 203d 206e 6f64 655f 6765 742e  time = node_get.
-00009e70: 6765 745f 7469 6d69 6e67 2829 0a20 2020  get_timing().   
-00009e80: 2020 2020 2020 2020 206e 6f64 655f 6e61           node_na
-00009e90: 6d65 203d 206e 6f64 655f 6765 742e 6765  me = node_get.ge
-00009ea0: 745f 6e6f 6465 5f64 6566 2829 5b22 6e61  t_node_def()["na
-00009eb0: 6d65 225d 0a20 2020 2020 2020 2020 2020  me"].           
-00009ec0: 206e 6f64 655f 6964 203d 206e 6f64 655f   node_id = node_
-00009ed0: 6765 742e 6765 745f 6964 2829 0a20 2020  get.get_id().   
-00009ee0: 2020 2020 2020 2020 206e 6f64 655f 746f           node_to
-00009ef0: 7461 6c2c 2061 7667 5f74 696d 652c 2066  tal, avg_time, f
-00009f00: 6e73 203d 2067 6574 5f66 696c 7465 7264  ns = get_filterd
-00009f10: 5f74 696d 6573 286e 6f64 655f 7469 6d65  _times(node_time
-00009f20: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
-00009f30: 6465 5f74 696d 696e 675b 6e6f 6465 5f69  de_timing[node_i
-00009f40: 645d 203d 207b 0a20 2020 2020 2020 2020  d] = {.         
-00009f50: 2020 2020 2020 2022 6e6f 6465 5f6e 616d         "node_nam
-00009f60: 6522 3a20 6e6f 6465 5f6e 616d 652c 0a20  e": node_name,. 
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00009f80: 6e6f 6465 5f74 6f74 616c 223a 206e 6f64  node_total": nod
-00009f90: 655f 746f 7461 6c2c 0a20 2020 2020 2020  e_total,.       
-00009fa0: 2020 2020 2020 2020 2022 6e6f 6465 5f61           "node_a
-00009fb0: 7667 223a 2061 7667 5f74 696d 652c 0a20  vg": avg_time,. 
-00009fc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00009fd0: 666e 7322 3a20 666e 732c 0a20 2020 2020  fns": fns,.     
-00009fe0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00009ff0: 2020 2020 2064 6167 5f74 6f74 616c 202b       dag_total +
-0000a000: 3d20 6e6f 6465 5f74 6f74 616c 0a20 2020  = node_total.   
-0000a010: 2020 2020 206e 6f64 655f 7469 6d69 6e67       node_timing
-0000a020: 5f73 6f72 7465 6420 3d20 736f 7274 6564  _sorted = sorted
-0000a030: 280a 2020 2020 2020 2020 2020 2020 6e6f  (.            no
-0000a040: 6465 5f74 696d 696e 672e 6974 656d 7328  de_timing.items(
-0000a050: 292c 0a20 2020 2020 2020 2020 2020 206b  ),.            k
-0000a060: 6579 3d6c 616d 6264 6120 783a 2078 5b31  ey=lambda x: x[1
-0000a070: 5d5b 226e 6f64 655f 746f 7461 6c22 5d2c  ]["node_total"],
-0000a080: 0a20 2020 2020 2020 2020 2020 2072 6576  .            rev
-0000a090: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
-0000a0a0: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-0000a0b0: 2020 2020 2020 2020 2264 6167 5f74 6f74          "dag_tot
-0000a0c0: 616c 223a 2064 6167 5f74 6f74 616c 2c0a  al": dag_total,.
-0000a0d0: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
-0000a0e0: 6573 223a 206e 6f64 655f 7469 6d69 6e67  es": node_timing
-0000a0f0: 5f73 6f72 7465 642c 0a20 2020 2020 2020  _sorted,.       
-0000a100: 207d 0a0a 2020 2020 6465 6620 6973 5f68   }..    def is_h
-0000a110: 6967 685f 7072 696f 7269 7479 2873 656c  igh_priority(sel
-0000a120: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
-0000a130: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
-0000a140: 7265 6672 6573 6828 290a 2020 2020 2020  refresh().      
-0000a150: 2020 7365 6c66 2e5f 6d61 7962 655f 6665    self._maybe_fe
-0000a160: 7463 6828 290a 2020 2020 2020 2020 6173  tch().        as
-0000a170: 7365 7274 2073 656c 662e 5f69 735f 6869  sert self._is_hi
-0000a180: 6768 5f70 7269 6f72 6974 7920 6973 206e  gh_priority is n
-0000a190: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-0000a1a0: 7265 7475 726e 2073 656c 662e 5f69 735f  return self._is_
-0000a1b0: 6869 6768 5f70 7269 6f72 6974 790a 0a20  high_priority.. 
-0000a1c0: 2020 2064 6566 2069 735f 7175 6575 6528     def is_queue(
-0000a1d0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000a1e0: 2020 2020 2020 2073 656c 662e 5f6d 6179         self._may
-0000a1f0: 6265 5f72 6566 7265 7368 2829 0a20 2020  be_refresh().   
-0000a200: 2020 2020 2073 656c 662e 5f6d 6179 6265       self._maybe
-0000a210: 5f66 6574 6368 2829 0a20 2020 2020 2020  _fetch().       
-0000a220: 2072 6574 7572 6e20 7365 6c66 2e5f 7175   return self._qu
-0000a230: 6575 655f 6d6e 6720 6973 206e 6f74 204e  eue_mng is not N
-0000a240: 6f6e 650a 0a20 2020 2064 6566 2067 6574  one..    def get
-0000a250: 5f71 7565 7565 5f6d 6e67 2873 656c 6629  _queue_mng(self)
-0000a260: 202d 3e20 4f70 7469 6f6e 616c 5b73 7472   -> Optional[str
-0000a270: 5d3a 0a20 2020 2020 2020 2073 656c 662e  ]:.        self.
-0000a280: 5f6d 6179 6265 5f72 6566 7265 7368 2829  _maybe_refresh()
-0000a290: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
-0000a2a0: 6179 6265 5f66 6574 6368 2829 0a20 2020  aybe_fetch().   
-0000a2b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000a2c0: 2e5f 7175 6575 655f 6d6e 670a 0a20 2020  ._queue_mng..   
-0000a2d0: 2064 6566 2067 6574 5f69 6e73 2873 656c   def get_ins(sel
-0000a2e0: 6629 202d 3e20 4c69 7374 5b73 7472 5d3a  f) -> List[str]:
-0000a2f0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
-0000a300: 6179 6265 5f72 6566 7265 7368 2829 0a20  aybe_refresh(). 
-0000a310: 2020 2020 2020 2073 656c 662e 5f6d 6179         self._may
-0000a320: 6265 5f66 6574 6368 2829 0a20 2020 2020  be_fetch().     
-0000a330: 2020 2061 7373 6572 7420 7365 6c66 2e5f     assert self._
-0000a340: 696e 7320 6973 206e 6f74 204e 6f6e 650a  ins is not None.
-0000a350: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000a360: 656c 662e 5f69 6e73 0a0a 2020 2020 6465  elf._ins..    de
-0000a370: 6620 6765 745f 6f75 7473 2873 656c 6629  f get_outs(self)
-0000a380: 202d 3e20 4c69 7374 5b54 7570 6c65 5b73   -> List[Tuple[s
-0000a390: 7472 2c20 7374 725d 5d3a 0a20 2020 2020  tr, str]]:.     
-0000a3a0: 2020 2073 656c 662e 5f6d 6179 6265 5f72     self._maybe_r
-0000a3b0: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
-0000a3c0: 2073 656c 662e 5f6d 6179 6265 5f66 6574   self._maybe_fet
-0000a3d0: 6368 2829 0a20 2020 2020 2020 2061 7373  ch().        ass
-0000a3e0: 6572 7420 7365 6c66 2e5f 6f75 7473 2069  ert self._outs i
-0000a3f0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0000a400: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000a410: 6f75 7473 0a0a 2020 2020 4063 6f6e 7465  outs..    @conte
-0000a420: 7874 6c69 622e 636f 6e74 6578 746d 616e  xtlib.contextman
-0000a430: 6167 6572 0a20 2020 2064 6566 2062 756c  ager.    def bul
-0000a440: 6b5f 6f70 6572 6174 696f 6e28 7365 6c66  k_operation(self
-0000a450: 2920 2d3e 2049 7465 7261 746f 725b 626f  ) -> Iterator[bo
-0000a460: 6f6c 5d3a 0a20 2020 2020 2020 2077 6974  ol]:.        wit
-0000a470: 6820 7365 6c66 2e5f 636c 6965 6e74 2e62  h self._client.b
-0000a480: 756c 6b5f 6f70 6572 6174 696f 6e28 2920  ulk_operation() 
-0000a490: 6173 2064 6f5f 7265 6672 6573 683a 0a20  as do_refresh:. 
-0000a4a0: 2020 2020 2020 2020 2020 2069 6620 646f             if do
-0000a4b0: 5f72 6566 7265 7368 3a0a 2020 2020 2020  _refresh:.      
-0000a4c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000a4d0: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
-0000a4e0: 2020 2020 2079 6965 6c64 2064 6f5f 7265       yield do_re
-0000a4f0: 6672 6573 680a 0a20 2020 2064 6566 2073  fresh..    def s
-0000a500: 6574 5f64 6167 2873 656c 662c 2064 6566  et_dag(self, def
-0000a510: 733a 2042 6173 6544 6167 4465 6629 202d  s: BaseDagDef) -
-0000a520: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000a530: 7365 6c66 2e5f 636c 6965 6e74 2e73 6574  self._client.set
-0000a540: 5f64 6167 2873 656c 662e 6765 745f 7572  _dag(self.get_ur
-0000a550: 6928 292c 2064 6566 7329 0a0a 2020 2020  i(), defs)..    
-0000a560: 6465 6620 6479 6e61 6d69 635f 6d6f 6465  def dynamic_mode
-0000a570: 6c28 0a20 2020 2020 2020 2020 2020 2073  l(.            s
-0000a580: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000a590: 2069 6e70 7574 733a 204c 6973 745b 416e   inputs: List[An
-0000a5a0: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
-0000a5b0: 666f 726d 6174 5f6d 6574 686f 643a 2073  format_method: s
-0000a5c0: 7472 203d 2022 7369 6d70 6c65 222c 0a20  tr = "simple",. 
-0000a5d0: 2020 2020 2020 2020 2020 206e 6f5f 6361             no_ca
-0000a5e0: 6368 653a 2062 6f6f 6c20 3d20 4661 6c73  che: bool = Fals
-0000a5f0: 6529 202d 3e20 4c69 7374 5b41 6e79 5d3a  e) -> List[Any]:
-0000a600: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
-0000a610: 6173 7428 4479 6e61 6d69 6352 6573 756c  ast(DynamicResul
-0000a620: 7473 2c20 7365 6c66 2e5f 636c 6965 6e74  ts, self._client
-0000a630: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
-0000a640: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
-0000a650: 445f 504f 5354 2c20 222f 6479 6e61 6d69  D_POST, "/dynami
-0000a660: 635f 6d6f 6465 6c22 2c20 7b0a 2020 2020  c_model", {.    
-0000a670: 2020 2020 2020 2020 2020 2020 2266 6f72              "for
-0000a680: 6d61 7422 3a20 666f 726d 6174 5f6d 6574  mat": format_met
-0000a690: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
-0000a6a0: 2020 2020 2022 696e 7075 7473 223a 2069       "inputs": i
-0000a6b0: 6e70 7574 732c 0a20 2020 2020 2020 2020  nputs,.         
-0000a6c0: 2020 2020 2020 2022 6e6f 5f63 6163 6865         "no_cache
-0000a6d0: 223a 206e 6f5f 6361 6368 652c 0a20 2020  ": no_cache,.   
-0000a6e0: 2020 2020 2020 2020 2020 2020 2022 6461               "da
-0000a6f0: 6722 3a20 7365 6c66 2e67 6574 5f75 7269  g": self.get_uri
-0000a700: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0000a710: 7d29 290a 2020 2020 2020 2020 7265 7475  })).        retu
-0000a720: 726e 2072 6573 5b22 7265 7375 6c74 7322  rn res["results"
-0000a730: 5d0a 0a20 2020 2064 6566 205f 6c65 6761  ]..    def _lega
-0000a740: 6379 5f64 796e 616d 6963 5f6c 6973 7428  cy_dynamic_list(
-0000a750: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a760: 662c 0a20 2020 2020 2020 2020 2020 2069  f,.            i
-0000a770: 6e70 7574 733a 204c 6973 745b 416e 795d  nputs: List[Any]
-0000a780: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-0000a790: 7075 745f 6b65 793a 204f 7074 696f 6e61  put_key: Optiona
-0000a7a0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000a7b0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-0000a7c0: 745f 6b65 793a 204f 7074 696f 6e61 6c5b  t_key: Optional[
-0000a7d0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000a7e0: 2020 2020 2020 2020 2073 706c 6974 5f74           split_t
-0000a7f0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
-0000a800: 203d 2031 3030 302c 0a20 2020 2020 2020   = 1000,.       
-0000a810: 2020 2020 206d 6178 5f74 6872 6561 6473       max_threads
-0000a820: 3a20 696e 7420 3d20 3530 2c0a 2020 2020  : int = 50,.    
-0000a830: 2020 2020 2020 2020 666f 726d 6174 5f6d          format_m
-0000a840: 6574 686f 643a 2073 7472 203d 2022 7369  ethod: str = "si
-0000a850: 6d70 6c65 222c 0a20 2020 2020 2020 2020  mple",.         
-0000a860: 2020 2066 6f72 6365 5f6b 6579 733a 2062     force_keys: b
-0000a870: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000a880: 2020 2020 2020 2020 206e 6f5f 6361 6368           no_cach
-0000a890: 653a 2062 6f6f 6c20 3d20 4661 6c73 6529  e: bool = False)
-0000a8a0: 202d 3e20 4c69 7374 5b41 6e79 5d3a 0a20   -> List[Any]:. 
-0000a8b0: 2020 2020 2020 2069 6620 7370 6c69 745f         if split_
-0000a8c0: 7468 2069 7320 4e6f 6e65 206f 7220 6c65  th is None or le
-0000a8d0: 6e28 696e 7075 7473 2920 3c3d 2073 706c  n(inputs) <= spl
-0000a8e0: 6974 5f74 683a 0a20 2020 2020 2020 2020  it_th:.         
-0000a8f0: 2020 2072 6573 203d 2063 6173 7428 4479     res = cast(Dy
-0000a900: 6e61 6d69 6352 6573 756c 7473 2c20 7365  namicResults, se
-0000a910: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-0000a920: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-0000a930: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-0000a940: 504f 5354 2c20 222f 6479 6e61 6d69 635f  POST, "/dynamic_
-0000a950: 6c69 7374 222c 207b 0a20 2020 2020 2020  list", {.       
-0000a960: 2020 2020 2020 2020 2020 2020 2022 666f               "fo
-0000a970: 7263 655f 6b65 7973 223a 2066 6f72 6365  rce_keys": force
-0000a980: 5f6b 6579 732c 0a20 2020 2020 2020 2020  _keys,.         
-0000a990: 2020 2020 2020 2020 2020 2022 666f 726d             "form
-0000a9a0: 6174 223a 2066 6f72 6d61 745f 6d65 7468  at": format_meth
-0000a9b0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
-0000a9c0: 2020 2020 2020 2020 2269 6e70 7574 5f6b          "input_k
-0000a9d0: 6579 223a 2069 6e70 7574 5f6b 6579 2c0a  ey": input_key,.
-0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9f0: 2020 2020 2269 6e70 7574 7322 3a20 696e      "inputs": in
-0000aa00: 7075 7473 2c0a 2020 2020 2020 2020 2020  puts,.          
-0000aa10: 2020 2020 2020 2020 2020 226e 6f5f 6361            "no_ca
-0000aa20: 6368 6522 3a20 6e6f 5f63 6163 6865 2c0a  che": no_cache,.
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa40: 2020 2020 226f 7574 7075 745f 6b65 7922      "output_key"
-0000aa50: 3a20 6f75 7470 7574 5f6b 6579 2c0a 2020  : output_key,.  
-0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa70: 2020 2264 6167 223a 2073 656c 662e 6765    "dag": self.ge
-0000aa80: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
-0000aa90: 2020 2020 2020 2020 207d 2929 0a20 2020           })).   
-0000aaa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000aab0: 7265 735b 2272 6573 756c 7473 225d 0a20  res["results"]. 
-0000aac0: 2020 2020 2020 2023 2046 4958 4d45 3a20         # FIXME: 
-0000aad0: 7772 6974 6520 6765 6e65 7269 6320 7370  write generic sp
-0000aae0: 6c69 7465 7261 746f 7220 696d 706c 656d  literator implem
-0000aaf0: 656e 7461 7469 6f6e 0a20 2020 2020 2020  entation.       
-0000ab00: 2073 706c 6974 5f6e 756d 3a20 696e 7420   split_num: int 
-0000ab10: 3d20 7370 6c69 745f 7468 0a20 2020 2020  = split_th.     
-0000ab20: 2020 2061 7373 6572 7420 7370 6c69 745f     assert split_
-0000ab30: 6e75 6d20 3e20 300a 2020 2020 2020 2020  num > 0.        
-0000ab40: 7265 735f 6172 723a 204c 6973 745b 416e  res_arr: List[An
-0000ab50: 795d 203d 205b 4e6f 6e65 5d20 2a20 6c65  y] = [None] * le
-0000ab60: 6e28 696e 7075 7473 290a 2020 2020 2020  n(inputs).      
-0000ab70: 2020 6578 633a 204c 6973 745b 4f70 7469    exc: List[Opti
-0000ab80: 6f6e 616c 5b42 6173 6545 7863 6570 7469  onal[BaseExcepti
-0000ab90: 6f6e 5d5d 203d 205b 4e6f 6e65 5d0a 2020  on]] = [None].  
-0000aba0: 2020 2020 2020 6163 7469 7665 5f74 6873        active_ths
-0000abb0: 3a20 5365 745b 7468 7265 6164 696e 672e  : Set[threading.
-0000abc0: 5468 7265 6164 5d20 3d20 7365 7428 290a  Thread] = set().
-0000abd0: 0a20 2020 2020 2020 2064 6566 2063 6f6d  .        def com
-0000abe0: 7075 7465 5f68 616c 6628 6375 723a 204c  pute_half(cur: L
-0000abf0: 6973 745b 416e 795d 2c20 6f66 6673 6574  ist[Any], offset
-0000ac00: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-0000ac10: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-0000ac20: 7863 5b30 5d20 6973 206e 6f74 204e 6f6e  xc[0] is not Non
-0000ac30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000ac40: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000ac50: 2020 2020 2020 6966 206c 656e 2863 7572        if len(cur
-0000ac60: 2920 3c3d 2073 706c 6974 5f6e 756d 3a0a  ) <= split_num:.
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000ac90: 2020 2020 2020 2020 2063 7572 5f72 6573           cur_res
-0000aca0: 203d 2073 656c 662e 5f6c 6567 6163 795f   = self._legacy_
-0000acb0: 6479 6e61 6d69 635f 6c69 7374 280a 2020  dynamic_list(.  
-0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acd0: 2020 2020 2020 6375 722c 0a20 2020 2020        cur,.     
-0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acf0: 2020 2069 6e70 7574 5f6b 6579 3d69 6e70     input_key=inp
-0000ad00: 7574 5f6b 6579 2c0a 2020 2020 2020 2020  ut_key,.        
-0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad20: 6f75 7470 7574 5f6b 6579 3d6f 7574 7075  output_key=outpu
-0000ad30: 745f 6b65 792c 0a20 2020 2020 2020 2020  t_key,.         
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ad50: 706c 6974 5f74 683d 4e6f 6e65 2c0a 2020  plit_th=None,.  
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 2020 2020 6d61 785f 7468 7265 6164        max_thread
-0000ad80: 733d 6d61 785f 7468 7265 6164 732c 0a20  s=max_threads,. 
-0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ada0: 2020 2020 2020 2066 6f72 6d61 745f 6d65         format_me
-0000adb0: 7468 6f64 3d66 6f72 6d61 745f 6d65 7468  thod=format_meth
-0000adc0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
-0000add0: 2020 2020 2020 2020 2020 2020 666f 7263              forc
-0000ade0: 655f 6b65 7973 3d66 6f72 6365 5f6b 6579  e_keys=force_key
-0000adf0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000ae00: 2020 2020 2020 2020 2020 206e 6f5f 6361             no_ca
-0000ae10: 6368 653d 6e6f 5f63 6163 6865 290a 2020  che=no_cache).  
-0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae30: 2020 7265 735f 6172 725b 6f66 6673 6574    res_arr[offset
-0000ae40: 3a6f 6666 7365 7420 2b20 6c65 6e28 6375  :offset + len(cu
-0000ae50: 725f 7265 7329 5d20 3d20 6375 725f 7265  r_res)] = cur_re
-0000ae60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000ae70: 2020 6578 6365 7074 2042 6173 6545 7863    except BaseExc
-0000ae80: 6570 7469 6f6e 2061 7320 653a 2020 2320  eption as e:  # 
-0000ae90: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-0000aea0: 6272 6f61 642d 6578 6365 7074 0a20 2020  broad-except.   
+000000b0: 696f 6e61 6c2c 0a20 2020 2067 6574 5f61  ional,.    get_a
+000000c0: 7267 732c 0a20 2020 206f 7665 726c 6f61  rgs,.    overloa
+000000d0: 642c 0a20 2020 2053 6574 2c0a 2020 2020  d,.    Set,.    
+000000e0: 5465 7874 494f 2c0a 2020 2020 5475 706c  TextIO,.    Tupl
+000000f0: 652c 0a20 2020 2054 5950 455f 4348 4543  e,.    TYPE_CHEC
+00000100: 4b49 4e47 2c0a 2020 2020 556e 696f 6e2c  KING,.    Union,
+00000110: 0a29 0a69 6d70 6f72 7420 696f 0a69 6d70  .).import io.imp
+00000120: 6f72 7420 6f73 0a69 6d70 6f72 7420 7069  ort os.import pi
+00000130: 636b 6c65 0a69 6d70 6f72 7420 7379 730a  ckle.import sys.
+00000140: 696d 706f 7274 206a 736f 6e0a 696d 706f  import json.impo
+00000150: 7274 2074 696d 650a 696d 706f 7274 2077  rt time.import w
+00000160: 6561 6b72 6566 0a69 6d70 6f72 7420 696e  eakref.import in
+00000170: 7370 6563 740a 696d 706f 7274 2074 6578  spect.import tex
+00000180: 7477 7261 700a 696d 706f 7274 2074 6872  twrap.import thr
+00000190: 6561 6469 6e67 0a69 6d70 6f72 7420 636f  eading.import co
+000001a0: 6e74 6578 746c 6962 0a66 726f 6d20 696f  ntextlib.from io
+000001b0: 2069 6d70 6f72 7420 4279 7465 7349 4f2c   import BytesIO,
+000001c0: 2053 7472 696e 6749 4f0a 6672 6f6d 2075   StringIO.from u
+000001d0: 726c 6c69 622e 7061 7273 6520 696d 706f  rllib.parse impo
+000001e0: 7274 2075 726c 7061 7273 652c 2075 726c  rt urlparse, url
+000001f0: 756e 7061 7273 650a 6672 6f6d 2070 6174  unparse.from pat
+00000200: 686c 6962 2069 6d70 6f72 7420 506f 7369  hlib import Posi
+00000210: 7850 6174 682c 2050 7572 6550 6174 680a  xPath, PurePath.
+00000220: 6672 6f6d 2067 7261 7068 7669 7a2e 6261  from graphviz.ba
+00000230: 636b 656e 6420 696d 706f 7274 2045 7865  ckend import Exe
+00000240: 6375 7461 626c 654e 6f74 466f 756e 640a  cutableNotFound.
+00000250: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
+00000260: 2070 640a 696d 706f 7274 2072 6571 7565   pd.import reque
+00000270: 7374 730a 6672 6f6d 2072 6571 7565 7374  sts.from request
+00000280: 7320 696d 706f 7274 2052 6573 706f 6e73  s import Respons
+00000290: 650a 6672 6f6d 2072 6571 7565 7374 732e  e.from requests.
+000002a0: 6578 6365 7074 696f 6e73 2069 6d70 6f72  exceptions impor
+000002b0: 7420 4854 5450 4572 726f 722c 2052 6571  t HTTPError, Req
+000002c0: 7565 7374 4578 6365 7074 696f 6e0a 6672  uestException.fr
+000002d0: 6f6d 2074 7970 696e 675f 6578 7465 6e73  om typing_extens
+000002e0: 696f 6e73 2069 6d70 6f72 7420 4c69 7465  ions import Lite
+000002f0: 7261 6c0a 696d 706f 7274 2071 7569 636b  ral.import quick
+00000300: 5f73 6572 7665 720a 0a66 726f 6d20 2e75  _server..from .u
+00000310: 7469 6c20 696d 706f 7274 2028 0a20 2020  til import (.   
+00000320: 2061 7379 6e63 5f63 6f6d 7075 7465 2c0a   async_compute,.
+00000330: 2020 2020 4279 7465 5265 7370 6f6e 7365      ByteResponse
+00000340: 2c0a 2020 2020 636f 6d70 7574 655f 7061  ,.    compute_pa
+00000350: 7261 6c6c 656c 2c0a 2020 2020 636f 6e74  rallel,.    cont
+00000360: 656e 745f 746f 5f63 7376 5f62 7974 6573  ent_to_csv_bytes
+00000370: 2c0a 2020 2020 6466 5f74 6f5f 6373 765f  ,.    df_to_csv_
+00000380: 6279 7465 732c 0a20 2020 2067 6574 5f61  bytes,.    get_a
+00000390: 6765 2c0a 2020 2020 6765 745f 6669 6c65  ge,.    get_file
+000003a0: 5f68 6173 682c 0a20 2020 2067 6574 5f66  _hash,.    get_f
+000003b0: 696c 655f 7570 6c6f 6164 5f63 6875 6e6b  ile_upload_chunk
+000003c0: 5f73 697a 652c 0a20 2020 2067 6574 5f6d  _size,.    get_m
+000003d0: 6178 5f72 6574 7279 2c0a 2020 2020 6765  ax_retry,.    ge
+000003e0: 745f 7072 6f67 7265 7373 5f62 6172 2c0a  t_progress_bar,.
+000003f0: 2020 2020 6765 745f 7265 7472 795f 736c      get_retry_sl
+00000400: 6565 702c 0a20 2020 2068 6173 5f67 7261  eep,.    has_gra
+00000410: 7068 5f65 6173 792c 0a20 2020 2069 6e74  ph_easy,.    int
+00000420: 6572 7072 6574 5f63 7479 7065 2c0a 2020  erpret_ctype,.  
+00000430: 2020 6973 5f6a 7570 7974 6572 2c0a 2020    is_jupyter,.  
+00000440: 2020 6d61 7962 655f 6a73 6f6e 5f6c 6f61    maybe_json_loa
+00000450: 6473 2c0a 2020 2020 6d65 7267 655f 6374  ds,.    merge_ct
+00000460: 7970 652c 0a20 2020 2073 6166 655f 6f70  ype,.    safe_op
+00000470: 745f 6e75 6d2c 0a20 2020 2053 6572 7665  t_num,.    Serve
+00000480: 7253 6964 6545 7272 6f72 2c0a 2020 2020  rSideError,.    
+00000490: 746f 5f62 6f6f 6c2c 0a29 0a66 726f 6d20  to_bool,.).from 
+000004a0: 2e74 7970 6573 2069 6d70 6f72 7420 280a  .types import (.
+000004b0: 2020 2020 416c 6c6f 7765 6443 7573 746f      AllowedCusto
+000004c0: 6d49 6d70 6f72 7473 2c0a 2020 2020 426c  mImports,.    Bl
+000004d0: 6f62 4465 7461 696c 732c 0a20 2020 2042  obDetails,.    B
+000004e0: 6c6f 6246 696c 6573 5265 7370 6f6e 7365  lobFilesResponse
+000004f0: 2c0a 2020 2020 426c 6f62 496e 6974 2c0a  ,.    BlobInit,.
+00000500: 2020 2020 426c 6f62 4f77 6e65 722c 0a20      BlobOwner,. 
+00000510: 2020 2042 6c6f 6254 7970 6552 6573 706f     BlobTypeRespo
+00000520: 6e73 652c 0a20 2020 2042 6c6f 6255 5249  nse,.    BlobURI
+00000530: 5265 7370 6f6e 7365 2c0a 2020 2020 4361  Response,.    Ca
+00000540: 6368 6553 7461 7473 2c0a 2020 2020 436f  cheStats,.    Co
+00000550: 7079 426c 6f62 2c0a 2020 2020 4461 6743  pyBlob,.    DagC
+00000560: 7265 6174 652c 0a20 2020 2044 6167 4475  reate,.    DagDu
+00000570: 7052 6573 706f 6e73 652c 0a20 2020 2044  pResponse,.    D
+00000580: 6167 496e 666f 2c0a 2020 2020 4461 6749  agInfo,.    DagI
+00000590: 6e69 742c 0a20 2020 2044 6167 4c69 7374  nit,.    DagList
+000005a0: 2c0a 2020 2020 4461 6750 7265 7474 794e  ,.    DagPrettyN
+000005b0: 6f64 652c 0a20 2020 2044 6167 5265 6c6f  ode,.    DagRelo
+000005c0: 6164 2c0a 2020 2020 4461 6753 7461 7475  ad,.    DagStatu
+000005d0: 732c 0a20 2020 2044 656c 6574 6542 6c6f  s,.    DeleteBlo
+000005e0: 6252 6573 706f 6e73 652c 0a20 2020 2044  bResponse,.    D
+000005f0: 796e 616d 6963 5265 7375 6c74 732c 0a20  ynamicResults,. 
+00000600: 2020 2044 796e 616d 6963 5374 6174 7573     DynamicStatus
+00000610: 5265 7370 6f6e 7365 2c0a 2020 2020 4553  Response,.    ES
+00000620: 5175 6572 7952 6573 706f 6e73 652c 0a20  QueryResponse,. 
+00000630: 2020 2046 696c 654d 6170 2c0a 2020 2020     FileMap,.    
+00000640: 466c 7573 6841 6c6c 5175 6575 6573 5265  FlushAllQueuesRe
+00000650: 7370 6f6e 7365 2c0a 2020 2020 496e 4375  sponse,.    InCu
+00000660: 7273 6f72 732c 0a20 2020 2049 6e73 7461  rsors,.    Insta
+00000670: 6e63 6553 7461 7475 732c 0a20 2020 204a  nceStatus,.    J
+00000680: 534f 4e42 6c6f 6241 7070 656e 6452 6573  SONBlobAppendRes
+00000690: 706f 6e73 652c 0a20 2020 204b 6166 6b61  ponse,.    Kafka
+000006a0: 4772 6f75 702c 0a20 2020 204b 6166 6b61  Group,.    Kafka
+000006b0: 4d65 7373 6167 652c 0a20 2020 204b 6166  Message,.    Kaf
+000006c0: 6b61 4f66 6673 6574 732c 0a20 2020 204b  kaOffsets,.    K
+000006d0: 6166 6b61 5468 726f 7567 6870 7574 2c0a  afkaThroughput,.
+000006e0: 2020 2020 4b61 666b 6154 6f70 6963 4e61      KafkaTopicNa
+000006f0: 6d65 732c 0a20 2020 204b 6166 6b61 546f  mes,.    KafkaTo
+00000700: 7069 6373 2c0a 2020 2020 4b6e 6f77 6e42  pics,.    KnownB
+00000710: 6c6f 6273 2c0a 2020 2020 4d69 6e69 6d61  lobs,.    Minima
+00000720: 6c51 7565 7565 5374 6174 7352 6573 706f  lQueueStatsRespo
+00000730: 6e73 652c 0a20 2020 204d 6f64 656c 496e  nse,.    ModelIn
+00000740: 666f 2c0a 2020 2020 4d6f 6465 6c50 6172  fo,.    ModelPar
+00000750: 616d 7352 6573 706f 6e73 652c 0a20 2020  amsResponse,.   
+00000760: 204d 6f64 656c 5265 6c65 6173 6552 6573   ModelReleaseRes
+00000770: 706f 6e73 652c 0a20 2020 204d 6f64 656c  ponse,.    Model
+00000780: 5665 7273 696f 6e52 6573 706f 6e73 652c  VersionResponse,
+00000790: 0a20 2020 204e 616d 6573 7061 6365 4c69  .    NamespaceLi
+000007a0: 7374 2c0a 2020 2020 4e61 6d65 7370 6163  st,.    Namespac
+000007b0: 6555 7064 6174 6553 6574 7469 6e67 732c  eUpdateSettings,
+000007c0: 0a20 2020 204e 6f64 6543 6875 6e6b 2c0a  .    NodeChunk,.
+000007d0: 2020 2020 4e6f 6465 4375 7374 6f6d 436f      NodeCustomCo
+000007e0: 6465 2c0a 2020 2020 4e6f 6465 4375 7374  de,.    NodeCust
+000007f0: 6f6d 496d 706f 7274 732c 0a20 2020 204e  omImports,.    N
+00000800: 6f64 6544 6566 2c0a 2020 2020 4e6f 6465  odeDef,.    Node
+00000810: 4465 6649 6e66 6f2c 0a20 2020 204e 6f64  DefInfo,.    Nod
+00000820: 6549 6e66 6f2c 0a20 2020 204e 6f64 6553  eInfo,.    NodeS
+00000830: 7461 7465 2c0a 2020 2020 4e6f 6465 5374  tate,.    NodeSt
+00000840: 6174 7573 2c0a 2020 2020 4e6f 6465 5469  atus,.    NodeTi
+00000850: 6d69 6e67 2c0a 2020 2020 4e6f 6465 5479  ming,.    NodeTy
+00000860: 7065 5265 7370 6f6e 7365 2c0a 2020 2020  peResponse,.    
+00000870: 4e6f 6465 5479 7065 732c 0a20 2020 204e  NodeTypes,.    N
+00000880: 6f64 6555 7365 7243 6f6c 756d 6e73 5265  odeUserColumnsRe
+00000890: 7370 6f6e 7365 2c0a 2020 2020 5072 6574  sponse,.    Pret
+000008a0: 7479 5265 7370 6f6e 7365 2c0a 2020 2020  tyResponse,.    
+000008b0: 5075 744e 6f64 6542 6c6f 622c 0a20 2020  PutNodeBlob,.   
+000008c0: 2051 7565 7565 4d6f 6465 2c0a 2020 2020   QueueMode,.    
+000008d0: 5175 6575 6553 7461 7473 5265 7370 6f6e  QueueStatsRespon
+000008e0: 7365 2c0a 2020 2020 5175 6575 6553 7461  se,.    QueueSta
+000008f0: 7475 732c 0a20 2020 2052 6561 644e 6f64  tus,.    ReadNod
+00000900: 652c 0a20 2020 2053 3343 6f6e 6669 672c  e,.    S3Config,
+00000910: 0a20 2020 2053 6574 4e61 6d65 6453 6563  .    SetNamedSec
+00000920: 7265 742c 0a20 2020 2053 6574 7469 6e67  ret,.    Setting
+00000930: 734f 626a 2c0a 2020 2020 5461 736b 5374  sObj,.    TaskSt
+00000940: 6174 7573 2c0a 2020 2020 5469 6d69 6e67  atus,.    Timing
+00000950: 2c0a 2020 2020 5469 6d69 6e67 5265 7375  ,.    TimingResu
+00000960: 6c74 2c0a 2020 2020 5469 6d69 6e67 732c  lt,.    Timings,
+00000970: 0a20 2020 2054 7269 746f 6e4d 6f64 656c  .    TritonModel
+00000980: 7352 6573 706f 6e73 652c 0a20 2020 2055  sResponse,.    U
+00000990: 5249 5072 6566 6978 2c0a 2020 2020 5570  RIPrefix,.    Up
+000009a0: 6c6f 6164 4669 6c65 7352 6573 706f 6e73  loadFilesRespons
+000009b0: 652c 0a20 2020 2055 7365 7244 6167 4465  e,.    UserDagDe
+000009c0: 662c 0a20 2020 2055 5549 4452 6573 706f  f,.    UUIDRespo
+000009d0: 6e73 652c 0a20 2020 2056 6572 7369 6f6e  nse,.    Version
+000009e0: 5265 7370 6f6e 7365 2c0a 2020 2020 576f  Response,.    Wo
+000009f0: 726b 6572 5363 616c 652c 0a29 0a0a 6966  rkerScale,.)..if
+00000a00: 2054 5950 455f 4348 4543 4b49 4e47 3a0a   TYPE_CHECKING:.
+00000a10: 2020 2020 5756 4420 3d20 7765 616b 7265      WVD = weakre
+00000a20: 662e 5765 616b 5661 6c75 6544 6963 7469  f.WeakValueDicti
+00000a30: 6f6e 6172 795b 7374 722c 2027 4461 6748  onary[str, 'DagH
+00000a40: 616e 646c 6527 5d0a 656c 7365 3a0a 2020  andle'].else:.  
+00000a50: 2020 5756 4420 3d20 7765 616b 7265 662e    WVD = weakref.
+00000a60: 5765 616b 5661 6c75 6544 6963 7469 6f6e  WeakValueDiction
+00000a70: 6172 790a 0a41 5049 5f56 4552 5349 4f4e  ary..API_VERSION
+00000a80: 203d 2035 0a4d 494e 5f41 5049 5f56 4552   = 5.MIN_API_VER
+00000a90: 5349 4f4e 203d 2034 0a44 4546 4155 4c54  SION = 4.DEFAULT
+00000aa0: 5f55 524c 203d 2022 6874 7470 3a2f 2f6c  _URL = "http://l
+00000ab0: 6f63 616c 686f 7374 3a38 3038 3022 0a44  ocalhost:8080".D
+00000ac0: 4546 4155 4c54 5f4e 414d 4553 5041 4345  EFAULT_NAMESPACE
+00000ad0: 203d 2022 6465 6661 756c 7422 0a0a 0a4d   = "default"...M
+00000ae0: 4554 484f 445f 4445 4c45 5445 203d 2022  ETHOD_DELETE = "
+00000af0: 4445 4c45 5445 220a 4d45 5448 4f44 5f46  DELETE".METHOD_F
+00000b00: 494c 4520 3d20 2246 494c 4522 0a4d 4554  ILE = "FILE".MET
+00000b10: 484f 445f 4745 5420 3d20 2247 4554 220a  HOD_GET = "GET".
+00000b20: 4d45 5448 4f44 5f4c 4f4e 4750 4f53 5420  METHOD_LONGPOST 
+00000b30: 3d20 224c 4f4e 4750 4f53 5422 0a4d 4554  = "LONGPOST".MET
+00000b40: 484f 445f 504f 5354 203d 2022 504f 5354  HOD_POST = "POST
+00000b50: 220a 4d45 5448 4f44 5f50 5554 203d 2022  ".METHOD_PUT = "
+00000b60: 5055 5422 0a0a 5052 4546 4958 203d 2022  PUT"..PREFIX = "
+00000b70: 2f78 796d 6522 0a0a 494e 5055 545f 4353  /xyme"..INPUT_CS
+00000b80: 565f 4558 5420 3d20 222e 6373 7622 0a49  V_EXT = ".csv".I
+00000b90: 4e50 5554 5f54 5356 5f45 5854 203d 2022  NPUT_TSV_EXT = "
+00000ba0: 2e74 7376 220a 494e 5055 545f 5a49 505f  .tsv".INPUT_ZIP_
+00000bb0: 4558 5420 3d20 222e 7a69 7022 0a49 4e50  EXT = ".zip".INP
+00000bc0: 5554 5f45 5854 203d 205b 494e 5055 545f  UT_EXT = [INPUT_
+00000bd0: 5a49 505f 4558 542c 2049 4e50 5554 5f43  ZIP_EXT, INPUT_C
+00000be0: 5356 5f45 5854 2c20 494e 5055 545f 5453  SV_EXT, INPUT_TS
+00000bf0: 565f 4558 545d 0a0a 0a46 554e 4320 3d20  V_EXT]...FUNC = 
+00000c00: 4361 6c6c 6162 6c65 5b2e 2e2e 2c20 416e  Callable[..., An
+00000c10: 795d 0a43 5553 544f 4d5f 4e4f 4445 5f54  y].CUSTOM_NODE_T
+00000c20: 5950 4553 203d 207b 0a20 2020 2022 6375  YPES = {.    "cu
+00000c30: 7374 6f6d 5f64 6174 6122 2c0a 2020 2020  stom_data",.    
+00000c40: 2263 7573 746f 6d5f 6a73 6f6e 222c 0a20  "custom_json",. 
+00000c50: 2020 2022 6375 7374 6f6d 5f6a 736f 6e5f     "custom_json_
+00000c60: 746f 5f64 6174 6122 2c0a 2020 2020 2263  to_data",.    "c
+00000c70: 7573 746f 6d5f 6a73 6f6e 5f6a 6f69 6e5f  ustom_json_join_
+00000c80: 6461 7461 222c 0a7d 0a4e 4f5f 5245 5452  data",.}.NO_RETR
+00000c90: 593a 204c 6973 745b 7374 725d 203d 205b  Y: List[str] = [
+00000ca0: 5d20 2023 205b 4d45 5448 4f44 5f50 4f53  ]  # [METHOD_POS
+00000cb0: 542c 204d 4554 484f 445f 4649 4c45 5d0a  T, METHOD_FILE].
+00000cc0: 0a43 4f4e 5355 4d45 525f 4441 4720 3d20  .CONSUMER_DAG = 
+00000cd0: 2264 6167 220a 436f 6e73 756d 6572 5479  "dag".ConsumerTy
+00000ce0: 7065 203d 204c 6974 6572 616c 5b0a 2020  pe = Literal[.  
+00000cf0: 2020 2265 7272 222c 0a20 2020 2022 6572    "err",.    "er
+00000d00: 725f 6d73 6722 2c0a 5d0a 434f 4e53 554d  r_msg",.].CONSUM
+00000d10: 4552 5f45 5252 3a20 436f 6e73 756d 6572  ER_ERR: Consumer
+00000d20: 5479 7065 203d 2022 6572 7222 0a43 4f4e  Type = "err".CON
+00000d30: 5355 4d45 525f 4552 525f 4d53 473a 2043  SUMER_ERR_MSG: C
+00000d40: 6f6e 7375 6d65 7254 7970 6520 3d20 2265  onsumerType = "e
+00000d50: 7272 5f6d 7367 220a 434f 4e53 554d 4552  rr_msg".CONSUMER
+00000d60: 5f54 5950 4553 3a20 5365 745b 436f 6e73  _TYPES: Set[Cons
+00000d70: 756d 6572 5479 7065 5d20 3d20 7365 7428  umerType] = set(
+00000d80: 6765 745f 6172 6773 2843 6f6e 7375 6d65  get_args(Consume
+00000d90: 7254 7970 6529 290a 0a0a 636c 6173 7320  rType))...class 
+00000da0: 4163 6365 7373 4465 6e69 6564 2845 7863  AccessDenied(Exc
+00000db0: 6570 7469 6f6e 293a 0a20 2020 2070 6173  eption):.    pas
+00000dc0: 730a 0a23 202a 2a2a 2041 6363 6573 7344  s..# *** AccessD
+00000dd0: 656e 6965 6420 2a2a 2a0a 0a0a 636c 6173  enied ***...clas
+00000de0: 7320 4c65 6761 6379 5665 7273 696f 6e28  s LegacyVersion(
+00000df0: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+00000e00: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00000e10: 662c 2061 7069 5f76 6572 7369 6f6e 3a20  f, api_version: 
+00000e20: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00000e30: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00000e40: 696e 6974 5f5f 2866 2265 7870 6563 7465  init__(f"expecte
+00000e50: 6420 7b41 5049 5f56 4552 5349 4f4e 7d20  d {API_VERSION} 
+00000e60: 676f 7420 7b61 7069 5f76 6572 7369 6f6e  got {api_version
+00000e70: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
+00000e80: 2e5f 6170 695f 7665 7273 696f 6e20 3d20  ._api_version = 
+00000e90: 6170 695f 7665 7273 696f 6e0a 0a20 2020  api_version..   
+00000ea0: 2064 6566 2067 6574 5f61 7069 5f76 6572   def get_api_ver
+00000eb0: 7369 6f6e 2873 656c 6629 202d 3e20 696e  sion(self) -> in
+00000ec0: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+00000ed0: 6e20 7365 6c66 2e5f 6170 695f 7665 7273  n self._api_vers
+00000ee0: 696f 6e0a 0a23 202a 2a2a 204c 6567 6163  ion..# *** Legac
+00000ef0: 7956 6572 7369 6f6e 202a 2a2a 0a0a 0a63  yVersion ***...c
+00000f00: 6c61 7373 204b 6166 6b61 4572 726f 724d  lass KafkaErrorM
+00000f10: 6573 7361 6765 5374 6174 653a 0a20 2020  essageState:.   
+00000f20: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000f30: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00000f40: 2020 2020 2073 656c 662e 5f6d 7367 5f6c       self._msg_l
+00000f50: 6f6f 6b75 703a 2044 6963 745b 7374 722c  ookup: Dict[str,
+00000f60: 2073 7472 5d20 3d20 7b7d 0a20 2020 2020   str] = {}.     
+00000f70: 2020 2073 656c 662e 5f75 6e6d 6174 6368     self._unmatch
+00000f80: 6564 3a20 4c69 7374 5b73 7472 5d20 3d20  ed: List[str] = 
+00000f90: 5b5d 0a0a 2020 2020 6465 6620 6765 745f  []..    def get_
+00000fa0: 6d73 6728 7365 6c66 2c20 696e 7075 745f  msg(self, input_
+00000fb0: 6964 3a20 7374 7229 202d 3e20 4f70 7469  id: str) -> Opti
+00000fc0: 6f6e 616c 5b73 7472 5d3a 0a20 2020 2020  onal[str]:.     
+00000fd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00000fe0: 6d73 675f 6c6f 6f6b 7570 2e67 6574 2869  msg_lookup.get(i
+00000ff0: 6e70 7574 5f69 6429 0a0a 2020 2020 6465  nput_id)..    de
+00001000: 6620 6164 645f 6d73 6728 7365 6c66 2c20  f add_msg(self, 
+00001010: 696e 7075 745f 6964 3a20 7374 722c 206d  input_id: str, m
+00001020: 7367 3a20 7374 7229 202d 3e20 4e6f 6e65  sg: str) -> None
+00001030: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00001040: 6d73 675f 6c6f 6f6b 7570 5b69 6e70 7574  msg_lookup[input
+00001050: 5f69 645d 203d 206d 7367 0a0a 2020 2020  _id] = msg..    
+00001060: 6465 6620 6765 745f 756e 6d61 7463 6865  def get_unmatche
+00001070: 6428 7365 6c66 2920 2d3e 2049 7465 7261  d(self) -> Itera
+00001080: 626c 655b 7374 725d 3a0a 2020 2020 2020  ble[str]:.      
+00001090: 2020 756e 6d61 7463 6865 6420 3d20 7365    unmatched = se
+000010a0: 6c66 2e5f 756e 6d61 7463 6865 640a 2020  lf._unmatched.  
+000010b0: 2020 2020 2020 7365 6c66 2e5f 756e 6d61        self._unma
+000010c0: 7463 6865 6420 3d20 5b5d 0a20 2020 2020  tched = [].     
+000010d0: 2020 2079 6965 6c64 2066 726f 6d20 756e     yield from un
+000010e0: 6d61 7463 6865 640a 0a20 2020 2064 6566  matched..    def
+000010f0: 2061 6464 5f75 6e6d 6174 6368 6564 2873   add_unmatched(s
+00001100: 656c 662c 206d 7367 3a20 7374 7229 202d  elf, msg: str) -
+00001110: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001120: 7365 6c66 2e5f 756e 6d61 7463 6865 642e  self._unmatched.
+00001130: 6170 7065 6e64 286d 7367 290a 0a23 202a  append(msg)..# *
+00001140: 2a2a 204b 6166 6b61 4572 726f 724d 6573  ** KafkaErrorMes
+00001150: 7361 6765 5374 6174 6520 2a2a 2a0a 0a0a  sageState ***...
+00001160: 636c 6173 7320 5859 4d45 436c 6965 6e74  class XYMEClient
+00001170: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00001180: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+00001190: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+000011a0: 2020 7572 6c3a 2073 7472 2c0a 2020 2020    url: str,.    
+000011b0: 2020 2020 2020 2020 746f 6b65 6e3a 204f          token: O
+000011c0: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+000011d0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
+000011e0: 6163 653a 2073 7472 2920 2d3e 204e 6f6e  ace: str) -> Non
+000011f0: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
+00001200: 5f75 726c 203d 2075 726c 2e72 7374 7269  _url = url.rstri
+00001210: 7028 222f 2229 0a20 2020 2020 2020 2069  p("/").        i
+00001220: 6620 746f 6b65 6e20 6973 204e 6f6e 653a  f token is None:
+00001230: 0a20 2020 2020 2020 2020 2020 2074 6f6b  .            tok
+00001240: 656e 203d 206f 732e 656e 7669 726f 6e2e  en = os.environ.
+00001250: 6765 7428 2258 594d 455f 5345 5256 4552  get("XYME_SERVER
+00001260: 5f54 4f4b 454e 2229 0a20 2020 2020 2020  _TOKEN").       
+00001270: 2073 656c 662e 5f74 6f6b 656e 203d 2074   self._token = t
+00001280: 6f6b 656e 0a20 2020 2020 2020 2073 656c  oken.        sel
+00001290: 662e 5f6e 616d 6573 7061 6365 203d 206e  f._namespace = n
+000012a0: 616d 6573 7061 6365 0a20 2020 2020 2020  amespace.       
+000012b0: 2073 656c 662e 5f6c 6173 745f 6163 7469   self._last_acti
+000012c0: 6f6e 203d 2074 696d 652e 6d6f 6e6f 746f  on = time.monoto
+000012d0: 6e69 6328 290a 2020 2020 2020 2020 7365  nic().        se
+000012e0: 6c66 2e5f 6175 746f 5f72 6566 7265 7368  lf._auto_refresh
+000012f0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00001300: 7365 6c66 2e5f 6461 675f 6361 6368 653a  self._dag_cache:
+00001310: 2057 5644 203d 2077 6561 6b72 6566 2e57   WVD = weakref.W
+00001320: 6561 6b56 616c 7565 4469 6374 696f 6e61  eakValueDictiona
+00001330: 7279 2829 0a20 2020 2020 2020 2073 656c  ry().        sel
+00001340: 662e 5f6e 6f64 655f 6465 6673 3a20 4f70  f._node_defs: Op
+00001350: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00001360: 204e 6f64 6544 6566 496e 666f 5d5d 203d   NodeDefInfo]] =
+00001370: 204e 6f6e 650a 0a20 2020 2020 2020 2064   None..        d
+00001380: 6566 2067 6574 5f76 6572 7369 6f6e 2829  ef get_version()
+00001390: 202d 3e20 5475 706c 655b 696e 742c 2069   -> Tuple[int, i
+000013a0: 6e74 5d3a 0a20 2020 2020 2020 2020 2020  nt]:.           
+000013b0: 2073 6572 7665 725f 7665 7273 696f 6e20   server_version 
+000013c0: 3d20 7365 6c66 2e67 6574 5f73 6572 7665  = self.get_serve
+000013d0: 725f 7665 7273 696f 6e28 290a 2020 2020  r_version().    
+000013e0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000013f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00001400: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+00001410: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
+00001420: 7276 6572 5f76 6572 7369 6f6e 5b22 6170  rver_version["ap
+00001430: 695f 7665 7273 696f 6e22 5d29 2c0a 2020  i_version"]),.  
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 696e 7428 7365 7276 6572 5f76 6572    int(server_ver
+00001460: 7369 6f6e 2e67 6574 2822 6170 695f 7665  sion.get("api_ve
+00001470: 7273 696f 6e5f 6d69 6e6f 7222 2c20 3029  rsion_minor", 0)
+00001480: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00001490: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000014a0: 2065 7863 6570 7420 2856 616c 7565 4572   except (ValueEr
+000014b0: 726f 722c 204b 6579 4572 726f 7229 2061  ror, KeyError) a
+000014c0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+000014d0: 2020 2020 2072 6169 7365 204c 6567 6163       raise Legac
+000014e0: 7956 6572 7369 6f6e 2831 2920 6672 6f6d  yVersion(1) from
+000014f0: 2065 0a0a 2020 2020 2020 2020 6170 695f   e..        api_
+00001500: 7665 7273 696f 6e2c 2061 7069 5f76 6572  version, api_ver
+00001510: 7369 6f6e 5f6d 696e 6f72 203d 2067 6574  sion_minor = get
+00001520: 5f76 6572 7369 6f6e 2829 0a20 2020 2020  _version().     
+00001530: 2020 2069 6620 6170 695f 7665 7273 696f     if api_versio
+00001540: 6e20 3c20 4d49 4e5f 4150 495f 5645 5253  n < MIN_API_VERS
+00001550: 494f 4e3a 0a20 2020 2020 2020 2020 2020  ION:.           
+00001560: 2072 6169 7365 204c 6567 6163 7956 6572   raise LegacyVer
+00001570: 7369 6f6e 2861 7069 5f76 6572 7369 6f6e  sion(api_version
+00001580: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00001590: 6170 695f 7665 7273 696f 6e20 3d20 6170  api_version = ap
+000015a0: 695f 7665 7273 696f 6e0a 2020 2020 2020  i_version.      
+000015b0: 2020 7365 6c66 2e5f 6170 695f 7665 7273    self._api_vers
+000015c0: 696f 6e5f 6d69 6e6f 7220 3d20 6170 695f  ion_minor = api_
+000015d0: 7665 7273 696f 6e5f 6d69 6e6f 720a 0a20  version_minor.. 
+000015e0: 2020 2064 6566 2067 6574 5f61 7069 5f76     def get_api_v
+000015f0: 6572 7369 6f6e 2873 656c 6629 202d 3e20  ersion(self) -> 
+00001600: 696e 743a 0a20 2020 2020 2020 2072 6574  int:.        ret
+00001610: 7572 6e20 7365 6c66 2e5f 6170 695f 7665  urn self._api_ve
+00001620: 7273 696f 6e0a 0a20 2020 2064 6566 2067  rsion..    def g
+00001630: 6574 5f61 7069 5f76 6572 7369 6f6e 5f6d  et_api_version_m
+00001640: 696e 6f72 2873 656c 6629 202d 3e20 696e  inor(self) -> in
+00001650: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+00001660: 6e20 7365 6c66 2e5f 6170 695f 7665 7273  n self._api_vers
+00001670: 696f 6e5f 6d69 6e6f 720a 0a20 2020 2064  ion_minor..    d
+00001680: 6566 2068 6173 5f76 6572 7369 6f6e 2873  ef has_version(s
+00001690: 656c 662c 206d 616a 6f72 3a20 696e 742c  elf, major: int,
+000016a0: 206d 696e 6f72 3a20 696e 7429 202d 3e20   minor: int) -> 
+000016b0: 626f 6f6c 3a0a 2020 2020 2020 2020 6966  bool:.        if
+000016c0: 2073 656c 662e 5f61 7069 5f76 6572 7369   self._api_versi
+000016d0: 6f6e 203e 206d 616a 6f72 3a0a 2020 2020  on > major:.    
+000016e0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+000016f0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00001700: 726e 2073 656c 662e 5f61 7069 5f76 6572  rn self._api_ver
+00001710: 7369 6f6e 203d 3d20 6d61 6a6f 7220 616e  sion == major an
+00001720: 6420 7365 6c66 2e5f 6170 695f 7665 7273  d self._api_vers
+00001730: 696f 6e5f 6d69 6e6f 7220 3e3d 206d 696e  ion_minor >= min
+00001740: 6f72 0a0a 2020 2020 6465 6620 7365 745f  or..    def set_
+00001750: 6175 746f 5f72 6566 7265 7368 2873 656c  auto_refresh(sel
+00001760: 662c 2069 735f 6175 746f 5f72 6566 7265  f, is_auto_refre
+00001770: 7368 3a20 626f 6f6c 2920 2d3e 204e 6f6e  sh: bool) -> Non
+00001780: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
+00001790: 5f61 7574 6f5f 7265 6672 6573 6820 3d20  _auto_refresh = 
+000017a0: 6973 5f61 7574 6f5f 7265 6672 6573 680a  is_auto_refresh.
+000017b0: 0a20 2020 2064 6566 2069 735f 6175 746f  .    def is_auto
+000017c0: 5f72 6566 7265 7368 2873 656c 6629 202d  _refresh(self) -
+000017d0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+000017e0: 7265 7475 726e 2073 656c 662e 5f61 7574  return self._aut
+000017f0: 6f5f 7265 6672 6573 680a 0a20 2020 2064  o_refresh..    d
+00001800: 6566 2072 6566 7265 7368 2873 656c 6629  ef refresh(self)
+00001810: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00001820: 2020 7365 6c66 2e5f 6e6f 6465 5f64 6566    self._node_def
+00001830: 7320 3d20 4e6f 6e65 0a0a 2020 2020 6465  s = None..    de
+00001840: 6620 5f6d 6179 6265 5f72 6566 7265 7368  f _maybe_refresh
+00001850: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00001860: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00001870: 6973 5f61 7574 6f5f 7265 6672 6573 6828  is_auto_refresh(
+00001880: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00001890: 656c 662e 7265 6672 6573 6828 290a 0a20  elf.refresh().. 
+000018a0: 2020 2023 2046 4958 4d45 3a20 446f 2077     # FIXME: Do w
+000018b0: 6520 7374 696c 6c20 6e65 6564 2074 6869  e still need thi
+000018c0: 733f 0a20 2020 2040 636f 6e74 6578 746c  s?.    @contextl
+000018d0: 6962 2e63 6f6e 7465 7874 6d61 6e61 6765  ib.contextmanage
+000018e0: 720a 2020 2020 6465 6620 6275 6c6b 5f6f  r.    def bulk_o
+000018f0: 7065 7261 7469 6f6e 2873 656c 6629 202d  peration(self) -
+00001900: 3e20 4974 6572 6174 6f72 5b62 6f6f 6c5d  > Iterator[bool]
+00001910: 3a0a 2020 2020 2020 2020 6f6c 645f 7265  :.        old_re
+00001920: 6672 6573 6820 3d20 7365 6c66 2e69 735f  fresh = self.is_
+00001930: 6175 746f 5f72 6566 7265 7368 2829 0a20  auto_refresh(). 
+00001940: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00001950: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00001960: 5f61 7574 6f5f 7265 6672 6573 6828 4661  _auto_refresh(Fa
+00001970: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00001980: 2079 6965 6c64 206f 6c64 5f72 6566 7265   yield old_refre
+00001990: 7368 0a20 2020 2020 2020 2066 696e 616c  sh.        final
+000019a0: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
+000019b0: 7365 6c66 2e73 6574 5f61 7574 6f5f 7265  self.set_auto_re
+000019c0: 6672 6573 6828 6f6c 645f 7265 6672 6573  fresh(old_refres
+000019d0: 6829 0a0a 2020 2020 6465 6620 5f72 6177  h)..    def _raw
+000019e0: 5f72 6571 7565 7374 5f62 7974 6573 280a  _request_bytes(.
+000019f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001a00: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00001a10: 7468 6f64 3a20 7374 722c 0a20 2020 2020  thod: str,.     
+00001a20: 2020 2020 2020 2070 6174 683a 2073 7472         path: str
+00001a30: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00001a40: 6773 3a20 4469 6374 5b73 7472 2c20 416e  gs: Dict[str, An
+00001a50: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
+00001a60: 6669 6c65 733a 204f 7074 696f 6e61 6c5b  files: Optional[
+00001a70: 4469 6374 5b73 7472 2c20 4279 7465 7349  Dict[str, BytesI
+00001a80: 4f5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  O]] = None,.    
+00001a90: 2020 2020 2020 2020 6164 645f 7072 6566          add_pref
+00001aa0: 6978 3a20 626f 6f6c 203d 2054 7275 652c  ix: bool = True,
+00001ab0: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+00001ac0: 5f6e 616d 6573 7061 6365 3a20 626f 6f6c  _namespace: bool
+00001ad0: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00001ae0: 2020 2020 2061 7069 5f76 6572 7369 6f6e       api_version
+00001af0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00001b00: 3d20 4e6f 6e65 2920 2d3e 2054 7570 6c65  = None) -> Tuple
+00001b10: 5b42 7974 6573 494f 2c20 7374 725d 3a0a  [BytesIO, str]:.
+00001b20: 2020 2020 2020 2020 6669 6c65 5f72 6573          file_res
+00001b30: 6574 7320 3d20 7b7d 0a20 2020 2020 2020  ets = {}.       
+00001b40: 2063 616e 5f72 6573 6574 203d 2054 7275   can_reset = Tru
+00001b50: 650a 2020 2020 2020 2020 6966 2066 696c  e.        if fil
+00001b60: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+00001b70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001b80: 2866 6e61 6d65 2c20 6662 7566 6629 2069  (fname, fbuff) i
+00001b90: 6e20 6669 6c65 732e 6974 656d 7328 293a  n files.items():
+00001ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001bb0: 2069 6620 6861 7361 7474 7228 6662 7566   if hasattr(fbuf
+00001bc0: 662c 2022 7365 656b 2229 3a0a 2020 2020  f, "seek"):.    
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 6669 6c65 5f72 6573 6574 735b 666e 616d  file_resets[fnam
+00001bf0: 655d 203d 2066 6275 6666 2e73 6565 6b28  e] = fbuff.seek(
+00001c00: 302c 2069 6f2e 5345 454b 5f43 5552 290a  0, io.SEEK_CUR).
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001c30: 2020 2020 2020 2020 2020 6361 6e5f 7265            can_re
+00001c40: 7365 7420 3d20 4661 6c73 650a 0a20 2020  set = False..   
+00001c50: 2020 2020 2064 6566 2072 6573 6574 5f66       def reset_f
+00001c60: 696c 6573 2829 202d 3e20 626f 6f6c 3a0a  iles() -> bool:.
+00001c70: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00001c80: 696c 6573 2069 7320 4e6f 6e65 3a0a 2020  iles is None:.  
+00001c90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001ca0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00001cb0: 2020 2020 2020 6966 206e 6f74 2063 616e        if not can
+00001cc0: 5f72 6573 6574 3a0a 2020 2020 2020 2020  _reset:.        
+00001cd0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00001ce0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00001cf0: 2066 6f72 2028 666e 616d 652c 2070 6f73   for (fname, pos
+00001d00: 2920 696e 2066 696c 655f 7265 7365 7473  ) in file_resets
+00001d10: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00001d20: 2020 2020 2020 2020 2020 6669 6c65 735b            files[
+00001d30: 666e 616d 655d 2e73 6565 6b28 706f 732c  fname].seek(pos,
+00001d40: 2069 6f2e 5345 454b 5f53 4554 290a 2020   io.SEEK_SET).  
+00001d50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001d60: 2054 7275 650a 0a20 2020 2020 2020 2072   True..        r
+00001d70: 6574 7279 203d 2030 0a20 2020 2020 2020  etry = 0.       
+00001d80: 206d 6178 5f72 6574 7279 203d 2067 6574   max_retry = get
+00001d90: 5f6d 6178 5f72 6574 7279 2829 0a20 2020  _max_retry().   
+00001da0: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
+00001db0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00001dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001dd0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00001de0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001df0: 6e20 7365 6c66 2e5f 6661 6c6c 6962 6c65  n self._fallible
+00001e00: 5f72 6177 5f72 6571 7565 7374 5f62 7974  _raw_request_byt
+00001e10: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00001e20: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+00001e30: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
+00001e40: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00001e50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001e60: 2020 2020 2020 2020 2020 6172 6773 2c0a            args,.
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e80: 2020 2020 2020 2020 6669 6c65 732c 0a20          files,. 
+00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 2020 2020 2020 2061 6464 5f70 7265 6669         add_prefi
+00001eb0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+00001ec0: 2020 2020 2020 2020 2020 2061 6464 5f6e             add_n
+00001ed0: 616d 6573 7061 6365 2c0a 2020 2020 2020  amespace,.      
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 2020 6170 695f 7665 7273 696f 6e29 0a20    api_version). 
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00001f10: 7863 6570 7420 4854 5450 4572 726f 7220  xcept HTTPError 
+00001f20: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00001f30: 2020 2020 2020 2020 2020 6966 2065 2e72            if e.r
+00001f40: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
+00001f50: 6f64 6520 696e 2028 3430 332c 2034 3034  ode in (403, 404
+00001f60: 2c20 3530 3029 3a0a 2020 2020 2020 2020  , 500):.        
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f80: 7265 7472 7920 3d20 6d61 785f 7265 7472  retry = max_retr
+00001f90: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+00001fa0: 2020 2020 2020 7261 6973 6520 650a 2020        raise e.  
+00001fb0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00001fc0: 2052 6571 7565 7374 4578 6365 7074 696f   RequestExceptio
+00001fd0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00001fe0: 2020 2069 6620 7265 7472 7920 3e3d 206d     if retry >= m
+00001ff0: 6178 5f72 6574 7279 3a0a 2020 2020 2020  ax_retry:.      
+00002000: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002010: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
+00002020: 2020 2020 6966 206e 6f74 2072 6573 6574      if not reset
+00002030: 5f66 696c 6573 2829 3a0a 2020 2020 2020  _files():.      
+00002040: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002050: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
+00002060: 2020 2020 6966 206d 6574 686f 6420 696e      if method in
+00002070: 204e 4f5f 5245 5452 593a 0a20 2020 2020   NO_RETRY:.     
+00002080: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002090: 6169 7365 0a20 2020 2020 2020 2020 2020  aise.           
+000020a0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+000020b0: 6765 745f 7265 7472 795f 736c 6565 7028  get_retry_sleep(
+000020c0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+000020d0: 6574 7279 202b 3d20 310a 0a20 2020 2064  etry += 1..    d
+000020e0: 6566 205f 7261 775f 7265 7175 6573 745f  ef _raw_request_
+000020f0: 7374 7228 0a20 2020 2020 2020 2020 2020  str(.           
+00002100: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00002110: 2020 206d 6574 686f 643a 2073 7472 2c0a     method: str,.
+00002120: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00002130: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
+00002140: 2020 2061 7267 733a 2044 6963 745b 7374     args: Dict[st
+00002150: 722c 2041 6e79 5d2c 0a20 2020 2020 2020  r, Any],.       
+00002160: 2020 2020 2061 6464 5f70 7265 6669 783a       add_prefix:
+00002170: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+00002180: 2020 2020 2020 2020 2020 6164 645f 6e61            add_na
+00002190: 6d65 7370 6163 653a 2062 6f6f 6c20 3d20  mespace: bool = 
+000021a0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000021b0: 2020 6170 695f 7665 7273 696f 6e3a 204f    api_version: O
+000021c0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000021d0: 6f6e 6529 202d 3e20 5465 7874 494f 3a0a  one) -> TextIO:.
+000021e0: 2020 2020 2020 2020 7265 7472 7920 3d20          retry = 
+000021f0: 300a 2020 2020 2020 2020 6d61 785f 7265  0.        max_re
+00002200: 7472 7920 3d20 6765 745f 6d61 785f 7265  try = get_max_re
+00002210: 7472 7928 290a 2020 2020 2020 2020 7768  try().        wh
+00002220: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+00002230: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00002240: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002270: 5f66 616c 6c69 626c 655f 7261 775f 7265  _fallible_raw_re
+00002280: 7175 6573 745f 7374 7228 0a20 2020 2020  quest_str(.     
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 206d 6574 686f 642c 0a20 2020 2020     method,.     
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2070 6174 682c 0a20 2020 2020 2020     path,.       
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2061 7267 732c 0a20 2020 2020 2020 2020   args,.         
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002300: 6464 5f70 7265 6669 782c 0a20 2020 2020  dd_prefix,.     
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2020 2061 6464 5f6e 616d 6573 7061 6365     add_namespace
+00002330: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002340: 2020 2020 2020 2020 2020 6170 695f 7665            api_ve
+00002350: 7273 696f 6e29 0a20 2020 2020 2020 2020  rsion).         
+00002360: 2020 2020 2020 2065 7863 6570 7420 4854         except HT
+00002370: 5450 4572 726f 7220 6173 2065 3a0a 2020  TPError as e:.  
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 6966 2065 2e72 6573 706f 6e73 652e    if e.response.
+000023a0: 7374 6174 7573 5f63 6f64 6520 696e 2028  status_code in (
+000023b0: 3430 332c 2034 3034 2c20 3530 3029 3a0a  403, 404, 500):.
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 2020 2020 2020 2020 7265 7472 7920 3d20          retry = 
+000023e0: 6d61 785f 7265 7472 790a 2020 2020 2020  max_retry.      
+000023f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002400: 6973 6520 650a 2020 2020 2020 2020 2020  ise e.          
+00002410: 2020 6578 6365 7074 2052 6571 7565 7374    except Request
+00002420: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
+00002430: 2020 2020 2020 2020 2020 2069 6620 6d65             if me
+00002440: 7468 6f64 2069 6e20 4e4f 5f52 4554 5259  thod in NO_RETRY
+00002450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002460: 2020 2020 2020 7261 6973 650a 2020 2020        raise.    
+00002470: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00002480: 6574 7279 203e 3d20 6d61 785f 7265 7472  etry >= max_retr
+00002490: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+000024a0: 2020 2020 2020 2072 6169 7365 0a20 2020         raise.   
+000024b0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+000024c0: 652e 736c 6565 7028 6765 745f 7265 7472  e.sleep(get_retr
+000024d0: 795f 736c 6565 7028 2929 0a20 2020 2020  y_sleep()).     
+000024e0: 2020 2020 2020 2072 6574 7279 202b 3d20         retry += 
+000024f0: 310a 0a20 2020 2064 6566 205f 7261 775f  1..    def _raw_
+00002500: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
+00002510: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+00002520: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+00002530: 6f64 3a20 7374 722c 0a20 2020 2020 2020  od: str,.       
+00002540: 2020 2020 2070 6174 683a 2073 7472 2c0a       path: str,.
+00002550: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00002560: 3a20 4469 6374 5b73 7472 2c20 416e 795d  : Dict[str, Any]
+00002570: 2c0a 2020 2020 2020 2020 2020 2020 6164  ,.            ad
+00002580: 645f 7072 6566 6978 3a20 626f 6f6c 203d  d_prefix: bool =
+00002590: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+000025a0: 2020 2061 6464 5f6e 616d 6573 7061 6365     add_namespace
+000025b0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+000025c0: 2020 2020 2020 2020 2020 2066 696c 6573             files
+000025d0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+000025e0: 7374 722c 2049 4f5b 6279 7465 735d 5d5d  str, IO[bytes]]]
+000025f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00002600: 2020 2020 2061 7069 5f76 6572 7369 6f6e       api_version
+00002610: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00002620: 3d20 4e6f 6e65 2920 2d3e 2044 6963 745b  = None) -> Dict[
+00002630: 7374 722c 2041 6e79 5d3a 0a20 2020 2020  str, Any]:.     
+00002640: 2020 2066 696c 655f 7265 7365 7473 203d     file_resets =
+00002650: 207b 7d0a 2020 2020 2020 2020 6361 6e5f   {}.        can_
+00002660: 7265 7365 7420 3d20 5472 7565 0a20 2020  reset = True.   
+00002670: 2020 2020 2069 6620 6669 6c65 7320 6973       if files is
+00002680: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00002690: 2020 2020 2020 2066 6f72 2028 666e 616d         for (fnam
+000026a0: 652c 2066 6275 6666 2920 696e 2066 696c  e, fbuff) in fil
+000026b0: 6573 2e69 7465 6d73 2829 3a0a 2020 2020  es.items():.    
+000026c0: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+000026d0: 6173 6174 7472 2866 6275 6666 2c20 2273  asattr(fbuff, "s
+000026e0: 6565 6b22 293a 0a20 2020 2020 2020 2020  eek"):.         
+000026f0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+00002700: 7265 7365 7473 5b66 6e61 6d65 5d20 3d20  resets[fname] = 
+00002710: 6662 7566 662e 7365 656b 2830 2c20 696f  fbuff.seek(0, io
+00002720: 2e53 4545 4b5f 4355 5229 0a20 2020 2020  .SEEK_CUR).     
+00002730: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 2020 2020 2063 616e 5f72 6573 6574 203d       can_reset =
+00002760: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00002770: 6465 6620 7265 7365 745f 6669 6c65 7328  def reset_files(
+00002780: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00002790: 2020 2020 2020 2069 6620 6669 6c65 7320         if files 
+000027a0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000027b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000027c0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+000027d0: 2069 6620 6e6f 7420 6361 6e5f 7265 7365   if not can_rese
+000027e0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+000027f0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00002800: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002810: 2866 6e61 6d65 2c20 706f 7329 2069 6e20  (fname, pos) in 
+00002820: 6669 6c65 5f72 6573 6574 732e 6974 656d  file_resets.item
+00002830: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00002840: 2020 2020 2066 696c 6573 5b66 6e61 6d65       files[fname
+00002850: 5d2e 7365 656b 2870 6f73 2c20 696f 2e53  ].seek(pos, io.S
+00002860: 4545 4b5f 5345 5429 0a20 2020 2020 2020  EEK_SET).       
+00002870: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00002880: 0a0a 2020 2020 2020 2020 7265 7472 7920  ..        retry 
+00002890: 3d20 300a 2020 2020 2020 2020 6d61 785f  = 0.        max_
+000028a0: 7265 7472 7920 3d20 6765 745f 6d61 785f  retry = get_max_
+000028b0: 7265 7472 7928 290a 2020 2020 2020 2020  retry().        
+000028c0: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+000028d0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000028e0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+000028f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002900: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002910: 662e 5f66 616c 6c69 626c 655f 7261 775f  f._fallible_raw_
+00002920: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 2020 6d65 7468 6f64 2c0a 2020        method,.  
+00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002960: 2020 2020 2020 7061 7468 2c0a 2020 2020        path,.    
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 2020 2020 6172 6773 2c0a 2020 2020 2020      args,.      
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 2020 6164 645f 7072 6566 6978 2c0a 2020    add_prefix,.  
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2020 2020 6164 645f 6e61 6d65 7370        add_namesp
+000029d0: 6163 652c 0a20 2020 2020 2020 2020 2020  ace,.           
+000029e0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000029f0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00002a00: 2020 2020 2020 2020 2020 2020 6170 695f              api_
+00002a10: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
+00002a20: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00002a30: 4854 5450 4572 726f 7220 6173 2065 3a0a  HTTPError as e:.
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 2020 2020 6966 2065 2e72 6573 706f 6e73      if e.respons
+00002a60: 652e 7374 6174 7573 5f63 6f64 6520 696e  e.status_code in
+00002a70: 2028 3430 332c 2034 3034 2c20 3530 3029   (403, 404, 500)
+00002a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002a90: 2020 2020 2020 2020 2020 7265 7472 7920            retry 
+00002aa0: 3d20 6d61 785f 7265 7472 790a 2020 2020  = max_retry.    
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 7261 6973 6520 650a 2020 2020 2020 2020  raise e.        
+00002ad0: 2020 2020 6578 6365 7074 2052 6571 7565      except Reque
+00002ae0: 7374 4578 6365 7074 696f 6e3a 0a20 2020  stException:.   
+00002af0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002b00: 7265 7472 7920 3e3d 206d 6178 5f72 6574  retry >= max_ret
+00002b10: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00002b20: 2020 2020 2020 2020 7261 6973 650a 2020          raise.  
+00002b30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002b40: 206e 6f74 2072 6573 6574 5f66 696c 6573   not reset_files
+00002b50: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00002b60: 2020 2020 2020 2020 7261 6973 650a 2020          raise.  
+00002b70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002b80: 206d 6574 686f 6420 696e 204e 4f5f 5245   method in NO_RE
+00002b90: 5452 593a 0a20 2020 2020 2020 2020 2020  TRY:.           
+00002ba0: 2020 2020 2020 2020 2072 6169 7365 0a20           raise. 
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00002bc0: 696d 652e 736c 6565 7028 6765 745f 7265  ime.sleep(get_re
+00002bd0: 7472 795f 736c 6565 7028 2929 0a20 2020  try_sleep()).   
+00002be0: 2020 2020 2020 2020 2072 6574 7279 202b           retry +
+00002bf0: 3d20 310a 0a20 2020 2064 6566 205f 6661  = 1..    def _fa
+00002c00: 6c6c 6962 6c65 5f72 6177 5f72 6571 7565  llible_raw_reque
+00002c10: 7374 5f62 7974 6573 280a 2020 2020 2020  st_bytes(.      
+00002c20: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00002c30: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+00002c40: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+00002c50: 2070 6174 683a 2073 7472 2c0a 2020 2020   path: str,.    
+00002c60: 2020 2020 2020 2020 6172 6773 3a20 4469          args: Di
+00002c70: 6374 5b73 7472 2c20 416e 795d 2c0a 2020  ct[str, Any],.  
+00002c80: 2020 2020 2020 2020 2020 6669 6c65 733a            files:
+00002c90: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00002ca0: 7472 2c20 4279 7465 7349 4f5d 5d2c 0a20  tr, BytesIO]],. 
+00002cb0: 2020 2020 2020 2020 2020 2061 6464 5f70             add_p
+00002cc0: 7265 6669 783a 2062 6f6f 6c2c 0a20 2020  refix: bool,.   
+00002cd0: 2020 2020 2020 2020 2061 6464 5f6e 616d           add_nam
+00002ce0: 6573 7061 6365 3a20 626f 6f6c 2c0a 2020  espace: bool,.  
+00002cf0: 2020 2020 2020 2020 2020 6170 695f 7665            api_ve
+00002d00: 7273 696f 6e3a 204f 7074 696f 6e61 6c5b  rsion: Optional[
+00002d10: 696e 745d 2920 2d3e 2054 7570 6c65 5b42  int]) -> Tuple[B
+00002d20: 7974 6573 494f 2c20 7374 725d 3a0a 2020  ytesIO, str]:.  
+00002d30: 2020 2020 2020 7072 6566 6978 203d 2022        prefix = "
+00002d40: 220a 2020 2020 2020 2020 6966 2061 6464  ".        if add
+00002d50: 5f70 7265 6669 783a 0a20 2020 2020 2020  _prefix:.       
+00002d60: 2020 2020 2069 6620 6170 695f 7665 7273       if api_vers
+00002d70: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00002d80: 2020 2020 2020 2020 2020 2020 2061 7069               api
+00002d90: 5f76 6572 7369 6f6e 203d 2073 656c 662e  _version = self.
+00002da0: 5f61 7069 5f76 6572 7369 6f6e 0a20 2020  _api_version.   
+00002db0: 2020 2020 2020 2020 2070 7265 6669 7820           prefix 
+00002dc0: 3d20 6622 7b50 5245 4649 587d 2f76 7b61  = f"{PREFIX}/v{a
+00002dd0: 7069 5f76 6572 7369 6f6e 7d22 0a20 2020  pi_version}".   
+00002de0: 2020 2020 2075 726c 203d 2066 227b 7365       url = f"{se
+00002df0: 6c66 2e5f 7572 6c7d 7b70 7265 6669 787d  lf._url}{prefix}
+00002e00: 7b70 6174 687d 220a 2020 2020 2020 2020  {path}".        
+00002e10: 6865 6164 6572 7320 3d20 7b0a 2020 2020  headers = {.    
+00002e20: 2020 2020 2020 2020 2261 7574 686f 7269          "authori
+00002e30: 7a61 7469 6f6e 223a 2073 656c 662e 5f74  zation": self._t
+00002e40: 6f6b 656e 2c0a 2020 2020 2020 2020 7d0a  oken,.        }.
+00002e50: 2020 2020 2020 2020 6966 2061 6464 5f6e          if add_n
+00002e60: 616d 6573 7061 6365 3a0a 2020 2020 2020  amespace:.      
+00002e70: 2020 2020 2020 6172 6773 5b22 6e61 6d65        args["name
+00002e80: 7370 6163 6522 5d20 3d20 7365 6c66 2e5f  space"] = self._
+00002e90: 6e61 6d65 7370 6163 650a 0a20 2020 2020  namespace..     
+00002ea0: 2020 2064 6566 2063 6865 636b 5f65 7272     def check_err
+00002eb0: 6f72 2872 6571 3a20 5265 7370 6f6e 7365  or(req: Response
+00002ec0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00002ed0: 2020 2020 2020 2069 6620 7265 712e 7374         if req.st
+00002ee0: 6174 7573 5f63 6f64 6520 3d3d 2034 3033  atus_code == 403
+00002ef0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002f00: 2020 7261 6973 6520 4163 6365 7373 4465    raise AccessDe
+00002f10: 6e69 6564 2872 6571 2e74 6578 7429 0a20  nied(req.text). 
+00002f20: 2020 2020 2020 2020 2020 2072 6571 2e72             req.r
+00002f30: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
+00002f40: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00002f50: 4e4f 5445 3a20 6e6f 2063 6f6e 7465 6e74  NOTE: no content
+00002f60: 2074 7970 6520 6368 6563 6b20 2d2d 2077   type check -- w
+00002f70: 696c 6c20 6265 2068 616e 646c 6564 2062  ill be handled b
+00002f80: 7920 696e 7465 7270 7265 745f 6374 7970  y interpret_ctyp
+00002f90: 650a 0a20 2020 2020 2020 2069 6620 6d65  e..        if me
+00002fa0: 7468 6f64 203d 3d20 4d45 5448 4f44 5f47  thod == METHOD_G
+00002fb0: 4554 3a0a 2020 2020 2020 2020 2020 2020  ET:.            
+00002fc0: 7265 7120 3d20 7265 7175 6573 7473 2e67  req = requests.g
+00002fd0: 6574 2875 726c 2c20 7061 7261 6d73 3d61  et(url, params=a
+00002fe0: 7267 732c 2068 6561 6465 7273 3d68 6561  rgs, headers=hea
+00002ff0: 6465 7273 290a 2020 2020 2020 2020 2020  ders).          
+00003000: 2020 6368 6563 6b5f 6572 726f 7228 7265    check_error(re
+00003010: 7129 0a20 2020 2020 2020 2020 2020 2072  q).            r
+00003020: 6574 7572 6e20 4279 7465 7349 4f28 7265  eturn BytesIO(re
+00003030: 712e 636f 6e74 656e 7429 2c20 7265 712e  q.content), req.
+00003040: 6865 6164 6572 735b 2263 6f6e 7465 6e74  headers["content
+00003050: 2d74 7970 6522 5d0a 2020 2020 2020 2020  -type"].        
+00003060: 6966 206d 6574 686f 6420 3d3d 204d 4554  if method == MET
+00003070: 484f 445f 504f 5354 3a0a 2020 2020 2020  HOD_POST:.      
+00003080: 2020 2020 2020 7265 7120 3d20 7265 7175        req = requ
+00003090: 6573 7473 2e70 6f73 7428 7572 6c2c 206a  ests.post(url, j
+000030a0: 736f 6e3d 6172 6773 2c20 6865 6164 6572  son=args, header
+000030b0: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
+000030c0: 2020 2020 2020 2063 6865 636b 5f65 7272         check_err
+000030d0: 6f72 2872 6571 290a 2020 2020 2020 2020  or(req).        
+000030e0: 2020 2020 7265 7475 726e 2042 7974 6573      return Bytes
+000030f0: 494f 2872 6571 2e63 6f6e 7465 6e74 292c  IO(req.content),
+00003100: 2072 6571 2e68 6561 6465 7273 5b22 636f   req.headers["co
+00003110: 6e74 656e 742d 7479 7065 225d 0a20 2020  ntent-type"].   
+00003120: 2020 2020 2069 6620 6d65 7468 6f64 203d       if method =
+00003130: 3d20 4d45 5448 4f44 5f46 494c 453a 0a20  = METHOD_FILE:. 
+00003140: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
+00003150: 6c65 7320 6973 204e 6f6e 653a 0a20 2020  les is None:.   
+00003160: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00003170: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00003180: 6669 6c65 206d 6574 686f 6420 6d75 7374  file method must
+00003190: 2068 6176 6520 6669 6c65 733a 207b 6669   have files: {fi
+000031a0: 6c65 737d 2229 0a20 2020 2020 2020 2020  les}").         
+000031b0: 2020 2072 6571 203d 2072 6571 7565 7374     req = request
+000031c0: 732e 706f 7374 280a 2020 2020 2020 2020  s.post(.        
+000031d0: 2020 2020 2020 2020 7572 6c2c 0a20 2020          url,.   
+000031e0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+000031f0: 613d 6172 6773 2c0a 2020 2020 2020 2020  a=args,.        
+00003200: 2020 2020 2020 2020 6669 6c65 733d 7b0a          files={.
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 2020 2020 6b65 793a 2028 0a20 2020 2020      key: (.     
+00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003240: 2020 2067 6574 6174 7472 2876 616c 7565     getattr(value
+00003250: 2c20 226e 616d 6522 2c20 6b65 7929 2c0a  , "name", key),.
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 2020 2020 2020 2020 7661 6c75 652c 0a20          value,. 
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
+000032a0: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
+000032b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000032c0: 2020 2020 2020 2029 2066 6f72 2028 6b65         ) for (ke
+000032d0: 792c 2076 616c 7565 2920 696e 2066 696c  y, value) in fil
+000032e0: 6573 2e69 7465 6d73 2829 0a20 2020 2020  es.items().     
+000032f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00003300: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00003310: 6164 6572 733d 6865 6164 6572 7329 0a20  aders=headers). 
+00003320: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00003330: 5f65 7272 6f72 2872 6571 290a 2020 2020  _error(req).    
+00003340: 2020 2020 2020 2020 7265 7475 726e 2042          return B
+00003350: 7974 6573 494f 2872 6571 2e63 6f6e 7465  ytesIO(req.conte
+00003360: 6e74 292c 2072 6571 2e68 6561 6465 7273  nt), req.headers
+00003370: 5b22 636f 6e74 656e 742d 7479 7065 225d  ["content-type"]
+00003380: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00003390: 616c 7565 4572 726f 7228 6622 756e 6b6e  alueError(f"unkn
+000033a0: 6f77 6e20 6d65 7468 6f64 207b 6d65 7468  own method {meth
+000033b0: 6f64 7d22 290a 0a20 2020 2064 6566 205f  od}")..    def _
+000033c0: 6661 6c6c 6962 6c65 5f72 6177 5f72 6571  fallible_raw_req
+000033d0: 7565 7374 5f73 7472 280a 2020 2020 2020  uest_str(.      
+000033e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000033f0: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+00003400: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+00003410: 2070 6174 683a 2073 7472 2c0a 2020 2020   path: str,.    
+00003420: 2020 2020 2020 2020 6172 6773 3a20 4469          args: Di
+00003430: 6374 5b73 7472 2c20 416e 795d 2c0a 2020  ct[str, Any],.  
+00003440: 2020 2020 2020 2020 2020 6164 645f 7072            add_pr
+00003450: 6566 6978 3a20 626f 6f6c 2c0a 2020 2020  efix: bool,.    
+00003460: 2020 2020 2020 2020 6164 645f 6e61 6d65          add_name
+00003470: 7370 6163 653a 2062 6f6f 6c2c 0a20 2020  space: bool,.   
+00003480: 2020 2020 2020 2020 2061 7069 5f76 6572           api_ver
+00003490: 7369 6f6e 3a20 4f70 7469 6f6e 616c 5b69  sion: Optional[i
+000034a0: 6e74 5d29 202d 3e20 5465 7874 494f 3a0a  nt]) -> TextIO:.
+000034b0: 2020 2020 2020 2020 7072 6566 6978 203d          prefix =
+000034c0: 2022 220a 2020 2020 2020 2020 6966 2061   "".        if a
+000034d0: 6464 5f70 7265 6669 783a 0a20 2020 2020  dd_prefix:.     
+000034e0: 2020 2020 2020 2069 6620 6170 695f 7665         if api_ve
+000034f0: 7273 696f 6e20 6973 204e 6f6e 653a 0a20  rsion is None:. 
+00003500: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003510: 7069 5f76 6572 7369 6f6e 203d 2073 656c  pi_version = sel
+00003520: 662e 5f61 7069 5f76 6572 7369 6f6e 0a20  f._api_version. 
+00003530: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00003540: 7820 3d20 6622 7b50 5245 4649 587d 2f76  x = f"{PREFIX}/v
+00003550: 7b61 7069 5f76 6572 7369 6f6e 7d22 0a20  {api_version}". 
+00003560: 2020 2020 2020 2075 726c 203d 2066 227b         url = f"{
+00003570: 7365 6c66 2e5f 7572 6c7d 7b70 7265 6669  self._url}{prefi
+00003580: 787d 7b70 6174 687d 220a 2020 2020 2020  x}{path}".      
+00003590: 2020 6865 6164 6572 7320 3d20 7b0a 2020    headers = {.  
+000035a0: 2020 2020 2020 2020 2020 2261 7574 686f            "autho
+000035b0: 7269 7a61 7469 6f6e 223a 2073 656c 662e  rization": self.
+000035c0: 5f74 6f6b 656e 2c0a 2020 2020 2020 2020  _token,.        
+000035d0: 7d0a 2020 2020 2020 2020 6966 2061 6464  }.        if add
+000035e0: 5f6e 616d 6573 7061 6365 3a0a 2020 2020  _namespace:.    
+000035f0: 2020 2020 2020 2020 6172 6773 5b22 6e61          args["na
+00003600: 6d65 7370 6163 6522 5d20 3d20 7365 6c66  mespace"] = self
+00003610: 2e5f 6e61 6d65 7370 6163 650a 0a20 2020  ._namespace..   
+00003620: 2020 2020 2064 6566 2063 6865 636b 5f65       def check_e
+00003630: 7272 6f72 2872 6571 3a20 5265 7370 6f6e  rror(req: Respon
+00003640: 7365 2920 2d3e 204e 6f6e 653a 0a20 2020  se) -> None:.   
+00003650: 2020 2020 2020 2020 2069 6620 7265 712e           if req.
+00003660: 7374 6174 7573 5f63 6f64 6520 3d3d 2034  status_code == 4
+00003670: 3033 3a0a 2020 2020 2020 2020 2020 2020  03:.            
+00003680: 2020 2020 7261 6973 6520 4163 6365 7373      raise Access
+00003690: 4465 6e69 6564 2872 6571 2e74 6578 7429  Denied(req.text)
+000036a0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+000036b0: 2e72 6169 7365 5f66 6f72 5f73 7461 7475  .raise_for_statu
+000036c0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000036d0: 6966 2072 6571 2e68 6561 6465 7273 5b22  if req.headers["
+000036e0: 636f 6e74 656e 742d 7479 7065 225d 203d  content-type"] =
+000036f0: 3d20 2261 7070 6c69 6361 7469 6f6e 2f70  = "application/p
+00003700: 726f 626c 656d 2b6a 736f 6e22 3a0a 2020  roblem+json":.  
+00003710: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00003720: 6973 6520 5365 7276 6572 5369 6465 4572  ise ServerSideEr
+00003730: 726f 7228 6a73 6f6e 2e6c 6f61 6473 2872  ror(json.loads(r
+00003740: 6571 2e74 6578 7429 5b22 6572 724d 6573  eq.text)["errMes
+00003750: 7361 6765 225d 290a 0a20 2020 2020 2020  sage"])..       
+00003760: 2069 6620 6d65 7468 6f64 203d 3d20 4d45   if method == ME
+00003770: 5448 4f44 5f47 4554 3a0a 2020 2020 2020  THOD_GET:.      
+00003780: 2020 2020 2020 7265 7120 3d20 7265 7175        req = requ
+00003790: 6573 7473 2e67 6574 2875 726c 2c20 7061  ests.get(url, pa
+000037a0: 7261 6d73 3d61 7267 732c 2068 6561 6465  rams=args, heade
+000037b0: 7273 3d68 6561 6465 7273 290a 2020 2020  rs=headers).    
+000037c0: 2020 2020 2020 2020 6368 6563 6b5f 6572          check_er
+000037d0: 726f 7228 7265 7129 0a20 2020 2020 2020  ror(req).       
+000037e0: 2020 2020 2072 6574 7572 6e20 5374 7269       return Stri
+000037f0: 6e67 494f 2872 6571 2e74 6578 7429 0a20  ngIO(req.text). 
+00003800: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+00003810: 203d 3d20 4d45 5448 4f44 5f50 4f53 543a   == METHOD_POST:
+00003820: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+00003830: 203d 2072 6571 7565 7374 732e 706f 7374   = requests.post
+00003840: 2875 726c 2c20 6a73 6f6e 3d61 7267 732c  (url, json=args,
+00003850: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
+00003860: 290a 2020 2020 2020 2020 2020 2020 6368  ).            ch
+00003870: 6563 6b5f 6572 726f 7228 7265 7129 0a20  eck_error(req). 
+00003880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003890: 6e20 5374 7269 6e67 494f 2872 6571 2e74  n StringIO(req.t
+000038a0: 6578 7429 0a20 2020 2020 2020 2072 6169  ext).        rai
+000038b0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+000038c0: 756e 6b6e 6f77 6e20 6d65 7468 6f64 207b  unknown method {
+000038d0: 6d65 7468 6f64 7d22 290a 0a20 2020 2064  method}")..    d
+000038e0: 6566 205f 6661 6c6c 6962 6c65 5f72 6177  ef _fallible_raw
+000038f0: 5f72 6571 7565 7374 5f6a 736f 6e28 0a20  _request_json(. 
+00003900: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00003910: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00003920: 686f 643a 2073 7472 2c0a 2020 2020 2020  hod: str,.      
+00003930: 2020 2020 2020 7061 7468 3a20 7374 722c        path: str,
+00003940: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00003950: 733a 2044 6963 745b 7374 722c 2041 6e79  s: Dict[str, Any
+00003960: 5d2c 0a20 2020 2020 2020 2020 2020 2061  ],.            a
+00003970: 6464 5f70 7265 6669 783a 2062 6f6f 6c2c  dd_prefix: bool,
+00003980: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+00003990: 5f6e 616d 6573 7061 6365 3a20 626f 6f6c  _namespace: bool
+000039a0: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+000039b0: 6c65 733a 204f 7074 696f 6e61 6c5b 4469  les: Optional[Di
+000039c0: 6374 5b73 7472 2c20 494f 5b62 7974 6573  ct[str, IO[bytes
+000039d0: 5d5d 5d2c 0a20 2020 2020 2020 2020 2020  ]]],.           
+000039e0: 2061 7069 5f76 6572 7369 6f6e 3a20 4f70   api_version: Op
+000039f0: 7469 6f6e 616c 5b69 6e74 5d29 202d 3e20  tional[int]) -> 
+00003a00: 4469 6374 5b73 7472 2c20 416e 795d 3a0a  Dict[str, Any]:.
+00003a10: 2020 2020 2020 2020 7072 6566 6978 203d          prefix =
+00003a20: 2022 220a 2020 2020 2020 2020 6966 2061   "".        if a
+00003a30: 6464 5f70 7265 6669 783a 0a20 2020 2020  dd_prefix:.     
+00003a40: 2020 2020 2020 2069 6620 6170 695f 7665         if api_ve
+00003a50: 7273 696f 6e20 6973 204e 6f6e 653a 0a20  rsion is None:. 
+00003a60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003a70: 7069 5f76 6572 7369 6f6e 203d 2073 656c  pi_version = sel
+00003a80: 662e 5f61 7069 5f76 6572 7369 6f6e 0a20  f._api_version. 
+00003a90: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00003aa0: 7820 3d20 6622 7b50 5245 4649 587d 2f76  x = f"{PREFIX}/v
+00003ab0: 7b61 7069 5f76 6572 7369 6f6e 7d22 0a20  {api_version}". 
+00003ac0: 2020 2020 2020 2075 726c 203d 2066 227b         url = f"{
+00003ad0: 7365 6c66 2e5f 7572 6c7d 7b70 7265 6669  self._url}{prefi
+00003ae0: 787d 7b70 6174 687d 220a 2020 2020 2020  x}{path}".      
+00003af0: 2020 6865 6164 6572 7320 3d20 7b0a 2020    headers = {.  
+00003b00: 2020 2020 2020 2020 2020 2261 7574 686f            "autho
+00003b10: 7269 7a61 7469 6f6e 223a 2073 656c 662e  rization": self.
+00003b20: 5f74 6f6b 656e 2c0a 2020 2020 2020 2020  _token,.        
+00003b30: 7d0a 2020 2020 2020 2020 6966 2061 6464  }.        if add
+00003b40: 5f6e 616d 6573 7061 6365 3a0a 2020 2020  _namespace:.    
+00003b50: 2020 2020 2020 2020 6172 6773 5b22 6e61          args["na
+00003b60: 6d65 7370 6163 6522 5d20 3d20 7365 6c66  mespace"] = self
+00003b70: 2e5f 6e61 6d65 7370 6163 650a 2020 2020  ._namespace.    
+00003b80: 2020 2020 6966 206d 6574 686f 6420 213d      if method !=
+00003b90: 204d 4554 484f 445f 4649 4c45 2061 6e64   METHOD_FILE and
+00003ba0: 2066 696c 6573 2069 7320 6e6f 7420 4e6f   files is not No
+00003bb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003bc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00003bd0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003be0: 2020 6622 6669 6c65 7320 6172 6520 6f6e    f"files are on
+00003bf0: 6c79 2061 6c6c 6f77 2066 6f72 2070 6f73  ly allow for pos
+00003c00: 7420 2867 6f74 207b 6d65 7468 6f64 7d29  t (got {method})
+00003c10: 3a20 7b66 696c 6573 7d22 290a 2020 2020  : {files}").    
+00003c20: 2020 2020 7265 7120 3d20 4e6f 6e65 0a0a      req = None..
+00003c30: 2020 2020 2020 2020 6465 6620 6368 6563          def chec
+00003c40: 6b5f 6572 726f 7228 7265 713a 2052 6573  k_error(req: Res
+00003c50: 706f 6e73 6529 202d 3e20 4e6f 6e65 3a0a  ponse) -> None:.
+00003c60: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00003c70: 6571 2e73 7461 7475 735f 636f 6465 203d  eq.status_code =
+00003c80: 3d20 3430 333a 0a20 2020 2020 2020 2020  = 403:.         
+00003c90: 2020 2020 2020 2072 6169 7365 2041 6363         raise Acc
+00003ca0: 6573 7344 656e 6965 6428 7265 712e 7465  essDenied(req.te
+00003cb0: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
+00003cc0: 7265 712e 7261 6973 655f 666f 725f 7374  req.raise_for_st
+00003cd0: 6174 7573 2829 0a20 2020 2020 2020 2020  atus().         
+00003ce0: 2020 2069 6620 7265 712e 6865 6164 6572     if req.header
+00003cf0: 735b 2263 6f6e 7465 6e74 2d74 7970 6522  s["content-type"
+00003d00: 5d20 3d3d 2022 6170 706c 6963 6174 696f  ] == "applicatio
+00003d10: 6e2f 7072 6f62 6c65 6d2b 6a73 6f6e 223a  n/problem+json":
+00003d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d30: 2072 6169 7365 2053 6572 7665 7253 6964   raise ServerSid
+00003d40: 6545 7272 6f72 286a 736f 6e2e 6c6f 6164  eError(json.load
+00003d50: 7328 7265 712e 7465 7874 295b 2265 7272  s(req.text)["err
+00003d60: 4d65 7373 6167 6522 5d29 0a0a 2020 2020  Message"])..    
+00003d70: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00003d80: 2020 2020 2069 6620 6d65 7468 6f64 203d       if method =
+00003d90: 3d20 4d45 5448 4f44 5f47 4554 3a0a 2020  = METHOD_GET:.  
+00003da0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00003db0: 7120 3d20 7265 7175 6573 7473 2e67 6574  q = requests.get
+00003dc0: 2875 726c 2c20 7061 7261 6d73 3d61 7267  (url, params=arg
+00003dd0: 732c 2068 6561 6465 7273 3d68 6561 6465  s, headers=heade
+00003de0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
+00003df0: 2020 2020 6368 6563 6b5f 6572 726f 7228      check_error(
+00003e00: 7265 7129 0a20 2020 2020 2020 2020 2020  req).           
+00003e10: 2020 2020 2072 6574 7572 6e20 6a73 6f6e       return json
+00003e20: 2e6c 6f61 6473 2872 6571 2e74 6578 7429  .loads(req.text)
+00003e30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003e40: 6d65 7468 6f64 203d 3d20 4d45 5448 4f44  method == METHOD
+00003e50: 5f46 494c 453a 0a20 2020 2020 2020 2020  _FILE:.         
+00003e60: 2020 2020 2020 2069 6620 6669 6c65 7320         if files 
+00003e70: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00003e80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00003e90: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00003ea0: 6669 6c65 206d 6574 686f 6420 6d75 7374  file method must
+00003eb0: 2068 6176 6520 6669 6c65 733a 207b 6669   have files: {fi
+00003ec0: 6c65 737d 2229 0a20 2020 2020 2020 2020  les}").         
+00003ed0: 2020 2020 2020 2072 6571 203d 2072 6571         req = req
+00003ee0: 7565 7374 732e 706f 7374 280a 2020 2020  uests.post(.    
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 7572 6c2c 0a20 2020 2020 2020 2020 2020  url,.           
+00003f10: 2020 2020 2020 2020 2064 6174 613d 6172           data=ar
+00003f20: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+00003f30: 2020 2020 2020 2020 6669 6c65 733d 7b0a          files={.
+00003f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f50: 2020 2020 2020 2020 6b65 793a 2028 0a20          key: (. 
+00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f70: 2020 2020 2020 2020 2020 2067 6574 6174             getat
+00003f80: 7472 2876 616c 7565 2c20 226e 616d 6522  tr(value, "name"
+00003f90: 2c20 6b65 7929 2c0a 2020 2020 2020 2020  , key),.        
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 2020 2020 7661 6c75 652c 0a20 2020 2020      value,.     
+00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fd0: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
+00003fe0: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
+00003ff0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00004000: 2020 2020 2020 2020 2020 2029 2066 6f72             ) for
+00004010: 2028 6b65 792c 2076 616c 7565 2920 696e   (key, value) in
+00004020: 2066 696c 6573 2e69 7465 6d73 2829 0a20   files.items(). 
+00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004040: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00004050: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00004060: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
+00004070: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00004080: 5f65 7272 6f72 2872 6571 290a 2020 2020  _error(req).    
+00004090: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000040a0: 726e 206a 736f 6e2e 6c6f 6164 7328 7265  rn json.loads(re
+000040b0: 712e 7465 7874 290a 2020 2020 2020 2020  q.text).        
+000040c0: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
+000040d0: 204d 4554 484f 445f 504f 5354 3a0a 2020   METHOD_POST:.  
+000040e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000040f0: 7120 3d20 7265 7175 6573 7473 2e70 6f73  q = requests.pos
+00004100: 7428 7572 6c2c 206a 736f 6e3d 6172 6773  t(url, json=args
+00004110: 2c20 6865 6164 6572 733d 6865 6164 6572  , headers=header
+00004120: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00004130: 2020 2063 6865 636b 5f65 7272 6f72 2872     check_error(r
+00004140: 6571 290a 2020 2020 2020 2020 2020 2020  eq).            
+00004150: 2020 2020 7265 7475 726e 206a 736f 6e2e      return json.
+00004160: 6c6f 6164 7328 7265 712e 7465 7874 290a  loads(req.text).
+00004170: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00004180: 6574 686f 6420 3d3d 204d 4554 484f 445f  ethod == METHOD_
+00004190: 5055 543a 0a20 2020 2020 2020 2020 2020  PUT:.           
+000041a0: 2020 2020 2072 6571 203d 2072 6571 7565       req = reque
+000041b0: 7374 732e 7075 7428 7572 6c2c 206a 736f  sts.put(url, jso
+000041c0: 6e3d 6172 6773 2c20 6865 6164 6572 733d  n=args, headers=
+000041d0: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
+000041e0: 2020 2020 2020 2020 2063 6865 636b 5f65           check_e
+000041f0: 7272 6f72 2872 6571 290a 2020 2020 2020  rror(req).      
+00004200: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004210: 206a 736f 6e2e 6c6f 6164 7328 7265 712e   json.loads(req.
+00004220: 7465 7874 290a 2020 2020 2020 2020 2020  text).          
+00004230: 2020 6966 206d 6574 686f 6420 3d3d 204d    if method == M
+00004240: 4554 484f 445f 4445 4c45 5445 3a0a 2020  ETHOD_DELETE:.  
+00004250: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004260: 7120 3d20 7265 7175 6573 7473 2e64 656c  q = requests.del
+00004270: 6574 6528 7572 6c2c 206a 736f 6e3d 6172  ete(url, json=ar
+00004280: 6773 2c20 6865 6164 6572 733d 6865 6164  gs, headers=head
+00004290: 6572 7329 0a20 2020 2020 2020 2020 2020  ers).           
+000042a0: 2020 2020 2063 6865 636b 5f65 7272 6f72       check_error
+000042b0: 2872 6571 290a 2020 2020 2020 2020 2020  (req).          
+000042c0: 2020 2020 2020 7265 7475 726e 206a 736f        return jso
+000042d0: 6e2e 6c6f 6164 7328 7265 712e 7465 7874  n.loads(req.text
+000042e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000042f0: 206d 6574 686f 6420 3d3d 204d 4554 484f   method == METHO
+00004300: 445f 4c4f 4e47 504f 5354 3a0a 2020 2020  D_LONGPOST:.    
+00004310: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00004320: 5b22 746f 6b65 6e22 5d20 3d20 7365 6c66  ["token"] = self
+00004330: 2e5f 746f 6b65 6e0a 2020 2020 2020 2020  ._token.        
+00004340: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004360: 2072 6573 203d 2071 7569 636b 5f73 6572   res = quick_ser
+00004370: 7665 722e 776f 726b 6572 5f72 6571 7565  ver.worker_reque
+00004380: 7374 2875 726c 2c20 6172 6773 290a 2020  st(url, args).  
+00004390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043a0: 2020 6966 2022 6572 724d 6573 7361 6765    if "errMessage
+000043b0: 2220 696e 2072 6573 3a0a 2020 2020 2020  " in res:.      
+000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043d0: 2020 7261 6973 6520 5365 7276 6572 5369    raise ServerSi
+000043e0: 6465 4572 726f 7228 7265 735b 2265 7272  deError(res["err
+000043f0: 4d65 7373 6167 6522 5d29 0a20 2020 2020  Message"]).     
+00004400: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004410: 6574 7572 6e20 7265 730a 2020 2020 2020  eturn res.      
+00004420: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00004430: 2071 7569 636b 5f73 6572 7665 722e 576f   quick_server.Wo
+00004440: 726b 6572 4572 726f 7220 6173 2065 3a0a  rkerError as e:.
+00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004460: 2020 2020 6966 2065 2e67 6574 5f73 7461      if e.get_sta
+00004470: 7475 735f 636f 6465 2829 203d 3d20 3430  tus_code() == 40
+00004480: 333a 0a20 2020 2020 2020 2020 2020 2020  3:.             
+00004490: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000044a0: 2041 6363 6573 7344 656e 6965 6428 652e   AccessDenied(e.
+000044b0: 6172 6773 2920 6672 6f6d 2065 0a20 2020  args) from e.   
+000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044d0: 2072 6169 7365 2065 0a20 2020 2020 2020   raise e.       
+000044e0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000044f0: 4572 726f 7228 6622 756e 6b6e 6f77 6e20  Error(f"unknown 
+00004500: 6d65 7468 6f64 207b 6d65 7468 6f64 7d22  method {method}"
+00004510: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00004520: 206a 736f 6e2e 6465 636f 6465 722e 4a53   json.decoder.JS
+00004530: 4f4e 4465 636f 6465 4572 726f 7220 6173  ONDecodeError as
+00004540: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00004550: 6966 2072 6571 2069 7320 4e6f 6e65 3a0a  if req is None:.
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 7261 6973 650a 2020 2020 2020 2020 2020  raise.          
+00004580: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00004590: 6f72 2872 6571 2e74 6578 7429 2066 726f  or(req.text) fro
+000045a0: 6d20 650a 0a20 2020 2064 6566 2072 6571  m e..    def req
+000045b0: 7565 7374 5f62 7974 6573 280a 2020 2020  uest_bytes(.    
+000045c0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000045d0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+000045e0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
+000045f0: 2020 2070 6174 683a 2073 7472 2c0a 2020     path: str,.  
+00004600: 2020 2020 2020 2020 2020 6172 6773 3a20            args: 
+00004610: 4469 6374 5b73 7472 2c20 416e 795d 2c0a  Dict[str, Any],.
+00004620: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00004630: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
+00004640: 5b73 7472 2c20 4279 7465 7349 4f5d 5d20  [str, BytesIO]] 
+00004650: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00004660: 2020 2020 6164 645f 7072 6566 6978 3a20      add_prefix: 
+00004670: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+00004680: 2020 2020 2020 2020 2061 6464 5f6e 616d           add_nam
+00004690: 6573 7061 6365 3a20 626f 6f6c 203d 2054  espace: bool = T
+000046a0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000046b0: 2061 7069 5f76 6572 7369 6f6e 3a20 4f70   api_version: Op
+000046c0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000046d0: 6e65 2920 2d3e 2054 7570 6c65 5b42 7974  ne) -> Tuple[Byt
+000046e0: 6573 494f 2c20 7374 725d 3a0a 2020 2020  esIO, str]:.    
+000046f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004700: 5f72 6177 5f72 6571 7565 7374 5f62 7974  _raw_request_byt
+00004710: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00004720: 6d65 7468 6f64 2c20 7061 7468 2c20 6172  method, path, ar
+00004730: 6773 2c20 6669 6c65 732c 2061 6464 5f70  gs, files, add_p
+00004740: 7265 6669 782c 2061 6464 5f6e 616d 6573  refix, add_names
+00004750: 7061 6365 2c20 6170 695f 7665 7273 696f  pace, api_versio
+00004760: 6e29 0a0a 2020 2020 6465 6620 7265 7175  n)..    def requ
+00004770: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
+00004780: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00004790: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+000047a0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+000047b0: 2070 6174 683a 2073 7472 2c0a 2020 2020   path: str,.    
+000047c0: 2020 2020 2020 2020 6172 6773 3a20 4469          args: Di
+000047d0: 6374 5b73 7472 2c20 416e 795d 2c0a 2020  ct[str, Any],.  
+000047e0: 2020 2020 2020 2020 2020 6164 645f 7072            add_pr
+000047f0: 6566 6978 3a20 626f 6f6c 203d 2054 7275  efix: bool = Tru
+00004800: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
+00004810: 6464 5f6e 616d 6573 7061 6365 3a20 626f  dd_namespace: bo
+00004820: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+00004830: 2020 2020 2020 2066 696c 6573 3a20 4f70         files: Op
+00004840: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00004850: 2049 4f5b 6279 7465 735d 5d5d 203d 204e   IO[bytes]]] = N
+00004860: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00004870: 2061 7069 5f76 6572 7369 6f6e 3a20 4f70   api_version: Op
+00004880: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00004890: 6e65 2920 2d3e 2044 6963 745b 7374 722c  ne) -> Dict[str,
+000048a0: 2041 6e79 5d3a 0a20 2020 2020 2020 2072   Any]:.        r
+000048b0: 6574 7572 6e20 7365 6c66 2e5f 7261 775f  eturn self._raw_
+000048c0: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
+000048d0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+000048e0: 2c20 7061 7468 2c20 6172 6773 2c20 6164  , path, args, ad
+000048f0: 645f 7072 6566 6978 2c20 6164 645f 6e61  d_prefix, add_na
+00004900: 6d65 7370 6163 652c 2066 696c 6573 2c20  mespace, files, 
+00004910: 6170 695f 7665 7273 696f 6e29 0a0a 2020  api_version)..  
+00004920: 2020 6465 6620 6765 745f 7365 7276 6572    def get_server
+00004930: 5f76 6572 7369 6f6e 2873 656c 6629 202d  _version(self) -
+00004940: 3e20 5665 7273 696f 6e52 6573 706f 6e73  > VersionRespons
+00004950: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+00004960: 6e20 6361 7374 2856 6572 7369 6f6e 5265  n cast(VersionRe
+00004970: 7370 6f6e 7365 2c20 7365 6c66 2e72 6571  sponse, self.req
+00004980: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00004990: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
+000049a0: 542c 0a20 2020 2020 2020 2020 2020 2066  T,.            f
+000049b0: 227b 5052 4546 4958 7d2f 767b 4150 495f  "{PREFIX}/v{API_
+000049c0: 5645 5253 494f 4e7d 2f76 6572 7369 6f6e  VERSION}/version
+000049d0: 222c 0a20 2020 2020 2020 2020 2020 207b  ",.            {
+000049e0: 7d2c 0a20 2020 2020 2020 2020 2020 2061  },.            a
+000049f0: 6464 5f70 7265 6669 783d 4661 6c73 652c  dd_prefix=False,
+00004a00: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+00004a10: 5f6e 616d 6573 7061 6365 3d46 616c 7365  _namespace=False
+00004a20: 2929 0a0a 2020 2020 6465 6620 6765 745f  ))..    def get_
+00004a30: 7665 7273 696f 6e5f 6f76 6572 7269 6465  version_override
+00004a40: 2873 656c 6629 202d 3e20 4469 6374 5b73  (self) -> Dict[s
+00004a50: 7472 2c20 4c69 7374 5b4f 7074 696f 6e61  tr, List[Optiona
+00004a60: 6c5b 7374 725d 5d5d 3a0a 2020 2020 2020  l[str]]]:.      
+00004a70: 2020 7365 7276 6572 5f76 6572 7369 6f6e    server_version
+00004a80: 203d 2073 656c 662e 6765 745f 7365 7276   = self.get_serv
+00004a90: 6572 5f76 6572 7369 6f6e 2829 0a20 2020  er_version().   
+00004aa0: 2020 2020 2069 6d67 5f72 6570 6f20 3d20       img_repo = 
+00004ab0: 7365 7276 6572 5f76 6572 7369 6f6e 5b22  server_version["
+00004ac0: 696d 6167 655f 7265 706f 225d 0a20 2020  image_repo"].   
+00004ad0: 2020 2020 2069 6d67 5f74 6167 203d 2073       img_tag = s
+00004ae0: 6572 7665 725f 7665 7273 696f 6e5b 2269  erver_version["i
+00004af0: 6d61 6765 5f74 6167 225d 0a20 2020 2020  mage_tag"].     
+00004b00: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
+00004b10: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+00004b20: 223a 205b 696d 675f 7265 706f 2c20 696d  ": [img_repo, im
+00004b30: 675f 7461 675d 2c0a 2020 2020 2020 2020  g_tag],.        
+00004b40: 7d0a 0a20 2020 2064 6566 2067 6574 5f6e  }..    def get_n
+00004b50: 616d 6573 7061 6365 7328 7365 6c66 2920  amespaces(self) 
+00004b60: 2d3e 204c 6973 745b 7374 725d 3a0a 2020  -> List[str]:.  
+00004b70: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00004b80: 7428 4e61 6d65 7370 6163 654c 6973 742c  t(NamespaceList,
+00004b90: 2073 656c 662e 7265 7175 6573 745f 6a73   self.request_js
+00004ba0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00004bb0: 4d45 5448 4f44 5f47 4554 2c20 222f 6e61  METHOD_GET, "/na
+00004bc0: 6d65 7370 6163 6573 222c 207b 7d29 295b  mespaces", {}))[
+00004bd0: 226e 616d 6573 7061 6365 7322 5d0a 0a20  "namespaces"].. 
+00004be0: 2020 2064 6566 2067 6574 5f64 6167 7328     def get_dags(
+00004bf0: 7365 6c66 2920 2d3e 204c 6973 745b 7374  self) -> List[st
+00004c00: 725d 3a0a 2020 2020 2020 2020 7265 7475  r]:.        retu
+00004c10: 726e 205b 0a20 2020 2020 2020 2020 2020  rn [.           
+00004c20: 2072 6573 5b22 6461 6722 5d0a 2020 2020   res["dag"].    
+00004c30: 2020 2020 2020 2020 666f 7220 7265 7320          for res 
+00004c40: 696e 2073 656c 662e 6765 745f 6461 675f  in self.get_dag_
+00004c50: 7469 6d65 7328 7265 7472 6965 7665 5f74  times(retrieve_t
+00004c60: 696d 6573 3d46 616c 7365 295b 315d 0a20  imes=False)[1]. 
+00004c70: 2020 2020 2020 205d 0a0a 2020 2020 6465         ]..    de
+00004c80: 6620 6765 745f 6461 675f 6167 6573 2873  f get_dag_ages(s
+00004c90: 656c 6629 202d 3e20 4c69 7374 5b44 6963  elf) -> List[Dic
+00004ca0: 745b 7374 722c 204f 7074 696f 6e61 6c5b  t[str, Optional[
+00004cb0: 7374 725d 5d5d 3a0a 2020 2020 2020 2020  str]]]:.        
+00004cc0: 6375 725f 7469 6d65 2c20 6461 6773 203d  cur_time, dags =
+00004cd0: 2073 656c 662e 6765 745f 6461 675f 7469   self.get_dag_ti
+00004ce0: 6d65 7328 7265 7472 6965 7665 5f74 696d  mes(retrieve_tim
+00004cf0: 6573 3d54 7275 6529 0a20 2020 2020 2020  es=True).       
+00004d00: 2072 6574 7572 6e20 5b0a 2020 2020 2020   return [.      
+00004d10: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00004d20: 2020 2020 2020 2020 2263 6f6e 6669 675f          "config_
+00004d30: 6572 726f 7222 3a20 6461 675f 7374 6174  error": dag_stat
+00004d40: 7573 5b22 636f 6e66 6967 5f65 7272 6f72  us["config_error
+00004d50: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+00004d60: 2020 2020 2263 7265 6174 6564 223a 2067      "created": g
+00004d70: 6574 5f61 6765 2863 7572 5f74 696d 652c  et_age(cur_time,
+00004d80: 2064 6167 5f73 7461 7475 735b 2263 7265   dag_status["cre
+00004d90: 6174 6564 225d 292c 0a20 2020 2020 2020  ated"]),.       
+00004da0: 2020 2020 2020 2020 2022 6461 6722 3a20           "dag": 
+00004db0: 6461 675f 7374 6174 7573 5b22 6461 6722  dag_status["dag"
+00004dc0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00004dd0: 2020 2022 6465 6c65 7465 6422 3a20 6765     "deleted": ge
+00004de0: 745f 6167 6528 6375 725f 7469 6d65 2c20  t_age(cur_time, 
+00004df0: 6461 675f 7374 6174 7573 5b22 6465 6c65  dag_status["dele
+00004e00: 7465 6422 5d29 2c0a 2020 2020 2020 2020  ted"]),.        
+00004e10: 2020 2020 2020 2020 226c 6174 6573 7422          "latest"
+00004e20: 3a20 6765 745f 6167 6528 6375 725f 7469  : get_age(cur_ti
+00004e30: 6d65 2c20 6461 675f 7374 6174 7573 5b22  me, dag_status["
+00004e40: 6c61 7465 7374 225d 292c 0a20 2020 2020  latest"]),.     
+00004e50: 2020 2020 2020 2020 2020 2022 6f6c 6465             "olde
+00004e60: 7374 223a 2067 6574 5f61 6765 2863 7572  st": get_age(cur
+00004e70: 5f74 696d 652c 2064 6167 5f73 7461 7475  _time, dag_statu
+00004e80: 735b 226f 6c64 6573 7422 5d29 2c0a 2020  s["oldest"]),.  
+00004e90: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00004ea0: 2020 2020 2020 2020 666f 7220 6461 675f          for dag_
+00004eb0: 7374 6174 7573 2069 6e20 736f 7274 6564  status in sorted
+00004ec0: 2864 6167 732c 206b 6579 3d6c 616d 6264  (dags, key=lambd
+00004ed0: 6120 656c 3a20 280a 2020 2020 2020 2020  a el: (.        
+00004ee0: 2020 2020 2020 2020 656c 5b22 636f 6e66          el["conf
+00004ef0: 6967 5f65 7272 6f72 225d 2069 7320 4e6f  ig_error"] is No
+00004f00: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00004f10: 2020 2020 7361 6665 5f6f 7074 5f6e 756d      safe_opt_num
+00004f20: 2865 6c5b 226f 6c64 6573 7422 5d29 2c0a  (el["oldest"]),.
+00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f40: 7361 6665 5f6f 7074 5f6e 756d 2865 6c5b  safe_opt_num(el[
+00004f50: 226c 6174 6573 7422 5d29 2c0a 2020 2020  "latest"]),.    
+00004f60: 2020 2020 2020 2020 2020 2020 656c 5b22              el["
+00004f70: 6461 6722 5d29 290a 2020 2020 2020 2020  dag"])).        
+00004f80: 5d0a 0a20 2020 2064 6566 2067 6574 5f64  ]..    def get_d
+00004f90: 6167 5f74 696d 6573 2873 656c 662c 2072  ag_times(self, r
+00004fa0: 6574 7269 6576 655f 7469 6d65 733a 2062  etrieve_times: b
+00004fb0: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2054  ool = True) -> T
+00004fc0: 7570 6c65 5b0a 2020 2020 2020 2020 2020  uple[.          
+00004fd0: 2020 666c 6f61 742c 204c 6973 745b 4461    float, List[Da
+00004fe0: 6753 7461 7475 735d 5d3a 0a20 2020 2020  gStatus]]:.     
+00004ff0: 2020 2072 6573 203d 2063 6173 7428 4461     res = cast(Da
+00005000: 674c 6973 742c 2073 656c 662e 7265 7175  gList, self.requ
+00005010: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
+00005020: 2020 2020 2020 4d45 5448 4f44 5f47 4554        METHOD_GET
+00005030: 2c20 222f 6461 6773 222c 207b 0a20 2020  , "/dags", {.   
+00005040: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00005050: 7472 6965 7665 5f74 696d 6573 223a 2069  trieve_times": i
+00005060: 6e74 2872 6574 7269 6576 655f 7469 6d65  nt(retrieve_time
+00005070: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00005080: 7d29 290a 2020 2020 2020 2020 7265 7475  })).        retu
+00005090: 726e 2072 6573 5b22 6375 725f 7469 6d65  rn res["cur_time
+000050a0: 225d 2c20 7265 735b 2264 6167 7322 5d0a  "], res["dags"].
+000050b0: 0a20 2020 2064 6566 2067 6574 5f64 6167  .    def get_dag
+000050c0: 2873 656c 662c 2064 6167 5f75 7269 3a20  (self, dag_uri: 
+000050d0: 7374 7229 202d 3e20 2744 6167 4861 6e64  str) -> 'DagHand
+000050e0: 6c65 273a 0a20 2020 2020 2020 2072 6573  le':.        res
+000050f0: 203d 2073 656c 662e 5f64 6167 5f63 6163   = self._dag_cac
+00005100: 6865 2e67 6574 2864 6167 5f75 7269 290a  he.get(dag_uri).
+00005110: 2020 2020 2020 2020 6966 2072 6573 2069          if res i
+00005120: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00005130: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00005140: 6573 0a20 2020 2020 2020 2072 6573 203d  es.        res =
+00005150: 2044 6167 4861 6e64 6c65 2873 656c 662c   DagHandle(self,
+00005160: 2064 6167 5f75 7269 290a 2020 2020 2020   dag_uri).      
+00005170: 2020 7365 6c66 2e5f 6461 675f 6361 6368    self._dag_cach
+00005180: 655b 6461 675f 7572 695d 203d 2072 6573  e[dag_uri] = res
+00005190: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000051a0: 7265 730a 0a20 2020 2064 6566 2067 6574  res..    def get
+000051b0: 5f62 6c6f 625f 6861 6e64 6c65 2873 656c  _blob_handle(sel
+000051c0: 662c 2075 7269 3a20 7374 722c 2069 735f  f, uri: str, is_
+000051d0: 6675 6c6c 3a20 626f 6f6c 203d 2046 616c  full: bool = Fal
+000051e0: 7365 2920 2d3e 2027 426c 6f62 4861 6e64  se) -> 'BlobHand
+000051f0: 6c65 273a 0a20 2020 2020 2020 2072 6574  le':.        ret
+00005200: 7572 6e20 426c 6f62 4861 6e64 6c65 2873  urn BlobHandle(s
+00005210: 656c 662c 2075 7269 2c20 6973 5f66 756c  elf, uri, is_ful
+00005220: 6c3d 6973 5f66 756c 6c29 0a0a 2020 2020  l=is_full)..    
+00005230: 6465 6620 6765 745f 6e6f 6465 5f64 6566  def get_node_def
+00005240: 7328 7365 6c66 2920 2d3e 2044 6963 745b  s(self) -> Dict[
+00005250: 7374 722c 204e 6f64 6544 6566 496e 666f  str, NodeDefInfo
+00005260: 5d3a 0a20 2020 2020 2020 2073 656c 662e  ]:.        self.
+00005270: 5f6d 6179 6265 5f72 6566 7265 7368 2829  _maybe_refresh()
+00005280: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005290: 2e5f 6e6f 6465 5f64 6566 7320 6973 206e  ._node_defs is n
+000052a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000052b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000052c0: 2e5f 6e6f 6465 5f64 6566 730a 2020 2020  ._node_defs.    
+000052d0: 2020 2020 7265 7320 3d20 6361 7374 284e      res = cast(N
+000052e0: 6f64 6554 7970 6573 2c20 7365 6c66 2e72  odeTypes, self.r
+000052f0: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
+00005300: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+00005310: 4745 542c 2022 2f6e 6f64 655f 7479 7065  GET, "/node_type
+00005320: 7322 2c20 7b7d 2c20 6164 645f 6e61 6d65  s", {}, add_name
+00005330: 7370 6163 653d 4661 6c73 6529 295b 2269  space=False))["i
+00005340: 6e66 6f22 5d0a 2020 2020 2020 2020 7365  nfo"].        se
+00005350: 6c66 2e5f 6e6f 6465 5f64 6566 7320 3d20  lf._node_defs = 
+00005360: 7265 730a 2020 2020 2020 2020 7265 7475  res.        retu
+00005370: 726e 2072 6573 0a0a 2020 2020 6465 6620  rn res..    def 
+00005380: 6372 6561 7465 5f6e 6577 5f62 6c6f 6228  create_new_blob(
+00005390: 7365 6c66 2c20 626c 6f62 5f74 7970 653a  self, blob_type:
+000053a0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
+000053b0: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+000053c0: 7428 426c 6f62 496e 6974 2c20 7365 6c66  t(BlobInit, self
+000053d0: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+000053e0: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+000053f0: 445f 504f 5354 2c20 222f 626c 6f62 5f69  D_POST, "/blob_i
+00005400: 6e69 7422 2c20 7b0a 2020 2020 2020 2020  nit", {.        
+00005410: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00005420: 626c 6f62 5f74 7970 652c 0a20 2020 2020  blob_type,.     
+00005430: 2020 2020 2020 207d 2c20 6164 645f 6e61         }, add_na
+00005440: 6d65 7370 6163 653d 4661 6c73 6529 295b  mespace=False))[
+00005450: 2262 6c6f 6222 5d0a 0a20 2020 2064 6566  "blob"]..    def
+00005460: 2067 6574 5f62 6c6f 625f 6f77 6e65 7228   get_blob_owner(
+00005470: 7365 6c66 2c20 626c 6f62 5f75 7269 3a20  self, blob_uri: 
+00005480: 7374 7229 202d 3e20 426c 6f62 4f77 6e65  str) -> BlobOwne
+00005490: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+000054a0: 6e20 6361 7374 2842 6c6f 624f 776e 6572  n cast(BlobOwner
+000054b0: 2c20 7365 6c66 2e72 6571 7565 7374 5f6a  , self.request_j
+000054c0: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+000054d0: 204d 4554 484f 445f 4745 542c 2022 2f62   METHOD_GET, "/b
+000054e0: 6c6f 625f 6f77 6e65 7222 2c20 7b0a 2020  lob_owner", {.  
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00005500: 6c6f 6222 3a20 626c 6f62 5f75 7269 2c0a  lob": blob_uri,.
+00005510: 2020 2020 2020 2020 2020 2020 7d29 290a              })).
+00005520: 0a20 2020 2064 6566 2073 6574 5f62 6c6f  .    def set_blo
+00005530: 625f 6f77 6e65 7228 0a20 2020 2020 2020  b_owner(.       
+00005540: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00005550: 2020 2020 2020 2062 6c6f 625f 7572 693a         blob_uri:
+00005560: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+00005570: 2020 6461 675f 6964 3a20 4f70 7469 6f6e    dag_id: Option
+00005580: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00005590: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+000055a0: 5f69 643a 204f 7074 696f 6e61 6c5b 7374  _id: Optional[st
+000055b0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000055c0: 2020 2020 2020 2065 7874 6572 6e61 6c5f         external_
+000055d0: 6f77 6e65 723a 2062 6f6f 6c20 3d20 4661  owner: bool = Fa
+000055e0: 6c73 6529 202d 3e20 426c 6f62 4f77 6e65  lse) -> BlobOwne
+000055f0: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+00005600: 6e20 6361 7374 2842 6c6f 624f 776e 6572  n cast(BlobOwner
+00005610: 2c20 7365 6c66 2e72 6571 7565 7374 5f6a  , self.request_j
+00005620: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00005630: 204d 4554 484f 445f 5055 542c 2022 2f62   METHOD_PUT, "/b
+00005640: 6c6f 625f 6f77 6e65 7222 2c20 7b0a 2020  lob_owner", {.  
+00005650: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00005660: 6c6f 6222 3a20 626c 6f62 5f75 7269 2c0a  lob": blob_uri,.
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 226f 776e 6572 5f64 6167 223a 2064 6167  "owner_dag": dag
+00005690: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+000056a0: 2020 2020 2022 6f77 6e65 725f 6e6f 6465       "owner_node
+000056b0: 223a 206e 6f64 655f 6964 2c0a 2020 2020  ": node_id,.    
+000056c0: 2020 2020 2020 2020 2020 2020 2265 7874              "ext
+000056d0: 6572 6e61 6c5f 6f77 6e65 7222 3a20 6578  ernal_owner": ex
+000056e0: 7465 726e 616c 5f6f 776e 6572 2c0a 2020  ternal_owner,.  
+000056f0: 2020 2020 2020 2020 2020 7d29 290a 0a20            })).. 
+00005700: 2020 2064 6566 2063 7265 6174 655f 6e65     def create_ne
+00005710: 775f 6461 6728 0a20 2020 2020 2020 2020  w_dag(.         
+00005720: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00005730: 2020 2020 2075 7365 726e 616d 653a 204f       username: O
+00005740: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00005750: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00005760: 2064 6167 6e61 6d65 3a20 4f70 7469 6f6e   dagname: Option
+00005770: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00005780: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00005790: 783a 204f 7074 696f 6e61 6c5b 696e 745d  x: Optional[int]
+000057a0: 203d 204e 6f6e 6529 202d 3e20 7374 723a   = None) -> str:
+000057b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000057c0: 6361 7374 2844 6167 496e 6974 2c20 7365  cast(DagInit, se
+000057d0: 6c66 2e72 6571 7565 7374 5f6a 736f 6e28  lf.request_json(
+000057e0: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+000057f0: 484f 445f 504f 5354 2c20 222f 6461 675f  HOD_POST, "/dag_
+00005800: 696e 6974 222c 207b 0a20 2020 2020 2020  init", {.       
+00005810: 2020 2020 2020 2020 2022 7573 6572 223a           "user":
+00005820: 2075 7365 726e 616d 652c 0a20 2020 2020   username,.     
+00005830: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00005840: 223a 2064 6167 6e61 6d65 2c0a 2020 2020  ": dagname,.    
+00005850: 2020 2020 2020 2020 2020 2020 2269 6e64              "ind
+00005860: 6578 223a 2069 6e64 6578 2c0a 2020 2020  ex": index,.    
+00005870: 2020 2020 2020 2020 7d29 295b 2264 6167          }))["dag
+00005880: 225d 0a0a 2020 2020 6465 6620 6765 745f  "]..    def get_
+00005890: 626c 6f62 5f74 7970 6528 7365 6c66 2c20  blob_type(self, 
+000058a0: 626c 6f62 5f75 7269 3a20 7374 7229 202d  blob_uri: str) -
+000058b0: 3e20 426c 6f62 5479 7065 5265 7370 6f6e  > BlobTypeRespon
+000058c0: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
+000058d0: 726e 2063 6173 7428 426c 6f62 5479 7065  rn cast(BlobType
+000058e0: 5265 7370 6f6e 7365 2c20 7365 6c66 2e72  Response, self.r
+000058f0: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
+00005900: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+00005910: 4745 542c 2022 2f62 6c6f 625f 7479 7065  GET, "/blob_type
+00005920: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+00005930: 2020 2020 2022 626c 6f62 5f75 7269 223a       "blob_uri":
+00005940: 2062 6c6f 625f 7572 692c 0a20 2020 2020   blob_uri,.     
+00005950: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005960: 2020 2929 0a0a 2020 2020 6465 6620 6765    ))..    def ge
+00005970: 745f 6373 765f 626c 6f62 2873 656c 662c  t_csv_blob(self,
+00005980: 2062 6c6f 625f 7572 693a 2073 7472 2920   blob_uri: str) 
+00005990: 2d3e 2027 4353 5642 6c6f 6248 616e 646c  -> 'CSVBlobHandl
+000059a0: 6527 3a0a 2020 2020 2020 2020 626c 6f62  e':.        blob
+000059b0: 5f74 7970 6520 3d20 7365 6c66 2e67 6574  _type = self.get
+000059c0: 5f62 6c6f 625f 7479 7065 2862 6c6f 625f  _blob_type(blob_
+000059d0: 7572 6929 0a20 2020 2020 2020 2069 6620  uri).        if 
+000059e0: 6e6f 7420 626c 6f62 5f74 7970 655b 2269  not blob_type["i
+000059f0: 735f 6373 7622 5d3a 0a20 2020 2020 2020  s_csv"]:.       
+00005a00: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00005a10: 4572 726f 7228 6622 626c 6f62 3a20 7b62  Error(f"blob: {b
+00005a20: 6c6f 625f 7572 697d 2069 7320 6e6f 7420  lob_uri} is not 
+00005a30: 6373 7620 7479 7065 2229 0a20 2020 2020  csv type").     
+00005a40: 2020 2072 6574 7572 6e20 4353 5642 6c6f     return CSVBlo
+00005a50: 6248 616e 646c 6528 7365 6c66 2c20 626c  bHandle(self, bl
+00005a60: 6f62 5f75 7269 2c20 6973 5f66 756c 6c3d  ob_uri, is_full=
+00005a70: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
+00005a80: 6765 745f 746f 7263 685f 626c 6f62 2873  get_torch_blob(s
+00005a90: 656c 662c 2062 6c6f 625f 7572 693a 2073  elf, blob_uri: s
+00005aa0: 7472 2920 2d3e 2027 546f 7263 6842 6c6f  tr) -> 'TorchBlo
+00005ab0: 6248 616e 646c 6527 3a0a 2020 2020 2020  bHandle':.      
+00005ac0: 2020 626c 6f62 5f74 7970 6520 3d20 7365    blob_type = se
+00005ad0: 6c66 2e67 6574 5f62 6c6f 625f 7479 7065  lf.get_blob_type
+00005ae0: 2862 6c6f 625f 7572 6929 0a20 2020 2020  (blob_uri).     
+00005af0: 2020 2069 6620 6e6f 7420 626c 6f62 5f74     if not blob_t
+00005b00: 7970 655b 2269 735f 746f 7263 6822 5d3a  ype["is_torch"]:
+00005b10: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00005b20: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00005b30: 626c 6f62 3a20 7b62 6c6f 625f 7572 697d  blob: {blob_uri}
+00005b40: 2069 7320 6e6f 7420 746f 7263 6820 7479   is not torch ty
+00005b50: 7065 2229 0a20 2020 2020 2020 2072 6574  pe").        ret
+00005b60: 7572 6e20 546f 7263 6842 6c6f 6248 616e  urn TorchBlobHan
+00005b70: 646c 6528 7365 6c66 2c20 626c 6f62 5f75  dle(self, blob_u
+00005b80: 7269 2c20 6973 5f66 756c 6c3d 4661 6c73  ri, is_full=Fals
+00005b90: 6529 0a0a 2020 2020 6465 6620 6765 745f  e)..    def get_
+00005ba0: 6375 7374 6f6d 5f63 6f64 655f 626c 6f62  custom_code_blob
+00005bb0: 2873 656c 662c 2062 6c6f 625f 7572 693a  (self, blob_uri:
+00005bc0: 2073 7472 2920 2d3e 2027 4375 7374 6f6d   str) -> 'Custom
+00005bd0: 436f 6465 426c 6f62 4861 6e64 6c65 273a  CodeBlobHandle':
+00005be0: 0a20 2020 2020 2020 2062 6c6f 625f 7479  .        blob_ty
+00005bf0: 7065 203d 2073 656c 662e 6765 745f 626c  pe = self.get_bl
+00005c00: 6f62 5f74 7970 6528 626c 6f62 5f75 7269  ob_type(blob_uri
+00005c10: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00005c20: 2062 6c6f 625f 7479 7065 5b22 6973 5f63   blob_type["is_c
+00005c30: 7573 746f 6d5f 636f 6465 225d 3a0a 2020  ustom_code"]:.  
+00005c40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00005c50: 5661 6c75 6545 7272 6f72 2866 2262 6c6f  ValueError(f"blo
+00005c60: 623a 207b 626c 6f62 5f75 7269 7d20 6973  b: {blob_uri} is
+00005c70: 206e 6f74 2063 7573 746f 6d20 636f 6465   not custom code
+00005c80: 2074 7970 6522 290a 2020 2020 2020 2020   type").        
+00005c90: 7265 7475 726e 2043 7573 746f 6d43 6f64  return CustomCod
+00005ca0: 6542 6c6f 6248 616e 646c 6528 7365 6c66  eBlobHandle(self
+00005cb0: 2c20 626c 6f62 5f75 7269 2c20 6973 5f66  , blob_uri, is_f
+00005cc0: 756c 6c3d 4661 6c73 6529 0a0a 2020 2020  ull=False)..    
+00005cd0: 6465 6620 6765 745f 6a73 6f6e 5f62 6c6f  def get_json_blo
+00005ce0: 6228 7365 6c66 2c20 626c 6f62 5f75 7269  b(self, blob_uri
+00005cf0: 3a20 7374 7229 202d 3e20 274a 534f 4e42  : str) -> 'JSONB
+00005d00: 6c6f 6248 616e 646c 6527 3a0a 2020 2020  lobHandle':.    
+00005d10: 2020 2020 626c 6f62 5f74 7970 6520 3d20      blob_type = 
+00005d20: 7365 6c66 2e67 6574 5f62 6c6f 625f 7479  self.get_blob_ty
+00005d30: 7065 2862 6c6f 625f 7572 6929 0a20 2020  pe(blob_uri).   
+00005d40: 2020 2020 2069 6620 6e6f 7420 626c 6f62       if not blob
+00005d50: 5f74 7970 655b 2269 735f 6a73 6f6e 225d  _type["is_json"]
+00005d60: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00005d70: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00005d80: 2262 6c6f 623a 207b 626c 6f62 5f75 7269  "blob: {blob_uri
+00005d90: 7d20 6973 206e 6f74 206a 736f 6e20 7479  } is not json ty
+00005da0: 7065 2229 0a20 2020 2020 2020 2072 6574  pe").        ret
+00005db0: 7572 6e20 4a53 4f4e 426c 6f62 4861 6e64  urn JSONBlobHand
+00005dc0: 6c65 2873 656c 662c 2062 6c6f 625f 7572  le(self, blob_ur
+00005dd0: 692c 2069 735f 6675 6c6c 3d46 616c 7365  i, is_full=False
+00005de0: 290a 0a20 2020 2064 6566 2064 7570 6c69  )..    def dupli
+00005df0: 6361 7465 5f64 6167 280a 2020 2020 2020  cate_dag(.      
+00005e00: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00005e10: 2020 2020 2020 2020 6461 675f 7572 693a          dag_uri:
+00005e20: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+00005e30: 2020 6465 7374 5f75 7269 3a20 4f70 7469    dest_uri: Opti
+00005e40: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00005e50: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00005e60: 7079 5f6e 6f6e 6f77 6e65 645f 626c 6f62  py_nonowned_blob
+00005e70: 733a 204f 7074 696f 6e61 6c5b 626f 6f6c  s: Optional[bool
+00005e80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00005e90: 2020 2020 2020 7265 7461 696e 5f6e 6f6e        retain_non
+00005ea0: 6f77 6e65 645f 626c 6f62 733a 2062 6f6f  owned_blobs: boo
+00005eb0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00005ec0: 2020 2020 2020 2077 6172 6e69 6e67 735f         warnings_
+00005ed0: 696f 3a20 4f70 7469 6f6e 616c 5b49 4f5b  io: Optional[IO[
+00005ee0: 416e 795d 5d20 3d20 7379 732e 7374 6465  Any]] = sys.stde
+00005ef0: 7272 2920 2d3e 2073 7472 3a0a 2020 2020  rr) -> str:.    
+00005f00: 2020 2020 6966 2063 6f70 795f 6e6f 6e6f      if copy_nono
+00005f10: 776e 6564 5f62 6c6f 6273 2069 7320 4e6f  wned_blobs is No
+00005f20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005f30: 636f 7079 5f6e 6f6e 6f77 6e65 645f 626c  copy_nonowned_bl
+00005f40: 6f62 7320 3d20 6e6f 7420 7265 7461 696e  obs = not retain
+00005f50: 5f6e 6f6e 6f77 6e65 645f 626c 6f62 730a  _nonowned_blobs.
+00005f60: 2020 2020 2020 2020 656c 6966 2077 6172          elif war
+00005f70: 6e69 6e67 735f 696f 2069 7320 6e6f 7420  nings_io is not 
+00005f80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005f90: 2020 7761 726e 696e 6773 5f69 6f2e 7772    warnings_io.wr
+00005fa0: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
+00005fb0: 2020 2020 2022 636f 7079 5f6e 6f6e 6f77       "copy_nonow
+00005fc0: 6e65 645f 626c 6f62 7320 6973 2064 6570  ned_blobs is dep
+00005fd0: 7265 6361 7465 643b 2022 0a20 2020 2020  recated; ".     
+00005fe0: 2020 2020 2020 2020 2020 2022 7573 6520             "use 
+00005ff0: 7265 7461 696e 5f6e 6f6e 6f77 6e65 645f  retain_nonowned_
+00006000: 626c 6f62 7320 696e 7374 6561 645c 6e22  blobs instead\n"
+00006010: 290a 2020 2020 2020 2020 2020 2020 7761  ).            wa
+00006020: 726e 696e 6773 5f69 6f2e 666c 7573 6828  rnings_io.flush(
+00006030: 290a 2020 2020 2020 2020 2320 4649 584d  ).        # FIXM
+00006040: 453a 2021 2121 7879 6d65 2d62 6163 6b65  E: !!!xyme-backe
+00006050: 6e64 2062 7567 2121 210a 2020 2020 2020  nd bug!!!.      
+00006060: 2020 636f 7079 5f6e 6f6e 6f77 6e65 645f    copy_nonowned_
+00006070: 626c 6f62 7320 3d20 6e6f 7420 636f 7079  blobs = not copy
+00006080: 5f6e 6f6e 6f77 6e65 645f 626c 6f62 730a  _nonowned_blobs.
+00006090: 2020 2020 2020 2020 6172 6773 203d 207b          args = {
+000060a0: 0a20 2020 2020 2020 2020 2020 2022 6461  .            "da
+000060b0: 6722 3a20 6461 675f 7572 692c 0a20 2020  g": dag_uri,.   
+000060c0: 2020 2020 2020 2020 2022 636f 7079 5f6e           "copy_n
+000060d0: 6f6e 6f77 6e65 645f 626c 6f62 7322 3a20  onowned_blobs": 
+000060e0: 636f 7079 5f6e 6f6e 6f77 6e65 645f 626c  copy_nonowned_bl
+000060f0: 6f62 732c 0a20 2020 2020 2020 207d 0a20  obs,.        }. 
+00006100: 2020 2020 2020 2069 6620 6465 7374 5f75         if dest_u
+00006110: 7269 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ri is not None:.
+00006120: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00006130: 5b22 6465 7374 225d 203d 2064 6573 745f  ["dest"] = dest_
+00006140: 7572 690a 2020 2020 2020 2020 7265 7475  uri.        retu
+00006150: 726e 2063 6173 7428 4461 6744 7570 5265  rn cast(DagDupRe
+00006160: 7370 6f6e 7365 2c20 7365 6c66 2e72 6571  sponse, self.req
+00006170: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00006180: 2020 2020 2020 204d 4554 484f 445f 504f         METHOD_PO
+00006190: 5354 2c20 222f 6461 675f 6475 7022 2c20  ST, "/dag_dup", 
+000061a0: 6172 6773 2929 5b22 6461 6722 5d0a 0a20  args))["dag"].. 
+000061b0: 2020 2064 6566 2073 6574 5f64 6167 280a     def set_dag(.
+000061c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000061d0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+000061e0: 675f 7572 693a 2073 7472 2c0a 2020 2020  g_uri: str,.    
+000061f0: 2020 2020 2020 2020 6465 6673 3a20 5573          defs: Us
+00006200: 6572 4461 6744 6566 2c0a 2020 2020 2020  erDagDef,.      
+00006210: 2020 2020 2020 7761 726e 696e 6773 5f69        warnings_i
+00006220: 6f3a 204f 7074 696f 6e61 6c5b 494f 5b41  o: Optional[IO[A
+00006230: 6e79 5d5d 203d 2073 7973 2e73 7464 6572  ny]] = sys.stder
+00006240: 7229 202d 3e20 2744 6167 4861 6e64 6c65  r) -> 'DagHandle
+00006250: 273a 0a20 2020 2020 2020 2064 6167 5f63  ':.        dag_c
+00006260: 7265 6174 6520 3d20 6361 7374 2844 6167  reate = cast(Dag
+00006270: 4372 6561 7465 2c20 7365 6c66 2e72 6571  Create, self.req
+00006280: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00006290: 2020 2020 2020 204d 4554 484f 445f 504f         METHOD_PO
+000062a0: 5354 2c20 222f 6461 675f 6372 6561 7465  ST, "/dag_create
+000062b0: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+000062c0: 2020 2020 2022 6461 6722 3a20 6461 675f       "dag": dag_
+000062d0: 7572 692c 0a20 2020 2020 2020 2020 2020  uri,.           
+000062e0: 2020 2020 2022 6465 6673 223a 2064 6566       "defs": def
+000062f0: 732c 0a20 2020 2020 2020 2020 2020 207d  s,.            }
+00006300: 2929 0a20 2020 2020 2020 2064 6167 5f75  )).        dag_u
+00006310: 7269 203d 2064 6167 5f63 7265 6174 655b  ri = dag_create[
+00006320: 2264 6167 225d 0a20 2020 2020 2020 2069  "dag"].        i
+00006330: 6620 7761 726e 696e 6773 5f69 6f20 6973  f warnings_io is
+00006340: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00006350: 2020 2020 2020 2077 6172 6e69 6e67 7320         warnings 
+00006360: 3d20 6461 675f 6372 6561 7465 5b22 7761  = dag_create["wa
+00006370: 726e 696e 6773 225d 0a20 2020 2020 2020  rnings"].       
+00006380: 2020 2020 2069 6620 6c65 6e28 7761 726e       if len(warn
+00006390: 696e 6773 2920 3e20 313a 0a20 2020 2020  ings) > 1:.     
+000063a0: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+000063b0: 6e67 735f 696f 2e77 7269 7465 280a 2020  ngs_io.write(.  
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 6622 7b6c 656e 2877 6172 6e69 6e67    f"{len(warning
+000063e0: 7329 7d20 7761 726e 696e 6773 2077 6869  s)} warnings whi
+000063f0: 6c65 2022 0a20 2020 2020 2020 2020 2020  le ".           
+00006400: 2020 2020 2020 2020 2066 2273 6574 7469           f"setti
+00006410: 6e67 2064 6167 207b 6461 675f 7572 697d  ng dag {dag_uri}
+00006420: 3a5c 6e22 290a 2020 2020 2020 2020 2020  :\n").          
+00006430: 2020 656c 6966 206c 656e 2877 6172 6e69    elif len(warni
+00006440: 6e67 7329 203d 3d20 313a 0a20 2020 2020  ngs) == 1:.     
+00006450: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00006460: 6e67 735f 696f 2e77 7269 7465 280a 2020  ngs_io.write(.  
+00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2020 6622 5761 726e 696e 6720 7768 696c    f"Warning whil
+00006490: 6520 7365 7474 696e 6720 6461 6720 7b64  e setting dag {d
+000064a0: 6167 5f75 7269 7d3a 5c6e 2229 0a20 2020  ag_uri}:\n").   
+000064b0: 2020 2020 2020 2020 2066 6f72 2077 6172           for war
+000064c0: 6e20 696e 2077 6172 6e69 6e67 733a 0a20  n in warnings:. 
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000064e0: 6172 6e69 6e67 735f 696f 2e77 7269 7465  arnings_io.write
+000064f0: 2866 227b 7761 726e 7d5c 6e22 290a 2020  (f"{warn}\n").  
+00006500: 2020 2020 2020 2020 2020 6966 2077 6172            if war
+00006510: 6e69 6e67 733a 0a20 2020 2020 2020 2020  nings:.         
+00006520: 2020 2020 2020 2077 6172 6e69 6e67 735f         warnings_
+00006530: 696f 2e66 6c75 7368 2829 0a20 2020 2020  io.flush().     
+00006540: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
+00006550: 6574 5f64 6167 2864 6167 5f75 7269 290a  et_dag(dag_uri).
+00006560: 0a20 2020 2064 6566 2073 6574 5f73 6574  .    def set_set
+00006570: 7469 6e67 7328 0a20 2020 2020 2020 2020  tings(.         
+00006580: 2020 2073 656c 662c 2063 6f6e 6669 675f     self, config_
+00006590: 746f 6b65 6e3a 2073 7472 2c20 7365 7474  token: str, sett
+000065a0: 696e 6773 3a20 5365 7474 696e 6773 4f62  ings: SettingsOb
+000065b0: 6a29 202d 3e20 5365 7474 696e 6773 4f62  j) -> SettingsOb
+000065c0: 6a3a 0a20 2020 2020 2020 2072 6574 7572  j:.        retur
+000065d0: 6e20 6361 7374 284e 616d 6573 7061 6365  n cast(Namespace
+000065e0: 5570 6461 7465 5365 7474 696e 6773 2c20  UpdateSettings, 
+000065f0: 7365 6c66 2e72 6571 7565 7374 5f6a 736f  self.request_jso
+00006600: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
+00006610: 4554 484f 445f 504f 5354 2c20 222f 7365  ETHOD_POST, "/se
+00006620: 7474 696e 6773 222c 207b 0a20 2020 2020  ttings", {.     
+00006630: 2020 2020 2020 2020 2020 2022 7365 7474             "sett
+00006640: 696e 6773 223a 2073 6574 7469 6e67 732c  ings": settings,
+00006650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006660: 2022 636f 6e66 6967 5f74 6f6b 656e 223a   "config_token":
+00006670: 2063 6f6e 6669 675f 746f 6b65 6e2c 0a20   config_token,. 
+00006680: 2020 2020 2020 2020 2020 207d 2929 5b22             }))["
+00006690: 7365 7474 696e 6773 225d 0a0a 2020 2020  settings"]..    
+000066a0: 6465 6620 6765 745f 7365 7474 696e 6773  def get_settings
+000066b0: 2873 656c 6629 202d 3e20 5365 7474 696e  (self) -> Settin
+000066c0: 6773 4f62 6a3a 0a20 2020 2020 2020 2072  gsObj:.        r
+000066d0: 6574 7572 6e20 6361 7374 284e 616d 6573  eturn cast(Names
+000066e0: 7061 6365 5570 6461 7465 5365 7474 696e  paceUpdateSettin
+000066f0: 6773 2c20 7365 6c66 2e72 6571 7565 7374  gs, self.request
+00006700: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
+00006710: 2020 204d 4554 484f 445f 4745 542c 2022     METHOD_GET, "
+00006720: 2f73 6574 7469 6e67 7322 2c20 7b7d 2929  /settings", {}))
+00006730: 5b22 7365 7474 696e 6773 225d 0a0a 2020  ["settings"]..  
+00006740: 2020 6465 6620 6765 745f 616c 6c6f 7765    def get_allowe
+00006750: 645f 6375 7374 6f6d 5f69 6d70 6f72 7473  d_custom_imports
+00006760: 2873 656c 6629 202d 3e20 416c 6c6f 7765  (self) -> Allowe
+00006770: 6443 7573 746f 6d49 6d70 6f72 7473 3a0a  dCustomImports:.
+00006780: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00006790: 6173 7428 416c 6c6f 7765 6443 7573 746f  ast(AllowedCusto
+000067a0: 6d49 6d70 6f72 7473 2c20 7365 6c66 2e72  mImports, self.r
+000067b0: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
+000067c0: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+000067d0: 4745 542c 2022 2f61 6c6c 6f77 6564 5f63  GET, "/allowed_c
+000067e0: 7573 746f 6d5f 696d 706f 7274 7322 2c20  ustom_imports", 
+000067f0: 7b7d 2c20 6164 645f 6e61 6d65 7370 6163  {}, add_namespac
+00006800: 653d 4661 6c73 6529 290a 0a20 2020 2040  e=False))..    @
+00006810: 6f76 6572 6c6f 6164 0a20 2020 2064 6566  overload.    def
+00006820: 2063 6865 636b 5f71 7565 7565 5f73 7461   check_queue_sta
+00006830: 7473 2820 2023 2070 796c 696e 743a 2064  ts(  # pylint: d
+00006840: 6973 6162 6c65 3d6e 6f2d 7365 6c66 2d75  isable=no-self-u
+00006850: 7365 0a20 2020 2020 2020 2020 2020 2073  se.            s
+00006860: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00006870: 2064 6167 3a20 4f70 7469 6f6e 616c 5b73   dag: Optional[s
+00006880: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
+00006890: 206d 696e 696d 616c 3a20 4c69 7465 7261   minimal: Litera
+000068a0: 6c5b 5472 7565 5d29 202d 3e20 4d69 6e69  l[True]) -> Mini
+000068b0: 6d61 6c51 7565 7565 5374 6174 7352 6573  malQueueStatsRes
+000068c0: 706f 6e73 653a 0a20 2020 2020 2020 202e  ponse:.        .
+000068d0: 2e2e 0a0a 2020 2020 406f 7665 726c 6f61  ....    @overloa
+000068e0: 640a 2020 2020 6465 6620 6368 6563 6b5f  d.    def check_
+000068f0: 7175 6575 655f 7374 6174 7328 2020 2320  queue_stats(  # 
+00006900: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00006910: 6e6f 2d73 656c 662d 7573 650a 2020 2020  no-self-use.    
+00006920: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00006930: 2020 2020 2020 2020 2020 6461 673a 204f            dag: O
+00006940: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+00006950: 2020 2020 2020 2020 2020 6d69 6e69 6d61            minima
+00006960: 6c3a 204c 6974 6572 616c 5b46 616c 7365  l: Literal[False
+00006970: 5d29 202d 3e20 5175 6575 6553 7461 7473  ]) -> QueueStats
+00006980: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00006990: 2020 2e2e 2e0a 0a20 2020 2040 6f76 6572    .....    @over
+000069a0: 6c6f 6164 0a20 2020 2064 6566 2063 6865  load.    def che
+000069b0: 636b 5f71 7565 7565 5f73 7461 7473 2820  ck_queue_stats( 
+000069c0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+000069d0: 6c65 3d6e 6f2d 7365 6c66 2d75 7365 0a20  le=no-self-use. 
+000069e0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+000069f0: 0a20 2020 2020 2020 2020 2020 2064 6167  .            dag
+00006a00: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d2c  : Optional[str],
+00006a10: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+00006a20: 696d 616c 3a20 626f 6f6c 2920 2d3e 2055  imal: bool) -> U
+00006a30: 6e69 6f6e 5b0a 2020 2020 2020 2020 2020  nion[.          
+00006a40: 2020 2020 2020 4d69 6e69 6d61 6c51 7565        MinimalQue
+00006a50: 7565 5374 6174 7352 6573 706f 6e73 652c  ueStatsResponse,
+00006a60: 2051 7565 7565 5374 6174 7352 6573 706f   QueueStatsRespo
+00006a70: 6e73 655d 3a0a 2020 2020 2020 2020 2e2e  nse]:.        ..
+00006a80: 2e0a 0a20 2020 2064 6566 2063 6865 636b  ...    def check
+00006a90: 5f71 7565 7565 5f73 7461 7473 280a 2020  _queue_stats(.  
+00006aa0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+00006ab0: 2020 2020 2020 2020 2020 2020 6461 673a              dag:
+00006ac0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00006ad0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00006ae0: 2020 206d 696e 696d 616c 3a20 626f 6f6c     minimal: bool
+00006af0: 203d 2046 616c 7365 2920 2d3e 2055 6e69   = False) -> Uni
+00006b00: 6f6e 5b0a 2020 2020 2020 2020 2020 2020  on[.            
+00006b10: 2020 2020 4d69 6e69 6d61 6c51 7565 7565      MinimalQueue
+00006b20: 5374 6174 7352 6573 706f 6e73 652c 2051  StatsResponse, Q
+00006b30: 7565 7565 5374 6174 7352 6573 706f 6e73  ueueStatsRespons
+00006b40: 655d 3a0a 2020 2020 2020 2020 6966 206d  e]:.        if m
+00006b50: 696e 696d 616c 3a0a 2020 2020 2020 2020  inimal:.        
+00006b60: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
+00006b70: 4d69 6e69 6d61 6c51 7565 7565 5374 6174  MinimalQueueStat
+00006b80: 7352 6573 706f 6e73 652c 2073 656c 662e  sResponse, self.
+00006b90: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+00006bb0: 5448 4f44 5f47 4554 2c20 222f 7175 6575  THOD_GET, "/queu
+00006bc0: 655f 7374 6174 7322 2c20 7b0a 2020 2020  e_stats", {.    
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2264 6167 223a 2064 6167 2c0a 2020 2020  "dag": dag,.    
+00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c00: 226d 696e 696d 616c 223a 2054 7275 652c  "minimal": True,
+00006c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c20: 207d 2929 0a20 2020 2020 2020 2072 6574   })).        ret
+00006c30: 7572 6e20 6361 7374 2851 7565 7565 5374  urn cast(QueueSt
+00006c40: 6174 7352 6573 706f 6e73 652c 2073 656c  atsResponse, sel
+00006c50: 662e 7265 7175 6573 745f 6a73 6f6e 280a  f.request_json(.
+00006c60: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00006c70: 4f44 5f47 4554 2c20 222f 7175 6575 655f  OD_GET, "/queue_
+00006c80: 7374 6174 7322 2c20 7b0a 2020 2020 2020  stats", {.      
+00006c90: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
+00006ca0: 2064 6167 2c0a 2020 2020 2020 2020 2020   dag,.          
+00006cb0: 2020 2020 2020 226d 696e 696d 616c 223a        "minimal":
+00006cc0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00006cd0: 2020 2020 7d29 290a 0a20 2020 2064 6566      }))..    def
+00006ce0: 2067 6574 5f69 6e73 7461 6e63 655f 7374   get_instance_st
+00006cf0: 6174 7573 280a 2020 2020 2020 2020 2020  atus(.          
+00006d00: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00006d10: 2020 2020 6461 675f 7572 693a 204f 7074      dag_uri: Opt
+00006d20: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00006d30: 652c 0a20 2020 2020 2020 2020 2020 206e  e,.            n
+00006d40: 6f64 655f 6964 3a20 4f70 7469 6f6e 616c  ode_id: Optional
+00006d50: 5b73 7472 5d20 3d20 4e6f 6e65 2920 2d3e  [str] = None) ->
+00006d60: 2044 6963 745b 496e 7374 616e 6365 5374   Dict[InstanceSt
+00006d70: 6174 7573 2c20 696e 745d 3a0a 2020 2020  atus, int]:.    
+00006d80: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
+00006d90: 4469 6374 5b49 6e73 7461 6e63 6553 7461  Dict[InstanceSta
+00006da0: 7475 732c 2069 6e74 5d2c 2073 656c 662e  tus, int], self.
+00006db0: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
+00006dc0: 2020 2020 2020 2020 2020 4d45 5448 4f44            METHOD
+00006dd0: 5f47 4554 2c20 222f 696e 7374 616e 6365  _GET, "/instance
+00006de0: 5f73 7461 7475 7322 2c20 7b0a 2020 2020  _status", {.    
+00006df0: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
+00006e00: 223a 2064 6167 5f75 7269 2c0a 2020 2020  ": dag_uri,.    
+00006e10: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
+00006e20: 6522 3a20 6e6f 6465 5f69 642c 0a20 2020  e": node_id,.   
+00006e30: 2020 2020 2020 2020 207d 2929 0a0a 2020           }))..  
+00006e40: 2020 6465 6620 6765 745f 7175 6575 655f    def get_queue_
+00006e50: 6d6f 6465 2873 656c 6629 202d 3e20 7374  mode(self) -> st
+00006e60: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+00006e70: 6e20 6361 7374 2851 7565 7565 4d6f 6465  n cast(QueueMode
+00006e80: 2c20 7365 6c66 2e72 6571 7565 7374 5f6a  , self.request_j
+00006e90: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00006ea0: 204d 4554 484f 445f 4745 542c 2022 2f71   METHOD_GET, "/q
+00006eb0: 7565 7565 5f6d 6f64 6522 2c20 7b7d 2c20  ueue_mode", {}, 
+00006ec0: 6164 645f 6e61 6d65 7370 6163 653d 4661  add_namespace=Fa
+00006ed0: 6c73 6529 295b 226d 6f64 6522 5d0a 0a20  lse))["mode"].. 
+00006ee0: 2020 2064 6566 2073 6574 5f71 7565 7565     def set_queue
+00006ef0: 5f6d 6f64 6528 7365 6c66 2c20 6d6f 6465  _mode(self, mode
+00006f00: 3a20 7374 7229 202d 3e20 7374 723a 0a20  : str) -> str:. 
+00006f10: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
+00006f20: 7374 2851 7565 7565 4d6f 6465 2c20 7365  st(QueueMode, se
+00006f30: 6c66 2e72 6571 7565 7374 5f6a 736f 6e28  lf.request_json(
+00006f40: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+00006f50: 484f 445f 5055 542c 2022 2f71 7565 7565  HOD_PUT, "/queue
+00006f60: 5f6d 6f64 6522 2c20 7b0a 2020 2020 2020  _mode", {.      
+00006f70: 2020 2020 2020 2020 2020 226d 6f64 6522            "mode"
+00006f80: 3a20 6d6f 6465 2c0a 2020 2020 2020 2020  : mode,.        
+00006f90: 2020 2020 7d2c 2061 6464 5f6e 616d 6573      }, add_names
+00006fa0: 7061 6365 3d46 616c 7365 2929 5b22 6d6f  pace=False))["mo
+00006fb0: 6465 225d 0a0a 2020 2020 6465 6620 666c  de"]..    def fl
+00006fc0: 7573 685f 616c 6c5f 7175 6575 655f 6461  ush_all_queue_da
+00006fd0: 7461 2873 656c 6629 202d 3e20 4e6f 6e65  ta(self) -> None
+00006fe0: 3a0a 0a20 2020 2020 2020 2064 6566 2064  :..        def d
+00006ff0: 6f5f 666c 7573 6828 2920 2d3e 2062 6f6f  o_flush() -> boo
+00007000: 6c3a 0a20 2020 2020 2020 2020 2020 2072  l:.            r
+00007010: 6573 203d 2063 6173 7428 466c 7573 6841  es = cast(FlushA
+00007020: 6c6c 5175 6575 6573 5265 7370 6f6e 7365  llQueuesResponse
+00007030: 2c20 7365 6c66 2e72 6571 7565 7374 5f6a  , self.request_j
+00007040: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00007050: 2020 2020 204d 4554 484f 445f 504f 5354       METHOD_POST
+00007060: 2c20 222f 666c 7573 685f 616c 6c5f 7175  , "/flush_all_qu
+00007070: 6575 6573 222c 207b 7d2c 2061 6464 5f6e  eues", {}, add_n
+00007080: 616d 6573 7061 6365 3d46 616c 7365 2929  amespace=False))
+00007090: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000070a0: 7572 6e20 626f 6f6c 2872 6573 5b22 7375  urn bool(res["su
+000070b0: 6363 6573 7322 5d29 0a0a 2020 2020 2020  ccess"])..      
+000070c0: 2020 7768 696c 6520 646f 5f66 6c75 7368    while do_flush
+000070d0: 2829 3a20 2023 2077 6520 666c 7573 6820  ():  # we flush 
+000070e0: 756e 7469 6c20 7468 6572 6520 6973 206e  until there is n
+000070f0: 6f74 6869 6e67 2074 6f20 666c 7573 6820  othing to flush 
+00007100: 616e 796d 6f72 650a 2020 2020 2020 2020  anymore.        
+00007110: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00007120: 2e30 290a 0a20 2020 2064 6566 2067 6574  .0)..    def get
+00007130: 5f63 6163 6865 5f73 7461 7473 2873 656c  _cache_stats(sel
+00007140: 6629 202d 3e20 4361 6368 6553 7461 7473  f) -> CacheStats
+00007150: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00007160: 2063 6173 7428 4361 6368 6553 7461 7473   cast(CacheStats
+00007170: 2c20 7365 6c66 2e72 6571 7565 7374 5f6a  , self.request_j
+00007180: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00007190: 204d 4554 484f 445f 4745 542c 2022 2f63   METHOD_GET, "/c
+000071a0: 6163 6865 5f73 7461 7473 222c 207b 7d2c  ache_stats", {},
+000071b0: 2061 6464 5f6e 616d 6573 7061 6365 3d46   add_namespace=F
+000071c0: 616c 7365 2929 0a0a 2020 2020 6465 6620  alse))..    def 
+000071d0: 7265 7365 745f 6361 6368 6528 7365 6c66  reset_cache(self
+000071e0: 2920 2d3e 2043 6163 6865 5374 6174 733a  ) -> CacheStats:
+000071f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007200: 6361 7374 2843 6163 6865 5374 6174 732c  cast(CacheStats,
+00007210: 2073 656c 662e 7265 7175 6573 745f 6a73   self.request_js
+00007220: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00007230: 4d45 5448 4f44 5f50 4f53 542c 2022 2f63  METHOD_POST, "/c
+00007240: 6163 6865 5f72 6573 6574 222c 207b 7d2c  ache_reset", {},
+00007250: 2061 6464 5f6e 616d 6573 7061 6365 3d46   add_namespace=F
+00007260: 616c 7365 2929 0a0a 2020 2020 6465 6620  alse))..    def 
+00007270: 6372 6561 7465 5f6b 6166 6b61 5f65 7272  create_kafka_err
+00007280: 6f72 5f74 6f70 6963 2873 656c 6629 202d  or_topic(self) -
+00007290: 3e20 4b61 666b 6154 6f70 6963 733a 0a20  > KafkaTopics:. 
+000072a0: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
+000072b0: 7374 284b 6166 6b61 546f 7069 6373 2c20  st(KafkaTopics, 
+000072c0: 7365 6c66 2e72 6571 7565 7374 5f6a 736f  self.request_jso
+000072d0: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
+000072e0: 4554 484f 445f 504f 5354 2c20 222f 6b61  ETHOD_POST, "/ka
+000072f0: 666b 615f 746f 7069 6373 222c 207b 0a20  fka_topics", {. 
+00007300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007310: 6e75 6d5f 7061 7274 6974 696f 6e73 223a  num_partitions":
+00007320: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+00007330: 7d29 290a 0a20 2020 2064 6566 2067 6574  }))..    def get
+00007340: 5f6b 6166 6b61 5f65 7272 6f72 5f74 6f70  _kafka_error_top
+00007350: 6963 2873 656c 6629 202d 3e20 7374 723a  ic(self) -> str:
+00007360: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
+00007370: 6173 7428 4b61 666b 6154 6f70 6963 4e61  ast(KafkaTopicNa
+00007380: 6d65 732c 2073 656c 662e 7265 7175 6573  mes, self.reques
+00007390: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+000073a0: 2020 2020 4d45 5448 4f44 5f47 4554 2c20      METHOD_GET, 
+000073b0: 222f 6b61 666b 615f 746f 7069 635f 6e61  "/kafka_topic_na
+000073c0: 6d65 7322 2c20 7b7d 2929 5b22 6572 726f  mes", {}))["erro
+000073d0: 7222 5d0a 2020 2020 2020 2020 6173 7365  r"].        asse
+000073e0: 7274 2072 6573 2069 7320 6e6f 7420 4e6f  rt res is not No
+000073f0: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+00007400: 6e20 7265 730a 0a20 2020 2064 6566 2067  n res..    def g
+00007410: 6574 5f6b 6166 6b61 5f65 7272 6f72 5f6d  et_kafka_error_m
+00007420: 6573 7361 6765 5f74 6f70 6963 2873 656c  essage_topic(sel
+00007430: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+00007440: 2020 2072 6573 203d 2063 6173 7428 4b61     res = cast(Ka
+00007450: 666b 6154 6f70 6963 4e61 6d65 732c 2073  fkaTopicNames, s
+00007460: 656c 662e 7265 7175 6573 745f 6a73 6f6e  elf.request_json
+00007470: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
+00007480: 5448 4f44 5f47 4554 2c20 222f 6b61 666b  THOD_GET, "/kafk
+00007490: 615f 746f 7069 635f 6e61 6d65 7322 2c20  a_topic_names", 
+000074a0: 7b7d 2929 5b22 6572 726f 725f 6d73 6722  {}))["error_msg"
+000074b0: 5d0a 2020 2020 2020 2020 6173 7365 7274  ].        assert
+000074c0: 2072 6573 2069 7320 6e6f 7420 4e6f 6e65   res is not None
+000074d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000074e0: 7265 730a 0a20 2020 2064 6566 2064 656c  res..    def del
+000074f0: 6574 655f 6b61 666b 615f 6572 726f 725f  ete_kafka_error_
+00007500: 746f 7069 6328 7365 6c66 2920 2d3e 204b  topic(self) -> K
+00007510: 6166 6b61 546f 7069 6373 3a0a 2020 2020  afkaTopics:.    
+00007520: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
+00007530: 4b61 666b 6154 6f70 6963 732c 2073 656c  KafkaTopics, sel
+00007540: 662e 7265 7175 6573 745f 6a73 6f6e 280a  f.request_json(.
+00007550: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00007560: 4f44 5f50 4f53 542c 2022 2f6b 6166 6b61  OD_POST, "/kafka
+00007570: 5f74 6f70 6963 7322 2c20 7b0a 2020 2020  _topics", {.    
+00007580: 2020 2020 2020 2020 2020 2020 226e 756d              "num
+00007590: 5f70 6172 7469 7469 6f6e 7322 3a20 302c  _partitions": 0,
+000075a0: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
+000075b0: 0a0a 2020 2020 6465 6620 7265 6164 5f6b  ..    def read_k
+000075c0: 6166 6b61 5f65 7272 6f72 7328 0a20 2020  afka_errors(.   
+000075d0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+000075e0: 2020 2020 2020 2020 2020 2063 6f6e 7375             consu
+000075f0: 6d65 725f 7479 7065 3a20 7374 722c 0a20  mer_type: str,. 
+00007600: 2020 2020 2020 2020 2020 206f 6666 7365             offse
+00007610: 743a 2073 7472 203d 2022 6375 7272 656e  t: str = "curren
+00007620: 7422 2920 2d3e 204c 6973 745b 7374 725d  t") -> List[str]
+00007630: 3a0a 2020 2020 2020 2020 6966 2063 6f6e  :.        if con
+00007640: 7375 6d65 725f 7479 7065 206e 6f74 2069  sumer_type not i
+00007650: 6e20 434f 4e53 554d 4552 5f54 5950 4553  n CONSUMER_TYPES
+00007660: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00007670: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007690: 6622 636f 6e73 756d 6572 5f74 7970 6520  f"consumer_type 
+000076a0: 6361 6e6e 6f74 2062 6520 7b63 6f6e 7375  cannot be {consu
+000076b0: 6d65 725f 7479 7065 7d20 220a 2020 2020  mer_type} ".    
+000076c0: 2020 2020 2020 2020 2020 2020 2266 6f72              "for
+000076d0: 2072 6561 6469 6e67 206b 6166 6b61 2065   reading kafka e
+000076e0: 7272 6f72 732e 2070 726f 7669 6465 2063  rrors. provide c
+000076f0: 6f6e 7375 6d65 7220 7479 7065 2066 726f  onsumer type fro
+00007700: 6d20 220a 2020 2020 2020 2020 2020 2020  m ".            
+00007710: 2020 2020 6622 7b43 4f4e 5355 4d45 525f      f"{CONSUMER_
+00007720: 5459 5045 537d 2229 0a20 2020 2020 2020  TYPES}").       
+00007730: 2072 6574 7572 6e20 6361 7374 284c 6973   return cast(Lis
+00007740: 745b 7374 725d 2c20 7365 6c66 2e72 6571  t[str], self.req
+00007750: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00007760: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
+00007770: 542c 2022 2f6b 6166 6b61 5f6d 7367 222c  T, "/kafka_msg",
+00007780: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00007790: 2020 2022 6f66 6673 6574 223a 206f 6666     "offset": off
+000077a0: 7365 742c 0a20 2020 2020 2020 2020 2020  set,.           
+000077b0: 2020 2020 2022 636f 6e73 756d 6572 5f74       "consumer_t
+000077c0: 7970 6522 3a20 636f 6e73 756d 6572 5f74  ype": consumer_t
+000077d0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+000077e0: 207d 2929 0a0a 2020 2020 6465 6620 7265   }))..    def re
+000077f0: 6164 5f6b 6166 6b61 5f66 756c 6c5f 6a73  ad_kafka_full_js
+00007800: 6f6e 5f65 7272 6f72 7328 0a20 2020 2020  on_errors(.     
+00007810: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00007820: 2020 2020 2020 2020 2069 6e70 7574 5f69           input_i
+00007830: 645f 7061 7468 3a20 4c69 7374 5b73 7472  d_path: List[str
+00007840: 5d2c 0a20 2020 2020 2020 2020 2020 2065  ],.            e
+00007850: 7272 5f6d 7367 5f73 7461 7465 3a20 4b61  rr_msg_state: Ka
+00007860: 666b 6145 7272 6f72 4d65 7373 6167 6553  fkaErrorMessageS
+00007870: 7461 7465 2c0a 2020 2020 2020 2020 2020  tate,.          
+00007880: 2020 2920 2d3e 2049 7465 7261 626c 655b    ) -> Iterable[
+00007890: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
+000078a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000078b0: 2020 2020 2020 5072 6f76 6964 6573 2069        Provides i
+000078c0: 6e66 6f72 6d61 7469 6f6e 2061 7320 746f  nformation as to
+000078d0: 2077 6861 7420 7468 6520 6572 726f 7220   what the error 
+000078e0: 6973 2061 6e64 2077 6861 7420 6973 2074  is and what is t
+000078f0: 6865 0a20 2020 2020 2020 2069 6e70 7574  he.        input
+00007900: 2069 6420 616e 6420 6974 7320 6173 736f   id and its asso
+00007910: 6369 6174 6564 2069 6e70 7574 206d 6573  ciated input mes
+00007920: 7361 6765 2e0a 0a20 2020 2020 2020 2041  sage...        A
+00007930: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00007940: 2069 6e70 7574 5f69 645f 7061 7468 2028   input_id_path (
+00007950: 4c69 7374 5b73 7472 5d29 3a0a 2020 2020  List[str]):.    
+00007960: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00007970: 7061 7468 206f 6620 7468 6520 6669 656c  path of the fiel
+00007980: 6420 746f 2062 6520 636f 6e73 6964 6572  d to be consider
+00007990: 6564 2061 7320 696e 7075 745f 6964 2069  ed as input_id i
+000079a0: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
+000079b0: 2020 2020 2020 696e 7075 7420 6a73 6f6e        input json
+000079c0: 2e0a 2020 2020 2020 2020 2020 2020 6572  ..            er
+000079d0: 725f 6d73 675f 7374 6174 6520 284b 6166  r_msg_state (Kaf
+000079e0: 6b61 4572 726f 724d 6573 7361 6765 5374  kaErrorMessageSt
+000079f0: 6174 6529 3a0a 2020 2020 2020 2020 2020  ate):.          
+00007a00: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
+00007a10: 6265 2070 6f70 756c 6174 6564 2077 6974  be populated wit
+00007a20: 6820 7468 6520 6d61 7070 696e 6773 206f  h the mappings o
+00007a30: 6620 696e 7075 745f 6964 730a 2020 2020  f input_ids.    
+00007a40: 2020 2020 2020 2020 2020 2020 746f 206d              to m
+00007a50: 6573 7361 6765 732e 2041 6c73 6f20 7374  essages. Also st
+00007a60: 6f72 6573 2061 6e79 2075 6e6d 6174 6368  ores any unmatch
+00007a70: 6564 206d 6573 7361 6765 7320 696e 2074  ed messages in t
+00007a80: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+00007a90: 2020 2075 6e6d 6174 6368 6564 206c 6973     unmatched lis
+00007aa0: 7420 616e 6420 6166 7465 7220 6669 6c6c  t and after fill
+00007ab0: 696e 6720 6d73 675f 6c6f 6f6b 7570 2c20  ing msg_lookup, 
+00007ac0: 6368 6563 6b20 6966 2074 6865 790a 2020  check if they.  
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 6861                ha
+00007ae0: 7665 206d 6174 6368 6573 2e20 496e 6974  ve matches. Init
+00007af0: 6961 6c6c 7920 616e 206f 626a 6563 7420  ially an object 
+00007b00: 6f66 204b 6166 6b61 4572 726f 724d 6573  of KafkaErrorMes
+00007b10: 7361 6765 5374 6174 650a 2020 2020 2020  sageState.      
+00007b20: 2020 2020 2020 2020 2020 6361 6e20 6265            can be
+00007b30: 2070 6173 7365 6420 666f 7220 7468 6973   passed for this
+00007b40: 2061 7267 756d 656e 742e 0a0a 2020 2020   argument...    
+00007b50: 2020 2020 5969 656c 6473 3a0a 2020 2020      Yields:.    
+00007b60: 2020 2020 2020 2020 4974 6572 6162 6c65          Iterable
+00007b70: 5b54 7570 6c65 5b73 7472 2c20 4f70 7469  [Tuple[str, Opti
+00007b80: 6f6e 616c 5b73 7472 5d5d 5d3a 2074 6865  onal[str]]]: the
+00007b90: 2065 7272 6f72 2c20 7468 6520 696e 7075   error, the inpu
+00007ba0: 7420 6d73 670a 2020 2020 2020 2020 2020  t msg.          
+00007bb0: 2020 6173 736f 6369 6174 6564 2077 6974    associated wit
+00007bc0: 6820 7468 6520 696e 7075 745f 6964 2e0a  h the input_id..
+00007bd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007be0: 2020 2020 6572 7273 203d 2073 656c 662e      errs = self.
+00007bf0: 7265 6164 5f6b 6166 6b61 5f65 7272 6f72  read_kafka_error
+00007c00: 7328 636f 6e73 756d 6572 5f74 7970 653d  s(consumer_type=
+00007c10: 434f 4e53 554d 4552 5f45 5252 290a 2020  CONSUMER_ERR).  
+00007c20: 2020 2020 2020 6d73 6773 203d 2073 656c        msgs = sel
+00007c30: 662e 7265 6164 5f6b 6166 6b61 5f65 7272  f.read_kafka_err
+00007c40: 6f72 7328 636f 6e73 756d 6572 5f74 7970  ors(consumer_typ
+00007c50: 653d 434f 4e53 554d 4552 5f45 5252 5f4d  e=CONSUMER_ERR_M
+00007c60: 5347 290a 0a20 2020 2020 2020 2064 6566  SG)..        def
+00007c70: 2070 6172 7365 5f69 6e70 7574 5f69 645f   parse_input_id_
+00007c80: 6a73 6f6e 286a 736f 6e5f 7374 723a 2073  json(json_str: s
+00007c90: 7472 2920 2d3e 204f 7074 696f 6e61 6c5b  tr) -> Optional[
+00007ca0: 7374 725d 3a0a 2020 2020 2020 2020 2020  str]:.          
+00007cb0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00007cc0: 2020 2020 2020 2072 6573 203d 206a 736f         res = jso
+00007cd0: 6e2e 6c6f 6164 7328 6a73 6f6e 5f73 7472  n.loads(json_str
+00007ce0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007cf0: 2020 666f 7220 7061 7468 2069 6e20 696e    for path in in
+00007d00: 7075 745f 6964 5f70 6174 683a 0a20 2020  put_id_path:.   
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 2072 6573 203d 2072 6573 5b70 6174 685d   res = res[path]
+00007d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d40: 2072 6574 7572 6e20 7265 730a 2020 2020   return res.    
+00007d50: 2020 2020 2020 2020 6578 6365 7074 206a          except j
+00007d60: 736f 6e2e 6465 636f 6465 722e 4a53 4f4e  son.decoder.JSON
+00007d70: 4465 636f 6465 4572 726f 723a 0a20 2020  DecodeError:.   
+00007d80: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007d90: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00007da0: 2020 2020 2065 7863 6570 7420 4b65 7945       except KeyE
+00007db0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00007dc0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00007dd0: 650a 0a20 2020 2020 2020 2064 6566 2070  e..        def p
+00007de0: 6172 7365 5f69 6e70 7574 5f69 645f 7465  arse_input_id_te
+00007df0: 7874 2874 6578 743a 2073 7472 2920 2d3e  xt(text: str) ->
+00007e00: 204f 7074 696f 6e61 6c5b 7374 725d 3a0a   Optional[str]:.
+00007e10: 2020 2020 2020 2020 2020 2020 6978 203d              ix =
+00007e20: 2074 6578 742e 6669 6e64 2822 5c6e 696e   text.find("\nin
+00007e30: 7075 745f 6964 3a20 2229 0a20 2020 2020  put_id: ").     
+00007e40: 2020 2020 2020 2069 6620 6978 2021 3d20         if ix != 
+00007e50: 2d31 3a0a 2020 2020 2020 2020 2020 2020  -1:.            
+00007e60: 2020 2020 7265 7475 726e 2074 6578 745b      return text[
+00007e70: 6978 202b 206c 656e 2822 5c6e 696e 7075  ix + len("\ninpu
+00007e80: 745f 6964 3a20 2229 3a5d 0a20 2020 2020  t_id: "):].     
+00007e90: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00007ea0: 6e65 0a0a 2020 2020 2020 2020 666f 7220  ne..        for 
+00007eb0: 6d73 6720 696e 206d 7367 733a 0a20 2020  msg in msgs:.   
+00007ec0: 2020 2020 2020 2020 2069 6e70 7574 5f69           input_i
+00007ed0: 6420 3d20 7061 7273 655f 696e 7075 745f  d = parse_input_
+00007ee0: 6964 5f6a 736f 6e28 6d73 6729 0a20 2020  id_json(msg).   
+00007ef0: 2020 2020 2020 2020 2069 6620 696e 7075           if inpu
+00007f00: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00007f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007f20: 2020 6572 725f 6d73 675f 7374 6174 652e    err_msg_state.
+00007f30: 6164 645f 6d73 6728 696e 7075 745f 6964  add_msg(input_id
+00007f40: 2c20 6d73 6729 0a20 2020 2020 2020 2066  , msg).        f
+00007f50: 6f72 206f 6c64 5f65 7272 2069 6e20 6572  or old_err in er
+00007f60: 725f 6d73 675f 7374 6174 652e 6765 745f  r_msg_state.get_
+00007f70: 756e 6d61 7463 6865 6428 293a 0a20 2020  unmatched():.   
+00007f80: 2020 2020 2020 2020 2069 6e70 7574 5f69           input_i
+00007f90: 6420 3d20 7061 7273 655f 696e 7075 745f  d = parse_input_
+00007fa0: 6964 5f74 6578 7428 6f6c 645f 6572 7229  id_text(old_err)
+00007fb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007fc0: 696e 7075 745f 6964 2069 7320 4e6f 6e65  input_id is None
+00007fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007fe0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00007ff0: 2020 2020 2020 206d 6174 6368 203d 2065         match = e
+00008000: 7272 5f6d 7367 5f73 7461 7465 2e67 6574  rr_msg_state.get
+00008010: 5f6d 7367 2869 6e70 7574 5f69 6429 0a20  _msg(input_id). 
+00008020: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
+00008030: 7463 6820 6973 204e 6f6e 653a 0a20 2020  tch is None:.   
+00008040: 2020 2020 2020 2020 2020 2020 2065 7272               err
+00008050: 5f6d 7367 5f73 7461 7465 2e61 6464 5f75  _msg_state.add_u
+00008060: 6e6d 6174 6368 6564 286f 6c64 5f65 7272  nmatched(old_err
+00008070: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00008080: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008090: 2020 2020 7969 656c 6420 286f 6c64 5f65      yield (old_e
+000080a0: 7272 2c20 6d61 7463 6829 0a20 2020 2020  rr, match).     
+000080b0: 2020 2066 6f72 2065 7272 2069 6e20 6572     for err in er
+000080c0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+000080d0: 696e 7075 745f 6964 203d 2070 6172 7365  input_id = parse
+000080e0: 5f69 6e70 7574 5f69 645f 7465 7874 2865  _input_id_text(e
+000080f0: 7272 290a 2020 2020 2020 2020 2020 2020  rr).            
+00008100: 6966 2069 6e70 7574 5f69 6420 6973 204e  if input_id is N
+00008110: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00008120: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00008130: 2020 2020 2020 2020 2020 6d61 7463 6820            match 
+00008140: 3d20 6572 725f 6d73 675f 7374 6174 652e  = err_msg_state.
+00008150: 6765 745f 6d73 6728 696e 7075 745f 6964  get_msg(input_id
+00008160: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00008170: 206d 6174 6368 2069 7320 4e6f 6e65 3a0a   match is None:.
+00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008190: 6572 725f 6d73 675f 7374 6174 652e 6164  err_msg_state.ad
+000081a0: 645f 756e 6d61 7463 6865 6428 6572 7229  d_unmatched(err)
+000081b0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+000081c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000081d0: 2020 2079 6965 6c64 2028 6572 722c 206d     yield (err, m
+000081e0: 6174 6368 290a 0a20 2020 2064 6566 2067  atch)..    def g
+000081f0: 6574 5f6e 616d 6564 5f73 6563 7265 7473  et_named_secrets
+00008200: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00008210: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00008220: 636f 6e66 6967 5f74 6f6b 656e 3a20 4f70  config_token: Op
+00008230: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00008240: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00008250: 7368 6f77 5f76 616c 7565 733a 2062 6f6f  show_values: boo
+00008260: 6c20 3d20 4661 6c73 6529 202d 3e20 4469  l = False) -> Di
+00008270: 6374 5b73 7472 2c20 4f70 7469 6f6e 616c  ct[str, Optional
+00008280: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+00008290: 6966 2073 686f 775f 7661 6c75 6573 2061  if show_values a
+000082a0: 6e64 2063 6f6e 6669 675f 746f 6b65 6e20  nd config_token 
+000082b0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000082c0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000082d0: 4572 726f 7228 2263 6f6e 6669 675f 746f  Error("config_to
+000082e0: 6b65 6e20 6d75 7374 2062 6520 7365 7420  ken must be set 
+000082f0: 746f 2073 686f 775f 7661 6c75 6573 2229  to show_values")
+00008300: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008310: 6361 7374 2844 6963 745b 7374 722c 204f  cast(Dict[str, O
+00008320: 7074 696f 6e61 6c5b 7374 725d 5d2c 2073  ptional[str]], s
+00008330: 656c 662e 7265 7175 6573 745f 6a73 6f6e  elf.request_json
+00008340: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
+00008350: 5448 4f44 5f47 4554 2c20 222f 6e61 6d65  THOD_GET, "/name
+00008360: 645f 7365 6372 6574 7322 2c20 7b0a 2020  d_secrets", {.  
+00008370: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00008380: 686f 7722 3a20 696e 7428 626f 6f6c 2873  how": int(bool(s
+00008390: 686f 775f 7661 6c75 6573 2929 2c0a 2020  how_values)),.  
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000083b0: 6f6e 6669 675f 746f 6b65 6e22 3a20 636f  onfig_token": co
+000083c0: 6e66 6967 5f74 6f6b 656e 2c0a 2020 2020  nfig_token,.    
+000083d0: 2020 2020 2020 2020 7d29 290a 0a20 2020          }))..   
+000083e0: 2064 6566 2073 6574 5f6e 616d 6564 5f73   def set_named_s
+000083f0: 6563 7265 7428 0a20 2020 2020 2020 2020  ecret(.         
+00008400: 2020 2073 656c 662c 2063 6f6e 6669 675f     self, config_
+00008410: 746f 6b65 6e3a 2073 7472 2c20 6b65 793a  token: str, key:
+00008420: 2073 7472 2c20 7661 6c75 653a 2073 7472   str, value: str
+00008430: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00008440: 2020 2072 6574 7572 6e20 6361 7374 2853     return cast(S
+00008450: 6574 4e61 6d65 6453 6563 7265 742c 2073  etNamedSecret, s
+00008460: 656c 662e 7265 7175 6573 745f 6a73 6f6e  elf.request_json
+00008470: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
+00008480: 5448 4f44 5f50 5554 2c20 222f 6e61 6d65  THOD_PUT, "/name
+00008490: 645f 7365 6372 6574 7322 2c20 7b0a 2020  d_secrets", {.  
+000084a0: 2020 2020 2020 2020 2020 2020 2020 226b                "k
+000084b0: 6579 223a 206b 6579 2c0a 2020 2020 2020  ey": key,.      
+000084c0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+000084d0: 223a 2076 616c 7565 2c0a 2020 2020 2020  ": value,.      
+000084e0: 2020 2020 2020 2020 2020 2263 6f6e 6669            "confi
+000084f0: 675f 746f 6b65 6e22 3a20 636f 6e66 6967  g_token": config
+00008500: 5f74 6f6b 656e 2c0a 2020 2020 2020 2020  _token,.        
+00008510: 2020 2020 7d29 295b 2272 6570 6c61 6365      }))["replace
+00008520: 6422 5d0a 0a20 2020 2064 6566 2067 6574  d"]..    def get
+00008530: 5f65 7272 6f72 5f6c 6f67 7328 7365 6c66  _error_logs(self
+00008540: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00008550: 2020 7769 7468 2073 656c 662e 5f72 6177    with self._raw
+00008560: 5f72 6571 7565 7374 5f73 7472 284d 4554  _request_str(MET
+00008570: 484f 445f 4745 542c 2022 2f65 7272 6f72  HOD_GET, "/error
+00008580: 5f6c 6f67 7322 2c20 7b7d 2920 6173 2066  _logs", {}) as f
+00008590: 696e 3a0a 2020 2020 2020 2020 2020 2020  in:.            
+000085a0: 7265 7475 726e 2066 696e 2e72 6561 6428  return fin.read(
+000085b0: 290a 0a20 2020 2064 6566 2067 6574 5f6b  )..    def get_k
+000085c0: 6e6f 776e 5f62 6c6f 6273 280a 2020 2020  nown_blobs(.    
+000085d0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000085e0: 2020 2020 2020 2020 2020 626c 6f62 5f74            blob_t
+000085f0: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+00008600: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00008610: 2020 2020 2020 2063 6f6e 6e65 6374 6f72         connector
+00008620: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00008630: 3d20 4e6f 6e65 2920 2d3e 204c 6973 745b  = None) -> List[
+00008640: 7374 725d 3a0a 2020 2020 2020 2020 7265  str]:.        re
+00008650: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
+00008660: 2020 2072 6573 5b30 5d0a 2020 2020 2020     res[0].      
+00008670: 2020 2020 2020 666f 7220 7265 7320 696e        for res in
+00008680: 2073 656c 662e 6765 745f 6b6e 6f77 6e5f   self.get_known_
+00008690: 626c 6f62 5f74 696d 6573 280a 2020 2020  blob_times(.    
+000086a0: 2020 2020 2020 2020 2020 2020 7265 7472              retr
+000086b0: 6965 7665 5f74 696d 6573 3d46 616c 7365  ieve_times=False
+000086c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000086d0: 2020 626c 6f62 5f74 7970 653d 626c 6f62    blob_type=blob
+000086e0: 5f74 7970 652c 0a20 2020 2020 2020 2020  _type,.         
+000086f0: 2020 2020 2020 2063 6f6e 6e65 6374 6f72         connector
+00008700: 3d63 6f6e 6e65 6374 6f72 295b 315d 0a20  =connector)[1]. 
+00008710: 2020 2020 2020 205d 0a0a 2020 2020 6465         ]..    de
+00008720: 6620 6765 745f 6b6e 6f77 6e5f 626c 6f62  f get_known_blob
+00008730: 5f61 6765 7328 0a20 2020 2020 2020 2020  _ages(.         
+00008740: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00008750: 2020 2020 2062 6c6f 625f 7479 7065 3a20       blob_type: 
+00008760: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00008770: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00008780: 2020 636f 6e6e 6563 746f 723a 204f 7074    connector: Opt
+00008790: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000087a0: 6529 202d 3e20 4c69 7374 5b54 7570 6c65  e) -> List[Tuple
+000087b0: 5b73 7472 2c20 7374 725d 5d3a 0a20 2020  [str, str]]:.   
+000087c0: 2020 2020 2063 7572 5f74 696d 652c 2062       cur_time, b
+000087d0: 6c6f 6273 203d 2073 656c 662e 6765 745f  lobs = self.get_
+000087e0: 6b6e 6f77 6e5f 626c 6f62 5f74 696d 6573  known_blob_times
+000087f0: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+00008800: 7472 6965 7665 5f74 696d 6573 3d54 7275  trieve_times=Tru
+00008810: 652c 2062 6c6f 625f 7479 7065 3d62 6c6f  e, blob_type=blo
+00008820: 625f 7479 7065 2c20 636f 6e6e 6563 746f  b_type, connecto
+00008830: 723d 636f 6e6e 6563 746f 7229 0a20 2020  r=connector).   
+00008840: 2020 2020 2072 6574 7572 6e20 5b0a 2020       return [.  
+00008850: 2020 2020 2020 2020 2020 2862 6c6f 625f            (blob_
+00008860: 6964 2c20 6765 745f 6167 6528 6375 725f  id, get_age(cur_
+00008870: 7469 6d65 2c20 626c 6f62 5f74 696d 6529  time, blob_time)
+00008880: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+00008890: 7220 2862 6c6f 625f 6964 2c20 626c 6f62  r (blob_id, blob
+000088a0: 5f74 696d 6529 2069 6e20 736f 7274 6564  _time) in sorted
+000088b0: 2862 6c6f 6273 2c20 6b65 793d 6c61 6d62  (blobs, key=lamb
+000088c0: 6461 2065 6c3a 2028 0a20 2020 2020 2020  da el: (.       
+000088d0: 2020 2020 2020 2020 2073 6166 655f 6f70           safe_op
+000088e0: 745f 6e75 6d28 656c 5b31 5d29 2c20 656c  t_num(el[1]), el
+000088f0: 5b30 5d29 290a 2020 2020 2020 2020 5d0a  [0])).        ].
+00008900: 0a20 2020 2064 6566 2067 6574 5f6b 6e6f  .    def get_kno
+00008910: 776e 5f62 6c6f 625f 7469 6d65 7328 0a20  wn_blob_times(. 
+00008920: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00008930: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008940: 7269 6576 655f 7469 6d65 733a 2062 6f6f  rieve_times: boo
+00008950: 6c2c 0a20 2020 2020 2020 2020 2020 2062  l,.            b
+00008960: 6c6f 625f 7479 7065 3a20 4f70 7469 6f6e  lob_type: Option
+00008970: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00008980: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+00008990: 6563 746f 723a 204f 7074 696f 6e61 6c5b  ector: Optional[
+000089a0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000089b0: 2020 2020 2020 2020 2029 202d 3e20 5475           ) -> Tu
+000089c0: 706c 655b 666c 6f61 742c 204c 6973 745b  ple[float, List[
+000089d0: 5475 706c 655b 7374 722c 204f 7074 696f  Tuple[str, Optio
+000089e0: 6e61 6c5b 666c 6f61 745d 5d5d 5d3a 0a20  nal[float]]]]:. 
+000089f0: 2020 2020 2020 206f 626a 3a20 4469 6374         obj: Dict
+00008a00: 5b73 7472 2c20 556e 696f 6e5b 696e 742c  [str, Union[int,
+00008a10: 2073 7472 5d5d 203d 207b 0a20 2020 2020   str]] = {.     
+00008a20: 2020 2020 2020 2022 7265 7472 6965 7665         "retrieve
+00008a30: 5f74 696d 6573 223a 2069 6e74 2872 6574  _times": int(ret
+00008a40: 7269 6576 655f 7469 6d65 7329 2c0a 2020  rieve_times),.  
+00008a50: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00008a60: 6966 2062 6c6f 625f 7479 7065 2069 7320  if blob_type is 
+00008a70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00008a80: 2020 2020 2020 6f62 6a5b 2262 6c6f 625f        obj["blob_
+00008a90: 7479 7065 225d 203d 2062 6c6f 625f 7479  type"] = blob_ty
+00008aa0: 7065 0a20 2020 2020 2020 2069 6620 636f  pe.        if co
+00008ab0: 6e6e 6563 746f 7220 6973 206e 6f74 204e  nnector is not N
+00008ac0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00008ad0: 206f 626a 5b22 636f 6e6e 6563 746f 7222   obj["connector"
+00008ae0: 5d20 3d20 636f 6e6e 6563 746f 720a 2020  ] = connector.  
+00008af0: 2020 2020 2020 7265 7320 3d20 6361 7374        res = cast
+00008b00: 284b 6e6f 776e 426c 6f62 732c 2073 656c  (KnownBlobs, sel
+00008b10: 662e 7265 7175 6573 745f 6a73 6f6e 280a  f.request_json(.
+00008b20: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00008b30: 4f44 5f47 4554 2c20 222f 6b6e 6f77 6e5f  OD_GET, "/known_
+00008b40: 626c 6f62 7322 2c20 6f62 6a29 290a 2020  blobs", obj)).  
+00008b50: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00008b60: 5b22 6375 725f 7469 6d65 225d 2c20 7265  ["cur_time"], re
+00008b70: 735b 2262 6c6f 6273 225d 0a0a 2020 2020  s["blobs"]..    
+00008b80: 6465 6620 6765 745f 7472 6974 6f6e 5f6d  def get_triton_m
+00008b90: 6f64 656c 7328 7365 6c66 2920 2d3e 204c  odels(self) -> L
+00008ba0: 6973 745b 7374 725d 3a0a 2020 2020 2020  ist[str]:.      
+00008bb0: 2020 7265 7475 726e 2063 6173 7428 5472    return cast(Tr
+00008bc0: 6974 6f6e 4d6f 6465 6c73 5265 7370 6f6e  itonModelsRespon
+00008bd0: 7365 2c20 7365 6c66 2e72 6571 7565 7374  se, self.request
+00008be0: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
+00008bf0: 2020 204d 4554 484f 445f 4745 542c 2022     METHOD_GET, "
+00008c00: 2f69 6e66 6572 656e 6365 5f6d 6f64 656c  /inference_model
+00008c10: 7322 2c20 7b7d 2929 5b22 6d6f 6465 6c73  s", {}))["models
+00008c20: 225d 0a0a 2020 2020 4073 7461 7469 636d  "]..    @staticm
+00008c30: 6574 686f 640a 2020 2020 6465 6620 7265  ethod.    def re
+00008c40: 6164 5f64 7663 280a 2020 2020 2020 2020  ad_dvc(.        
+00008c50: 2020 2020 7061 7468 3a20 7374 722c 0a20      path: str,. 
+00008c60: 2020 2020 2020 2020 2020 2072 6570 6f3a             repo:
+00008c70: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+00008c80: 2020 7265 763a 204f 7074 696f 6e61 6c5b    rev: Optional[
+00008c90: 7374 725d 203d 2022 4845 4144 222c 0a20  str] = "HEAD",. 
+00008ca0: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00008cb0: 6e67 735f 696f 3a20 4f70 7469 6f6e 616c  ngs_io: Optional
+00008cc0: 5b49 4f5b 416e 795d 5d20 3d20 7379 732e  [IO[Any]] = sys.
+00008cd0: 7374 6465 7272 2920 2d3e 2041 6e79 3a0a  stderr) -> Any:.
+00008ce0: 2020 2020 2020 2020 2222 2252 6561 6469          """Readi
+00008cf0: 6e67 2064 7663 2066 696c 6520 636f 6e74  ng dvc file cont
+00008d00: 656e 7420 6672 6f6d 2067 6974 2074 7261  ent from git tra
+00008d10: 636b 6564 2044 5643 2070 726f 6a65 6374  cked DVC project
+00008d20: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00008d30: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00008d40: 6820 2873 7472 293a 0a20 2020 2020 2020  h (str):.       
+00008d50: 2020 2020 2020 2020 2046 696c 6520 7061           File pa
+00008d60: 7468 2074 6f20 7265 6164 2c20 7265 6c61  th to read, rela
+00008d70: 7469 7665 2074 6f20 7468 6520 726f 6f74  tive to the root
+00008d80: 206f 6620 7468 6520 7265 706f 2e0a 2020   of the repo..  
+00008d90: 2020 2020 2020 2020 2020 7265 706f 2028            repo (
+00008da0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00008db0: 2020 2020 2020 7370 6563 6966 6965 7320        specifies 
+00008dc0: 7468 6520 6c6f 6361 7469 6f6e 206f 6620  the location of 
+00008dd0: 7468 6520 4456 4320 7072 6f6a 6563 742e  the DVC project.
+00008de0: 2049 7420 6361 6e20 6265 2061 0a20 2020   It can be a.   
+00008df0: 2020 2020 2020 2020 2020 2020 2067 6974               git
+00008e00: 6875 6220 5552 4c20 6f72 2061 2066 696c  hub URL or a fil
+00008e10: 6520 7379 7374 656d 2070 6174 682e 0a20  e system path.. 
+00008e20: 2020 2020 2020 2020 2020 2072 6576 2028             rev (
+00008e30: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00008e40: 2020 2020 2020 4769 7420 636f 6d6d 6974        Git commit
+00008e50: 2028 616e 7920 7265 7669 7369 6f6e 2073   (any revision s
+00008e60: 7563 6820 6173 2061 2062 7261 6e63 6820  uch as a branch 
+00008e70: 6f72 2074 6167 206e 616d 652c 206f 7220  or tag name, or 
+00008e80: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00008e90: 2020 636f 6d6d 6974 2068 6173 6829 2e20    commit hash). 
+00008ea0: 4966 2072 6570 6f20 6973 206e 6f74 2061  If repo is not a
+00008eb0: 2047 6974 2072 6570 6f2c 2074 6869 7320   Git repo, this 
+00008ec0: 6f70 7469 6f6e 2069 730a 2020 2020 2020  option is.      
+00008ed0: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
+00008ee0: 642e 2044 6566 6175 6c74 3a20 4845 4144  d. Default: HEAD
+00008ef0: 2e0a 2020 2020 2020 2020 2020 2020 7761  ..            wa
+00008f00: 726e 696e 6773 5f69 6f20 286f 7074 696f  rnings_io (optio
+00008f10: 6e61 6c20 494f 293a 0a20 2020 2020 2020  nal IO):.       
+00008f20: 2020 2020 2020 2020 2049 4f20 7374 7265           IO stre
+00008f30: 616d 2077 6865 7265 2074 6865 2077 6172  am where the war
+00008f40: 6e69 6e67 2077 696c 6c20 6265 2070 7269  ning will be pri
+00008f50: 6e74 6564 2074 6f0a 0a20 2020 2020 2020  nted to..       
+00008f60: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00008f70: 2020 2020 2020 7468 6520 636f 6e74 656e        the conten
+00008f80: 7420 6f66 2074 6865 2066 696c 652e 0a20  t of the file.. 
+00008f90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008fa0: 2020 2066 726f 6d20 2e75 7469 6c20 696d     from .util im
+00008fb0: 706f 7274 2068 6173 5f64 7663 0a0a 2020  port has_dvc..  
+00008fc0: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
+00008fd0: 5f64 7663 2829 3a0a 2020 2020 2020 2020  _dvc():.        
+00008fe0: 2020 2020 6966 2077 6172 6e69 6e67 735f      if warnings_
+00008ff0: 696f 2069 7320 6e6f 7420 4e6f 6e65 3a0a  io is not None:.
+00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009010: 7761 726e 696e 6773 5f69 6f2e 7772 6974  warnings_io.writ
+00009020: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00009030: 2020 2020 2020 2022 506c 6561 7365 2069         "Please i
+00009040: 6e73 7461 6c6c 2064 7663 2068 7474 7073  nstall dvc https
+00009050: 3a2f 2f64 7663 2e6f 7267 2f64 6f63 2f69  ://dvc.org/doc/i
+00009060: 6e73 7461 6c6c 2229 0a20 2020 2020 2020  nstall").       
+00009070: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00009080: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+00009090: 2064 7663 2e61 7069 0a0a 2020 2020 2020   dvc.api..      
+000090a0: 2020 7265 7320 3d20 6476 632e 6170 692e    res = dvc.api.
+000090b0: 7265 6164 2870 6174 682c 2072 6570 6f3d  read(path, repo=
+000090c0: 7265 706f 2c20 7265 763d 7265 762c 206d  repo, rev=rev, m
+000090d0: 6f64 653d 2272 2229 0a20 2020 2020 2020  ode="r").       
+000090e0: 206d 6179 6265 5f70 6172 7365 203d 206d   maybe_parse = m
+000090f0: 6179 6265 5f6a 736f 6e5f 6c6f 6164 7328  aybe_json_loads(
+00009100: 7265 7329 0a20 2020 2020 2020 2069 6620  res).        if 
+00009110: 6d61 7962 655f 7061 7273 6520 6973 206e  maybe_parse is n
+00009120: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00009130: 2020 2020 2072 6574 7572 6e20 6d61 7962       return mayb
+00009140: 655f 7061 7273 650a 2020 2020 2020 2020  e_parse.        
+00009150: 7265 7475 726e 2072 6573 0a0a 2020 2020  return res..    
+00009160: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00009170: 2020 6465 6620 6765 745f 656e 765f 7374    def get_env_st
+00009180: 7228 6b65 793a 2073 7472 2c20 6465 6661  r(key: str, defa
+00009190: 756c 743a 204f 7074 696f 6e61 6c5b 7374  ult: Optional[st
+000091a0: 725d 203d 204e 6f6e 6529 202d 3e20 7374  r] = None) -> st
+000091b0: 723a 0a20 2020 2020 2020 2072 6573 203d  r:.        res =
+000091c0: 206f 732e 6765 7465 6e76 286b 6579 2c20   os.getenv(key, 
+000091d0: 6465 6661 756c 743d 6465 6661 756c 7429  default=default)
+000091e0: 0a20 2020 2020 2020 2069 6620 7265 7320  .        if res 
+000091f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00009200: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00009210: 4572 726f 7228 6622 656e 7669 726f 6e6d  Error(f"environm
+00009220: 656e 7420 7661 7269 6162 6c65 207b 6b65  ent variable {ke
+00009230: 797d 2069 7320 6e6f 7420 7365 7422 290a  y} is not set").
+00009240: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00009250: 227b 7265 737d 220a 0a20 2020 2040 7374  "{res}"..    @st
+00009260: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00009270: 6566 2067 6574 5f65 6e76 5f69 6e74 286b  ef get_env_int(k
+00009280: 6579 3a20 7374 722c 2064 6566 6175 6c74  ey: str, default
+00009290: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+000092a0: 3d20 4e6f 6e65 2920 2d3e 2069 6e74 3a0a  = None) -> int:.
+000092b0: 2020 2020 2020 2020 7265 7320 3d20 6f73          res = os
+000092c0: 2e67 6574 656e 7628 6b65 792c 2064 6566  .getenv(key, def
+000092d0: 6175 6c74 3d64 6566 6175 6c74 290a 2020  ault=default).  
+000092e0: 2020 2020 2020 6966 2072 6573 2069 7320        if res is 
+000092f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009300: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00009310: 6f72 2866 2265 6e76 6972 6f6e 6d65 6e74  or(f"environment
+00009320: 2076 6172 6961 626c 6520 7b6b 6579 7d20   variable {key} 
+00009330: 6973 206e 6f74 2073 6574 2229 0a20 2020  is not set").   
+00009340: 2020 2020 2072 6574 7572 6e20 696e 7428       return int(
+00009350: 7265 7329 0a0a 2020 2020 4073 7461 7469  res)..    @stati
+00009360: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00009370: 6765 745f 656e 765f 626f 6f6c 286b 6579  get_env_bool(key
+00009380: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
+00009390: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+000093a0: 204e 6f6e 6529 202d 3e20 626f 6f6c 3a0a   None) -> bool:.
+000093b0: 2020 2020 2020 2020 7265 7320 3d20 6f73          res = os
+000093c0: 2e67 6574 656e 7628 6b65 792c 2064 6566  .getenv(key, def
+000093d0: 6175 6c74 3d64 6566 6175 6c74 290a 2020  ault=default).  
+000093e0: 2020 2020 2020 6966 2072 6573 2069 7320        if res is 
+000093f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009400: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00009410: 6f72 2866 2265 6e76 6972 6f6e 6d65 6e74  or(f"environment
+00009420: 2076 6172 6961 626c 6520 7b6b 6579 7d20   variable {key} 
+00009430: 6973 206e 6f74 2073 6574 2229 0a20 2020  is not set").   
+00009440: 2020 2020 2072 6574 7572 6e20 746f 5f62       return to_b
+00009450: 6f6f 6c28 7265 7329 0a0a 2020 2020 4073  ool(res)..    @s
+00009460: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00009470: 6465 6620 6c6f 6164 5f6a 736f 6e28 6a73  def load_json(js
+00009480: 6f6e 5f70 6174 683a 2073 7472 2920 2d3e  on_path: str) ->
+00009490: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
+000094a0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+000094b0: 656e 286a 736f 6e5f 7061 7468 2c20 2272  en(json_path, "r
+000094c0: 2229 2061 7320 6669 6e3a 0a20 2020 2020  ") as fin:.     
+000094d0: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
+000094e0: 6f6e 2e6c 6f61 6428 6669 6e29 0a0a 2020  on.load(fin)..  
+000094f0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00009500: 2020 2064 6566 206c 6f61 645f 7333 5f63     def load_s3_c
+00009510: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
+00009520: 675f 7061 7468 3a20 7374 7229 202d 3e20  g_path: str) -> 
+00009530: 5333 436f 6e66 6967 3a0a 2020 2020 2020  S3Config:.      
+00009540: 2020 7265 7475 726e 2063 6173 7428 5333    return cast(S3
+00009550: 436f 6e66 6967 2c20 636c 732e 6c6f 6164  Config, cls.load
+00009560: 5f6a 736f 6e28 636f 6e66 6967 5f70 6174  _json(config_pat
+00009570: 6829 290a 0a20 2020 2040 636c 6173 736d  h))..    @classm
+00009580: 6574 686f 640a 2020 2020 6465 6620 646f  ethod.    def do
+00009590: 776e 6c6f 6164 5f73 335f 6672 6f6d 5f66  wnload_s3_from_f
+000095a0: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+000095b0: 2063 6c73 2c20 6465 7374 5f70 6174 683a   cls, dest_path:
+000095c0: 204c 6973 745b 7374 725d 2c20 636f 6e66   List[str], conf
+000095d0: 6967 5f70 6174 683a 2073 7472 2920 2d3e  ig_path: str) ->
+000095e0: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
+000095f0: 6c73 2e64 6f77 6e6c 6f61 645f 7333 2864  ls.download_s3(d
+00009600: 6573 745f 7061 7468 2c20 636c 732e 6c6f  est_path, cls.lo
+00009610: 6164 5f73 335f 636f 6e66 6967 2863 6f6e  ad_s3_config(con
+00009620: 6669 675f 7061 7468 2929 0a0a 2020 2020  fig_path))..    
+00009630: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00009640: 2020 6465 6620 646f 776e 6c6f 6164 5f73    def download_s
+00009650: 3328 6465 7374 5f70 6174 683a 204c 6973  3(dest_path: Lis
+00009660: 745b 7374 725d 2c20 636f 6e66 6967 3a20  t[str], config: 
+00009670: 5333 436f 6e66 6967 2920 2d3e 204e 6f6e  S3Config) -> Non
+00009680: 653a 0a20 2020 2020 2020 2069 6d70 6f72  e:.        impor
+00009690: 7420 626f 746f 330a 0a20 2020 2020 2020  t boto3..       
+000096a0: 2073 3320 3d20 626f 746f 332e 636c 6965   s3 = boto3.clie
+000096b0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+000096c0: 2273 3322 2c0a 2020 2020 2020 2020 2020  "s3",.          
+000096d0: 2020 6177 735f 6163 6365 7373 5f6b 6579    aws_access_key
+000096e0: 5f69 643d 636f 6e66 6967 5b22 6163 6365  _id=config["acce
+000096f0: 726e 5f61 7773 5f6b 6579 225d 2c0a 2020  rn_aws_key"],.  
+00009700: 2020 2020 2020 2020 2020 6177 735f 7365            aws_se
+00009710: 6372 6574 5f61 6363 6573 735f 6b65 793d  cret_access_key=
+00009720: 636f 6e66 6967 5b22 6163 6365 726e 5f61  config["accern_a
+00009730: 7773 5f61 6363 6573 735f 6b65 7922 5d29  ws_access_key"])
+00009740: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00009750: 6c65 6e28 6465 7374 5f70 6174 6829 203d  len(dest_path) =
+00009760: 3d20 6c65 6e28 636f 6e66 6967 5b22 6d6f  = len(config["mo
+00009770: 6465 6c5f 646f 776e 6c6f 6164 5f70 6174  del_download_pat
+00009780: 6822 5d29 0a20 2020 2020 2020 2066 6f72  h"]).        for
+00009790: 2028 6465 7374 2c20 7061 7468 2920 696e   (dest, path) in
+000097a0: 207a 6970 2864 6573 745f 7061 7468 2c20   zip(dest_path, 
+000097b0: 636f 6e66 6967 5b22 6d6f 6465 6c5f 646f  config["model_do
+000097c0: 776e 6c6f 6164 5f70 6174 6822 5d29 3a0a  wnload_path"]):.
+000097d0: 2020 2020 2020 2020 2020 2020 7333 2e64              s3.d
+000097e0: 6f77 6e6c 6f61 645f 6669 6c65 2863 6f6e  ownload_file(con
+000097f0: 6669 675b 226d 6f64 656c 5f64 6f77 6e6c  fig["model_downl
+00009800: 6f61 645f 6275 636b 6574 225d 2c20 7061  oad_bucket"], pa
+00009810: 7468 2c20 6465 7374 290a 0a20 2020 2040  th, dest)..    @
+00009820: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00009830: 6465 6620 7570 6c6f 6164 5f73 335f 6672  def upload_s3_fr
+00009840: 6f6d 5f66 696c 6528 0a20 2020 2020 2020  om_file(.       
+00009850: 2020 2020 2063 6c73 2c20 736f 7572 6365       cls, source
+00009860: 5f70 6174 683a 204c 6973 745b 7374 725d  _path: List[str]
+00009870: 2c20 636f 6e66 6967 5f70 6174 683a 2073  , config_path: s
+00009880: 7472 2920 2d3e 204e 6f6e 653a 0a20 2020  tr) -> None:.   
+00009890: 2020 2020 2063 6c73 2e75 706c 6f61 645f       cls.upload_
+000098a0: 7333 2873 6f75 7263 655f 7061 7468 2c20  s3(source_path, 
+000098b0: 636c 732e 6c6f 6164 5f73 335f 636f 6e66  cls.load_s3_conf
+000098c0: 6967 2863 6f6e 6669 675f 7061 7468 2929  ig(config_path))
+000098d0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+000098e0: 686f 640a 2020 2020 6465 6620 7570 6c6f  hod.    def uplo
+000098f0: 6164 5f73 3328 736f 7572 6365 5f70 6174  ad_s3(source_pat
+00009900: 683a 204c 6973 745b 7374 725d 2c20 636f  h: List[str], co
+00009910: 6e66 6967 3a20 5333 436f 6e66 6967 2920  nfig: S3Config) 
+00009920: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00009930: 2069 6d70 6f72 7420 626f 746f 330a 0a20   import boto3.. 
+00009940: 2020 2020 2020 2073 3320 3d20 626f 746f         s3 = boto
+00009950: 332e 636c 6965 6e74 280a 2020 2020 2020  3.client(.      
+00009960: 2020 2020 2020 2273 3322 2c0a 2020 2020        "s3",.    
+00009970: 2020 2020 2020 2020 6177 735f 6163 6365          aws_acce
+00009980: 7373 5f6b 6579 5f69 643d 636f 6e66 6967  ss_key_id=config
+00009990: 5b22 6163 6365 726e 5f61 7773 5f6b 6579  ["accern_aws_key
+000099a0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+000099b0: 6177 735f 7365 6372 6574 5f61 6363 6573  aws_secret_acces
+000099c0: 735f 6b65 793d 636f 6e66 6967 5b22 6163  s_key=config["ac
+000099d0: 6365 726e 5f61 7773 5f61 6363 6573 735f  cern_aws_access_
+000099e0: 6b65 7922 5d29 0a20 2020 2020 2020 2061  key"]).        a
+000099f0: 7373 6572 7420 6c65 6e28 736f 7572 6365  ssert len(source
+00009a00: 5f70 6174 6829 203d 3d20 6c65 6e28 636f  _path) == len(co
+00009a10: 6e66 6967 5b22 6d6f 6465 6c5f 646f 776e  nfig["model_down
+00009a20: 6c6f 6164 5f70 6174 6822 5d29 0a20 2020  load_path"]).   
+00009a30: 2020 2020 2066 6f72 2028 736f 7572 6365       for (source
+00009a40: 2c20 7061 7468 2920 696e 207a 6970 2873  , path) in zip(s
+00009a50: 6f75 7263 655f 7061 7468 2c20 636f 6e66  ource_path, conf
+00009a60: 6967 5b22 6d6f 6465 6c5f 646f 776e 6c6f  ig["model_downlo
+00009a70: 6164 5f70 6174 6822 5d29 3a0a 2020 2020  ad_path"]):.    
+00009a80: 2020 2020 2020 2020 7333 2e75 706c 6f61          s3.uploa
+00009a90: 645f 6669 6c65 2873 6f75 7263 652c 2063  d_file(source, c
+00009aa0: 6f6e 6669 675b 226d 6f64 656c 5f64 6f77  onfig["model_dow
+00009ab0: 6e6c 6f61 645f 6275 636b 6574 225d 2c20  nload_bucket"], 
+00009ac0: 7061 7468 290a 0a20 2020 2064 6566 2067  path)..    def g
+00009ad0: 6574 5f75 7569 6428 7365 6c66 2920 2d3e  et_uuid(self) ->
+00009ae0: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+00009af0: 7475 726e 2063 6173 7428 5555 4944 5265  turn cast(UUIDRe
+00009b00: 7370 6f6e 7365 2c20 7365 6c66 2e72 6571  sponse, self.req
+00009b10: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00009b20: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
+00009b30: 542c 2022 2f75 7569 6422 2c20 7b7d 2929  T, "/uuid", {}))
+00009b40: 5b22 7575 6964 225d 0a0a 2020 2020 6465  ["uuid"]..    de
+00009b50: 6620 6465 6c65 7465 5f62 6c6f 6273 2873  f delete_blobs(s
+00009b60: 656c 662c 2062 6c6f 625f 7572 6973 3a20  elf, blob_uris: 
+00009b70: 4c69 7374 5b73 7472 5d29 202d 3e20 4465  List[str]) -> De
+00009b80: 6c65 7465 426c 6f62 5265 7370 6f6e 7365  leteBlobResponse
+00009b90: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00009ba0: 2063 6173 7428 4465 6c65 7465 426c 6f62   cast(DeleteBlob
+00009bb0: 5265 7370 6f6e 7365 2c20 7365 6c66 2e72  Response, self.r
+00009bc0: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
+00009bd0: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+00009be0: 4445 4c45 5445 2c20 222f 626c 6f62 222c  DELETE, "/blob",
+00009bf0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00009c00: 2020 2022 626c 6f62 5f75 7269 7322 3a20     "blob_uris": 
+00009c10: 626c 6f62 5f75 7269 732c 0a20 2020 2020  blob_uris,.     
+00009c20: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00009c30: 2020 2929 0a0a 2320 2a2a 2a20 5859 4d45    ))..# *** XYME
+00009c40: 436c 6965 6e74 202a 2a2a 0a0a 0a63 6c61  Client ***...cla
+00009c50: 7373 2044 6167 4861 6e64 6c65 3a0a 2020  ss DagHandle:.  
+00009c60: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00009c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009c80: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+00009c90: 6965 6e74 3a20 5859 4d45 436c 6965 6e74  ient: XYMEClient
+00009ca0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00009cb0: 675f 7572 693a 2073 7472 2920 2d3e 204e  g_uri: str) -> N
+00009cc0: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
+00009cd0: 662e 5f63 6c69 656e 7420 3d20 636c 6965  f._client = clie
+00009ce0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+00009cf0: 5f64 6167 5f75 7269 203d 2064 6167 5f75  _dag_uri = dag_u
+00009d00: 7269 0a20 2020 2020 2020 2073 656c 662e  ri.        self.
+00009d10: 5f6e 616d 653a 204f 7074 696f 6e61 6c5b  _name: Optional[
+00009d20: 7374 725d 203d 204e 6f6e 650a 2020 2020  str] = None.    
+00009d30: 2020 2020 7365 6c66 2e5f 636f 6d70 616e      self._compan
+00009d40: 793a 204f 7074 696f 6e61 6c5b 7374 725d  y: Optional[str]
+00009d50: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00009d60: 7365 6c66 2e5f 7374 6174 655f 7572 693a  self._state_uri:
+00009d70: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00009d80: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00009d90: 6c66 2e5f 7572 695f 7072 6566 6978 3a20  lf._uri_prefix: 
+00009da0: 4f70 7469 6f6e 616c 5b55 5249 5072 6566  Optional[URIPref
+00009db0: 6978 5d20 3d20 4e6f 6e65 0a20 2020 2020  ix] = None.     
+00009dc0: 2020 2073 656c 662e 5f69 735f 6869 6768     self._is_high
+00009dd0: 5f70 7269 6f72 6974 793a 204f 7074 696f  _priority: Optio
+00009de0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00009df0: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
+00009e00: 7565 7565 5f6d 6e67 3a20 4f70 7469 6f6e  ueue_mng: Option
+00009e10: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
+00009e20: 2020 2020 2020 2073 656c 662e 5f76 6572         self._ver
+00009e30: 7369 6f6e 5f6f 7665 7272 6964 653a 204f  sion_override: O
+00009e40: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00009e50: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00009e60: 2e5f 6e6f 6465 733a 2044 6963 745b 7374  ._nodes: Dict[st
+00009e70: 722c 204e 6f64 6548 616e 646c 655d 203d  r, NodeHandle] =
+00009e80: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
+00009e90: 2e5f 6e6f 6465 5f6c 6f6f 6b75 703a 2044  ._node_lookup: D
+00009ea0: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+00009eb0: 7b7d 0a20 2020 2020 2020 2073 656c 662e  {}.        self.
+00009ec0: 5f64 796e 616d 6963 5f65 7272 6f72 3a20  _dynamic_error: 
+00009ed0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00009ee0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00009ef0: 662e 5f69 6e73 3a20 4f70 7469 6f6e 616c  f._ins: Optional
+00009f00: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
+00009f10: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00009f20: 5f6f 7574 733a 204f 7074 696f 6e61 6c5b  _outs: Optional[
+00009f30: 4c69 7374 5b54 7570 6c65 5b73 7472 2c20  List[Tuple[str, 
+00009f40: 7374 725d 5d5d 203d 204e 6f6e 650a 2020  str]]] = None.  
+00009f50: 2020 2020 2020 7365 6c66 2e5f 6b61 666b        self._kafk
+00009f60: 615f 696e 7075 745f 746f 7069 633a 204f  a_input_topic: O
+00009f70: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00009f80: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00009f90: 2e5f 6b61 666b 615f 6f75 7470 7574 5f74  ._kafka_output_t
+00009fa0: 6f70 6963 3a20 4f70 7469 6f6e 616c 5b73  opic: Optional[s
+00009fb0: 7472 5d20 3d20 4e6f 6e65 0a0a 2020 2020  tr] = None..    
+00009fc0: 6465 6620 7265 6672 6573 6828 7365 6c66  def refresh(self
+00009fd0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00009fe0: 2020 2073 656c 662e 5f6e 616d 6520 3d20     self._name = 
+00009ff0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000a000: 662e 5f63 6f6d 7061 6e79 203d 204e 6f6e  f._company = Non
+0000a010: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000a020: 7374 6174 655f 7572 6920 3d20 4e6f 6e65  state_uri = None
+0000a030: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
+0000a040: 7269 5f70 7265 6669 7820 3d20 4e6f 6e65  ri_prefix = None
+0000a050: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+0000a060: 735f 6869 6768 5f70 7269 6f72 6974 7920  s_high_priority 
+0000a070: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000a080: 656c 662e 5f71 7565 7565 5f6d 6e67 203d  elf._queue_mng =
+0000a090: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0000a0a0: 6c66 2e5f 7665 7273 696f 6e5f 6f76 6572  lf._version_over
+0000a0b0: 7269 6465 203d 204e 6f6e 650a 2020 2020  ride = None.    
+0000a0c0: 2020 2020 7365 6c66 2e5f 696e 7320 3d20      self._ins = 
+0000a0d0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000a0e0: 662e 5f6f 7574 7320 3d20 4e6f 6e65 0a20  f._outs = None. 
+0000a0f0: 2020 2020 2020 2073 656c 662e 5f6b 6166         self._kaf
+0000a100: 6b61 5f69 6e70 7574 5f74 6f70 6963 203d  ka_input_topic =
+0000a110: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0000a120: 6c66 2e5f 6b61 666b 615f 6f75 7470 7574  lf._kafka_output
+0000a130: 5f74 6f70 6963 203d 204e 6f6e 650a 2020  _topic = None.  
+0000a140: 2020 2020 2020 2320 4e4f 5445 3a20 7765        # NOTE: we
+0000a150: 2064 6f6e 2774 2072 6573 6574 206e 6f64   don't reset nod
+0000a160: 6573 0a0a 2020 2020 6465 6620 5f6d 6179  es..    def _may
+0000a170: 6265 5f72 6566 7265 7368 2873 656c 6629  be_refresh(self)
+0000a180: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000a190: 2020 6966 2073 656c 662e 5f63 6c69 656e    if self._clien
+0000a1a0: 742e 6973 5f61 7574 6f5f 7265 6672 6573  t.is_auto_refres
+0000a1b0: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
+0000a1c0: 2073 656c 662e 7265 6672 6573 6828 290a   self.refresh().
+0000a1d0: 0a20 2020 2064 6566 205f 6d61 7962 655f  .    def _maybe_
+0000a1e0: 6665 7463 6828 7365 6c66 2920 2d3e 204e  fetch(self) -> N
+0000a1f0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+0000a200: 7365 6c66 2e5f 6e61 6d65 2069 7320 4e6f  self._name is No
+0000a210: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a220: 7365 6c66 2e5f 6665 7463 685f 696e 666f  self._fetch_info
+0000a230: 2829 0a0a 2020 2020 6465 6620 6765 745f  ()..    def get_
+0000a240: 696e 666f 2873 656c 6629 202d 3e20 4461  info(self) -> Da
+0000a250: 6749 6e66 6f3a 0a20 2020 2020 2020 2072  gInfo:.        r
+0000a260: 6574 7572 6e20 6361 7374 2844 6167 496e  eturn cast(DagIn
+0000a270: 666f 2c20 7365 6c66 2e5f 636c 6965 6e74  fo, self._client
+0000a280: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+0000a290: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+0000a2a0: 445f 4745 542c 2022 2f64 6167 5f69 6e66  D_GET, "/dag_inf
+0000a2b0: 6f22 2c20 7b0a 2020 2020 2020 2020 2020  o", {.          
+0000a2c0: 2020 2020 2020 2264 6167 223a 2073 656c        "dag": sel
+0000a2d0: 662e 6765 745f 7572 6928 292c 0a20 2020  f.get_uri(),.   
+0000a2e0: 2020 2020 2020 2020 207d 2929 0a0a 2020           }))..  
+0000a2f0: 2020 6465 6620 5f66 6574 6368 5f69 6e66    def _fetch_inf
+0000a300: 6f28 7365 6c66 2920 2d3e 204e 6f6e 653a  o(self) -> None:
+0000a310: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
+0000a320: 7365 6c66 2e67 6574 5f69 6e66 6f28 290a  self.get_info().
+0000a330: 2020 2020 2020 2020 7365 6c66 2e5f 6e61          self._na
+0000a340: 6d65 203d 2069 6e66 6f5b 226e 616d 6522  me = info["name"
+0000a350: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
+0000a360: 636f 6d70 616e 7920 3d20 696e 666f 5b22  company = info["
+0000a370: 636f 6d70 616e 7922 5d0a 2020 2020 2020  company"].      
+0000a380: 2020 7365 6c66 2e5f 7374 6174 655f 7572    self._state_ur
+0000a390: 6920 3d20 696e 666f 5b22 7374 6174 655f  i = info["state_
+0000a3a0: 7572 6922 5d0a 2020 2020 2020 2020 7365  uri"].        se
+0000a3b0: 6c66 2e5f 7572 695f 7072 6566 6978 203d  lf._uri_prefix =
+0000a3c0: 2069 6e66 6f5b 2275 7269 5f70 7265 6669   info["uri_prefi
+0000a3d0: 7822 5d0a 2020 2020 2020 2020 7365 6c66  x"].        self
+0000a3e0: 2e5f 6973 5f68 6967 685f 7072 696f 7269  ._is_high_priori
+0000a3f0: 7479 203d 2069 6e66 6f5b 2268 6967 685f  ty = info["high_
+0000a400: 7072 696f 7269 7479 225d 0a20 2020 2020  priority"].     
+0000a410: 2020 2073 656c 662e 5f71 7565 7565 5f6d     self._queue_m
+0000a420: 6e67 203d 2069 6e66 6f5b 2271 7565 7565  ng = info["queue
+0000a430: 5f6d 6e67 225d 0a20 2020 2020 2020 2073  _mng"].        s
+0000a440: 656c 662e 5f76 6572 7369 6f6e 5f6f 7665  elf._version_ove
+0000a450: 7272 6964 6520 3d20 696e 666f 5b22 7665  rride = info["ve
+0000a460: 7273 696f 6e5f 6f76 6572 7269 6465 225d  rsion_override"]
+0000a470: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+0000a480: 6e73 203d 2069 6e66 6f5b 2269 6e73 225d  ns = info["ins"]
+0000a490: 0a20 2020 2020 2020 2073 656c 662e 5f6f  .        self._o
+0000a4a0: 7574 7320 3d20 5b28 656c 5b30 5d2c 2065  uts = [(el[0], e
+0000a4b0: 6c5b 315d 2920 666f 7220 656c 2069 6e20  l[1]) for el in 
+0000a4c0: 696e 666f 5b22 6f75 7473 225d 5d0a 2020  info["outs"]].  
+0000a4d0: 2020 2020 2020 7365 6c66 2e5f 6b61 666b        self._kafk
+0000a4e0: 615f 696e 7075 745f 746f 7069 6320 3d20  a_input_topic = 
+0000a4f0: 696e 666f 5b22 6b61 666b 615f 696e 7075  info["kafka_inpu
+0000a500: 745f 746f 7069 6322 5d0a 2020 2020 2020  t_topic"].      
+0000a510: 2020 7365 6c66 2e5f 6b61 666b 615f 6f75    self._kafka_ou
+0000a520: 7470 7574 5f74 6f70 6963 203d 2069 6e66  tput_topic = inf
+0000a530: 6f5b 226b 6166 6b61 5f6f 7574 7075 745f  o["kafka_output_
+0000a540: 746f 7069 6322 5d0a 2020 2020 2020 2020  topic"].        
+0000a550: 6f6c 645f 6e6f 6465 7320 3d20 7b7d 2069  old_nodes = {} i
+0000a560: 6620 7365 6c66 2e5f 6e6f 6465 7320 6973  f self._nodes is
+0000a570: 204e 6f6e 6520 656c 7365 2073 656c 662e   None else self.
+0000a580: 5f6e 6f64 6573 0a20 2020 2020 2020 2073  _nodes.        s
+0000a590: 656c 662e 5f6e 6f64 6573 203d 207b 0a20  elf._nodes = {. 
+0000a5a0: 2020 2020 2020 2020 2020 206e 6f64 655b             node[
+0000a5b0: 2269 6422 5d3a 204e 6f64 6548 616e 646c  "id"]: NodeHandl
+0000a5c0: 652e 6672 6f6d 5f6e 6f64 655f 696e 666f  e.from_node_info
+0000a5d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a5e0: 2020 7365 6c66 2e5f 636c 6965 6e74 2c20    self._client, 
+0000a5f0: 7365 6c66 2c20 6e6f 6465 2c20 6f6c 645f  self, node, old_
+0000a600: 6e6f 6465 732e 6765 7428 6e6f 6465 5b22  nodes.get(node["
+0000a610: 6964 225d 2929 0a20 2020 2020 2020 2020  id"])).         
+0000a620: 2020 2066 6f72 206e 6f64 6520 696e 2069     for node in i
+0000a630: 6e66 6f5b 226e 6f64 6573 225d 0a20 2020  nfo["nodes"].   
+0000a640: 2020 2020 207d 0a20 2020 2020 2020 2073       }.        s
+0000a650: 656c 662e 5f6e 6f64 655f 6c6f 6f6b 7570  elf._node_lookup
+0000a660: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0000a670: 206e 6f64 655b 226e 616d 6522 5d3a 206e   node["name"]: n
+0000a680: 6f64 655b 2269 6422 5d0a 2020 2020 2020  ode["id"].      
+0000a690: 2020 2020 2020 666f 7220 6e6f 6465 2069        for node i
+0000a6a0: 6e20 696e 666f 5b22 6e6f 6465 7322 5d0a  n info["nodes"].
+0000a6b0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000a6c0: 6f64 655b 226e 616d 6522 5d20 6973 206e  ode["name"] is n
+0000a6d0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0000a6e0: 7d0a 0a20 2020 2064 6566 2067 6574 5f6e  }..    def get_n
+0000a6f0: 6f64 6573 2873 656c 6629 202d 3e20 4c69  odes(self) -> Li
+0000a700: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
+0000a710: 2073 656c 662e 5f6d 6179 6265 5f72 6566   self._maybe_ref
+0000a720: 7265 7368 2829 0a20 2020 2020 2020 2073  resh().        s
+0000a730: 656c 662e 5f6d 6179 6265 5f66 6574 6368  elf._maybe_fetch
+0000a740: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+0000a750: 6e20 6c69 7374 2873 656c 662e 5f6e 6f64  n list(self._nod
+0000a760: 6573 2e6b 6579 7328 2929 0a0a 2020 2020  es.keys())..    
+0000a770: 6465 6620 6765 745f 6e6f 6465 2873 656c  def get_node(sel
+0000a780: 662c 206e 6f64 655f 6e61 6d65 3a20 7374  f, node_name: st
+0000a790: 7229 202d 3e20 274e 6f64 6548 616e 646c  r) -> 'NodeHandl
+0000a7a0: 6527 3a0a 2020 2020 2020 2020 7365 6c66  e':.        self
+0000a7b0: 2e5f 6d61 7962 655f 7265 6672 6573 6828  ._maybe_refresh(
+0000a7c0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+0000a7d0: 6d61 7962 655f 6665 7463 6828 290a 2020  maybe_fetch().  
+0000a7e0: 2020 2020 2020 6e6f 6465 5f69 6420 3d20        node_id = 
+0000a7f0: 7365 6c66 2e5f 6e6f 6465 5f6c 6f6f 6b75  self._node_looku
+0000a800: 702e 6765 7428 6e6f 6465 5f6e 616d 652c  p.get(node_name,
+0000a810: 206e 6f64 655f 6e61 6d65 290a 2020 2020   node_name).    
+0000a820: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000a830: 5f6e 6f64 6573 5b6e 6f64 655f 6964 5d0a  _nodes[node_id].
+0000a840: 0a20 2020 2064 6566 2067 6574 5f75 7269  .    def get_uri
+0000a850: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+0000a860: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000a870: 6c66 2e5f 6461 675f 7572 690a 0a20 2020  lf._dag_uri..   
+0000a880: 2064 6566 2067 6574 5f6e 616d 6528 7365   def get_name(se
+0000a890: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+0000a8a0: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
+0000a8b0: 7265 6672 6573 6828 290a 2020 2020 2020  refresh().      
+0000a8c0: 2020 7365 6c66 2e5f 6d61 7962 655f 6665    self._maybe_fe
+0000a8d0: 7463 6828 290a 2020 2020 2020 2020 6173  tch().        as
+0000a8e0: 7365 7274 2073 656c 662e 5f6e 616d 6520  sert self._name 
+0000a8f0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+0000a900: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000a910: 5f6e 616d 650a 0a20 2020 2064 6566 2067  _name..    def g
+0000a920: 6574 5f63 6f6d 7061 6e79 2873 656c 6629  et_company(self)
+0000a930: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000a940: 2073 656c 662e 5f6d 6179 6265 5f72 6566   self._maybe_ref
+0000a950: 7265 7368 2829 0a20 2020 2020 2020 2073  resh().        s
+0000a960: 656c 662e 5f6d 6179 6265 5f66 6574 6368  elf._maybe_fetch
+0000a970: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
+0000a980: 7420 7365 6c66 2e5f 636f 6d70 616e 7920  t self._company 
+0000a990: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+0000a9a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000a9b0: 5f63 6f6d 7061 6e79 0a0a 2020 2020 6465  _company..    de
+0000a9c0: 6620 6765 745f 7374 6174 655f 7572 6928  f get_state_uri(
+0000a9d0: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0000a9e0: 2020 2020 2020 7365 6c66 2e5f 6d61 7962        self._mayb
+0000a9f0: 655f 7265 6672 6573 6828 290a 2020 2020  e_refresh().    
+0000aa00: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
+0000aa10: 6665 7463 6828 290a 2020 2020 2020 2020  fetch().        
+0000aa20: 6173 7365 7274 2073 656c 662e 5f73 7461  assert self._sta
+0000aa30: 7465 5f75 7269 2069 7320 6e6f 7420 4e6f  te_uri is not No
+0000aa40: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+0000aa50: 6e20 7365 6c66 2e5f 7374 6174 655f 7572  n self._state_ur
+0000aa60: 690a 0a20 2020 2064 6566 2067 6574 5f76  i..    def get_v
+0000aa70: 6572 7369 6f6e 5f6f 7665 7272 6964 6528  ersion_override(
+0000aa80: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0000aa90: 2020 2020 2020 7365 6c66 2e5f 6d61 7962        self._mayb
+0000aaa0: 655f 7265 6672 6573 6828 290a 2020 2020  e_refresh().    
+0000aab0: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
+0000aac0: 6665 7463 6828 290a 2020 2020 2020 2020  fetch().        
+0000aad0: 6173 7365 7274 2073 656c 662e 5f76 6572  assert self._ver
+0000aae0: 7369 6f6e 5f6f 7665 7272 6964 6520 6973  sion_override is
+0000aaf0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+0000ab00: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
+0000ab10: 6572 7369 6f6e 5f6f 7665 7272 6964 650a  ersion_override.
+0000ab20: 0a20 2020 2064 6566 2067 6574 5f6b 6166  .    def get_kaf
+0000ab30: 6b61 5f74 6f70 6963 7328 7365 6c66 2920  ka_topics(self) 
+0000ab40: 2d3e 2054 7570 6c65 5b4f 7074 696f 6e61  -> Tuple[Optiona
+0000ab50: 6c5b 7374 725d 2c20 4f70 7469 6f6e 616c  l[str], Optional
+0000ab60: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+0000ab70: 7365 6c66 2e5f 6d61 7962 655f 7265 6672  self._maybe_refr
+0000ab80: 6573 6828 290a 2020 2020 2020 2020 7365  esh().        se
+0000ab90: 6c66 2e5f 6d61 7962 655f 6665 7463 6828  lf._maybe_fetch(
+0000aba0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000abb0: 2073 656c 662e 5f6b 6166 6b61 5f69 6e70   self._kafka_inp
+0000abc0: 7574 5f74 6f70 6963 2c20 7365 6c66 2e5f  ut_topic, self._
+0000abd0: 6b61 666b 615f 6f75 7470 7574 5f74 6f70  kafka_output_top
+0000abe0: 6963 0a0a 2020 2020 6465 6620 6765 745f  ic..    def get_
+0000abf0: 7572 695f 7072 6566 6978 2873 656c 6629  uri_prefix(self)
+0000ac00: 202d 3e20 5552 4950 7265 6669 783a 0a20   -> URIPrefix:. 
+0000ac10: 2020 2020 2020 2073 656c 662e 5f6d 6179         self._may
+0000ac20: 6265 5f72 6566 7265 7368 2829 0a20 2020  be_refresh().   
+0000ac30: 2020 2020 2073 656c 662e 5f6d 6179 6265       self._maybe
+0000ac40: 5f66 6574 6368 2829 0a20 2020 2020 2020  _fetch().       
+0000ac50: 2061 7373 6572 7420 7365 6c66 2e5f 7572   assert self._ur
+0000ac60: 695f 7072 6566 6978 2069 7320 6e6f 7420  i_prefix is not 
+0000ac70: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+0000ac80: 7572 6e20 7365 6c66 2e5f 7572 695f 7072  urn self._uri_pr
+0000ac90: 6566 6978 0a0a 2020 2020 6465 6620 6765  efix..    def ge
+0000aca0: 745f 7469 6d69 6e67 280a 2020 2020 2020  t_timing(.      
+0000acb0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000acc0: 2020 2020 2020 2020 626c 6163 6b6c 6973          blacklis
+0000acd0: 743a 204f 7074 696f 6e61 6c5b 4c69 7374  t: Optional[List
+0000ace0: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
+0000acf0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+0000ad00: 5469 6d69 6e67 5265 7375 6c74 3a0a 2020  TimingResult:.  
+0000ad10: 2020 2020 2020 626c 6973 7420 3d20 5b5d        blist = []
+0000ad20: 2069 6620 626c 6163 6b6c 6973 7420 6973   if blacklist is
+0000ad30: 204e 6f6e 6520 656c 7365 2062 6c61 636b   None else black
+0000ad40: 6c69 7374 0a20 2020 2020 2020 206e 6f64  list.        nod
+0000ad50: 655f 7469 6d69 6e67 3a20 4469 6374 5b73  e_timing: Dict[s
+0000ad60: 7472 2c20 4e6f 6465 5469 6d69 6e67 5d20  tr, NodeTiming] 
+0000ad70: 3d20 7b7d 0a20 2020 2020 2020 206e 6f64  = {}.        nod
+0000ad80: 6573 203d 2073 656c 662e 6765 745f 6e6f  es = self.get_no
+0000ad90: 6465 7328 290a 0a20 2020 2020 2020 2064  des()..        d
+0000ada0: 6566 2067 6574 5f66 696c 7465 7264 5f74  ef get_filterd_t
+0000adb0: 696d 6573 280a 2020 2020 2020 2020 2020  imes(.          
+0000adc0: 2020 2020 2020 6e6f 6465 5f74 696d 653a        node_time:
+0000add0: 204c 6973 745b 5469 6d69 6e67 5d29 202d   List[Timing]) -
+0000ade0: 3e20 5475 706c 655b 666c 6f61 742c 2066  > Tuple[float, f
+0000adf0: 6c6f 6174 2c20 4c69 7374 5b54 696d 696e  loat, List[Timin
+0000ae00: 675d 5d3a 0a20 2020 2020 2020 2020 2020  g]]:.           
+0000ae10: 2066 6e73 203d 205b 5d0a 2020 2020 2020   fns = [].      
+0000ae20: 2020 2020 2020 6e6f 6465 5f74 6f74 616c        node_total
+0000ae30: 203d 2030 2e30 0a20 2020 2020 2020 2020   = 0.0.         
+0000ae40: 2020 2066 6f72 2076 616c 7565 2069 6e20     for value in 
+0000ae50: 6e6f 6465 5f74 696d 653a 0a20 2020 2020  node_time:.     
+0000ae60: 2020 2020 2020 2020 2020 2069 6620 7661             if va
+0000ae70: 6c75 655b 226e 616d 6522 5d20 6e6f 7420  lue["name"] not 
+0000ae80: 696e 2062 6c69 7374 3a0a 2020 2020 2020  in blist:.      
+0000ae90: 2020 2020 2020 2020 2020 2020 2020 666e                fn
+0000aea0: 732e 6170 7065 6e64 2876 616c 7565 290a  s.append(value).
 0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 2065 7863 5b30 5d20 3d20 650a 2020 2020   exc[0] = e.    
-0000aed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000aee0: 726e 0a20 2020 2020 2020 2020 2020 2068  rn.            h
-0000aef0: 616c 665f 6978 3a20 696e 7420 3d20 6c65  alf_ix: int = le
-0000af00: 6e28 6375 7229 202f 2f20 320a 2020 2020  n(cur) // 2.    
-0000af10: 2020 2020 2020 2020 6172 6773 5f66 6972          args_fir
-0000af20: 7374 203d 2028 6375 725b 3a68 616c 665f  st = (cur[:half_
-0000af30: 6978 5d2c 206f 6666 7365 7429 0a20 2020  ix], offset).   
-0000af40: 2020 2020 2020 2020 2061 7267 735f 7365           args_se
-0000af50: 636f 6e64 203d 2028 6375 725b 6861 6c66  cond = (cur[half
-0000af60: 5f69 783a 5d2c 206f 6666 7365 7420 2b20  _ix:], offset + 
-0000af70: 6861 6c66 5f69 7829 0a20 2020 2020 2020  half_ix).       
-0000af80: 2020 2020 2069 6620 6c65 6e28 6163 7469       if len(acti
-0000af90: 7665 5f74 6873 2920 3c20 6d61 785f 7468  ve_ths) < max_th
-0000afa0: 7265 6164 733a 0a20 2020 2020 2020 2020  reads:.         
-0000afb0: 2020 2020 2020 2063 6f6d 705f 7468 203d         comp_th =
-0000afc0: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
-0000afd0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-0000afe0: 2020 2020 2020 2074 6172 6765 743d 636f         target=co
-0000aff0: 6d70 7574 655f 6861 6c66 2c20 6172 6773  mpute_half, args
-0000b000: 3d61 7267 735f 6669 7273 7429 0a20 2020  =args_first).   
-0000b010: 2020 2020 2020 2020 2020 2020 2061 6374               act
-0000b020: 6976 655f 7468 732e 6164 6428 636f 6d70  ive_ths.add(comp
-0000b030: 5f74 6829 0a20 2020 2020 2020 2020 2020  _th).           
-0000b040: 2020 2020 2063 6f6d 705f 7468 2e73 7461       comp_th.sta
-0000b050: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
-0000b060: 2020 2020 2063 6f6d 7075 7465 5f68 616c       compute_hal
-0000b070: 6628 2a61 7267 735f 7365 636f 6e64 290a  f(*args_second).
-0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 636f 6d70 5f74 682e 6a6f 696e 2829 0a20  comp_th.join(). 
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000b0b0: 6374 6976 655f 7468 732e 7265 6d6f 7665  ctive_ths.remove
-0000b0c0: 2863 6f6d 705f 7468 290a 2020 2020 2020  (comp_th).      
-0000b0d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000b0e0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-0000b0f0: 7574 655f 6861 6c66 282a 6172 6773 5f66  ute_half(*args_f
-0000b100: 6972 7374 290a 2020 2020 2020 2020 2020  irst).          
-0000b110: 2020 2020 2020 636f 6d70 7574 655f 6861        compute_ha
-0000b120: 6c66 282a 6172 6773 5f73 6563 6f6e 6429  lf(*args_second)
-0000b130: 0a0a 2020 2020 2020 2020 636f 6d70 7574  ..        comput
-0000b140: 655f 6861 6c66 2869 6e70 7574 732c 2030  e_half(inputs, 0
-0000b150: 290a 2020 2020 2020 2020 666f 7220 7265  ).        for re
-0000b160: 6d61 696e 5f74 6820 696e 2061 6374 6976  main_th in activ
-0000b170: 655f 7468 733a 0a20 2020 2020 2020 2020  e_ths:.         
-0000b180: 2020 2072 656d 6169 6e5f 7468 2e6a 6f69     remain_th.joi
-0000b190: 6e28 290a 2020 2020 2020 2020 7261 6973  n().        rais
-0000b1a0: 655f 6520 3d20 6578 635b 305d 0a20 2020  e_e = exc[0].   
-0000b1b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000b1c0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000b1d0: 6e63 6528 7261 6973 655f 652c 2042 6173  nce(raise_e, Bas
-0000b1e0: 6545 7863 6570 7469 6f6e 293a 0a20 2020  eException):.   
-0000b1f0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000b200: 7365 2072 6169 7365 5f65 2020 2320 7079  se raise_e  # py
-0000b210: 6c69 6e74 3a20 6469 7361 626c 653d 7261  lint: disable=ra
-0000b220: 6973 696e 672d 6261 642d 7479 7065 0a20  ising-bad-type. 
-0000b230: 2020 2020 2020 2065 7863 6570 7420 5265         except Re
-0000b240: 7175 6573 7445 7863 6570 7469 6f6e 2061  questException a
-0000b250: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0000b260: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000b270: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000b280: 2020 2022 7265 7175 6573 7420 6572 726f     "request erro
-0000b290: 7220 7768 696c 6520 7072 6f63 6573 7369  r while processi
-0000b2a0: 6e67 2e20 7072 6f63 6573 7369 6e67 2074  ng. processing t
-0000b2b0: 696d 6520 7065 7220 6261 7463 6820 220a  ime per batch ".
-0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2d0: 226d 6967 6874 2062 6520 746f 6f20 6c61  "might be too la
-0000b2e0: 7267 652e 2074 7279 2072 6564 7563 696e  rge. try reducin
-0000b2f0: 6720 7370 6c69 745f 7468 2229 2066 726f  g split_th") fro
-0000b300: 6d20 650a 2020 2020 2020 2020 7265 7475  m e.        retu
-0000b310: 726e 2072 6573 5f61 7272 0a0a 2020 2020  rn res_arr..    
-0000b320: 6465 6620 6479 6e61 6d69 635f 6c69 7374  def dynamic_list
-0000b330: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0000b340: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000b350: 696e 7075 7473 3a20 4c69 7374 5b41 6e79  inputs: List[Any
-0000b360: 5d2c 0a20 2020 2020 2020 2020 2020 2069  ],.            i
-0000b370: 6e70 7574 5f6b 6579 3a20 4f70 7469 6f6e  nput_key: Option
-0000b380: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000b390: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000b3a0: 7574 5f6b 6579 3a20 4f70 7469 6f6e 616c  ut_key: Optional
-0000b3b0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000b3c0: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
-0000b3d0: 7468 3a20 4f70 7469 6f6e 616c 5b69 6e74  th: Optional[int
-0000b3e0: 5d20 3d20 3130 3030 2c0a 2020 2020 2020  ] = 1000,.      
-0000b3f0: 2020 2020 2020 6d61 785f 7468 7265 6164        max_thread
-0000b400: 733a 2069 6e74 203d 2035 302c 0a20 2020  s: int = 50,.   
-0000b410: 2020 2020 2020 2020 2066 6f72 6d61 745f           format_
-0000b420: 6d65 7468 6f64 3a20 7374 7220 3d20 2273  method: str = "s
-0000b430: 696d 706c 6522 2c0a 2020 2020 2020 2020  imple",.        
-0000b440: 2020 2020 666f 7263 655f 6b65 7973 3a20      force_keys: 
-0000b450: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-0000b460: 2020 2020 2020 2020 2020 6e6f 5f63 6163            no_cac
-0000b470: 6865 3a20 626f 6f6c 203d 2046 616c 7365  he: bool = False
-0000b480: 2920 2d3e 204c 6973 745b 416e 795d 3a0a  ) -> List[Any]:.
-0000b490: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b4a0: 5f63 6c69 656e 742e 5f61 7069 5f76 6572  _client._api_ver
-0000b4b0: 7369 6f6e 203c 2035 3a0a 2020 2020 2020  sion < 5:.      
-0000b4c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000b4d0: 662e 5f6c 6567 6163 795f 6479 6e61 6d69  f._legacy_dynami
-0000b4e0: 635f 6c69 7374 280a 2020 2020 2020 2020  c_list(.        
-0000b4f0: 2020 2020 2020 2020 696e 7075 7473 2c0a          inputs,.
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 696e 7075 745f 6b65 793d 696e 7075 745f  input_key=input_
-0000b520: 6b65 792c 0a20 2020 2020 2020 2020 2020  key,.           
-0000b530: 2020 2020 206f 7574 7075 745f 6b65 793d       output_key=
-0000b540: 6f75 7470 7574 5f6b 6579 2c0a 2020 2020  output_key,.    
-0000b550: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
-0000b560: 745f 7468 3d4e 6f6e 652c 0a20 2020 2020  t_th=None,.     
-0000b570: 2020 2020 2020 2020 2020 206d 6178 5f74             max_t
-0000b580: 6872 6561 6473 3d6d 6178 5f74 6872 6561  hreads=max_threa
-0000b590: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-0000b5a0: 2020 2020 666f 726d 6174 5f6d 6574 686f      format_metho
-0000b5b0: 643d 666f 726d 6174 5f6d 6574 686f 642c  d=format_method,
-0000b5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b5d0: 2066 6f72 6365 5f6b 6579 733d 666f 7263   force_keys=forc
-0000b5e0: 655f 6b65 7973 2c0a 2020 2020 2020 2020  e_keys,.        
-0000b5f0: 2020 2020 2020 2020 6e6f 5f63 6163 6865          no_cache
-0000b600: 3d6e 6f5f 6361 6368 6529 0a0a 2020 2020  =no_cache)..    
-0000b610: 2020 2020 6966 2073 706c 6974 5f74 6820      if split_th 
-0000b620: 6973 204e 6f6e 6520 6f72 206c 656e 2869  is None or len(i
-0000b630: 6e70 7574 7329 203c 3d20 7370 6c69 745f  nputs) <= split_
-0000b640: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-0000b650: 7265 7320 3d20 6361 7374 2844 796e 616d  res = cast(Dynam
-0000b660: 6963 5265 7375 6c74 732c 2073 656c 662e  icResults, self.
-0000b670: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
-0000b680: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
-0000b690: 2020 2020 2020 4d45 5448 4f44 5f50 4f53        METHOD_POS
-0000b6a0: 542c 2022 2f64 796e 616d 6963 5f6c 6973  T, "/dynamic_lis
-0000b6b0: 7422 2c20 7b0a 2020 2020 2020 2020 2020  t", {.          
-0000b6c0: 2020 2020 2020 2020 2020 2266 6f72 6365            "force
-0000b6d0: 5f6b 6579 7322 3a20 666f 7263 655f 6b65  _keys": force_ke
-0000b6e0: 7973 2c0a 2020 2020 2020 2020 2020 2020  ys,.            
-0000b6f0: 2020 2020 2020 2020 2266 6f72 6d61 7422          "format"
-0000b700: 3a20 666f 726d 6174 5f6d 6574 686f 642c  : format_method,
-0000b710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b720: 2020 2020 2022 696e 7075 745f 6b65 7922       "input_key"
-0000b730: 3a20 696e 7075 745f 6b65 792c 0a20 2020  : input_key,.   
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2022 696e 7075 7473 223a 2069 6e70 7574   "inputs": input
-0000b760: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000b770: 2020 2020 2020 2022 6e6f 5f63 6163 6865         "no_cache
-0000b780: 223a 206e 6f5f 6361 6368 652c 0a20 2020  ": no_cache,.   
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2022 6f75 7470 7574 5f6b 6579 223a 206f   "output_key": o
-0000b7b0: 7574 7075 745f 6b65 792c 0a20 2020 2020  utput_key,.     
-0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000b7d0: 6461 6722 3a20 7365 6c66 2e67 6574 5f75  dag": self.get_u
-0000b7e0: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
-0000b7f0: 2020 2020 2020 7d29 290a 2020 2020 2020        })).      
-0000b800: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000b810: 5b22 7265 7375 6c74 7322 5d0a 0a20 2020  ["results"]..   
-0000b820: 2020 2020 2073 706c 6974 5f6e 756d 3a20       split_num: 
-0000b830: 696e 7420 3d20 7370 6c69 745f 7468 0a20  int = split_th. 
-0000b840: 2020 2020 2020 2061 7373 6572 7420 7370         assert sp
-0000b850: 6c69 745f 6e75 6d20 3e20 300a 0a20 2020  lit_num > 0..   
-0000b860: 2020 2020 2064 6566 2063 6f6d 7075 7465       def compute
-0000b870: 5f64 796e 616d 6963 5f6c 6973 7428 6375  _dynamic_list(cu
-0000b880: 723a 2069 6e74 2c20 5f3a 2074 6872 6561  r: int, _: threa
-0000b890: 6469 6e67 2e52 4c6f 636b 2920 2d3e 2041  ding.RLock) -> A
-0000b8a0: 6e79 3a0a 2020 2020 2020 2020 2020 2020  ny:.            
-0000b8b0: 7265 7375 6c74 203d 204e 6f6e 650a 2020  result = None.  
-0000b8c0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b8e0: 6573 756c 7420 3d20 7365 6c66 2e64 796e  esult = self.dyn
-0000b8f0: 616d 6963 5f6c 6973 7428 0a20 2020 2020  amic_list(.     
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000b910: 6e70 7574 735b 6375 723a 6375 7220 2b20  nputs[cur:cur + 
-0000b920: 7370 6c69 745f 6e75 6d5d 2c0a 2020 2020  split_num],.    
-0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 696e 7075 745f 6b65 793d 696e 7075 745f  input_key=input_
-0000b950: 6b65 792c 0a20 2020 2020 2020 2020 2020  key,.           
-0000b960: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000b970: 6b65 793d 6f75 7470 7574 5f6b 6579 2c0a  key=output_key,.
-0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b990: 2020 2020 7370 6c69 745f 7468 3d4e 6f6e      split_th=Non
-0000b9a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000b9b0: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
-0000b9c0: 6473 3d6d 6178 5f74 6872 6561 6473 2c0a  ds=max_threads,.
-0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9e0: 2020 2020 666f 726d 6174 5f6d 6574 686f      format_metho
-0000b9f0: 643d 666f 726d 6174 5f6d 6574 686f 642c  d=format_method,
-0000ba00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ba10: 2020 2020 2066 6f72 6365 5f6b 6579 733d       force_keys=
-0000ba20: 666f 7263 655f 6b65 7973 2c0a 2020 2020  force_keys,.    
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba40: 6e6f 5f63 6163 6865 3d6e 6f5f 6361 6368  no_cache=no_cach
-0000ba50: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
-0000ba60: 7863 6570 7420 4261 7365 4578 6365 7074  xcept BaseExcept
-0000ba70: 696f 6e20 6173 2065 3a20 2023 2070 796c  ion as e:  # pyl
-0000ba80: 696e 743a 2064 6973 6162 6c65 3d62 726f  int: disable=bro
-0000ba90: 6164 2d65 7863 6570 740a 2020 2020 2020  ad-except.      
-0000baa0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000bad0: 2865 2c20 4261 7365 4578 6365 7074 696f  (e, BaseExceptio
-0000bae0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-0000baf0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000bb00: 6520 650a 2020 2020 2020 2020 2020 2020  e e.            
-0000bb10: 2020 2020 6578 6365 7074 2052 6571 7565      except Reque
-0000bb20: 7374 4578 6365 7074 696f 6e20 6173 2065  stException as e
-0000bb30: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
-0000bb40: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000bb50: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2020 2272 6571 7565 7374 2065 7272 6f72    "request error
-0000bb80: 2077 6869 6c65 2070 726f 6365 7373 696e   while processin
-0000bb90: 672e 2229 2066 726f 6d20 6572 720a 2020  g.") from err.  
-0000bba0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000bbb0: 2072 6573 756c 740a 0a20 2020 2020 2020   result..       
-0000bbc0: 2074 6173 6b73 203d 206c 6973 7428 7261   tasks = list(ra
-0000bbd0: 6e67 6528 302c 206c 656e 2869 6e70 7574  nge(0, len(input
-0000bbe0: 7329 2c20 7370 6c69 745f 6e75 6d29 290a  s), split_num)).
-0000bbf0: 2020 2020 2020 2020 6172 7220 3d20 636f          arr = co
-0000bc00: 6d70 7574 655f 7061 7261 6c6c 656c 280a  mpute_parallel(.
-0000bc10: 2020 2020 2020 2020 2020 2020 7461 736b              task
-0000bc20: 732c 2063 6f6d 7075 7465 5f64 796e 616d  s, compute_dynam
-0000bc30: 6963 5f6c 6973 742c 204e 6f6e 652c 206d  ic_list, None, m
-0000bc40: 6178 5f74 6872 6561 6473 290a 2020 2020  ax_threads).    
-0000bc50: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
-0000bc60: 6974 6572 746f 6f6c 732e 6368 6169 6e28  itertools.chain(
-0000bc70: 2a61 7272 2929 0a0a 2020 2020 6465 6620  *arr))..    def 
-0000bc80: 6479 6e61 6d69 6328 7365 6c66 2c20 696e  dynamic(self, in
-0000bc90: 7075 745f 6461 7461 3a20 4279 7465 7349  put_data: BytesI
-0000bca0: 4f29 202d 3e20 4f70 7469 6f6e 616c 5b42  O) -> Optional[B
-0000bcb0: 7974 6552 6573 706f 6e73 655d 3a0a 2020  yteResponse]:.  
-0000bcc0: 2020 2020 2020 6375 725f 7265 732c 2063        cur_res, c
-0000bcd0: 7479 7065 203d 2073 656c 662e 5f63 6c69  type = self._cli
-0000bce0: 656e 742e 7265 7175 6573 745f 6279 7465  ent.request_byte
-0000bcf0: 7328 0a20 2020 2020 2020 2020 2020 204d  s(.            M
-0000bd00: 4554 484f 445f 4649 4c45 2c20 222f 6479  ETHOD_FILE, "/dy
-0000bd10: 6e61 6d69 6322 2c20 7b0a 2020 2020 2020  namic", {.      
-0000bd20: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
-0000bd30: 2073 656c 662e 6765 745f 7572 6928 292c   self.get_uri(),
-0000bd40: 0a20 2020 2020 2020 2020 2020 207d 2c20  .            }, 
-0000bd50: 6669 6c65 733d 7b0a 2020 2020 2020 2020  files={.        
-0000bd60: 2020 2020 2020 2020 2266 696c 6522 3a20          "file": 
-0000bd70: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
-0000bd80: 2020 2020 2020 2020 7d29 0a20 2020 2020          }).     
-0000bd90: 2020 2072 6574 7572 6e20 696e 7465 7270     return interp
-0000bda0: 7265 745f 6374 7970 6528 6375 725f 7265  ret_ctype(cur_re
-0000bdb0: 732c 2063 7479 7065 290a 0a20 2020 2064  s, ctype)..    d
-0000bdc0: 6566 2064 796e 616d 6963 5f6f 626a 2873  ef dynamic_obj(s
-0000bdd0: 656c 662c 2069 6e70 7574 5f6f 626a 3a20  elf, input_obj: 
-0000bde0: 416e 7929 202d 3e20 4f70 7469 6f6e 616c  Any) -> Optional
-0000bdf0: 5b42 7974 6552 6573 706f 6e73 655d 3a0a  [ByteResponse]:.
-0000be00: 2020 2020 2020 2020 6269 6f20 3d20 4279          bio = By
-0000be10: 7465 7349 4f28 6a73 6f6e 2e64 756d 7073  tesIO(json.dumps
-0000be20: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-0000be30: 7075 745f 6f62 6a2c 0a20 2020 2020 2020  put_obj,.       
-0000be40: 2020 2020 2073 6570 6172 6174 6f72 733d       separators=
-0000be50: 2822 2c22 2c20 223a 2229 2c0a 2020 2020  (",", ":"),.    
-0000be60: 2020 2020 2020 2020 696e 6465 6e74 3d4e          indent=N
-0000be70: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000be80: 2073 6f72 745f 6b65 7973 3d54 7275 6529   sort_keys=True)
-0000be90: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-0000bea0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000beb0: 2073 656c 662e 6479 6e61 6d69 6328 6269   self.dynamic(bi
-0000bec0: 6f29 0a0a 2020 2020 6465 6620 6479 6e61  o)..    def dyna
-0000bed0: 6d69 635f 6173 796e 6328 0a20 2020 2020  mic_async(.     
-0000bee0: 2020 2020 2020 2073 656c 662c 2069 6e70         self, inp
-0000bef0: 7574 5f64 6174 613a 204c 6973 745b 4279  ut_data: List[By
-0000bf00: 7465 7349 4f5d 2920 2d3e 204c 6973 745b  tesIO]) -> List[
-0000bf10: 2743 6f6d 7075 7461 7469 6f6e 4861 6e64  'ComputationHand
-0000bf20: 6c65 275d 3a0a 2020 2020 2020 2020 6e61  le']:.        na
-0000bf30: 6d65 7320 3d20 5b66 2266 696c 657b 706f  mes = [f"file{po
-0000bf40: 737d 2220 666f 7220 706f 7320 696e 2072  s}" for pos in r
-0000bf50: 616e 6765 286c 656e 2869 6e70 7574 5f64  ange(len(input_d
-0000bf60: 6174 6129 295d 0a20 2020 2020 2020 2072  ata))].        r
-0000bf70: 6573 3a20 4469 6374 5b73 7472 2c20 7374  es: Dict[str, st
-0000bf80: 725d 203d 2073 656c 662e 5f63 6c69 656e  r] = self._clien
-0000bf90: 742e 7265 7175 6573 745f 6a73 6f6e 280a  t.request_json(.
-0000bfa0: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
-0000bfb0: 4f44 5f46 494c 452c 2022 2f64 796e 616d  OD_FILE, "/dynam
-0000bfc0: 6963 5f61 7379 6e63 222c 207b 0a20 2020  ic_async", {.   
-0000bfd0: 2020 2020 2020 2020 2020 2020 2022 6461               "da
-0000bfe0: 6722 3a20 7365 6c66 2e67 6574 5f75 7269  g": self.get_uri
-0000bff0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0000c000: 7d2c 2066 696c 6573 3d64 6963 7428 7a69  }, files=dict(zi
-0000c010: 7028 6e61 6d65 732c 2069 6e70 7574 5f64  p(names, input_d
-0000c020: 6174 6129 2929 0a20 2020 2020 2020 2072  ata))).        r
-0000c030: 6574 7572 6e20 5b0a 2020 2020 2020 2020  eturn [.        
-0000c040: 2020 2020 436f 6d70 7574 6174 696f 6e48      ComputationH
-0000c050: 616e 646c 6528 0a20 2020 2020 2020 2020  andle(.         
-0000c060: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000c070: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000c080: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
-0000c090: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-0000c0a0: 5f64 796e 616d 6963 5f65 7272 6f72 5f6d  _dynamic_error_m
-0000c0b0: 6573 7361 6765 2c0a 2020 2020 2020 2020  essage,.        
-0000c0c0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000c0d0: 5f64 796e 616d 6963 5f65 7272 6f72 5f6d  _dynamic_error_m
-0000c0e0: 6573 7361 6765 290a 2020 2020 2020 2020  essage).        
-0000c0f0: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
-0000c100: 6e61 6d65 735d 0a0a 2020 2020 6465 6620  names]..    def 
-0000c110: 7365 745f 6479 6e61 6d69 635f 6572 726f  set_dynamic_erro
-0000c120: 725f 6d65 7373 6167 6528 7365 6c66 2c20  r_message(self, 
-0000c130: 6d73 673a 204f 7074 696f 6e61 6c5b 7374  msg: Optional[st
-0000c140: 725d 2920 2d3e 204e 6f6e 653a 0a20 2020  r]) -> None:.   
-0000c150: 2020 2020 2073 656c 662e 5f64 796e 616d       self._dynam
-0000c160: 6963 5f65 7272 6f72 203d 206d 7367 0a0a  ic_error = msg..
-0000c170: 2020 2020 6465 6620 6765 745f 6479 6e61      def get_dyna
-0000c180: 6d69 635f 6572 726f 725f 6d65 7373 6167  mic_error_messag
-0000c190: 6528 7365 6c66 2920 2d3e 204f 7074 696f  e(self) -> Optio
-0000c1a0: 6e61 6c5b 7374 725d 3a0a 2020 2020 2020  nal[str]:.      
-0000c1b0: 2020 7265 7475 726e 2073 656c 662e 5f64    return self._d
-0000c1c0: 796e 616d 6963 5f65 7272 6f72 0a0a 2020  ynamic_error..  
-0000c1d0: 2020 6465 6620 6479 6e61 6d69 635f 6173    def dynamic_as
-0000c1e0: 796e 635f 6f62 6a28 0a20 2020 2020 2020  ync_obj(.       
-0000c1f0: 2020 2020 2073 656c 662c 2069 6e70 7574       self, input
-0000c200: 5f64 6174 613a 204c 6973 745b 416e 795d  _data: List[Any]
-0000c210: 2920 2d3e 204c 6973 745b 2743 6f6d 7075  ) -> List['Compu
-0000c220: 7461 7469 6f6e 4861 6e64 6c65 275d 3a0a  tationHandle']:.
-0000c230: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000c240: 656c 662e 6479 6e61 6d69 635f 6173 796e  elf.dynamic_asyn
-0000c250: 6328 5b0a 2020 2020 2020 2020 2020 2020  c([.            
-0000c260: 4279 7465 7349 4f28 6a73 6f6e 2e64 756d  BytesIO(json.dum
-0000c270: 7073 280a 2020 2020 2020 2020 2020 2020  ps(.            
-0000c280: 2020 2020 696e 7075 745f 6f62 6a2c 0a20      input_obj,. 
-0000c290: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c2a0: 6570 6172 6174 6f72 733d 2822 2c22 2c20  eparators=(",", 
-0000c2b0: 223a 2229 2c0a 2020 2020 2020 2020 2020  ":"),.          
-0000c2c0: 2020 2020 2020 696e 6465 6e74 3d4e 6f6e        indent=Non
-0000c2d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000c2e0: 2020 2073 6f72 745f 6b65 7973 3d54 7275     sort_keys=Tru
-0000c2f0: 6529 2e65 6e63 6f64 6528 2275 7466 2d38  e).encode("utf-8
-0000c300: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-0000c310: 666f 7220 696e 7075 745f 6f62 6a20 696e  for input_obj in
-0000c320: 2069 6e70 7574 5f64 6174 610a 2020 2020   input_data.    
-0000c330: 2020 2020 5d29 0a0a 2020 2020 6465 6620      ])..    def 
-0000c340: 6765 745f 6479 6e61 6d69 635f 7265 7375  get_dynamic_resu
-0000c350: 6c74 2873 656c 662c 2076 616c 7565 5f69  lt(self, value_i
-0000c360: 643a 2073 7472 2920 2d3e 204f 7074 696f  d: str) -> Optio
-0000c370: 6e61 6c5b 4279 7465 5265 7370 6f6e 7365  nal[ByteResponse
-0000c380: 5d3a 0a20 2020 2020 2020 2074 7279 3a0a  ]:.        try:.
-0000c390: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
-0000c3a0: 7265 732c 2063 7479 7065 203d 2073 656c  res, ctype = sel
-0000c3b0: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
-0000c3c0: 745f 6279 7465 7328 0a20 2020 2020 2020  t_bytes(.       
-0000c3d0: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-0000c3e0: 4745 542c 2022 2f64 796e 616d 6963 5f72  GET, "/dynamic_r
-0000c3f0: 6573 756c 7422 2c20 7b0a 2020 2020 2020  esult", {.      
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-0000c410: 6167 223a 2073 656c 662e 6765 745f 7572  ag": self.get_ur
-0000c420: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
-0000c430: 2020 2020 2020 2020 2022 6964 223a 2076           "id": v
-0000c440: 616c 7565 5f69 642c 0a20 2020 2020 2020  alue_id,.       
-0000c450: 2020 2020 2020 2020 207d 290a 2020 2020           }).    
-0000c460: 2020 2020 6578 6365 7074 2048 5454 5045      except HTTPE
-0000c470: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-0000c480: 2020 2020 2020 2069 6620 652e 7265 7370         if e.resp
-0000c490: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
-0000c4a0: 203d 3d20 3430 343a 0a20 2020 2020 2020   == 404:.       
-0000c4b0: 2020 2020 2020 2020 2072 6169 7365 204b           raise K
-0000c4c0: 6579 4572 726f 7228 6622 7661 6c75 655f  eyError(f"value_
-0000c4d0: 6964 207b 7661 6c75 655f 6964 7d20 646f  id {value_id} do
-0000c4e0: 6573 206e 6f74 2065 7869 7374 2229 2066  es not exist") f
-0000c4f0: 726f 6d20 650a 2020 2020 2020 2020 2020  rom e.          
-0000c500: 2020 7261 6973 6520 650a 2020 2020 2020    raise e.      
-0000c510: 2020 7265 7475 726e 2069 6e74 6572 7072    return interpr
-0000c520: 6574 5f63 7479 7065 2863 7572 5f72 6573  et_ctype(cur_res
-0000c530: 2c20 6374 7970 6529 0a0a 2020 2020 6465  , ctype)..    de
-0000c540: 6620 6765 745f 6479 6e61 6d69 635f 7374  f get_dynamic_st
-0000c550: 6174 7573 280a 2020 2020 2020 2020 2020  atus(.          
-0000c560: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000c570: 2020 2020 7661 6c75 655f 6964 733a 204c      value_ids: L
-0000c580: 6973 745b 2743 6f6d 7075 7461 7469 6f6e  ist['Computation
-0000c590: 4861 6e64 6c65 275d 2920 2d3e 2044 6963  Handle']) -> Dic
-0000c5a0: 745b 0a20 2020 2020 2020 2020 2020 2020  t[.             
-0000c5b0: 2020 2027 436f 6d70 7574 6174 696f 6e48     'ComputationH
-0000c5c0: 616e 646c 6527 2c20 5175 6575 6553 7461  andle', QueueSta
-0000c5d0: 7475 735d 3a0a 2020 2020 2020 2020 7265  tus]:.        re
-0000c5e0: 7320 3d20 6361 7374 2844 796e 616d 6963  s = cast(Dynamic
-0000c5f0: 5374 6174 7573 5265 7370 6f6e 7365 2c20  StatusResponse, 
-0000c600: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
-0000c610: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-0000c620: 2020 2020 2020 204d 4554 484f 445f 504f         METHOD_PO
-0000c630: 5354 2c20 222f 6479 6e61 6d69 635f 7374  ST, "/dynamic_st
-0000c640: 6174 7573 222c 207b 0a20 2020 2020 2020  atus", {.       
-0000c650: 2020 2020 2020 2020 2022 7661 6c75 655f           "value_
-0000c660: 6964 7322 3a20 5b76 616c 7565 5f69 642e  ids": [value_id.
-0000c670: 6765 745f 6964 2829 2066 6f72 2076 616c  get_id() for val
-0000c680: 7565 5f69 6420 696e 2076 616c 7565 5f69  ue_id in value_i
-0000c690: 6473 5d2c 0a20 2020 2020 2020 2020 2020  ds],.           
-0000c6a0: 2020 2020 2022 6461 6722 3a20 7365 6c66       "dag": self
-0000c6b0: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
-0000c6c0: 2020 2020 2020 2020 7d29 290a 2020 2020          })).    
-0000c6d0: 2020 2020 7374 6174 7573 203d 2072 6573      status = res
-0000c6e0: 5b22 7374 6174 7573 225d 0a20 2020 2020  ["status"].     
-0000c6f0: 2020 2068 6e64 5f6d 6170 203d 207b 7661     hnd_map = {va
-0000c700: 6c75 655f 6964 2e67 6574 5f69 6428 293a  lue_id.get_id():
-0000c710: 2076 616c 7565 5f69 6420 666f 7220 7661   value_id for va
-0000c720: 6c75 655f 6964 2069 6e20 7661 6c75 655f  lue_id in value_
-0000c730: 6964 737d 0a20 2020 2020 2020 2072 6574  ids}.        ret
-0000c740: 7572 6e20 7b0a 2020 2020 2020 2020 2020  urn {.          
-0000c750: 2020 686e 645f 6d61 705b 6b65 795d 3a20    hnd_map[key]: 
-0000c760: 6361 7374 2851 7565 7565 5374 6174 7573  cast(QueueStatus
-0000c770: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
-0000c780: 2020 2020 2066 6f72 206b 6579 2c20 7661       for key, va
-0000c790: 6c75 6520 696e 2073 7461 7475 732e 6974  lue in status.it
-0000c7a0: 656d 7328 290a 2020 2020 2020 2020 7d0a  ems().        }.
-0000c7b0: 0a20 2020 2064 6566 2067 6574 5f64 796e  .    def get_dyn
-0000c7c0: 616d 6963 5f62 756c 6b28 0a20 2020 2020  amic_bulk(.     
-0000c7d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000c7e0: 2020 2020 2020 2020 2069 6e70 7574 5f64           input_d
-0000c7f0: 6174 613a 204c 6973 745b 4279 7465 7349  ata: List[BytesI
-0000c800: 4f5d 2c0a 2020 2020 2020 2020 2020 2020  O],.            
-0000c810: 6d61 785f 6275 6666 3a20 696e 7420 3d20  max_buff: int = 
-0000c820: 3430 3030 2c0a 2020 2020 2020 2020 2020  4000,.          
-0000c830: 2020 626c 6f63 6b5f 7369 7a65 3a20 696e    block_size: in
-0000c840: 7420 3d20 352c 0a20 2020 2020 2020 2020  t = 5,.         
-0000c850: 2020 206e 756d 5f74 6872 6561 6473 3a20     num_threads: 
-0000c860: 696e 7420 3d20 3230 2920 2d3e 2049 7465  int = 20) -> Ite
-0000c870: 7261 626c 655b 4f70 7469 6f6e 616c 5b42  rable[Optional[B
-0000c880: 7974 6552 6573 706f 6e73 655d 5d3a 0a0a  yteResponse]]:..
-0000c890: 2020 2020 2020 2020 6465 6620 6765 7428          def get(
-0000c8a0: 686e 643a 2027 436f 6d70 7574 6174 696f  hnd: 'Computatio
-0000c8b0: 6e48 616e 646c 6527 2920 2d3e 204f 7074  nHandle') -> Opt
-0000c8c0: 696f 6e61 6c5b 4279 7465 5265 7370 6f6e  ional[ByteRespon
-0000c8d0: 7365 5d3a 0a20 2020 2020 2020 2020 2020  se]:.           
-0000c8e0: 2072 6574 7572 6e20 686e 642e 6765 7428   return hnd.get(
-0000c8f0: 290a 0a20 2020 2020 2020 2073 7563 6365  )..        succe
-0000c900: 7373 203d 2046 616c 7365 0a20 2020 2020  ss = False.     
-0000c910: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000c920: 2020 2020 7969 656c 6420 6672 6f6d 2061      yield from a
-0000c930: 7379 6e63 5f63 6f6d 7075 7465 280a 2020  sync_compute(.  
-0000c940: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000c950: 7075 745f 6461 7461 2c0a 2020 2020 2020  put_data,.      
-0000c960: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000c970: 796e 616d 6963 5f61 7379 6e63 2c0a 2020  ynamic_async,.  
-0000c980: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-0000c990: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000c9a0: 2020 206c 616d 6264 613a 2073 656c 662e     lambda: self.
-0000c9b0: 6368 6563 6b5f 7175 6575 655f 7374 6174  check_queue_stat
-0000c9c0: 7328 6d69 6e69 6d61 6c3d 5472 7565 292c  s(minimal=True),
-0000c9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c9e0: 2073 656c 662e 6765 745f 6479 6e61 6d69   self.get_dynami
-0000c9f0: 635f 7374 6174 7573 2c0a 2020 2020 2020  c_status,.      
-0000ca00: 2020 2020 2020 2020 2020 6d61 785f 6275            max_bu
-0000ca10: 6666 2c0a 2020 2020 2020 2020 2020 2020  ff,.            
-0000ca20: 2020 2020 626c 6f63 6b5f 7369 7a65 2c0a      block_size,.
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 6e75 6d5f 7468 7265 6164 7329 0a20 2020  num_threads).   
-0000ca50: 2020 2020 2020 2020 2073 7563 6365 7373           success
-0000ca60: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-0000ca70: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
-0000ca80: 2020 2020 2069 6620 7375 6363 6573 733a       if success:
-0000ca90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000caa0: 2073 656c 662e 7365 745f 6479 6e61 6d69   self.set_dynami
-0000cab0: 635f 6572 726f 725f 6d65 7373 6167 6528  c_error_message(
-0000cac0: 4e6f 6e65 290a 0a20 2020 2064 6566 2067  None)..    def g
-0000cad0: 6574 5f64 796e 616d 6963 5f62 756c 6b5f  et_dynamic_bulk_
-0000cae0: 6f62 6a28 0a20 2020 2020 2020 2020 2020  obj(.           
-0000caf0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-0000cb00: 2020 2069 6e70 7574 5f64 6174 613a 204c     input_data: L
-0000cb10: 6973 745b 416e 795d 2c0a 2020 2020 2020  ist[Any],.      
-0000cb20: 2020 2020 2020 6d61 785f 6275 6666 3a20        max_buff: 
-0000cb30: 696e 7420 3d20 3430 3030 2c0a 2020 2020  int = 4000,.    
-0000cb40: 2020 2020 2020 2020 626c 6f63 6b5f 7369          block_si
-0000cb50: 7a65 3a20 696e 7420 3d20 352c 0a20 2020  ze: int = 5,.   
-0000cb60: 2020 2020 2020 2020 206e 756d 5f74 6872           num_thr
-0000cb70: 6561 6473 3a20 696e 7420 3d20 3230 2920  eads: int = 20) 
-0000cb80: 2d3e 2049 7465 7261 626c 655b 4f70 7469  -> Iterable[Opti
-0000cb90: 6f6e 616c 5b42 7974 6552 6573 706f 6e73  onal[ByteRespons
-0000cba0: 655d 5d3a 0a0a 2020 2020 2020 2020 6465  e]]:..        de
-0000cbb0: 6620 6765 7428 686e 643a 2027 436f 6d70  f get(hnd: 'Comp
-0000cbc0: 7574 6174 696f 6e48 616e 646c 6527 2920  utationHandle') 
-0000cbd0: 2d3e 204f 7074 696f 6e61 6c5b 4279 7465  -> Optional[Byte
-0000cbe0: 5265 7370 6f6e 7365 5d3a 0a20 2020 2020  Response]:.     
-0000cbf0: 2020 2020 2020 2072 6574 7572 6e20 686e         return hn
-0000cc00: 642e 6765 7428 290a 0a20 2020 2020 2020  d.get()..       
-0000cc10: 2073 7563 6365 7373 203d 2046 616c 7365   success = False
-0000cc20: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000cc30: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-0000cc40: 6672 6f6d 2061 7379 6e63 5f63 6f6d 7075  from async_compu
-0000cc50: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-0000cc60: 2020 2020 696e 7075 745f 6461 7461 2c0a      input_data,.
-0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc80: 7365 6c66 2e64 796e 616d 6963 5f61 7379  self.dynamic_asy
-0000cc90: 6e63 5f6f 626a 2c0a 2020 2020 2020 2020  nc_obj,.        
-0000cca0: 2020 2020 2020 2020 6765 742c 0a20 2020          get,.   
-0000ccb0: 2020 2020 2020 2020 2020 2020 206c 616d               lam
-0000ccc0: 6264 613a 2073 656c 662e 6368 6563 6b5f  bda: self.check_
-0000ccd0: 7175 6575 655f 7374 6174 7328 6d69 6e69  queue_stats(mini
-0000cce0: 6d61 6c3d 5472 7565 292c 0a20 2020 2020  mal=True),.     
-0000ccf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cd00: 6765 745f 6479 6e61 6d69 635f 7374 6174  get_dynamic_stat
-0000cd10: 7573 2c0a 2020 2020 2020 2020 2020 2020  us,.            
-0000cd20: 2020 2020 6d61 785f 6275 6666 2c0a 2020      max_buff,.  
-0000cd30: 2020 2020 2020 2020 2020 2020 2020 626c                bl
-0000cd40: 6f63 6b5f 7369 7a65 2c0a 2020 2020 2020  ock_size,.      
-0000cd50: 2020 2020 2020 2020 2020 6e75 6d5f 7468            num_th
-0000cd60: 7265 6164 7329 0a20 2020 2020 2020 2020  reads).         
-0000cd70: 2020 2073 7563 6365 7373 203d 2054 7275     success = Tru
-0000cd80: 650a 2020 2020 2020 2020 6669 6e61 6c6c  e.        finall
-0000cd90: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-0000cda0: 6620 7375 6363 6573 733a 0a20 2020 2020  f success:.     
-0000cdb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cdc0: 7365 745f 6479 6e61 6d69 635f 6572 726f  set_dynamic_erro
-0000cdd0: 725f 6d65 7373 6167 6528 4e6f 6e65 290a  r_message(None).
-0000cde0: 0a20 2020 2064 6566 205f 7072 6574 7479  .    def _pretty
-0000cdf0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0000ce00: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000ce10: 6e6f 6465 735f 6f6e 6c79 3a20 626f 6f6c  nodes_only: bool
-0000ce20: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
-0000ce30: 6c6f 775f 756e 6963 6f64 653a 2062 6f6f  low_unicode: boo
-0000ce40: 6c2c 0a20 2020 2020 2020 2020 2020 206d  l,.            m
-0000ce50: 6574 686f 643a 204f 7074 696f 6e61 6c5b  ethod: Optional[
-0000ce60: 7374 725d 203d 2022 6163 6365 726e 222c  str] = "accern",
-0000ce70: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
-0000ce80: 6c64 733a 204f 7074 696f 6e61 6c5b 4c69  lds: Optional[Li
-0000ce90: 7374 5b73 7472 5d5d 203d 204e 6f6e 6529  st[str]] = None)
-0000cea0: 202d 3e20 5072 6574 7479 5265 7370 6f6e   -> PrettyRespon
-0000ceb0: 7365 3a0a 2020 2020 2020 2020 6172 6773  se:.        args
-0000cec0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0000ced0: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
-0000cee0: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
-0000cef0: 2020 2020 226e 6f64 6573 5f6f 6e6c 7922      "nodes_only"
-0000cf00: 3a20 6e6f 6465 735f 6f6e 6c79 2c0a 2020  : nodes_only,.  
-0000cf10: 2020 2020 2020 2020 2020 2261 6c6c 6f77            "allow
-0000cf20: 5f75 6e69 636f 6465 223a 2061 6c6c 6f77  _unicode": allow
-0000cf30: 5f75 6e69 636f 6465 2c0a 2020 2020 2020  _unicode,.      
-0000cf40: 2020 2020 2020 226d 6574 686f 6422 3a20        "method": 
-0000cf50: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
-0000cf60: 7d0a 2020 2020 2020 2020 6966 2066 6965  }.        if fie
-0000cf70: 6c64 7320 6973 206e 6f74 204e 6f6e 653a  lds is not None:
-0000cf80: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-0000cf90: 735b 2266 6965 6c64 7322 5d20 3d20 222c  s["fields"] = ",
-0000cfa0: 222e 6a6f 696e 2866 6965 6c64 7329 0a20  ".join(fields). 
-0000cfb0: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
-0000cfc0: 7374 2850 7265 7474 7952 6573 706f 6e73  st(PrettyRespons
-0000cfd0: 652c 2073 656c 662e 5f63 6c69 656e 742e  e, self._client.
-0000cfe0: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
-0000cff0: 2020 2020 2020 2020 2020 4d45 5448 4f44            METHOD
-0000d000: 5f47 4554 2c20 222f 7072 6574 7479 222c  _GET, "/pretty",
-0000d010: 2061 7267 7329 290a 0a20 2020 2064 6566   args))..    def
-0000d020: 2070 7265 7474 7928 0a20 2020 2020 2020   pretty(.       
-0000d030: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000d040: 2020 2020 2020 206e 6f64 6573 5f6f 6e6c         nodes_onl
-0000d050: 793a 2062 6f6f 6c20 3d20 4661 6c73 652c  y: bool = False,
-0000d060: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-0000d070: 6f77 5f75 6e69 636f 6465 3a20 626f 6f6c  ow_unicode: bool
-0000d080: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-0000d090: 2020 2020 206d 6574 686f 643a 204f 7074       method: Opt
-0000d0a0: 696f 6e61 6c5b 7374 725d 203d 2022 646f  ional[str] = "do
-0000d0b0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-0000d0c0: 6669 656c 6473 3a20 4f70 7469 6f6e 616c  fields: Optional
-0000d0d0: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
-0000d0e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000d0f0: 6f75 7470 7574 5f66 6f72 6d61 743a 204f  output_format: O
-0000d100: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-0000d110: 706e 6722 2c0a 2020 2020 2020 2020 2020  png",.          
-0000d120: 2020 6469 7370 6c61 793a 204f 7074 696f    display: Optio
-0000d130: 6e61 6c5b 494f 5b41 6e79 5d5d 203d 2073  nal[IO[Any]] = s
-0000d140: 7973 2e73 7464 6f75 7429 202d 3e20 4f70  ys.stdout) -> Op
-0000d150: 7469 6f6e 616c 5b73 7472 5d3a 0a0a 2020  tional[str]:..  
-0000d160: 2020 2020 2020 6465 6620 7265 6e64 6572        def render
-0000d170: 2876 616c 7565 3a20 7374 7229 202d 3e20  (value: str) -> 
-0000d180: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
-0000d190: 2020 2020 2020 2020 2020 2069 6620 6469             if di
-0000d1a0: 7370 6c61 7920 6973 206e 6f74 204e 6f6e  splay is not Non
-0000d1b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000d1c0: 2020 2064 6973 706c 6179 2e77 7269 7465     display.write
-0000d1d0: 2876 616c 7565 290a 2020 2020 2020 2020  (value).        
-0000d1e0: 2020 2020 2020 2020 6469 7370 6c61 792e          display.
-0000d1f0: 666c 7573 6828 290a 2020 2020 2020 2020  flush().        
-0000d200: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-0000d210: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000d220: 7265 7475 726e 2076 616c 7565 0a0a 2020  return value..  
-0000d230: 2020 2020 2020 6772 6170 685f 7374 7220        graph_str 
-0000d240: 3d20 7365 6c66 2e5f 7072 6574 7479 280a  = self._pretty(.
-0000d250: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-0000d260: 735f 6f6e 6c79 3d6e 6f64 6573 5f6f 6e6c  s_only=nodes_onl
-0000d270: 792c 0a20 2020 2020 2020 2020 2020 2061  y,.            a
-0000d280: 6c6c 6f77 5f75 6e69 636f 6465 3d61 6c6c  llow_unicode=all
-0000d290: 6f77 5f75 6e69 636f 6465 2c0a 2020 2020  ow_unicode,.    
-0000d2a0: 2020 2020 2020 2020 6d65 7468 6f64 3d6d          method=m
-0000d2b0: 6574 686f 642c 0a20 2020 2020 2020 2020  ethod,.         
-0000d2c0: 2020 2066 6965 6c64 733d 6669 656c 6473     fields=fields
-0000d2d0: 295b 2270 7265 7474 7922 5d0a 2020 2020  )["pretty"].    
-0000d2e0: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
-0000d2f0: 2022 6163 6365 726e 223a 0a20 2020 2020   "accern":.     
-0000d300: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000d310: 6e64 6572 2867 7261 7068 5f73 7472 290a  nder(graph_str).
-0000d320: 2020 2020 2020 2020 6966 206d 6574 686f          if metho
-0000d330: 6420 3d3d 2022 646f 7422 3a0a 2020 2020  d == "dot":.    
-0000d340: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000d350: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-0000d360: 6d20 6772 6170 6876 697a 2069 6d70 6f72  m graphviz impor
-0000d370: 7420 536f 7572 6365 0a0a 2020 2020 2020  t Source..      
-0000d380: 2020 2020 2020 2020 2020 6772 6170 6820            graph 
-0000d390: 3d20 536f 7572 6365 2867 7261 7068 5f73  = Source(graph_s
-0000d3a0: 7472 290a 2020 2020 2020 2020 2020 2020  tr).            
-0000d3b0: 2020 2020 6966 206f 7574 7075 745f 666f      if output_fo
-0000d3c0: 726d 6174 203d 3d20 2264 6f74 223a 0a20  rmat == "dot":. 
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2072 6574 7572 6e20 7265 6e64 6572     return render
-0000d3f0: 2867 7261 7068 5f73 7472 290a 2020 2020  (graph_str).    
-0000d400: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0000d410: 7574 7075 745f 666f 726d 6174 203d 3d20  utput_format == 
-0000d420: 2273 7667 223a 0a20 2020 2020 2020 2020  "svg":.         
-0000d430: 2020 2020 2020 2020 2020 2073 7667 5f73             svg_s
-0000d440: 7472 203d 2067 7261 7068 2e70 6970 6528  tr = graph.pipe(
-0000d450: 666f 726d 6174 3d22 7376 6722 290a 2020  format="svg").  
-0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d470: 2020 6966 2064 6973 706c 6179 2069 7320    if display is 
-0000d480: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4a0: 2020 6966 206e 6f74 2069 735f 6a75 7079    if not is_jupy
-0000d4b0: 7465 7228 293a 0a20 2020 2020 2020 2020  ter():.         
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4d0: 2020 2064 6973 706c 6179 2e77 7269 7465     display.write
-0000d4e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d500: 2020 2257 6172 6e69 6e67 3a20 4970 7974    "Warning: Ipyt
-0000d510: 686f 6e20 696e 7374 616e 6365 206e 6f74  hon instance not
-0000d520: 2066 6f75 6e64 2e5c 6e22 290a 2020 2020   found.\n").    
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 2020 2020 2020 2020 6469 7370 6c61 792e          display.
-0000d550: 7772 6974 6528 7376 675f 7374 7229 0a20  write(svg_str). 
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-0000d580: 6179 2e66 6c75 7368 2829 0a20 2020 2020  ay.flush().     
+0000aec0: 2020 2020 6e6f 6465 5f74 6f74 616c 202b      node_total +
+0000aed0: 3d20 7661 6c75 655b 2274 6f74 616c 225d  = value["total"]
+0000aee0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000aef0: 6e6f 7420 666e 733a 0a20 2020 2020 2020  not fns:.       
+0000af00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000af10: 2830 2c20 302c 2066 6e73 290a 2020 2020  (0, 0, fns).    
+0000af20: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+0000af30: 6e6f 6465 5f74 6f74 616c 2c20 6e6f 6465  node_total, node
+0000af40: 5f74 6f74 616c 202f 206c 656e 2866 6e73  _total / len(fns
+0000af50: 292c 2066 6e73 290a 0a20 2020 2020 2020  ), fns)..       
+0000af60: 2064 6167 5f74 6f74 616c 203d 2030 2e30   dag_total = 0.0
+0000af70: 0a20 2020 2020 2020 2066 6f72 206e 6f64  .        for nod
+0000af80: 6520 696e 206e 6f64 6573 3a0a 2020 2020  e in nodes:.    
+0000af90: 2020 2020 2020 2020 6e6f 6465 5f67 6574          node_get
+0000afa0: 203d 2073 656c 662e 6765 745f 6e6f 6465   = self.get_node
+0000afb0: 286e 6f64 6529 0a20 2020 2020 2020 2020  (node).         
+0000afc0: 2020 206e 6f64 655f 7469 6d65 203d 206e     node_time = n
+0000afd0: 6f64 655f 6765 742e 6765 745f 7469 6d69  ode_get.get_timi
+0000afe0: 6e67 2829 0a20 2020 2020 2020 2020 2020  ng().           
+0000aff0: 206e 6f64 655f 6e61 6d65 203d 206e 6f64   node_name = nod
+0000b000: 655f 6765 742e 6765 745f 6e6f 6465 5f64  e_get.get_node_d
+0000b010: 6566 2829 5b22 6e61 6d65 225d 0a20 2020  ef()["name"].   
+0000b020: 2020 2020 2020 2020 206e 6f64 655f 6964           node_id
+0000b030: 203d 206e 6f64 655f 6765 742e 6765 745f   = node_get.get_
+0000b040: 6964 2829 0a20 2020 2020 2020 2020 2020  id().           
+0000b050: 206e 6f64 655f 746f 7461 6c2c 2061 7667   node_total, avg
+0000b060: 5f74 696d 652c 2066 6e73 203d 2067 6574  _time, fns = get
+0000b070: 5f66 696c 7465 7264 5f74 696d 6573 286e  _filterd_times(n
+0000b080: 6f64 655f 7469 6d65 290a 2020 2020 2020  ode_time).      
+0000b090: 2020 2020 2020 6e6f 6465 5f74 696d 696e        node_timin
+0000b0a0: 675b 6e6f 6465 5f69 645d 203d 207b 0a20  g[node_id] = {. 
+0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000b0c0: 6e6f 6465 5f6e 616d 6522 3a20 6e6f 6465  node_name": node
+0000b0d0: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+0000b0e0: 2020 2020 2020 2022 6e6f 6465 5f74 6f74         "node_tot
+0000b0f0: 616c 223a 206e 6f64 655f 746f 7461 6c2c  al": node_total,
+0000b100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b110: 2022 6e6f 6465 5f61 7667 223a 2061 7667   "node_avg": avg
+0000b120: 5f74 696d 652c 0a20 2020 2020 2020 2020  _time,.         
+0000b130: 2020 2020 2020 2022 666e 7322 3a20 666e         "fns": fn
+0000b140: 732c 0a20 2020 2020 2020 2020 2020 207d  s,.            }
+0000b150: 0a20 2020 2020 2020 2020 2020 2064 6167  .            dag
+0000b160: 5f74 6f74 616c 202b 3d20 6e6f 6465 5f74  _total += node_t
+0000b170: 6f74 616c 0a20 2020 2020 2020 206e 6f64  otal.        nod
+0000b180: 655f 7469 6d69 6e67 5f73 6f72 7465 6420  e_timing_sorted 
+0000b190: 3d20 736f 7274 6564 280a 2020 2020 2020  = sorted(.      
+0000b1a0: 2020 2020 2020 6e6f 6465 5f74 696d 696e        node_timin
+0000b1b0: 672e 6974 656d 7328 292c 0a20 2020 2020  g.items(),.     
+0000b1c0: 2020 2020 2020 206b 6579 3d6c 616d 6264         key=lambd
+0000b1d0: 6120 783a 2078 5b31 5d5b 226e 6f64 655f  a x: x[1]["node_
+0000b1e0: 746f 7461 6c22 5d2c 0a20 2020 2020 2020  total"],.       
+0000b1f0: 2020 2020 2072 6576 6572 7365 3d54 7275       reverse=Tru
+0000b200: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+0000b210: 6e20 7b0a 2020 2020 2020 2020 2020 2020  n {.            
+0000b220: 2264 6167 5f74 6f74 616c 223a 2064 6167  "dag_total": dag
+0000b230: 5f74 6f74 616c 2c0a 2020 2020 2020 2020  _total,.        
+0000b240: 2020 2020 226e 6f64 6573 223a 206e 6f64      "nodes": nod
+0000b250: 655f 7469 6d69 6e67 5f73 6f72 7465 642c  e_timing_sorted,
+0000b260: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+0000b270: 6465 6620 6973 5f68 6967 685f 7072 696f  def is_high_prio
+0000b280: 7269 7479 2873 656c 6629 202d 3e20 626f  rity(self) -> bo
+0000b290: 6f6c 3a0a 2020 2020 2020 2020 7365 6c66  ol:.        self
+0000b2a0: 2e5f 6d61 7962 655f 7265 6672 6573 6828  ._maybe_refresh(
+0000b2b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+0000b2c0: 6d61 7962 655f 6665 7463 6828 290a 2020  maybe_fetch().  
+0000b2d0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+0000b2e0: 662e 5f69 735f 6869 6768 5f70 7269 6f72  f._is_high_prior
+0000b2f0: 6974 7920 6973 206e 6f74 204e 6f6e 650a  ity is not None.
+0000b300: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000b310: 656c 662e 5f69 735f 6869 6768 5f70 7269  elf._is_high_pri
+0000b320: 6f72 6974 790a 0a20 2020 2064 6566 2069  ority..    def i
+0000b330: 735f 7175 6575 6528 7365 6c66 2920 2d3e  s_queue(self) ->
+0000b340: 2062 6f6f 6c3a 0a20 2020 2020 2020 2073   bool:.        s
+0000b350: 656c 662e 5f6d 6179 6265 5f72 6566 7265  elf._maybe_refre
+0000b360: 7368 2829 0a20 2020 2020 2020 2073 656c  sh().        sel
+0000b370: 662e 5f6d 6179 6265 5f66 6574 6368 2829  f._maybe_fetch()
+0000b380: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b390: 7365 6c66 2e5f 7175 6575 655f 6d6e 6720  self._queue_mng 
+0000b3a0: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
+0000b3b0: 2064 6566 2067 6574 5f71 7565 7565 5f6d   def get_queue_m
+0000b3c0: 6e67 2873 656c 6629 202d 3e20 4f70 7469  ng(self) -> Opti
+0000b3d0: 6f6e 616c 5b73 7472 5d3a 0a20 2020 2020  onal[str]:.     
+0000b3e0: 2020 2073 656c 662e 5f6d 6179 6265 5f72     self._maybe_r
+0000b3f0: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
+0000b400: 2073 656c 662e 5f6d 6179 6265 5f66 6574   self._maybe_fet
+0000b410: 6368 2829 0a20 2020 2020 2020 2072 6574  ch().        ret
+0000b420: 7572 6e20 7365 6c66 2e5f 7175 6575 655f  urn self._queue_
+0000b430: 6d6e 670a 0a20 2020 2064 6566 2067 6574  mng..    def get
+0000b440: 5f69 6e73 2873 656c 6629 202d 3e20 4c69  _ins(self) -> Li
+0000b450: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
+0000b460: 2073 656c 662e 5f6d 6179 6265 5f72 6566   self._maybe_ref
+0000b470: 7265 7368 2829 0a20 2020 2020 2020 2073  resh().        s
+0000b480: 656c 662e 5f6d 6179 6265 5f66 6574 6368  elf._maybe_fetch
+0000b490: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
+0000b4a0: 7420 7365 6c66 2e5f 696e 7320 6973 206e  t self._ins is n
+0000b4b0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0000b4c0: 7265 7475 726e 2073 656c 662e 5f69 6e73  return self._ins
+0000b4d0: 0a0a 2020 2020 6465 6620 6765 745f 6f75  ..    def get_ou
+0000b4e0: 7473 2873 656c 6629 202d 3e20 4c69 7374  ts(self) -> List
+0000b4f0: 5b54 7570 6c65 5b73 7472 2c20 7374 725d  [Tuple[str, str]
+0000b500: 5d3a 0a20 2020 2020 2020 2073 656c 662e  ]:.        self.
+0000b510: 5f6d 6179 6265 5f72 6566 7265 7368 2829  _maybe_refresh()
+0000b520: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+0000b530: 6179 6265 5f66 6574 6368 2829 0a20 2020  aybe_fetch().   
+0000b540: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+0000b550: 2e5f 6f75 7473 2069 7320 6e6f 7420 4e6f  ._outs is not No
+0000b560: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+0000b570: 6e20 7365 6c66 2e5f 6f75 7473 0a0a 2020  n self._outs..  
+0000b580: 2020 4063 6f6e 7465 7874 6c69 622e 636f    @contextlib.co
+0000b590: 6e74 6578 746d 616e 6167 6572 0a20 2020  ntextmanager.   
+0000b5a0: 2064 6566 2062 756c 6b5f 6f70 6572 6174   def bulk_operat
+0000b5b0: 696f 6e28 7365 6c66 2920 2d3e 2049 7465  ion(self) -> Ite
+0000b5c0: 7261 746f 725b 626f 6f6c 5d3a 0a20 2020  rator[bool]:.   
+0000b5d0: 2020 2020 2077 6974 6820 7365 6c66 2e5f       with self._
+0000b5e0: 636c 6965 6e74 2e62 756c 6b5f 6f70 6572  client.bulk_oper
+0000b5f0: 6174 696f 6e28 2920 6173 2064 6f5f 7265  ation() as do_re
+0000b600: 6672 6573 683a 0a20 2020 2020 2020 2020  fresh:.         
+0000b610: 2020 2069 6620 646f 5f72 6566 7265 7368     if do_refresh
+0000b620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b630: 2020 7365 6c66 2e72 6566 7265 7368 2829    self.refresh()
+0000b640: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+0000b650: 6c64 2064 6f5f 7265 6672 6573 680a 0a20  ld do_refresh.. 
+0000b660: 2020 2064 6566 2073 6574 5f64 6167 2873     def set_dag(s
+0000b670: 656c 662c 2064 6566 733a 2055 7365 7244  elf, defs: UserD
+0000b680: 6167 4465 6629 202d 3e20 4e6f 6e65 3a0a  agDef) -> None:.
+0000b690: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+0000b6a0: 6965 6e74 2e73 6574 5f64 6167 2873 656c  ient.set_dag(sel
+0000b6b0: 662e 6765 745f 7572 6928 292c 2064 6566  f.get_uri(), def
+0000b6c0: 7329 0a0a 2020 2020 6465 6620 6479 6e61  s)..    def dyna
+0000b6d0: 6d69 635f 6d6f 6465 6c28 0a20 2020 2020  mic_model(.     
+0000b6e0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000b6f0: 2020 2020 2020 2020 2069 6e70 7574 733a           inputs:
+0000b700: 204c 6973 745b 416e 795d 2c0a 2020 2020   List[Any],.    
+0000b710: 2020 2020 2020 2020 666f 726d 6174 5f6d          format_m
+0000b720: 6574 686f 643a 2073 7472 203d 2022 7369  ethod: str = "si
+0000b730: 6d70 6c65 222c 0a20 2020 2020 2020 2020  mple",.         
+0000b740: 2020 206e 6f5f 6361 6368 653a 2062 6f6f     no_cache: boo
+0000b750: 6c20 3d20 4661 6c73 6529 202d 3e20 4c69  l = False) -> Li
+0000b760: 7374 5b41 6e79 5d3a 0a20 2020 2020 2020  st[Any]:.       
+0000b770: 2072 6573 203d 2063 6173 7428 4479 6e61   res = cast(Dyna
+0000b780: 6d69 6352 6573 756c 7473 2c20 7365 6c66  micResults, self
+0000b790: 2e5f 636c 6965 6e74 2e72 6571 7565 7374  ._client.request
+0000b7a0: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
+0000b7b0: 2020 204d 4554 484f 445f 504f 5354 2c20     METHOD_POST, 
+0000b7c0: 222f 6479 6e61 6d69 635f 6d6f 6465 6c22  "/dynamic_model"
+0000b7d0: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
+0000b7e0: 2020 2020 2266 6f72 6d61 7422 3a20 666f      "format": fo
+0000b7f0: 726d 6174 5f6d 6574 686f 642c 0a20 2020  rmat_method,.   
+0000b800: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+0000b810: 7075 7473 223a 2069 6e70 7574 732c 0a20  puts": inputs,. 
+0000b820: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000b830: 6e6f 5f63 6163 6865 223a 206e 6f5f 6361  no_cache": no_ca
+0000b840: 6368 652c 0a20 2020 2020 2020 2020 2020  che,.           
+0000b850: 2020 2020 2022 6461 6722 3a20 7365 6c66       "dag": self
+0000b860: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
+0000b870: 2020 2020 2020 2020 7d29 290a 2020 2020          })).    
+0000b880: 2020 2020 7265 7475 726e 2072 6573 5b22      return res["
+0000b890: 7265 7375 6c74 7322 5d0a 0a20 2020 2064  results"]..    d
+0000b8a0: 6566 205f 6c65 6761 6379 5f64 796e 616d  ef _legacy_dynam
+0000b8b0: 6963 5f6c 6973 7428 0a20 2020 2020 2020  ic_list(.       
+0000b8c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000b8d0: 2020 2020 2020 2069 6e70 7574 733a 204c         inputs: L
+0000b8e0: 6973 745b 416e 795d 2c0a 2020 2020 2020  ist[Any],.      
+0000b8f0: 2020 2020 2020 696e 7075 745f 6b65 793a        input_key:
+0000b900: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000b910: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000b920: 2020 206f 7574 7075 745f 6b65 793a 204f     output_key: O
+0000b930: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000b940: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000b950: 2073 706c 6974 5f74 683a 204f 7074 696f   split_th: Optio
+0000b960: 6e61 6c5b 696e 745d 203d 2031 3030 302c  nal[int] = 1000,
+0000b970: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000b980: 5f74 6872 6561 6473 3a20 696e 7420 3d20  _threads: int = 
+0000b990: 3530 2c0a 2020 2020 2020 2020 2020 2020  50,.            
+0000b9a0: 666f 726d 6174 5f6d 6574 686f 643a 2073  format_method: s
+0000b9b0: 7472 203d 2022 7369 6d70 6c65 222c 0a20  tr = "simple",. 
+0000b9c0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+0000b9d0: 5f6b 6579 733a 2062 6f6f 6c20 3d20 4661  _keys: bool = Fa
+0000b9e0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0000b9f0: 206e 6f5f 6361 6368 653a 2062 6f6f 6c20   no_cache: bool 
+0000ba00: 3d20 4661 6c73 6529 202d 3e20 4c69 7374  = False) -> List
+0000ba10: 5b41 6e79 5d3a 0a20 2020 2020 2020 2069  [Any]:.        i
+0000ba20: 6620 7370 6c69 745f 7468 2069 7320 4e6f  f split_th is No
+0000ba30: 6e65 206f 7220 6c65 6e28 696e 7075 7473  ne or len(inputs
+0000ba40: 2920 3c3d 2073 706c 6974 5f74 683a 0a20  ) <= split_th:. 
+0000ba50: 2020 2020 2020 2020 2020 2072 6573 203d             res =
+0000ba60: 2063 6173 7428 4479 6e61 6d69 6352 6573   cast(DynamicRes
+0000ba70: 756c 7473 2c20 7365 6c66 2e5f 636c 6965  ults, self._clie
+0000ba80: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
+0000ba90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000baa0: 204d 4554 484f 445f 504f 5354 2c20 222f   METHOD_POST, "/
+0000bab0: 6479 6e61 6d69 635f 6c69 7374 222c 207b  dynamic_list", {
+0000bac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bad0: 2020 2020 2022 666f 7263 655f 6b65 7973       "force_keys
+0000bae0: 223a 2066 6f72 6365 5f6b 6579 732c 0a20  ": force_keys,. 
+0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb00: 2020 2022 666f 726d 6174 223a 2066 6f72     "format": for
+0000bb10: 6d61 745f 6d65 7468 6f64 2c0a 2020 2020  mat_method,.    
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2269 6e70 7574 5f6b 6579 223a 2069 6e70  "input_key": inp
+0000bb40: 7574 5f6b 6579 2c0a 2020 2020 2020 2020  ut_key,.        
+0000bb50: 2020 2020 2020 2020 2020 2020 2269 6e70              "inp
+0000bb60: 7574 7322 3a20 696e 7075 7473 2c0a 2020  uts": inputs,.  
+0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb80: 2020 226e 6f5f 6361 6368 6522 3a20 6e6f    "no_cache": no
+0000bb90: 5f63 6163 6865 2c0a 2020 2020 2020 2020  _cache,.        
+0000bba0: 2020 2020 2020 2020 2020 2020 226f 7574              "out
+0000bbb0: 7075 745f 6b65 7922 3a20 6f75 7470 7574  put_key": output
+0000bbc0: 5f6b 6579 2c0a 2020 2020 2020 2020 2020  _key,.          
+0000bbd0: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
+0000bbe0: 2073 656c 662e 6765 745f 7572 6928 292c   self.get_uri(),
+0000bbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc00: 207d 2929 0a20 2020 2020 2020 2020 2020   })).           
+0000bc10: 2072 6574 7572 6e20 7265 735b 2272 6573   return res["res
+0000bc20: 756c 7473 225d 0a20 2020 2020 2020 2023  ults"].        #
+0000bc30: 2046 4958 4d45 3a20 7772 6974 6520 6765   FIXME: write ge
+0000bc40: 6e65 7269 6320 7370 6c69 7465 7261 746f  neric spliterato
+0000bc50: 7220 696d 706c 656d 656e 7461 7469 6f6e  r implementation
+0000bc60: 0a20 2020 2020 2020 2073 706c 6974 5f6e  .        split_n
+0000bc70: 756d 3a20 696e 7420 3d20 7370 6c69 745f  um: int = split_
+0000bc80: 7468 0a20 2020 2020 2020 2061 7373 6572  th.        asser
+0000bc90: 7420 7370 6c69 745f 6e75 6d20 3e20 300a  t split_num > 0.
+0000bca0: 2020 2020 2020 2020 7265 735f 6172 723a          res_arr:
+0000bcb0: 204c 6973 745b 416e 795d 203d 205b 4e6f   List[Any] = [No
+0000bcc0: 6e65 5d20 2a20 6c65 6e28 696e 7075 7473  ne] * len(inputs
+0000bcd0: 290a 2020 2020 2020 2020 6578 633a 204c  ).        exc: L
+0000bce0: 6973 745b 4f70 7469 6f6e 616c 5b42 6173  ist[Optional[Bas
+0000bcf0: 6545 7863 6570 7469 6f6e 5d5d 203d 205b  eException]] = [
+0000bd00: 4e6f 6e65 5d0a 2020 2020 2020 2020 6163  None].        ac
+0000bd10: 7469 7665 5f74 6873 3a20 5365 745b 7468  tive_ths: Set[th
+0000bd20: 7265 6164 696e 672e 5468 7265 6164 5d20  reading.Thread] 
+0000bd30: 3d20 7365 7428 290a 0a20 2020 2020 2020  = set()..       
+0000bd40: 2064 6566 2063 6f6d 7075 7465 5f68 616c   def compute_hal
+0000bd50: 6628 6375 723a 204c 6973 745b 416e 795d  f(cur: List[Any]
+0000bd60: 2c20 6f66 6673 6574 3a20 696e 7429 202d  , offset: int) -
+0000bd70: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000bd80: 2020 2020 6966 2065 7863 5b30 5d20 6973      if exc[0] is
+0000bd90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000bda0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000bdb0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+0000bdc0: 206c 656e 2863 7572 2920 3c3d 2073 706c   len(cur) <= spl
+0000bdd0: 6974 5f6e 756d 3a0a 2020 2020 2020 2020  it_num:.        
+0000bde0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be00: 2063 7572 5f72 6573 203d 2073 656c 662e   cur_res = self.
+0000be10: 5f6c 6567 6163 795f 6479 6e61 6d69 635f  _legacy_dynamic_
+0000be20: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
+0000be30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000be40: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000be50: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000be60: 5f6b 6579 3d69 6e70 7574 5f6b 6579 2c0a  _key=input_key,.
+0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be80: 2020 2020 2020 2020 6f75 7470 7574 5f6b          output_k
+0000be90: 6579 3d6f 7574 7075 745f 6b65 792c 0a20  ey=output_key,. 
+0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000beb0: 2020 2020 2020 2073 706c 6974 5f74 683d         split_th=
+0000bec0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+0000bee0: 785f 7468 7265 6164 733d 6d61 785f 7468  x_threads=max_th
+0000bef0: 7265 6164 732c 0a20 2020 2020 2020 2020  reads,.         
+0000bf00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000bf10: 6f72 6d61 745f 6d65 7468 6f64 3d66 6f72  ormat_method=for
+0000bf20: 6d61 745f 6d65 7468 6f64 2c0a 2020 2020  mat_method,.    
+0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf40: 2020 2020 666f 7263 655f 6b65 7973 3d66      force_keys=f
+0000bf50: 6f72 6365 5f6b 6579 732c 0a20 2020 2020  orce_keys,.     
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 206e 6f5f 6361 6368 653d 6e6f 5f63     no_cache=no_c
+0000bf80: 6163 6865 290a 2020 2020 2020 2020 2020  ache).          
+0000bf90: 2020 2020 2020 2020 2020 7265 735f 6172            res_ar
+0000bfa0: 725b 6f66 6673 6574 3a6f 6666 7365 7420  r[offset:offset 
+0000bfb0: 2b20 6c65 6e28 6375 725f 7265 7329 5d20  + len(cur_res)] 
+0000bfc0: 3d20 6375 725f 7265 730a 2020 2020 2020  = cur_res.      
+0000bfd0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000bfe0: 2042 6173 6545 7863 6570 7469 6f6e 2061   BaseException a
+0000bff0: 7320 653a 2020 2320 7079 6c69 6e74 3a20  s e:  # pylint: 
+0000c000: 6469 7361 626c 653d 6272 6f61 642d 6578  disable=broad-ex
+0000c010: 6365 7074 0a20 2020 2020 2020 2020 2020  cept.           
+0000c020: 2020 2020 2020 2020 2065 7863 5b30 5d20           exc[0] 
+0000c030: 3d20 650a 2020 2020 2020 2020 2020 2020  = e.            
+0000c040: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000c050: 2020 2020 2020 2068 616c 665f 6978 3a20         half_ix: 
+0000c060: 696e 7420 3d20 6c65 6e28 6375 7229 202f  int = len(cur) /
+0000c070: 2f20 320a 2020 2020 2020 2020 2020 2020  / 2.            
+0000c080: 6172 6773 5f66 6972 7374 203d 2028 6375  args_first = (cu
+0000c090: 725b 3a68 616c 665f 6978 5d2c 206f 6666  r[:half_ix], off
+0000c0a0: 7365 7429 0a20 2020 2020 2020 2020 2020  set).           
+0000c0b0: 2061 7267 735f 7365 636f 6e64 203d 2028   args_second = (
+0000c0c0: 6375 725b 6861 6c66 5f69 783a 5d2c 206f  cur[half_ix:], o
+0000c0d0: 6666 7365 7420 2b20 6861 6c66 5f69 7829  ffset + half_ix)
+0000c0e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c0f0: 6c65 6e28 6163 7469 7665 5f74 6873 2920  len(active_ths) 
+0000c100: 3c20 6d61 785f 7468 7265 6164 733a 0a20  < max_threads:. 
+0000c110: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000c120: 6f6d 705f 7468 203d 2074 6872 6561 6469  omp_th = threadi
+0000c130: 6e67 2e54 6872 6561 6428 0a20 2020 2020  ng.Thread(.     
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000c150: 6172 6765 743d 636f 6d70 7574 655f 6861  arget=compute_ha
+0000c160: 6c66 2c20 6172 6773 3d61 7267 735f 6669  lf, args=args_fi
+0000c170: 7273 7429 0a20 2020 2020 2020 2020 2020  rst).           
+0000c180: 2020 2020 2061 6374 6976 655f 7468 732e       active_ths.
+0000c190: 6164 6428 636f 6d70 5f74 6829 0a20 2020  add(comp_th).   
+0000c1a0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+0000c1b0: 705f 7468 2e73 7461 7274 2829 0a20 2020  p_th.start().   
+0000c1c0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+0000c1d0: 7075 7465 5f68 616c 6628 2a61 7267 735f  pute_half(*args_
+0000c1e0: 7365 636f 6e64 290a 2020 2020 2020 2020  second).        
+0000c1f0: 2020 2020 2020 2020 636f 6d70 5f74 682e          comp_th.
+0000c200: 6a6f 696e 2829 0a20 2020 2020 2020 2020  join().         
+0000c210: 2020 2020 2020 2061 6374 6976 655f 7468         active_th
+0000c220: 732e 7265 6d6f 7665 2863 6f6d 705f 7468  s.remove(comp_th
+0000c230: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000c240: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c250: 2020 2020 636f 6d70 7574 655f 6861 6c66      compute_half
+0000c260: 282a 6172 6773 5f66 6972 7374 290a 2020  (*args_first).  
+0000c270: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000c280: 6d70 7574 655f 6861 6c66 282a 6172 6773  mpute_half(*args
+0000c290: 5f73 6563 6f6e 6429 0a0a 2020 2020 2020  _second)..      
+0000c2a0: 2020 636f 6d70 7574 655f 6861 6c66 2869    compute_half(i
+0000c2b0: 6e70 7574 732c 2030 290a 2020 2020 2020  nputs, 0).      
+0000c2c0: 2020 666f 7220 7265 6d61 696e 5f74 6820    for remain_th 
+0000c2d0: 696e 2061 6374 6976 655f 7468 733a 0a20  in active_ths:. 
+0000c2e0: 2020 2020 2020 2020 2020 2072 656d 6169             remai
+0000c2f0: 6e5f 7468 2e6a 6f69 6e28 290a 2020 2020  n_th.join().    
+0000c300: 2020 2020 7261 6973 655f 6520 3d20 6578      raise_e = ex
+0000c310: 635b 305d 0a20 2020 2020 2020 2074 7279  c[0].        try
+0000c320: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000c330: 2069 7369 6e73 7461 6e63 6528 7261 6973   isinstance(rais
+0000c340: 655f 652c 2042 6173 6545 7863 6570 7469  e_e, BaseExcepti
+0000c350: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
+0000c360: 2020 2020 2072 6169 7365 2072 6169 7365       raise raise
+0000c370: 5f65 2020 2320 7079 6c69 6e74 3a20 6469  _e  # pylint: di
+0000c380: 7361 626c 653d 7261 6973 696e 672d 6261  sable=raising-ba
+0000c390: 642d 7479 7065 0a20 2020 2020 2020 2065  d-type.        e
+0000c3a0: 7863 6570 7420 5265 7175 6573 7445 7863  xcept RequestExc
+0000c3b0: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+0000c3c0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000c3d0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+0000c3e0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
+0000c3f0: 6573 7420 6572 726f 7220 7768 696c 6520  est error while 
+0000c400: 7072 6f63 6573 7369 6e67 2e20 7072 6f63  processing. proc
+0000c410: 6573 7369 6e67 2074 696d 6520 7065 7220  essing time per 
+0000c420: 6261 7463 6820 220a 2020 2020 2020 2020  batch ".        
+0000c430: 2020 2020 2020 2020 226d 6967 6874 2062          "might b
+0000c440: 6520 746f 6f20 6c61 7267 652e 2074 7279  e too large. try
+0000c450: 2072 6564 7563 696e 6720 7370 6c69 745f   reducing split_
+0000c460: 7468 2229 2066 726f 6d20 650a 2020 2020  th") from e.    
+0000c470: 2020 2020 7265 7475 726e 2072 6573 5f61      return res_a
+0000c480: 7272 0a0a 2020 2020 6465 6620 6479 6e61  rr..    def dyna
+0000c490: 6d69 635f 6c69 7374 280a 2020 2020 2020  mic_list(.      
+0000c4a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000c4b0: 2020 2020 2020 2020 696e 7075 7473 3a20          inputs: 
+0000c4c0: 4c69 7374 5b41 6e79 5d2c 0a20 2020 2020  List[Any],.     
+0000c4d0: 2020 2020 2020 2069 6e70 7574 5f6b 6579         input_key
+0000c4e0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000c4f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000c500: 2020 2020 6f75 7470 7574 5f6b 6579 3a20      output_key: 
+0000c510: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000c520: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000c530: 2020 7370 6c69 745f 7468 3a20 4f70 7469    split_th: Opti
+0000c540: 6f6e 616c 5b69 6e74 5d20 3d20 3130 3030  onal[int] = 1000
+0000c550: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+0000c560: 785f 7468 7265 6164 733a 2069 6e74 203d  x_threads: int =
+0000c570: 2035 302c 0a20 2020 2020 2020 2020 2020   50,.           
+0000c580: 2066 6f72 6d61 745f 6d65 7468 6f64 3a20   format_method: 
+0000c590: 7374 7220 3d20 2273 696d 706c 6522 2c0a  str = "simple",.
+0000c5a0: 2020 2020 2020 2020 2020 2020 666f 7263              forc
+0000c5b0: 655f 6b65 7973 3a20 626f 6f6c 203d 2046  e_keys: bool = F
+0000c5c0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+0000c5d0: 2020 6e6f 5f63 6163 6865 3a20 626f 6f6c    no_cache: bool
+0000c5e0: 203d 2046 616c 7365 2920 2d3e 204c 6973   = False) -> Lis
+0000c5f0: 745b 416e 795d 3a0a 2020 2020 2020 2020  t[Any]:.        
+0000c600: 6966 2073 656c 662e 5f63 6c69 656e 742e  if self._client.
+0000c610: 5f61 7069 5f76 6572 7369 6f6e 203c 2035  _api_version < 5
+0000c620: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000c630: 7475 726e 2073 656c 662e 5f6c 6567 6163  turn self._legac
+0000c640: 795f 6479 6e61 6d69 635f 6c69 7374 280a  y_dynamic_list(.
+0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c660: 696e 7075 7473 2c0a 2020 2020 2020 2020  inputs,.        
+0000c670: 2020 2020 2020 2020 696e 7075 745f 6b65          input_ke
+0000c680: 793d 696e 7075 745f 6b65 792c 0a20 2020  y=input_key,.   
+0000c690: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0000c6a0: 7075 745f 6b65 793d 6f75 7470 7574 5f6b  put_key=output_k
+0000c6b0: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
+0000c6c0: 2020 2020 7370 6c69 745f 7468 3d4e 6f6e      split_th=Non
+0000c6d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000c6e0: 2020 206d 6178 5f74 6872 6561 6473 3d6d     max_threads=m
+0000c6f0: 6178 5f74 6872 6561 6473 2c0a 2020 2020  ax_threads,.    
+0000c700: 2020 2020 2020 2020 2020 2020 666f 726d              form
+0000c710: 6174 5f6d 6574 686f 643d 666f 726d 6174  at_method=format
+0000c720: 5f6d 6574 686f 642c 0a20 2020 2020 2020  _method,.       
+0000c730: 2020 2020 2020 2020 2066 6f72 6365 5f6b           force_k
+0000c740: 6579 733d 666f 7263 655f 6b65 7973 2c0a  eys=force_keys,.
+0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c760: 6e6f 5f63 6163 6865 3d6e 6f5f 6361 6368  no_cache=no_cach
+0000c770: 6529 0a0a 2020 2020 2020 2020 6966 2073  e)..        if s
+0000c780: 706c 6974 5f74 6820 6973 204e 6f6e 6520  plit_th is None 
+0000c790: 6f72 206c 656e 2869 6e70 7574 7329 203c  or len(inputs) <
+0000c7a0: 3d20 7370 6c69 745f 7468 3a0a 2020 2020  = split_th:.    
+0000c7b0: 2020 2020 2020 2020 7265 7320 3d20 6361          res = ca
+0000c7c0: 7374 2844 796e 616d 6963 5265 7375 6c74  st(DynamicResult
+0000c7d0: 732c 2073 656c 662e 5f63 6c69 656e 742e  s, self._client.
+0000c7e0: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000c800: 5448 4f44 5f50 4f53 542c 2022 2f64 796e  THOD_POST, "/dyn
+0000c810: 616d 6963 5f6c 6973 7422 2c20 7b0a 2020  amic_list", {.  
+0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c830: 2020 2266 6f72 6365 5f6b 6579 7322 3a20    "force_keys": 
+0000c840: 666f 7263 655f 6b65 7973 2c0a 2020 2020  force_keys,.    
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2266 6f72 6d61 7422 3a20 666f 726d 6174  "format": format
+0000c870: 5f6d 6574 686f 642c 0a20 2020 2020 2020  _method,.       
+0000c880: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+0000c890: 7075 745f 6b65 7922 3a20 696e 7075 745f  put_key": input_
+0000c8a0: 6b65 792c 0a20 2020 2020 2020 2020 2020  key,.           
+0000c8b0: 2020 2020 2020 2020 2022 696e 7075 7473           "inputs
+0000c8c0: 223a 2069 6e70 7574 732c 0a20 2020 2020  ": inputs,.     
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c8e0: 6e6f 5f63 6163 6865 223a 206e 6f5f 6361  no_cache": no_ca
+0000c8f0: 6368 652c 0a20 2020 2020 2020 2020 2020  che,.           
+0000c900: 2020 2020 2020 2020 2022 6f75 7470 7574           "output
+0000c910: 5f6b 6579 223a 206f 7574 7075 745f 6b65  _key": output_ke
+0000c920: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+0000c930: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
+0000c940: 6c66 2e67 6574 5f75 7269 2829 2c0a 2020  lf.get_uri(),.  
+0000c950: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+0000c960: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000c970: 7475 726e 2072 6573 5b22 7265 7375 6c74  turn res["result
+0000c980: 7322 5d0a 0a20 2020 2020 2020 2073 706c  s"]..        spl
+0000c990: 6974 5f6e 756d 3a20 696e 7420 3d20 7370  it_num: int = sp
+0000c9a0: 6c69 745f 7468 0a20 2020 2020 2020 2061  lit_th.        a
+0000c9b0: 7373 6572 7420 7370 6c69 745f 6e75 6d20  ssert split_num 
+0000c9c0: 3e20 300a 0a20 2020 2020 2020 2064 6566  > 0..        def
+0000c9d0: 2063 6f6d 7075 7465 5f64 796e 616d 6963   compute_dynamic
+0000c9e0: 5f6c 6973 7428 6375 723a 2069 6e74 2c20  _list(cur: int, 
+0000c9f0: 5f3a 2074 6872 6561 6469 6e67 2e52 4c6f  _: threading.RLo
+0000ca00: 636b 2920 2d3e 2041 6e79 3a0a 2020 2020  ck) -> Any:.    
+0000ca10: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000ca20: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000ca30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000ca40: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000ca50: 7365 6c66 2e64 796e 616d 6963 5f6c 6973  self.dynamic_lis
+0000ca60: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000ca70: 2020 2020 2020 2069 6e70 7574 735b 6375         inputs[cu
+0000ca80: 723a 6375 7220 2b20 7370 6c69 745f 6e75  r:cur + split_nu
+0000ca90: 6d5d 2c0a 2020 2020 2020 2020 2020 2020  m],.            
+0000caa0: 2020 2020 2020 2020 696e 7075 745f 6b65          input_ke
+0000cab0: 793d 696e 7075 745f 6b65 792c 0a20 2020  y=input_key,.   
+0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cad0: 206f 7574 7075 745f 6b65 793d 6f75 7470   output_key=outp
+0000cae0: 7574 5f6b 6579 2c0a 2020 2020 2020 2020  ut_key,.        
+0000caf0: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
+0000cb00: 745f 7468 3d4e 6f6e 652c 0a20 2020 2020  t_th=None,.     
+0000cb10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000cb20: 6178 5f74 6872 6561 6473 3d6d 6178 5f74  ax_threads=max_t
+0000cb30: 6872 6561 6473 2c0a 2020 2020 2020 2020  hreads,.        
+0000cb40: 2020 2020 2020 2020 2020 2020 666f 726d              form
+0000cb50: 6174 5f6d 6574 686f 643d 666f 726d 6174  at_method=format
+0000cb60: 5f6d 6574 686f 642c 0a20 2020 2020 2020  _method,.       
+0000cb70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000cb80: 6365 5f6b 6579 733d 666f 7263 655f 6b65  ce_keys=force_ke
+0000cb90: 7973 2c0a 2020 2020 2020 2020 2020 2020  ys,.            
+0000cba0: 2020 2020 2020 2020 6e6f 5f63 6163 6865          no_cache
+0000cbb0: 3d6e 6f5f 6361 6368 6529 0a20 2020 2020  =no_cache).     
+0000cbc0: 2020 2020 2020 2065 7863 6570 7420 4261         except Ba
+0000cbd0: 7365 4578 6365 7074 696f 6e20 6173 2065  seException as e
+0000cbe0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+0000cbf0: 6162 6c65 3d62 726f 6164 2d65 7863 6570  able=broad-excep
+0000cc00: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000cc10: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000cc20: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000cc30: 696e 7374 616e 6365 2865 2c20 4261 7365  instance(e, Base
+0000cc40: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 2020 2020 7261 6973 6520 650a 2020 2020      raise e.    
+0000cc70: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000cc80: 7074 2052 6571 7565 7374 4578 6365 7074  pt RequestExcept
+0000cc90: 696f 6e20 6173 2065 7272 3a0a 2020 2020  ion as err:.    
+0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccb0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000ccc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000ccd0: 2020 2020 2020 2020 2020 2272 6571 7565            "reque
+0000cce0: 7374 2065 7272 6f72 2077 6869 6c65 2070  st error while p
+0000ccf0: 726f 6365 7373 696e 672e 2229 2066 726f  rocessing.") fro
+0000cd00: 6d20 6572 720a 2020 2020 2020 2020 2020  m err.          
+0000cd10: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0000cd20: 0a20 2020 2020 2020 2074 6173 6b73 203d  .        tasks =
+0000cd30: 206c 6973 7428 7261 6e67 6528 302c 206c   list(range(0, l
+0000cd40: 656e 2869 6e70 7574 7329 2c20 7370 6c69  en(inputs), spli
+0000cd50: 745f 6e75 6d29 290a 2020 2020 2020 2020  t_num)).        
+0000cd60: 6172 7220 3d20 636f 6d70 7574 655f 7061  arr = compute_pa
+0000cd70: 7261 6c6c 656c 280a 2020 2020 2020 2020  rallel(.        
+0000cd80: 2020 2020 7461 736b 732c 2063 6f6d 7075      tasks, compu
+0000cd90: 7465 5f64 796e 616d 6963 5f6c 6973 742c  te_dynamic_list,
+0000cda0: 204e 6f6e 652c 206d 6178 5f74 6872 6561   None, max_threa
+0000cdb0: 6473 290a 2020 2020 2020 2020 7265 7475  ds).        retu
+0000cdc0: 726e 206c 6973 7428 6974 6572 746f 6f6c  rn list(itertool
+0000cdd0: 732e 6368 6169 6e28 2a61 7272 2929 0a0a  s.chain(*arr))..
+0000cde0: 2020 2020 6465 6620 6479 6e61 6d69 6328      def dynamic(
+0000cdf0: 7365 6c66 2c20 696e 7075 745f 6461 7461  self, input_data
+0000ce00: 3a20 4279 7465 7349 4f29 202d 3e20 4f70  : BytesIO) -> Op
+0000ce10: 7469 6f6e 616c 5b42 7974 6552 6573 706f  tional[ByteRespo
+0000ce20: 6e73 655d 3a0a 2020 2020 2020 2020 6375  nse]:.        cu
+0000ce30: 725f 7265 732c 2063 7479 7065 203d 2073  r_res, ctype = s
+0000ce40: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
+0000ce50: 6573 745f 6279 7465 7328 0a20 2020 2020  est_bytes(.     
+0000ce60: 2020 2020 2020 204d 4554 484f 445f 4649         METHOD_FI
+0000ce70: 4c45 2c20 222f 6479 6e61 6d69 6322 2c20  LE, "/dynamic", 
+0000ce80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0000ce90: 2020 2264 6167 223a 2073 656c 662e 6765    "dag": self.ge
+0000cea0: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
+0000ceb0: 2020 2020 207d 2c20 6669 6c65 733d 7b0a       }, files={.
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ced0: 2266 696c 6522 3a20 696e 7075 745f 6461  "file": input_da
+0000cee0: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+0000cef0: 7d29 0a20 2020 2020 2020 2072 6574 7572  }).        retur
+0000cf00: 6e20 696e 7465 7270 7265 745f 6374 7970  n interpret_ctyp
+0000cf10: 6528 6375 725f 7265 732c 2063 7479 7065  e(cur_res, ctype
+0000cf20: 290a 0a20 2020 2064 6566 2064 796e 616d  )..    def dynam
+0000cf30: 6963 5f6f 626a 2873 656c 662c 2069 6e70  ic_obj(self, inp
+0000cf40: 7574 5f6f 626a 3a20 416e 7929 202d 3e20  ut_obj: Any) -> 
+0000cf50: 4f70 7469 6f6e 616c 5b42 7974 6552 6573  Optional[ByteRes
+0000cf60: 706f 6e73 655d 3a0a 2020 2020 2020 2020  ponse]:.        
+0000cf70: 6269 6f20 3d20 4279 7465 7349 4f28 6a73  bio = BytesIO(js
+0000cf80: 6f6e 2e64 756d 7073 280a 2020 2020 2020  on.dumps(.      
+0000cf90: 2020 2020 2020 696e 7075 745f 6f62 6a2c        input_obj,
+0000cfa0: 0a20 2020 2020 2020 2020 2020 2073 6570  .            sep
+0000cfb0: 6172 6174 6f72 733d 2822 2c22 2c20 223a  arators=(",", ":
+0000cfc0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0000cfd0: 696e 6465 6e74 3d4e 6f6e 652c 0a20 2020  indent=None,.   
+0000cfe0: 2020 2020 2020 2020 2073 6f72 745f 6b65           sort_ke
+0000cff0: 7973 3d54 7275 6529 2e65 6e63 6f64 6528  ys=True).encode(
+0000d000: 2275 7466 2d38 2229 290a 2020 2020 2020  "utf-8")).      
+0000d010: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
+0000d020: 6e61 6d69 6328 6269 6f29 0a0a 2020 2020  namic(bio)..    
+0000d030: 6465 6620 6479 6e61 6d69 635f 6173 796e  def dynamic_asyn
+0000d040: 6328 0a20 2020 2020 2020 2020 2020 2073  c(.            s
+0000d050: 656c 662c 2069 6e70 7574 5f64 6174 613a  elf, input_data:
+0000d060: 204c 6973 745b 4279 7465 7349 4f5d 2920   List[BytesIO]) 
+0000d070: 2d3e 204c 6973 745b 2743 6f6d 7075 7461  -> List['Computa
+0000d080: 7469 6f6e 4861 6e64 6c65 275d 3a0a 2020  tionHandle']:.  
+0000d090: 2020 2020 2020 6e61 6d65 7320 3d20 5b66        names = [f
+0000d0a0: 2266 696c 657b 706f 737d 2220 666f 7220  "file{pos}" for 
+0000d0b0: 706f 7320 696e 2072 616e 6765 286c 656e  pos in range(len
+0000d0c0: 2869 6e70 7574 5f64 6174 6129 295d 0a20  (input_data))]. 
+0000d0d0: 2020 2020 2020 2072 6573 3a20 4469 6374         res: Dict
+0000d0e0: 5b73 7472 2c20 7374 725d 203d 2073 656c  [str, str] = sel
+0000d0f0: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+0000d100: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+0000d110: 2020 2020 4d45 5448 4f44 5f46 494c 452c      METHOD_FILE,
+0000d120: 2022 2f64 796e 616d 6963 5f61 7379 6e63   "/dynamic_async
+0000d130: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+0000d140: 2020 2020 2022 6461 6722 3a20 7365 6c66       "dag": self
+0000d150: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
+0000d160: 2020 2020 2020 2020 7d2c 2066 696c 6573          }, files
+0000d170: 3d64 6963 7428 7a69 7028 6e61 6d65 732c  =dict(zip(names,
+0000d180: 2069 6e70 7574 5f64 6174 6129 2929 0a20   input_data))). 
+0000d190: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
+0000d1a0: 2020 2020 2020 2020 2020 2020 436f 6d70              Comp
+0000d1b0: 7574 6174 696f 6e48 616e 646c 6528 0a20  utationHandle(. 
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d1d0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000d1e0: 2020 2020 2072 6573 5b6e 616d 655d 2c0a       res[name],.
+0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d200: 7365 6c66 2e67 6574 5f64 796e 616d 6963  self.get_dynamic
+0000d210: 5f65 7272 6f72 5f6d 6573 7361 6765 2c0a  _error_message,.
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d230: 7365 6c66 2e73 6574 5f64 796e 616d 6963  self.set_dynamic
+0000d240: 5f65 7272 6f72 5f6d 6573 7361 6765 290a  _error_message).
+0000d250: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d260: 6e61 6d65 2069 6e20 6e61 6d65 735d 0a0a  name in names]..
+0000d270: 2020 2020 6465 6620 7365 745f 6479 6e61      def set_dyna
+0000d280: 6d69 635f 6572 726f 725f 6d65 7373 6167  mic_error_messag
+0000d290: 6528 7365 6c66 2c20 6d73 673a 204f 7074  e(self, msg: Opt
+0000d2a0: 696f 6e61 6c5b 7374 725d 2920 2d3e 204e  ional[str]) -> N
+0000d2b0: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
+0000d2c0: 662e 5f64 796e 616d 6963 5f65 7272 6f72  f._dynamic_error
+0000d2d0: 203d 206d 7367 0a0a 2020 2020 6465 6620   = msg..    def 
+0000d2e0: 6765 745f 6479 6e61 6d69 635f 6572 726f  get_dynamic_erro
+0000d2f0: 725f 6d65 7373 6167 6528 7365 6c66 2920  r_message(self) 
+0000d300: 2d3e 204f 7074 696f 6e61 6c5b 7374 725d  -> Optional[str]
+0000d310: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000d320: 2073 656c 662e 5f64 796e 616d 6963 5f65   self._dynamic_e
+0000d330: 7272 6f72 0a0a 2020 2020 6465 6620 6479  rror..    def dy
+0000d340: 6e61 6d69 635f 6173 796e 635f 6f62 6a28  namic_async_obj(
+0000d350: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d360: 662c 2069 6e70 7574 5f64 6174 613a 204c  f, input_data: L
+0000d370: 6973 745b 416e 795d 2920 2d3e 204c 6973  ist[Any]) -> Lis
+0000d380: 745b 2743 6f6d 7075 7461 7469 6f6e 4861  t['ComputationHa
+0000d390: 6e64 6c65 275d 3a0a 2020 2020 2020 2020  ndle']:.        
+0000d3a0: 7265 7475 726e 2073 656c 662e 6479 6e61  return self.dyna
+0000d3b0: 6d69 635f 6173 796e 6328 5b0a 2020 2020  mic_async([.    
+0000d3c0: 2020 2020 2020 2020 4279 7465 7349 4f28          BytesIO(
+0000d3d0: 6a73 6f6e 2e64 756d 7073 280a 2020 2020  json.dumps(.    
+0000d3e0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+0000d3f0: 745f 6f62 6a2c 0a20 2020 2020 2020 2020  t_obj,.         
+0000d400: 2020 2020 2020 2073 6570 6172 6174 6f72         separator
+0000d410: 733d 2822 2c22 2c20 223a 2229 2c0a 2020  s=(",", ":"),.  
+0000d420: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000d430: 6465 6e74 3d4e 6f6e 652c 0a20 2020 2020  dent=None,.     
+0000d440: 2020 2020 2020 2020 2020 2073 6f72 745f             sort_
+0000d450: 6b65 7973 3d54 7275 6529 2e65 6e63 6f64  keys=True).encod
+0000d460: 6528 2275 7466 2d38 2229 290a 2020 2020  e("utf-8")).    
+0000d470: 2020 2020 2020 2020 666f 7220 696e 7075          for inpu
+0000d480: 745f 6f62 6a20 696e 2069 6e70 7574 5f64  t_obj in input_d
+0000d490: 6174 610a 2020 2020 2020 2020 5d29 0a0a  ata.        ])..
+0000d4a0: 2020 2020 6465 6620 6765 745f 6479 6e61      def get_dyna
+0000d4b0: 6d69 635f 7265 7375 6c74 2873 656c 662c  mic_result(self,
+0000d4c0: 2076 616c 7565 5f69 643a 2073 7472 2920   value_id: str) 
+0000d4d0: 2d3e 204f 7074 696f 6e61 6c5b 4279 7465  -> Optional[Byte
+0000d4e0: 5265 7370 6f6e 7365 5d3a 0a20 2020 2020  Response]:.     
+0000d4f0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000d500: 2020 2020 6375 725f 7265 732c 2063 7479      cur_res, cty
+0000d510: 7065 203d 2073 656c 662e 5f63 6c69 656e  pe = self._clien
+0000d520: 742e 7265 7175 6573 745f 6279 7465 7328  t.request_bytes(
+0000d530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d540: 204d 4554 484f 445f 4745 542c 2022 2f64   METHOD_GET, "/d
+0000d550: 796e 616d 6963 5f72 6573 756c 7422 2c20  ynamic_result", 
+0000d560: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0000d570: 2020 2020 2020 2264 6167 223a 2073 656c        "dag": sel
+0000d580: 662e 6765 745f 7572 6928 292c 0a20 2020  f.get_uri(),.   
 0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5c0: 2020 2020 2066 726f 6d20 4950 7974 686f       from IPytho
-0000d5d0: 6e2e 6469 7370 6c61 7920 696d 706f 7274  n.display import
-0000d5e0: 2064 6973 706c 6179 2061 7320 6964 6973   display as idis
-0000d5f0: 706c 6179 0a20 2020 2020 2020 2020 2020  play.           
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 2066 726f 6d20 4950 7974 686f 6e2e 6469   from IPython.di
-0000d620: 7370 6c61 7920 696d 706f 7274 2053 5647  splay import SVG
-0000d630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d640: 2020 2020 2020 2020 2020 2020 2069 6469               idi
-0000d650: 7370 6c61 7928 5356 4728 7376 675f 7374  splay(SVG(svg_st
-0000d660: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
-0000d670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d680: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-0000d690: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d6a0: 726e 2073 7667 5f73 7472 0a20 2020 2020  rn svg_str.     
-0000d6b0: 2020 2020 2020 2020 2020 2069 6620 6f75             if ou
-0000d6c0: 7470 7574 5f66 6f72 6d61 7420 3d3d 2022  tput_format == "
-0000d6d0: 706e 6722 3a0a 2020 2020 2020 2020 2020  png":.          
-0000d6e0: 2020 2020 2020 2020 2020 6772 6170 6820            graph 
-0000d6f0: 3d20 536f 7572 6365 2867 7261 7068 5f73  = Source(graph_s
-0000d700: 7472 290a 2020 2020 2020 2020 2020 2020  tr).            
-0000d710: 2020 2020 2020 2020 706e 675f 7374 7220          png_str 
-0000d720: 3d20 6772 6170 682e 7069 7065 2866 6f72  = graph.pipe(for
-0000d730: 6d61 743d 2270 6e67 2229 0a20 2020 2020  mat="png").     
-0000d740: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d750: 6620 6469 7370 6c61 7920 6973 206e 6f74  f display is not
-0000d760: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d780: 6620 6e6f 7420 6973 5f6a 7570 7974 6572  f not is_jupyter
-0000d790: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7b0: 6469 7370 6c61 792e 7772 6974 6528 0a20  display.write(. 
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000d7e0: 5761 726e 696e 673a 2049 7079 7468 6f6e  Warning: Ipython
-0000d7f0: 2069 6e73 7461 6e63 6520 6e6f 7420 666f   instance not fo
-0000d800: 756e 642e 5c6e 2229 0a20 2020 2020 2020  und.\n").       
-0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2020 2020 2064 6973 706c 6179 2e77 7269       display.wri
-0000d830: 7465 2870 6e67 5f73 7472 290a 2020 2020  te(png_str).    
-0000d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d850: 2020 2020 2020 2020 6469 7370 6c61 792e          display.
-0000d860: 666c 7573 6828 290a 2020 2020 2020 2020  flush().        
-0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d880: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2020 6672 6f6d 2049 5079 7468 6f6e 2e64    from IPython.d
-0000d8b0: 6973 706c 6179 2069 6d70 6f72 7420 6469  isplay import di
-0000d8c0: 7370 6c61 7920 6173 2069 6469 7370 6c61  splay as idispla
-0000d8d0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-0000d8f0: 6f6d 2049 5079 7468 6f6e 2e64 6973 706c  om IPython.displ
-0000d900: 6179 2069 6d70 6f72 7420 496d 6167 650a  ay import Image.
-0000d910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d920: 2020 2020 2020 2020 2020 2020 2069 6469               idi
-0000d930: 7370 6c61 7928 496d 6167 6528 706e 675f  splay(Image(png_
-0000d940: 7374 7229 290a 2020 2020 2020 2020 2020  str)).          
-0000d950: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000d960: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-0000d970: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000d980: 7475 726e 2070 6e67 5f73 7472 0a20 2020  turn png_str.   
-0000d990: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d9a0: 6f75 7470 7574 5f66 6f72 6d61 7420 3d3d  output_format ==
-0000d9b0: 2022 6173 6369 6922 3a0a 2020 2020 2020   "ascii":.      
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000d9d0: 206e 6f74 2068 6173 5f67 7261 7068 5f65   not has_graph_e
-0000d9e0: 6173 7928 293a 0a20 2020 2020 2020 2020  asy():.         
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000da00: 6574 7572 6e20 7265 6e64 6572 2867 7261  eturn render(gra
-0000da10: 7068 5f73 7472 290a 0a20 2020 2020 2020  ph_str)..       
-0000da20: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
-0000da30: 6f72 7420 7375 6270 726f 6365 7373 0a20  ort subprocess. 
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2063 6d64 203d 205b 2265 6368 6f22     cmd = ["echo"
-0000da60: 2c20 6772 6170 685f 7374 725d 0a20 2020  , graph_str].   
-0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2077 6974 6820 7375 6270 726f 6365 7373   with subprocess
-0000da90: 2e50 6f70 656e 2863 6d64 2c20 7374 646f  .Popen(cmd, stdo
-0000daa0: 7574 3d73 7562 7072 6f63 6573 732e 5049  ut=subprocess.PI
-0000dab0: 5045 2920 6173 2070 313a 0a20 2020 2020  PE) as p1:.     
-0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 2020 2070 3220 3d20 7375 6270 726f 6365     p2 = subproce
-0000dae0: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-0000daf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000db00: 2020 2020 2020 2020 2020 2020 205b 2267               ["g
-0000db10: 7261 7068 2d65 6173 7922 5d2c 2073 7464  raph-easy"], std
-0000db20: 696e 3d70 312e 7374 646f 7574 290a 2020  in=p1.stdout).  
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 2020 2020 7265 7320 3d20 7032 2e64        res = p2.d
-0000db50: 6563 6f64 6528 2275 7466 2d38 2229 0a20  ecode("utf-8"). 
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2020 2072 6574 7572 6e20 7265 6e64 6572     return render
-0000db80: 2872 6573 290a 2020 2020 2020 2020 2020  (res).          
-0000db90: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000dba0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-0000dbb0: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
-0000dbc0: 7661 6c69 6420 666f 726d 6174 207b 6f75  valid format {ou
-0000dbd0: 7470 7574 5f66 6f72 6d61 747d 2c20 220a  tput_format}, ".
-0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 2020 2275 7365 2073 7667 2c20 706e      "use svg, pn
-0000dc00: 672c 2061 7363 6969 2c20 6f72 2064 6f74  g, ascii, or dot
-0000dc10: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0000dc20: 7863 6570 7420 4578 6563 7574 6162 6c65  xcept Executable
-0000dc30: 4e6f 7446 6f75 6e64 2061 7320 653a 0a20  NotFound as e:. 
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000dc50: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-0000dc60: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000dc70: 2020 2020 2020 2022 7573 6520 2762 7265         "use 'bre
-0000dc80: 7720 696e 7374 616c 6c20 6772 6170 6876  w install graphv
-0000dc90: 697a 2720 6f72 2075 7365 2027 6d65 7468  iz' or use 'meth
-0000dca0: 6f64 3d61 6363 6572 6e27 222c 0a20 2020  od=accern'",.   
-0000dcb0: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
-0000dcc0: 726f 6d20 650a 2020 2020 2020 2020 7261  rom e.        ra
-0000dcd0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-0000dce0: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
-0000dcf0: 7661 6c69 6420 6d65 7468 6f64 207b 6d65  valid method {me
-0000dd00: 7468 6f64 7d2c 2075 7365 2061 6363 6572  thod}, use accer
-0000dd10: 6e20 6f72 2064 6f74 2229 0a0a 2020 2020  n or dot")..    
-0000dd20: 6465 6620 7072 6574 7479 5f6f 626a 280a  def pretty_obj(.
-0000dd30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dd40: 2c0a 2020 2020 2020 2020 2020 2020 6e6f  ,.            no
-0000dd50: 6465 735f 6f6e 6c79 3a20 626f 6f6c 203d  des_only: bool =
-0000dd60: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-0000dd70: 2020 2020 616c 6c6f 775f 756e 6963 6f64      allow_unicod
-0000dd80: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0a  e: bool = True,.
-0000dd90: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
-0000dda0: 6473 3a20 4f70 7469 6f6e 616c 5b4c 6973  ds: Optional[Lis
-0000ddb0: 745b 7374 725d 5d20 3d20 4e6f 6e65 2920  t[str]] = None) 
-0000ddc0: 2d3e 204c 6973 745b 4461 6750 7265 7474  -> List[DagPrett
-0000ddd0: 794e 6f64 655d 3a0a 2020 2020 2020 2020  yNode]:.        
-0000dde0: 7265 7475 726e 2073 656c 662e 5f70 7265  return self._pre
-0000ddf0: 7474 7928 0a20 2020 2020 2020 2020 2020  tty(.           
-0000de00: 206e 6f64 6573 5f6f 6e6c 793d 6e6f 6465   nodes_only=node
-0000de10: 735f 6f6e 6c79 2c0a 2020 2020 2020 2020  s_only,.        
-0000de20: 2020 2020 616c 6c6f 775f 756e 6963 6f64      allow_unicod
-0000de30: 653d 616c 6c6f 775f 756e 6963 6f64 652c  e=allow_unicode,
-0000de40: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
-0000de50: 6c64 733d 6669 656c 6473 295b 226e 6f64  lds=fields)["nod
-0000de60: 6573 225d 0a0a 2020 2020 6465 6620 6765  es"]..    def ge
-0000de70: 745f 6465 6628 7365 6c66 2c20 6675 6c6c  t_def(self, full
-0000de80: 3a20 626f 6f6c 203d 2054 7275 6529 202d  : bool = True) -
-0000de90: 3e20 4461 6744 6566 3a0a 2020 2020 2020  > DagDef:.      
-0000dea0: 2020 7265 7475 726e 2063 6173 7428 4461    return cast(Da
-0000deb0: 6744 6566 2c20 7365 6c66 2e5f 636c 6965  gDef, self._clie
-0000dec0: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-0000ded0: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-0000dee0: 484f 445f 4745 542c 2022 2f64 6167 5f64  HOD_GET, "/dag_d
-0000def0: 6566 222c 207b 0a20 2020 2020 2020 2020  ef", {.         
-0000df00: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
-0000df10: 6c66 2e67 6574 5f75 7269 2829 2c0a 2020  lf.get_uri(),.  
-0000df20: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-0000df30: 756c 6c22 3a20 6675 6c6c 2c0a 2020 2020  ull": full,.    
-0000df40: 2020 2020 2020 2020 7d29 290a 0a20 2020          }))..   
-0000df50: 2064 6566 2073 6574 5f61 7474 7228 7365   def set_attr(se
-0000df60: 6c66 2c20 6174 7472 3a20 7374 722c 2076  lf, attr: str, v
-0000df70: 616c 7565 3a20 416e 7929 202d 3e20 4e6f  alue: Any) -> No
-0000df80: 6e65 3a0a 2020 2020 2020 2020 6461 675f  ne:.        dag_
-0000df90: 6465 6620 3d20 7365 6c66 2e67 6574 5f64  def = self.get_d
-0000dfa0: 6566 2829 0a20 2020 2020 2020 2064 6167  ef().        dag
-0000dfb0: 5f64 6566 5b61 7474 725d 203d 2076 616c  _def[attr] = val
-0000dfc0: 7565 2020 2320 7479 7065 3a20 6967 6e6f  ue  # type: igno
-0000dfd0: 7265 0a20 2020 2020 2020 2073 656c 662e  re.        self.
-0000dfe0: 5f63 6c69 656e 742e 7365 745f 6461 6728  _client.set_dag(
-0000dff0: 7365 6c66 2e67 6574 5f75 7269 2829 2c20  self.get_uri(), 
-0000e000: 6461 675f 6465 6629 0a0a 2020 2020 6465  dag_def)..    de
-0000e010: 6620 7365 745f 6e61 6d65 2873 656c 662c  f set_name(self,
-0000e020: 2076 616c 7565 3a20 7374 7229 202d 3e20   value: str) -> 
-0000e030: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
-0000e040: 6c66 2e73 6574 5f61 7474 7228 226e 616d  lf.set_attr("nam
-0000e050: 6522 2c20 7661 6c75 6529 0a0a 2020 2020  e", value)..    
-0000e060: 6465 6620 7365 745f 636f 6d70 616e 7928  def set_company(
-0000e070: 7365 6c66 2c20 7661 6c75 653a 2073 7472  self, value: str
-0000e080: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000e090: 2020 2073 656c 662e 7365 745f 6174 7472     self.set_attr
-0000e0a0: 2822 636f 6d70 616e 7922 2c20 7661 6c75  ("company", valu
-0000e0b0: 6529 0a0a 2020 2020 6465 6620 7365 745f  e)..    def set_
-0000e0c0: 7374 6174 655f 7572 6928 7365 6c66 2c20  state_uri(self, 
-0000e0d0: 7661 6c75 653a 2073 7472 2920 2d3e 204e  value: str) -> N
-0000e0e0: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
-0000e0f0: 662e 7365 745f 6174 7472 2822 7374 6174  f.set_attr("stat
-0000e100: 655f 7572 6922 2c20 7661 6c75 6529 0a0a  e_uri", value)..
-0000e110: 2020 2020 6465 6620 7365 745f 7572 695f      def set_uri_
-0000e120: 7072 6566 6978 2873 656c 662c 2076 616c  prefix(self, val
-0000e130: 7565 3a20 5552 4950 7265 6669 7829 202d  ue: URIPrefix) -
-0000e140: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000e150: 7365 6c66 2e73 6574 5f61 7474 7228 2275  self.set_attr("u
-0000e160: 7269 5f70 7265 6669 7822 2c20 7661 6c75  ri_prefix", valu
-0000e170: 6529 0a0a 2020 2020 6465 6620 7365 745f  e)..    def set_
-0000e180: 6869 6768 5f70 7269 6f72 6974 7928 7365  high_priority(se
-0000e190: 6c66 2c20 7661 6c75 653a 2062 6f6f 6c29  lf, value: bool)
-0000e1a0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000e1b0: 2020 7365 6c66 2e73 6574 5f61 7474 7228    self.set_attr(
-0000e1c0: 2268 6967 685f 7072 696f 7269 7479 222c  "high_priority",
-0000e1d0: 2076 616c 7565 290a 0a20 2020 2064 6566   value)..    def
-0000e1e0: 2073 6574 5f71 7565 7565 5f6d 6e67 2873   set_queue_mng(s
-0000e1f0: 656c 662c 2076 616c 7565 3a20 4f70 7469  elf, value: Opti
-0000e200: 6f6e 616c 5b73 7472 5d29 202d 3e20 4e6f  onal[str]) -> No
-0000e210: 6e65 3a0a 2020 2020 2020 2020 7365 6c66  ne:.        self
-0000e220: 2e73 6574 5f61 7474 7228 2271 7565 7565  .set_attr("queue
-0000e230: 5f6d 6e67 222c 2076 616c 7565 290a 0a20  _mng", value).. 
-0000e240: 2020 2064 6566 2073 6574 5f76 6572 7369     def set_versi
-0000e250: 6f6e 5f6f 7665 7272 6964 6528 7365 6c66  on_override(self
-0000e260: 2c20 7661 6c75 653a 204f 7074 696f 6e61  , value: Optiona
-0000e270: 6c5b 7374 725d 2920 2d3e 204e 6f6e 653a  l[str]) -> None:
-0000e280: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000e290: 745f 6174 7472 2822 7665 7273 696f 6e5f  t_attr("version_
-0000e2a0: 6f76 6572 7269 6465 222c 2076 616c 7565  override", value
-0000e2b0: 290a 0a20 2020 2040 6f76 6572 6c6f 6164  )..    @overload
-0000e2c0: 0a20 2020 2064 6566 2063 6865 636b 5f71  .    def check_q
-0000e2d0: 7565 7565 5f73 7461 7473 2820 2023 2070  ueue_stats(  # p
-0000e2e0: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-0000e2f0: 6f2d 7365 6c66 2d75 7365 0a20 2020 2020  o-self-use.     
-0000e300: 2020 2020 2020 2073 656c 662c 206d 696e         self, min
-0000e310: 696d 616c 3a20 4c69 7465 7261 6c5b 5472  imal: Literal[Tr
-0000e320: 7565 5d29 202d 3e20 4d69 6e69 6d61 6c51  ue]) -> MinimalQ
-0000e330: 7565 7565 5374 6174 7352 6573 706f 6e73  ueueStatsRespons
-0000e340: 653a 0a20 2020 2020 2020 202e 2e2e 0a0a  e:.        .....
-0000e350: 2020 2020 406f 7665 726c 6f61 640a 2020      @overload.  
-0000e360: 2020 6465 6620 6368 6563 6b5f 7175 6575    def check_queu
-0000e370: 655f 7374 6174 7328 2020 2320 7079 6c69  e_stats(  # pyli
-0000e380: 6e74 3a20 6469 7361 626c 653d 6e6f 2d73  nt: disable=no-s
-0000e390: 656c 662d 7573 650a 2020 2020 2020 2020  elf-use.        
-0000e3a0: 2020 2020 7365 6c66 2c20 6d69 6e69 6d61      self, minima
-0000e3b0: 6c3a 204c 6974 6572 616c 5b46 616c 7365  l: Literal[False
-0000e3c0: 5d29 202d 3e20 5175 6575 6553 7461 7473  ]) -> QueueStats
-0000e3d0: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-0000e3e0: 2020 2e2e 2e0a 0a20 2020 2040 6f76 6572    .....    @over
-0000e3f0: 6c6f 6164 0a20 2020 2064 6566 2063 6865  load.    def che
-0000e400: 636b 5f71 7565 7565 5f73 7461 7473 2820  ck_queue_stats( 
-0000e410: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-0000e420: 6c65 3d6e 6f2d 7365 6c66 2d75 7365 0a20  le=no-self-use. 
-0000e430: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-0000e440: 206d 696e 696d 616c 3a20 626f 6f6c 2920   minimal: bool) 
-0000e450: 2d3e 2055 6e69 6f6e 5b0a 2020 2020 2020  -> Union[.      
-0000e460: 2020 2020 2020 2020 2020 4d69 6e69 6d61            Minima
-0000e470: 6c51 7565 7565 5374 6174 7352 6573 706f  lQueueStatsRespo
-0000e480: 6e73 652c 2051 7565 7565 5374 6174 7352  nse, QueueStatsR
-0000e490: 6573 706f 6e73 655d 3a0a 2020 2020 2020  esponse]:.      
-0000e4a0: 2020 2e2e 2e0a 0a20 2020 2064 6566 2063    .....    def c
-0000e4b0: 6865 636b 5f71 7565 7565 5f73 7461 7473  heck_queue_stats
-0000e4c0: 2873 656c 662c 206d 696e 696d 616c 3a20  (self, minimal: 
-0000e4d0: 626f 6f6c 2920 2d3e 2055 6e69 6f6e 5b0a  bool) -> Union[.
-0000e4e0: 2020 2020 2020 2020 2020 2020 4d69 6e69              Mini
-0000e4f0: 6d61 6c51 7565 7565 5374 6174 7352 6573  malQueueStatsRes
-0000e500: 706f 6e73 652c 2051 7565 7565 5374 6174  ponse, QueueStat
-0000e510: 7352 6573 706f 6e73 655d 3a0a 2020 2020  sResponse]:.    
-0000e520: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e530: 5f63 6c69 656e 742e 6368 6563 6b5f 7175  _client.check_qu
-0000e540: 6575 655f 7374 6174 7328 7365 6c66 2e67  eue_stats(self.g
-0000e550: 6574 5f75 7269 2829 2c20 6d69 6e69 6d61  et_uri(), minima
-0000e560: 6c3d 6d69 6e69 6d61 6c29 0a0a 2020 2020  l=minimal)..    
-0000e570: 6465 6620 7363 616c 655f 776f 726b 6572  def scale_worker
-0000e580: 2873 656c 662c 2072 6570 6c69 6361 733a  (self, replicas:
-0000e590: 2069 6e74 2920 2d3e 2069 6e74 3a0a 2020   int) -> int:.  
-0000e5a0: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
-0000e5b0: 7428 576f 726b 6572 5363 616c 652c 2073  t(WorkerScale, s
-0000e5c0: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
-0000e5d0: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-0000e5e0: 2020 2020 2020 4d45 5448 4f44 5f50 5554        METHOD_PUT
-0000e5f0: 2c20 222f 776f 726b 6572 222c 207b 0a20  , "/worker", {. 
-0000e600: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e610: 6461 6722 3a20 7365 6c66 2e67 6574 5f75  dag": self.get_u
-0000e620: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
-0000e630: 2020 2020 2020 2272 6570 6c69 6361 7322        "replicas"
-0000e640: 3a20 7265 706c 6963 6173 2c0a 2020 2020  : replicas,.    
-0000e650: 2020 2020 2020 2020 2020 2020 2274 6173              "tas
-0000e660: 6b22 3a20 4e6f 6e65 2c0a 2020 2020 2020  k": None,.      
-0000e670: 2020 2020 2020 7d29 295b 226e 756d 5f72        }))["num_r
-0000e680: 6570 6c69 6361 7322 5d0a 0a20 2020 2064  eplicas"]..    d
-0000e690: 6566 2072 656c 6f61 6428 7365 6c66 2c20  ef reload(self, 
-0000e6a0: 7469 6d65 7374 616d 703a 204f 7074 696f  timestamp: Optio
-0000e6b0: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
-0000e6c0: 6529 202d 3e20 666c 6f61 743a 0a20 2020  e) -> float:.   
-0000e6d0: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
-0000e6e0: 2844 6167 5265 6c6f 6164 2c20 7365 6c66  (DagReload, self
-0000e6f0: 2e5f 636c 6965 6e74 2e72 6571 7565 7374  ._client.request
-0000e700: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
-0000e710: 2020 204d 4554 484f 445f 5055 542c 2022     METHOD_PUT, "
-0000e720: 2f64 6167 5f72 656c 6f61 6422 2c20 7b0a  /dag_reload", {.
-0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2264 6167 223a 2073 656c 662e 6765 745f  "dag": self.get_
-0000e750: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
-0000e760: 2020 2020 2020 2022 7768 656e 223a 2074         "when": t
-0000e770: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
-0000e780: 2020 2020 2020 7d29 295b 2277 6865 6e22        }))["when"
-0000e790: 5d0a 0a20 2020 2064 6566 2067 6574 5f6b  ]..    def get_k
-0000e7a0: 6166 6b61 5f69 6e70 7574 5f74 6f70 6963  afka_input_topic
-0000e7b0: 2873 656c 662c 2070 6f73 7466 6978 3a20  (self, postfix: 
-0000e7c0: 7374 7220 3d20 2222 2920 2d3e 2073 7472  str = "") -> str
-0000e7d0: 3a0a 2020 2020 2020 2020 7265 7320 3d20  :.        res = 
-0000e7e0: 6361 7374 284b 6166 6b61 546f 7069 634e  cast(KafkaTopicN
-0000e7f0: 616d 6573 2c20 7365 6c66 2e5f 636c 6965  ames, self._clie
-0000e800: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-0000e810: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-0000e820: 484f 445f 4745 542c 2022 2f6b 6166 6b61  HOD_GET, "/kafka
-0000e830: 5f74 6f70 6963 5f6e 616d 6573 222c 207b  _topic_names", {
-0000e840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e850: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
-0000e860: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
-0000e870: 2020 2020 2020 2020 2270 6f73 7466 6978          "postfix
-0000e880: 223a 2070 6f73 7466 6978 2c0a 2020 2020  ": postfix,.    
-0000e890: 2020 2020 2020 2020 2020 2020 226e 6f5f              "no_
-0000e8a0: 6f75 7470 7574 223a 2054 7275 652c 0a20  output": True,. 
-0000e8b0: 2020 2020 2020 2020 2020 207d 2929 5b22             }))["
-0000e8c0: 696e 7075 7422 5d0a 2020 2020 2020 2020  input"].        
-0000e8d0: 6173 7365 7274 2072 6573 2069 7320 6e6f  assert res is no
-0000e8e0: 7420 4e6f 6e65 0a20 2020 2020 2020 2072  t None.        r
-0000e8f0: 6574 7572 6e20 7265 730a 0a20 2020 2064  eturn res..    d
-0000e900: 6566 2067 6574 5f6b 6166 6b61 5f6f 7574  ef get_kafka_out
-0000e910: 7075 745f 746f 7069 6328 7365 6c66 2920  put_topic(self) 
-0000e920: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0000e930: 7265 7320 3d20 6361 7374 284b 6166 6b61  res = cast(Kafka
-0000e940: 546f 7069 634e 616d 6573 2c20 7365 6c66  TopicNames, self
-0000e950: 2e5f 636c 6965 6e74 2e72 6571 7565 7374  ._client.request
-0000e960: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
-0000e970: 2020 204d 4554 484f 445f 4745 542c 2022     METHOD_GET, "
-0000e980: 2f6b 6166 6b61 5f74 6f70 6963 5f6e 616d  /kafka_topic_nam
-0000e990: 6573 222c 207b 0a20 2020 2020 2020 2020  es", {.         
-0000e9a0: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
-0000e9b0: 6c66 2e67 6574 5f75 7269 2829 2c0a 2020  lf.get_uri(),.  
-0000e9c0: 2020 2020 2020 2020 2020 7d29 295b 226f            }))["o
-0000e9d0: 7574 7075 7422 5d0a 2020 2020 2020 2020  utput"].        
-0000e9e0: 6173 7365 7274 2072 6573 2069 7320 6e6f  assert res is no
-0000e9f0: 7420 4e6f 6e65 0a20 2020 2020 2020 2072  t None.        r
-0000ea00: 6574 7572 6e20 7265 730a 0a20 2020 2064  eturn res..    d
-0000ea10: 6566 2073 6574 5f6b 6166 6b61 5f74 6f70  ef set_kafka_top
-0000ea20: 6963 5f70 6172 7469 7469 6f6e 7328 0a20  ic_partitions(. 
-0000ea30: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-0000ea40: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-0000ea50: 5f70 6172 7469 7469 6f6e 733a 2069 6e74  _partitions: int
-0000ea60: 2c0a 2020 2020 2020 2020 2020 2020 706f  ,.            po
-0000ea70: 7374 6669 783a 2073 7472 203d 2022 222c  stfix: str = "",
-0000ea80: 0a20 2020 2020 2020 2020 2020 206c 6172  .            lar
-0000ea90: 6765 5f69 6e70 7574 5f72 6574 656e 7469  ge_input_retenti
-0000eaa0: 6f6e 3a20 626f 6f6c 203d 2046 616c 7365  on: bool = False
-0000eab0: 2c0a 2020 2020 2020 2020 2020 2020 6e6f  ,.            no
-0000eac0: 5f6f 7574 7075 743a 2062 6f6f 6c20 3d20  _output: bool = 
-0000ead0: 4661 6c73 6529 202d 3e20 4b61 666b 6154  False) -> KafkaT
-0000eae0: 6f70 6963 733a 0a20 2020 2020 2020 2072  opics:.        r
-0000eaf0: 6574 7572 6e20 6361 7374 284b 6166 6b61  eturn cast(Kafka
-0000eb00: 546f 7069 6373 2c20 7365 6c66 2e5f 636c  Topics, self._cl
-0000eb10: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
-0000eb20: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-0000eb30: 4554 484f 445f 504f 5354 2c20 222f 6b61  ETHOD_POST, "/ka
-0000eb40: 666b 615f 746f 7069 6373 222c 207b 0a20  fka_topics", {. 
-0000eb50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000eb60: 6461 6722 3a20 7365 6c66 2e67 6574 5f75  dag": self.get_u
-0000eb70: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
-0000eb80: 2020 2020 2020 226e 756d 5f70 6172 7469        "num_parti
-0000eb90: 7469 6f6e 7322 3a20 6e75 6d5f 7061 7274  tions": num_part
-0000eba0: 6974 696f 6e73 2c0a 2020 2020 2020 2020  itions,.        
-0000ebb0: 2020 2020 2020 2020 2270 6f73 7466 6978          "postfix
-0000ebc0: 223a 2070 6f73 7466 6978 2c0a 2020 2020  ": postfix,.    
-0000ebd0: 2020 2020 2020 2020 2020 2020 226c 6172              "lar
-0000ebe0: 6765 5f69 6e70 7574 5f72 6574 656e 7469  ge_input_retenti
-0000ebf0: 6f6e 223a 206c 6172 6765 5f69 6e70 7574  on": large_input
-0000ec00: 5f72 6574 656e 7469 6f6e 2c0a 2020 2020  _retention,.    
-0000ec10: 2020 2020 2020 2020 2020 2020 226e 6f5f              "no_
-0000ec20: 6f75 7470 7574 223a 206e 6f5f 6f75 7470  output": no_outp
-0000ec30: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
-0000ec40: 7d29 290a 0a20 2020 2064 6566 2070 6f73  }))..    def pos
-0000ec50: 745f 6b61 666b 615f 6f62 6a73 2873 656c  t_kafka_objs(sel
-0000ec60: 662c 2069 6e70 7574 5f6f 626a 733a 204c  f, input_objs: L
-0000ec70: 6973 745b 416e 795d 2920 2d3e 204c 6973  ist[Any]) -> Lis
-0000ec80: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
-0000ec90: 6269 6f73 203d 205b 0a20 2020 2020 2020  bios = [.       
-0000eca0: 2020 2020 2042 7974 6573 494f 286a 736f       BytesIO(jso
-0000ecb0: 6e2e 6475 6d70 7328 0a20 2020 2020 2020  n.dumps(.       
-0000ecc0: 2020 2020 2020 2020 2069 6e70 7574 5f6f           input_o
-0000ecd0: 626a 2c0a 2020 2020 2020 2020 2020 2020  bj,.            
-0000ece0: 2020 2020 7365 7061 7261 746f 7273 3d28      separators=(
-0000ecf0: 222c 222c 2022 3a22 292c 0a20 2020 2020  ",", ":"),.     
-0000ed00: 2020 2020 2020 2020 2020 2069 6e64 656e             inden
-0000ed10: 743d 4e6f 6e65 2c0a 2020 2020 2020 2020  t=None,.        
-0000ed20: 2020 2020 2020 2020 736f 7274 5f6b 6579          sort_key
-0000ed30: 733d 5472 7565 292e 656e 636f 6465 2822  s=True).encode("
-0000ed40: 7574 662d 3822 2929 0a20 2020 2020 2020  utf-8")).       
-0000ed50: 2020 2020 2066 6f72 2069 6e70 7574 5f6f       for input_o
-0000ed60: 626a 2069 6e20 696e 7075 745f 6f62 6a73  bj in input_objs
-0000ed70: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-0000ed80: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
-0000ed90: 6f73 745f 6b61 666b 615f 6d73 6773 2862  ost_kafka_msgs(b
-0000eda0: 696f 7329 0a0a 2020 2020 6465 6620 706f  ios)..    def po
-0000edb0: 7374 5f6b 6166 6b61 5f6d 7367 7328 0a20  st_kafka_msgs(. 
-0000edc0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-0000edd0: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-0000ede0: 7574 5f64 6174 613a 204c 6973 745b 4279  ut_data: List[By
-0000edf0: 7465 7349 4f5d 2c0a 2020 2020 2020 2020  tesIO],.        
-0000ee00: 2020 2020 706f 7374 6669 783a 2073 7472      postfix: str
-0000ee10: 203d 2022 2229 202d 3e20 4c69 7374 5b73   = "") -> List[s
-0000ee20: 7472 5d3a 0a20 2020 2020 2020 206e 616d  tr]:.        nam
-0000ee30: 6573 203d 205b 6622 6669 6c65 7b70 6f73  es = [f"file{pos
-0000ee40: 7d22 2066 6f72 2070 6f73 2069 6e20 7261  }" for pos in ra
-0000ee50: 6e67 6528 6c65 6e28 696e 7075 745f 6461  nge(len(input_da
-0000ee60: 7461 2929 5d0a 2020 2020 2020 2020 7265  ta))].        re
-0000ee70: 7320 3d20 6361 7374 284b 6166 6b61 4d65  s = cast(KafkaMe
-0000ee80: 7373 6167 652c 2073 656c 662e 5f63 6c69  ssage, self._cli
-0000ee90: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-0000eea0: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-0000eeb0: 5448 4f44 5f46 494c 452c 2022 2f6b 6166  THOD_FILE, "/kaf
-0000eec0: 6b61 5f6d 7367 222c 207b 0a20 2020 2020  ka_msg", {.     
-0000eed0: 2020 2020 2020 2020 2020 2022 6461 6722             "dag"
-0000eee0: 3a20 7365 6c66 2e67 6574 5f75 7269 2829  : self.get_uri()
-0000eef0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ef00: 2020 2270 6f73 7466 6978 223a 2070 6f73    "postfix": pos
-0000ef10: 7466 6978 2c0a 2020 2020 2020 2020 2020  tfix,.          
-0000ef20: 2020 7d2c 2066 696c 6573 3d64 6963 7428    }, files=dict(
-0000ef30: 7a69 7028 6e61 6d65 732c 2069 6e70 7574  zip(names, input
-0000ef40: 5f64 6174 6129 2929 290a 2020 2020 2020  _data)))).      
-0000ef50: 2020 6d73 6773 203d 2072 6573 5b22 6d65    msgs = res["me
-0000ef60: 7373 6167 6573 225d 0a20 2020 2020 2020  ssages"].       
-0000ef70: 2072 6574 7572 6e20 5b6d 7367 735b 6b65   return [msgs[ke
-0000ef80: 795d 2066 6f72 206b 6579 2069 6e20 6e61  y] for key in na
-0000ef90: 6d65 735d 0a0a 2020 2020 6465 6620 7265  mes]..    def re
-0000efa0: 6164 5f6b 6166 6b61 5f6f 7574 7075 7428  ad_kafka_output(
-0000efb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000efc0: 662c 0a20 2020 2020 2020 2020 2020 206f  f,.            o
-0000efd0: 6666 7365 743a 2073 7472 203d 2022 6375  ffset: str = "cu
-0000efe0: 7272 656e 7422 2c0a 2020 2020 2020 2020  rrent",.        
-0000eff0: 2020 2020 6d61 785f 726f 7773 3a20 696e      max_rows: in
-0000f000: 7420 3d20 3130 3029 202d 3e20 4f70 7469  t = 100) -> Opti
-0000f010: 6f6e 616c 5b42 7974 6552 6573 706f 6e73  onal[ByteRespons
-0000f020: 655d 3a0a 2020 2020 2020 2020 6f66 6673  e]:.        offs
-0000f030: 6574 5f73 7472 203d 205b 6f66 6673 6574  et_str = [offset
-0000f040: 5d0a 0a20 2020 2020 2020 2064 6566 2072  ]..        def r
-0000f050: 6561 645f 7369 6e67 6c65 2829 202d 3e20  ead_single() -> 
-0000f060: 5475 706c 655b 4f70 7469 6f6e 616c 5b42  Tuple[Optional[B
-0000f070: 7974 6552 6573 706f 6e73 655d 2c20 7374  yteResponse], st
-0000f080: 725d 3a0a 2020 2020 2020 2020 2020 2020  r]:.            
-0000f090: 6375 722c 2072 6561 645f 6374 7970 6520  cur, read_ctype 
-0000f0a0: 3d20 7365 6c66 2e5f 636c 6965 6e74 2e72  = self._client.r
-0000f0b0: 6571 7565 7374 5f62 7974 6573 280a 2020  equest_bytes(.  
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000f0d0: 5448 4f44 5f47 4554 2c20 222f 6b61 666b  THOD_GET, "/kafk
-0000f0e0: 615f 6d73 6722 2c20 7b0a 2020 2020 2020  a_msg", {.      
-0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-0000f100: 6167 223a 2073 656c 662e 6765 745f 7572  ag": self.get_ur
-0000f110: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
-0000f120: 2020 2020 2020 2020 2022 6f66 6673 6574           "offset
-0000f130: 223a 206f 6666 7365 745f 7374 725b 305d  ": offset_str[0]
-0000f140: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f150: 2020 7d29 0a20 2020 2020 2020 2020 2020    }).           
-0000f160: 206f 6666 7365 745f 7374 725b 305d 203d   offset_str[0] =
-0000f170: 2022 6375 7272 656e 7422 0a20 2020 2020   "current".     
-0000f180: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
-0000f190: 7465 7270 7265 745f 6374 7970 6528 6375  terpret_ctype(cu
-0000f1a0: 722c 2072 6561 645f 6374 7970 6529 2c20  r, read_ctype), 
-0000f1b0: 7265 6164 5f63 7479 7065 0a0a 2020 2020  read_ctype..    
-0000f1c0: 2020 2020 6966 206d 6178 5f72 6f77 7320      if max_rows 
-0000f1d0: 3c3d 2031 3a0a 2020 2020 2020 2020 2020  <= 1:.          
-0000f1e0: 2020 7265 7475 726e 2072 6561 645f 7369    return read_si
-0000f1f0: 6e67 6c65 2829 5b30 5d0a 0a20 2020 2020  ngle()[0]..     
-0000f200: 2020 2072 6573 3a20 4c69 7374 5b42 7974     res: List[Byt
-0000f210: 6552 6573 706f 6e73 655d 203d 205b 5d0a  eResponse] = [].
-0000f220: 2020 2020 2020 2020 6374 7970 653a 204f          ctype: O
-0000f230: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000f240: 6f6e 650a 2020 2020 2020 2020 7768 696c  one.        whil
-0000f250: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
-0000f260: 2020 2020 7661 6c2c 2063 7572 5f63 7479      val, cur_cty
-0000f270: 7065 203d 2072 6561 645f 7369 6e67 6c65  pe = read_single
-0000f280: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-0000f290: 6620 7661 6c20 6973 204e 6f6e 653a 0a20  f val is None:. 
-0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000f2b0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-0000f2c0: 2069 6620 6374 7970 6520 6973 204e 6f6e   if ctype is Non
-0000f2d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000f2e0: 2020 2063 7479 7065 203d 2063 7572 5f63     ctype = cur_c
-0000f2f0: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
-0000f300: 2065 6c69 6620 6374 7970 6520 213d 2063   elif ctype != c
-0000f310: 7572 5f63 7479 7065 3a0a 2020 2020 2020  ur_ctype:.      
-0000f320: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000f330: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 6622 696e 636f 6e73 6973 7465 6e74 2072  f"inconsistent r
-0000f360: 6574 7572 6e20 7479 7065 7320 7b63 7479  eturn types {cty
-0000f370: 7065 7d20 213d 207b 6375 725f 6374 7970  pe} != {cur_ctyp
-0000f380: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-0000f390: 2072 6573 2e61 7070 656e 6428 7661 6c29   res.append(val)
-0000f3a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f3b0: 6c65 6e28 7265 7329 203e 3d20 6d61 785f  len(res) >= max_
-0000f3c0: 726f 7773 3a0a 2020 2020 2020 2020 2020  rows:.          
-0000f3d0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-0000f3e0: 2020 2020 6966 206e 6f74 2072 6573 206f      if not res o
-0000f3f0: 7220 6374 7970 6520 6973 204e 6f6e 653a  r ctype is None:
-0000f400: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000f410: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-0000f420: 2072 6574 7572 6e20 6d65 7267 655f 6374   return merge_ct
-0000f430: 7970 6528 7265 732c 2063 7479 7065 290a  ype(res, ctype).
-0000f440: 0a20 2020 2064 6566 2067 6574 5f6b 6166  .    def get_kaf
-0000f450: 6b61 5f6f 6666 7365 7473 280a 2020 2020  ka_offsets(.    
-0000f460: 2020 2020 2020 2020 7365 6c66 2c20 616c          self, al
-0000f470: 6976 653a 2062 6f6f 6c2c 2070 6f73 7466  ive: bool, postf
-0000f480: 6978 3a20 4f70 7469 6f6e 616c 5b73 7472  ix: Optional[str
-0000f490: 5d20 3d20 4e6f 6e65 2920 2d3e 204b 6166  ] = None) -> Kaf
-0000f4a0: 6b61 4f66 6673 6574 733a 0a20 2020 2020  kaOffsets:.     
-0000f4b0: 2020 2061 7267 7320 3d20 7b0a 2020 2020     args = {.    
-0000f4c0: 2020 2020 2020 2020 2264 6167 223a 2073          "dag": s
-0000f4d0: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
-0000f4e0: 2020 2020 2020 2020 2020 2022 616c 6976             "aliv
-0000f4f0: 6522 3a20 696e 7428 616c 6976 6529 2c0a  e": int(alive),.
-0000f500: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0000f510: 2020 6966 2070 6f73 7466 6978 2069 7320    if postfix is 
-0000f520: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000f530: 2020 2020 2020 6172 6773 5b22 706f 7374        args["post
-0000f540: 6669 7822 5d20 3d20 706f 7374 6669 780a  fix"] = postfix.
-0000f550: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0000f560: 6173 7428 4b61 666b 614f 6666 7365 7473  ast(KafkaOffsets
-0000f570: 2c20 7365 6c66 2e5f 636c 6965 6e74 2e72  , self._client.r
-0000f580: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
-0000f590: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-0000f5a0: 4745 542c 2022 2f6b 6166 6b61 5f6f 6666  GET, "/kafka_off
-0000f5b0: 7365 7473 222c 2061 7267 7329 290a 0a20  sets", args)).. 
-0000f5c0: 2020 2064 6566 2067 6574 5f6b 6166 6b61     def get_kafka
-0000f5d0: 5f74 6872 6f75 6768 7075 7428 0a20 2020  _throughput(.   
-0000f5e0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-0000f5f0: 2020 2020 2020 2020 2020 2070 6f73 7466             postf
-0000f600: 6978 3a20 4f70 7469 6f6e 616c 5b73 7472  ix: Optional[str
-0000f610: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000f620: 2020 2020 2020 7365 676d 656e 745f 696e        segment_in
-0000f630: 7465 7276 616c 3a20 666c 6f61 7420 3d20  terval: float = 
-0000f640: 3132 302e 302c 0a20 2020 2020 2020 2020  120.0,.         
-0000f650: 2020 2073 6567 6d65 6e74 733a 2069 6e74     segments: int
-0000f660: 203d 2035 2920 2d3e 204b 6166 6b61 5468   = 5) -> KafkaTh
-0000f670: 726f 7567 6870 7574 3a0a 2020 2020 2020  roughput:.      
-0000f680: 2020 6173 7365 7274 2073 6567 6d65 6e74    assert segment
-0000f690: 7320 3e20 300a 2020 2020 2020 2020 6173  s > 0.        as
-0000f6a0: 7365 7274 2073 6567 6d65 6e74 5f69 6e74  sert segment_int
-0000f6b0: 6572 7661 6c20 3e20 302e 300a 2020 2020  erval > 0.0.    
-0000f6c0: 2020 2020 6f66 6673 6574 7320 3d20 7365      offsets = se
-0000f6d0: 6c66 2e67 6574 5f6b 6166 6b61 5f6f 6666  lf.get_kafka_off
-0000f6e0: 7365 7473 2870 6f73 7466 6978 3d70 6f73  sets(postfix=pos
-0000f6f0: 7466 6978 2c20 616c 6976 653d 4661 6c73  tfix, alive=Fals
-0000f700: 6529 0a20 2020 2020 2020 206e 6f77 203d  e).        now =
-0000f710: 2074 696d 652e 6d6f 6e6f 746f 6e69 6328   time.monotonic(
-0000f720: 290a 2020 2020 2020 2020 6d65 6173 7572  ).        measur
-0000f730: 656d 656e 7473 3a20 4c69 7374 5b54 7570  ements: List[Tup
-0000f740: 6c65 5b69 6e74 2c20 696e 742c 2069 6e74  le[int, int, int
-0000f750: 2c20 666c 6f61 745d 5d20 3d20 5b28 0a20  , float]] = [(. 
-0000f760: 2020 2020 2020 2020 2020 206f 6666 7365             offse
-0000f770: 7473 5b22 696e 7075 7422 5d2c 0a20 2020  ts["input"],.   
-0000f780: 2020 2020 2020 2020 206f 6666 7365 7473           offsets
-0000f790: 5b22 6f75 7470 7574 225d 2c0a 2020 2020  ["output"],.    
-0000f7a0: 2020 2020 2020 2020 6f66 6673 6574 735b          offsets[
-0000f7b0: 2265 7272 6f72 225d 2c0a 2020 2020 2020  "error"],.      
-0000f7c0: 2020 2020 2020 6e6f 772c 0a20 2020 2020        now,.     
-0000f7d0: 2020 2029 5d0a 2020 2020 2020 2020 666f     )].        fo
-0000f7e0: 7220 5f20 696e 2072 616e 6765 2873 6567  r _ in range(seg
-0000f7f0: 6d65 6e74 7329 3a0a 2020 2020 2020 2020  ments):.        
-0000f800: 2020 2020 7072 6576 203d 206e 6f77 0a20      prev = now. 
-0000f810: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-0000f820: 206e 6f77 202d 2070 7265 7620 3c20 7365   now - prev < se
-0000f830: 676d 656e 745f 696e 7465 7276 616c 3a0a  gment_interval:.
-0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f850: 7469 6d65 2e73 6c65 6570 286d 6178 2830  time.sleep(max(0
-0000f860: 2e30 2c20 7365 676d 656e 745f 696e 7465  .0, segment_inte
-0000f870: 7276 616c 202d 2028 6e6f 7720 2d20 7072  rval - (now - pr
-0000f880: 6576 2929 290a 2020 2020 2020 2020 2020  ev))).          
-0000f890: 2020 2020 2020 6e6f 7720 3d20 7469 6d65        now = time
-0000f8a0: 2e6d 6f6e 6f74 6f6e 6963 2829 0a20 2020  .monotonic().   
-0000f8b0: 2020 2020 2020 2020 206f 6666 7365 7473           offsets
-0000f8c0: 203d 2073 656c 662e 6765 745f 6b61 666b   = self.get_kafk
-0000f8d0: 615f 6f66 6673 6574 7328 706f 7374 6669  a_offsets(postfi
-0000f8e0: 783d 706f 7374 6669 782c 2061 6c69 7665  x=postfix, alive
-0000f8f0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-0000f900: 2020 2020 6d65 6173 7572 656d 656e 7473      measurements
-0000f910: 2e61 7070 656e 6428 280a 2020 2020 2020  .append((.      
-0000f920: 2020 2020 2020 2020 2020 6f66 6673 6574            offset
-0000f930: 735b 2269 6e70 7574 225d 2c0a 2020 2020  s["input"],.    
-0000f940: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
-0000f950: 6574 735b 226f 7574 7075 7422 5d2c 0a20  ets["output"],. 
-0000f960: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000f970: 6666 7365 7473 5b22 6572 726f 7222 5d2c  ffsets["error"],
-0000f980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f990: 206e 6f77 2c0a 2020 2020 2020 2020 2020   now,.          
-0000f9a0: 2020 2929 0a20 2020 2020 2020 2066 6972    )).        fir
-0000f9b0: 7374 203d 206d 6561 7375 7265 6d65 6e74  st = measurement
-0000f9c0: 735b 305d 0a20 2020 2020 2020 206c 6173  s[0].        las
-0000f9d0: 7420 3d20 6d65 6173 7572 656d 656e 7473  t = measurements
-0000f9e0: 5b2d 315d 0a20 2020 2020 2020 2074 6f74  [-1].        tot
-0000f9f0: 616c 5f69 6e70 7574 203d 206c 6173 745b  al_input = last[
-0000fa00: 305d 202d 2066 6972 7374 5b30 5d0a 2020  0] - first[0].  
-0000fa10: 2020 2020 2020 746f 7461 6c5f 6f75 7470        total_outp
-0000fa20: 7574 203d 206c 6173 745b 315d 202d 2066  ut = last[1] - f
-0000fa30: 6972 7374 5b31 5d0a 2020 2020 2020 2020  irst[1].        
-0000fa40: 6572 726f 7273 203d 206c 6173 745b 325d  errors = last[2]
-0000fa50: 202d 2066 6972 7374 5b32 5d0a 2020 2020   - first[2].    
-0000fa60: 2020 2020 746f 7461 6c20 3d20 6c61 7374      total = last
-0000fa70: 5b33 5d20 2d20 6669 7273 745b 335d 0a20  [3] - first[3]. 
-0000fa80: 2020 2020 2020 2069 6e70 7574 5f73 6567         input_seg
-0000fa90: 6d65 6e74 733a 204c 6973 745b 666c 6f61  ments: List[floa
-0000faa0: 745d 203d 205b 5d0a 2020 2020 2020 2020  t] = [].        
-0000fab0: 6f75 7470 7574 5f73 6567 6d65 6e74 733a  output_segments:
-0000fac0: 204c 6973 745b 666c 6f61 745d 203d 205b   List[float] = [
-0000fad0: 5d0a 2020 2020 2020 2020 6375 725f 696e  ].        cur_in
-0000fae0: 7075 7420 3d20 6669 7273 745b 305d 0a20  put = first[0]. 
-0000faf0: 2020 2020 2020 2063 7572 5f6f 7574 7075         cur_outpu
-0000fb00: 7420 3d20 6669 7273 745b 315d 0a20 2020  t = first[1].   
-0000fb10: 2020 2020 2063 7572 5f74 696d 6520 3d20       cur_time = 
-0000fb20: 6669 7273 745b 335d 0a20 2020 2020 2020  first[3].       
-0000fb30: 2066 6f72 2028 6e65 7874 5f69 6e70 7574   for (next_input
-0000fb40: 2c20 6e65 7874 5f6f 7574 7075 742c 205f  , next_output, _
-0000fb50: 2c20 6e65 7874 5f74 696d 6529 2069 6e20  , next_time) in 
-0000fb60: 6d65 6173 7572 656d 656e 7473 5b31 3a5d  measurements[1:]
-0000fb70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fb80: 675f 7469 6d65 203d 206e 6578 745f 7469  g_time = next_ti
-0000fb90: 6d65 202d 2063 7572 5f74 696d 650a 2020  me - cur_time.  
-0000fba0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000fbb0: 7365 676d 656e 7473 2e61 7070 656e 6428  segments.append(
-0000fbc0: 286e 6578 745f 696e 7075 7420 2d20 6375  (next_input - cu
-0000fbd0: 725f 696e 7075 7429 202f 2073 6567 5f74  r_input) / seg_t
-0000fbe0: 696d 6529 0a20 2020 2020 2020 2020 2020  ime).           
-0000fbf0: 206f 7574 7075 745f 7365 676d 656e 7473   output_segments
-0000fc00: 2e61 7070 656e 6428 286e 6578 745f 6f75  .append((next_ou
-0000fc10: 7470 7574 202d 2063 7572 5f6f 7574 7075  tput - cur_outpu
-0000fc20: 7429 202f 2073 6567 5f74 696d 6529 0a20  t) / seg_time). 
-0000fc30: 2020 2020 2020 2020 2020 2063 7572 5f69             cur_i
-0000fc40: 6e70 7574 203d 206e 6578 745f 696e 7075  nput = next_inpu
-0000fc50: 740a 2020 2020 2020 2020 2020 2020 6375  t.            cu
-0000fc60: 725f 6f75 7470 7574 203d 206e 6578 745f  r_output = next_
-0000fc70: 6f75 7470 7574 0a20 2020 2020 2020 2020  output.         
-0000fc80: 2020 2063 7572 5f74 696d 6520 3d20 6e65     cur_time = ne
-0000fc90: 7874 5f74 696d 650a 2020 2020 2020 2020  xt_time.        
-0000fca0: 696e 7075 7473 203d 2070 642e 5365 7269  inputs = pd.Seri
-0000fcb0: 6573 2869 6e70 7574 5f73 6567 6d65 6e74  es(input_segment
-0000fcc0: 7329 0a20 2020 2020 2020 206f 7574 7075  s).        outpu
-0000fcd0: 7473 203d 2070 642e 5365 7269 6573 286f  ts = pd.Series(o
-0000fce0: 7574 7075 745f 7365 676d 656e 7473 290a  utput_segments).
-0000fcf0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-0000fd00: 0a20 2020 2020 2020 2020 2020 2022 6461  .            "da
-0000fd10: 6722 3a20 7365 6c66 2e67 6574 5f75 7269  g": self.get_uri
-0000fd20: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0000fd30: 2269 6e70 7574 223a 207b 0a20 2020 2020  "input": {.     
-0000fd40: 2020 2020 2020 2020 2020 2022 7468 726f             "thro
-0000fd50: 7567 6870 7574 223a 2074 6f74 616c 5f69  ughput": total_i
-0000fd60: 6e70 7574 202f 2074 6f74 616c 2c0a 2020  nput / total,.  
-0000fd70: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0000fd80: 6178 223a 2069 6e70 7574 732e 6d61 7828  ax": inputs.max(
-0000fd90: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000fda0: 2020 2022 6d69 6e22 3a20 696e 7075 7473     "min": inputs
-0000fdb0: 2e6d 696e 2829 2c0a 2020 2020 2020 2020  .min(),.        
-0000fdc0: 2020 2020 2020 2020 2273 7464 6465 7622          "stddev"
-0000fdd0: 3a20 696e 7075 7473 2e73 7464 2829 2c0a  : inputs.std(),.
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdf0: 2273 6567 6d65 6e74 7322 3a20 7365 676d  "segments": segm
-0000fe00: 656e 7473 2c0a 2020 2020 2020 2020 2020  ents,.          
-0000fe10: 2020 2020 2020 2263 6f75 6e74 223a 2074        "count": t
-0000fe20: 6f74 616c 5f69 6e70 7574 2c0a 2020 2020  otal_input,.    
-0000fe30: 2020 2020 2020 2020 2020 2020 2274 6f74              "tot
-0000fe40: 616c 223a 2074 6f74 616c 2c0a 2020 2020  al": total,.    
-0000fe50: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-0000fe60: 2020 2020 2020 2022 6f75 7470 7574 223a         "output":
-0000fe70: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0000fe80: 2020 2022 7468 726f 7567 6870 7574 223a     "throughput":
-0000fe90: 2074 6f74 616c 5f6f 7574 7075 7420 2f20   total_output / 
-0000fea0: 746f 7461 6c2c 0a20 2020 2020 2020 2020  total,.         
-0000feb0: 2020 2020 2020 2022 6d61 7822 3a20 6f75         "max": ou
-0000fec0: 7470 7574 732e 6d61 7828 292c 0a20 2020  tputs.max(),.   
-0000fed0: 2020 2020 2020 2020 2020 2020 2022 6d69               "mi
-0000fee0: 6e22 3a20 6f75 7470 7574 732e 6d69 6e28  n": outputs.min(
-0000fef0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000ff00: 2020 2022 7374 6464 6576 223a 206f 7574     "stddev": out
-0000ff10: 7075 7473 2e73 7464 2829 2c0a 2020 2020  puts.std(),.    
-0000ff20: 2020 2020 2020 2020 2020 2020 2273 6567              "seg
-0000ff30: 6d65 6e74 7322 3a20 7365 676d 656e 7473  ments": segments
-0000ff40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ff50: 2020 2263 6f75 6e74 223a 2074 6f74 616c    "count": total
-0000ff60: 5f6f 7574 7075 742c 0a20 2020 2020 2020  _output,.       
-0000ff70: 2020 2020 2020 2020 2022 746f 7461 6c22           "total"
-0000ff80: 3a20 746f 7461 6c2c 0a20 2020 2020 2020  : total,.       
-0000ff90: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-0000ffa0: 2020 2020 2266 6173 7465 7222 3a20 2262      "faster": "b
-0000ffb0: 6f74 6822 2069 6620 746f 7461 6c5f 696e  oth" if total_in
-0000ffc0: 7075 7420 3d3d 2074 6f74 616c 5f6f 7574  put == total_out
-0000ffd0: 7075 7420 656c 7365 2028 0a20 2020 2020  put else (.     
-0000ffe0: 2020 2020 2020 2020 2020 2022 696e 7075             "inpu
-0000fff0: 7422 2069 6620 746f 7461 6c5f 696e 7075  t" if total_inpu
-00010000: 7420 3e20 746f 7461 6c5f 6f75 7470 7574  t > total_output
-00010010: 2065 6c73 6520 226f 7574 7075 7422 292c   else "output"),
-00010020: 0a20 2020 2020 2020 2020 2020 2022 6572  .            "er
-00010030: 726f 7273 223a 2065 7272 6f72 732c 0a20  rors": errors,. 
-00010040: 2020 2020 2020 207d 0a0a 2020 2020 6465         }..    de
-00010050: 6620 6765 745f 6b61 666b 615f 6772 6f75  f get_kafka_grou
-00010060: 7028 7365 6c66 2920 2d3e 204b 6166 6b61  p(self) -> Kafka
-00010070: 4772 6f75 703a 0a20 2020 2020 2020 2072  Group:.        r
-00010080: 6574 7572 6e20 6361 7374 284b 6166 6b61  eturn cast(Kafka
-00010090: 4772 6f75 702c 2073 656c 662e 5f63 6c69  Group, self._cli
-000100a0: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-000100b0: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-000100c0: 5448 4f44 5f47 4554 2c20 222f 6b61 666b  THOD_GET, "/kafk
-000100d0: 615f 6772 6f75 7022 2c20 7b0a 2020 2020  a_group", {.    
-000100e0: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
-000100f0: 223a 2073 656c 662e 6765 745f 7572 6928  ": self.get_uri(
-00010100: 292c 0a20 2020 2020 2020 2020 2020 207d  ),.            }
-00010110: 2929 0a0a 2020 2020 6465 6620 7365 745f  ))..    def set_
-00010120: 6b61 666b 615f 6772 6f75 7028 0a20 2020  kafka_group(.   
-00010130: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00010140: 2020 2020 2020 2020 2020 2067 726f 7570             group
-00010150: 5f69 643a 204f 7074 696f 6e61 6c5b 7374  _id: Optional[st
-00010160: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00010170: 2020 2020 2020 2072 6573 6574 3a20 4f70         reset: Op
-00010180: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00010190: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000101a0: 2a2a 6b77 6172 6773 3a20 416e 7929 202d  **kwargs: Any) -
-000101b0: 3e20 4b61 666b 6147 726f 7570 3a0a 2020  > KafkaGroup:.  
-000101c0: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
-000101d0: 7428 4b61 666b 6147 726f 7570 2c20 7365  t(KafkaGroup, se
-000101e0: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-000101f0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-00010200: 2020 2020 204d 4554 484f 445f 5055 542c       METHOD_PUT,
-00010210: 2022 2f6b 6166 6b61 5f67 726f 7570 222c   "/kafka_group",
-00010220: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00010230: 2020 2022 6461 6722 3a20 7365 6c66 2e67     "dag": self.g
-00010240: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
-00010250: 2020 2020 2020 2020 2020 2267 726f 7570            "group
-00010260: 5f69 6422 3a20 6772 6f75 705f 6964 2c0a  _id": group_id,.
-00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010280: 2272 6573 6574 223a 2072 6573 6574 2c0a  "reset": reset,.
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
-000102b0: 2020 2020 2020 7d29 290a 0a20 2020 2064        }))..    d
-000102c0: 6566 2064 656c 6574 6528 7365 6c66 2920  ef delete(self) 
-000102d0: 2d3e 2044 656c 6574 6542 6c6f 6252 6573  -> DeleteBlobRes
-000102e0: 706f 6e73 653a 0a20 2020 2020 2020 2072  ponse:.        r
-000102f0: 6574 7572 6e20 6361 7374 2844 656c 6574  eturn cast(Delet
-00010300: 6542 6c6f 6252 6573 706f 6e73 652c 2073  eBlobResponse, s
-00010310: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
-00010320: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-00010330: 2020 2020 2020 4d45 5448 4f44 5f44 454c        METHOD_DEL
-00010340: 4554 452c 2022 2f62 6c6f 6222 2c20 7b0a  ETE, "/blob", {.
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 2262 6c6f 625f 7572 6973 223a 205b 7365  "blob_uris": [se
-00010370: 6c66 2e67 6574 5f75 7269 2829 5d2c 0a20  lf.get_uri()],. 
-00010380: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00010390: 2020 2020 2020 2929 0a0a 2020 2020 6465        ))..    de
-000103a0: 6620 646f 776e 6c6f 6164 5f66 756c 6c5f  f download_full_
-000103b0: 6461 675f 7a69 7028 0a20 2020 2020 2020  dag_zip(.       
-000103c0: 2020 2020 2073 656c 662c 2074 6f5f 7061       self, to_pa
-000103d0: 7468 3a20 4f70 7469 6f6e 616c 5b73 7472  th: Optional[str
-000103e0: 5d29 202d 3e20 4f70 7469 6f6e 616c 5b69  ]) -> Optional[i
-000103f0: 6f2e 4279 7465 7349 4f5d 3a0a 2020 2020  o.BytesIO]:.    
-00010400: 2020 2020 6375 725f 7265 732c 205f 203d      cur_res, _ =
-00010410: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
-00010420: 7175 6573 745f 6279 7465 7328 0a20 2020  quest_bytes(.   
-00010430: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-00010440: 4745 542c 2022 2f64 6f77 6e6c 6f61 645f  GET, "/download_
-00010450: 6461 675f 7a69 7022 2c20 7b0a 2020 2020  dag_zip", {.    
-00010460: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
-00010470: 223a 2073 656c 662e 6765 745f 7572 6928  ": self.get_uri(
-00010480: 292c 0a20 2020 2020 2020 2020 2020 207d  ),.            }
-00010490: 290a 2020 2020 2020 2020 6966 2074 6f5f  ).        if to_
-000104a0: 7061 7468 2069 7320 4e6f 6e65 3a0a 2020  path is None:.  
-000104b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000104c0: 2069 6f2e 4279 7465 7349 4f28 6375 725f   io.BytesIO(cur_
-000104d0: 7265 732e 7265 6164 2829 290a 2020 2020  res.read()).    
-000104e0: 2020 2020 7769 7468 206f 7065 6e28 746f      with open(to
-000104f0: 5f70 6174 682c 2022 7762 2229 2061 7320  _path, "wb") as 
-00010500: 6669 6c65 5f64 6f77 6e6c 6f61 643a 0a20  file_download:. 
-00010510: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-00010520: 646f 776e 6c6f 6164 2e77 7269 7465 2863  download.write(c
-00010530: 7572 5f72 6573 2e72 6561 6428 2929 0a20  ur_res.read()). 
-00010540: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00010550: 6e65 0a0a 2020 2020 6465 6620 5f75 706c  ne..    def _upl
-00010560: 6f61 645f 6461 675f 626c 6f62 7328 0a20  oad_dag_blobs(. 
-00010570: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00010580: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-00010590: 6469 723a 2073 7472 2c0a 2020 2020 2020  dir: str,.      
-000105a0: 2020 2020 2020 626c 6f62 735f 6d61 703a        blobs_map:
-000105b0: 204c 6973 745b 426c 6f62 4465 7461 696c   List[BlobDetail
-000105c0: 735d 2c0a 2020 2020 2020 2020 2020 2020  s],.            
-000105d0: 6d61 785f 7468 7265 6164 733a 2069 6e74  max_threads: int
-000105e0: 2920 2d3e 204c 6973 745b 2742 6c6f 6248  ) -> List['BlobH
-000105f0: 616e 646c 6527 5d3a 0a20 2020 2020 2020  andle']:.       
-00010600: 2062 6c6f 625f 6861 6e64 6c65 7320 3d20   blob_handles = 
-00010610: 5b5d 0a20 2020 2020 2020 2066 6f72 2062  [].        for b
-00010620: 6c6f 6220 696e 2062 6c6f 6273 5f6d 6170  lob in blobs_map
-00010630: 3a0a 2020 2020 2020 2020 2020 2020 626c  :.            bl
-00010640: 6f62 5f66 696c 6520 3d20 6f73 2e70 6174  ob_file = os.pat
-00010650: 682e 6a6f 696e 2874 6d70 6469 722c 2062  h.join(tmpdir, b
-00010660: 6c6f 625b 2266 6e61 6d65 225d 290a 2020  lob["fname"]).  
-00010670: 2020 2020 2020 2020 2020 626c 6f62 5f68            blob_h
-00010680: 616e 646c 6520 3d20 7365 6c66 2e5f 636c  andle = self._cl
-00010690: 6965 6e74 2e67 6574 5f62 6c6f 625f 6861  ient.get_blob_ha
-000106a0: 6e64 6c65 2862 6c6f 625b 2262 6c6f 625f  ndle(blob["blob_
-000106b0: 7572 6922 5d29 0a20 2020 2020 2020 2020  uri"]).         
-000106c0: 2020 2062 6c6f 625f 6861 6e64 6c65 732e     blob_handles.
-000106d0: 6578 7465 6e64 2862 6c6f 625f 6861 6e64  extend(blob_hand
-000106e0: 6c65 2e75 706c 6f61 645f 7a69 7028 626c  le.upload_zip(bl
-000106f0: 6f62 5f66 696c 652c 206d 6178 5f74 6872  ob_file, max_thr
-00010700: 6561 6473 2929 0a20 2020 2020 2020 2072  eads)).        r
-00010710: 6574 7572 6e20 626c 6f62 5f68 616e 646c  eturn blob_handl
-00010720: 6573 0a0a 2020 2020 6465 6620 7570 6c6f  es..    def uplo
-00010730: 6164 5f66 756c 6c5f 6461 675f 7a69 7028  ad_full_dag_zip(
-00010740: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010750: 662c 2073 6f75 7263 653a 2073 7472 2c20  f, source: str, 
-00010760: 6d61 785f 7468 7265 6164 733a 2069 6e74  max_threads: int
-00010770: 203d 2031 3029 202d 3e20 4c69 7374 5b27   = 10) -> List['
-00010780: 426c 6f62 4861 6e64 6c65 275d 3a0a 2020  BlobHandle']:.  
-00010790: 2020 2020 2020 6461 675f 626c 6f62 5f68        dag_blob_h
-000107a0: 616e 646c 6520 3d20 7365 6c66 2e5f 636c  andle = self._cl
-000107b0: 6965 6e74 2e67 6574 5f62 6c6f 625f 6861  ient.get_blob_ha
-000107c0: 6e64 6c65 2873 656c 662e 6765 745f 7572  ndle(self.get_ur
-000107d0: 6928 2929 0a20 2020 2020 2020 2062 6c6f  i()).        blo
-000107e0: 625f 6861 6e64 6c65 7320 3d20 5b5d 0a20  b_handles = []. 
-000107f0: 2020 2020 2020 2077 6974 6820 7465 6d70         with temp
-00010800: 6669 6c65 2e54 656d 706f 7261 7279 4469  file.TemporaryDi
-00010810: 7265 6374 6f72 7928 2920 6173 2074 6d70  rectory() as tmp
-00010820: 6469 723a 0a20 2020 2020 2020 2020 2020  dir:.           
-00010830: 2073 6875 7469 6c2e 756e 7061 636b 5f61   shutil.unpack_a
-00010840: 7263 6869 7665 2873 6f75 7263 652c 2074  rchive(source, t
-00010850: 6d70 6469 722c 2022 7a69 7022 290a 2020  mpdir, "zip").  
-00010860: 2020 2020 2020 2020 2020 666d 6170 5f6a            fmap_j
-00010870: 736f 6e20 3d20 6f73 2e70 6174 682e 6a6f  son = os.path.jo
-00010880: 696e 2874 6d70 6469 722c 2022 6669 6c65  in(tmpdir, "file
-00010890: 6d61 702e 6a73 6f6e 2229 0a20 2020 2020  map.json").     
-000108a0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-000108b0: 2866 6d61 705f 6a73 6f6e 2c20 2272 2229  (fmap_json, "r")
-000108c0: 2061 7320 666d 6170 3a0a 2020 2020 2020   as fmap:.      
-000108d0: 2020 2020 2020 2020 2020 6669 6c65 5f6d            file_m
-000108e0: 6170 3a20 4669 6c65 4d61 7020 3d20 6a73  ap: FileMap = js
-000108f0: 6f6e 2e6c 6f61 6428 666d 6170 290a 2020  on.load(fmap).  
-00010900: 2020 2020 2020 2020 2020 6461 675f 666e            dag_fn
-00010910: 616d 6520 3d20 6669 6c65 5f6d 6170 5b22  ame = file_map["
-00010920: 6461 675f 626c 6f62 225d 0a20 2020 2020  dag_blob"].     
-00010930: 2020 2020 2020 2064 6167 5f66 696c 6520         dag_file 
-00010940: 3d20 6f73 2e70 6174 682e 6a6f 696e 2874  = os.path.join(t
-00010950: 6d70 6469 722c 2066 227b 6461 675f 666e  mpdir, f"{dag_fn
-00010960: 616d 657d 2229 0a20 2020 2020 2020 2020  ame}").         
-00010970: 2020 2062 6c6f 625f 6861 6e64 6c65 732e     blob_handles.
-00010980: 6578 7465 6e64 280a 2020 2020 2020 2020  extend(.        
-00010990: 2020 2020 2020 2020 6461 675f 626c 6f62          dag_blob
-000109a0: 5f68 616e 646c 652e 7570 6c6f 6164 5f7a  _handle.upload_z
-000109b0: 6970 2864 6167 5f66 696c 652c 206d 6178  ip(dag_file, max
-000109c0: 5f74 6872 6561 6473 2929 0a20 2020 2020  _threads)).     
-000109d0: 2020 2020 2020 2062 6c6f 625f 6861 6e64         blob_hand
-000109e0: 6c65 732e 6578 7465 6e64 2873 656c 662e  les.extend(self.
-000109f0: 5f75 706c 6f61 645f 6461 675f 626c 6f62  _upload_dag_blob
-00010a00: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00010a10: 2020 2074 6d70 6469 722c 2066 696c 655f     tmpdir, file_
-00010a20: 6d61 705b 2262 6c6f 6273 225d 2c20 6d61  map["blobs"], ma
-00010a30: 785f 7468 7265 6164 7329 290a 2020 2020  x_threads)).    
-00010a40: 2020 2020 7265 7475 726e 2062 6c6f 625f      return blob_
-00010a50: 6861 6e64 6c65 730a 0a20 2020 2064 6566  handles..    def
-00010a60: 205f 5f68 6173 685f 5f28 7365 6c66 2920   __hash__(self) 
-00010a70: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00010a80: 7265 7475 726e 2068 6173 6828 7365 6c66  return hash(self
-00010a90: 2e67 6574 5f75 7269 2829 290a 0a20 2020  .get_uri())..   
-00010aa0: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
-00010ab0: 2c20 6f74 6865 723a 206f 626a 6563 7429  , other: object)
-00010ac0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00010ad0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00010ae0: 6e63 6528 6f74 6865 722c 2073 656c 662e  nce(other, self.
-00010af0: 5f5f 636c 6173 735f 5f29 3a0a 2020 2020  __class__):.    
-00010b00: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00010b10: 616c 7365 0a20 2020 2020 2020 2072 6574  alse.        ret
-00010b20: 7572 6e20 7365 6c66 2e67 6574 5f75 7269  urn self.get_uri
-00010b30: 2829 203d 3d20 6f74 6865 722e 6765 745f  () == other.get_
-00010b40: 7572 6928 290a 0a20 2020 2064 6566 205f  uri()..    def _
-00010b50: 5f6e 655f 5f28 7365 6c66 2c20 6f74 6865  _ne__(self, othe
-00010b60: 723a 206f 626a 6563 7429 202d 3e20 626f  r: object) -> bo
-00010b70: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-00010b80: 726e 206e 6f74 2073 656c 662e 5f5f 6571  rn not self.__eq
-00010b90: 5f5f 286f 7468 6572 290a 0a20 2020 2064  __(other)..    d
-00010ba0: 6566 205f 5f73 7472 5f5f 2873 656c 6629  ef __str__(self)
-00010bb0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00010bc0: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
-00010bd0: 5f75 7269 2829 0a0a 2020 2020 6465 6620  _uri()..    def 
-00010be0: 5f5f 7265 7072 5f5f 2873 656c 6629 202d  __repr__(self) -
-00010bf0: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
-00010c00: 6574 7572 6e20 6622 7b73 656c 662e 5f5f  eturn f"{self.__
-00010c10: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-00010c20: 7d5b 7b73 656c 662e 6765 745f 7572 6928  }[{self.get_uri(
-00010c30: 297d 5d22 0a0a 2320 2a2a 2a20 4461 6748  )}]"..# *** DagH
-00010c40: 616e 646c 6520 2a2a 2a0a 0a0a 636c 6173  andle ***...clas
-00010c50: 7320 4e6f 6465 4861 6e64 6c65 3a0a 2020  s NodeHandle:.  
-00010c60: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00010c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010c80: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
-00010c90: 6965 6e74 3a20 5859 4d45 436c 6965 6e74  ient: XYMEClient
-00010ca0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00010cb0: 673a 2044 6167 4861 6e64 6c65 2c0a 2020  g: DagHandle,.  
-00010cc0: 2020 2020 2020 2020 2020 6e6f 6465 5f69            node_i
-00010cd0: 643a 2073 7472 2c0a 2020 2020 2020 2020  d: str,.        
-00010ce0: 2020 2020 6e6f 6465 5f6e 616d 653a 2073      node_name: s
-00010cf0: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-00010d00: 6b69 6e64 3a20 7374 7229 202d 3e20 4e6f  kind: str) -> No
-00010d10: 6e65 3a0a 2020 2020 2020 2020 7365 6c66  ne:.        self
-00010d20: 2e5f 636c 6965 6e74 203d 2063 6c69 656e  ._client = clien
-00010d30: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
-00010d40: 6461 6720 3d20 6461 670a 2020 2020 2020  dag = dag.      
-00010d50: 2020 7365 6c66 2e5f 6e6f 6465 5f69 6420    self._node_id 
-00010d60: 3d20 6e6f 6465 5f69 640a 2020 2020 2020  = node_id.      
-00010d70: 2020 7365 6c66 2e5f 6e6f 6465 5f6e 616d    self._node_nam
-00010d80: 6520 3d20 6e6f 6465 5f6e 616d 650a 2020  e = node_name.  
-00010d90: 2020 2020 2020 7365 6c66 2e5f 7479 7065        self._type
-00010da0: 203d 206b 696e 640a 2020 2020 2020 2020   = kind.        
-00010db0: 7365 6c66 2e5f 626c 6f62 733a 2044 6963  self._blobs: Dic
-00010dc0: 745b 7374 722c 2042 6c6f 6248 616e 646c  t[str, BlobHandl
-00010dd0: 655d 203d 207b 7d0a 2020 2020 2020 2020  e] = {}.        
-00010de0: 7365 6c66 2e5f 696e 7075 7473 3a20 4469  self._inputs: Di
-00010df0: 6374 5b73 7472 2c20 5475 706c 655b 7374  ct[str, Tuple[st
-00010e00: 722c 2073 7472 5d5d 203d 207b 7d0a 2020  r, str]] = {}.  
-00010e10: 2020 2020 2020 7365 6c66 2e5f 7374 6174        self._stat
-00010e20: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-00010e30: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00010e40: 7365 6c66 2e5f 636f 6e66 6967 5f65 7272  self._config_err
-00010e50: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
-00010e60: 5d20 3d20 4e6f 6e65 0a20 2020 2020 2020  ] = None.       
-00010e70: 2073 656c 662e 5f69 735f 6d6f 6465 6c3a   self._is_model:
-00010e80: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-00010e90: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-00010ea0: 656c 662e 5f76 6572 7369 6f6e 5f6f 7665  elf._version_ove
-00010eb0: 7272 6964 653a 204f 7074 696f 6e61 6c5b  rride: Optional[
-00010ec0: 7374 725d 203d 204e 6f6e 650a 0a20 2020  str] = None..   
-00010ed0: 2064 6566 2061 735f 6f77 6e65 7228 7365   def as_owner(se
-00010ee0: 6c66 2920 2d3e 2042 6c6f 624f 776e 6572  lf) -> BlobOwner
-00010ef0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00010f00: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00010f10: 6f77 6e65 725f 6461 6722 3a20 7365 6c66  owner_dag": self
-00010f20: 2e67 6574 5f64 6167 2829 2e67 6574 5f75  .get_dag().get_u
-00010f30: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
-00010f40: 2020 226f 776e 6572 5f6e 6f64 6522 3a20    "owner_node": 
-00010f50: 7365 6c66 2e67 6574 5f69 6428 292c 0a20  self.get_id(),. 
-00010f60: 2020 2020 2020 207d 0a0a 2020 2020 4073         }..    @s
-00010f70: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00010f80: 6465 6620 6672 6f6d 5f6e 6f64 655f 696e  def from_node_in
-00010f90: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
-00010fa0: 636c 6965 6e74 3a20 5859 4d45 436c 6965  client: XYMEClie
-00010fb0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-00010fc0: 6461 673a 2044 6167 4861 6e64 6c65 2c0a  dag: DagHandle,.
-00010fd0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-00010fe0: 5f69 6e66 6f3a 204e 6f64 6549 6e66 6f2c  _info: NodeInfo,
-00010ff0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-00011000: 763a 204f 7074 696f 6e61 6c5b 274e 6f64  v: Optional['Nod
-00011010: 6548 616e 646c 6527 5d29 202d 3e20 274e  eHandle']) -> 'N
-00011020: 6f64 6548 616e 646c 6527 3a0a 2020 2020  odeHandle':.    
-00011030: 2020 2020 6966 2070 7265 7620 6973 204e      if prev is N
-00011040: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00011050: 2072 6573 203d 204e 6f64 6548 616e 646c   res = NodeHandl
-00011060: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00011070: 2020 2063 6c69 656e 742c 0a20 2020 2020     client,.     
-00011080: 2020 2020 2020 2020 2020 2064 6167 2c0a             dag,.
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 6e6f 6465 5f69 6e66 6f5b 2269 6422 5d2c  node_info["id"],
-000110b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110c0: 206e 6f64 655f 696e 666f 5b22 6e61 6d65   node_info["name
-000110d0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-000110e0: 2020 2020 6e6f 6465 5f69 6e66 6f5b 2274      node_info["t
-000110f0: 7970 6522 5d29 0a20 2020 2020 2020 2065  ype"]).        e
-00011100: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00011110: 2069 6620 7072 6576 2e67 6574 5f64 6167   if prev.get_dag
-00011120: 2829 2021 3d20 6461 673a 0a20 2020 2020  () != dag:.     
-00011130: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00011140: 2056 616c 7565 4572 726f 7228 6622 7b70   ValueError(f"{p
-00011150: 7265 762e 6765 745f 6461 6728 297d 2021  rev.get_dag()} !
-00011160: 3d20 7b64 6167 7d22 290a 2020 2020 2020  = {dag}").      
-00011170: 2020 2020 2020 7265 7320 3d20 7072 6576        res = prev
-00011180: 0a20 2020 2020 2020 2072 6573 2e75 7064  .        res.upd
-00011190: 6174 655f 696e 666f 286e 6f64 655f 696e  ate_info(node_in
-000111a0: 666f 290a 2020 2020 2020 2020 7265 7475  fo).        retu
-000111b0: 726e 2072 6573 0a0a 2020 2020 6465 6620  rn res..    def 
-000111c0: 7570 6461 7465 5f69 6e66 6f28 7365 6c66  update_info(self
-000111d0: 2c20 6e6f 6465 5f69 6e66 6f3a 204e 6f64  , node_info: Nod
-000111e0: 6549 6e66 6f29 202d 3e20 4e6f 6e65 3a0a  eInfo) -> None:.
-000111f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011200: 6765 745f 6964 2829 2021 3d20 6e6f 6465  get_id() != node
-00011210: 5f69 6e66 6f5b 2269 6422 5d3a 0a20 2020  _info["id"]:.   
-00011220: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00011230: 616c 7565 4572 726f 7228 6622 7b73 656c  alueError(f"{sel
-00011240: 662e 5f6e 6f64 655f 6964 7d20 213d 207b  f._node_id} != {
-00011250: 6e6f 6465 5f69 6e66 6f5b 2769 6427 5d7d  node_info['id']}
-00011260: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00011270: 5f6e 6f64 655f 6e61 6d65 203d 206e 6f64  _node_name = nod
-00011280: 655f 696e 666f 5b22 6e61 6d65 225d 0a20  e_info["name"]. 
-00011290: 2020 2020 2020 2073 656c 662e 5f74 7970         self._typ
-000112a0: 6520 3d20 6e6f 6465 5f69 6e66 6f5b 2274  e = node_info["t
-000112b0: 7970 6522 5d0a 2020 2020 2020 2020 7365  ype"].        se
-000112c0: 6c66 2e5f 626c 6f62 7320 3d20 7b0a 2020  lf._blobs = {.  
-000112d0: 2020 2020 2020 2020 2020 6b65 793a 2042            key: B
-000112e0: 6c6f 6248 616e 646c 6528 7365 6c66 2e5f  lobHandle(self._
-000112f0: 636c 6965 6e74 2c20 7661 6c75 652c 2069  client, value, i
-00011300: 735f 6675 6c6c 3d46 616c 7365 290a 2020  s_full=False).  
-00011310: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-00011320: 6579 2c20 7661 6c75 6529 2069 6e20 6e6f  ey, value) in no
-00011330: 6465 5f69 6e66 6f5b 2262 6c6f 6273 225d  de_info["blobs"]
-00011340: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
-00011350: 207d 0a20 2020 2020 2020 2073 656c 662e   }.        self.
-00011360: 5f69 6e70 7574 7320 3d20 6e6f 6465 5f69  _inputs = node_i
-00011370: 6e66 6f5b 2269 6e70 7574 7322 5d0a 2020  nfo["inputs"].  
-00011380: 2020 2020 2020 7365 6c66 2e5f 7374 6174        self._stat
-00011390: 6520 3d20 6e6f 6465 5f69 6e66 6f5b 2273  e = node_info["s
-000113a0: 7461 7465 225d 0a20 2020 2020 2020 2073  tate"].        s
-000113b0: 656c 662e 5f63 6f6e 6669 675f 6572 726f  elf._config_erro
-000113c0: 7220 3d20 6e6f 6465 5f69 6e66 6f5b 2263  r = node_info["c
-000113d0: 6f6e 6669 675f 6572 726f 7222 5d0a 2020  onfig_error"].  
-000113e0: 2020 2020 2020 7365 6c66 2e5f 7665 7273        self._vers
-000113f0: 696f 6e5f 6f76 6572 7269 6465 203d 206e  ion_override = n
-00011400: 6f64 655f 696e 666f 5b22 7665 7273 696f  ode_info["versio
-00011410: 6e5f 6f76 6572 7269 6465 225d 0a0a 2020  n_override"]..  
-00011420: 2020 6465 6620 6765 745f 6461 6728 7365    def get_dag(se
-00011430: 6c66 2920 2d3e 2044 6167 4861 6e64 6c65  lf) -> DagHandle
-00011440: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00011450: 2073 656c 662e 5f64 6167 0a0a 2020 2020   self._dag..    
-00011460: 6465 6620 6765 745f 6964 2873 656c 6629  def get_id(self)
-00011470: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00011480: 2072 6574 7572 6e20 7365 6c66 2e5f 6e6f   return self._no
-00011490: 6465 5f69 640a 0a20 2020 2064 6566 2067  de_id..    def g
-000114a0: 6574 5f6e 616d 6528 7365 6c66 2920 2d3e  et_name(self) ->
-000114b0: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
-000114c0: 7475 726e 2073 656c 662e 5f6e 6f64 655f  turn self._node_
-000114d0: 6e61 6d65 0a0a 2020 2020 6465 6620 6765  name..    def ge
-000114e0: 745f 7479 7065 2873 656c 6629 202d 3e20  t_type(self) -> 
-000114f0: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
-00011500: 7572 6e20 7365 6c66 2e5f 7479 7065 0a0a  urn self._type..
-00011510: 2020 2020 6465 6620 6765 745f 6e6f 6465      def get_node
-00011520: 5f64 6566 2873 656c 6629 202d 3e20 4e6f  _def(self) -> No
-00011530: 6465 4465 6649 6e66 6f3a 0a20 2020 2020  deDefInfo:.     
-00011540: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00011550: 636c 6965 6e74 2e67 6574 5f6e 6f64 655f  client.get_node_
-00011560: 6465 6673 2829 5b73 656c 662e 6765 745f  defs()[self.get_
-00011570: 7479 7065 2829 5d0a 0a20 2020 2064 6566  type()]..    def
-00011580: 2067 6574 5f69 6e70 7574 7328 7365 6c66   get_inputs(self
-00011590: 2920 2d3e 2053 6574 5b73 7472 5d3a 0a20  ) -> Set[str]:. 
-000115a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000115b0: 7428 7365 6c66 2e5f 696e 7075 7473 2e6b  t(self._inputs.k
-000115c0: 6579 7328 2929 0a0a 2020 2020 6465 6620  eys())..    def 
-000115d0: 6765 745f 696e 7075 7428 7365 6c66 2c20  get_input(self, 
-000115e0: 6b65 793a 2073 7472 2920 2d3e 2054 7570  key: str) -> Tup
-000115f0: 6c65 5b27 4e6f 6465 4861 6e64 6c65 272c  le['NodeHandle',
-00011600: 2073 7472 5d3a 0a20 2020 2020 2020 206e   str]:.        n
-00011610: 6f64 655f 6964 2c20 6f75 745f 6b65 7920  ode_id, out_key 
-00011620: 3d20 7365 6c66 2e5f 696e 7075 7473 5b6b  = self._inputs[k
-00011630: 6579 5d0a 2020 2020 2020 2020 7265 7475  ey].        retu
-00011640: 726e 2073 656c 662e 6765 745f 6461 6728  rn self.get_dag(
-00011650: 292e 6765 745f 6e6f 6465 286e 6f64 655f  ).get_node(node_
-00011660: 6964 292c 206f 7574 5f6b 6579 0a0a 2020  id), out_key..  
-00011670: 2020 6465 6620 6765 745f 7374 6174 7573    def get_status
-00011680: 2873 656c 6629 202d 3e20 5461 736b 5374  (self) -> TaskSt
-00011690: 6174 7573 3a0a 2020 2020 2020 2020 7265  atus:.        re
-000116a0: 7475 726e 2063 6173 7428 4e6f 6465 5374  turn cast(NodeSt
-000116b0: 6174 7573 2c20 7365 6c66 2e5f 636c 6965  atus, self._clie
-000116c0: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-000116d0: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-000116e0: 484f 445f 4745 542c 2022 2f6e 6f64 655f  HOD_GET, "/node_
-000116f0: 7374 6174 7573 222c 207b 0a20 2020 2020  status", {.     
-00011700: 2020 2020 2020 2020 2020 2022 6461 6722             "dag"
-00011710: 3a20 7365 6c66 2e67 6574 5f64 6167 2829  : self.get_dag()
-00011720: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
-00011730: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
-00011740: 6522 3a20 7365 6c66 2e67 6574 5f69 6428  e": self.get_id(
-00011750: 292c 0a20 2020 2020 2020 2020 2020 207d  ),.            }
-00011760: 2929 5b22 7374 6174 7573 225d 0a0a 2020  ))["status"]..  
-00011770: 2020 6465 6620 6861 735f 636f 6e66 6967    def has_config
-00011780: 5f65 7272 6f72 2873 656c 6629 202d 3e20  _error(self) -> 
-00011790: 626f 6f6c 3a0a 2020 2020 2020 2020 7265  bool:.        re
-000117a0: 7475 726e 2073 656c 662e 5f63 6f6e 6669  turn self._confi
-000117b0: 675f 6572 726f 7220 6973 206e 6f74 204e  g_error is not N
-000117c0: 6f6e 650a 0a20 2020 2064 6566 2067 6574  one..    def get
-000117d0: 5f63 6f6e 6669 675f 6572 726f 7228 7365  _config_error(se
-000117e0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-000117f0: 7374 725d 3a0a 2020 2020 2020 2020 7265  str]:.        re
-00011800: 7475 726e 2073 656c 662e 5f63 6f6e 6669  turn self._confi
-00011810: 675f 6572 726f 720a 0a20 2020 2064 6566  g_error..    def
-00011820: 2067 6574 5f76 6572 7369 6f6e 5f6f 7665   get_version_ove
-00011830: 7272 6964 6528 7365 6c66 2920 2d3e 204f  rride(self) -> O
-00011840: 7074 696f 6e61 6c5b 7374 725d 3a0a 2020  ptional[str]:.  
-00011850: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00011860: 662e 5f76 6572 7369 6f6e 5f6f 7665 7272  f._version_overr
-00011870: 6964 650a 0a20 2020 2064 6566 2067 6574  ide..    def get
-00011880: 5f62 6c6f 6273 2873 656c 6629 202d 3e20  _blobs(self) -> 
-00011890: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
-000118a0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-000118b0: 2873 656c 662e 5f62 6c6f 6273 2e6b 6579  (self._blobs.key
-000118c0: 7328 2929 0a0a 2020 2020 6465 6620 6765  s())..    def ge
-000118d0: 745f 626c 6f62 5f68 616e 646c 6573 2873  t_blob_handles(s
-000118e0: 656c 6629 202d 3e20 4469 6374 5b73 7472  elf) -> Dict[str
-000118f0: 2c20 2742 6c6f 6248 616e 646c 6527 5d3a  , 'BlobHandle']:
-00011900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011910: 7365 6c66 2e5f 626c 6f62 730a 0a20 2020  self._blobs..   
-00011920: 2064 6566 2067 6574 5f62 6c6f 625f 6861   def get_blob_ha
-00011930: 6e64 6c65 2873 656c 662c 206b 6579 3a20  ndle(self, key: 
-00011940: 7374 7229 202d 3e20 2742 6c6f 6248 616e  str) -> 'BlobHan
-00011950: 646c 6527 3a0a 2020 2020 2020 2020 7265  dle':.        re
-00011960: 7475 726e 2073 656c 662e 5f62 6c6f 6273  turn self._blobs
-00011970: 5b6b 6579 5d0a 0a20 2020 2064 6566 2073  [key]..    def s
-00011980: 6574 5f62 6c6f 625f 7572 6928 7365 6c66  et_blob_uri(self
-00011990: 2c20 6b65 793a 2073 7472 2c20 626c 6f62  , key: str, blob
-000119a0: 5f75 7269 3a20 7374 7229 202d 3e20 7374  _uri: str) -> st
-000119b0: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-000119c0: 6e20 6361 7374 2850 7574 4e6f 6465 426c  n cast(PutNodeBl
-000119d0: 6f62 2c20 7365 6c66 2e5f 636c 6965 6e74  ob, self._client
-000119e0: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
-000119f0: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
-00011a00: 445f 5055 542c 2022 2f6e 6f64 655f 626c  D_PUT, "/node_bl
-00011a10: 6f62 222c 207b 0a20 2020 2020 2020 2020  ob", {.         
-00011a20: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
-00011a30: 6c66 2e67 6574 5f64 6167 2829 2e67 6574  lf.get_dag().get
-00011a40: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
-00011a50: 2020 2020 2020 2020 226e 6f64 6522 3a20          "node": 
-00011a60: 7365 6c66 2e67 6574 5f69 6428 292c 0a20  self.get_id(),. 
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011a80: 626c 6f62 5f6b 6579 223a 206b 6579 2c0a  blob_key": key,.
-00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011aa0: 2262 6c6f 625f 7572 6922 3a20 626c 6f62  "blob_uri": blob
-00011ab0: 5f75 7269 2c0a 2020 2020 2020 2020 2020  _uri,.          
-00011ac0: 2020 7d29 295b 226e 6577 5f75 7269 225d    }))["new_uri"]
-00011ad0: 0a0a 2020 2020 6465 6620 6765 745f 696e  ..    def get_in
-00011ae0: 5f63 7572 736f 725f 7374 6174 6573 2873  _cursor_states(s
-00011af0: 656c 6629 202d 3e20 4469 6374 5b73 7472  elf) -> Dict[str
-00011b00: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
-00011b10: 7265 7475 726e 2063 6173 7428 496e 4375  return cast(InCu
-00011b20: 7273 6f72 732c 2073 656c 662e 5f63 6c69  rsors, self._cli
-00011b30: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-00011b40: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-00011b50: 5448 4f44 5f47 4554 2c20 222f 6e6f 6465  THOD_GET, "/node
-00011b60: 5f69 6e5f 6375 7273 6f72 7322 2c20 7b0a  _in_cursors", {.
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 2264 6167 223a 2073 656c 662e 6765 745f  "dag": self.get_
-00011b90: 6461 6728 292e 6765 745f 7572 6928 292c  dag().get_uri(),
-00011ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011bb0: 2022 6e6f 6465 223a 2073 656c 662e 6765   "node": self.ge
-00011bc0: 745f 6964 2829 2c0a 2020 2020 2020 2020  t_id(),.        
-00011bd0: 2020 2020 7d29 295b 2263 7572 736f 7273      }))["cursors
-00011be0: 225d 0a0a 2020 2020 6465 6620 6765 745f  "]..    def get_
-00011bf0: 6869 6768 6573 745f 6368 756e 6b28 7365  highest_chunk(se
-00011c00: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00011c10: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
-00011c20: 4e6f 6465 4368 756e 6b2c 2073 656c 662e  NodeChunk, self.
-00011c30: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
-00011c40: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
-00011c50: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
-00011c60: 6e6f 6465 5f63 6875 6e6b 222c 207b 0a20  node_chunk", {. 
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011c80: 6461 6722 3a20 7365 6c66 2e67 6574 5f64  dag": self.get_d
-00011c90: 6167 2829 2e67 6574 5f75 7269 2829 2c0a  ag().get_uri(),.
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 226e 6f64 6522 3a20 7365 6c66 2e67 6574  "node": self.get
-00011cc0: 5f69 6428 292c 0a20 2020 2020 2020 2020  _id(),.         
-00011cd0: 2020 207d 2929 5b22 6368 756e 6b22 5d0a     }))["chunk"].
-00011ce0: 0a20 2020 2064 6566 2067 6574 5f73 686f  .    def get_sho
-00011cf0: 7274 5f73 7461 7475 7328 7365 6c66 2c20  rt_status(self, 
-00011d00: 616c 6c6f 775f 756e 6963 6f64 653a 2062  allow_unicode: b
-00011d10: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2073  ool = True) -> s
-00011d20: 7472 3a0a 2020 2020 2020 2020 7374 6174  tr:.        stat
-00011d30: 7573 5f6d 6170 3a20 4469 6374 5b54 6173  us_map: Dict[Tas
-00011d40: 6b53 7461 7475 732c 2073 7472 5d20 3d20  kStatus, str] = 
-00011d50: 7b0a 2020 2020 2020 2020 2020 2020 2262  {.            "b
-00011d60: 6c6f 636b 6564 223a 2022 4222 2c0a 2020  locked": "B",.  
-00011d70: 2020 2020 2020 2020 2020 2277 6169 7469            "waiti
-00011d80: 6e67 223a 2022 5722 2c0a 2020 2020 2020  ng": "W",.      
-00011d90: 2020 2020 2020 2272 756e 6e69 6e67 223a        "running":
-00011da0: 2022 e286 9222 2069 6620 616c 6c6f 775f   "..." if allow_
-00011db0: 756e 6963 6f64 6520 656c 7365 2022 5222  unicode else "R"
-00011dc0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
-00011dd0: 6f6d 706c 6574 6522 3a20 22e2 9c93 2220  omplete": "..." 
-00011de0: 6966 2061 6c6c 6f77 5f75 6e69 636f 6465  if allow_unicode
-00011df0: 2065 6c73 6520 2243 222c 0a20 2020 2020   else "C",.     
-00011e00: 2020 2020 2020 2022 656f 7322 3a20 2258         "eos": "X
-00011e10: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00011e20: 7061 7573 6564 223a 2022 5022 2c0a 2020  paused": "P",.  
-00011e30: 2020 2020 2020 2020 2020 2265 7272 6f72            "error
-00011e40: 223a 2022 2122 2c0a 2020 2020 2020 2020  ": "!",.        
-00011e50: 2020 2020 2275 6e6b 6e6f 776e 223a 2022      "unknown": "
-00011e60: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
-00011e70: 2276 6972 7475 616c 223a 2022 e288 b422  "virtual": "..."
-00011e80: 2069 6620 616c 6c6f 775f 756e 6963 6f64   if allow_unicod
-00011e90: 6520 656c 7365 2022 5622 2c0a 2020 2020  e else "V",.    
-00011ea0: 2020 2020 2020 2020 2271 7565 7565 223a          "queue":
-00011eb0: 2022 3d22 2c0a 2020 2020 2020 2020 7d0a   "=",.        }.
-00011ec0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00011ed0: 7461 7475 735f 6d61 705b 7365 6c66 2e67  tatus_map[self.g
-00011ee0: 6574 5f73 7461 7475 7328 295d 0a0a 2020  et_status()]..  
-00011ef0: 2020 6465 6620 6765 745f 6c6f 6773 2873    def get_logs(s
-00011f00: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-00011f10: 2020 2020 2077 6974 6820 7365 6c66 2e5f       with self._
-00011f20: 636c 6965 6e74 2e5f 7261 775f 7265 7175  client._raw_requ
-00011f30: 6573 745f 7374 7228 0a20 2020 2020 2020  est_str(.       
-00011f40: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-00011f50: 4745 542c 2022 2f6e 6f64 655f 6c6f 6773  GET, "/node_logs
-00011f60: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
-00011f70: 2020 2020 2020 2020 2022 6461 6722 3a20           "dag": 
-00011f80: 7365 6c66 2e67 6574 5f64 6167 2829 2e67  self.get_dag().g
-00011f90: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00011fb0: 6f64 6522 3a20 7365 6c66 2e67 6574 5f69  ode": self.get_i
-00011fc0: 6428 292c 0a20 2020 2020 2020 2020 2020  d(),.           
-00011fd0: 2020 2020 207d 2920 6173 2066 696e 3a0a       }) as fin:.
-00011fe0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011ff0: 726e 2066 696e 2e72 6561 6428 290a 0a20  rn fin.read().. 
-00012000: 2020 2064 6566 2067 6574 5f74 696d 696e     def get_timin
-00012010: 6728 7365 6c66 2920 2d3e 204c 6973 745b  g(self) -> List[
-00012020: 5469 6d69 6e67 5d3a 0a20 2020 2020 2020  Timing]:.       
-00012030: 2072 6574 7572 6e20 6361 7374 2854 696d   return cast(Tim
-00012040: 696e 6773 2c20 7365 6c66 2e5f 636c 6965  ings, self._clie
-00012050: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-00012060: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00012070: 484f 445f 4745 542c 2022 2f6e 6f64 655f  HOD_GET, "/node_
-00012080: 7065 7266 222c 207b 0a20 2020 2020 2020  perf", {.       
-00012090: 2020 2020 2020 2020 2022 6461 6722 3a20           "dag": 
-000120a0: 7365 6c66 2e67 6574 5f64 6167 2829 2e67  self.get_dag().g
-000120b0: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
-000120c0: 2020 2020 2020 2020 2020 226e 6f64 6522            "node"
-000120d0: 3a20 7365 6c66 2e67 6574 5f69 6428 292c  : self.get_id(),
-000120e0: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
-000120f0: 5b22 7469 6d65 7322 5d0a 0a20 2020 2064  ["times"]..    d
-00012100: 6566 2072 6561 645f 626c 6f62 280a 2020  ef read_blob(.  
-00012110: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-00012120: 2020 2020 2020 2020 2020 2020 6b65 793a              key:
-00012130: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00012140: 2020 6368 756e 6b3a 204f 7074 696f 6e61    chunk: Optiona
-00012150: 6c5b 696e 745d 2c0a 2020 2020 2020 2020  l[int],.        
-00012160: 2020 2020 666f 7263 655f 7265 6672 6573      force_refres
-00012170: 683a 2062 6f6f 6c29 202d 3e20 2742 6c6f  h: bool) -> 'Blo
-00012180: 6248 616e 646c 6527 3a0a 2020 2020 2020  bHandle':.      
-00012190: 2020 2320 4649 584d 453a 2021 2121 2121    # FIXME: !!!!!
-000121a0: 2120 6578 706c 6963 6974 6c79 2072 6570  ! explicitly rep
-000121b0: 6561 7420 6f6e 2074 696d 656f 7574 0a20  eat on timeout. 
-000121c0: 2020 2020 2020 2064 6167 203d 2073 656c         dag = sel
-000121d0: 662e 6765 745f 6461 6728 290a 2020 2020  f.get_dag().    
-000121e0: 2020 2020 7265 7320 3d20 6361 7374 2852      res = cast(R
-000121f0: 6561 644e 6f64 652c 2073 656c 662e 5f63  eadNode, self._c
-00012200: 6c69 656e 742e 7265 7175 6573 745f 6a73  lient.request_js
-00012210: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00012220: 4d45 5448 4f44 5f50 4f53 542c 2022 2f72  METHOD_POST, "/r
-00012230: 6561 645f 6e6f 6465 222c 207b 0a20 2020  ead_node", {.   
-00012240: 2020 2020 2020 2020 2020 2020 2022 6461               "da
-00012250: 6722 3a20 6461 672e 6765 745f 7572 6928  g": dag.get_uri(
-00012260: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00012270: 2020 2022 6e6f 6465 223a 2073 656c 662e     "node": self.
-00012280: 6765 745f 6964 2829 2c0a 2020 2020 2020  get_id(),.      
-00012290: 2020 2020 2020 2020 2020 226b 6579 223a            "key":
-000122a0: 206b 6579 2c0a 2020 2020 2020 2020 2020   key,.          
-000122b0: 2020 2020 2020 2263 6875 6e6b 223a 2063        "chunk": c
-000122c0: 6875 6e6b 2c0a 2020 2020 2020 2020 2020  hunk,.          
-000122d0: 2020 2020 2020 2269 735f 626c 6f63 6b69        "is_blocki
-000122e0: 6e67 223a 2054 7275 652c 0a20 2020 2020  ng": True,.     
-000122f0: 2020 2020 2020 2020 2020 2022 666f 7263             "forc
-00012300: 655f 7265 6672 6573 6822 3a20 666f 7263  e_refresh": forc
-00012310: 655f 7265 6672 6573 682c 0a20 2020 2020  e_refresh,.     
-00012320: 2020 2020 2020 207d 2929 0a20 2020 2020         })).     
-00012330: 2020 2075 7269 203d 2072 6573 5b22 7265     uri = res["re
-00012340: 7375 6c74 5f75 7269 225d 0a20 2020 2020  sult_uri"].     
-00012350: 2020 2069 6620 7572 6920 6973 204e 6f6e     if uri is Non
-00012360: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00012370: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00012380: 6622 7572 6920 6973 204e 6f6e 653a 207b  f"uri is None: {
-00012390: 7265 737d 2229 0a20 2020 2020 2020 2072  res}").        r
-000123a0: 6574 7572 6e20 426c 6f62 4861 6e64 6c65  eturn BlobHandle
-000123b0: 2873 656c 662e 5f63 6c69 656e 742c 2075  (self._client, u
-000123c0: 7269 2c20 6973 5f66 756c 6c3d 5472 7565  ri, is_full=True
-000123d0: 290a 0a20 2020 2064 6566 2067 6574 5f69  )..    def get_i
-000123e0: 6e64 6578 5f63 6f6c 2873 656c 6629 202d  ndex_col(self) -
-000123f0: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
-00012400: 6574 7572 6e20 225f 696e 6465 7822 2069  eturn "_index" i
-00012410: 6620 7365 6c66 2e5f 636c 6965 6e74 2e68  f self._client.h
-00012420: 6173 5f76 6572 7369 6f6e 2834 2c20 3129  as_version(4, 1)
-00012430: 2065 6c73 6520 2269 6e64 6578 220a 0a20   else "index".. 
-00012440: 2020 2064 6566 2067 6574 5f72 6f77 5f69     def get_row_i
-00012450: 645f 636f 6c28 7365 6c66 2920 2d3e 2073  d_col(self) -> s
-00012460: 7472 3a0a 2020 2020 2020 2020 7265 7475  tr:.        retu
-00012470: 726e 2022 5f72 6f77 5f69 6422 2069 6620  rn "_row_id" if 
-00012480: 7365 6c66 2e5f 636c 6965 6e74 2e68 6173  self._client.has
-00012490: 5f76 6572 7369 6f6e 2834 2c20 3129 2065  _version(4, 1) e
-000124a0: 6c73 6520 2272 6f77 5f69 6422 0a0a 2020  lse "row_id"..  
-000124b0: 2020 6465 6620 7265 6164 280a 2020 2020    def read(.    
-000124c0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000124d0: 2020 2020 2020 2020 2020 6b65 793a 2073            key: s
-000124e0: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-000124f0: 6368 756e 6b3a 204f 7074 696f 6e61 6c5b  chunk: Optional[
-00012500: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
-00012510: 2020 666f 7263 655f 7265 6672 6573 683a    force_refresh:
-00012520: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00012530: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-00012540: 725f 6964 3a20 626f 6f6c 203d 2054 7275  r_id: bool = Tru
-00012550: 6529 202d 3e20 4f70 7469 6f6e 616c 5b42  e) -> Optional[B
-00012560: 7974 6552 6573 706f 6e73 655d 3a0a 2020  yteResponse]:.  
-00012570: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00012580: 7365 6c66 2e72 6561 645f 626c 6f62 286b  self.read_blob(k
-00012590: 6579 2c20 6368 756e 6b2c 2066 6f72 6365  ey, chunk, force
-000125a0: 5f72 6566 7265 7368 292e 6765 745f 636f  _refresh).get_co
-000125b0: 6e74 656e 7428 290a 2020 2020 2020 2020  ntent().        
-000125c0: 6966 2066 696c 7465 725f 6964 2061 6e64  if filter_id and
-000125d0: 2069 7369 6e73 7461 6e63 6528 636f 6e74   isinstance(cont
-000125e0: 656e 742c 2070 642e 4461 7461 4672 616d  ent, pd.DataFram
-000125f0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00012600: 6466 3a20 7064 2e44 6174 6146 7261 6d65  df: pd.DataFrame
-00012610: 203d 2063 6f6e 7465 6e74 0a20 2020 2020   = content.     
-00012620: 2020 2020 2020 2064 6620 3d20 6466 5b64         df = df[d
-00012630: 665b 7365 6c66 2e67 6574 5f72 6f77 5f69  f[self.get_row_i
-00012640: 645f 636f 6c28 295d 203e 3d20 305d 0a20  d_col()] >= 0]. 
-00012650: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-00012660: 6466 2e73 6574 5f69 6e64 6578 2873 656c  df.set_index(sel
-00012670: 662e 6765 745f 696e 6465 785f 636f 6c28  f.get_index_col(
-00012680: 292c 2064 726f 703d 5472 7565 290a 2020  ), drop=True).  
-00012690: 2020 2020 2020 2020 2020 6466 2e69 6e64            df.ind
-000126a0: 6578 2e6e 616d 6520 3d20 4e6f 6e65 0a20  ex.name = None. 
-000126b0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-000126c0: 6e74 203d 2064 662e 636f 7079 2829 0a20  nt = df.copy(). 
-000126d0: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-000126e0: 6e74 656e 740a 0a20 2020 2064 6566 2072  ntent..    def r
-000126f0: 6561 645f 616c 6c28 0a20 2020 2020 2020  ead_all(.       
-00012700: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00012710: 2020 2020 2020 206b 6579 3a20 7374 722c         key: str,
-00012720: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00012730: 6365 5f72 6566 7265 7368 3a20 626f 6f6c  ce_refresh: bool
-00012740: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00012750: 2020 2020 2020 6669 6c74 6572 5f69 643a        filter_id:
-00012760: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
-00012770: 204f 7074 696f 6e61 6c5b 4279 7465 5265   Optional[ByteRe
-00012780: 7370 6f6e 7365 5d3a 0a20 2020 2020 2020  sponse]:.       
-00012790: 2073 656c 662e 7265 6164 280a 2020 2020   self.read(.    
-000127a0: 2020 2020 2020 2020 6b65 792c 2063 6875          key, chu
-000127b0: 6e6b 3d4e 6f6e 652c 2066 6f72 6365 5f72  nk=None, force_r
-000127c0: 6566 7265 7368 3d66 6f72 6365 5f72 6566  efresh=force_ref
-000127d0: 7265 7368 2c20 6669 6c74 6572 5f69 643d  resh, filter_id=
-000127e0: 4661 6c73 6529 0a20 2020 2020 2020 2072  False).        r
-000127f0: 6573 3a20 4c69 7374 5b42 7974 6552 6573  es: List[ByteRes
-00012800: 706f 6e73 655d 203d 205b 5d0a 2020 2020  ponse] = [].    
-00012810: 2020 2020 6374 7970 653a 204f 7074 696f      ctype: Optio
-00012820: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00012830: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-00012840: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00012850: 626c 6f62 203d 2073 656c 662e 7265 6164  blob = self.read
-00012860: 5f62 6c6f 6228 6b65 792c 2063 6875 6e6b  _blob(key, chunk
-00012870: 3d6c 656e 2872 6573 292c 2066 6f72 6365  =len(res), force
-00012880: 5f72 6566 7265 7368 3d46 616c 7365 290a  _refresh=False).
-00012890: 2020 2020 2020 2020 2020 2020 6375 7220              cur 
-000128a0: 3d20 626c 6f62 2e67 6574 5f63 6f6e 7465  = blob.get_conte
-000128b0: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
-000128c0: 2069 6620 6375 7220 6973 204e 6f6e 653a   if cur is None:
-000128d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128e0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-000128f0: 2020 2063 7572 5f63 7479 7065 203d 2062     cur_ctype = b
-00012900: 6c6f 622e 6765 745f 6374 7970 6528 290a  lob.get_ctype().
-00012910: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00012920: 7479 7065 2069 7320 4e6f 6e65 3a0a 2020  type is None:.  
-00012930: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-00012940: 7970 6520 3d20 6375 725f 6374 7970 650a  ype = cur_ctype.
-00012950: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00012960: 2063 7479 7065 2021 3d20 6375 725f 6374   ctype != cur_ct
-00012970: 7970 653a 0a20 2020 2020 2020 2020 2020  ype:.           
-00012980: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00012990: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000129a0: 2020 2020 2020 2020 2020 2066 2269 6e63             f"inc
-000129b0: 6f6e 7369 7374 656e 7420 7265 7475 726e  onsistent return
-000129c0: 2074 7970 6573 207b 6374 7970 657d 2021   types {ctype} !
-000129d0: 3d20 7b63 7572 5f63 7479 7065 7d22 290a  = {cur_ctype}").
-000129e0: 2020 2020 2020 2020 2020 2020 7265 732e              res.
-000129f0: 6170 7065 6e64 2863 7572 290a 2020 2020  append(cur).    
-00012a00: 2020 2020 6966 206e 6f74 2072 6573 206f      if not res o
-00012a10: 7220 6374 7970 6520 6973 204e 6f6e 653a  r ctype is None:
-00012a20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00012a30: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-00012a40: 2063 6f6e 7465 6e74 203d 206d 6572 6765   content = merge
-00012a50: 5f63 7479 7065 2872 6573 2c20 6374 7970  _ctype(res, ctyp
-00012a60: 6529 0a20 2020 2020 2020 2069 6620 6669  e).        if fi
-00012a70: 6c74 6572 5f69 6420 616e 6420 6973 696e  lter_id and isin
-00012a80: 7374 616e 6365 2863 6f6e 7465 6e74 2c20  stance(content, 
-00012a90: 7064 2e44 6174 6146 7261 6d65 293a 0a20  pd.DataFrame):. 
-00012aa0: 2020 2020 2020 2020 2020 2064 663a 2070             df: p
-00012ab0: 642e 4461 7461 4672 616d 6520 3d20 636f  d.DataFrame = co
-00012ac0: 6e74 656e 740a 2020 2020 2020 2020 2020  ntent.          
-00012ad0: 2020 6466 203d 2064 665b 6466 5b73 656c    df = df[df[sel
-00012ae0: 662e 6765 745f 726f 775f 6964 5f63 6f6c  f.get_row_id_col
-00012af0: 2829 5d20 3e3d 2030 5d0a 2020 2020 2020  ()] >= 0].      
-00012b00: 2020 2020 2020 6466 203d 2064 662e 7365        df = df.se
-00012b10: 745f 696e 6465 7828 7365 6c66 2e67 6574  t_index(self.get
-00012b20: 5f69 6e64 6578 5f63 6f6c 2829 2c20 6472  _index_col(), dr
-00012b30: 6f70 3d54 7275 6529 0a20 2020 2020 2020  op=True).       
-00012b40: 2020 2020 2064 662e 696e 6465 782e 6e61       df.index.na
-00012b50: 6d65 203d 204e 6f6e 650a 2020 2020 2020  me = None.      
-00012b60: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00012b70: 6466 2e63 6f70 7928 290a 2020 2020 2020  df.copy().      
-00012b80: 2020 7265 7475 726e 2063 6f6e 7465 6e74    return content
-00012b90: 0a0a 2020 2020 6465 6620 636c 6561 7228  ..    def clear(
-00012ba0: 7365 6c66 2920 2d3e 204e 6f64 6553 7461  self) -> NodeSta
-00012bb0: 7465 3a0a 2020 2020 2020 2020 7265 7475  te:.        retu
-00012bc0: 726e 2063 6173 7428 4e6f 6465 5374 6174  rn cast(NodeStat
-00012bd0: 652c 2073 656c 662e 5f63 6c69 656e 742e  e, self._client.
-00012be0: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
-00012bf0: 2020 2020 2020 2020 2020 4d45 5448 4f44            METHOD
-00012c00: 5f50 5554 2c20 222f 6e6f 6465 5f73 7461  _PUT, "/node_sta
-00012c10: 7465 222c 207b 0a20 2020 2020 2020 2020  te", {.         
-00012c20: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
-00012c30: 6c66 2e67 6574 5f64 6167 2829 2e67 6574  lf.get_dag().get
-00012c40: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
-00012c50: 2020 2020 2020 2020 226e 6f64 6522 3a20          "node": 
-00012c60: 7365 6c66 2e67 6574 5f69 6428 292c 0a20  self.get_id(),. 
-00012c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012c80: 6163 7469 6f6e 223a 2022 7265 7365 7422  action": "reset"
-00012c90: 2c0a 2020 2020 2020 2020 2020 2020 7d29  ,.            })
-00012ca0: 290a 0a20 2020 2064 6566 2072 6571 7565  )..    def reque
-00012cb0: 7565 2873 656c 6629 202d 3e20 4e6f 6465  ue(self) -> Node
-00012cc0: 5374 6174 653a 0a20 2020 2020 2020 2072  State:.        r
-00012cd0: 6574 7572 6e20 6361 7374 284e 6f64 6553  eturn cast(NodeS
-00012ce0: 7461 7465 2c20 7365 6c66 2e5f 636c 6965  tate, self._clie
-00012cf0: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-00012d00: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00012d10: 484f 445f 5055 542c 2022 2f6e 6f64 655f  HOD_PUT, "/node_
-00012d20: 7374 6174 6522 2c20 7b0a 2020 2020 2020  state", {.      
-00012d30: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
-00012d40: 2073 656c 662e 6765 745f 6461 6728 292e   self.get_dag().
-00012d50: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
-00012d60: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
-00012d70: 223a 2073 656c 662e 6765 745f 6964 2829  ": self.get_id()
-00012d80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012d90: 2020 2261 6374 696f 6e22 3a20 2272 6571    "action": "req
-00012da0: 7565 7565 222c 0a20 2020 2020 2020 2020  ueue",.         
-00012db0: 2020 207d 2929 0a0a 2020 2020 6465 6620     }))..    def 
-00012dc0: 6669 785f 6572 726f 7228 7365 6c66 2920  fix_error(self) 
-00012dd0: 2d3e 204e 6f64 6553 7461 7465 3a0a 2020  -> NodeState:.  
-00012de0: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
-00012df0: 7428 4e6f 6465 5374 6174 652c 2073 656c  t(NodeState, sel
-00012e00: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
-00012e10: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
-00012e20: 2020 2020 4d45 5448 4f44 5f50 5554 2c20      METHOD_PUT, 
-00012e30: 222f 6e6f 6465 5f73 7461 7465 222c 207b  "/node_state", {
-00012e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e50: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
-00012e60: 5f64 6167 2829 2e67 6574 5f75 7269 2829  _dag().get_uri()
-00012e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012e80: 2020 226e 6f64 6522 3a20 7365 6c66 2e67    "node": self.g
-00012e90: 6574 5f69 6428 292c 0a20 2020 2020 2020  et_id(),.       
-00012ea0: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
-00012eb0: 223a 2022 6669 785f 6572 726f 7222 2c0a  ": "fix_error",.
-00012ec0: 2020 2020 2020 2020 2020 2020 7d29 290a              })).
-00012ed0: 0a20 2020 2064 6566 2067 6574 5f62 6c6f  .    def get_blo
-00012ee0: 625f 7572 6928 0a20 2020 2020 2020 2020  b_uri(.         
-00012ef0: 2020 2073 656c 662c 2062 6c6f 625f 6b65     self, blob_ke
-00012f00: 793a 2073 7472 2c20 626c 6f62 5f74 7970  y: str, blob_typ
-00012f10: 653a 2073 7472 2920 2d3e 2054 7570 6c65  e: str) -> Tuple
-00012f20: 5b73 7472 2c20 426c 6f62 4f77 6e65 725d  [str, BlobOwner]
-00012f30: 3a0a 2020 2020 2020 2020 7265 7320 3d20  :.        res = 
-00012f40: 6361 7374 2842 6c6f 6255 5249 5265 7370  cast(BlobURIResp
-00012f50: 6f6e 7365 2c20 7365 6c66 2e5f 636c 6965  onse, self._clie
-00012f60: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-00012f70: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00012f80: 484f 445f 4745 542c 2022 2f62 6c6f 625f  HOD_GET, "/blob_
-00012f90: 7572 6922 2c20 7b0a 2020 2020 2020 2020  uri", {.        
-00012fa0: 2020 2020 2020 2020 2264 6167 223a 2073          "dag": s
-00012fb0: 656c 662e 6765 745f 6461 6728 292e 6765  elf.get_dag().ge
-00012fc0: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
-00012fd0: 2020 2020 2020 2020 2022 6e6f 6465 223a           "node":
-00012fe0: 2073 656c 662e 6765 745f 6964 2829 2c0a   self.get_id(),.
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 226b 6579 223a 2062 6c6f 625f 6b65 792c  "key": blob_key,
-00013010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013020: 2022 7479 7065 223a 2062 6c6f 625f 7479   "type": blob_ty
-00013030: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00013040: 7d29 290a 2020 2020 2020 2020 7265 7475  })).        retu
-00013050: 726e 2072 6573 5b22 7572 6922 5d2c 2072  rn res["uri"], r
-00013060: 6573 5b22 6f77 6e65 7222 5d0a 0a20 2020  es["owner"]..   
-00013070: 2064 6566 2067 6574 5f63 7376 5f62 6c6f   def get_csv_blo
-00013080: 6228 7365 6c66 2c20 6b65 793a 2073 7472  b(self, key: str
-00013090: 203d 2022 6f72 6967 2229 202d 3e20 2743   = "orig") -> 'C
-000130a0: 5356 426c 6f62 4861 6e64 6c65 273a 0a20  SVBlobHandle':. 
-000130b0: 2020 2020 2020 2075 7269 2c20 6f77 6e65         uri, owne
-000130c0: 7220 3d20 7365 6c66 2e67 6574 5f62 6c6f  r = self.get_blo
-000130d0: 625f 7572 6928 6b65 792c 2022 6373 7622  b_uri(key, "csv"
-000130e0: 290a 2020 2020 2020 2020 626c 6f62 203d  ).        blob =
-000130f0: 2043 5356 426c 6f62 4861 6e64 6c65 2873   CSVBlobHandle(s
-00013100: 656c 662e 5f63 6c69 656e 742c 2075 7269  elf._client, uri
-00013110: 2c20 6973 5f66 756c 6c3d 4661 6c73 6529  , is_full=False)
-00013120: 0a20 2020 2020 2020 2062 6c6f 622e 7365  .        blob.se
-00013130: 745f 6c6f 6361 6c5f 6f77 6e65 7228 6f77  t_local_owner(ow
-00013140: 6e65 7229 0a20 2020 2020 2020 2072 6574  ner).        ret
-00013150: 7572 6e20 626c 6f62 0a0a 2020 2020 6465  urn blob..    de
-00013160: 6620 6765 745f 746f 7263 685f 626c 6f62  f get_torch_blob
-00013170: 2873 656c 662c 206b 6579 3a20 7374 7220  (self, key: str 
-00013180: 3d20 226f 7269 6722 2920 2d3e 2027 546f  = "orig") -> 'To
-00013190: 7263 6842 6c6f 6248 616e 646c 6527 3a0a  rchBlobHandle':.
-000131a0: 2020 2020 2020 2020 7572 692c 206f 776e          uri, own
-000131b0: 6572 203d 2073 656c 662e 6765 745f 626c  er = self.get_bl
-000131c0: 6f62 5f75 7269 286b 6579 2c20 2274 6f72  ob_uri(key, "tor
-000131d0: 6368 2229 0a20 2020 2020 2020 2062 6c6f  ch").        blo
-000131e0: 6220 3d20 546f 7263 6842 6c6f 6248 616e  b = TorchBlobHan
-000131f0: 646c 6528 7365 6c66 2e5f 636c 6965 6e74  dle(self._client
-00013200: 2c20 7572 692c 2069 735f 6675 6c6c 3d46  , uri, is_full=F
-00013210: 616c 7365 290a 2020 2020 2020 2020 626c  alse).        bl
-00013220: 6f62 2e73 6574 5f6c 6f63 616c 5f6f 776e  ob.set_local_own
-00013230: 6572 286f 776e 6572 290a 2020 2020 2020  er(owner).      
-00013240: 2020 7265 7475 726e 2062 6c6f 620a 0a20    return blob.. 
-00013250: 2020 2064 6566 2067 6574 5f6a 736f 6e5f     def get_json_
-00013260: 626c 6f62 2873 656c 662c 206b 6579 3a20  blob(self, key: 
-00013270: 7374 7220 3d20 226a 736f 6e73 5f69 6e22  str = "jsons_in"
-00013280: 2920 2d3e 2027 4a53 4f4e 426c 6f62 4861  ) -> 'JSONBlobHa
-00013290: 6e64 6c65 273a 0a20 2020 2020 2020 2075  ndle':.        u
-000132a0: 7269 2c20 6f77 6e65 7220 3d20 7365 6c66  ri, owner = self
-000132b0: 2e67 6574 5f62 6c6f 625f 7572 6928 6b65  .get_blob_uri(ke
-000132c0: 792c 2022 6a73 6f6e 2229 0a20 2020 2020  y, "json").     
-000132d0: 2020 2062 6c6f 6220 3d20 4a53 4f4e 426c     blob = JSONBl
-000132e0: 6f62 4861 6e64 6c65 2873 656c 662e 5f63  obHandle(self._c
-000132f0: 6c69 656e 742c 2075 7269 2c20 6973 5f66  lient, uri, is_f
-00013300: 756c 6c3d 4661 6c73 6529 0a20 2020 2020  ull=False).     
-00013310: 2020 2062 6c6f 622e 7365 745f 6c6f 6361     blob.set_loca
-00013320: 6c5f 6f77 6e65 7228 6f77 6e65 7229 0a20  l_owner(owner). 
-00013330: 2020 2020 2020 2072 6574 7572 6e20 626c         return bl
-00013340: 6f62 0a0a 2020 2020 6465 6620 6765 745f  ob..    def get_
-00013350: 6375 7374 6f6d 5f63 6f64 655f 626c 6f62  custom_code_blob
-00013360: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00013370: 6c66 2c20 6b65 793a 2073 7472 203d 2022  lf, key: str = "
-00013380: 6375 7374 6f6d 5f63 6f64 6522 2920 2d3e  custom_code") ->
-00013390: 2027 4375 7374 6f6d 436f 6465 426c 6f62   'CustomCodeBlob
-000133a0: 4861 6e64 6c65 273a 0a20 2020 2020 2020  Handle':.       
-000133b0: 2075 7269 2c20 6f77 6e65 7220 3d20 7365   uri, owner = se
-000133c0: 6c66 2e67 6574 5f62 6c6f 625f 7572 6928  lf.get_blob_uri(
-000133d0: 6b65 792c 2022 6375 7374 6f6d 5f63 6f64  key, "custom_cod
-000133e0: 6522 290a 2020 2020 2020 2020 626c 6f62  e").        blob
-000133f0: 203d 2043 7573 746f 6d43 6f64 6542 6c6f   = CustomCodeBlo
-00013400: 6248 616e 646c 6528 7365 6c66 2e5f 636c  bHandle(self._cl
-00013410: 6965 6e74 2c20 7572 692c 2069 735f 6675  ient, uri, is_fu
-00013420: 6c6c 3d46 616c 7365 290a 2020 2020 2020  ll=False).      
-00013430: 2020 626c 6f62 2e73 6574 5f6c 6f63 616c    blob.set_local
-00013440: 5f6f 776e 6572 286f 776e 6572 290a 2020  _owner(owner).  
-00013450: 2020 2020 2020 7265 7475 726e 2062 6c6f        return blo
-00013460: 620a 0a20 2020 2064 6566 2063 6865 636b  b..    def check
-00013470: 5f63 7573 746f 6d5f 636f 6465 5f6e 6f64  _custom_code_nod
-00013480: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-00013490: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000134a0: 7365 6c66 2e67 6574 5f74 7970 6528 2920  self.get_type() 
-000134b0: 696e 2043 5553 544f 4d5f 4e4f 4445 5f54  in CUSTOM_NODE_T
-000134c0: 5950 4553 3a0a 2020 2020 2020 2020 2020  YPES:.          
-000134d0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000134e0: 6f72 2866 227b 7365 6c66 7d20 6973 206e  or(f"{self} is n
-000134f0: 6f74 2061 2063 7573 746f 6d20 636f 6465  ot a custom code
-00013500: 206e 6f64 652e 2229 0a0a 2020 2020 6465   node.")..    de
-00013510: 6620 7365 745f 6375 7374 6f6d 5f69 6d70  f set_custom_imp
-00013520: 6f72 7473 280a 2020 2020 2020 2020 2020  orts(.          
-00013530: 2020 7365 6c66 2c20 6d6f 6475 6c65 733a    self, modules:
-00013540: 204c 6973 745b 4c69 7374 5b73 7472 5d5d   List[List[str]]
-00013550: 2920 2d3e 204e 6f64 6543 7573 746f 6d49  ) -> NodeCustomI
-00013560: 6d70 6f72 7473 3a0a 2020 2020 2020 2020  mports:.        
-00013570: 7365 6c66 2e63 6865 636b 5f63 7573 746f  self.check_custo
-00013580: 6d5f 636f 6465 5f6e 6f64 6528 290a 2020  m_code_node().  
-00013590: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
-000135a0: 7428 4e6f 6465 4375 7374 6f6d 496d 706f  t(NodeCustomImpo
-000135b0: 7274 732c 2073 656c 662e 5f63 6c69 656e  rts, self._clien
-000135c0: 742e 7265 7175 6573 745f 6a73 6f6e 280a  t.request_json(.
-000135d0: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
-000135e0: 4f44 5f50 5554 2c20 222f 6375 7374 6f6d  OD_PUT, "/custom
-000135f0: 5f69 6d70 6f72 7473 222c 207b 0a20 2020  _imports", {.   
-00013600: 2020 2020 2020 2020 2020 2020 2022 6461               "da
-00013610: 6722 3a20 7365 6c66 2e67 6574 5f64 6167  g": self.get_dag
-00013620: 2829 2e67 6574 5f75 7269 2829 2c0a 2020  ().get_uri(),.  
-00013630: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00013640: 6f64 6522 3a20 7365 6c66 2e67 6574 5f69  ode": self.get_i
-00013650: 6428 292c 0a20 2020 2020 2020 2020 2020  d(),.           
-00013660: 2020 2020 2022 6d6f 6475 6c65 7322 3a20       "modules": 
-00013670: 6d6f 6475 6c65 732c 0a20 2020 2020 2020  modules,.       
-00013680: 2020 2020 207d 2929 0a0a 2020 2020 6465       }))..    de
-00013690: 6620 6765 745f 6375 7374 6f6d 5f69 6d70  f get_custom_imp
-000136a0: 6f72 7473 2873 656c 6629 202d 3e20 4e6f  orts(self) -> No
-000136b0: 6465 4375 7374 6f6d 496d 706f 7274 733a  deCustomImports:
-000136c0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-000136d0: 6563 6b5f 6375 7374 6f6d 5f63 6f64 655f  eck_custom_code_
-000136e0: 6e6f 6465 2829 0a20 2020 2020 2020 2072  node().        r
-000136f0: 6574 7572 6e20 6361 7374 284e 6f64 6543  eturn cast(NodeC
-00013700: 7573 746f 6d49 6d70 6f72 7473 2c20 7365  ustomImports, se
-00013710: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-00013720: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-00013730: 2020 2020 204d 4554 484f 445f 4745 542c       METHOD_GET,
-00013740: 2022 2f63 7573 746f 6d5f 696d 706f 7274   "/custom_import
-00013750: 7322 2c20 7b0a 2020 2020 2020 2020 2020  s", {.          
-00013760: 2020 2020 2020 2264 6167 223a 2073 656c        "dag": sel
-00013770: 662e 6765 745f 6461 6728 292e 6765 745f  f.get_dag().get_
-00013780: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
-00013790: 2020 2020 2020 2022 6e6f 6465 223a 2073         "node": s
-000137a0: 656c 662e 6765 745f 6964 2829 2c0a 2020  elf.get_id(),.  
-000137b0: 2020 2020 2020 2020 2020 7d29 290a 0a20            })).. 
-000137c0: 2020 2064 6566 2073 6574 5f65 735f 7175     def set_es_qu
-000137d0: 6572 7928 7365 6c66 2c20 7175 6572 793a  ery(self, query:
-000137e0: 2044 6963 745b 7374 722c 2041 6e79 5d29   Dict[str, Any])
-000137f0: 202d 3e20 4553 5175 6572 7952 6573 706f   -> ESQueryRespo
-00013800: 6e73 653a 0a20 2020 2020 2020 2069 6620  nse:.        if 
-00013810: 7365 6c66 2e67 6574 5f74 7970 6528 2920  self.get_type() 
-00013820: 213d 2022 6573 5f72 6561 6465 7222 3a0a  != "es_reader":.
-00013830: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00013840: 6520 5661 6c75 6545 7272 6f72 2866 227b  e ValueError(f"{
-00013850: 7365 6c66 7d20 6973 206e 6f74 2061 6e20  self} is not an 
-00013860: 4553 2072 6561 6465 7220 6e6f 6465 2229  ES reader node")
-00013870: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00013880: 2063 6173 7428 4553 5175 6572 7952 6573   cast(ESQueryRes
-00013890: 706f 6e73 652c 2073 656c 662e 5f63 6c69  ponse, self._cli
-000138a0: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-000138b0: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-000138c0: 5448 4f44 5f50 4f53 542c 2022 2f65 735f  THOD_POST, "/es_
-000138d0: 7175 6572 7922 2c20 7b0a 2020 2020 2020  query", {.      
-000138e0: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
-000138f0: 2073 656c 662e 6765 745f 6461 6728 292e   self.get_dag().
-00013900: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
-00013910: 2020 2020 2020 2020 2020 2022 626c 6f62             "blob
-00013920: 223a 2073 656c 662e 6765 745f 626c 6f62  ": self.get_blob
-00013930: 5f68 616e 646c 6528 2265 7322 292e 6765  _handle("es").ge
-00013940: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
-00013950: 2020 2020 2020 2020 2022 6573 5f71 7565           "es_que
-00013960: 7279 223a 2071 7565 7279 2c0a 2020 2020  ry": query,.    
-00013970: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00013980: 2020 2029 290a 0a20 2020 2064 6566 2067     ))..    def g
-00013990: 6574 5f65 735f 7175 6572 7928 7365 6c66  et_es_query(self
-000139a0: 2920 2d3e 2045 5351 7565 7279 5265 7370  ) -> ESQueryResp
-000139b0: 6f6e 7365 3a0a 2020 2020 2020 2020 6966  onse:.        if
-000139c0: 2073 656c 662e 6765 745f 7479 7065 2829   self.get_type()
-000139d0: 2021 3d20 2265 735f 7265 6164 6572 223a   != "es_reader":
-000139e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000139f0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
-00013a00: 7b73 656c 667d 2069 7320 6e6f 7420 616e  {self} is not an
-00013a10: 2045 5320 7265 6164 6572 206e 6f64 6522   ES reader node"
-00013a20: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00013a30: 6e20 6361 7374 2845 5351 7565 7279 5265  n cast(ESQueryRe
-00013a40: 7370 6f6e 7365 2c20 7365 6c66 2e5f 636c  sponse, self._cl
-00013a50: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
-00013a60: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-00013a70: 4554 484f 445f 4745 542c 2022 2f65 735f  ETHOD_GET, "/es_
-00013a80: 7175 6572 7922 2c20 7b0a 2020 2020 2020  query", {.      
-00013a90: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
-00013aa0: 2073 656c 662e 6765 745f 6461 6728 292e   self.get_dag().
-00013ab0: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
-00013ac0: 2020 2020 2020 2020 2020 2022 626c 6f62             "blob
-00013ad0: 223a 2073 656c 662e 6765 745f 626c 6f62  ": self.get_blob
-00013ae0: 5f68 616e 646c 6528 2265 7322 292e 6765  _handle("es").ge
-00013af0: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
-00013b00: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00013b10: 2929 0a0a 2020 2020 6465 6620 6765 745f  ))..    def get_
-00013b20: 7573 6572 5f63 6f6c 756d 6e73 2873 656c  user_columns(sel
-00013b30: 662c 206b 6579 3a20 7374 7229 202d 3e20  f, key: str) -> 
-00013b40: 4e6f 6465 5573 6572 436f 6c75 6d6e 7352  NodeUserColumnsR
-00013b50: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00013b60: 2072 6574 7572 6e20 6361 7374 284e 6f64   return cast(Nod
-00013b70: 6555 7365 7243 6f6c 756d 6e73 5265 7370  eUserColumnsResp
-00013b80: 6f6e 7365 2c20 7365 6c66 2e5f 636c 6965  onse, self._clie
-00013b90: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-00013ba0: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00013bb0: 484f 445f 4745 542c 2022 2f75 7365 725f  HOD_GET, "/user_
-00013bc0: 636f 6c75 6d6e 7322 2c20 7b0a 2020 2020  columns", {.    
-00013bd0: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
-00013be0: 223a 2073 656c 662e 6765 745f 6461 6728  ": self.get_dag(
-00013bf0: 292e 6765 745f 7572 6928 292c 0a20 2020  ).get_uri(),.   
-00013c00: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00013c10: 6465 223a 2073 656c 662e 6765 745f 6964  de": self.get_id
-00013c20: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00013c30: 2020 2020 226b 6579 223a 206b 6579 2c0a      "key": key,.
-00013c40: 2020 2020 2020 2020 2020 2020 7d29 290a              })).
-00013c50: 0a20 2020 2064 6566 2067 6574 5f69 6e70  .    def get_inp
-00013c60: 7574 5f65 7861 6d70 6c65 2873 656c 6629  ut_example(self)
-00013c70: 202d 3e20 4469 6374 5b73 7472 2c20 4f70   -> Dict[str, Op
-00013c80: 7469 6f6e 616c 5b42 7974 6552 6573 706f  tional[ByteRespo
-00013c90: 6e73 655d 5d3a 0a20 2020 2020 2020 2072  nse]]:.        r
-00013ca0: 6573 203d 207b 7d0a 2020 2020 2020 2020  es = {}.        
-00013cb0: 666f 7220 6b65 7920 696e 2073 656c 662e  for key in self.
-00013cc0: 6765 745f 696e 7075 7473 2829 3a0a 2020  get_inputs():.  
-00013cd0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-00013ce0: 6e6f 6465 2c20 6f75 745f 6b65 7920 3d20  node, out_key = 
-00013cf0: 7365 6c66 2e67 6574 5f69 6e70 7574 286b  self.get_input(k
-00013d00: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
-00013d10: 6466 203d 2069 6e70 7574 5f6e 6f64 652e  df = input_node.
-00013d20: 7265 6164 286f 7574 5f6b 6579 2c20 3029  read(out_key, 0)
-00013d30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013d40: 6466 2069 7320 6e6f 7420 4e6f 6e65 2061  df is not None a
-00013d50: 6e64 2069 7369 6e73 7461 6e63 6528 6466  nd isinstance(df
-00013d60: 2c20 7064 2e44 6174 6146 7261 6d65 293a  , pd.DataFrame):
-00013d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013d80: 2075 7365 725f 636f 6c75 6d6e 7320 3d20   user_columns = 
-00013d90: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-00013da0: 2020 2020 2020 696e 7075 745f 6e6f 6465        input_node
-00013db0: 2e67 6574 5f75 7365 725f 636f 6c75 6d6e  .get_user_column
-00013dc0: 7328 6f75 745f 6b65 7929 5b22 7573 6572  s(out_key)["user
-00013dd0: 5f63 6f6c 756d 6e73 225d 0a20 2020 2020  _columns"].     
-00013de0: 2020 2020 2020 2020 2020 2072 6d61 7020             rmap 
-00013df0: 3d20 7b63 6f6c 3a20 636f 6c2e 7265 706c  = {col: col.repl
-00013e00: 6163 6528 2275 7365 725f 222c 2022 2229  ace("user_", "")
-00013e10: 2066 6f72 2063 6f6c 2069 6e20 7573 6572   for col in user
-00013e20: 5f63 6f6c 756d 6e73 7d0a 2020 2020 2020  _columns}.      
-00013e30: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
-00013e40: 662e 6c6f 635b 3a2c 2075 7365 725f 636f  f.loc[:, user_co
-00013e50: 6c75 6d6e 735d 2e72 656e 616d 6528 636f  lumns].rename(co
-00013e60: 6c75 6d6e 733d 726d 6170 290a 2020 2020  lumns=rmap).    
-00013e70: 2020 2020 2020 2020 7265 735b 6b65 795d          res[key]
-00013e80: 203d 2064 660a 2020 2020 2020 2020 7265   = df.        re
-00013e90: 7475 726e 2072 6573 0a0a 2020 2020 6465  turn res..    de
-00013ea0: 6620 6765 745f 6465 6628 7365 6c66 2920  f get_def(self) 
-00013eb0: 2d3e 204e 6f64 6544 6566 3a0a 2020 2020  -> NodeDef:.    
-00013ec0: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
-00013ed0: 4e6f 6465 4465 662c 2073 656c 662e 5f63  NodeDef, self._c
-00013ee0: 6c69 656e 742e 7265 7175 6573 745f 6a73  lient.request_js
-00013ef0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00013f00: 4d45 5448 4f44 5f47 4554 2c20 222f 6e6f  METHOD_GET, "/no
-00013f10: 6465 5f64 6566 222c 207b 0a20 2020 2020  de_def", {.     
-00013f20: 2020 2020 2020 2020 2020 2022 6461 6722             "dag"
-00013f30: 3a20 7365 6c66 2e67 6574 5f64 6167 2829  : self.get_dag()
-00013f40: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
-00013f50: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
-00013f60: 6522 3a20 7365 6c66 2e67 6574 5f69 6428  e": self.get_id(
-00013f70: 292c 0a20 2020 2020 2020 2020 2020 207d  ),.            }
-00013f80: 2929 0a0a 2020 2020 2320 4d6f 6465 6c4c  ))..    # ModelL
-00013f90: 696b 6520 4e6f 6465 7320 6f6e 6c79 0a0a  ike Nodes only..
-00013fa0: 2020 2020 6465 6620 6973 5f6d 6f64 656c      def is_model
-00013fb0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00013fc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00013fd0: 5f69 735f 6d6f 6465 6c20 6973 204e 6f6e  _is_model is Non
-00013fe0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00013ff0: 656c 662e 5f69 735f 6d6f 6465 6c20 3d20  elf._is_model = 
-00014000: 6361 7374 284e 6f64 6554 7970 6552 6573  cast(NodeTypeRes
-00014010: 706f 6e73 652c 2073 656c 662e 5f63 6c69  ponse, self._cli
-00014020: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-00014030: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014040: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
-00014050: 6e6f 6465 5f74 7970 6522 2c20 7b0a 2020  node_type", {.  
-00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014070: 2020 2264 6167 223a 2073 656c 662e 6765    "dag": self.ge
-00014080: 745f 6461 6728 292e 6765 745f 7572 6928  t_dag().get_uri(
-00014090: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000140a0: 2020 2020 2020 2022 6e6f 6465 223a 2073         "node": s
-000140b0: 656c 662e 6765 745f 6964 2829 2c0a 2020  elf.get_id(),.  
-000140c0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
-000140d0: 295b 2269 735f 6d6f 6465 6c22 5d0a 0a20  )["is_model"].. 
-000140e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000140f0: 6c66 2e5f 6973 5f6d 6f64 656c 0a0a 2020  lf._is_model..  
-00014100: 2020 6465 6620 656e 7375 7265 5f69 735f    def ensure_is_
-00014110: 6d6f 6465 6c28 7365 6c66 2920 2d3e 204e  model(self) -> N
-00014120: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-00014130: 6e6f 7420 7365 6c66 2e69 735f 6d6f 6465  not self.is_mode
-00014140: 6c28 293a 0a20 2020 2020 2020 2020 2020  l():.           
-00014150: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00014160: 7228 6622 7b73 656c 667d 2069 7320 6e6f  r(f"{self} is no
-00014170: 7420 6120 6d6f 6465 6c20 6e6f 6465 2e22  t a model node."
-00014180: 290a 0a20 2020 2064 6566 2073 6574 7570  )..    def setup
-00014190: 5f6d 6f64 656c 2873 656c 662c 206f 626a  _model(self, obj
-000141a0: 3a20 4469 6374 5b73 7472 2c20 416e 795d  : Dict[str, Any]
-000141b0: 2920 2d3e 204d 6f64 656c 496e 666f 3a0a  ) -> ModelInfo:.
-000141c0: 2020 2020 2020 2020 7365 6c66 2e65 6e73          self.ens
-000141d0: 7572 655f 6973 5f6d 6f64 656c 2829 0a20  ure_is_model(). 
-000141e0: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
-000141f0: 7374 284d 6f64 656c 496e 666f 2c20 7365  st(ModelInfo, se
-00014200: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-00014210: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-00014220: 2020 2020 204d 4554 484f 445f 5055 542c       METHOD_PUT,
-00014230: 2022 2f6d 6f64 656c 5f73 6574 7570 222c   "/model_setup",
-00014240: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00014250: 2020 2022 6461 6722 3a20 7365 6c66 2e67     "dag": self.g
-00014260: 6574 5f64 6167 2829 2e67 6574 5f75 7269  et_dag().get_uri
-00014270: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00014280: 2020 2020 226e 6f64 6522 3a20 7365 6c66      "node": self
-00014290: 2e67 6574 5f69 6428 292c 0a20 2020 2020  .get_id(),.     
-000142a0: 2020 2020 2020 2020 2020 2022 636f 6e66             "conf
-000142b0: 6967 223a 206f 626a 2c0a 2020 2020 2020  ig": obj,.      
-000142c0: 2020 2020 2020 7d29 290a 0a20 2020 2064        }))..    d
-000142d0: 6566 2067 6574 5f6d 6f64 656c 5f70 6172  ef get_model_par
-000142e0: 616d 7328 7365 6c66 2920 2d3e 204d 6f64  ams(self) -> Mod
-000142f0: 656c 5061 7261 6d73 5265 7370 6f6e 7365  elParamsResponse
-00014300: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
-00014310: 6e73 7572 655f 6973 5f6d 6f64 656c 2829  nsure_is_model()
-00014320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014330: 6361 7374 284d 6f64 656c 5061 7261 6d73  cast(ModelParams
-00014340: 5265 7370 6f6e 7365 2c20 7365 6c66 2e5f  Response, self._
-00014350: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
-00014360: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
-00014370: 204d 4554 484f 445f 4745 542c 2022 2f6d   METHOD_GET, "/m
-00014380: 6f64 656c 5f70 6172 616d 7322 2c20 7b0a  odel_params", {.
-00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143a0: 2264 6167 223a 2073 656c 662e 6765 745f  "dag": self.get_
-000143b0: 6461 6728 292e 6765 745f 7572 6928 292c  dag().get_uri(),
-000143c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000143d0: 2022 6e6f 6465 223a 2073 656c 662e 6765   "node": self.ge
-000143e0: 745f 6964 2829 2c0a 2020 2020 2020 2020  t_id(),.        
-000143f0: 2020 2020 7d29 290a 0a20 2020 2064 6566      }))..    def
-00014400: 205f 5f68 6173 685f 5f28 7365 6c66 2920   __hash__(self) 
-00014410: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00014420: 7265 7475 726e 2068 6173 6828 2873 656c  return hash((sel
-00014430: 662e 6765 745f 6461 6728 292c 2073 656c  f.get_dag(), sel
-00014440: 662e 6765 745f 6964 2829 2929 0a0a 2020  f.get_id()))..  
-00014450: 2020 6465 6620 5f5f 6571 5f5f 2873 656c    def __eq__(sel
-00014460: 662c 206f 7468 6572 3a20 6f62 6a65 6374  f, other: object
-00014470: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00014480: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00014490: 616e 6365 286f 7468 6572 2c20 7365 6c66  ance(other, self
-000144a0: 2e5f 5f63 6c61 7373 5f5f 293a 0a20 2020  .__class__):.   
-000144b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000144c0: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-000144d0: 2073 656c 662e 6765 745f 6461 6728 2920   self.get_dag() 
-000144e0: 213d 206f 7468 6572 2e67 6574 5f64 6167  != other.get_dag
-000144f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014500: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00014510: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00014520: 2e67 6574 5f69 6428 2920 3d3d 206f 7468  .get_id() == oth
-00014530: 6572 2e67 6574 5f69 6428 290a 0a20 2020  er.get_id()..   
-00014540: 2064 6566 205f 5f6e 655f 5f28 7365 6c66   def __ne__(self
-00014550: 2c20 6f74 6865 723a 206f 626a 6563 7429  , other: object)
-00014560: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00014570: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
-00014580: 662e 5f5f 6571 5f5f 286f 7468 6572 290a  f.__eq__(other).
-00014590: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
-000145a0: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-000145b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000145c0: 6c66 2e67 6574 5f69 6428 290a 0a20 2020  lf.get_id()..   
-000145d0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-000145e0: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
-000145f0: 2020 2020 7265 7475 726e 2066 227b 7365      return f"{se
-00014600: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
-00014610: 616d 655f 5f7d 5b7b 7365 6c66 2e67 6574  ame__}[{self.get
-00014620: 5f69 6428 297d 5d22 0a0a 2320 2a2a 2a20  _id()}]"..# *** 
-00014630: 4e6f 6465 4861 6e64 6c65 202a 2a2a 0a0a  NodeHandle ***..
-00014640: 0a45 4d50 5459 5f42 4c4f 425f 5052 4546  .EMPTY_BLOB_PREF
-00014650: 4958 203d 2022 6e75 6c6c 3a2f 2f22 0a0a  IX = "null://"..
-00014660: 0a63 6c61 7373 2042 6c6f 6248 616e 646c  .class BlobHandl
-00014670: 653a 0a20 2020 2064 6566 205f 5f69 6e69  e:.    def __ini
-00014680: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
-00014690: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-000146a0: 2020 2063 6c69 656e 743a 2058 594d 4543     client: XYMEC
-000146b0: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
-000146c0: 2020 2075 7269 3a20 7374 722c 0a20 2020     uri: str,.   
-000146d0: 2020 2020 2020 2020 2069 735f 6675 6c6c           is_full
-000146e0: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
-000146f0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00014700: 6c69 656e 7420 3d20 636c 6965 6e74 0a20  lient = client. 
-00014710: 2020 2020 2020 2073 656c 662e 5f75 7269         self._uri
-00014720: 203d 2075 7269 0a20 2020 2020 2020 2073   = uri.        s
-00014730: 656c 662e 5f69 735f 6675 6c6c 203d 2069  elf._is_full = i
-00014740: 735f 6675 6c6c 0a20 2020 2020 2020 2073  s_full.        s
-00014750: 656c 662e 5f63 7479 7065 3a20 4f70 7469  elf._ctype: Opti
-00014760: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00014770: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00014780: 6d70 5f75 7269 3a20 4f70 7469 6f6e 616c  mp_uri: Optional
-00014790: 5b73 7472 5d20 3d20 4e6f 6e65 0a20 2020  [str] = None.   
-000147a0: 2020 2020 2073 656c 662e 5f6f 776e 6572       self._owner
-000147b0: 3a20 4f70 7469 6f6e 616c 5b42 6c6f 624f  : Optional[BlobO
-000147c0: 776e 6572 5d20 3d20 4e6f 6e65 0a20 2020  wner] = None.   
-000147d0: 2020 2020 2073 656c 662e 5f69 6e66 6f3a       self._info:
-000147e0: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-000147f0: 7472 2c20 416e 795d 5d20 3d20 4e6f 6e65  tr, Any]] = None
-00014800: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-00014810: 6172 656e 743a 204f 7074 696f 6e61 6c5b  arent: Optional[
-00014820: 426c 6f62 4861 6e64 6c65 5d20 3d20 4e6f  BlobHandle] = No
-00014830: 6e65 0a0a 2020 2020 6465 6620 6973 5f66  ne..    def is_f
-00014840: 756c 6c28 7365 6c66 2920 2d3e 2062 6f6f  ull(self) -> boo
-00014850: 6c3a 0a20 2020 2020 2020 2072 6574 7572  l:.        retur
-00014860: 6e20 7365 6c66 2e5f 6973 5f66 756c 6c0a  n self._is_full.
-00014870: 0a20 2020 2064 6566 2069 735f 656d 7074  .    def is_empt
-00014880: 7928 7365 6c66 2920 2d3e 2062 6f6f 6c3a  y(self) -> bool:
-00014890: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000148a0: 7365 6c66 2e5f 7572 692e 7374 6172 7473  self._uri.starts
-000148b0: 7769 7468 2845 4d50 5459 5f42 4c4f 425f  with(EMPTY_BLOB_
-000148c0: 5052 4546 4958 290a 0a20 2020 2064 6566  PREFIX)..    def
-000148d0: 2067 6574 5f75 7269 2873 656c 6629 202d   get_uri(self) -
-000148e0: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
-000148f0: 6574 7572 6e20 7365 6c66 2e5f 7572 690a  eturn self._uri.
-00014900: 0a20 2020 2064 6566 2067 6574 5f70 6174  .    def get_pat
-00014910: 6828 7365 6c66 2c20 2a70 6174 683a 2073  h(self, *path: s
-00014920: 7472 2920 2d3e 2027 426c 6f62 4861 6e64  tr) -> 'BlobHand
-00014930: 6c65 273a 0a20 2020 2020 2020 2069 6620  le':.        if 
-00014940: 7365 6c66 2e69 735f 6675 6c6c 2829 3a0a  self.is_full():.
-00014950: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00014960: 6520 5661 6c75 6545 7272 6f72 2866 2255  e ValueError(f"U
-00014970: 5249 206d 7573 7420 6e6f 7420 6265 2066  RI must not be f
-00014980: 756c 6c3a 207b 7365 6c66 7d22 290a 2020  ull: {self}").  
-00014990: 2020 2020 2020 7265 7475 726e 2042 6c6f        return Blo
-000149a0: 6248 616e 646c 6528 0a20 2020 2020 2020  bHandle(.       
-000149b0: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
-000149c0: 742c 2066 227b 7365 6c66 2e5f 7572 697d  t, f"{self._uri}
-000149d0: 2f7b 272f 272e 6a6f 696e 2870 6174 6829  /{'/'.join(path)
-000149e0: 7d22 2c20 6973 5f66 756c 6c3d 5472 7565  }", is_full=True
-000149f0: 290a 0a20 2020 2064 6566 2067 6574 5f70  )..    def get_p
-00014a00: 6172 656e 7428 7365 6c66 2920 2d3e 2027  arent(self) -> '
-00014a10: 426c 6f62 4861 6e64 6c65 273a 0a20 2020  BlobHandle':.   
-00014a20: 2020 2020 2069 6620 7365 6c66 2e5f 7061       if self._pa
-00014a30: 7265 6e74 2069 7320 4e6f 6e65 3a0a 2020  rent is None:.  
-00014a40: 2020 2020 2020 2020 2020 7572 6920 3d20            uri = 
-00014a50: 7572 6c70 6172 7365 2873 656c 662e 5f75  urlparse(self._u
-00014a60: 7269 290a 2020 2020 2020 2020 2020 2020  ri).            
-00014a70: 7061 7468 203d 2050 7572 6550 6174 6828  path = PurePath(
-00014a80: 2a50 6f73 6978 5061 7468 2875 7269 2e70  *PosixPath(uri.p
-00014a90: 6174 6829 2e70 6172 7473 5b3a 335d 290a  ath).parts[:3]).
-00014aa0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00014ab0: 7572 6920 3d20 7572 6c75 6e70 6172 7365  uri = urlunparse
-00014ac0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014ad0: 2020 2875 7269 2e73 6368 656d 652c 2075    (uri.scheme, u
-00014ae0: 7269 2e6e 6574 6c6f 632c 2070 6174 682e  ri.netloc, path.
-00014af0: 6173 5f70 6f73 6978 2829 2c20 4e6f 6e65  as_posix(), None
-00014b00: 2c20 4e6f 6e65 2c20 4e6f 6e65 2929 0a20  , None, None)). 
-00014b10: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00014b20: 2042 6c6f 6248 616e 646c 6528 7365 6c66   BlobHandle(self
-00014b30: 2e5f 636c 6965 6e74 2c20 6e65 775f 7572  ._client, new_ur
-00014b40: 692c 2069 735f 6675 6c6c 3d46 616c 7365  i, is_full=False
-00014b50: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00014b60: 6c66 2e5f 7061 7265 6e74 203d 2072 6573  lf._parent = res
-00014b70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014b80: 7365 6c66 2e5f 7061 7265 6e74 0a0a 2020  self._parent..  
-00014b90: 2020 6465 6620 6765 745f 6374 7970 6528    def get_ctype(
-00014ba0: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-00014bb0: 6c5b 7374 725d 3a0a 2020 2020 2020 2020  l[str]:.        
-00014bc0: 7265 7475 726e 2073 656c 662e 5f63 7479  return self._cty
-00014bd0: 7065 0a0a 2020 2020 6465 6620 636c 6561  pe..    def clea
-00014be0: 725f 696e 666f 5f63 6163 6865 2873 656c  r_info_cache(sel
-00014bf0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00014c00: 2020 2020 7365 6c66 2e5f 696e 666f 203d      self._info =
-00014c10: 204e 6f6e 650a 0a20 2020 2064 6566 2067   None..    def g
-00014c20: 6574 5f69 6e66 6f28 7365 6c66 2920 2d3e  et_info(self) ->
-00014c30: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
-00014c40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00014c50: 2e69 735f 6675 6c6c 2829 3a0a 2020 2020  .is_full():.    
-00014c60: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00014c70: 6c75 6545 7272 6f72 2866 2255 5249 206d  lueError(f"URI m
-00014c80: 7573 7420 6e6f 7420 6265 2066 756c 6c3a  ust not be full:
-00014c90: 207b 7365 6c66 7d22 290a 2020 2020 2020   {self}").      
-00014ca0: 2020 6966 2073 656c 662e 5f69 6e66 6f20    if self._info 
-00014cb0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00014cc0: 2020 2020 2069 6e66 6f20 3d20 7365 6c66       info = self
-00014cd0: 2e67 6574 5f70 6174 6828 2269 6e66 6f2e  .get_path("info.
-00014ce0: 6a73 6f6e 2229 2e67 6574 5f63 6f6e 7465  json").get_conte
-00014cf0: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
-00014d00: 2061 7373 6572 7420 696e 666f 2069 7320   assert info is 
-00014d10: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-00014d20: 2020 2020 2073 656c 662e 5f69 6e66 6f20       self._info 
-00014d30: 3d20 6361 7374 2844 6963 745b 7374 722c  = cast(Dict[str,
-00014d40: 2041 6e79 5d2c 2069 6e66 6f29 0a20 2020   Any], info).   
-00014d50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00014d60: 2e5f 696e 666f 0a0a 2020 2020 6465 6620  ._info..    def 
-00014d70: 6765 745f 636f 6e74 656e 7428 7365 6c66  get_content(self
-00014d80: 2920 2d3e 204f 7074 696f 6e61 6c5b 4279  ) -> Optional[By
-00014d90: 7465 5265 7370 6f6e 7365 5d3a 0a20 2020  teResponse]:.   
-00014da0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00014db0: 2e69 735f 6675 6c6c 2829 3a0a 2020 2020  .is_full():.    
-00014dc0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00014dd0: 6c75 6545 7272 6f72 2866 2255 5249 206d  lueError(f"URI m
-00014de0: 7573 7420 6265 2066 756c 6c3a 207b 7365  ust be full: {se
-00014df0: 6c66 7d22 290a 2020 2020 2020 2020 6966  lf}").        if
-00014e00: 2073 656c 662e 6973 5f65 6d70 7479 2829   self.is_empty()
-00014e10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00014e20: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00014e30: 2020 736c 6565 705f 7469 6d65 203d 2030    sleep_time = 0
-00014e40: 2e31 0a20 2020 2020 2020 2073 6c65 6570  .1.        sleep
-00014e50: 5f6d 756c 203d 2031 2e31 0a20 2020 2020  _mul = 1.1.     
-00014e60: 2020 2073 6c65 6570 5f6d 6178 203d 2035     sleep_max = 5
-00014e70: 2e30 0a20 2020 2020 2020 2074 6f74 616c  .0.        total
-00014e80: 5f74 696d 6520 3d20 3630 2e30 0a20 2020  _time = 60.0.   
-00014e90: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
-00014ea0: 3d20 7469 6d65 2e6d 6f6e 6f74 6f6e 6963  = time.monotonic
-00014eb0: 2829 0a20 2020 2020 2020 2077 6869 6c65  ().        while
-00014ec0: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
-00014ed0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00014ee0: 2020 2020 2020 2020 6669 6e2c 2063 7479          fin, cty
-00014ef0: 7065 203d 2073 656c 662e 5f63 6c69 656e  pe = self._clien
-00014f00: 742e 7265 7175 6573 745f 6279 7465 7328  t.request_bytes(
-00014f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f20: 2020 2020 204d 4554 484f 445f 504f 5354       METHOD_POST
-00014f30: 2c20 222f 7572 6922 2c20 7b0a 2020 2020  , "/uri", {.    
-00014f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f50: 2020 2020 2275 7269 223a 2073 656c 662e      "uri": self.
-00014f60: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
-00014f70: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00014f80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014f90: 2020 7365 6c66 2e5f 6374 7970 6520 3d20    self._ctype = 
-00014fa0: 6374 7970 650a 2020 2020 2020 2020 2020  ctype.          
-00014fb0: 2020 2020 2020 7265 7475 726e 2069 6e74        return int
-00014fc0: 6572 7072 6574 5f63 7479 7065 2866 696e  erpret_ctype(fin
-00014fd0: 2c20 6374 7970 6529 0a20 2020 2020 2020  , ctype).       
-00014fe0: 2020 2020 2065 7863 6570 7420 4854 5450       except HTTP
-00014ff0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00015000: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-00015010: 2e72 6573 706f 6e73 652e 7374 6174 7573  .response.status
-00015020: 5f63 6f64 6520 213d 2034 3034 3a0a 2020  _code != 404:.  
-00015030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015040: 2020 7261 6973 6520 650a 2020 2020 2020    raise e.      
-00015050: 2020 2020 2020 2020 2020 6966 2074 696d            if tim
-00015060: 652e 6d6f 6e6f 746f 6e69 6328 2920 2d20  e.monotonic() - 
-00015070: 7374 6172 745f 7469 6d65 203e 3d20 746f  start_time >= to
-00015080: 7461 6c5f 7469 6d65 3a0a 2020 2020 2020  tal_time:.      
-00015090: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000150a0: 6973 6520 650a 2020 2020 2020 2020 2020  ise e.          
-000150b0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-000150c0: 2873 6c65 6570 5f74 696d 6529 0a20 2020  (sleep_time).   
-000150d0: 2020 2020 2020 2020 2020 2020 2073 6c65               sle
-000150e0: 6570 5f74 696d 6520 3d20 6d69 6e28 736c  ep_time = min(sl
-000150f0: 6565 705f 7469 6d65 202a 2073 6c65 6570  eep_time * sleep
-00015100: 5f6d 756c 2c20 736c 6565 705f 6d61 7829  _mul, sleep_max)
-00015110: 0a0a 2020 2020 6465 6620 6c69 7374 5f66  ..    def list_f
-00015120: 696c 6573 2873 656c 6629 202d 3e20 4c69  iles(self) -> Li
-00015130: 7374 5b27 426c 6f62 4861 6e64 6c65 275d  st['BlobHandle']
-00015140: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00015150: 662e 6973 5f66 756c 6c28 293a 0a20 2020  f.is_full():.   
-00015160: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00015170: 616c 7565 4572 726f 7228 6622 5552 4920  alueError(f"URI 
-00015180: 6d75 7374 206e 6f74 2062 6520 6675 6c6c  must not be full
-00015190: 3a20 7b73 656c 667d 2229 0a20 2020 2020  : {self}").     
-000151a0: 2020 2072 6573 7020 3d20 6361 7374 2842     resp = cast(B
-000151b0: 6c6f 6246 696c 6573 5265 7370 6f6e 7365  lobFilesResponse
-000151c0: 2c20 7365 6c66 2e5f 636c 6965 6e74 2e72  , self._client.r
-000151d0: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
-000151e0: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-000151f0: 4745 542c 2022 2f62 6c6f 625f 6669 6c65  GET, "/blob_file
-00015200: 7322 2c20 7b0a 2020 2020 2020 2020 2020  s", {.          
-00015210: 2020 2020 2020 2262 6c6f 6222 3a20 7365        "blob": se
-00015220: 6c66 2e67 6574 5f75 7269 2829 2c0a 2020  lf.get_uri(),.  
-00015230: 2020 2020 2020 2020 2020 7d29 290a 2020            })).  
-00015240: 2020 2020 2020 7265 7475 726e 205b 0a20        return [. 
-00015250: 2020 2020 2020 2020 2020 2042 6c6f 6248             BlobH
-00015260: 616e 646c 6528 7365 6c66 2e5f 636c 6965  andle(self._clie
-00015270: 6e74 2c20 626c 6f62 5f75 7269 2c20 6973  nt, blob_uri, is
-00015280: 5f66 756c 6c3d 5472 7565 290a 2020 2020  _full=True).    
-00015290: 2020 2020 2020 2020 666f 7220 626c 6f62          for blob
-000152a0: 5f75 7269 2069 6e20 7265 7370 5b22 6669  _uri in resp["fi
-000152b0: 6c65 7322 5d0a 2020 2020 2020 2020 5d0a  les"].        ].
-000152c0: 0a20 2020 2064 6566 2061 735f 7374 7228  .    def as_str(
-000152d0: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
-000152e0: 2020 2020 2020 7265 7475 726e 2066 227b        return f"{
-000152f0: 7365 6c66 2e67 6574 5f75 7269 2829 7d22  self.get_uri()}"
-00015300: 0a0a 2020 2020 6465 6620 7365 745f 6f77  ..    def set_ow
-00015310: 6e65 7228 7365 6c66 2c20 6f77 6e65 723a  ner(self, owner:
-00015320: 204e 6f64 6548 616e 646c 6529 202d 3e20   NodeHandle) -> 
-00015330: 426c 6f62 4f77 6e65 723a 0a20 2020 2020  BlobOwner:.     
-00015340: 2020 2069 6620 7365 6c66 2e69 735f 6675     if self.is_fu
-00015350: 6c6c 2829 3a0a 2020 2020 2020 2020 2020  ll():.          
-00015360: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00015370: 6f72 2866 2255 5249 206d 7573 7420 6e6f  or(f"URI must no
-00015380: 7420 6265 2066 756c 6c3a 207b 7365 6c66  t be full: {self
-00015390: 7d22 290a 2020 2020 2020 2020 7265 7475  }").        retu
-000153a0: 726e 2063 6173 7428 426c 6f62 4f77 6e65  rn cast(BlobOwne
-000153b0: 722c 2073 656c 662e 5f63 6c69 656e 742e  r, self._client.
-000153c0: 7265 7175 6573 745f 6a73 6f6e 280a 2020  request_json(.  
-000153d0: 2020 2020 2020 2020 2020 4d45 5448 4f44            METHOD
-000153e0: 5f50 5554 2c20 222f 626c 6f62 5f6f 776e  _PUT, "/blob_own
-000153f0: 6572 222c 207b 0a20 2020 2020 2020 2020  er", {.         
-00015400: 2020 2020 2020 2022 626c 6f62 223a 2073         "blob": s
-00015410: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
-00015420: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00015430: 6f77 6e65 725f 6461 6722 3a20 6f77 6e65  owner_dag": owne
-00015440: 722e 6765 745f 6461 6728 292e 6765 745f  r.get_dag().get_
-00015450: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
-00015460: 2020 2020 2020 2022 6f77 6e65 725f 6e6f         "owner_no
-00015470: 6465 223a 206f 776e 6572 2e67 6574 5f69  de": owner.get_i
-00015480: 6428 292c 0a20 2020 2020 2020 2020 2020  d(),.           
-00015490: 207d 2929 0a0a 2020 2020 6465 6620 6765   }))..    def ge
-000154a0: 745f 6f77 6e65 7228 7365 6c66 2920 2d3e  t_owner(self) ->
-000154b0: 2042 6c6f 624f 776e 6572 3a0a 2020 2020   BlobOwner:.    
-000154c0: 2020 2020 6966 2073 656c 662e 5f6f 776e      if self._own
-000154d0: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
-000154e0: 2020 2020 2020 2020 7365 6c66 2e5f 6f77          self._ow
-000154f0: 6e65 7220 3d20 7365 6c66 2e5f 636c 6965  ner = self._clie
-00015500: 6e74 2e67 6574 5f62 6c6f 625f 6f77 6e65  nt.get_blob_owne
-00015510: 7228 7365 6c66 2e67 6574 5f75 7269 2829  r(self.get_uri()
-00015520: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00015530: 2073 656c 662e 5f6f 776e 6572 0a0a 2020   self._owner..  
-00015540: 2020 6465 6620 7365 745f 6c6f 6361 6c5f    def set_local_
-00015550: 6f77 6e65 7228 7365 6c66 2c20 6f77 6e65  owner(self, owne
-00015560: 723a 2042 6c6f 624f 776e 6572 2920 2d3e  r: BlobOwner) ->
-00015570: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-00015580: 656c 662e 5f6f 776e 6572 203d 206f 776e  elf._owner = own
-00015590: 6572 0a0a 2020 2020 6465 6620 6765 745f  er..    def get_
-000155a0: 6f77 6e65 725f 6461 6728 7365 6c66 2920  owner_dag(self) 
-000155b0: 2d3e 204f 7074 696f 6e61 6c5b 7374 725d  -> Optional[str]
-000155c0: 3a0a 2020 2020 2020 2020 6f77 6e65 7220  :.        owner 
-000155d0: 3d20 7365 6c66 2e67 6574 5f6f 776e 6572  = self.get_owner
-000155e0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-000155f0: 6e20 6f77 6e65 725b 226f 776e 6572 5f64  n owner["owner_d
-00015600: 6167 225d 0a0a 2020 2020 6465 6620 6765  ag"]..    def ge
-00015610: 745f 6f77 6e65 725f 6e6f 6465 2873 656c  t_owner_node(sel
-00015620: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-00015630: 2020 206f 776e 6572 203d 2073 656c 662e     owner = self.
-00015640: 6765 745f 6f77 6e65 7228 290a 2020 2020  get_owner().    
-00015650: 2020 2020 7265 7475 726e 206f 776e 6572      return owner
-00015660: 5b22 6f77 6e65 725f 6e6f 6465 225d 0a0a  ["owner_node"]..
-00015670: 2020 2020 6465 6620 7365 745f 6d6f 6465      def set_mode
-00015680: 6c5f 7468 7265 7368 6f6c 6428 0a20 2020  l_threshold(.   
-00015690: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-000156a0: 2020 2020 2020 2020 2020 2074 6872 6573             thres
-000156b0: 686f 6c64 3a20 666c 6f61 742c 0a20 2020  hold: float,.   
-000156c0: 2020 2020 2020 2020 2070 6f73 5f6c 6162           pos_lab
-000156d0: 656c 3a20 7374 7229 202d 3e20 4d6f 6465  el: str) -> Mode
-000156e0: 6c49 6e66 6f3a 0a20 2020 2020 2020 2072  lInfo:.        r
-000156f0: 6574 7572 6e20 6361 7374 284d 6f64 656c  eturn cast(Model
-00015700: 496e 666f 2c20 7365 6c66 2e5f 636c 6965  Info, self._clie
-00015710: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-00015720: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-00015730: 484f 445f 5055 542c 2022 2f74 6872 6573  HOD_PUT, "/thres
-00015740: 686f 6c64 222c 207b 0a20 2020 2020 2020  hold", {.       
-00015750: 2020 2020 2020 2020 2022 626c 6f62 223a           "blob":
-00015760: 2073 656c 662e 6765 745f 7572 6928 292c   self.get_uri(),
-00015770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015780: 2022 7468 7265 7368 6f6c 6422 3a20 7468   "threshold": th
-00015790: 7265 7368 6f6c 642c 0a20 2020 2020 2020  reshold,.       
-000157a0: 2020 2020 2020 2020 2022 706f 735f 6c61           "pos_la
-000157b0: 6265 6c22 3a20 706f 735f 6c61 6265 6c2c  bel": pos_label,
-000157c0: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
-000157d0: 0a0a 2020 2020 6465 6620 6465 6c5f 6d6f  ..    def del_mo
-000157e0: 6465 6c5f 7468 7265 7368 6f6c 6428 7365  del_threshold(se
-000157f0: 6c66 2920 2d3e 204d 6f64 656c 496e 666f  lf) -> ModelInfo
-00015800: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00015810: 2063 6173 7428 4d6f 6465 6c49 6e66 6f2c   cast(ModelInfo,
-00015820: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
-00015830: 7175 6573 745f 6a73 6f6e 280a 2020 2020  quest_json(.    
-00015840: 2020 2020 2020 2020 4d45 5448 4f44 5f44          METHOD_D
-00015850: 454c 4554 452c 2022 2f74 6872 6573 686f  ELETE, "/thresho
-00015860: 6c64 222c 207b 0a20 2020 2020 2020 2020  ld", {.         
-00015870: 2020 2020 2020 2022 626c 6f62 223a 2073         "blob": s
-00015880: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
-00015890: 2020 2020 2020 2020 2020 207d 2929 0a0a             }))..
-000158a0: 2020 2020 6465 6620 6765 745f 6d6f 6465      def get_mode
-000158b0: 6c5f 696e 666f 2873 656c 6629 202d 3e20  l_info(self) -> 
-000158c0: 4d6f 6465 6c49 6e66 6f3a 0a20 2020 2020  ModelInfo:.     
-000158d0: 2020 2072 6574 7572 6e20 6361 7374 284d     return cast(M
-000158e0: 6f64 656c 496e 666f 2c20 7365 6c66 2e5f  odelInfo, self._
-000158f0: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
-00015900: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
-00015910: 204d 4554 484f 445f 4745 542c 2022 2f6d   METHOD_GET, "/m
-00015920: 6f64 656c 5f69 6e66 6f22 2c20 7b0a 2020  odel_info", {.  
-00015930: 2020 2020 2020 2020 2020 2020 2020 2262                "b
-00015940: 6c6f 6222 3a20 7365 6c66 2e67 6574 5f75  lob": self.get_u
-00015950: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
-00015960: 2020 7d29 290a 0a20 2020 2064 6566 2063    }))..    def c
-00015970: 6f70 795f 746f 280a 2020 2020 2020 2020  opy_to(.        
-00015980: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00015990: 2020 2020 2020 746f 5f75 7269 3a20 7374        to_uri: st
-000159a0: 722c 0a20 2020 2020 2020 2020 2020 206e  r,.            n
-000159b0: 6577 5f6f 776e 6572 3a20 4f70 7469 6f6e  ew_owner: Option
-000159c0: 616c 5b4e 6f64 6548 616e 646c 655d 203d  al[NodeHandle] =
-000159d0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-000159e0: 2020 2065 7874 6572 6e61 6c5f 6f77 6e65     external_owne
-000159f0: 723a 2062 6f6f 6c20 3d20 4661 6c73 6529  r: bool = False)
-00015a00: 202d 3e20 2742 6c6f 6248 616e 646c 6527   -> 'BlobHandle'
-00015a10: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00015a20: 662e 6973 5f66 756c 6c28 293a 0a20 2020  f.is_full():.   
-00015a30: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00015a40: 616c 7565 4572 726f 7228 6622 5552 4920  alueError(f"URI 
-00015a50: 6d75 7374 206e 6f74 2062 6520 6675 6c6c  must not be full
-00015a60: 3a20 7b73 656c 667d 2229 0a0a 2020 2020  : {self}")..    
-00015a70: 2020 2020 6f77 6e65 725f 6461 6720 3d20      owner_dag = 
-00015a80: 5c0a 2020 2020 2020 2020 2020 2020 4e6f  \.            No
-00015a90: 6e65 2069 6620 6e65 775f 6f77 6e65 7220  ne if new_owner 
-00015aa0: 6973 204e 6f6e 6520 656c 7365 206e 6577  is None else new
-00015ab0: 5f6f 776e 6572 2e67 6574 5f64 6167 2829  _owner.get_dag()
-00015ac0: 2e67 6574 5f75 7269 2829 0a20 2020 2020  .get_uri().     
-00015ad0: 2020 206f 776e 6572 5f6e 6f64 6520 3d20     owner_node = 
-00015ae0: 4e6f 6e65 2069 6620 6e65 775f 6f77 6e65  None if new_owne
-00015af0: 7220 6973 204e 6f6e 6520 656c 7365 206e  r is None else n
-00015b00: 6577 5f6f 776e 6572 2e67 6574 5f69 6428  ew_owner.get_id(
-00015b10: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
-00015b20: 6361 7374 2843 6f70 7942 6c6f 622c 2073  cast(CopyBlob, s
-00015b30: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
-00015b40: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-00015b50: 2020 2020 2020 4d45 5448 4f44 5f50 4f53        METHOD_POS
-00015b60: 542c 2022 2f63 6f70 795f 626c 6f62 222c  T, "/copy_blob",
-00015b70: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00015b80: 2020 2022 6672 6f6d 5f75 7269 223a 2073     "from_uri": s
-00015b90: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
-00015ba0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00015bb0: 6f77 6e65 725f 6461 6722 3a20 6f77 6e65  owner_dag": owne
-00015bc0: 725f 6461 672c 0a20 2020 2020 2020 2020  r_dag,.         
-00015bd0: 2020 2020 2020 2022 6f77 6e65 725f 6e6f         "owner_no
-00015be0: 6465 223a 206f 776e 6572 5f6e 6f64 652c  de": owner_node,
-00015bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c00: 2022 6578 7465 726e 616c 5f6f 776e 6572   "external_owner
-00015c10: 223a 2065 7874 6572 6e61 6c5f 6f77 6e65  ": external_owne
-00015c20: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00015c30: 2020 2022 746f 5f75 7269 223a 2074 6f5f     "to_uri": to_
-00015c40: 7572 692c 0a20 2020 2020 2020 2020 2020  uri,.           
-00015c50: 207d 2929 0a20 2020 2020 2020 2072 6574   })).        ret
-00015c60: 7572 6e20 426c 6f62 4861 6e64 6c65 2873  urn BlobHandle(s
-00015c70: 656c 662e 5f63 6c69 656e 742c 2072 6573  elf._client, res
-00015c80: 5b22 6e65 775f 7572 6922 5d2c 2069 735f  ["new_uri"], is_
-00015c90: 6675 6c6c 3d46 616c 7365 290a 0a20 2020  full=False)..   
-00015ca0: 2064 6566 2064 6f77 6e6c 6f61 645f 7a69   def download_zi
-00015cb0: 7028 7365 6c66 2c20 746f 5f70 6174 683a  p(self, to_path:
-00015cc0: 204f 7074 696f 6e61 6c5b 7374 725d 2920   Optional[str]) 
-00015cd0: 2d3e 204f 7074 696f 6e61 6c5b 696f 2e42  -> Optional[io.B
-00015ce0: 7974 6573 494f 5d3a 0a20 2020 2020 2020  ytesIO]:.       
-00015cf0: 2069 6620 7365 6c66 2e69 735f 6675 6c6c   if self.is_full
-00015d00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00015d10: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00015d20: 2866 2255 5249 206d 7573 7420 6e6f 7420  (f"URI must not 
-00015d30: 6265 2066 756c 6c3a 207b 7365 6c66 7d22  be full: {self}"
-00015d40: 290a 2020 2020 2020 2020 6375 725f 7265  ).        cur_re
-00015d50: 732c 205f 203d 2073 656c 662e 5f63 6c69  s, _ = self._cli
-00015d60: 656e 742e 7265 7175 6573 745f 6279 7465  ent.request_byte
-00015d70: 7328 0a20 2020 2020 2020 2020 2020 204d  s(.            M
-00015d80: 4554 484f 445f 4745 542c 2022 2f64 6f77  ETHOD_GET, "/dow
-00015d90: 6e6c 6f61 645f 7a69 7022 2c20 7b0a 2020  nload_zip", {.  
-00015da0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
-00015db0: 6c6f 6222 3a20 7365 6c66 2e67 6574 5f75  lob": self.get_u
-00015dc0: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
-00015dd0: 2020 7d29 0a20 2020 2020 2020 2069 6620    }).        if 
-00015de0: 746f 5f70 6174 6820 6973 204e 6f6e 653a  to_path is None:
-00015df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015e00: 7572 6e20 696f 2e42 7974 6573 494f 2863  urn io.BytesIO(c
-00015e10: 7572 5f72 6573 2e72 6561 6428 2929 0a20  ur_res.read()). 
-00015e20: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00015e30: 2874 6f5f 7061 7468 2c20 2277 6222 2920  (to_path, "wb") 
-00015e40: 6173 2066 696c 655f 646f 776e 6c6f 6164  as file_download
-00015e50: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-00015e60: 6c65 5f64 6f77 6e6c 6f61 642e 7772 6974  le_download.writ
-00015e70: 6528 6375 725f 7265 732e 7265 6164 2829  e(cur_res.read()
-00015e80: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00015e90: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
-00015ea0: 7065 7266 6f72 6d5f 7570 6c6f 6164 5f61  perform_upload_a
-00015eb0: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
-00015ec0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00015ed0: 2020 2020 2061 6374 696f 6e3a 2073 7472       action: str
-00015ee0: 2c0a 2020 2020 2020 2020 2020 2020 6164  ,.            ad
-00015ef0: 6469 7469 6f6e 616c 3a20 4469 6374 5b73  ditional: Dict[s
-00015f00: 7472 2c20 556e 696f 6e5b 7374 722c 2069  tr, Union[str, i
-00015f10: 6e74 2c20 4c69 7374 5b69 6e74 5d5d 5d2c  nt, List[int]]],
-00015f20: 0a20 2020 2020 2020 2020 2020 2066 6f62  .            fob
-00015f30: 6a3a 204f 7074 696f 6e61 6c5b 494f 5b62  j: Optional[IO[b
-00015f40: 7974 6573 5d5d 2920 2d3e 2055 706c 6f61  ytes]]) -> Uploa
-00015f50: 6446 696c 6573 5265 7370 6f6e 7365 3a0a  dFilesResponse:.
-00015f60: 2020 2020 2020 2020 6172 6773 3a20 4469          args: Di
-00015f70: 6374 5b73 7472 2c20 556e 696f 6e5b 7374  ct[str, Union[st
-00015f80: 722c 2069 6e74 2c20 4c69 7374 5b69 6e74  r, int, List[int
-00015f90: 5d5d 5d20 3d20 7b0a 2020 2020 2020 2020  ]]] = {.        
-00015fa0: 2020 2020 2261 6374 696f 6e22 3a20 6163      "action": ac
-00015fb0: 7469 6f6e 2c0a 2020 2020 2020 2020 7d0a  tion,.        }.
-00015fc0: 2020 2020 2020 2020 6172 6773 2e75 7064          args.upd
-00015fd0: 6174 6528 6164 6469 7469 6f6e 616c 290a  ate(additional).
-00015fe0: 2020 2020 2020 2020 6966 2066 6f62 6a20          if fobj 
-00015ff0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00016000: 2020 2020 2020 2020 206d 6574 686f 6420           method 
-00016010: 3d20 4d45 5448 4f44 5f46 494c 450a 2020  = METHOD_FILE.  
-00016020: 2020 2020 2020 2020 2020 6669 6c65 733a            files:
-00016030: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-00016040: 7472 2c20 494f 5b62 7974 6573 5d5d 5d20  tr, IO[bytes]]] 
-00016050: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00016060: 2020 2020 2266 696c 6522 3a20 666f 626a      "file": fobj
-00016070: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
-00016080: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016090: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-000160a0: 203d 204d 4554 484f 445f 504f 5354 0a20   = METHOD_POST. 
-000160b0: 2020 2020 2020 2020 2020 2066 696c 6573             files
-000160c0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-000160d0: 6966 2061 6374 696f 6e20 3d3d 2022 636c  if action == "cl
-000160e0: 6561 7222 3a0a 2020 2020 2020 2020 2020  ear":.          
-000160f0: 2020 7365 6c66 2e5f 746d 705f 7572 6920    self._tmp_uri 
-00016100: 3d20 4e6f 6e65 0a20 2020 2020 2020 2072  = None.        r
-00016110: 6574 7572 6e20 6361 7374 2855 706c 6f61  eturn cast(Uploa
-00016120: 6446 696c 6573 5265 7370 6f6e 7365 2c20  dFilesResponse, 
-00016130: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
-00016140: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-00016150: 2020 2020 2020 206d 6574 686f 642c 2022         method, "
-00016160: 2f75 706c 6f61 645f 6669 6c65 222c 2061  /upload_file", a
-00016170: 7267 732c 2066 696c 6573 3d66 696c 6573  rgs, files=files
-00016180: 2929 0a0a 2020 2020 6465 6620 5f73 7461  ))..    def _sta
-00016190: 7274 5f75 706c 6f61 6428 7365 6c66 2c20  rt_upload(self, 
-000161a0: 7369 7a65 3a20 696e 742c 2068 6173 685f  size: int, hash_
-000161b0: 7374 723a 2073 7472 2c20 6578 743a 2073  str: str, ext: s
-000161c0: 7472 2920 2d3e 2073 7472 3a0a 2020 2020  tr) -> str:.    
-000161d0: 2020 2020 7265 7320 3d20 7365 6c66 2e5f      res = self._
-000161e0: 7065 7266 6f72 6d5f 7570 6c6f 6164 5f61  perform_upload_a
-000161f0: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
-00016200: 2020 2022 7374 6172 7422 2c0a 2020 2020     "start",.    
-00016210: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00016220: 2020 2020 2020 2020 2020 2274 6172 6765            "targe
-00016230: 7422 3a20 7365 6c66 2e67 6574 5f75 7269  t": self.get_uri
-00016240: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00016250: 2020 2020 2268 6173 6822 3a20 6861 7368      "hash": hash
-00016260: 5f73 7472 2c0a 2020 2020 2020 2020 2020  _str,.          
-00016270: 2020 2020 2020 2273 697a 6522 3a20 7369        "size": si
-00016280: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-00016290: 2020 2020 2265 7874 223a 2065 7874 2c0a      "ext": ext,.
-000162a0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000162b0: 2020 2020 2020 2020 2020 2066 6f62 6a3d             fobj=
-000162c0: 4e6f 6e65 290a 2020 2020 2020 2020 6173  None).        as
-000162d0: 7365 7274 2072 6573 5b22 7572 6922 5d20  sert res["uri"] 
-000162e0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-000162f0: 2020 2020 7265 7475 726e 2072 6573 5b22      return res["
-00016300: 7572 6922 5d0a 0a20 2020 2064 6566 205f  uri"]..    def _
-00016310: 6c65 6761 6379 5f61 7070 656e 645f 7570  legacy_append_up
-00016320: 6c6f 6164 280a 2020 2020 2020 2020 2020  load(.          
-00016330: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00016340: 2020 2020 7572 693a 2073 7472 2c0a 2020      uri: str,.  
-00016350: 2020 2020 2020 2020 2020 666f 626a 3a20            fobj: 
-00016360: 494f 5b62 7974 6573 5d29 202d 3e20 696e  IO[bytes]) -> in
-00016370: 743a 0a20 2020 2020 2020 2072 6573 203d  t:.        res =
-00016380: 2073 656c 662e 5f70 6572 666f 726d 5f75   self._perform_u
-00016390: 706c 6f61 645f 6163 7469 6f6e 280a 2020  pload_action(.  
-000163a0: 2020 2020 2020 2020 2020 2261 7070 656e            "appen
-000163b0: 6422 2c20 7b22 7572 6922 3a20 7572 697d  d", {"uri": uri}
-000163c0: 2c20 666f 626a 3d66 6f62 6a29 0a20 2020  , fobj=fobj).   
-000163d0: 2020 2020 2072 6574 7572 6e20 7265 735b       return res[
-000163e0: 2270 6f73 225d 0a0a 2020 2020 6465 6620  "pos"]..    def 
-000163f0: 5f61 7070 656e 645f 7570 6c6f 6164 280a  _append_upload(.
-00016400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016410: 2c0a 2020 2020 2020 2020 2020 2020 7572  ,.            ur
-00016420: 693a 2073 7472 2c0a 2020 2020 2020 2020  i: str,.        
-00016430: 2020 2020 666f 626a 3a20 494f 5b62 7974      fobj: IO[byt
-00016440: 6573 5d2c 0a20 2020 2020 2020 2020 2020  es],.           
-00016450: 206f 6666 7365 743a 2069 6e74 2920 2d3e   offset: int) ->
-00016460: 2069 6e74 3a0a 2020 2020 2020 2020 7265   int:.        re
-00016470: 7320 3d20 7365 6c66 2e5f 7065 7266 6f72  s = self._perfor
-00016480: 6d5f 7570 6c6f 6164 5f61 6374 696f 6e28  m_upload_action(
-00016490: 0a20 2020 2020 2020 2020 2020 2022 6170  .            "ap
-000164a0: 7065 6e64 222c 207b 2275 7269 223a 2075  pend", {"uri": u
-000164b0: 7269 2c20 226f 6666 7365 7422 3a20 6f66  ri, "offset": of
-000164c0: 6673 6574 7d2c 2066 6f62 6a3d 666f 626a  fset}, fobj=fobj
-000164d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000164e0: 2072 6573 5b22 706f 7322 5d0a 0a20 2020   res["pos"]..   
-000164f0: 2064 6566 205f 6669 6e69 7368 5f75 706c   def _finish_upl
-00016500: 6f61 645f 7a69 7028 7365 6c66 2920 2d3e  oad_zip(self) ->
-00016510: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
-00016520: 2020 2020 7572 6920 3d20 7365 6c66 2e5f      uri = self._
-00016530: 746d 705f 7572 690a 2020 2020 2020 2020  tmp_uri.        
-00016540: 6966 2075 7269 2069 7320 4e6f 6e65 3a0a  if uri is None:.
-00016550: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00016560: 6520 5661 6c75 6545 7272 6f72 2822 746d  e ValueError("tm
-00016570: 705f 7572 6920 6973 204e 6f6e 6522 290a  p_uri is None").
-00016580: 2020 2020 2020 2020 7265 7320 3d20 6361          res = ca
-00016590: 7374 2855 706c 6f61 6446 696c 6573 5265  st(UploadFilesRe
-000165a0: 7370 6f6e 7365 2c20 7365 6c66 2e5f 636c  sponse, self._cl
-000165b0: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
-000165c0: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
-000165d0: 4554 484f 445f 504f 5354 2c20 222f 6669  ETHOD_POST, "/fi
-000165e0: 6e69 7368 5f7a 6970 222c 207b 2275 7269  nish_zip", {"uri
-000165f0: 223a 2075 7269 7d29 290a 2020 2020 2020  ": uri})).      
-00016600: 2020 7265 7475 726e 2072 6573 5b22 6669    return res["fi
-00016610: 6c65 7322 5d0a 0a20 2020 2064 6566 205f  les"]..    def _
-00016620: 6669 6e69 7368 5f75 706c 6f61 645f 736b  finish_upload_sk
-00016630: 6c69 6b65 280a 2020 2020 2020 2020 2020  like(.          
-00016640: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00016650: 2020 2020 7863 6f6c 733a 204c 6973 745b      xcols: List[
-00016660: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
-00016670: 2020 6973 5f63 6c66 3a20 626f 6f6c 2c0a    is_clf: bool,.
-00016680: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00016690: 6c5f 6e61 6d65 3a20 7374 722c 0a20 2020  l_name: str,.   
-000166a0: 2020 2020 2020 2020 206d 6179 6265 5f63           maybe_c
-000166b0: 6c61 7373 6573 3a20 4f70 7469 6f6e 616c  lasses: Optional
-000166c0: 5b4c 6973 745b 7374 725d 5d2c 0a20 2020  [List[str]],.   
-000166d0: 2020 2020 2020 2020 206d 6179 6265 5f72           maybe_r
-000166e0: 616e 6765 3a20 5475 706c 655b 4f70 7469  ange: Tuple[Opti
-000166f0: 6f6e 616c 5b66 6c6f 6174 5d2c 204f 7074  onal[float], Opt
-00016700: 696f 6e61 6c5b 666c 6f61 745d 5d2c 0a20  ional[float]],. 
-00016710: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
-00016720: 696e 6974 3a20 626f 6f6c 2920 2d3e 2055  init: bool) -> U
-00016730: 706c 6f61 6446 696c 6573 5265 7370 6f6e  ploadFilesRespon
-00016740: 7365 3a0a 2020 2020 2020 2020 7572 6920  se:.        uri 
-00016750: 3d20 7365 6c66 2e5f 746d 705f 7572 690a  = self._tmp_uri.
-00016760: 2020 2020 2020 2020 6966 2075 7269 2069          if uri i
-00016770: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00016780: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00016790: 7272 6f72 2822 746d 705f 7572 6920 6973  rror("tmp_uri is
-000167a0: 204e 6f6e 6522 290a 2020 2020 2020 2020   None").        
-000167b0: 7265 7475 726e 2063 6173 7428 5570 6c6f  return cast(Uplo
-000167c0: 6164 4669 6c65 7352 6573 706f 6e73 652c  adFilesResponse,
-000167d0: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
-000167e0: 7175 6573 745f 6a73 6f6e 280a 2020 2020  quest_json(.    
-000167f0: 2020 2020 2020 2020 4d45 5448 4f44 5f50          METHOD_P
-00016800: 4f53 542c 2022 2f66 696e 6973 685f 736b  OST, "/finish_sk
-00016810: 6c69 6b65 222c 207b 0a20 2020 2020 2020  like", {.       
-00016820: 2020 2020 2020 2020 2022 636c 6173 7365           "classe
-00016830: 7322 3a20 6d61 7962 655f 636c 6173 7365  s": maybe_classe
-00016840: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00016850: 2020 2022 6675 6c6c 5f69 6e69 7422 3a20     "full_init": 
-00016860: 6675 6c6c 5f69 6e69 742c 0a20 2020 2020  full_init,.     
-00016870: 2020 2020 2020 2020 2020 2022 6973 5f63             "is_c
-00016880: 6c66 223a 2069 735f 636c 662c 0a20 2020  lf": is_clf,.   
-00016890: 2020 2020 2020 2020 2020 2020 2022 6d6f               "mo
-000168a0: 6465 6c5f 7572 6922 3a20 7365 6c66 2e67  del_uri": self.g
-000168b0: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
-000168c0: 2020 2020 2020 2020 2020 226d 6f64 656c            "model
-000168d0: 5f6e 616d 6522 3a20 6d6f 6465 6c5f 6e61  _name": model_na
-000168e0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-000168f0: 2020 2020 226f 7574 7075 745f 7261 6e67      "output_rang
-00016900: 6522 3a20 6d61 7962 655f 7261 6e67 652c  e": maybe_range,
-00016910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016920: 2022 6f77 6e65 725f 6461 6722 3a20 7365   "owner_dag": se
-00016930: 6c66 2e67 6574 5f6f 776e 6572 5f64 6167  lf.get_owner_dag
-00016940: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-00016950: 2020 2020 226f 776e 6572 5f6e 6f64 6522      "owner_node"
-00016960: 3a20 7365 6c66 2e67 6574 5f6f 776e 6572  : self.get_owner
-00016970: 5f6e 6f64 6528 292c 0a20 2020 2020 2020  _node(),.       
-00016980: 2020 2020 2020 2020 2022 746d 705f 7572           "tmp_ur
-00016990: 6922 3a20 7572 692c 0a20 2020 2020 2020  i": uri,.       
-000169a0: 2020 2020 2020 2020 2022 7863 6f6c 7322           "xcols"
-000169b0: 3a20 7863 6f6c 732c 0a20 2020 2020 2020  : xcols,.       
-000169c0: 2020 2020 207d 2929 0a0a 2020 2020 6465       }))..    de
-000169d0: 6620 5f63 6c65 6172 5f75 706c 6f61 6428  f _clear_upload(
-000169e0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-000169f0: 2020 2020 2020 2075 7269 203d 2073 656c         uri = sel
-00016a00: 662e 5f74 6d70 5f75 7269 0a20 2020 2020  f._tmp_uri.     
-00016a10: 2020 2069 6620 7572 6920 6973 204e 6f6e     if uri is Non
-00016a20: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00016a30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00016a40: 2274 6d70 5f75 7269 2069 7320 4e6f 6e65  "tmp_uri is None
-00016a50: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00016a60: 5f70 6572 666f 726d 5f75 706c 6f61 645f  _perform_upload_
-00016a70: 6163 7469 6f6e 2822 636c 6561 7222 2c20  action("clear", 
-00016a80: 7b22 7572 6922 3a20 7572 697d 2c20 666f  {"uri": uri}, fo
-00016a90: 626a 3d4e 6f6e 6529 0a0a 2020 2020 6465  bj=None)..    de
-00016aa0: 6620 5f6c 6567 6163 795f 7570 6c6f 6164  f _legacy_upload
-00016ab0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
-00016ac0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00016ad0: 2020 2020 2066 696c 655f 636f 6e74 656e       file_conten
-00016ae0: 743a 2049 4f5b 6279 7465 735d 2c0a 2020  t: IO[bytes],.  
-00016af0: 2020 2020 2020 2020 2020 6578 743a 2073            ext: s
-00016b00: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-00016b10: 7072 6f67 7265 7373 5f62 6172 3a20 4f70  progress_bar: Op
-00016b20: 7469 6f6e 616c 5b49 4f5b 416e 795d 5d20  tional[IO[Any]] 
-00016b30: 3d20 7379 732e 7374 646f 7574 2920 2d3e  = sys.stdout) ->
-00016b40: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-00016b50: 6e69 745f 706f 7320 3d20 6669 6c65 5f63  nit_pos = file_c
-00016b60: 6f6e 7465 6e74 2e73 6565 6b28 302c 2069  ontent.seek(0, i
-00016b70: 6f2e 5345 454b 5f43 5552 290a 2020 2020  o.SEEK_CUR).    
-00016b80: 2020 2020 6669 6c65 5f68 6173 6820 3d20      file_hash = 
-00016b90: 6765 745f 6669 6c65 5f68 6173 6828 6669  get_file_hash(fi
-00016ba0: 6c65 5f63 6f6e 7465 6e74 290a 2020 2020  le_content).    
-00016bb0: 2020 2020 746f 7461 6c5f 7369 7a65 203d      total_size =
-00016bc0: 2066 696c 655f 636f 6e74 656e 742e 7365   file_content.se
-00016bd0: 656b 2830 2c20 696f 2e53 4545 4b5f 454e  ek(0, io.SEEK_EN
-00016be0: 4429 202d 2069 6e69 745f 706f 730a 2020  D) - init_pos.  
-00016bf0: 2020 2020 2020 6669 6c65 5f63 6f6e 7465        file_conte
-00016c00: 6e74 2e73 6565 6b28 696e 6974 5f70 6f73  nt.seek(init_pos
-00016c10: 2c20 696f 2e53 4545 4b5f 5345 5429 0a20  , io.SEEK_SET). 
-00016c20: 2020 2020 2020 2069 6620 7072 6f67 7265         if progre
-00016c30: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-00016c40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00016c50: 7072 6f67 7265 7373 5f62 6172 2e77 7269  progress_bar.wri
-00016c60: 7465 2822 5570 6c6f 6164 696e 6720 6669  te("Uploading fi
-00016c70: 6c65 3a5c 6e22 290a 2020 2020 2020 2020  le:\n").        
-00016c80: 7072 696e 745f 7072 6f67 7265 7373 203d  print_progress =
-00016c90: 2067 6574 5f70 726f 6772 6573 735f 6261   get_progress_ba
-00016ca0: 7228 6f75 743d 7072 6f67 7265 7373 5f62  r(out=progress_b
-00016cb0: 6172 290a 2020 2020 2020 2020 746d 705f  ar).        tmp_
-00016cc0: 7572 6920 3d20 7365 6c66 2e5f 7374 6172  uri = self._star
-00016cd0: 745f 7570 6c6f 6164 2874 6f74 616c 5f73  t_upload(total_s
-00016ce0: 697a 652c 2066 696c 655f 6861 7368 2c20  ize, file_hash, 
-00016cf0: 6578 7429 0a20 2020 2020 2020 2073 656c  ext).        sel
-00016d00: 662e 5f74 6d70 5f75 7269 203d 2074 6d70  f._tmp_uri = tmp
-00016d10: 5f75 7269 0a20 2020 2020 2020 2063 7572  _uri.        cur
-00016d20: 5f73 697a 6520 3d20 300a 2020 2020 2020  _size = 0.      
-00016d30: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
-00016d40: 2020 2020 2020 2020 2020 7072 696e 745f            print_
-00016d50: 7072 6f67 7265 7373 2863 7572 5f73 697a  progress(cur_siz
-00016d60: 6520 2f20 746f 7461 6c5f 7369 7a65 2c20  e / total_size, 
-00016d70: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00016d80: 2020 2062 7566 6620 3d20 6669 6c65 5f63     buff = file_c
-00016d90: 6f6e 7465 6e74 2e72 6561 6428 6765 745f  ontent.read(get_
-00016da0: 6669 6c65 5f75 706c 6f61 645f 6368 756e  file_upload_chun
-00016db0: 6b5f 7369 7a65 2829 290a 2020 2020 2020  k_size()).      
-00016dc0: 2020 2020 2020 6966 206e 6f74 2062 7566        if not buf
-00016dd0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-00016de0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00016df0: 2020 2020 206e 6577 5f73 697a 6520 3d20       new_size = 
-00016e00: 7365 6c66 2e5f 6c65 6761 6379 5f61 7070  self._legacy_app
-00016e10: 656e 645f 7570 6c6f 6164 2874 6d70 5f75  end_upload(tmp_u
-00016e20: 7269 2c20 4279 7465 7349 4f28 6275 6666  ri, BytesIO(buff
-00016e30: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-00016e40: 6620 6e65 775f 7369 7a65 202d 2063 7572  f new_size - cur
-00016e50: 5f73 697a 6520 213d 206c 656e 2862 7566  _size != len(buf
-00016e60: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-00016e70: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00016e80: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00016e90: 2020 2020 2020 2020 2020 6622 696e 636f            f"inco
-00016ea0: 6d70 6c65 7465 2063 6875 6e6b 2075 706c  mplete chunk upl
-00016eb0: 6f61 6420 6e3a 7b6e 6577 5f73 697a 657d  oad n:{new_size}
-00016ec0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00016ed0: 2020 2020 2020 2066 226f 3a7b 6375 725f         f"o:{cur_
-00016ee0: 7369 7a65 7d20 623a 7b6c 656e 2862 7566  size} b:{len(buf
-00016ef0: 6629 7d22 290a 2020 2020 2020 2020 2020  f)}").          
-00016f00: 2020 6375 725f 7369 7a65 203d 206e 6577    cur_size = new
-00016f10: 5f73 697a 650a 2020 2020 2020 2020 7072  _size.        pr
-00016f20: 696e 745f 7072 6f67 7265 7373 2863 7572  int_progress(cur
-00016f30: 5f73 697a 6520 2f20 746f 7461 6c5f 7369  _size / total_si
-00016f40: 7a65 2c20 5472 7565 290a 0a20 2020 2064  ze, True)..    d
-00016f50: 6566 205f 7570 6c6f 6164 5f66 696c 6528  ef _upload_file(
-00016f60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016f70: 662c 0a20 2020 2020 2020 2020 2020 2066  f,.            f
-00016f80: 696c 655f 636f 6e74 656e 743a 2049 4f5b  ile_content: IO[
-00016f90: 6279 7465 735d 2c0a 2020 2020 2020 2020  bytes],.        
-00016fa0: 2020 2020 6d61 785f 7468 7265 6164 733a      max_threads:
-00016fb0: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
-00016fc0: 2020 6578 743a 2073 7472 2c0a 2020 2020    ext: str,.    
-00016fd0: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-00016fe0: 5f62 6172 3a20 4f70 7469 6f6e 616c 5b49  _bar: Optional[I
-00016ff0: 4f5b 416e 795d 5d20 3d20 7379 732e 7374  O[Any]] = sys.st
-00017000: 646f 7574 2920 2d3e 204e 6f6e 653a 0a20  dout) -> None:. 
-00017010: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00017020: 636c 6965 6e74 2e5f 6170 695f 7665 7273  client._api_vers
-00017030: 696f 6e20 3c20 353a 0a20 2020 2020 2020  ion < 5:.       
-00017040: 2020 2020 2073 656c 662e 5f6c 6567 6163       self._legac
-00017050: 795f 7570 6c6f 6164 5f66 696c 6528 6669  y_upload_file(fi
-00017060: 6c65 5f63 6f6e 7465 6e74 2c20 6578 743d  le_content, ext=
-00017070: 227a 6970 2229 0a20 2020 2020 2020 2020  "zip").         
-00017080: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00017090: 2020 696e 6974 5f70 6f73 203d 2066 696c    init_pos = fil
-000170a0: 655f 636f 6e74 656e 742e 7365 656b 2830  e_content.seek(0
-000170b0: 2c20 696f 2e53 4545 4b5f 4355 5229 0a20  , io.SEEK_CUR). 
-000170c0: 2020 2020 2020 2066 696c 655f 6861 7368         file_hash
-000170d0: 203d 2067 6574 5f66 696c 655f 6861 7368   = get_file_hash
-000170e0: 2866 696c 655f 636f 6e74 656e 7429 0a20  (file_content). 
-000170f0: 2020 2020 2020 2074 6f74 616c 5f73 697a         total_siz
-00017100: 6520 3d20 6669 6c65 5f63 6f6e 7465 6e74  e = file_content
-00017110: 2e73 6565 6b28 302c 2069 6f2e 5345 454b  .seek(0, io.SEEK
-00017120: 5f45 4e44 2920 2d20 696e 6974 5f70 6f73  _END) - init_pos
-00017130: 0a20 2020 2020 2020 2066 696c 655f 636f  .        file_co
-00017140: 6e74 656e 742e 7365 656b 2869 6e69 745f  ntent.seek(init_
-00017150: 706f 732c 2069 6f2e 5345 454b 5f53 4554  pos, io.SEEK_SET
-00017160: 290a 2020 2020 2020 2020 6966 2070 726f  ).        if pro
-00017170: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00017180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00017190: 2020 2070 726f 6772 6573 735f 6261 722e     progress_bar.
-000171a0: 7772 6974 6528 2255 706c 6f61 6469 6e67  write("Uploading
-000171b0: 2066 696c 653a 5c6e 2229 0a20 2020 2020   file:\n").     
-000171c0: 2020 2070 7269 6e74 5f70 726f 6772 6573     print_progres
-000171d0: 7320 3d20 6765 745f 7072 6f67 7265 7373  s = get_progress
-000171e0: 5f62 6172 286f 7574 3d70 726f 6772 6573  _bar(out=progres
-000171f0: 735f 6261 7229 0a20 2020 2020 2020 2074  s_bar).        t
-00017200: 6d70 5f75 7269 203d 2073 656c 662e 5f73  mp_uri = self._s
-00017210: 7461 7274 5f75 706c 6f61 6428 746f 7461  tart_upload(tota
-00017220: 6c5f 7369 7a65 2c20 6669 6c65 5f68 6173  l_size, file_has
-00017230: 682c 2065 7874 290a 2020 2020 2020 2020  h, ext).        
-00017240: 7365 6c66 2e5f 746d 705f 7572 6920 3d20  self._tmp_uri = 
-00017250: 746d 705f 7572 690a 2020 2020 2020 2020  tmp_uri.        
-00017260: 7570 6c6f 6164 5f63 6875 6e6b 5f73 697a  upload_chunk_siz
-00017270: 6520 3d20 6765 745f 6669 6c65 5f75 706c  e = get_file_upl
-00017280: 6f61 645f 6368 756e 6b5f 7369 7a65 2829  oad_chunk_size()
-00017290: 0a20 2020 2020 2020 2074 6f74 616c 5f63  .        total_c
-000172a0: 6875 6e6b 7320 3d20 6d61 7468 2e63 6569  hunks = math.cei
-000172b0: 6c28 746f 7461 6c5f 7369 7a65 202f 2075  l(total_size / u
-000172c0: 706c 6f61 645f 6368 756e 6b5f 7369 7a65  pload_chunk_size
-000172d0: 290a 0a20 2020 2020 2020 2062 6567 696e  )..        begin
-000172e0: 7320 3d20 5b63 6875 6e6b 202a 2075 706c  s = [chunk * upl
-000172f0: 6f61 645f 6368 756e 6b5f 7369 7a65 2066  oad_chunk_size f
-00017300: 6f72 2063 6875 6e6b 2069 6e20 7261 6e67  or chunk in rang
-00017310: 6528 746f 7461 6c5f 6368 756e 6b73 295d  e(total_chunks)]
-00017320: 0a0a 2020 2020 2020 2020 6465 6620 636f  ..        def co
-00017330: 6d70 7574 655f 7570 6c6f 6164 280a 2020  mpute_upload(.  
-00017340: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-00017350: 6673 6574 3a20 696e 742c 0a20 2020 2020  fset: int,.     
-00017360: 2020 2020 2020 2020 2020 2063 6f6d 7075             compu
-00017370: 7465 5f6c 6f63 6b3a 2074 6872 6561 6469  te_lock: threadi
-00017380: 6e67 2e52 4c6f 636b 2920 2d3e 204e 6f6e  ng.RLock) -> Non
-00017390: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-000173a0: 7373 6572 7420 7365 6c66 2e5f 746d 705f  ssert self._tmp_
-000173b0: 7572 6920 6973 206e 6f74 204e 6f6e 650a  uri is not None.
-000173c0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-000173d0: 2063 6f6d 7075 7465 5f6c 6f63 6b3a 0a20   compute_lock:. 
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000173f0: 696c 655f 636f 6e74 656e 742e 7365 656b  ile_content.seek
-00017400: 286f 6666 7365 742c 2069 6f2e 5345 454b  (offset, io.SEEK
-00017410: 5f53 4554 290a 2020 2020 2020 2020 2020  _SET).          
-00017420: 2020 2020 2020 6275 6666 203d 2066 696c        buff = fil
-00017430: 655f 636f 6e74 656e 742e 7265 6164 2875  e_content.read(u
-00017440: 706c 6f61 645f 6368 756e 6b5f 7369 7a65  pload_chunk_size
-00017450: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
-00017460: 775f 7369 7a65 203d 2073 656c 662e 5f61  w_size = self._a
-00017470: 7070 656e 645f 7570 6c6f 6164 280a 2020  ppend_upload(.  
-00017480: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017490: 6c66 2e5f 746d 705f 7572 692c 0a20 2020  lf._tmp_uri,.   
-000174a0: 2020 2020 2020 2020 2020 2020 2042 7974               Byt
-000174b0: 6573 494f 2862 7566 6629 2c0a 2020 2020  esIO(buff),.    
-000174c0: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
-000174d0: 6574 290a 2020 2020 2020 2020 2020 2020  et).            
-000174e0: 6966 206e 6577 5f73 697a 6520 213d 206c  if new_size != l
-000174f0: 656e 2862 7566 6629 3a0a 2020 2020 2020  en(buff):.      
-00017500: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017510: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 6622 696e 636f 6d70 6c65 7465 2063 6875  f"incomplete chu
-00017540: 6e6b 2075 706c 6f61 6420 6e3a 7b6e 6577  nk upload n:{new
-00017550: 5f73 697a 657d 2022 0a20 2020 2020 2020  _size} ".       
-00017560: 2020 2020 2020 2020 2020 2020 2066 2262               f"b
-00017570: 3a7b 6c65 6e28 6275 6666 297d 206f 6666  :{len(buff)} off
-00017580: 7365 743a 207b 6f66 6673 6574 7d22 290a  set: {offset}").
-00017590: 0a20 2020 2020 2020 2063 6f6d 7075 7465  .        compute
-000175a0: 5f70 6172 616c 6c65 6c28 6265 6769 6e73  _parallel(begins
-000175b0: 2c20 636f 6d70 7574 655f 7570 6c6f 6164  , compute_upload
-000175c0: 2c20 7072 696e 745f 7072 6f67 7265 7373  , print_progress
-000175d0: 2c20 6d61 785f 7468 7265 6164 7329 0a0a  , max_threads)..
-000175e0: 2020 2020 6465 6620 7570 6c6f 6164 5f7a      def upload_z
-000175f0: 6970 280a 2020 2020 2020 2020 2020 2020  ip(.            
-00017600: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00017610: 2020 736f 7572 6365 3a20 556e 696f 6e5b    source: Union[
-00017620: 7374 722c 2069 6f2e 4279 7465 7349 4f5d  str, io.BytesIO]
-00017630: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-00017640: 785f 7468 7265 6164 733a 2069 6e74 203d  x_threads: int =
-00017650: 2031 3029 202d 3e20 4c69 7374 5b27 426c   10) -> List['Bl
-00017660: 6f62 4861 6e64 6c65 275d 3a0a 2020 2020  obHandle']:.    
-00017670: 2020 2020 6669 6c65 733a 204c 6973 745b      files: List[
-00017680: 7374 725d 203d 205b 5d0a 2020 2020 2020  str] = [].      
-00017690: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000176a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000176b0: 2873 6f75 7263 652c 2073 7472 2920 6f72  (source, str) or
-000176c0: 206e 6f74 2068 6173 6174 7472 2873 6f75   not hasattr(sou
-000176d0: 7263 652c 2022 7265 6164 2229 3a0a 2020  rce, "read"):.  
-000176e0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-000176f0: 7468 206f 7065 6e28 6622 7b73 6f75 7263  th open(f"{sourc
-00017700: 657d 222c 2022 7262 2229 2061 7320 6669  e}", "rb") as fi
-00017710: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-00017720: 2020 2020 2020 2073 656c 662e 5f75 706c         self._upl
-00017730: 6f61 645f 6669 6c65 2866 696e 2c20 6d61  oad_file(fin, ma
-00017740: 785f 7468 7265 6164 732c 2065 7874 3d22  x_threads, ext="
-00017750: 7a69 7022 290a 2020 2020 2020 2020 2020  zip").          
-00017760: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00017770: 2020 2020 2020 2020 7365 6c66 2e5f 7570          self._up
-00017780: 6c6f 6164 5f66 696c 6528 736f 7572 6365  load_file(source
-00017790: 2c20 6d61 785f 7468 7265 6164 732c 2065  , max_threads, e
-000177a0: 7874 3d22 7a69 7022 290a 2020 2020 2020  xt="zip").      
-000177b0: 2020 2020 2020 6669 6c65 7320 3d20 7365        files = se
-000177c0: 6c66 2e5f 6669 6e69 7368 5f75 706c 6f61  lf._finish_uploa
-000177d0: 645f 7a69 7028 290a 2020 2020 2020 2020  d_zip().        
-000177e0: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
-000177f0: 2020 2020 2073 656c 662e 5f63 6c65 6172       self._clear
-00017800: 5f75 706c 6f61 6428 290a 2020 2020 2020  _upload().      
-00017810: 2020 7265 7475 726e 205b 0a20 2020 2020    return [.     
-00017820: 2020 2020 2020 2042 6c6f 6248 616e 646c         BlobHandl
-00017830: 6528 7365 6c66 2e5f 636c 6965 6e74 2c20  e(self._client, 
-00017840: 626c 6f62 5f75 7269 2c20 6973 5f66 756c  blob_uri, is_ful
-00017850: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
-00017860: 2020 2020 666f 7220 626c 6f62 5f75 7269      for blob_uri
-00017870: 2069 6e20 6669 6c65 730a 2020 2020 2020   in files.      
-00017880: 2020 5d0a 0a20 2020 2064 6566 2075 706c    ]..    def upl
-00017890: 6f61 645f 736b 6c69 6b65 5f6d 6f64 656c  oad_sklike_model
-000178a0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
-000178b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000178c0: 2020 2020 206d 6f64 656c 5f6f 626a 3a20       model_obj: 
-000178d0: 494f 5b62 7974 6573 5d2c 0a20 2020 2020  IO[bytes],.     
-000178e0: 2020 2020 2020 2078 636f 6c73 3a20 4c69         xcols: Li
-000178f0: 7374 5b73 7472 5d2c 0a20 2020 2020 2020  st[str],.       
-00017900: 2020 2020 2069 735f 636c 663a 2062 6f6f       is_clf: boo
-00017910: 6c2c 0a20 2020 2020 2020 2020 2020 206d  l,.            m
-00017920: 6f64 656c 5f6e 616d 653a 2073 7472 2c0a  odel_name: str,.
-00017930: 2020 2020 2020 2020 2020 2020 6d61 7962              mayb
-00017940: 655f 636c 6173 7365 733a 204f 7074 696f  e_classes: Optio
-00017950: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
-00017960: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00017970: 2020 206d 6179 6265 5f72 616e 6765 3a20     maybe_range: 
-00017980: 4f70 7469 6f6e 616c 5b0a 2020 2020 2020  Optional[.      
-00017990: 2020 2020 2020 2020 2020 5475 706c 655b            Tuple[
-000179a0: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d2c  Optional[float],
-000179b0: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-000179c0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-000179d0: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
-000179e0: 6473 3a20 696e 7420 3d20 3130 2c0a 2020  ds: int = 10,.  
-000179f0: 2020 2020 2020 2020 2020 6675 6c6c 5f69            full_i
-00017a00: 6e69 743a 2062 6f6f 6c20 3d20 5472 7565  nit: bool = True
-00017a10: 2920 2d3e 2055 706c 6f61 6446 696c 6573  ) -> UploadFiles
-00017a20: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00017a30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00017a40: 2020 2073 656c 662e 5f75 706c 6f61 645f     self._upload_
-00017a50: 6669 6c65 286d 6f64 656c 5f6f 626a 2c20  file(model_obj, 
-00017a60: 6d61 785f 7468 7265 6164 732c 2065 7874  max_threads, ext
-00017a70: 3d22 706b 6c22 290a 2020 2020 2020 2020  ="pkl").        
-00017a80: 2020 2020 6f75 7470 7574 5f72 616e 6765      output_range
-00017a90: 203d 2028 4e6f 6e65 2c20 4e6f 6e65 2920   = (None, None) 
-00017aa0: 6966 206d 6179 6265 5f72 616e 6765 2069  if maybe_range i
-00017ab0: 7320 4e6f 6e65 2065 6c73 6520 6d61 7962  s None else mayb
-00017ac0: 655f 7261 6e67 650a 2020 2020 2020 2020  e_range.        
-00017ad0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00017ae0: 5f66 696e 6973 685f 7570 6c6f 6164 5f73  _finish_upload_s
-00017af0: 6b6c 696b 6528 0a20 2020 2020 2020 2020  klike(.         
-00017b00: 2020 2020 2020 206d 6f64 656c 5f6e 616d         model_nam
-00017b10: 653d 6d6f 6465 6c5f 6e61 6d65 2c0a 2020  e=model_name,.  
-00017b20: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00017b30: 7962 655f 636c 6173 7365 733d 6d61 7962  ybe_classes=mayb
-00017b40: 655f 636c 6173 7365 732c 0a20 2020 2020  e_classes,.     
-00017b50: 2020 2020 2020 2020 2020 206d 6179 6265             maybe
-00017b60: 5f72 616e 6765 3d6f 7574 7075 745f 7261  _range=output_ra
-00017b70: 6e67 652c 0a20 2020 2020 2020 2020 2020  nge,.           
-00017b80: 2020 2020 2078 636f 6c73 3d78 636f 6c73       xcols=xcols
-00017b90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017ba0: 2020 6973 5f63 6c66 3d69 735f 636c 662c    is_clf=is_clf,
-00017bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017bc0: 2066 756c 6c5f 696e 6974 3d66 756c 6c5f   full_init=full_
-00017bd0: 696e 6974 290a 2020 2020 2020 2020 6669  init).        fi
-00017be0: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
-00017bf0: 2020 2073 656c 662e 5f63 6c65 6172 5f75     self._clear_u
-00017c00: 706c 6f61 6428 290a 0a20 2020 2064 6566  pload()..    def
-00017c10: 2075 706c 6f61 645f 736b 6c69 6b65 5f6d   upload_sklike_m
-00017c20: 6f64 656c 280a 2020 2020 2020 2020 2020  odel(.          
-00017c30: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00017c40: 2020 2020 6d6f 6465 6c3a 2041 6e79 2c0a      model: Any,.
-00017c50: 2020 2020 2020 2020 2020 2020 7863 6f6c              xcol
-00017c60: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
-00017c70: 2020 2020 2020 2020 2020 6973 5f63 6c66            is_clf
-00017c80: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
-00017c90: 2020 2020 6d61 7962 655f 636c 6173 7365      maybe_classe
-00017ca0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00017cb0: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
-00017cc0: 2020 2020 2020 2020 2020 206d 6179 6265             maybe
-00017cd0: 5f72 616e 6765 3a20 4f70 7469 6f6e 616c  _range: Optional
-00017ce0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00017cf0: 2020 5475 706c 655b 4f70 7469 6f6e 616c    Tuple[Optional
-00017d00: 5b66 6c6f 6174 5d2c 204f 7074 696f 6e61  [float], Optiona
-00017d10: 6c5b 666c 6f61 745d 5d5d 203d 204e 6f6e  l[float]]] = Non
-00017d20: 652c 0a20 2020 2020 2020 2020 2020 2066  e,.            f
-00017d30: 756c 6c5f 696e 6974 3a20 626f 6f6c 203d  ull_init: bool =
-00017d40: 2054 7275 6529 202d 3e20 5570 6c6f 6164   True) -> Upload
-00017d50: 4669 6c65 7352 6573 706f 6e73 653a 0a20  FilesResponse:. 
-00017d60: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00017d70: 2020 2020 2020 2020 6d6f 6465 6c5f 6e61          model_na
-00017d80: 6d65 203d 2074 7970 6528 6d6f 6465 6c29  me = type(model)
-00017d90: 2e5f 5f6e 616d 655f 5f0a 2020 2020 2020  .__name__.      
-00017da0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00017db0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00017dc0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00017dd0: 4572 726f 7228 6622 6361 6e20 6e6f 7420  Error(f"can not 
-00017de0: 696e 6665 7220 6d6f 6465 6c20 6e61 6d65  infer model name
-00017df0: 207b 6d6f 6465 6c7d 2229 2066 726f 6d20   {model}") from 
-00017e00: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
-00017e10: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00017e20: 5f63 6c66 2061 6e64 206d 6179 6265 5f63  _clf and maybe_c
-00017e30: 6c61 7373 6573 2069 7320 4e6f 6e65 3a0a  lasses is None:.
-00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e50: 6d61 7962 655f 636c 6173 7365 7320 3d20  maybe_classes = 
-00017e60: 6d6f 6465 6c2e 636c 6173 7365 735f 0a20  model.classes_. 
-00017e70: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00017e80: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-00017e90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017ea0: 5661 6c75 6545 7272 6f72 2866 2263 616e  ValueError(f"can
-00017eb0: 206e 6f74 2069 6e66 6572 2063 6c61 7373   not infer class
-00017ec0: 6573 2066 726f 6d20 7b6d 6f64 656c 7d22  es from {model}"
-00017ed0: 2920 6672 6f6d 2065 0a20 2020 2020 2020  ) from e.       
-00017ee0: 2064 756d 7020 3d20 7069 636b 6c65 2e64   dump = pickle.d
-00017ef0: 756d 7073 286d 6f64 656c 2c20 7069 636b  umps(model, pick
-00017f00: 6c65 2e48 4947 4845 5354 5f50 524f 544f  le.HIGHEST_PROTO
-00017f10: 434f 4c29 0a20 2020 2020 2020 2077 6974  COL).        wit
-00017f20: 6820 696f 2e42 7974 6573 494f 2864 756d  h io.BytesIO(dum
-00017f30: 7029 2061 7320 6275 6666 6572 3a0a 2020  p) as buffer:.  
-00017f40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017f50: 2073 656c 662e 7570 6c6f 6164 5f73 6b6c   self.upload_skl
-00017f60: 696b 655f 6d6f 6465 6c5f 6669 6c65 280a  ike_model_file(.
-00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f80: 6275 6666 6572 2c0a 2020 2020 2020 2020  buffer,.        
-00017f90: 2020 2020 2020 2020 7863 6f6c 732c 0a20          xcols,. 
-00017fa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00017fb0: 735f 636c 662c 0a20 2020 2020 2020 2020  s_clf,.         
-00017fc0: 2020 2020 2020 206d 6f64 656c 5f6e 616d         model_nam
-00017fd0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00017fe0: 2020 206d 6179 6265 5f63 6c61 7373 6573     maybe_classes
-00017ff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018000: 2020 6d61 7962 655f 7261 6e67 652c 0a20    maybe_range,. 
-00018010: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00018020: 756c 6c5f 696e 6974 290a 0a20 2020 2064  ull_init)..    d
-00018030: 6566 2063 6f6e 7665 7274 5f6d 6f64 656c  ef convert_model
-00018040: 2873 656c 662c 2072 656c 6f61 643a 2062  (self, reload: b
-00018050: 6f6f 6c20 3d20 5472 7565 2920 2d3e 204d  ool = True) -> M
-00018060: 6f64 656c 5265 6c65 6173 6552 6573 706f  odelReleaseRespo
-00018070: 6e73 653a 0a20 2020 2020 2020 2072 6574  nse:.        ret
-00018080: 7572 6e20 6361 7374 284d 6f64 656c 5265  urn cast(ModelRe
-00018090: 6c65 6173 6552 6573 706f 6e73 652c 2073  leaseResponse, s
-000180a0: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
-000180b0: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
-000180c0: 2020 2020 2020 4d45 5448 4f44 5f50 4f53        METHOD_POS
-000180d0: 542c 2022 2f63 6f6e 7665 7274 5f6d 6f64  T, "/convert_mod
-000180e0: 656c 222c 207b 0a20 2020 2020 2020 2020  el", {.         
-000180f0: 2020 2020 2020 2022 626c 6f62 223a 2073         "blob": s
-00018100: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
-00018110: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00018120: 7265 6c6f 6164 223a 2072 656c 6f61 642c  reload": reload,
-00018130: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
-00018140: 0a0a 2020 2020 6465 6620 6465 6c65 7465  ..    def delete
-00018150: 2873 656c 6629 202d 3e20 4465 6c65 7465  (self) -> Delete
-00018160: 426c 6f62 5265 7370 6f6e 7365 3a0a 2020  BlobResponse:.  
-00018170: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
-00018180: 7428 4465 6c65 7465 426c 6f62 5265 7370  t(DeleteBlobResp
-00018190: 6f6e 7365 2c20 7365 6c66 2e5f 636c 6965  onse, self._clie
-000181a0: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
-000181b0: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
-000181c0: 484f 445f 4445 4c45 5445 2c20 222f 626c  HOD_DELETE, "/bl
-000181d0: 6f62 222c 207b 0a20 2020 2020 2020 2020  ob", {.         
-000181e0: 2020 2020 2020 2022 626c 6f62 5f75 7269         "blob_uri
-000181f0: 7322 3a20 5b73 656c 662e 6765 745f 7572  s": [self.get_ur
-00018200: 6928 295d 2c0a 2020 2020 2020 2020 2020  i()],.          
-00018210: 2020 7d2c 0a20 2020 2020 2020 2029 290a    },.        )).
-00018220: 0a20 2020 2064 6566 2067 6574 5f6d 6f64  .    def get_mod
-00018230: 656c 5f72 656c 6561 7365 2873 656c 6629  el_release(self)
-00018240: 202d 3e20 4d6f 6465 6c52 656c 6561 7365   -> ModelRelease
-00018250: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00018260: 2020 7265 7475 726e 2063 6173 7428 4d6f    return cast(Mo
-00018270: 6465 6c52 656c 6561 7365 5265 7370 6f6e  delReleaseRespon
-00018280: 7365 2c20 7365 6c66 2e5f 636c 6965 6e74  se, self._client
-00018290: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
-000182a0: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
-000182b0: 445f 4745 542c 2022 2f6d 6f64 656c 5f72  D_GET, "/model_r
-000182c0: 656c 6561 7365 222c 207b 0a20 2020 2020  elease", {.     
-000182d0: 2020 2020 2020 2020 2020 2022 626c 6f62             "blob
-000182e0: 223a 2073 656c 662e 6765 745f 7572 6928  ": self.get_uri(
-000182f0: 292c 0a20 2020 2020 2020 2020 2020 207d  ),.            }
-00018300: 2929 0a0a 2020 2020 6465 6620 6765 745f  ))..    def get_
-00018310: 6d6f 6465 6c5f 7665 7273 696f 6e28 7365  model_version(se
-00018320: 6c66 2920 2d3e 204d 6f64 656c 5665 7273  lf) -> ModelVers
-00018330: 696f 6e52 6573 706f 6e73 653a 0a20 2020  ionResponse:.   
-00018340: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
-00018350: 284d 6f64 656c 5665 7273 696f 6e52 6573  (ModelVersionRes
-00018360: 706f 6e73 652c 2073 656c 662e 5f63 6c69  ponse, self._cli
-00018370: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-00018380: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-00018390: 5448 4f44 5f47 4554 2c20 222f 6d6f 6465  THOD_GET, "/mode
-000183a0: 6c5f 7665 7273 696f 6e22 2c20 7b0a 2020  l_version", {.  
-000183b0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000183c0: 6f64 656c 5f75 7269 223a 2073 656c 662e  odel_uri": self.
-000183d0: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
-000183e0: 2020 2020 2020 207d 2929 0a0a 2020 2020         }))..    
-000183f0: 6465 6620 5f63 6f70 795f 6d6f 6465 6c5f  def _copy_model_
-00018400: 7665 7273 696f 6e28 0a20 2020 2020 2020  version(.       
-00018410: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00018420: 2020 2020 2020 206d 6f64 656c 5f75 7269         model_uri
-00018430: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
-00018440: 2020 2072 6561 645f 7665 7273 696f 6e3a     read_version:
-00018450: 204f 7074 696f 6e61 6c5b 696e 745d 2c0a   Optional[int],.
-00018460: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00018470: 655f 7665 7273 696f 6e3a 2069 6e74 2c0a  e_version: int,.
-00018480: 2020 2020 2020 2020 2020 2020 6f76 6572              over
-00018490: 7772 6974 653a 2062 6f6f 6c29 202d 3e20  write: bool) -> 
-000184a0: 4d6f 6465 6c56 6572 7369 6f6e 5265 7370  ModelVersionResp
-000184b0: 6f6e 7365 3a0a 2020 2020 2020 2020 7265  onse:.        re
-000184c0: 7475 726e 2063 6173 7428 4d6f 6465 6c56  turn cast(ModelV
-000184d0: 6572 7369 6f6e 5265 7370 6f6e 7365 2c20  ersionResponse, 
-000184e0: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
-000184f0: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-00018500: 2020 2020 2020 204d 4554 484f 445f 5055         METHOD_PU
-00018510: 542c 2022 2f6d 6f64 656c 5f76 6572 7369  T, "/model_versi
-00018520: 6f6e 222c 207b 0a20 2020 2020 2020 2020  on", {.         
-00018530: 2020 2020 2020 2022 6d6f 6465 6c5f 7572         "model_ur
-00018540: 6922 3a20 6d6f 6465 6c5f 7572 692c 0a20  i": model_uri,. 
-00018550: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00018560: 7265 6164 5f76 6572 7369 6f6e 223a 2072  read_version": r
-00018570: 6561 645f 7665 7273 696f 6e2c 0a20 2020  ead_version,.   
-00018580: 2020 2020 2020 2020 2020 2020 2022 7772               "wr
-00018590: 6974 655f 7665 7273 696f 6e22 3a20 7772  ite_version": wr
-000185a0: 6974 655f 7665 7273 696f 6e2c 0a20 2020  ite_version,.   
-000185b0: 2020 2020 2020 2020 2020 2020 2022 6f76               "ov
-000185c0: 6572 7772 6974 6522 3a20 6f76 6572 7772  erwrite": overwr
-000185d0: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-000185e0: 207d 2929 0a0a 2020 2020 6465 6620 636f   }))..    def co
-000185f0: 7079 5f6d 6f64 656c 5f76 6572 7369 6f6e  py_model_version
-00018600: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00018610: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00018620: 7265 6164 5f76 6572 7369 6f6e 3a20 696e  read_version: in
-00018630: 742c 0a20 2020 2020 2020 2020 2020 2077  t,.            w
-00018640: 7269 7465 5f76 6572 7369 6f6e 3a20 696e  rite_version: in
-00018650: 742c 0a20 2020 2020 2020 2020 2020 206f  t,.            o
-00018660: 7665 7277 7269 7465 3a20 626f 6f6c 2920  verwrite: bool) 
-00018670: 2d3e 204d 6f64 656c 5665 7273 696f 6e52  -> ModelVersionR
-00018680: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00018690: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
-000186a0: 7079 5f6d 6f64 656c 5f76 6572 7369 6f6e  py_model_version
-000186b0: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
-000186c0: 6465 6c5f 7572 693d 7365 6c66 2e67 6574  del_uri=self.get
-000186d0: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
-000186e0: 2020 2020 7265 6164 5f76 6572 7369 6f6e      read_version
-000186f0: 3d72 6561 645f 7665 7273 696f 6e2c 0a20  =read_version,. 
-00018700: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00018710: 5f76 6572 7369 6f6e 3d77 7269 7465 5f76  _version=write_v
-00018720: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
-00018730: 2020 2020 6f76 6572 7772 6974 653d 6f76      overwrite=ov
-00018740: 6572 7772 6974 6529 0a0a 2020 2020 6465  erwrite)..    de
-00018750: 6620 6465 6c65 7465 5f6d 6f64 656c 5f76  f delete_model_v
-00018760: 6572 7369 6f6e 2873 656c 662c 2076 6572  ersion(self, ver
-00018770: 7369 6f6e 3a20 696e 7429 202d 3e20 4d6f  sion: int) -> Mo
-00018780: 6465 6c56 6572 7369 6f6e 5265 7370 6f6e  delVersionRespon
-00018790: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-000187a0: 726e 2073 656c 662e 5f63 6f70 795f 6d6f  rn self._copy_mo
-000187b0: 6465 6c5f 7665 7273 696f 6e28 0a20 2020  del_version(.   
-000187c0: 2020 2020 2020 2020 206d 6f64 656c 5f75           model_u
-000187d0: 7269 3d73 656c 662e 6765 745f 7572 6928  ri=self.get_uri(
-000187e0: 292c 0a20 2020 2020 2020 2020 2020 2072  ),.            r
-000187f0: 6561 645f 7665 7273 696f 6e3d 4e6f 6e65  ead_version=None
-00018800: 2c0a 2020 2020 2020 2020 2020 2020 7772  ,.            wr
-00018810: 6974 655f 7665 7273 696f 6e3d 7665 7273  ite_version=vers
-00018820: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00018830: 206f 7665 7277 7269 7465 3d54 7275 6529   overwrite=True)
-00018840: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
-00018850: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
-00018860: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018870: 6861 7368 2873 656c 662e 6173 5f73 7472  hash(self.as_str
-00018880: 2829 290a 0a20 2020 2064 6566 205f 5f65  ())..    def __e
-00018890: 715f 5f28 7365 6c66 2c20 6f74 6865 723a  q__(self, other:
-000188a0: 206f 626a 6563 7429 202d 3e20 626f 6f6c   object) -> bool
-000188b0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-000188c0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-000188d0: 722c 2073 656c 662e 5f5f 636c 6173 735f  r, self.__class_
-000188e0: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
-000188f0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00018900: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00018910: 2e61 735f 7374 7228 2920 3d3d 206f 7468  .as_str() == oth
-00018920: 6572 2e61 735f 7374 7228 290a 0a20 2020  er.as_str()..   
-00018930: 2064 6566 205f 5f6e 655f 5f28 7365 6c66   def __ne__(self
-00018940: 2c20 6f74 6865 723a 206f 626a 6563 7429  , other: object)
-00018950: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00018960: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
-00018970: 662e 5f5f 6571 5f5f 286f 7468 6572 290a  f.__eq__(other).
-00018980: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
-00018990: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-000189a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000189b0: 6c66 2e61 735f 7374 7228 290a 0a20 2020  lf.as_str()..   
-000189c0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-000189d0: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
-000189e0: 2020 2020 7265 7475 726e 2066 227b 7365      return f"{se
-000189f0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
-00018a00: 616d 655f 5f7d 5b7b 7365 6c66 2e61 735f  ame__}[{self.as_
-00018a10: 7374 7228 297d 5d22 0a0a 2320 2a2a 2a20  str()}]"..# *** 
-00018a20: 426c 6f62 4861 6e64 6c65 202a 2a2a 0a0a  BlobHandle ***..
-00018a30: 0a63 6c61 7373 2043 5356 426c 6f62 4861  .class CSVBlobHa
-00018a40: 6e64 6c65 2842 6c6f 6248 616e 646c 6529  ndle(BlobHandle)
-00018a50: 3a0a 2020 2020 6465 6620 6669 6e69 7368  :.    def finish
-00018a60: 5f63 7376 5f75 706c 6f61 6428 0a20 2020  _csv_upload(.   
-00018a70: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00018a80: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-00018a90: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-00018aa0: 725d 203d 204e 6f6e 6529 202d 3e20 5570  r] = None) -> Up
-00018ab0: 6c6f 6164 4669 6c65 7352 6573 706f 6e73  loadFilesRespons
-00018ac0: 653a 0a20 2020 2020 2020 2074 6d70 5f75  e:.        tmp_u
-00018ad0: 7269 203d 2073 656c 662e 5f74 6d70 5f75  ri = self._tmp_u
-00018ae0: 7269 0a20 2020 2020 2020 2069 6620 746d  ri.        if tm
-00018af0: 705f 7572 6920 6973 204e 6f6e 653a 0a20  p_uri is None:. 
-00018b00: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00018b10: 2056 616c 7565 4572 726f 7228 2274 6d70   ValueError("tmp
-00018b20: 5f75 7269 2069 7320 4e6f 6e65 2229 0a20  _uri is None"). 
-00018b30: 2020 2020 2020 2061 7267 733a 2044 6963         args: Dic
-00018b40: 745b 7374 722c 204f 7074 696f 6e61 6c5b  t[str, Optional[
-00018b50: 556e 696f 6e5b 7374 722c 2069 6e74 5d5d  Union[str, int]]
-00018b60: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
-00018b70: 2020 2274 6d70 5f75 7269 223a 2074 6d70    "tmp_uri": tmp
-00018b80: 5f75 7269 2c0a 2020 2020 2020 2020 2020  _uri,.          
-00018b90: 2020 2263 7376 5f75 7269 223a 2073 656c    "csv_uri": sel
-00018ba0: 662e 6765 745f 7572 6928 292c 0a20 2020  f.get_uri(),.   
-00018bb0: 2020 2020 2020 2020 2022 6f77 6e65 725f           "owner_
-00018bc0: 6461 6722 3a20 7365 6c66 2e67 6574 5f6f  dag": self.get_o
-00018bd0: 776e 6572 5f64 6167 2829 2c0a 2020 2020  wner_dag(),.    
-00018be0: 2020 2020 2020 2020 226f 776e 6572 5f6e          "owner_n
-00018bf0: 6f64 6522 3a20 7365 6c66 2e67 6574 5f6f  ode": self.get_o
-00018c00: 776e 6572 5f6e 6f64 6528 292c 0a20 2020  wner_node(),.   
-00018c10: 2020 2020 2020 2020 2022 6669 6c65 6e61           "filena
-00018c20: 6d65 223a 2066 696c 656e 616d 652c 0a20  me": filename,. 
-00018c30: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00018c40: 2072 6574 7572 6e20 6361 7374 2855 706c   return cast(Upl
-00018c50: 6f61 6446 696c 6573 5265 7370 6f6e 7365  oadFilesResponse
-00018c60: 2c20 7365 6c66 2e5f 636c 6965 6e74 2e72  , self._client.r
-00018c70: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
-00018c80: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
-00018c90: 504f 5354 2c20 222f 6669 6e69 7368 5f63  POST, "/finish_c
-00018ca0: 7376 222c 2061 7267 7329 290a 0a20 2020  sv", args))..   
-00018cb0: 2064 6566 2061 6464 5f66 726f 6d5f 6669   def add_from_fi
-00018cc0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00018cd0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00018ce0: 2020 6669 6c65 6e61 6d65 3a20 7374 722c    filename: str,
-00018cf0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00018d00: 6772 6573 735f 6261 723a 204f 7074 696f  gress_bar: Optio
-00018d10: 6e61 6c5b 494f 5b41 6e79 5d5d 203d 2073  nal[IO[Any]] = s
-00018d20: 7973 2e73 7464 6f75 742c 0a20 2020 2020  ys.stdout,.     
-00018d30: 2020 2020 2020 2072 6571 7565 7565 5f6f         requeue_o
-00018d40: 6e5f 6669 6e69 7368 3a20 4f70 7469 6f6e  n_finish: Option
-00018d50: 616c 5b4e 6f64 6548 616e 646c 655d 203d  al[NodeHandle] =
-00018d60: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00018d70: 2020 206d 6178 5f74 6872 6561 6473 3a20     max_threads: 
-00018d80: 696e 7420 3d20 3130 2920 2d3e 204f 7074  int = 10) -> Opt
-00018d90: 696f 6e61 6c5b 5570 6c6f 6164 4669 6c65  ional[UploadFile
-00018da0: 7352 6573 706f 6e73 655d 3a0a 2020 2020  sResponse]:.    
-00018db0: 2020 2020 666e 616d 6520 3d20 6669 6c65      fname = file
-00018dc0: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-00018dd0: 6669 6c65 6e61 6d65 2e65 6e64 7377 6974  filename.endswit
-00018de0: 6828 494e 5055 545f 5a49 505f 4558 5429  h(INPUT_ZIP_EXT)
-00018df0: 3a0a 2020 2020 2020 2020 2020 2020 666e  :.            fn
-00018e00: 616d 6520 3d20 6669 6c65 6e61 6d65 5b3a  ame = filename[:
-00018e10: 2d6c 656e 2849 4e50 5554 5f5a 4950 5f45  -len(INPUT_ZIP_E
-00018e20: 5854 295d 0a20 2020 2020 2020 2065 7874  XT)].        ext
-00018e30: 5f70 6f73 203d 2066 6e61 6d65 2e72 6669  _pos = fname.rfi
-00018e40: 6e64 2822 2e22 290a 2020 2020 2020 2020  nd(".").        
-00018e50: 6966 2065 7874 5f70 6f73 203e 3d20 303a  if ext_pos >= 0:
-00018e60: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-00018e70: 203d 2066 696c 656e 616d 655b 6578 745f   = filename[ext_
-00018e80: 706f 7320 2b20 313a 5d20 2023 2066 756c  pos + 1:]  # ful
-00018e90: 6c20 6669 6c65 6e61 6d65 0a20 2020 2020  l filename.     
-00018ea0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00018eb0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00018ec0: 4572 726f 7228 2263 6f75 6c64 206e 6f74  Error("could not
-00018ed0: 2064 6574 6572 6d69 6e65 2065 7874 656e   determine exten
-00018ee0: 7369 6f6e 2229 0a20 2020 2020 2020 2074  sion").        t
-00018ef0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00018f00: 7769 7468 206f 7065 6e28 6669 6c65 6e61  with open(filena
-00018f10: 6d65 2c20 2272 6222 2920 6173 2066 6275  me, "rb") as fbu
-00018f20: 6666 3a0a 2020 2020 2020 2020 2020 2020  ff:.            
-00018f30: 2020 2020 7365 6c66 2e5f 7570 6c6f 6164      self._upload
-00018f40: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
-00018f50: 2020 2020 2020 2020 2020 2066 6275 6666             fbuff
-00018f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018f70: 2020 2020 2020 6d61 785f 7468 7265 6164        max_thread
-00018f80: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00018f90: 2020 2020 2020 2065 7874 3d65 7874 2c0a         ext=ext,.
-00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fb0: 2020 2020 7072 6f67 7265 7373 5f62 6172      progress_bar
-00018fc0: 3d70 726f 6772 6573 735f 6261 7229 0a20  =progress_bar). 
-00018fd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00018fe0: 6e20 7365 6c66 2e66 696e 6973 685f 6373  n self.finish_cs
-00018ff0: 765f 7570 6c6f 6164 2866 696c 656e 616d  v_upload(filenam
-00019000: 6529 0a20 2020 2020 2020 2066 696e 616c  e).        final
-00019010: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
-00019020: 6966 2072 6571 7565 7565 5f6f 6e5f 6669  if requeue_on_fi
-00019030: 6e69 7368 2069 7320 6e6f 7420 4e6f 6e65  nish is not None
-00019040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019050: 2020 7265 7175 6575 655f 6f6e 5f66 696e    requeue_on_fin
-00019060: 6973 682e 7265 7175 6575 6528 290a 2020  ish.requeue().  
-00019070: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00019080: 636c 6561 725f 7570 6c6f 6164 2829 0a0a  clear_upload()..
-00019090: 2020 2020 6465 6620 6164 645f 6672 6f6d      def add_from
-000190a0: 5f64 6628 0a20 2020 2020 2020 2020 2020  _df(.           
-000190b0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-000190c0: 2020 2064 663a 2070 642e 4461 7461 4672     df: pd.DataFr
-000190d0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-000190e0: 2070 726f 6772 6573 735f 6261 723a 204f   progress_bar: O
-000190f0: 7074 696f 6e61 6c5b 494f 5b41 6e79 5d5d  ptional[IO[Any]]
-00019100: 203d 2073 7973 2e73 7464 6f75 742c 0a20   = sys.stdout,. 
-00019110: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-00019120: 7565 5f6f 6e5f 6669 6e69 7368 3a20 4f70  ue_on_finish: Op
-00019130: 7469 6f6e 616c 5b4e 6f64 6548 616e 646c  tional[NodeHandl
-00019140: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
-00019150: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
-00019160: 6473 3a20 696e 7420 3d20 3130 2920 2d3e  ds: int = 10) ->
-00019170: 204f 7074 696f 6e61 6c5b 5570 6c6f 6164   Optional[Upload
-00019180: 4669 6c65 7352 6573 706f 6e73 655d 3a0a  FilesResponse]:.
-00019190: 2020 2020 2020 2020 696f 5f69 6e20 3d20          io_in = 
-000191a0: 4e6f 6e65 0a20 2020 2020 2020 2074 7279  None.        try
-000191b0: 3a0a 2020 2020 2020 2020 2020 2020 696f  :.            io
-000191c0: 5f69 6e20 3d20 6466 5f74 6f5f 6373 765f  _in = df_to_csv_
-000191d0: 6279 7465 7328 6466 290a 2020 2020 2020  bytes(df).      
-000191e0: 2020 2020 2020 7365 6c66 2e5f 7570 6c6f        self._uplo
-000191f0: 6164 5f66 696c 6528 0a20 2020 2020 2020  ad_file(.       
-00019200: 2020 2020 2020 2020 2069 6f5f 696e 2c0a           io_in,.
-00019210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019220: 6d61 785f 7468 7265 6164 732c 0a20 2020  max_threads,.   
-00019230: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-00019240: 3d22 6373 7622 2c0a 2020 2020 2020 2020  ="csv",.        
-00019250: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-00019260: 5f62 6172 3d70 726f 6772 6573 735f 6261  _bar=progress_ba
-00019270: 7229 0a20 2020 2020 2020 2020 2020 2072  r).            r
-00019280: 6574 7572 6e20 7365 6c66 2e66 696e 6973  eturn self.finis
-00019290: 685f 6373 765f 7570 6c6f 6164 2829 0a20  h_csv_upload(). 
-000192a0: 2020 2020 2020 2066 696e 616c 6c79 3a0a         finally:.
-000192b0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-000192c0: 6571 7565 7565 5f6f 6e5f 6669 6e69 7368  equeue_on_finish
-000192d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000192e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000192f0: 7175 6575 655f 6f6e 5f66 696e 6973 682e  queue_on_finish.
-00019300: 7265 7175 6575 6528 290a 2020 2020 2020  requeue().      
-00019310: 2020 2020 2020 6966 2069 6f5f 696e 2069        if io_in i
-00019320: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00019330: 2020 2020 2020 2020 2020 2020 696f 5f69              io_i
-00019340: 6e2e 636c 6f73 6528 290a 2020 2020 2020  n.close().      
-00019350: 2020 2020 2020 7365 6c66 2e5f 636c 6561        self._clea
-00019360: 725f 7570 6c6f 6164 2829 0a0a 2020 2020  r_upload()..    
-00019370: 6465 6620 6164 645f 6672 6f6d 5f63 6f6e  def add_from_con
-00019380: 7465 6e74 280a 2020 2020 2020 2020 2020  tent(.          
-00019390: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000193a0: 2020 2020 636f 6e74 656e 743a 2055 6e69      content: Uni
-000193b0: 6f6e 5b62 7974 6573 2c20 7374 722c 2070  on[bytes, str, p
-000193c0: 642e 4461 7461 4672 616d 655d 2c0a 2020  d.DataFrame],.  
-000193d0: 2020 2020 2020 2020 2020 7072 6f67 7265            progre
-000193e0: 7373 5f62 6172 3a20 4f70 7469 6f6e 616c  ss_bar: Optional
-000193f0: 5b49 4f5b 416e 795d 5d20 3d20 7379 732e  [IO[Any]] = sys.
-00019400: 7374 646f 7574 2c0a 2020 2020 2020 2020  stdout,.        
-00019410: 2020 2020 7265 7175 6575 655f 6f6e 5f66      requeue_on_f
-00019420: 696e 6973 683a 204f 7074 696f 6e61 6c5b  inish: Optional[
-00019430: 4e6f 6465 4861 6e64 6c65 5d20 3d20 4e6f  NodeHandle] = No
-00019440: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00019450: 6d61 785f 7468 7265 6164 733a 2069 6e74  max_threads: int
-00019460: 203d 2031 3029 202d 3e20 4f70 7469 6f6e   = 10) -> Option
-00019470: 616c 5b55 706c 6f61 6446 696c 6573 5265  al[UploadFilesRe
-00019480: 7370 6f6e 7365 5d3a 0a20 2020 2020 2020  sponse]:.       
-00019490: 2069 6f5f 696e 203d 204e 6f6e 650a 2020   io_in = None.  
-000194a0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000194b0: 2020 2020 2020 2069 6f5f 696e 203d 2063         io_in = c
-000194c0: 6f6e 7465 6e74 5f74 6f5f 6373 765f 6279  ontent_to_csv_by
-000194d0: 7465 7328 636f 6e74 656e 7429 0a20 2020  tes(content).   
-000194e0: 2020 2020 2020 2020 2073 656c 662e 5f75           self._u
-000194f0: 706c 6f61 645f 6669 6c65 280a 2020 2020  pload_file(.    
-00019500: 2020 2020 2020 2020 2020 2020 696f 5f69              io_i
-00019510: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00019520: 2020 206d 6178 5f74 6872 6561 6473 2c0a     max_threads,.
-00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019540: 6578 743d 2263 7376 222c 0a20 2020 2020  ext="csv",.     
-00019550: 2020 2020 2020 2020 2020 2070 726f 6772             progr
-00019560: 6573 735f 6261 723d 7072 6f67 7265 7373  ess_bar=progress
-00019570: 5f62 6172 290a 2020 2020 2020 2020 2020  _bar).          
-00019580: 2020 7265 7475 726e 2073 656c 662e 6669    return self.fi
-00019590: 6e69 7368 5f63 7376 5f75 706c 6f61 6428  nish_csv_upload(
-000195a0: 290a 2020 2020 2020 2020 6669 6e61 6c6c  ).        finall
-000195b0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-000195c0: 6620 7265 7175 6575 655f 6f6e 5f66 696e  f requeue_on_fin
-000195d0: 6973 6820 6973 206e 6f74 204e 6f6e 653a  ish is not None:
-000195e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000195f0: 2072 6571 7565 7565 5f6f 6e5f 6669 6e69   requeue_on_fini
-00019600: 7368 2e72 6571 7565 7565 2829 0a20 2020  sh.requeue().   
-00019610: 2020 2020 2020 2020 2069 6620 696f 5f69           if io_i
-00019620: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00019630: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00019640: 6f5f 696e 2e63 6c6f 7365 2829 0a20 2020  o_in.close().   
-00019650: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00019660: 6c65 6172 5f75 706c 6f61 6428 290a 0a23  lear_upload()..#
-00019670: 202a 2a2a 2043 5356 426c 6f62 4861 6e64   *** CSVBlobHand
-00019680: 6c65 202a 2a2a 0a0a 0a63 6c61 7373 2054  le ***...class T
-00019690: 6f72 6368 426c 6f62 4861 6e64 6c65 2842  orchBlobHandle(B
-000196a0: 6c6f 6248 616e 646c 6529 3a0a 2020 2020  lobHandle):.    
-000196b0: 6465 6620 6669 6e69 7368 5f74 6f72 6368  def finish_torch
-000196c0: 5f75 706c 6f61 6428 0a20 2020 2020 2020  _upload(.       
-000196d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000196e0: 2020 2020 2020 2066 696c 656e 616d 653a         filename:
-000196f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00019700: 204e 6f6e 6529 202d 3e20 5570 6c6f 6164   None) -> Upload
-00019710: 4669 6c65 7352 6573 706f 6e73 653a 0a20  FilesResponse:. 
-00019720: 2020 2020 2020 2074 6d70 5f75 7269 203d         tmp_uri =
-00019730: 2073 656c 662e 5f74 6d70 5f75 7269 0a20   self._tmp_uri. 
-00019740: 2020 2020 2020 2069 6620 746d 705f 7572         if tmp_ur
-00019750: 6920 6973 204e 6f6e 653a 0a20 2020 2020  i is None:.     
-00019760: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00019770: 7565 4572 726f 7228 2274 6d70 5f75 7269  ueError("tmp_uri
-00019780: 2069 7320 4e6f 6e65 2229 0a20 2020 2020   is None").     
-00019790: 2020 2061 7267 733a 2044 6963 745b 7374     args: Dict[st
-000197a0: 722c 204f 7074 696f 6e61 6c5b 556e 696f  r, Optional[Unio
-000197b0: 6e5b 7374 722c 2069 6e74 5d5d 5d20 3d20  n[str, int]]] = 
-000197c0: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
-000197d0: 6d70 5f75 7269 223a 2074 6d70 5f75 7269  mp_uri": tmp_uri
-000197e0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-000197f0: 6f72 6368 5f75 7269 223a 2073 656c 662e  orch_uri": self.
-00019800: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
-00019810: 2020 2020 2020 2022 6f77 6e65 725f 6461         "owner_da
-00019820: 6722 3a20 7365 6c66 2e67 6574 5f6f 776e  g": self.get_own
-00019830: 6572 5f64 6167 2829 2c0a 2020 2020 2020  er_dag(),.      
-00019840: 2020 2020 2020 226f 776e 6572 5f6e 6f64        "owner_nod
-00019850: 6522 3a20 7365 6c66 2e67 6574 5f6f 776e  e": self.get_own
-00019860: 6572 5f6e 6f64 6528 292c 0a20 2020 2020  er_node(),.     
-00019870: 2020 2020 2020 2022 6669 6c65 6e61 6d65         "filename
-00019880: 223a 2066 696c 656e 616d 652c 0a20 2020  ": filename,.   
-00019890: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
-000198a0: 6574 7572 6e20 6361 7374 2855 706c 6f61  eturn cast(Uploa
-000198b0: 6446 696c 6573 5265 7370 6f6e 7365 2c20  dFilesResponse, 
-000198c0: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
-000198d0: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-000198e0: 2020 2020 2020 204d 4554 484f 445f 504f         METHOD_PO
-000198f0: 5354 2c20 222f 6669 6e69 7368 5f74 6f72  ST, "/finish_tor
-00019900: 6368 222c 2061 7267 7329 290a 0a20 2020  ch", args))..   
-00019910: 2064 6566 2061 6464 5f66 726f 6d5f 6669   def add_from_fi
-00019920: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00019930: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00019940: 2020 6669 6c65 6e61 6d65 3a20 7374 722c    filename: str,
-00019950: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00019960: 6772 6573 735f 6261 723a 204f 7074 696f  gress_bar: Optio
-00019970: 6e61 6c5b 494f 5b41 6e79 5d5d 203d 2073  nal[IO[Any]] = s
-00019980: 7973 2e73 7464 6f75 742c 0a20 2020 2020  ys.stdout,.     
-00019990: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
-000199a0: 6473 3a20 696e 7420 3d20 3130 2920 2d3e  ds: int = 10) ->
-000199b0: 204f 7074 696f 6e61 6c5b 5570 6c6f 6164   Optional[Upload
-000199c0: 4669 6c65 7352 6573 706f 6e73 655d 3a0a  FilesResponse]:.
-000199d0: 2020 2020 2020 2020 666e 616d 6520 3d20          fname = 
-000199e0: 6669 6c65 6e61 6d65 0a20 2020 2020 2020  filename.       
-000199f0: 2069 6620 6669 6c65 6e61 6d65 2e65 6e64   if filename.end
-00019a00: 7377 6974 6828 494e 5055 545f 5a49 505f  swith(INPUT_ZIP_
-00019a10: 4558 5429 3a0a 2020 2020 2020 2020 2020  EXT):.          
-00019a20: 2020 666e 616d 6520 3d20 6669 6c65 6e61    fname = filena
-00019a30: 6d65 5b3a 2d6c 656e 2849 4e50 5554 5f5a  me[:-len(INPUT_Z
-00019a40: 4950 5f45 5854 295d 0a20 2020 2020 2020  IP_EXT)].       
-00019a50: 2065 7874 5f70 6f73 203d 2066 6e61 6d65   ext_pos = fname
-00019a60: 2e72 6669 6e64 2822 2e22 290a 2020 2020  .rfind(".").    
-00019a70: 2020 2020 6966 2065 7874 5f70 6f73 203e      if ext_pos >
-00019a80: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00019a90: 2065 7874 203d 2066 696c 656e 616d 655b   ext = filename[
-00019aa0: 6578 745f 706f 7320 2b20 313a 5d20 2023  ext_pos + 1:]  #
-00019ab0: 2066 756c 6c20 6669 6c65 6e61 6d65 0a20   full filename. 
-00019ac0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00019ad0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00019ae0: 616c 7565 4572 726f 7228 2263 6f75 6c64  alueError("could
-00019af0: 206e 6f74 2064 6574 6572 6d69 6e65 2065   not determine e
-00019b00: 7874 656e 7369 6f6e 2229 0a20 2020 2020  xtension").     
-00019b10: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00019b20: 2020 2020 7769 7468 206f 7065 6e28 6669      with open(fi
-00019b30: 6c65 6e61 6d65 2c20 2272 6222 2920 6173  lename, "rb") as
-00019b40: 2066 6275 6666 3a0a 2020 2020 2020 2020   fbuff:.        
-00019b50: 2020 2020 2020 2020 7365 6c66 2e5f 7570          self._up
-00019b60: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
-00019b70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019b80: 6275 6666 2c0a 2020 2020 2020 2020 2020  buff,.          
-00019b90: 2020 2020 2020 2020 2020 6d61 785f 7468            max_th
-00019ba0: 7265 6164 732c 0a20 2020 2020 2020 2020  reads,.         
-00019bb0: 2020 2020 2020 2020 2020 2065 7874 3d65             ext=e
-00019bc0: 7874 2c0a 2020 2020 2020 2020 2020 2020  xt,.            
-00019bd0: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-00019be0: 5f62 6172 3d70 726f 6772 6573 735f 6261  _bar=progress_ba
-00019bf0: 7229 0a20 2020 2020 2020 2020 2020 2072  r).            r
-00019c00: 6574 7572 6e20 7365 6c66 2e66 696e 6973  eturn self.finis
-00019c10: 685f 746f 7263 685f 7570 6c6f 6164 2866  h_torch_upload(f
-00019c20: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
-00019c30: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-00019c40: 2020 2020 2020 7365 6c66 2e5f 636c 6561        self._clea
-00019c50: 725f 7570 6c6f 6164 2829 0a0a 2320 2a2a  r_upload()..# **
-00019c60: 2a20 546f 7263 6842 6c6f 6248 616e 646c  * TorchBlobHandl
-00019c70: 6520 2a2a 2a0a 0a0a 636c 6173 7320 4a53  e ***...class JS
-00019c80: 4f4e 426c 6f62 4861 6e64 6c65 2842 6c6f  ONBlobHandle(Blo
-00019c90: 6248 616e 646c 6529 3a0a 2020 2020 6465  bHandle):.    de
-00019ca0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00019cb0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00019cc0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00019cd0: 3a20 5859 4d45 436c 6965 6e74 2c0a 2020  : XYMEClient,.  
-00019ce0: 2020 2020 2020 2020 2020 7572 693a 2073            uri: s
-00019cf0: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-00019d00: 6973 5f66 756c 6c3a 2062 6f6f 6c29 202d  is_full: bool) -
-00019d10: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00019d20: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00019d30: 2863 6c69 656e 742c 2075 7269 2c20 6973  (client, uri, is
-00019d40: 5f66 756c 6c29 0a20 2020 2020 2020 2073  _full).        s
-00019d50: 656c 662e 5f63 6f75 6e74 3a20 4f70 7469  elf._count: Opti
-00019d60: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00019d70: 0a0a 2020 2020 6465 6620 6765 745f 636f  ..    def get_co
-00019d80: 756e 7428 7365 6c66 2920 2d3e 204f 7074  unt(self) -> Opt
-00019d90: 696f 6e61 6c5b 696e 745d 3a0a 2020 2020  ional[int]:.    
-00019da0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00019db0: 5f63 6f75 6e74 0a0a 2020 2020 6465 6620  _count..    def 
-00019dc0: 6170 7065 6e64 5f6a 736f 6e73 280a 2020  append_jsons(.  
-00019dd0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-00019de0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
-00019df0: 733a 204c 6973 745b 416e 795d 2c0a 2020  s: List[Any],.  
-00019e00: 2020 2020 2020 2020 2020 7265 7175 6575            requeu
-00019e10: 655f 6f6e 5f66 696e 6973 683a 204f 7074  e_on_finish: Opt
-00019e20: 696f 6e61 6c5b 4e6f 6465 4861 6e64 6c65  ional[NodeHandle
-00019e30: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00019e40: 2020 2020 2020 2920 2d3e 204e 6f6e 653a        ) -> None:
-00019e50: 0a20 2020 2020 2020 206f 626a 203d 207b  .        obj = {
-00019e60: 0a20 2020 2020 2020 2020 2020 2022 626c  .            "bl
-00019e70: 6f62 223a 2073 656c 662e 6765 745f 7572  ob": self.get_ur
-00019e80: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
-00019e90: 2022 6a73 6f6e 7322 3a20 6a73 6f6e 732c   "jsons": jsons,
-00019ea0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00019eb0: 2020 2069 6620 7265 7175 6575 655f 6f6e     if requeue_on
-00019ec0: 5f66 696e 6973 6820 6973 206e 6f74 204e  _finish is not N
-00019ed0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00019ee0: 206f 626a 5b22 6461 6722 5d20 3d20 7265   obj["dag"] = re
-00019ef0: 7175 6575 655f 6f6e 5f66 696e 6973 682e  queue_on_finish.
-00019f00: 6765 745f 6461 6728 292e 6765 745f 7572  get_dag().get_ur
-00019f10: 6928 290a 2020 2020 2020 2020 2020 2020  i().            
-00019f20: 6f62 6a5b 226e 6f64 6522 5d20 3d20 7265  obj["node"] = re
-00019f30: 7175 6575 655f 6f6e 5f66 696e 6973 682e  queue_on_finish.
-00019f40: 6765 745f 6964 2829 0a20 2020 2020 2020  get_id().       
-00019f50: 2072 6573 203d 2063 6173 7428 4a53 4f4e   res = cast(JSON
-00019f60: 426c 6f62 4170 7065 6e64 5265 7370 6f6e  BlobAppendRespon
-00019f70: 7365 2c20 7365 6c66 2e5f 636c 6965 6e74  se, self._client
-00019f80: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
-00019f90: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
-00019fa0: 445f 5055 542c 2022 2f6a 736f 6e5f 6170  D_PUT, "/json_ap
-00019fb0: 7065 6e64 222c 206f 626a 2929 0a20 2020  pend", obj)).   
-00019fc0: 2020 2020 2073 656c 662e 5f63 6f75 6e74       self._count
-00019fd0: 203d 2072 6573 5b22 636f 756e 7422 5d0a   = res["count"].
-00019fe0: 0a23 202a 2a2a 204a 534f 4e42 6c6f 6248  .# *** JSONBlobH
-00019ff0: 616e 646c 6520 2a2a 2a0a 0a0a 636c 6173  andle ***...clas
-0001a000: 7320 4375 7374 6f6d 436f 6465 426c 6f62  s CustomCodeBlob
-0001a010: 4861 6e64 6c65 2842 6c6f 6248 616e 646c  Handle(BlobHandl
-0001a020: 6529 3a0a 2020 2020 6465 6620 7365 745f  e):.    def set_
-0001a030: 6375 7374 6f6d 5f69 6d70 6f72 7473 280a  custom_imports(.
-0001a040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001a050: 2c20 6d6f 6475 6c65 733a 204c 6973 745b  , modules: List[
-0001a060: 4c69 7374 5b73 7472 5d5d 2920 2d3e 204e  List[str]]) -> N
-0001a070: 6f64 6543 7573 746f 6d49 6d70 6f72 7473  odeCustomImports
-0001a080: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001a090: 2063 6173 7428 4e6f 6465 4375 7374 6f6d   cast(NodeCustom
-0001a0a0: 496d 706f 7274 732c 2073 656c 662e 5f63  Imports, self._c
-0001a0b0: 6c69 656e 742e 7265 7175 6573 745f 6a73  lient.request_js
-0001a0c0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-0001a0d0: 4d45 5448 4f44 5f50 5554 2c20 222f 6375  METHOD_PUT, "/cu
-0001a0e0: 7374 6f6d 5f69 6d70 6f72 7473 222c 207b  stom_imports", {
-0001a0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a100: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
-0001a110: 5f6f 776e 6572 5f64 6167 2829 2c0a 2020  _owner_dag(),.  
-0001a120: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-0001a130: 6f64 6522 3a20 7365 6c66 2e67 6574 5f6f  ode": self.get_o
-0001a140: 776e 6572 5f6e 6f64 6528 292c 0a20 2020  wner_node(),.   
-0001a150: 2020 2020 2020 2020 2020 2020 2022 6d6f               "mo
-0001a160: 6475 6c65 7322 3a20 6d6f 6475 6c65 732c  dules": modules,
-0001a170: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
-0001a180: 0a0a 2020 2020 6465 6620 6765 745f 6375  ..    def get_cu
-0001a190: 7374 6f6d 5f69 6d70 6f72 7473 2873 656c  stom_imports(sel
-0001a1a0: 6629 202d 3e20 4e6f 6465 4375 7374 6f6d  f) -> NodeCustom
-0001a1b0: 496d 706f 7274 733a 0a20 2020 2020 2020  Imports:.       
-0001a1c0: 2072 6574 7572 6e20 6361 7374 284e 6f64   return cast(Nod
-0001a1d0: 6543 7573 746f 6d49 6d70 6f72 7473 2c20  eCustomImports, 
-0001a1e0: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
-0001a1f0: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
-0001a200: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
-0001a210: 542c 2022 2f63 7573 746f 6d5f 696d 706f  T, "/custom_impo
-0001a220: 7274 7322 2c20 7b0a 2020 2020 2020 2020  rts", {.        
-0001a230: 2020 2020 2020 2020 2264 6167 223a 2073          "dag": s
-0001a240: 656c 662e 6765 745f 6f77 6e65 725f 6461  elf.get_owner_da
-0001a250: 6728 292c 0a20 2020 2020 2020 2020 2020  g(),.           
-0001a260: 2020 2020 2022 6e6f 6465 223a 2073 656c       "node": sel
-0001a270: 662e 6765 745f 6f77 6e65 725f 6e6f 6465  f.get_owner_node
-0001a280: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0001a290: 7d29 290a 0a20 2020 2064 6566 2073 6574  }))..    def set
-0001a2a0: 5f63 7573 746f 6d5f 636f 6465 2873 656c  _custom_code(sel
-0001a2b0: 662c 2066 756e 633a 2046 554e 4329 202d  f, func: FUNC) -
-0001a2c0: 3e20 4e6f 6465 4375 7374 6f6d 436f 6465  > NodeCustomCode
-0001a2d0: 3a0a 2020 2020 2020 2020 6672 6f6d 2052  :.        from R
-0001a2e0: 6573 7472 6963 7465 6450 7974 686f 6e20  estrictedPython 
-0001a2f0: 696d 706f 7274 2063 6f6d 7069 6c65 5f72  import compile_r
-0001a300: 6573 7472 6963 7465 640a 0a20 2020 2020  estricted..     
-0001a310: 2020 2064 6566 2066 6e5f 6173 5f73 7472     def fn_as_str
-0001a320: 2866 756e 3a20 4655 4e43 2920 2d3e 2073  (fun: FUNC) -> s
-0001a330: 7472 3a0a 2020 2020 2020 2020 2020 2020  tr:.            
-0001a340: 626f 6479 203d 2074 6578 7477 7261 702e  body = textwrap.
-0001a350: 6465 6465 6e74 2869 6e73 7065 6374 2e67  dedent(inspect.g
-0001a360: 6574 736f 7572 6365 2866 756e 2929 0a20  etsource(fun)). 
-0001a370: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-0001a380: 2062 6f64 7920 2b20 7465 7874 7772 6170   body + textwrap
-0001a390: 2e64 6564 656e 7428 6622 2222 0a20 2020  .dedent(f""".   
-0001a3a0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-0001a3b0: 3d20 7b66 756e 2e5f 5f6e 616d 655f 5f7d  = {fun.__name__}
-0001a3c0: 282a 6461 7461 2c20 2a2a 6b77 6172 6773  (*data, **kwargs
-0001a3d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001a3e0: 2072 6573 756c 7420 6973 204e 6f6e 653a   result is None:
-0001a3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a400: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001a410: 7228 227b 6675 6e2e 5f5f 6e61 6d65 5f5f  r("{fun.__name__
-0001a420: 7d20 6d75 7374 2072 6574 7572 6e20 6120  } must return a 
-0001a430: 7661 6c75 6522 290a 2020 2020 2020 2020  value").        
-0001a440: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
-0001a450: 2020 2020 2063 6f6d 7069 6c65 5f72 6573       compile_res
-0001a460: 7472 6963 7465 6428 7265 732c 2022 696e  tricted(res, "in
-0001a470: 6c69 6e65 222c 2022 6578 6563 2229 0a20  line", "exec"). 
-0001a480: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001a490: 6e20 7265 730a 0a20 2020 2020 2020 2072  n res..        r
-0001a4a0: 6177 5f63 6f64 6520 3d20 666e 5f61 735f  aw_code = fn_as_
-0001a4b0: 7374 7228 6675 6e63 290a 2020 2020 2020  str(func).      
-0001a4c0: 2020 7265 7475 726e 2063 6173 7428 4e6f    return cast(No
-0001a4d0: 6465 4375 7374 6f6d 436f 6465 2c20 7365  deCustomCode, se
-0001a4e0: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
-0001a4f0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
-0001a500: 2020 2020 204d 4554 484f 445f 5055 542c       METHOD_PUT,
-0001a510: 2022 2f63 7573 746f 6d5f 636f 6465 222c   "/custom_code",
-0001a520: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0001a530: 2020 2022 6461 6722 3a20 7365 6c66 2e67     "dag": self.g
-0001a540: 6574 5f6f 776e 6572 5f64 6167 2829 2c0a  et_owner_dag(),.
-0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a560: 226e 6f64 6522 3a20 7365 6c66 2e67 6574  "node": self.get
-0001a570: 5f6f 776e 6572 5f6e 6f64 6528 292c 0a20  _owner_node(),. 
-0001a580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001a590: 636f 6465 223a 2072 6177 5f63 6f64 652c  code": raw_code,
-0001a5a0: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
-0001a5b0: 0a0a 2020 2020 6465 6620 6765 745f 6375  ..    def get_cu
-0001a5c0: 7374 6f6d 5f63 6f64 6528 7365 6c66 2920  stom_code(self) 
-0001a5d0: 2d3e 204e 6f64 6543 7573 746f 6d43 6f64  -> NodeCustomCod
-0001a5e0: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-0001a5f0: 6e20 6361 7374 284e 6f64 6543 7573 746f  n cast(NodeCusto
-0001a600: 6d43 6f64 652c 2073 656c 662e 5f63 6c69  mCode, self._cli
-0001a610: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
-0001a620: 280a 2020 2020 2020 2020 2020 2020 4d45  (.            ME
-0001a630: 5448 4f44 5f47 4554 2c20 222f 6375 7374  THOD_GET, "/cust
-0001a640: 6f6d 5f63 6f64 6522 2c20 7b0a 2020 2020  om_code", {.    
-0001a650: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
-0001a660: 223a 2073 656c 662e 6765 745f 6f77 6e65  ": self.get_owne
-0001a670: 725f 6461 6728 292c 0a20 2020 2020 2020  r_dag(),.       
-0001a680: 2020 2020 2020 2020 2022 6e6f 6465 223a           "node":
-0001a690: 2073 656c 662e 6765 745f 6f77 6e65 725f   self.get_owner_
-0001a6a0: 6e6f 6465 2829 2c0a 2020 2020 2020 2020  node(),.        
-0001a6b0: 2020 2020 7d29 290a 0a23 202a 2a2a 2043      }))..# *** C
-0001a6c0: 7573 746f 6d43 6f64 6542 6c6f 6248 616e  ustomCodeBlobHan
-0001a6d0: 646c 6520 2a2a 2a0a 0a0a 636c 6173 7320  dle ***...class 
-0001a6e0: 436f 6d70 7574 6174 696f 6e48 616e 646c  ComputationHandl
-0001a6f0: 653a 0a20 2020 2064 6566 205f 5f69 6e69  e:.    def __ini
-0001a700: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
-0001a710: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-0001a720: 2020 2064 6167 3a20 4461 6748 616e 646c     dag: DagHandl
-0001a730: 652c 0a20 2020 2020 2020 2020 2020 2076  e,.            v
-0001a740: 616c 7565 5f69 643a 2073 7472 2c0a 2020  alue_id: str,.  
-0001a750: 2020 2020 2020 2020 2020 6765 745f 6479            get_dy
-0001a760: 6e5f 6572 726f 723a 2043 616c 6c61 626c  n_error: Callabl
-0001a770: 655b 5b5d 2c20 4f70 7469 6f6e 616c 5b73  e[[], Optional[s
-0001a780: 7472 5d5d 2c0a 2020 2020 2020 2020 2020  tr]],.          
-0001a790: 2020 7365 745f 6479 6e5f 6572 726f 723a    set_dyn_error:
-0001a7a0: 2043 616c 6c61 626c 655b 5b73 7472 5d2c   Callable[[str],
-0001a7b0: 204e 6f6e 655d 2920 2d3e 204e 6f6e 653a   None]) -> None:
-0001a7c0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-0001a7d0: 6167 203d 2064 6167 0a20 2020 2020 2020  ag = dag.       
-0001a7e0: 2073 656c 662e 5f76 616c 7565 5f69 6420   self._value_id 
-0001a7f0: 3d20 7661 6c75 655f 6964 0a20 2020 2020  = value_id.     
-0001a800: 2020 2073 656c 662e 5f76 616c 7565 3a20     self._value: 
-0001a810: 4f70 7469 6f6e 616c 5b42 7974 6552 6573  Optional[ByteRes
-0001a820: 706f 6e73 655d 203d 204e 6f6e 650a 2020  ponse] = None.  
-0001a830: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
-0001a840: 6479 6e5f 6572 726f 7220 3d20 6765 745f  dyn_error = get_
-0001a850: 6479 6e5f 6572 726f 720a 2020 2020 2020  dyn_error.      
-0001a860: 2020 7365 6c66 2e5f 7365 745f 6479 6e5f    self._set_dyn_
-0001a870: 6572 726f 7220 3d20 7365 745f 6479 6e5f  error = set_dyn_
-0001a880: 6572 726f 720a 0a20 2020 2064 6566 2068  error..    def h
-0001a890: 6173 5f66 6574 6368 6564 2873 656c 6629  as_fetched(self)
-0001a8a0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0001a8b0: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
-0001a8c0: 616c 7565 2069 7320 6e6f 7420 4e6f 6e65  alue is not None
-0001a8d0: 0a0a 2020 2020 6465 6620 6765 7428 7365  ..    def get(se
-0001a8e0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-0001a8f0: 4279 7465 5265 7370 6f6e 7365 5d3a 0a20  ByteResponse]:. 
-0001a900: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0001a910: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001a920: 5f76 616c 7565 2069 7320 4e6f 6e65 3a0a  _value is None:.
-0001a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a940: 7365 6c66 2e5f 7661 6c75 6520 3d20 7365  self._value = se
-0001a950: 6c66 2e5f 6461 672e 6765 745f 6479 6e61  lf._dag.get_dyna
-0001a960: 6d69 635f 7265 7375 6c74 2873 656c 662e  mic_result(self.
-0001a970: 5f76 616c 7565 5f69 6429 0a20 2020 2020  _value_id).     
-0001a980: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001a990: 6c66 2e5f 7661 6c75 650a 2020 2020 2020  lf._value.      
-0001a9a0: 2020 6578 6365 7074 2053 6572 7665 7253    except ServerS
-0001a9b0: 6964 6545 7272 6f72 2061 7320 653a 0a20  ideError as e:. 
-0001a9c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0001a9d0: 6c66 2e5f 6765 745f 6479 6e5f 6572 726f  lf._get_dyn_erro
-0001a9e0: 7228 2920 6973 204e 6f6e 653a 0a20 2020  r() is None:.   
-0001a9f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001aa00: 662e 5f73 6574 5f64 796e 5f65 7272 6f72  f._set_dyn_error
-0001aa10: 2873 7472 2865 2929 0a20 2020 2020 2020  (str(e)).       
-0001aa20: 2020 2020 2072 6169 7365 2065 0a20 2020       raise e.   
-0001aa30: 2020 2020 2065 7863 6570 7420 4b65 7945       except KeyE
-0001aa40: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-0001aa50: 2020 2020 2020 206d 6179 6265 5f65 7272         maybe_err
-0001aa60: 6f72 203d 2073 656c 662e 5f67 6574 5f64  or = self._get_d
-0001aa70: 796e 5f65 7272 6f72 2829 0a20 2020 2020  yn_error().     
-0001aa80: 2020 2020 2020 2069 6620 6d61 7962 655f         if maybe_
-0001aa90: 6572 726f 7220 6973 206e 6f74 204e 6f6e  error is not Non
-0001aaa0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001aab0: 2020 2072 6169 7365 2053 6572 7665 7253     raise ServerS
-0001aac0: 6964 6545 7272 6f72 286d 6179 6265 5f65  ideError(maybe_e
-0001aad0: 7272 6f72 2920 6672 6f6d 2065 0a20 2020  rror) from e.   
-0001aae0: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
-0001aaf0: 0a0a 2020 2020 6465 6620 6765 745f 6964  ..    def get_id
-0001ab00: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-0001ab10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001ab20: 6c66 2e5f 7661 6c75 655f 6964 0a0a 2020  lf._value_id..  
-0001ab30: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
-0001ab40: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
-0001ab50: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
-0001ab60: 2e5f 7661 6c75 650a 2020 2020 2020 2020  ._value.        
-0001ab70: 6966 2076 616c 7565 2069 7320 4e6f 6e65  if value is None
-0001ab80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001ab90: 7475 726e 2066 2276 616c 7565 5f69 643d  turn f"value_id=
-0001aba0: 7b73 656c 662e 5f76 616c 7565 5f69 647d  {self._value_id}
-0001abb0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0001abc0: 2066 2276 616c 7565 287b 7479 7065 2876   f"value({type(v
-0001abd0: 616c 7565 297d 293d 7b76 616c 7565 7d22  alue)})={value}"
-0001abe0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-0001abf0: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
-0001ac00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001ac10: 6622 7b73 656c 662e 5f5f 636c 6173 735f  f"{self.__class_
-0001ac20: 5f2e 5f5f 6e61 6d65 5f5f 7d5b 7b73 656c  _.__name__}[{sel
-0001ac30: 662e 5f5f 7374 725f 5f28 297d 5d22 0a0a  f.__str__()}]"..
-0001ac40: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
-0001ac50: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-0001ac60: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
-0001ac70: 7368 2873 656c 662e 6765 745f 6964 2829  sh(self.get_id()
-0001ac80: 290a 0a20 2020 2064 6566 205f 5f65 715f  )..    def __eq_
-0001ac90: 5f28 7365 6c66 2c20 6f74 6865 723a 206f  _(self, other: o
-0001aca0: 626a 6563 7429 202d 3e20 626f 6f6c 3a0a  bject) -> bool:.
-0001acb0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0001acc0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-0001acd0: 2073 656c 662e 5f5f 636c 6173 735f 5f29   self.__class__)
-0001ace0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001acf0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-0001ad00: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-0001ad10: 6574 5f69 6428 2920 3d3d 206f 7468 6572  et_id() == other
-0001ad20: 2e67 6574 5f69 6428 290a 0a20 2020 2064  .get_id()..    d
-0001ad30: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
-0001ad40: 6f74 6865 723a 206f 626a 6563 7429 202d  other: object) -
-0001ad50: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0001ad60: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
-0001ad70: 5f5f 6571 5f5f 286f 7468 6572 290a 0a23  __eq__(other)..#
-0001ad80: 202a 2a2a 2043 6f6d 7075 7461 7469 6f6e   *** Computation
-0001ad90: 4861 6e64 6c65 202a 2a2a 0a0a 0a64 6566  Handle ***...def
-0001ada0: 2064 6566 6175 6c74 5f78 796d 655f 636c   default_xyme_cl
-0001adb0: 6965 6e74 2829 202d 3e20 5859 4d45 436c  ient() -> XYMECl
-0001adc0: 6965 6e74 3a0a 2020 2020 7265 7475 726e  ient:.    return
-0001add0: 2063 7265 6174 655f 7879 6d65 5f63 6c69   create_xyme_cli
-0001ade0: 656e 7428 0a20 2020 2020 2020 2075 726c  ent(.        url
-0001adf0: 3d44 4546 4155 4c54 5f55 524c 2c0a 2020  =DEFAULT_URL,.  
-0001ae00: 2020 2020 2020 746f 6b65 6e3d 6f73 2e67        token=os.g
-0001ae10: 6574 656e 7628 2258 594d 455f 5345 5256  etenv("XYME_SERV
-0001ae20: 4552 5f54 4f4b 454e 2229 2c0a 2020 2020  ER_TOKEN"),.    
-0001ae30: 2020 2020 6e61 6d65 7370 6163 653d 4445      namespace=DE
-0001ae40: 4641 554c 545f 4e41 4d45 5350 4143 4529  FAULT_NAMESPACE)
-0001ae50: 0a0a 0a64 6566 2063 7265 6174 655f 7879  ...def create_xy
-0001ae60: 6d65 5f63 6c69 656e 7428 0a20 2020 2020  me_client(.     
-0001ae70: 2020 2075 726c 3a20 7374 722c 0a20 2020     url: str,.   
-0001ae80: 2020 2020 2074 6f6b 656e 3a20 4f70 7469       token: Opti
-0001ae90: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0001aea0: 2c0a 2020 2020 2020 2020 6e61 6d65 7370  ,.        namesp
-0001aeb0: 6163 653a 2073 7472 203d 2044 4546 4155  ace: str = DEFAU
-0001aec0: 4c54 5f4e 414d 4553 5041 4345 2920 2d3e  LT_NAMESPACE) ->
-0001aed0: 2058 594d 4543 6c69 656e 743a 0a20 2020   XYMEClient:.   
-0001aee0: 2074 7279 3a0a 2020 2020 2020 2020 7265   try:.        re
-0001aef0: 7475 726e 2058 594d 4543 6c69 656e 7428  turn XYMEClient(
-0001af00: 7572 6c2c 2074 6f6b 656e 2c20 6e61 6d65  url, token, name
-0001af10: 7370 6163 6529 0a20 2020 2065 7863 6570  space).    excep
-0001af20: 7420 4c65 6761 6379 5665 7273 696f 6e20  t LegacyVersion 
-0001af30: 6173 206c 7665 3a0a 2020 2020 2020 2020  as lve:.        
-0001af40: 6170 695f 7665 7273 696f 6e20 3d20 6c76  api_version = lv
-0001af50: 652e 6765 745f 6170 695f 7665 7273 696f  e.get_api_versio
-0001af60: 6e28 290a 2020 2020 2020 2020 6966 2061  n().        if a
-0001af70: 7069 5f76 6572 7369 6f6e 203d 3d20 333a  pi_version == 3:
-0001af80: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0001af90: 6d20 6163 6365 726e 5f78 796d 652e 7633  m accern_xyme.v3
-0001afa0: 2e61 6363 6572 6e5f 7879 6d65 2069 6d70  .accern_xyme imp
-0001afb0: 6f72 7420 6372 6561 7465 5f78 796d 655f  ort create_xyme_
-0001afc0: 636c 6965 6e74 5f76 330a 0a20 2020 2020  client_v3..     
-0001afd0: 2020 2020 2020 2072 6574 7572 6e20 6372         return cr
-0001afe0: 6561 7465 5f78 796d 655f 636c 6965 6e74  eate_xyme_client
-0001aff0: 5f76 3328 7572 6c2c 2074 6f6b 656e 2920  _v3(url, token) 
-0001b000: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
-0001b010: 2020 2020 2020 2020 7261 6973 6520 6c76          raise lv
-0001b020: 650a                                     e.
+0000d5a0: 2022 6964 223a 2076 616c 7565 5f69 642c   "id": value_id,
+0000d5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d5c0: 207d 290a 2020 2020 2020 2020 6578 6365   }).        exce
+0000d5d0: 7074 2048 5454 5045 7272 6f72 2061 7320  pt HTTPError as 
+0000d5e0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+0000d5f0: 6620 652e 7265 7370 6f6e 7365 2e73 7461  f e.response.sta
+0000d600: 7475 735f 636f 6465 203d 3d20 3430 343a  tus_code == 404:
+0000d610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d620: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
+0000d630: 6622 7661 6c75 655f 6964 207b 7661 6c75  f"value_id {valu
+0000d640: 655f 6964 7d20 646f 6573 206e 6f74 2065  e_id} does not e
+0000d650: 7869 7374 2229 2066 726f 6d20 650a 2020  xist") from e.  
+0000d660: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d670: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000d680: 2069 6e74 6572 7072 6574 5f63 7479 7065   interpret_ctype
+0000d690: 2863 7572 5f72 6573 2c20 6374 7970 6529  (cur_res, ctype)
+0000d6a0: 0a0a 2020 2020 6465 6620 6765 745f 6479  ..    def get_dy
+0000d6b0: 6e61 6d69 635f 7374 6174 7573 280a 2020  namic_status(.  
+0000d6c0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+0000d6d0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+0000d6e0: 655f 6964 733a 204c 6973 745b 2743 6f6d  e_ids: List['Com
+0000d6f0: 7075 7461 7469 6f6e 4861 6e64 6c65 275d  putationHandle']
+0000d700: 2920 2d3e 2044 6963 745b 0a20 2020 2020  ) -> Dict[.     
+0000d710: 2020 2020 2020 2020 2020 2027 436f 6d70             'Comp
+0000d720: 7574 6174 696f 6e48 616e 646c 6527 2c20  utationHandle', 
+0000d730: 5175 6575 6553 7461 7475 735d 3a0a 2020  QueueStatus]:.  
+0000d740: 2020 2020 2020 7265 7320 3d20 6361 7374        res = cast
+0000d750: 2844 796e 616d 6963 5374 6174 7573 5265  (DynamicStatusRe
+0000d760: 7370 6f6e 7365 2c20 7365 6c66 2e5f 636c  sponse, self._cl
+0000d770: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
+0000d780: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
+0000d790: 4554 484f 445f 504f 5354 2c20 222f 6479  ETHOD_POST, "/dy
+0000d7a0: 6e61 6d69 635f 7374 6174 7573 222c 207b  namic_status", {
+0000d7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d7c0: 2022 7661 6c75 655f 6964 7322 3a20 5b76   "value_ids": [v
+0000d7d0: 616c 7565 5f69 642e 6765 745f 6964 2829  alue_id.get_id()
+0000d7e0: 2066 6f72 2076 616c 7565 5f69 6420 696e   for value_id in
+0000d7f0: 2076 616c 7565 5f69 6473 5d2c 0a20 2020   value_ids],.   
+0000d800: 2020 2020 2020 2020 2020 2020 2022 6461               "da
+0000d810: 6722 3a20 7365 6c66 2e67 6574 5f75 7269  g": self.get_uri
+0000d820: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0000d830: 7d29 290a 2020 2020 2020 2020 7374 6174  })).        stat
+0000d840: 7573 203d 2072 6573 5b22 7374 6174 7573  us = res["status
+0000d850: 225d 0a20 2020 2020 2020 2068 6e64 5f6d  "].        hnd_m
+0000d860: 6170 203d 207b 7661 6c75 655f 6964 2e67  ap = {value_id.g
+0000d870: 6574 5f69 6428 293a 2076 616c 7565 5f69  et_id(): value_i
+0000d880: 6420 666f 7220 7661 6c75 655f 6964 2069  d for value_id i
+0000d890: 6e20 7661 6c75 655f 6964 737d 0a20 2020  n value_ids}.   
+0000d8a0: 2020 2020 2072 6574 7572 6e20 7b0a 2020       return {.  
+0000d8b0: 2020 2020 2020 2020 2020 686e 645f 6d61            hnd_ma
+0000d8c0: 705b 6b65 795d 3a20 6361 7374 2851 7565  p[key]: cast(Que
+0000d8d0: 7565 5374 6174 7573 2c20 7661 6c75 6529  ueStatus, value)
+0000d8e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000d8f0: 206b 6579 2c20 7661 6c75 6520 696e 2073   key, value in s
+0000d900: 7461 7475 732e 6974 656d 7328 290a 2020  tatus.items().  
+0000d910: 2020 2020 2020 7d0a 0a20 2020 2064 6566        }..    def
+0000d920: 2067 6574 5f64 796e 616d 6963 5f62 756c   get_dynamic_bul
+0000d930: 6b28 0a20 2020 2020 2020 2020 2020 2073  k(.            s
+0000d940: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000d950: 2069 6e70 7574 5f64 6174 613a 204c 6973   input_data: Lis
+0000d960: 745b 4279 7465 7349 4f5d 2c0a 2020 2020  t[BytesIO],.    
+0000d970: 2020 2020 2020 2020 6d61 785f 6275 6666          max_buff
+0000d980: 3a20 696e 7420 3d20 3430 3030 2c0a 2020  : int = 4000,.  
+0000d990: 2020 2020 2020 2020 2020 626c 6f63 6b5f            block_
+0000d9a0: 7369 7a65 3a20 696e 7420 3d20 352c 0a20  size: int = 5,. 
+0000d9b0: 2020 2020 2020 2020 2020 206e 756d 5f74             num_t
+0000d9c0: 6872 6561 6473 3a20 696e 7420 3d20 3230  hreads: int = 20
+0000d9d0: 2920 2d3e 2049 7465 7261 626c 655b 4f70  ) -> Iterable[Op
+0000d9e0: 7469 6f6e 616c 5b42 7974 6552 6573 706f  tional[ByteRespo
+0000d9f0: 6e73 655d 5d3a 0a0a 2020 2020 2020 2020  nse]]:..        
+0000da00: 6465 6620 6765 7428 686e 643a 2027 436f  def get(hnd: 'Co
+0000da10: 6d70 7574 6174 696f 6e48 616e 646c 6527  mputationHandle'
+0000da20: 2920 2d3e 204f 7074 696f 6e61 6c5b 4279  ) -> Optional[By
+0000da30: 7465 5265 7370 6f6e 7365 5d3a 0a20 2020  teResponse]:.   
+0000da40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000da50: 686e 642e 6765 7428 290a 0a20 2020 2020  hnd.get()..     
+0000da60: 2020 2073 7563 6365 7373 203d 2046 616c     success = Fal
+0000da70: 7365 0a20 2020 2020 2020 2074 7279 3a0a  se.        try:.
+0000da80: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+0000da90: 6420 6672 6f6d 2061 7379 6e63 5f63 6f6d  d from async_com
+0000daa0: 7075 7465 280a 2020 2020 2020 2020 2020  pute(.          
+0000dab0: 2020 2020 2020 696e 7075 745f 6461 7461        input_data
+0000dac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dad0: 2020 7365 6c66 2e64 796e 616d 6963 5f61    self.dynamic_a
+0000dae0: 7379 6e63 2c0a 2020 2020 2020 2020 2020  sync,.          
+0000daf0: 2020 2020 2020 6765 742c 0a20 2020 2020        get,.     
+0000db00: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
+0000db10: 613a 2073 656c 662e 6368 6563 6b5f 7175  a: self.check_qu
+0000db20: 6575 655f 7374 6174 7328 6d69 6e69 6d61  eue_stats(minima
+0000db30: 6c3d 5472 7565 292c 0a20 2020 2020 2020  l=True),.       
+0000db40: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+0000db50: 745f 6479 6e61 6d69 635f 7374 6174 7573  t_dynamic_status
+0000db60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000db70: 2020 6d61 785f 6275 6666 2c0a 2020 2020    max_buff,.    
+0000db80: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
+0000db90: 6b5f 7369 7a65 2c0a 2020 2020 2020 2020  k_size,.        
+0000dba0: 2020 2020 2020 2020 6e75 6d5f 7468 7265          num_thre
+0000dbb0: 6164 7329 0a20 2020 2020 2020 2020 2020  ads).           
+0000dbc0: 2073 7563 6365 7373 203d 2054 7275 650a   success = True.
+0000dbd0: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
+0000dbe0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000dbf0: 7375 6363 6573 733a 0a20 2020 2020 2020  success:.       
+0000dc00: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000dc10: 745f 6479 6e61 6d69 635f 6572 726f 725f  t_dynamic_error_
+0000dc20: 6d65 7373 6167 6528 4e6f 6e65 290a 0a20  message(None).. 
+0000dc30: 2020 2064 6566 2067 6574 5f64 796e 616d     def get_dynam
+0000dc40: 6963 5f62 756c 6b5f 6f62 6a28 0a20 2020  ic_bulk_obj(.   
+0000dc50: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+0000dc60: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000dc70: 5f64 6174 613a 204c 6973 745b 416e 795d  _data: List[Any]
+0000dc80: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+0000dc90: 785f 6275 6666 3a20 696e 7420 3d20 3430  x_buff: int = 40
+0000dca0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+0000dcb0: 626c 6f63 6b5f 7369 7a65 3a20 696e 7420  block_size: int 
+0000dcc0: 3d20 352c 0a20 2020 2020 2020 2020 2020  = 5,.           
+0000dcd0: 206e 756d 5f74 6872 6561 6473 3a20 696e   num_threads: in
+0000dce0: 7420 3d20 3230 2920 2d3e 2049 7465 7261  t = 20) -> Itera
+0000dcf0: 626c 655b 4f70 7469 6f6e 616c 5b42 7974  ble[Optional[Byt
+0000dd00: 6552 6573 706f 6e73 655d 5d3a 0a0a 2020  eResponse]]:..  
+0000dd10: 2020 2020 2020 6465 6620 6765 7428 686e        def get(hn
+0000dd20: 643a 2027 436f 6d70 7574 6174 696f 6e48  d: 'ComputationH
+0000dd30: 616e 646c 6527 2920 2d3e 204f 7074 696f  andle') -> Optio
+0000dd40: 6e61 6c5b 4279 7465 5265 7370 6f6e 7365  nal[ByteResponse
+0000dd50: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
+0000dd60: 6574 7572 6e20 686e 642e 6765 7428 290a  eturn hnd.get().
+0000dd70: 0a20 2020 2020 2020 2073 7563 6365 7373  .        success
+0000dd80: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+0000dd90: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000dda0: 2020 7969 656c 6420 6672 6f6d 2061 7379    yield from asy
+0000ddb0: 6e63 5f63 6f6d 7075 7465 280a 2020 2020  nc_compute(.    
+0000ddc0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+0000ddd0: 745f 6461 7461 2c0a 2020 2020 2020 2020  t_data,.        
+0000dde0: 2020 2020 2020 2020 7365 6c66 2e64 796e          self.dyn
+0000ddf0: 616d 6963 5f61 7379 6e63 5f6f 626a 2c0a  amic_async_obj,.
+0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de10: 6765 742c 0a20 2020 2020 2020 2020 2020  get,.           
+0000de20: 2020 2020 206c 616d 6264 613a 2073 656c       lambda: sel
+0000de30: 662e 6368 6563 6b5f 7175 6575 655f 7374  f.check_queue_st
+0000de40: 6174 7328 6d69 6e69 6d61 6c3d 5472 7565  ats(minimal=True
+0000de50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000de60: 2020 2073 656c 662e 6765 745f 6479 6e61     self.get_dyna
+0000de70: 6d69 635f 7374 6174 7573 2c0a 2020 2020  mic_status,.    
+0000de80: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000de90: 6275 6666 2c0a 2020 2020 2020 2020 2020  buff,.          
+0000dea0: 2020 2020 2020 626c 6f63 6b5f 7369 7a65        block_size
+0000deb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dec0: 2020 6e75 6d5f 7468 7265 6164 7329 0a20    num_threads). 
+0000ded0: 2020 2020 2020 2020 2020 2073 7563 6365             succe
+0000dee0: 7373 203d 2054 7275 650a 2020 2020 2020  ss = True.      
+0000def0: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+0000df00: 2020 2020 2020 2069 6620 7375 6363 6573         if succes
+0000df10: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000df20: 2020 2073 656c 662e 7365 745f 6479 6e61     self.set_dyna
+0000df30: 6d69 635f 6572 726f 725f 6d65 7373 6167  mic_error_messag
+0000df40: 6528 4e6f 6e65 290a 0a20 2020 2064 6566  e(None)..    def
+0000df50: 205f 7072 6574 7479 280a 2020 2020 2020   _pretty(.      
+0000df60: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000df70: 2020 2020 2020 2020 6e6f 6465 735f 6f6e          nodes_on
+0000df80: 6c79 3a20 626f 6f6c 2c0a 2020 2020 2020  ly: bool,.      
+0000df90: 2020 2020 2020 616c 6c6f 775f 756e 6963        allow_unic
+0000dfa0: 6f64 653a 2062 6f6f 6c2c 0a20 2020 2020  ode: bool,.     
+0000dfb0: 2020 2020 2020 206d 6574 686f 643a 204f         method: O
+0000dfc0: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
+0000dfd0: 6163 6365 726e 222c 0a20 2020 2020 2020  accern",.       
+0000dfe0: 2020 2020 2066 6965 6c64 733a 204f 7074       fields: Opt
+0000dff0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+0000e000: 203d 204e 6f6e 6529 202d 3e20 5072 6574   = None) -> Pret
+0000e010: 7479 5265 7370 6f6e 7365 3a0a 2020 2020  tyResponse:.    
+0000e020: 2020 2020 6172 6773 203d 207b 0a20 2020      args = {.   
+0000e030: 2020 2020 2020 2020 2022 6461 6722 3a20           "dag": 
+0000e040: 7365 6c66 2e67 6574 5f75 7269 2829 2c0a  self.get_uri(),.
+0000e050: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
+0000e060: 6573 5f6f 6e6c 7922 3a20 6e6f 6465 735f  es_only": nodes_
+0000e070: 6f6e 6c79 2c0a 2020 2020 2020 2020 2020  only,.          
+0000e080: 2020 2261 6c6c 6f77 5f75 6e69 636f 6465    "allow_unicode
+0000e090: 223a 2061 6c6c 6f77 5f75 6e69 636f 6465  ": allow_unicode
+0000e0a0: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+0000e0b0: 6574 686f 6422 3a20 6d65 7468 6f64 2c0a  ethod": method,.
+0000e0c0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0000e0d0: 2020 6966 2066 6965 6c64 7320 6973 206e    if fields is n
+0000e0e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000e0f0: 2020 2020 2061 7267 735b 2266 6965 6c64       args["field
+0000e100: 7322 5d20 3d20 222c 222e 6a6f 696e 2866  s"] = ",".join(f
+0000e110: 6965 6c64 7329 0a20 2020 2020 2020 2072  ields).        r
+0000e120: 6574 7572 6e20 6361 7374 2850 7265 7474  eturn cast(Prett
+0000e130: 7952 6573 706f 6e73 652c 2073 656c 662e  yResponse, self.
+0000e140: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
+0000e150: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
+0000e160: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
+0000e170: 7072 6574 7479 222c 2061 7267 7329 290a  pretty", args)).
+0000e180: 0a20 2020 2064 6566 2070 7265 7474 7928  .    def pretty(
+0000e190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e1a0: 662c 0a20 2020 2020 2020 2020 2020 206e  f,.            n
+0000e1b0: 6f64 6573 5f6f 6e6c 793a 2062 6f6f 6c20  odes_only: bool 
+0000e1c0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+0000e1d0: 2020 2020 2061 6c6c 6f77 5f75 6e69 636f       allow_unico
+0000e1e0: 6465 3a20 626f 6f6c 203d 2054 7275 652c  de: bool = True,
+0000e1f0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0000e200: 686f 643a 204f 7074 696f 6e61 6c5b 7374  hod: Optional[st
+0000e210: 725d 203d 2022 646f 7422 2c0a 2020 2020  r] = "dot",.    
+0000e220: 2020 2020 2020 2020 6669 656c 6473 3a20          fields: 
+0000e230: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+0000e240: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+0000e250: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
+0000e260: 6f72 6d61 743a 204f 7074 696f 6e61 6c5b  ormat: Optional[
+0000e270: 7374 725d 203d 2022 706e 6722 2c0a 2020  str] = "png",.  
+0000e280: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+0000e290: 793a 204f 7074 696f 6e61 6c5b 494f 5b41  y: Optional[IO[A
+0000e2a0: 6e79 5d5d 203d 2073 7973 2e73 7464 6f75  ny]] = sys.stdou
+0000e2b0: 7429 202d 3e20 4f70 7469 6f6e 616c 5b73  t) -> Optional[s
+0000e2c0: 7472 5d3a 0a0a 2020 2020 2020 2020 6465  tr]:..        de
+0000e2d0: 6620 7265 6e64 6572 2876 616c 7565 3a20  f render(value: 
+0000e2e0: 7374 7229 202d 3e20 4f70 7469 6f6e 616c  str) -> Optional
+0000e2f0: 5b73 7472 5d3a 0a20 2020 2020 2020 2020  [str]:.         
+0000e300: 2020 2069 6620 6469 7370 6c61 7920 6973     if display is
+0000e310: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e320: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+0000e330: 6179 2e77 7269 7465 2876 616c 7565 290a  ay.write(value).
+0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e350: 6469 7370 6c61 792e 666c 7573 6828 290a  display.flush().
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+0000e380: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+0000e390: 616c 7565 0a0a 2020 2020 2020 2020 6772  alue..        gr
+0000e3a0: 6170 685f 7374 7220 3d20 7365 6c66 2e5f  aph_str = self._
+0000e3b0: 7072 6574 7479 280a 2020 2020 2020 2020  pretty(.        
+0000e3c0: 2020 2020 6e6f 6465 735f 6f6e 6c79 3d6e      nodes_only=n
+0000e3d0: 6f64 6573 5f6f 6e6c 792c 0a20 2020 2020  odes_only,.     
+0000e3e0: 2020 2020 2020 2061 6c6c 6f77 5f75 6e69         allow_uni
+0000e3f0: 636f 6465 3d61 6c6c 6f77 5f75 6e69 636f  code=allow_unico
+0000e400: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+0000e410: 6d65 7468 6f64 3d6d 6574 686f 642c 0a20  method=method,. 
+0000e420: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+0000e430: 733d 6669 656c 6473 295b 2270 7265 7474  s=fields)["prett
+0000e440: 7922 5d0a 2020 2020 2020 2020 6966 206d  y"].        if m
+0000e450: 6574 686f 6420 3d3d 2022 6163 6365 726e  ethod == "accern
+0000e460: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
+0000e470: 6574 7572 6e20 7265 6e64 6572 2867 7261  eturn render(gra
+0000e480: 7068 5f73 7472 290a 2020 2020 2020 2020  ph_str).        
+0000e490: 6966 206d 6574 686f 6420 3d3d 2022 646f  if method == "do
+0000e4a0: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
+0000e4b0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000e4c0: 2020 2020 2066 726f 6d20 6772 6170 6876       from graphv
+0000e4d0: 697a 2069 6d70 6f72 7420 536f 7572 6365  iz import Source
+0000e4e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e4f0: 2020 6772 6170 6820 3d20 536f 7572 6365    graph = Source
+0000e500: 2867 7261 7068 5f73 7472 290a 2020 2020  (graph_str).    
+0000e510: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+0000e520: 7574 7075 745f 666f 726d 6174 203d 3d20  utput_format == 
+0000e530: 2264 6f74 223a 0a20 2020 2020 2020 2020  "dot":.         
+0000e540: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e550: 6e20 7265 6e64 6572 2867 7261 7068 5f73  n render(graph_s
+0000e560: 7472 290a 2020 2020 2020 2020 2020 2020  tr).            
+0000e570: 2020 2020 6966 206f 7574 7075 745f 666f      if output_fo
+0000e580: 726d 6174 203d 3d20 2273 7667 223a 0a20  rmat == "svg":. 
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 2020 2073 7667 5f73 7472 203d 2067 7261     svg_str = gra
+0000e5b0: 7068 2e70 6970 6528 666f 726d 6174 3d22  ph.pipe(format="
+0000e5c0: 7376 6722 290a 2020 2020 2020 2020 2020  svg").          
+0000e5d0: 2020 2020 2020 2020 2020 6966 2064 6973            if dis
+0000e5e0: 706c 6179 2069 7320 6e6f 7420 4e6f 6e65  play is not None
+0000e5f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e600: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000e610: 2069 735f 6a75 7079 7465 7228 293a 0a20   is_jupyter():. 
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e630: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+0000e640: 6179 2e77 7269 7465 280a 2020 2020 2020  ay.write(.      
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 2020 2020 2257 6172 6e69            "Warni
+0000e670: 6e67 3a20 4970 7974 686f 6e20 696e 7374  ng: Ipython inst
+0000e680: 616e 6365 206e 6f74 2066 6f75 6e64 2e5c  ance not found.\
+0000e690: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6b0: 6469 7370 6c61 792e 7772 6974 6528 7376  display.write(sv
+0000e6c0: 675f 7374 7229 0a20 2020 2020 2020 2020  g_str).         
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 2020 2064 6973 706c 6179 2e66 6c75 7368     display.flush
+0000e6f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000e700: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000e710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e720: 2020 2020 2020 2020 2020 2020 2066 726f               fro
+0000e730: 6d20 4950 7974 686f 6e2e 6469 7370 6c61  m IPython.displa
+0000e740: 7920 696d 706f 7274 2064 6973 706c 6179  y import display
+0000e750: 2061 7320 6964 6973 706c 6179 0a20 2020   as idisplay.   
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 2020 2066 726f 6d20 4950           from IP
+0000e780: 7974 686f 6e2e 6469 7370 6c61 7920 696d  ython.display im
+0000e790: 706f 7274 2053 5647 0a20 2020 2020 2020  port SVG.       
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7b0: 2020 2020 2069 6469 7370 6c61 7928 5356       idisplay(SV
+0000e7c0: 4728 7376 675f 7374 7229 290a 2020 2020  G(svg_str)).    
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7e0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 2020 2020 7265 7475 726e 2073 7667 5f73      return svg_s
+0000e810: 7472 0a20 2020 2020 2020 2020 2020 2020  tr.             
+0000e820: 2020 2069 6620 6f75 7470 7574 5f66 6f72     if output_for
+0000e830: 6d61 7420 3d3d 2022 706e 6722 3a0a 2020  mat == "png":.  
+0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e850: 2020 6772 6170 6820 3d20 536f 7572 6365    graph = Source
+0000e860: 2867 7261 7068 5f73 7472 290a 2020 2020  (graph_str).    
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e880: 706e 675f 7374 7220 3d20 6772 6170 682e  png_str = graph.
+0000e890: 7069 7065 2866 6f72 6d61 743d 2270 6e67  pipe(format="png
+0000e8a0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000e8b0: 2020 2020 2020 2069 6620 6469 7370 6c61         if displa
+0000e8c0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8e0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0000e8f0: 5f6a 7570 7974 6572 2829 3a0a 2020 2020  _jupyter():.    
+0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e910: 2020 2020 2020 2020 6469 7370 6c61 792e          display.
+0000e920: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
+0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e940: 2020 2020 2020 2022 5761 726e 696e 673a         "Warning:
+0000e950: 2049 7079 7468 6f6e 2069 6e73 7461 6e63   Ipython instanc
+0000e960: 6520 6e6f 7420 666f 756e 642e 5c6e 2229  e not found.\n")
+0000e970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e980: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+0000e990: 706c 6179 2e77 7269 7465 2870 6e67 5f73  play.write(png_s
+0000e9a0: 7472 290a 2020 2020 2020 2020 2020 2020  tr).            
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9c0: 6469 7370 6c61 792e 666c 7573 6828 290a  display.flush().
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea00: 2020 2020 2020 2020 2020 6672 6f6d 2049            from I
+0000ea10: 5079 7468 6f6e 2e64 6973 706c 6179 2069  Python.display i
+0000ea20: 6d70 6f72 7420 6469 7370 6c61 7920 6173  mport display as
+0000ea30: 2069 6469 7370 6c61 790a 2020 2020 2020   idisplay.      
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 2020 2020 2020 6672 6f6d 2049 5079 7468        from IPyth
+0000ea60: 6f6e 2e64 6973 706c 6179 2069 6d70 6f72  on.display impor
+0000ea70: 7420 496d 6167 650a 0a20 2020 2020 2020  t Image..       
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea90: 2020 2020 2069 6469 7370 6c61 7928 496d       idisplay(Im
+0000eaa0: 6167 6528 706e 675f 7374 7229 290a 2020  age(png_str)).  
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+0000ead0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000eae0: 2020 2020 2020 7265 7475 726e 2070 6e67        return png
+0000eaf0: 5f73 7472 0a20 2020 2020 2020 2020 2020  _str.           
+0000eb00: 2020 2020 2069 6620 6f75 7470 7574 5f66       if output_f
+0000eb10: 6f72 6d61 7420 3d3d 2022 6173 6369 6922  ormat == "ascii"
+0000eb20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000eb30: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
+0000eb40: 5f67 7261 7068 5f65 6173 7928 293a 0a20  _graph_easy():. 
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb60: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000eb70: 6e64 6572 2867 7261 7068 5f73 7472 290a  nder(graph_str).
+0000eb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb90: 2020 2020 2069 6d70 6f72 7420 7375 6270       import subp
+0000eba0: 726f 6365 7373 0a20 2020 2020 2020 2020  rocess.         
+0000ebb0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+0000ebc0: 205b 2265 6368 6f22 2c20 6772 6170 685f   ["echo", graph_
+0000ebd0: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
+0000ebe0: 2020 2020 2020 2020 2077 6974 6820 7375           with su
+0000ebf0: 6270 726f 6365 7373 2e50 6f70 656e 2863  bprocess.Popen(c
+0000ec00: 6d64 2c20 7374 646f 7574 3d73 7562 7072  md, stdout=subpr
+0000ec10: 6f63 6573 732e 5049 5045 2920 6173 2070  ocess.PIPE) as p
+0000ec20: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000ec30: 2020 2020 2020 2020 2020 2070 3220 3d20             p2 = 
+0000ec40: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
+0000ec50: 5f6f 7574 7075 7428 0a20 2020 2020 2020  _output(.       
+0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec70: 2020 2020 205b 2267 7261 7068 2d65 6173       ["graph-eas
+0000ec80: 7922 5d2c 2073 7464 696e 3d70 312e 7374  y"], stdin=p1.st
+0000ec90: 646f 7574 290a 2020 2020 2020 2020 2020  dout).          
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000ecb0: 7320 3d20 7032 2e64 6563 6f64 6528 2275  s = p2.decode("u
+0000ecc0: 7466 2d38 2229 0a20 2020 2020 2020 2020  tf-8").         
+0000ecd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ece0: 6e20 7265 6e64 6572 2872 6573 290a 2020  n render(res).  
+0000ecf0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000ed00: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+0000ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed20: 2020 2020 6622 696e 7661 6c69 6420 666f      f"invalid fo
+0000ed30: 726d 6174 207b 6f75 7470 7574 5f66 6f72  rmat {output_for
+0000ed40: 6d61 747d 2c20 220a 2020 2020 2020 2020  mat}, ".        
+0000ed50: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+0000ed60: 2073 7667 2c20 706e 672c 2061 7363 6969   svg, png, ascii
+0000ed70: 2c20 6f72 2064 6f74 2229 0a20 2020 2020  , or dot").     
+0000ed80: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+0000ed90: 6563 7574 6162 6c65 4e6f 7446 6f75 6e64  ecutableNotFound
+0000eda0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+0000edb0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+0000edc0: 7469 6d65 4572 726f 7228 0a20 2020 2020  timeError(.     
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ede0: 7573 6520 2762 7265 7720 696e 7374 616c  use 'brew instal
+0000edf0: 6c20 6772 6170 6876 697a 2720 6f72 2075  l graphviz' or u
+0000ee00: 7365 2027 6d65 7468 6f64 3d61 6363 6572  se 'method=accer
+0000ee10: 6e27 222c 0a20 2020 2020 2020 2020 2020  n'",.           
+0000ee20: 2020 2020 2029 2066 726f 6d20 650a 2020       ) from e.  
+0000ee30: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000ee40: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0000ee50: 2020 2020 6622 696e 7661 6c69 6420 6d65      f"invalid me
+0000ee60: 7468 6f64 207b 6d65 7468 6f64 7d2c 2075  thod {method}, u
+0000ee70: 7365 2061 6363 6572 6e20 6f72 2064 6f74  se accern or dot
+0000ee80: 2229 0a0a 2020 2020 6465 6620 7072 6574  ")..    def pret
+0000ee90: 7479 5f6f 626a 280a 2020 2020 2020 2020  ty_obj(.        
+0000eea0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000eeb0: 2020 2020 2020 6e6f 6465 735f 6f6e 6c79        nodes_only
+0000eec0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0000eed0: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
+0000eee0: 775f 756e 6963 6f64 653a 2062 6f6f 6c20  w_unicode: bool 
+0000eef0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+0000ef00: 2020 2020 6669 656c 6473 3a20 4f70 7469      fields: Opti
+0000ef10: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
+0000ef20: 3d20 4e6f 6e65 2920 2d3e 204c 6973 745b  = None) -> List[
+0000ef30: 4461 6750 7265 7474 794e 6f64 655d 3a0a  DagPrettyNode]:.
+0000ef40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000ef50: 656c 662e 5f70 7265 7474 7928 0a20 2020  elf._pretty(.   
+0000ef60: 2020 2020 2020 2020 206e 6f64 6573 5f6f           nodes_o
+0000ef70: 6e6c 793d 6e6f 6465 735f 6f6e 6c79 2c0a  nly=nodes_only,.
+0000ef80: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
+0000ef90: 775f 756e 6963 6f64 653d 616c 6c6f 775f  w_unicode=allow_
+0000efa0: 756e 6963 6f64 652c 0a20 2020 2020 2020  unicode,.       
+0000efb0: 2020 2020 2066 6965 6c64 733d 6669 656c       fields=fiel
+0000efc0: 6473 295b 226e 6f64 6573 225d 0a0a 2020  ds)["nodes"]..  
+0000efd0: 2020 6465 6620 6765 745f 6465 6628 7365    def get_def(se
+0000efe0: 6c66 2c20 6675 6c6c 3a20 626f 6f6c 203d  lf, full: bool =
+0000eff0: 2054 7275 6529 202d 3e20 5573 6572 4461   True) -> UserDa
+0000f000: 6744 6566 3a0a 2020 2020 2020 2020 7265  gDef:.        re
+0000f010: 7475 726e 2063 6173 7428 5573 6572 4461  turn cast(UserDa
+0000f020: 6744 6566 2c20 7365 6c66 2e5f 636c 6965  gDef, self._clie
+0000f030: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
+0000f040: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+0000f050: 484f 445f 4745 542c 2022 2f64 6167 5f64  HOD_GET, "/dag_d
+0000f060: 6566 222c 207b 0a20 2020 2020 2020 2020  ef", {.         
+0000f070: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
+0000f080: 6c66 2e67 6574 5f75 7269 2829 2c0a 2020  lf.get_uri(),.  
+0000f090: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+0000f0a0: 756c 6c22 3a20 6675 6c6c 2c0a 2020 2020  ull": full,.    
+0000f0b0: 2020 2020 2020 2020 7d29 290a 0a20 2020          }))..   
+0000f0c0: 2064 6566 2073 6574 5f61 7474 7228 7365   def set_attr(se
+0000f0d0: 6c66 2c20 6174 7472 3a20 7374 722c 2076  lf, attr: str, v
+0000f0e0: 616c 7565 3a20 416e 7929 202d 3e20 4e6f  alue: Any) -> No
+0000f0f0: 6e65 3a0a 2020 2020 2020 2020 6461 675f  ne:.        dag_
+0000f100: 6465 6620 3d20 7365 6c66 2e67 6574 5f64  def = self.get_d
+0000f110: 6566 2829 0a20 2020 2020 2020 2064 6167  ef().        dag
+0000f120: 5f64 6566 5b61 7474 725d 203d 2076 616c  _def[attr] = val
+0000f130: 7565 2020 2320 7479 7065 3a20 6967 6e6f  ue  # type: igno
+0000f140: 7265 0a20 2020 2020 2020 2073 656c 662e  re.        self.
+0000f150: 5f63 6c69 656e 742e 7365 745f 6461 6728  _client.set_dag(
+0000f160: 7365 6c66 2e67 6574 5f75 7269 2829 2c20  self.get_uri(), 
+0000f170: 6461 675f 6465 6629 0a0a 2020 2020 6465  dag_def)..    de
+0000f180: 6620 7365 745f 6e61 6d65 2873 656c 662c  f set_name(self,
+0000f190: 2076 616c 7565 3a20 7374 7229 202d 3e20   value: str) -> 
+0000f1a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
+0000f1b0: 6c66 2e73 6574 5f61 7474 7228 226e 616d  lf.set_attr("nam
+0000f1c0: 6522 2c20 7661 6c75 6529 0a0a 2020 2020  e", value)..    
+0000f1d0: 6465 6620 7365 745f 636f 6d70 616e 7928  def set_company(
+0000f1e0: 7365 6c66 2c20 7661 6c75 653a 2073 7472  self, value: str
+0000f1f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000f200: 2020 2073 656c 662e 7365 745f 6174 7472     self.set_attr
+0000f210: 2822 636f 6d70 616e 7922 2c20 7661 6c75  ("company", valu
+0000f220: 6529 0a0a 2020 2020 6465 6620 7365 745f  e)..    def set_
+0000f230: 7374 6174 655f 7572 6928 7365 6c66 2c20  state_uri(self, 
+0000f240: 7661 6c75 653a 2073 7472 2920 2d3e 204e  value: str) -> N
+0000f250: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
+0000f260: 662e 7365 745f 6174 7472 2822 7374 6174  f.set_attr("stat
+0000f270: 655f 7572 6922 2c20 7661 6c75 6529 0a0a  e_uri", value)..
+0000f280: 2020 2020 6465 6620 7365 745f 7572 695f      def set_uri_
+0000f290: 7072 6566 6978 2873 656c 662c 2076 616c  prefix(self, val
+0000f2a0: 7565 3a20 5552 4950 7265 6669 7829 202d  ue: URIPrefix) -
+0000f2b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000f2c0: 7365 6c66 2e73 6574 5f61 7474 7228 2275  self.set_attr("u
+0000f2d0: 7269 5f70 7265 6669 7822 2c20 7661 6c75  ri_prefix", valu
+0000f2e0: 6529 0a0a 2020 2020 6465 6620 7365 745f  e)..    def set_
+0000f2f0: 6869 6768 5f70 7269 6f72 6974 7928 7365  high_priority(se
+0000f300: 6c66 2c20 7661 6c75 653a 2062 6f6f 6c29  lf, value: bool)
+0000f310: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000f320: 2020 7365 6c66 2e73 6574 5f61 7474 7228    self.set_attr(
+0000f330: 2268 6967 685f 7072 696f 7269 7479 222c  "high_priority",
+0000f340: 2076 616c 7565 290a 0a20 2020 2064 6566   value)..    def
+0000f350: 2073 6574 5f71 7565 7565 5f6d 6e67 2873   set_queue_mng(s
+0000f360: 656c 662c 2076 616c 7565 3a20 4f70 7469  elf, value: Opti
+0000f370: 6f6e 616c 5b73 7472 5d29 202d 3e20 4e6f  onal[str]) -> No
+0000f380: 6e65 3a0a 2020 2020 2020 2020 7365 6c66  ne:.        self
+0000f390: 2e73 6574 5f61 7474 7228 2271 7565 7565  .set_attr("queue
+0000f3a0: 5f6d 6e67 222c 2076 616c 7565 290a 0a20  _mng", value).. 
+0000f3b0: 2020 2064 6566 2073 6574 5f76 6572 7369     def set_versi
+0000f3c0: 6f6e 5f6f 7665 7272 6964 6528 7365 6c66  on_override(self
+0000f3d0: 2c20 7661 6c75 653a 204f 7074 696f 6e61  , value: Optiona
+0000f3e0: 6c5b 7374 725d 2920 2d3e 204e 6f6e 653a  l[str]) -> None:
+0000f3f0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000f400: 745f 6174 7472 2822 7665 7273 696f 6e5f  t_attr("version_
+0000f410: 6f76 6572 7269 6465 222c 2076 616c 7565  override", value
+0000f420: 290a 0a20 2020 2064 6566 2073 6574 5f6b  )..    def set_k
+0000f430: 6166 6b61 5f69 6e70 7574 5f74 6f70 6963  afka_input_topic
+0000f440: 2873 656c 662c 2076 616c 7565 3a20 4f70  (self, value: Op
+0000f450: 7469 6f6e 616c 5b73 7472 5d29 202d 3e20  tional[str]) -> 
+0000f460: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
+0000f470: 6c66 2e73 6574 5f61 7474 7228 226b 6166  lf.set_attr("kaf
+0000f480: 6b61 5f69 6e70 7574 5f74 6f70 6963 222c  ka_input_topic",
+0000f490: 2076 616c 7565 290a 0a20 2020 2064 6566   value)..    def
+0000f4a0: 2073 6574 5f6b 6166 6b61 5f6f 7574 7075   set_kafka_outpu
+0000f4b0: 745f 746f 7069 6328 7365 6c66 2c20 7661  t_topic(self, va
+0000f4c0: 6c75 653a 204f 7074 696f 6e61 6c5b 7374  lue: Optional[st
+0000f4d0: 725d 2920 2d3e 204e 6f6e 653a 0a20 2020  r]) -> None:.   
+0000f4e0: 2020 2020 2073 656c 662e 7365 745f 6174       self.set_at
+0000f4f0: 7472 2822 6b61 666b 615f 6f75 7470 7574  tr("kafka_output
+0000f500: 5f74 6f70 6963 222c 2076 616c 7565 290a  _topic", value).
+0000f510: 0a20 2020 2040 6f76 6572 6c6f 6164 0a20  .    @overload. 
+0000f520: 2020 2064 6566 2063 6865 636b 5f71 7565     def check_que
+0000f530: 7565 5f73 7461 7473 2820 2023 2070 796c  ue_stats(  # pyl
+0000f540: 696e 743a 2064 6973 6162 6c65 3d6e 6f2d  int: disable=no-
+0000f550: 7365 6c66 2d75 7365 0a20 2020 2020 2020  self-use.       
+0000f560: 2020 2020 2073 656c 662c 206d 696e 696d       self, minim
+0000f570: 616c 3a20 4c69 7465 7261 6c5b 5472 7565  al: Literal[True
+0000f580: 5d29 202d 3e20 4d69 6e69 6d61 6c51 7565  ]) -> MinimalQue
+0000f590: 7565 5374 6174 7352 6573 706f 6e73 653a  ueStatsResponse:
+0000f5a0: 0a20 2020 2020 2020 202e 2e2e 0a0a 2020  .        .....  
+0000f5b0: 2020 406f 7665 726c 6f61 640a 2020 2020    @overload.    
+0000f5c0: 6465 6620 6368 6563 6b5f 7175 6575 655f  def check_queue_
+0000f5d0: 7374 6174 7328 2020 2320 7079 6c69 6e74  stats(  # pylint
+0000f5e0: 3a20 6469 7361 626c 653d 6e6f 2d73 656c  : disable=no-sel
+0000f5f0: 662d 7573 650a 2020 2020 2020 2020 2020  f-use.          
+0000f600: 2020 7365 6c66 2c20 6d69 6e69 6d61 6c3a    self, minimal:
+0000f610: 204c 6974 6572 616c 5b46 616c 7365 5d29   Literal[False])
+0000f620: 202d 3e20 5175 6575 6553 7461 7473 5265   -> QueueStatsRe
+0000f630: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+0000f640: 2e2e 2e0a 0a20 2020 2040 6f76 6572 6c6f  .....    @overlo
+0000f650: 6164 0a20 2020 2064 6566 2063 6865 636b  ad.    def check
+0000f660: 5f71 7565 7565 5f73 7461 7473 2820 2023  _queue_stats(  #
+0000f670: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+0000f680: 3d6e 6f2d 7365 6c66 2d75 7365 0a20 2020  =no-self-use.   
+0000f690: 2020 2020 2020 2020 2073 656c 662c 206d           self, m
+0000f6a0: 696e 696d 616c 3a20 626f 6f6c 2920 2d3e  inimal: bool) ->
+0000f6b0: 2055 6e69 6f6e 5b0a 2020 2020 2020 2020   Union[.        
+0000f6c0: 2020 2020 2020 2020 4d69 6e69 6d61 6c51          MinimalQ
+0000f6d0: 7565 7565 5374 6174 7352 6573 706f 6e73  ueueStatsRespons
+0000f6e0: 652c 2051 7565 7565 5374 6174 7352 6573  e, QueueStatsRes
+0000f6f0: 706f 6e73 655d 3a0a 2020 2020 2020 2020  ponse]:.        
+0000f700: 2e2e 2e0a 0a20 2020 2064 6566 2063 6865  .....    def che
+0000f710: 636b 5f71 7565 7565 5f73 7461 7473 2873  ck_queue_stats(s
+0000f720: 656c 662c 206d 696e 696d 616c 3a20 626f  elf, minimal: bo
+0000f730: 6f6c 2920 2d3e 2055 6e69 6f6e 5b0a 2020  ol) -> Union[.  
+0000f740: 2020 2020 2020 2020 2020 4d69 6e69 6d61            Minima
+0000f750: 6c51 7565 7565 5374 6174 7352 6573 706f  lQueueStatsRespo
+0000f760: 6e73 652c 2051 7565 7565 5374 6174 7352  nse, QueueStatsR
+0000f770: 6573 706f 6e73 655d 3a0a 2020 2020 2020  esponse]:.      
+0000f780: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
+0000f790: 6c69 656e 742e 6368 6563 6b5f 7175 6575  lient.check_queu
+0000f7a0: 655f 7374 6174 7328 7365 6c66 2e67 6574  e_stats(self.get
+0000f7b0: 5f75 7269 2829 2c20 6d69 6e69 6d61 6c3d  _uri(), minimal=
+0000f7c0: 6d69 6e69 6d61 6c29 0a0a 2020 2020 6465  minimal)..    de
+0000f7d0: 6620 7363 616c 655f 776f 726b 6572 2873  f scale_worker(s
+0000f7e0: 656c 662c 2072 6570 6c69 6361 733a 2069  elf, replicas: i
+0000f7f0: 6e74 2920 2d3e 2069 6e74 3a0a 2020 2020  nt) -> int:.    
+0000f800: 2020 2020 7265 7475 726e 2063 6173 7428      return cast(
+0000f810: 576f 726b 6572 5363 616c 652c 2073 656c  WorkerScale, sel
+0000f820: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+0000f830: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+0000f840: 2020 2020 4d45 5448 4f44 5f50 5554 2c20      METHOD_PUT, 
+0000f850: 222f 776f 726b 6572 222c 207b 0a20 2020  "/worker", {.   
+0000f860: 2020 2020 2020 2020 2020 2020 2022 6461               "da
+0000f870: 6722 3a20 7365 6c66 2e67 6574 5f75 7269  g": self.get_uri
+0000f880: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0000f890: 2020 2020 2272 6570 6c69 6361 7322 3a20      "replicas": 
+0000f8a0: 7265 706c 6963 6173 2c0a 2020 2020 2020  replicas,.      
+0000f8b0: 2020 2020 2020 2020 2020 2274 6173 6b22            "task"
+0000f8c0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+0000f8d0: 2020 2020 7d29 295b 226e 756d 5f72 6570      }))["num_rep
+0000f8e0: 6c69 6361 7322 5d0a 0a20 2020 2064 6566  licas"]..    def
+0000f8f0: 2072 656c 6f61 6428 7365 6c66 2c20 7469   reload(self, ti
+0000f900: 6d65 7374 616d 703a 204f 7074 696f 6e61  mestamp: Optiona
+0000f910: 6c5b 666c 6f61 745d 203d 204e 6f6e 6529  l[float] = None)
+0000f920: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
+0000f930: 2020 2072 6574 7572 6e20 6361 7374 2844     return cast(D
+0000f940: 6167 5265 6c6f 6164 2c20 7365 6c66 2e5f  agReload, self._
+0000f950: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
+0000f960: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+0000f970: 204d 4554 484f 445f 5055 542c 2022 2f64   METHOD_PUT, "/d
+0000f980: 6167 5f72 656c 6f61 6422 2c20 7b0a 2020  ag_reload", {.  
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+0000f9a0: 6167 223a 2073 656c 662e 6765 745f 7572  ag": self.get_ur
+0000f9b0: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
+0000f9c0: 2020 2020 2022 7768 656e 223a 2074 696d       "when": tim
+0000f9d0: 6573 7461 6d70 2c0a 2020 2020 2020 2020  estamp,.        
+0000f9e0: 2020 2020 7d29 295b 2277 6865 6e22 5d0a      }))["when"].
+0000f9f0: 0a20 2020 2064 6566 2067 6574 5f6b 6166  .    def get_kaf
+0000fa00: 6b61 5f69 6e70 7574 5f74 6f70 6963 2873  ka_input_topic(s
+0000fa10: 656c 662c 2070 6f73 7466 6978 3a20 7374  elf, postfix: st
+0000fa20: 7220 3d20 2222 2920 2d3e 2073 7472 3a0a  r = "") -> str:.
+0000fa30: 2020 2020 2020 2020 7265 7320 3d20 6361          res = ca
+0000fa40: 7374 284b 6166 6b61 546f 7069 634e 616d  st(KafkaTopicNam
+0000fa50: 6573 2c20 7365 6c66 2e5f 636c 6965 6e74  es, self._client
+0000fa60: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+0000fa70: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+0000fa80: 445f 4745 542c 2022 2f6b 6166 6b61 5f74  D_GET, "/kafka_t
+0000fa90: 6f70 6963 5f6e 616d 6573 222c 207b 0a20  opic_names", {. 
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fab0: 6461 6722 3a20 7365 6c66 2e67 6574 5f75  dag": self.get_u
+0000fac0: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
+0000fad0: 2020 2020 2020 2270 6f73 7466 6978 223a        "postfix":
+0000fae0: 2070 6f73 7466 6978 2c0a 2020 2020 2020   postfix,.      
+0000faf0: 2020 2020 2020 2020 2020 226e 6f5f 6f75            "no_ou
+0000fb00: 7470 7574 223a 2054 7275 652c 0a20 2020  tput": True,.   
+0000fb10: 2020 2020 2020 2020 207d 2929 5b22 696e           }))["in
+0000fb20: 7075 7422 5d0a 2020 2020 2020 2020 6173  put"].        as
+0000fb30: 7365 7274 2072 6573 2069 7320 6e6f 7420  sert res is not 
+0000fb40: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+0000fb50: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
+0000fb60: 2067 6574 5f6b 6166 6b61 5f6f 7574 7075   get_kafka_outpu
+0000fb70: 745f 746f 7069 6328 7365 6c66 2920 2d3e  t_topic(self) ->
+0000fb80: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+0000fb90: 7320 3d20 6361 7374 284b 6166 6b61 546f  s = cast(KafkaTo
+0000fba0: 7069 634e 616d 6573 2c20 7365 6c66 2e5f  picNames, self._
+0000fbb0: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
+0000fbc0: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+0000fbd0: 204d 4554 484f 445f 4745 542c 2022 2f6b   METHOD_GET, "/k
+0000fbe0: 6166 6b61 5f74 6f70 6963 5f6e 616d 6573  afka_topic_names
+0000fbf0: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+0000fc00: 2020 2020 2022 6461 6722 3a20 7365 6c66       "dag": self
+0000fc10: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
+0000fc20: 2020 2020 2020 2020 7d29 295b 226f 7574          }))["out
+0000fc30: 7075 7422 5d0a 2020 2020 2020 2020 6173  put"].        as
+0000fc40: 7365 7274 2072 6573 2069 7320 6e6f 7420  sert res is not 
+0000fc50: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+0000fc60: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
+0000fc70: 2073 6574 5f6b 6166 6b61 5f74 6f70 6963   set_kafka_topic
+0000fc80: 5f70 6172 7469 7469 6f6e 7328 0a20 2020  _partitions(.   
+0000fc90: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+0000fca0: 2020 2020 2020 2020 2020 206e 756d 5f70             num_p
+0000fcb0: 6172 7469 7469 6f6e 733a 2069 6e74 2c0a  artitions: int,.
+0000fcc0: 2020 2020 2020 2020 2020 2020 706f 7374              post
+0000fcd0: 6669 783a 2073 7472 203d 2022 222c 0a20  fix: str = "",. 
+0000fce0: 2020 2020 2020 2020 2020 206c 6172 6765             large
+0000fcf0: 5f69 6e70 7574 5f72 6574 656e 7469 6f6e  _input_retention
+0000fd00: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0000fd10: 2020 2020 2020 2020 2020 2020 6e6f 5f6f              no_o
+0000fd20: 7574 7075 743a 2062 6f6f 6c20 3d20 4661  utput: bool = Fa
+0000fd30: 6c73 6529 202d 3e20 4b61 666b 6154 6f70  lse) -> KafkaTop
+0000fd40: 6963 733a 0a20 2020 2020 2020 2072 6574  ics:.        ret
+0000fd50: 7572 6e20 6361 7374 284b 6166 6b61 546f  urn cast(KafkaTo
+0000fd60: 7069 6373 2c20 7365 6c66 2e5f 636c 6965  pics, self._clie
+0000fd70: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
+0000fd80: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+0000fd90: 484f 445f 504f 5354 2c20 222f 6b61 666b  HOD_POST, "/kafk
+0000fda0: 615f 746f 7069 6373 222c 207b 0a20 2020  a_topics", {.   
+0000fdb0: 2020 2020 2020 2020 2020 2020 2022 6461               "da
+0000fdc0: 6722 3a20 7365 6c66 2e67 6574 5f75 7269  g": self.get_uri
+0000fdd0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0000fde0: 2020 2020 226e 756d 5f70 6172 7469 7469      "num_partiti
+0000fdf0: 6f6e 7322 3a20 6e75 6d5f 7061 7274 6974  ons": num_partit
+0000fe00: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+0000fe10: 2020 2020 2020 2270 6f73 7466 6978 223a        "postfix":
+0000fe20: 2070 6f73 7466 6978 2c0a 2020 2020 2020   postfix,.      
+0000fe30: 2020 2020 2020 2020 2020 226c 6172 6765            "large
+0000fe40: 5f69 6e70 7574 5f72 6574 656e 7469 6f6e  _input_retention
+0000fe50: 223a 206c 6172 6765 5f69 6e70 7574 5f72  ": large_input_r
+0000fe60: 6574 656e 7469 6f6e 2c0a 2020 2020 2020  etention,.      
+0000fe70: 2020 2020 2020 2020 2020 226e 6f5f 6f75            "no_ou
+0000fe80: 7470 7574 223a 206e 6f5f 6f75 7470 7574  tput": no_output
+0000fe90: 2c0a 2020 2020 2020 2020 2020 2020 7d29  ,.            })
+0000fea0: 290a 0a20 2020 2064 6566 2070 6f73 745f  )..    def post_
+0000feb0: 6b61 666b 615f 6f62 6a73 2873 656c 662c  kafka_objs(self,
+0000fec0: 2069 6e70 7574 5f6f 626a 733a 204c 6973   input_objs: Lis
+0000fed0: 745b 416e 795d 2920 2d3e 204c 6973 745b  t[Any]) -> List[
+0000fee0: 7374 725d 3a0a 2020 2020 2020 2020 6269  str]:.        bi
+0000fef0: 6f73 203d 205b 0a20 2020 2020 2020 2020  os = [.         
+0000ff00: 2020 2042 7974 6573 494f 286a 736f 6e2e     BytesIO(json.
+0000ff10: 6475 6d70 7328 0a20 2020 2020 2020 2020  dumps(.         
+0000ff20: 2020 2020 2020 2069 6e70 7574 5f6f 626a         input_obj
+0000ff30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ff40: 2020 7365 7061 7261 746f 7273 3d28 222c    separators=(",
+0000ff50: 222c 2022 3a22 292c 0a20 2020 2020 2020  ", ":"),.       
+0000ff60: 2020 2020 2020 2020 2069 6e64 656e 743d           indent=
+0000ff70: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000ff80: 2020 2020 2020 736f 7274 5f6b 6579 733d        sort_keys=
+0000ff90: 5472 7565 292e 656e 636f 6465 2822 7574  True).encode("ut
+0000ffa0: 662d 3822 2929 0a20 2020 2020 2020 2020  f-8")).         
+0000ffb0: 2020 2066 6f72 2069 6e70 7574 5f6f 626a     for input_obj
+0000ffc0: 2069 6e20 696e 7075 745f 6f62 6a73 0a20   in input_objs. 
+0000ffd0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+0000ffe0: 2072 6574 7572 6e20 7365 6c66 2e70 6f73   return self.pos
+0000fff0: 745f 6b61 666b 615f 6d73 6773 2862 696f  t_kafka_msgs(bio
+00010000: 7329 0a0a 2020 2020 6465 6620 706f 7374  s)..    def post
+00010010: 5f6b 6166 6b61 5f6d 7367 7328 0a20 2020  _kafka_msgs(.   
+00010020: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00010030: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00010040: 5f64 6174 613a 204c 6973 745b 4279 7465  _data: List[Byte
+00010050: 7349 4f5d 2c0a 2020 2020 2020 2020 2020  sIO],.          
+00010060: 2020 706f 7374 6669 783a 2073 7472 203d    postfix: str =
+00010070: 2022 2229 202d 3e20 4c69 7374 5b73 7472   "") -> List[str
+00010080: 5d3a 0a20 2020 2020 2020 206e 616d 6573  ]:.        names
+00010090: 203d 205b 6622 6669 6c65 7b70 6f73 7d22   = [f"file{pos}"
+000100a0: 2066 6f72 2070 6f73 2069 6e20 7261 6e67   for pos in rang
+000100b0: 6528 6c65 6e28 696e 7075 745f 6461 7461  e(len(input_data
+000100c0: 2929 5d0a 2020 2020 2020 2020 7265 7320  ))].        res 
+000100d0: 3d20 6361 7374 284b 6166 6b61 4d65 7373  = cast(KafkaMess
+000100e0: 6167 652c 2073 656c 662e 5f63 6c69 656e  age, self._clien
+000100f0: 742e 7265 7175 6573 745f 6a73 6f6e 280a  t.request_json(.
+00010100: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00010110: 4f44 5f46 494c 452c 2022 2f6b 6166 6b61  OD_FILE, "/kafka
+00010120: 5f6d 7367 222c 207b 0a20 2020 2020 2020  _msg", {.       
+00010130: 2020 2020 2020 2020 2022 6461 6722 3a20           "dag": 
+00010140: 7365 6c66 2e67 6574 5f75 7269 2829 2c0a  self.get_uri(),.
+00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010160: 2270 6f73 7466 6978 223a 2070 6f73 7466  "postfix": postf
+00010170: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
+00010180: 7d2c 2066 696c 6573 3d64 6963 7428 7a69  }, files=dict(zi
+00010190: 7028 6e61 6d65 732c 2069 6e70 7574 5f64  p(names, input_d
+000101a0: 6174 6129 2929 290a 2020 2020 2020 2020  ata)))).        
+000101b0: 6d73 6773 203d 2072 6573 5b22 6d65 7373  msgs = res["mess
+000101c0: 6167 6573 225d 0a20 2020 2020 2020 2072  ages"].        r
+000101d0: 6574 7572 6e20 5b6d 7367 735b 6b65 795d  eturn [msgs[key]
+000101e0: 2066 6f72 206b 6579 2069 6e20 6e61 6d65   for key in name
+000101f0: 735d 0a0a 2020 2020 6465 6620 7265 6164  s]..    def read
+00010200: 5f6b 6166 6b61 5f6f 7574 7075 7428 0a20  _kafka_output(. 
+00010210: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00010220: 0a20 2020 2020 2020 2020 2020 206f 6666  .            off
+00010230: 7365 743a 2073 7472 203d 2022 6375 7272  set: str = "curr
+00010240: 656e 7422 2c0a 2020 2020 2020 2020 2020  ent",.          
+00010250: 2020 6d61 785f 726f 7773 3a20 696e 7420    max_rows: int 
+00010260: 3d20 3130 3029 202d 3e20 4f70 7469 6f6e  = 100) -> Option
+00010270: 616c 5b42 7974 6552 6573 706f 6e73 655d  al[ByteResponse]
+00010280: 3a0a 2020 2020 2020 2020 6f66 6673 6574  :.        offset
+00010290: 5f73 7472 203d 205b 6f66 6673 6574 5d0a  _str = [offset].
+000102a0: 0a20 2020 2020 2020 2064 6566 2072 6561  .        def rea
+000102b0: 645f 7369 6e67 6c65 2829 202d 3e20 5475  d_single() -> Tu
+000102c0: 706c 655b 4f70 7469 6f6e 616c 5b42 7974  ple[Optional[Byt
+000102d0: 6552 6573 706f 6e73 655d 2c20 7374 725d  eResponse], str]
+000102e0: 3a0a 2020 2020 2020 2020 2020 2020 6375  :.            cu
+000102f0: 722c 2072 6561 645f 6374 7970 6520 3d20  r, read_ctype = 
+00010300: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
+00010310: 7565 7374 5f62 7974 6573 280a 2020 2020  uest_bytes(.    
+00010320: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00010330: 4f44 5f47 4554 2c20 222f 6b61 666b 615f  OD_GET, "/kafka_
+00010340: 6d73 6722 2c20 7b0a 2020 2020 2020 2020  msg", {.        
+00010350: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
+00010360: 223a 2073 656c 662e 6765 745f 7572 6928  ": self.get_uri(
+00010370: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00010380: 2020 2020 2020 2022 6f66 6673 6574 223a         "offset":
+00010390: 206f 6666 7365 745f 7374 725b 305d 2c0a   offset_str[0],.
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2020 2020 2263 6f6e 7375 6d65 725f 7479      "consumer_ty
+000103c0: 7065 223a 2043 4f4e 5355 4d45 525f 4441  pe": CONSUMER_DA
+000103d0: 472c 0a20 2020 2020 2020 2020 2020 2020  G,.             
+000103e0: 2020 207d 290a 2020 2020 2020 2020 2020     }).          
+000103f0: 2020 6f66 6673 6574 5f73 7472 5b30 5d20    offset_str[0] 
+00010400: 3d20 2263 7572 7265 6e74 220a 2020 2020  = "current".    
+00010410: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00010420: 6e74 6572 7072 6574 5f63 7479 7065 2863  nterpret_ctype(c
+00010430: 7572 2c20 7265 6164 5f63 7479 7065 292c  ur, read_ctype),
+00010440: 2072 6561 645f 6374 7970 650a 0a20 2020   read_ctype..   
+00010450: 2020 2020 2069 6620 6d61 785f 726f 7773       if max_rows
+00010460: 203c 3d20 313a 0a20 2020 2020 2020 2020   <= 1:.         
+00010470: 2020 2072 6574 7572 6e20 7265 6164 5f73     return read_s
+00010480: 696e 676c 6528 295b 305d 0a0a 2020 2020  ingle()[0]..    
+00010490: 2020 2020 7265 733a 204c 6973 745b 4279      res: List[By
+000104a0: 7465 5265 7370 6f6e 7365 5d20 3d20 5b5d  teResponse] = []
+000104b0: 0a20 2020 2020 2020 2063 7479 7065 3a20  .        ctype: 
+000104c0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000104d0: 4e6f 6e65 0a20 2020 2020 2020 2077 6869  None.        whi
+000104e0: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+000104f0: 2020 2020 2076 616c 2c20 6375 725f 6374       val, cur_ct
+00010500: 7970 6520 3d20 7265 6164 5f73 696e 676c  ype = read_singl
+00010510: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00010520: 6966 2076 616c 2069 7320 4e6f 6e65 3a0a  if val is None:.
+00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010540: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+00010550: 2020 6966 2063 7479 7065 2069 7320 4e6f    if ctype is No
+00010560: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00010570: 2020 2020 6374 7970 6520 3d20 6375 725f      ctype = cur_
+00010580: 6374 7970 650a 2020 2020 2020 2020 2020  ctype.          
+00010590: 2020 656c 6966 2063 7479 7065 2021 3d20    elif ctype != 
+000105a0: 6375 725f 6374 7970 653a 0a20 2020 2020  cur_ctype:.     
+000105b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000105c0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 2066 2269 6e63 6f6e 7369 7374 656e 7420   f"inconsistent 
+000105f0: 7265 7475 726e 2074 7970 6573 207b 6374  return types {ct
+00010600: 7970 657d 2021 3d20 7b63 7572 5f63 7479  ype} != {cur_cty
+00010610: 7065 7d22 290a 2020 2020 2020 2020 2020  pe}").          
+00010620: 2020 7265 732e 6170 7065 6e64 2876 616c    res.append(val
+00010630: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00010640: 206c 656e 2872 6573 2920 3e3d 206d 6178   len(res) >= max
+00010650: 5f72 6f77 733a 0a20 2020 2020 2020 2020  _rows:.         
+00010660: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00010670: 2020 2020 2069 6620 6e6f 7420 7265 7320       if not res 
+00010680: 6f72 2063 7479 7065 2069 7320 4e6f 6e65  or ctype is None
+00010690: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000106a0: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+000106b0: 2020 7265 7475 726e 206d 6572 6765 5f63    return merge_c
+000106c0: 7479 7065 2872 6573 2c20 6374 7970 6529  type(res, ctype)
+000106d0: 0a0a 2020 2020 6465 6620 6765 745f 6b61  ..    def get_ka
+000106e0: 666b 615f 6f66 6673 6574 7328 0a20 2020  fka_offsets(.   
+000106f0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00010700: 2020 2020 2020 2020 2020 2061 6c69 7665             alive
+00010710: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
+00010720: 2020 2020 706f 7374 6669 783a 204f 7074      postfix: Opt
+00010730: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00010740: 6529 202d 3e20 4b61 666b 614f 6666 7365  e) -> KafkaOffse
+00010750: 7473 3a0a 2020 2020 2020 2020 6172 6773  ts:.        args
+00010760: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00010770: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
+00010780: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
+00010790: 2020 2020 2261 6c69 7665 223a 2069 6e74      "alive": int
+000107a0: 2861 6c69 7665 292c 0a20 2020 2020 2020  (alive),.       
+000107b0: 207d 0a20 2020 2020 2020 2069 6620 706f   }.        if po
+000107c0: 7374 6669 7820 6973 206e 6f74 204e 6f6e  stfix is not Non
+000107d0: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+000107e0: 7267 735b 2270 6f73 7466 6978 225d 203d  rgs["postfix"] =
+000107f0: 2070 6f73 7466 6978 0a20 2020 2020 2020   postfix.       
+00010800: 2072 6574 7572 6e20 6361 7374 284b 6166   return cast(Kaf
+00010810: 6b61 4f66 6673 6574 732c 2073 656c 662e  kaOffsets, self.
+00010820: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
+00010830: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
+00010840: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
+00010850: 6b61 666b 615f 6f66 6673 6574 7322 2c20  kafka_offsets", 
+00010860: 6172 6773 2929 0a0a 2020 2020 6465 6620  args))..    def 
+00010870: 6765 745f 6b61 666b 615f 7468 726f 7567  get_kafka_throug
+00010880: 6870 7574 280a 2020 2020 2020 2020 2020  hput(.          
+00010890: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000108a0: 2020 2020 706f 7374 6669 783a 204f 7074      postfix: Opt
+000108b0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000108c0: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
+000108d0: 6567 6d65 6e74 5f69 6e74 6572 7661 6c3a  egment_interval:
+000108e0: 2066 6c6f 6174 203d 2031 3230 2e30 2c0a   float = 120.0,.
+000108f0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+00010900: 656e 7473 3a20 696e 7420 3d20 3529 202d  ents: int = 5) -
+00010910: 3e20 4b61 666b 6154 6872 6f75 6768 7075  > KafkaThroughpu
+00010920: 743a 0a20 2020 2020 2020 2061 7373 6572  t:.        asser
+00010930: 7420 7365 676d 656e 7473 203e 2030 0a20  t segments > 0. 
+00010940: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+00010950: 676d 656e 745f 696e 7465 7276 616c 203e  gment_interval >
+00010960: 2030 2e30 0a20 2020 2020 2020 206f 6666   0.0.        off
+00010970: 7365 7473 203d 2073 656c 662e 6765 745f  sets = self.get_
+00010980: 6b61 666b 615f 6f66 6673 6574 7328 706f  kafka_offsets(po
+00010990: 7374 6669 783d 706f 7374 6669 782c 2061  stfix=postfix, a
+000109a0: 6c69 7665 3d46 616c 7365 290a 2020 2020  live=False).    
+000109b0: 2020 2020 6e6f 7720 3d20 7469 6d65 2e6d      now = time.m
+000109c0: 6f6e 6f74 6f6e 6963 2829 0a20 2020 2020  onotonic().     
+000109d0: 2020 206d 6561 7375 7265 6d65 6e74 733a     measurements:
+000109e0: 204c 6973 745b 5475 706c 655b 696e 742c   List[Tuple[int,
+000109f0: 2069 6e74 2c20 696e 742c 2069 6e74 2c20   int, int, int, 
+00010a00: 666c 6f61 745d 5d20 3d20 5b28 0a20 2020  float]] = [(.   
+00010a10: 2020 2020 2020 2020 206f 6666 7365 7473           offsets
+00010a20: 5b22 696e 7075 7422 5d2c 0a20 2020 2020  ["input"],.     
+00010a30: 2020 2020 2020 206f 6666 7365 7473 5b22         offsets["
+00010a40: 6f75 7470 7574 225d 2c0a 2020 2020 2020  output"],.      
+00010a50: 2020 2020 2020 6f66 6673 6574 735b 2265        offsets["e
+00010a60: 7272 6f72 225d 2c0a 2020 2020 2020 2020  rror"],.        
+00010a70: 2020 2020 6f66 6673 6574 735b 2265 7272      offsets["err
+00010a80: 6f72 5f6d 7367 225d 2c0a 2020 2020 2020  or_msg"],.      
+00010a90: 2020 2020 2020 6e6f 772c 0a20 2020 2020        now,.     
+00010aa0: 2020 2029 5d0a 2020 2020 2020 2020 666f     )].        fo
+00010ab0: 7220 5f20 696e 2072 616e 6765 2873 6567  r _ in range(seg
+00010ac0: 6d65 6e74 7329 3a0a 2020 2020 2020 2020  ments):.        
+00010ad0: 2020 2020 7072 6576 203d 206e 6f77 0a20      prev = now. 
+00010ae0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+00010af0: 206e 6f77 202d 2070 7265 7620 3c20 7365   now - prev < se
+00010b00: 676d 656e 745f 696e 7465 7276 616c 3a0a  gment_interval:.
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b20: 7469 6d65 2e73 6c65 6570 286d 6178 2830  time.sleep(max(0
+00010b30: 2e30 2c20 7365 676d 656e 745f 696e 7465  .0, segment_inte
+00010b40: 7276 616c 202d 2028 6e6f 7720 2d20 7072  rval - (now - pr
+00010b50: 6576 2929 290a 2020 2020 2020 2020 2020  ev))).          
+00010b60: 2020 2020 2020 6e6f 7720 3d20 7469 6d65        now = time
+00010b70: 2e6d 6f6e 6f74 6f6e 6963 2829 0a20 2020  .monotonic().   
+00010b80: 2020 2020 2020 2020 206f 6666 7365 7473           offsets
+00010b90: 203d 2073 656c 662e 6765 745f 6b61 666b   = self.get_kafk
+00010ba0: 615f 6f66 6673 6574 7328 706f 7374 6669  a_offsets(postfi
+00010bb0: 783d 706f 7374 6669 782c 2061 6c69 7665  x=postfix, alive
+00010bc0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00010bd0: 2020 2020 6d65 6173 7572 656d 656e 7473      measurements
+00010be0: 2e61 7070 656e 6428 280a 2020 2020 2020  .append((.      
+00010bf0: 2020 2020 2020 2020 2020 6f66 6673 6574            offset
+00010c00: 735b 2269 6e70 7574 225d 2c0a 2020 2020  s["input"],.    
+00010c10: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
+00010c20: 6574 735b 226f 7574 7075 7422 5d2c 0a20  ets["output"],. 
+00010c30: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00010c40: 6666 7365 7473 5b22 6572 726f 7222 5d2c  ffsets["error"],
+00010c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c60: 206f 6666 7365 7473 5b22 6572 726f 725f   offsets["error_
+00010c70: 6d73 6722 5d2c 0a20 2020 2020 2020 2020  msg"],.         
+00010c80: 2020 2020 2020 206e 6f77 2c0a 2020 2020         now,.    
+00010c90: 2020 2020 2020 2020 2929 0a20 2020 2020          )).     
+00010ca0: 2020 2066 6972 7374 203d 206d 6561 7375     first = measu
+00010cb0: 7265 6d65 6e74 735b 305d 0a20 2020 2020  rements[0].     
+00010cc0: 2020 206c 6173 7420 3d20 6d65 6173 7572     last = measur
+00010cd0: 656d 656e 7473 5b2d 315d 0a20 2020 2020  ements[-1].     
+00010ce0: 2020 2074 6f74 616c 5f69 6e70 7574 203d     total_input =
+00010cf0: 206c 6173 745b 305d 202d 2066 6972 7374   last[0] - first
+00010d00: 5b30 5d0a 2020 2020 2020 2020 746f 7461  [0].        tota
+00010d10: 6c5f 6f75 7470 7574 203d 206c 6173 745b  l_output = last[
+00010d20: 315d 202d 2066 6972 7374 5b31 5d0a 2020  1] - first[1].  
+00010d30: 2020 2020 2020 6572 726f 7273 203d 206c        errors = l
+00010d40: 6173 745b 325d 202d 2066 6972 7374 5b32  ast[2] - first[2
+00010d50: 5d0a 2020 2020 2020 2020 6572 726f 725f  ].        error_
+00010d60: 6d73 6773 203d 206c 6173 745b 335d 202d  msgs = last[3] -
+00010d70: 2066 6972 7374 5b33 5d0a 2020 2020 2020   first[3].      
+00010d80: 2020 746f 7461 6c20 3d20 6c61 7374 5b34    total = last[4
+00010d90: 5d20 2d20 6669 7273 745b 345d 0a20 2020  ] - first[4].   
+00010da0: 2020 2020 2069 6e70 7574 5f73 6567 6d65       input_segme
+00010db0: 6e74 733a 204c 6973 745b 666c 6f61 745d  nts: List[float]
+00010dc0: 203d 205b 5d0a 2020 2020 2020 2020 6f75   = [].        ou
+00010dd0: 7470 7574 5f73 6567 6d65 6e74 733a 204c  tput_segments: L
+00010de0: 6973 745b 666c 6f61 745d 203d 205b 5d0a  ist[float] = [].
+00010df0: 2020 2020 2020 2020 6375 725f 696e 7075          cur_inpu
+00010e00: 7420 3d20 6669 7273 745b 305d 0a20 2020  t = first[0].   
+00010e10: 2020 2020 2063 7572 5f6f 7574 7075 7420       cur_output 
+00010e20: 3d20 6669 7273 745b 315d 0a20 2020 2020  = first[1].     
+00010e30: 2020 2063 7572 5f74 696d 6520 3d20 6669     cur_time = fi
+00010e40: 7273 745b 345d 0a20 2020 2020 2020 2066  rst[4].        f
+00010e50: 6f72 2028 6e65 7874 5f69 6e70 7574 2c20  or (next_input, 
+00010e60: 6e65 7874 5f6f 7574 7075 742c 205f 2c20  next_output, _, 
+00010e70: 5f2c 206e 6578 745f 7469 6d65 2920 696e  _, next_time) in
+00010e80: 206d 6561 7375 7265 6d65 6e74 735b 313a   measurements[1:
+00010e90: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+00010ea0: 6567 5f74 696d 6520 3d20 6e65 7874 5f74  eg_time = next_t
+00010eb0: 696d 6520 2d20 6375 725f 7469 6d65 0a20  ime - cur_time. 
+00010ec0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00010ed0: 5f73 6567 6d65 6e74 732e 6170 7065 6e64  _segments.append
+00010ee0: 2828 6e65 7874 5f69 6e70 7574 202d 2063  ((next_input - c
+00010ef0: 7572 5f69 6e70 7574 2920 2f20 7365 675f  ur_input) / seg_
+00010f00: 7469 6d65 290a 2020 2020 2020 2020 2020  time).          
+00010f10: 2020 6f75 7470 7574 5f73 6567 6d65 6e74    output_segment
+00010f20: 732e 6170 7065 6e64 2828 6e65 7874 5f6f  s.append((next_o
+00010f30: 7574 7075 7420 2d20 6375 725f 6f75 7470  utput - cur_outp
+00010f40: 7574 2920 2f20 7365 675f 7469 6d65 290a  ut) / seg_time).
+00010f50: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
+00010f60: 696e 7075 7420 3d20 6e65 7874 5f69 6e70  input = next_inp
+00010f70: 7574 0a20 2020 2020 2020 2020 2020 2063  ut.            c
+00010f80: 7572 5f6f 7574 7075 7420 3d20 6e65 7874  ur_output = next
+00010f90: 5f6f 7574 7075 740a 2020 2020 2020 2020  _output.        
+00010fa0: 2020 2020 6375 725f 7469 6d65 203d 206e      cur_time = n
+00010fb0: 6578 745f 7469 6d65 0a20 2020 2020 2020  ext_time.       
+00010fc0: 2069 6e70 7574 7320 3d20 7064 2e53 6572   inputs = pd.Ser
+00010fd0: 6965 7328 696e 7075 745f 7365 676d 656e  ies(input_segmen
+00010fe0: 7473 290a 2020 2020 2020 2020 6f75 7470  ts).        outp
+00010ff0: 7574 7320 3d20 7064 2e53 6572 6965 7328  uts = pd.Series(
+00011000: 6f75 7470 7574 5f73 6567 6d65 6e74 7329  output_segments)
+00011010: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011020: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
+00011030: 6167 223a 2073 656c 662e 6765 745f 7572  ag": self.get_ur
+00011040: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
+00011050: 2022 696e 7075 7422 3a20 7b0a 2020 2020   "input": {.    
+00011060: 2020 2020 2020 2020 2020 2020 2274 6872              "thr
+00011070: 6f75 6768 7075 7422 3a20 746f 7461 6c5f  oughput": total_
+00011080: 696e 7075 7420 2f20 746f 7461 6c2c 0a20  input / total,. 
+00011090: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000110a0: 6d61 7822 3a20 696e 7075 7473 2e6d 6178  max": inputs.max
+000110b0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+000110c0: 2020 2020 226d 696e 223a 2069 6e70 7574      "min": input
+000110d0: 732e 6d69 6e28 292c 0a20 2020 2020 2020  s.min(),.       
+000110e0: 2020 2020 2020 2020 2022 7374 6464 6576           "stddev
+000110f0: 223a 2069 6e70 7574 732e 7374 6428 292c  ": inputs.std(),
+00011100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011110: 2022 7365 676d 656e 7473 223a 2073 6567   "segments": seg
+00011120: 6d65 6e74 732c 0a20 2020 2020 2020 2020  ments,.         
+00011130: 2020 2020 2020 2022 636f 756e 7422 3a20         "count": 
+00011140: 746f 7461 6c5f 696e 7075 742c 0a20 2020  total_input,.   
+00011150: 2020 2020 2020 2020 2020 2020 2022 746f               "to
+00011160: 7461 6c22 3a20 746f 7461 6c2c 0a20 2020  tal": total,.   
+00011170: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00011180: 2020 2020 2020 2020 226f 7574 7075 7422          "output"
+00011190: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000111a0: 2020 2020 2274 6872 6f75 6768 7075 7422      "throughput"
+000111b0: 3a20 746f 7461 6c5f 6f75 7470 7574 202f  : total_output /
+000111c0: 2074 6f74 616c 2c0a 2020 2020 2020 2020   total,.        
+000111d0: 2020 2020 2020 2020 226d 6178 223a 206f          "max": o
+000111e0: 7574 7075 7473 2e6d 6178 2829 2c0a 2020  utputs.max(),.  
+000111f0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00011200: 696e 223a 206f 7574 7075 7473 2e6d 696e  in": outputs.min
+00011210: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00011220: 2020 2020 2273 7464 6465 7622 3a20 6f75      "stddev": ou
+00011230: 7470 7574 732e 7374 6428 292c 0a20 2020  tputs.std(),.   
+00011240: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00011250: 676d 656e 7473 223a 2073 6567 6d65 6e74  gments": segment
+00011260: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00011270: 2020 2022 636f 756e 7422 3a20 746f 7461     "count": tota
+00011280: 6c5f 6f75 7470 7574 2c0a 2020 2020 2020  l_output,.      
+00011290: 2020 2020 2020 2020 2020 2274 6f74 616c            "total
+000112a0: 223a 2074 6f74 616c 2c0a 2020 2020 2020  ": total,.      
+000112b0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000112c0: 2020 2020 2022 6661 7374 6572 223a 2022       "faster": "
+000112d0: 626f 7468 2220 6966 2074 6f74 616c 5f69  both" if total_i
+000112e0: 6e70 7574 203d 3d20 746f 7461 6c5f 6f75  nput == total_ou
+000112f0: 7470 7574 2065 6c73 6520 280a 2020 2020  tput else (.    
+00011300: 2020 2020 2020 2020 2020 2020 2269 6e70              "inp
+00011310: 7574 2220 6966 2074 6f74 616c 5f69 6e70  ut" if total_inp
+00011320: 7574 203e 2074 6f74 616c 5f6f 7574 7075  ut > total_outpu
+00011330: 7420 656c 7365 2022 6f75 7470 7574 2229  t else "output")
+00011340: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00011350: 7272 6f72 7322 3a20 6572 726f 7273 2c0a  rrors": errors,.
+00011360: 2020 2020 2020 2020 2020 2020 2265 7272              "err
+00011370: 6f72 5f6d 7367 7322 3a20 6572 726f 725f  or_msgs": error_
+00011380: 6d73 6773 2c0a 2020 2020 2020 2020 7d0a  msgs,.        }.
+00011390: 0a20 2020 2064 6566 2067 6574 5f6b 6166  .    def get_kaf
+000113a0: 6b61 5f67 726f 7570 2873 656c 6629 202d  ka_group(self) -
+000113b0: 3e20 4b61 666b 6147 726f 7570 3a0a 2020  > KafkaGroup:.  
+000113c0: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+000113d0: 7428 4b61 666b 6147 726f 7570 2c20 7365  t(KafkaGroup, se
+000113e0: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
+000113f0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
+00011400: 2020 2020 204d 4554 484f 445f 4745 542c       METHOD_GET,
+00011410: 2022 2f6b 6166 6b61 5f67 726f 7570 222c   "/kafka_group",
+00011420: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00011430: 2020 2022 6461 6722 3a20 7365 6c66 2e67     "dag": self.g
+00011440: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
+00011450: 2020 2020 2020 7d29 290a 0a20 2020 2064        }))..    d
+00011460: 6566 2073 6574 5f6b 6166 6b61 5f67 726f  ef set_kafka_gro
+00011470: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+00011480: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00011490: 2020 6772 6f75 705f 6964 3a20 4f70 7469    group_id: Opti
+000114a0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000114b0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+000114c0: 7365 743a 204f 7074 696f 6e61 6c5b 7374  set: Optional[st
+000114d0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000114e0: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+000114f0: 2041 6e79 2920 2d3e 204b 6166 6b61 4772   Any) -> KafkaGr
+00011500: 6f75 703a 0a20 2020 2020 2020 2072 6574  oup:.        ret
+00011510: 7572 6e20 6361 7374 284b 6166 6b61 4772  urn cast(KafkaGr
+00011520: 6f75 702c 2073 656c 662e 5f63 6c69 656e  oup, self._clien
+00011530: 742e 7265 7175 6573 745f 6a73 6f6e 280a  t.request_json(.
+00011540: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00011550: 4f44 5f50 5554 2c20 222f 6b61 666b 615f  OD_PUT, "/kafka_
+00011560: 6772 6f75 7022 2c20 7b0a 2020 2020 2020  group", {.      
+00011570: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
+00011580: 2073 656c 662e 6765 745f 7572 6928 292c   self.get_uri(),
+00011590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000115a0: 2022 6772 6f75 705f 6964 223a 2067 726f   "group_id": gro
+000115b0: 7570 5f69 642c 0a20 2020 2020 2020 2020  up_id,.         
+000115c0: 2020 2020 2020 2022 7265 7365 7422 3a20         "reset": 
+000115d0: 7265 7365 742c 0a20 2020 2020 2020 2020  reset,.         
+000115e0: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+000115f0: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
+00011600: 0a0a 2020 2020 6465 6620 6465 6c65 7465  ..    def delete
+00011610: 2873 656c 6629 202d 3e20 4465 6c65 7465  (self) -> Delete
+00011620: 426c 6f62 5265 7370 6f6e 7365 3a0a 2020  BlobResponse:.  
+00011630: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00011640: 7428 4465 6c65 7465 426c 6f62 5265 7370  t(DeleteBlobResp
+00011650: 6f6e 7365 2c20 7365 6c66 2e5f 636c 6965  onse, self._clie
+00011660: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
+00011670: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+00011680: 484f 445f 4445 4c45 5445 2c20 222f 626c  HOD_DELETE, "/bl
+00011690: 6f62 222c 207b 0a20 2020 2020 2020 2020  ob", {.         
+000116a0: 2020 2020 2020 2022 626c 6f62 5f75 7269         "blob_uri
+000116b0: 7322 3a20 5b73 656c 662e 6765 745f 7572  s": [self.get_ur
+000116c0: 6928 295d 2c0a 2020 2020 2020 2020 2020  i()],.          
+000116d0: 2020 7d2c 0a20 2020 2020 2020 2029 290a    },.        )).
+000116e0: 0a20 2020 2064 6566 2064 6f77 6e6c 6f61  .    def downloa
+000116f0: 645f 6675 6c6c 5f64 6167 5f7a 6970 280a  d_full_dag_zip(.
+00011700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011710: 2c20 746f 5f70 6174 683a 204f 7074 696f  , to_path: Optio
+00011720: 6e61 6c5b 7374 725d 2920 2d3e 204f 7074  nal[str]) -> Opt
+00011730: 696f 6e61 6c5b 696f 2e42 7974 6573 494f  ional[io.BytesIO
+00011740: 5d3a 0a20 2020 2020 2020 2063 7572 5f72  ]:.        cur_r
+00011750: 6573 2c20 5f20 3d20 7365 6c66 2e5f 636c  es, _ = self._cl
+00011760: 6965 6e74 2e72 6571 7565 7374 5f62 7974  ient.request_byt
+00011770: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00011780: 4d45 5448 4f44 5f47 4554 2c20 222f 646f  METHOD_GET, "/do
+00011790: 776e 6c6f 6164 5f64 6167 5f7a 6970 222c  wnload_dag_zip",
+000117a0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000117b0: 2020 2022 6461 6722 3a20 7365 6c66 2e67     "dag": self.g
+000117c0: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
+000117d0: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
+000117e0: 2069 6620 746f 5f70 6174 6820 6973 204e   if to_path is N
+000117f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011800: 2072 6574 7572 6e20 696f 2e42 7974 6573   return io.Bytes
+00011810: 494f 2863 7572 5f72 6573 2e72 6561 6428  IO(cur_res.read(
+00011820: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00011830: 6f70 656e 2874 6f5f 7061 7468 2c20 2277  open(to_path, "w
+00011840: 6222 2920 6173 2066 696c 655f 646f 776e  b") as file_down
+00011850: 6c6f 6164 3a0a 2020 2020 2020 2020 2020  load:.          
+00011860: 2020 6669 6c65 5f64 6f77 6e6c 6f61 642e    file_download.
+00011870: 7772 6974 6528 6375 725f 7265 732e 7265  write(cur_res.re
+00011880: 6164 2829 290a 2020 2020 2020 2020 7265  ad()).        re
+00011890: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
+000118a0: 6566 205f 7570 6c6f 6164 5f64 6167 5f62  ef _upload_dag_b
+000118b0: 6c6f 6273 280a 2020 2020 2020 2020 2020  lobs(.          
+000118c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000118d0: 2020 2020 746d 7064 6972 3a20 7374 722c      tmpdir: str,
+000118e0: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
+000118f0: 6273 5f6d 6170 3a20 4c69 7374 5b42 6c6f  bs_map: List[Blo
+00011900: 6244 6574 6169 6c73 5d2c 0a20 2020 2020  bDetails],.     
+00011910: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
+00011920: 6473 3a20 696e 7429 202d 3e20 4c69 7374  ds: int) -> List
+00011930: 5b27 426c 6f62 4861 6e64 6c65 275d 3a0a  ['BlobHandle']:.
+00011940: 2020 2020 2020 2020 626c 6f62 5f68 616e          blob_han
+00011950: 646c 6573 203d 205b 5d0a 2020 2020 2020  dles = [].      
+00011960: 2020 666f 7220 626c 6f62 2069 6e20 626c    for blob in bl
+00011970: 6f62 735f 6d61 703a 0a20 2020 2020 2020  obs_map:.       
+00011980: 2020 2020 2062 6c6f 625f 6669 6c65 203d       blob_file =
+00011990: 206f 732e 7061 7468 2e6a 6f69 6e28 746d   os.path.join(tm
+000119a0: 7064 6972 2c20 626c 6f62 5b22 666e 616d  pdir, blob["fnam
+000119b0: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
+000119c0: 2062 6c6f 625f 6861 6e64 6c65 203d 2073   blob_handle = s
+000119d0: 656c 662e 5f63 6c69 656e 742e 6765 745f  elf._client.get_
+000119e0: 626c 6f62 5f68 616e 646c 6528 626c 6f62  blob_handle(blob
+000119f0: 5b22 626c 6f62 5f75 7269 225d 290a 2020  ["blob_uri"]).  
+00011a00: 2020 2020 2020 2020 2020 626c 6f62 5f68            blob_h
+00011a10: 616e 646c 6573 2e65 7874 656e 6428 626c  andles.extend(bl
+00011a20: 6f62 5f68 616e 646c 652e 7570 6c6f 6164  ob_handle.upload
+00011a30: 5f7a 6970 2862 6c6f 625f 6669 6c65 2c20  _zip(blob_file, 
+00011a40: 6d61 785f 7468 7265 6164 7329 290a 2020  max_threads)).  
+00011a50: 2020 2020 2020 7265 7475 726e 2062 6c6f        return blo
+00011a60: 625f 6861 6e64 6c65 730a 0a20 2020 2064  b_handles..    d
+00011a70: 6566 2075 706c 6f61 645f 6675 6c6c 5f64  ef upload_full_d
+00011a80: 6167 5f7a 6970 280a 2020 2020 2020 2020  ag_zip(.        
+00011a90: 2020 2020 7365 6c66 2c20 736f 7572 6365      self, source
+00011aa0: 3a20 7374 722c 206d 6178 5f74 6872 6561  : str, max_threa
+00011ab0: 6473 3a20 696e 7420 3d20 3130 2920 2d3e  ds: int = 10) ->
+00011ac0: 204c 6973 745b 2742 6c6f 6248 616e 646c   List['BlobHandl
+00011ad0: 6527 5d3a 0a20 2020 2020 2020 2064 6167  e']:.        dag
+00011ae0: 5f62 6c6f 625f 6861 6e64 6c65 203d 2073  _blob_handle = s
+00011af0: 656c 662e 5f63 6c69 656e 742e 6765 745f  elf._client.get_
+00011b00: 626c 6f62 5f68 616e 646c 6528 7365 6c66  blob_handle(self
+00011b10: 2e67 6574 5f75 7269 2829 290a 2020 2020  .get_uri()).    
+00011b20: 2020 2020 626c 6f62 5f68 616e 646c 6573      blob_handles
+00011b30: 203d 205b 5d0a 2020 2020 2020 2020 7769   = [].        wi
+00011b40: 7468 2074 656d 7066 696c 652e 5465 6d70  th tempfile.Temp
+00011b50: 6f72 6172 7944 6972 6563 746f 7279 2829  oraryDirectory()
+00011b60: 2061 7320 746d 7064 6972 3a0a 2020 2020   as tmpdir:.    
+00011b70: 2020 2020 2020 2020 7368 7574 696c 2e75          shutil.u
+00011b80: 6e70 6163 6b5f 6172 6368 6976 6528 736f  npack_archive(so
+00011b90: 7572 6365 2c20 746d 7064 6972 2c20 227a  urce, tmpdir, "z
+00011ba0: 6970 2229 0a20 2020 2020 2020 2020 2020  ip").           
+00011bb0: 2066 6d61 705f 6a73 6f6e 203d 206f 732e   fmap_json = os.
+00011bc0: 7061 7468 2e6a 6f69 6e28 746d 7064 6972  path.join(tmpdir
+00011bd0: 2c20 2266 696c 656d 6170 2e6a 736f 6e22  , "filemap.json"
+00011be0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+00011bf0: 7468 206f 7065 6e28 666d 6170 5f6a 736f  th open(fmap_jso
+00011c00: 6e2c 2022 7222 2920 6173 2066 6d61 703a  n, "r") as fmap:
+00011c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c20: 2066 696c 655f 6d61 703a 2046 696c 654d   file_map: FileM
+00011c30: 6170 203d 206a 736f 6e2e 6c6f 6164 2866  ap = json.load(f
+00011c40: 6d61 7029 0a20 2020 2020 2020 2020 2020  map).           
+00011c50: 2064 6167 5f66 6e61 6d65 203d 2066 696c   dag_fname = fil
+00011c60: 655f 6d61 705b 2264 6167 5f62 6c6f 6222  e_map["dag_blob"
+00011c70: 5d0a 2020 2020 2020 2020 2020 2020 6461  ].            da
+00011c80: 675f 6669 6c65 203d 206f 732e 7061 7468  g_file = os.path
+00011c90: 2e6a 6f69 6e28 746d 7064 6972 2c20 6622  .join(tmpdir, f"
+00011ca0: 7b64 6167 5f66 6e61 6d65 7d22 290a 2020  {dag_fname}").  
+00011cb0: 2020 2020 2020 2020 2020 626c 6f62 5f68            blob_h
+00011cc0: 616e 646c 6573 2e65 7874 656e 6428 0a20  andles.extend(. 
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00011ce0: 6167 5f62 6c6f 625f 6861 6e64 6c65 2e75  ag_blob_handle.u
+00011cf0: 706c 6f61 645f 7a69 7028 6461 675f 6669  pload_zip(dag_fi
+00011d00: 6c65 2c20 6d61 785f 7468 7265 6164 7329  le, max_threads)
+00011d10: 290a 2020 2020 2020 2020 2020 2020 626c  ).            bl
+00011d20: 6f62 5f68 616e 646c 6573 2e65 7874 656e  ob_handles.exten
+00011d30: 6428 7365 6c66 2e5f 7570 6c6f 6164 5f64  d(self._upload_d
+00011d40: 6167 5f62 6c6f 6273 280a 2020 2020 2020  ag_blobs(.      
+00011d50: 2020 2020 2020 2020 2020 746d 7064 6972            tmpdir
+00011d60: 2c20 6669 6c65 5f6d 6170 5b22 626c 6f62  , file_map["blob
+00011d70: 7322 5d2c 206d 6178 5f74 6872 6561 6473  s"], max_threads
+00011d80: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+00011d90: 6e20 626c 6f62 5f68 616e 646c 6573 0a0a  n blob_handles..
+00011da0: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
+00011db0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00011dc0: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+00011dd0: 7368 2873 656c 662e 6765 745f 7572 6928  sh(self.get_uri(
+00011de0: 2929 0a0a 2020 2020 6465 6620 5f5f 6571  ))..    def __eq
+00011df0: 5f5f 2873 656c 662c 206f 7468 6572 3a20  __(self, other: 
+00011e00: 6f62 6a65 6374 2920 2d3e 2062 6f6f 6c3a  object) -> bool:
+00011e10: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00011e20: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+00011e30: 2c20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  , self.__class__
+00011e40: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00011e50: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00011e60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00011e70: 6765 745f 7572 6928 2920 3d3d 206f 7468  get_uri() == oth
+00011e80: 6572 2e67 6574 5f75 7269 2829 0a0a 2020  er.get_uri()..  
+00011e90: 2020 6465 6620 5f5f 6e65 5f5f 2873 656c    def __ne__(sel
+00011ea0: 662c 206f 7468 6572 3a20 6f62 6a65 6374  f, other: object
+00011eb0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00011ec0: 2020 2072 6574 7572 6e20 6e6f 7420 7365     return not se
+00011ed0: 6c66 2e5f 5f65 715f 5f28 6f74 6865 7229  lf.__eq__(other)
+00011ee0: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00011ef0: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
+00011f00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011f10: 656c 662e 6765 745f 7572 6928 290a 0a20  elf.get_uri().. 
+00011f20: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+00011f30: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+00011f40: 2020 2020 2020 7265 7475 726e 2066 227b        return f"{
+00011f50: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
+00011f60: 5f6e 616d 655f 5f7d 5b7b 7365 6c66 2e67  _name__}[{self.g
+00011f70: 6574 5f75 7269 2829 7d5d 220a 0a23 202a  et_uri()}]"..# *
+00011f80: 2a2a 2044 6167 4861 6e64 6c65 202a 2a2a  ** DagHandle ***
+00011f90: 0a0a 0a63 6c61 7373 204e 6f64 6548 616e  ...class NodeHan
+00011fa0: 646c 653a 0a20 2020 2064 6566 205f 5f69  dle:.    def __i
+00011fb0: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
+00011fc0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00011fd0: 2020 2020 2063 6c69 656e 743a 2058 594d       client: XYM
+00011fe0: 4543 6c69 656e 742c 0a20 2020 2020 2020  EClient,.       
+00011ff0: 2020 2020 2064 6167 3a20 4461 6748 616e       dag: DagHan
+00012000: 646c 652c 0a20 2020 2020 2020 2020 2020  dle,.           
+00012010: 206e 6f64 655f 6964 3a20 7374 722c 0a20   node_id: str,. 
+00012020: 2020 2020 2020 2020 2020 206e 6f64 655f             node_
+00012030: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+00012040: 2020 2020 2020 206b 696e 643a 2073 7472         kind: str
+00012050: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012060: 2020 2073 656c 662e 5f63 6c69 656e 7420     self._client 
+00012070: 3d20 636c 6965 6e74 0a20 2020 2020 2020  = client.       
+00012080: 2073 656c 662e 5f64 6167 203d 2064 6167   self._dag = dag
+00012090: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
+000120a0: 6f64 655f 6964 203d 206e 6f64 655f 6964  ode_id = node_id
+000120b0: 0a20 2020 2020 2020 2073 656c 662e 5f6e  .        self._n
+000120c0: 6f64 655f 6e61 6d65 203d 206e 6f64 655f  ode_name = node_
+000120d0: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+000120e0: 662e 5f74 7970 6520 3d20 6b69 6e64 0a20  f._type = kind. 
+000120f0: 2020 2020 2020 2073 656c 662e 5f62 6c6f         self._blo
+00012100: 6273 3a20 4469 6374 5b73 7472 2c20 426c  bs: Dict[str, Bl
+00012110: 6f62 4861 6e64 6c65 5d20 3d20 7b7d 0a20  obHandle] = {}. 
+00012120: 2020 2020 2020 2073 656c 662e 5f69 6e70         self._inp
+00012130: 7574 733a 2044 6963 745b 7374 722c 2054  uts: Dict[str, T
+00012140: 7570 6c65 5b73 7472 2c20 7374 725d 5d20  uple[str, str]] 
+00012150: 3d20 7b7d 0a20 2020 2020 2020 2073 656c  = {}.        sel
+00012160: 662e 5f73 7461 7465 3a20 4f70 7469 6f6e  f._state: Option
+00012170: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a20  al[int] = None. 
+00012180: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+00012190: 6669 675f 6572 726f 723a 204f 7074 696f  fig_error: Optio
+000121a0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000121b0: 2020 2020 2020 2020 7365 6c66 2e5f 6973          self._is
+000121c0: 5f6d 6f64 656c 3a20 4f70 7469 6f6e 616c  _model: Optional
+000121d0: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 2020  [bool] = None.  
+000121e0: 2020 2020 2020 7365 6c66 2e5f 7665 7273        self._vers
+000121f0: 696f 6e5f 6f76 6572 7269 6465 3a20 4f70  ion_override: Op
+00012200: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00012210: 6e65 0a0a 2020 2020 6465 6620 6173 5f6f  ne..    def as_o
+00012220: 776e 6572 2873 656c 6629 202d 3e20 426c  wner(self) -> Bl
+00012230: 6f62 4f77 6e65 723a 0a20 2020 2020 2020  obOwner:.       
+00012240: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
+00012250: 2020 2020 2020 226f 776e 6572 5f64 6167        "owner_dag
+00012260: 223a 2073 656c 662e 6765 745f 6461 6728  ": self.get_dag(
+00012270: 292e 6765 745f 7572 6928 292c 0a20 2020  ).get_uri(),.   
+00012280: 2020 2020 2020 2020 2022 6f77 6e65 725f           "owner_
+00012290: 6e6f 6465 223a 2073 656c 662e 6765 745f  node": self.get_
+000122a0: 6964 2829 2c0a 2020 2020 2020 2020 7d0a  id(),.        }.
+000122b0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+000122c0: 6f64 0a20 2020 2064 6566 2066 726f 6d5f  od.    def from_
+000122d0: 6e6f 6465 5f69 6e66 6f28 0a20 2020 2020  node_info(.     
+000122e0: 2020 2020 2020 2063 6c69 656e 743a 2058         client: X
+000122f0: 594d 4543 6c69 656e 742c 0a20 2020 2020  YMEClient,.     
+00012300: 2020 2020 2020 2064 6167 3a20 4461 6748         dag: DagH
+00012310: 616e 646c 652c 0a20 2020 2020 2020 2020  andle,.         
+00012320: 2020 206e 6f64 655f 696e 666f 3a20 4e6f     node_info: No
+00012330: 6465 496e 666f 2c0a 2020 2020 2020 2020  deInfo,.        
+00012340: 2020 2020 7072 6576 3a20 4f70 7469 6f6e      prev: Option
+00012350: 616c 5b27 4e6f 6465 4861 6e64 6c65 275d  al['NodeHandle']
+00012360: 2920 2d3e 2027 4e6f 6465 4861 6e64 6c65  ) -> 'NodeHandle
+00012370: 273a 0a20 2020 2020 2020 2069 6620 7072  ':.        if pr
+00012380: 6576 2069 7320 4e6f 6e65 3a0a 2020 2020  ev is None:.    
+00012390: 2020 2020 2020 2020 7265 7320 3d20 4e6f          res = No
+000123a0: 6465 4861 6e64 6c65 280a 2020 2020 2020  deHandle(.      
+000123b0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000123c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000123d0: 2020 6461 672c 0a20 2020 2020 2020 2020    dag,.         
+000123e0: 2020 2020 2020 206e 6f64 655f 696e 666f         node_info
+000123f0: 5b22 6964 225d 2c0a 2020 2020 2020 2020  ["id"],.        
+00012400: 2020 2020 2020 2020 6e6f 6465 5f69 6e66          node_inf
+00012410: 6f5b 226e 616d 6522 5d2c 0a20 2020 2020  o["name"],.     
+00012420: 2020 2020 2020 2020 2020 206e 6f64 655f             node_
+00012430: 696e 666f 5b22 7479 7065 225d 290a 2020  info["type"]).  
+00012440: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012450: 2020 2020 2020 2020 6966 2070 7265 762e          if prev.
+00012460: 6765 745f 6461 6728 2920 213d 2064 6167  get_dag() != dag
+00012470: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012480: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00012490: 6f72 2866 227b 7072 6576 2e67 6574 5f64  or(f"{prev.get_d
+000124a0: 6167 2829 7d20 213d 207b 6461 677d 2229  ag()} != {dag}")
+000124b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000124c0: 203d 2070 7265 760a 2020 2020 2020 2020   = prev.        
+000124d0: 7265 732e 7570 6461 7465 5f69 6e66 6f28  res.update_info(
+000124e0: 6e6f 6465 5f69 6e66 6f29 0a20 2020 2020  node_info).     
+000124f0: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
+00012500: 2020 2064 6566 2075 7064 6174 655f 696e     def update_in
+00012510: 666f 2873 656c 662c 206e 6f64 655f 696e  fo(self, node_in
+00012520: 666f 3a20 4e6f 6465 496e 666f 2920 2d3e  fo: NodeInfo) ->
+00012530: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+00012540: 6620 7365 6c66 2e67 6574 5f69 6428 2920  f self.get_id() 
+00012550: 213d 206e 6f64 655f 696e 666f 5b22 6964  != node_info["id
+00012560: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00012570: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00012580: 2866 227b 7365 6c66 2e5f 6e6f 6465 5f69  (f"{self._node_i
+00012590: 647d 2021 3d20 7b6e 6f64 655f 696e 666f  d} != {node_info
+000125a0: 5b27 6964 275d 7d22 290a 2020 2020 2020  ['id']}").      
+000125b0: 2020 7365 6c66 2e5f 6e6f 6465 5f6e 616d    self._node_nam
+000125c0: 6520 3d20 6e6f 6465 5f69 6e66 6f5b 226e  e = node_info["n
+000125d0: 616d 6522 5d0a 2020 2020 2020 2020 7365  ame"].        se
+000125e0: 6c66 2e5f 7479 7065 203d 206e 6f64 655f  lf._type = node_
+000125f0: 696e 666f 5b22 7479 7065 225d 0a20 2020  info["type"].   
+00012600: 2020 2020 2073 656c 662e 5f62 6c6f 6273       self._blobs
+00012610: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00012620: 206b 6579 3a20 426c 6f62 4861 6e64 6c65   key: BlobHandle
+00012630: 2873 656c 662e 5f63 6c69 656e 742c 2076  (self._client, v
+00012640: 616c 7565 2c20 6973 5f66 756c 6c3d 4661  alue, is_full=Fa
+00012650: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00012660: 2066 6f72 2028 6b65 792c 2076 616c 7565   for (key, value
+00012670: 2920 696e 206e 6f64 655f 696e 666f 5b22  ) in node_info["
+00012680: 626c 6f62 7322 5d2e 6974 656d 7328 290a  blobs"].items().
+00012690: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000126a0: 2020 7365 6c66 2e5f 696e 7075 7473 203d    self._inputs =
+000126b0: 206e 6f64 655f 696e 666f 5b22 696e 7075   node_info["inpu
+000126c0: 7473 225d 0a20 2020 2020 2020 2073 656c  ts"].        sel
+000126d0: 662e 5f73 7461 7465 203d 206e 6f64 655f  f._state = node_
+000126e0: 696e 666f 5b22 7374 6174 6522 5d0a 2020  info["state"].  
+000126f0: 2020 2020 2020 7365 6c66 2e5f 636f 6e66        self._conf
+00012700: 6967 5f65 7272 6f72 203d 206e 6f64 655f  ig_error = node_
+00012710: 696e 666f 5b22 636f 6e66 6967 5f65 7272  info["config_err
+00012720: 6f72 225d 0a20 2020 2020 2020 2073 656c  or"].        sel
+00012730: 662e 5f76 6572 7369 6f6e 5f6f 7665 7272  f._version_overr
+00012740: 6964 6520 3d20 6e6f 6465 5f69 6e66 6f5b  ide = node_info[
+00012750: 2276 6572 7369 6f6e 5f6f 7665 7272 6964  "version_overrid
+00012760: 6522 5d0a 0a20 2020 2064 6566 2067 6574  e"]..    def get
+00012770: 5f64 6167 2873 656c 6629 202d 3e20 4461  _dag(self) -> Da
+00012780: 6748 616e 646c 653a 0a20 2020 2020 2020  gHandle:.       
+00012790: 2072 6574 7572 6e20 7365 6c66 2e5f 6461   return self._da
+000127a0: 670a 0a20 2020 2064 6566 2067 6574 5f69  g..    def get_i
+000127b0: 6428 7365 6c66 2920 2d3e 2073 7472 3a0a  d(self) -> str:.
+000127c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000127d0: 656c 662e 5f6e 6f64 655f 6964 0a0a 2020  elf._node_id..  
+000127e0: 2020 6465 6620 6765 745f 6e61 6d65 2873    def get_name(s
+000127f0: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+00012800: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012810: 2e5f 6e6f 6465 5f6e 616d 650a 0a20 2020  ._node_name..   
+00012820: 2064 6566 2067 6574 5f74 7970 6528 7365   def get_type(se
+00012830: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+00012840: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00012850: 5f74 7970 650a 0a20 2020 2064 6566 2067  _type..    def g
+00012860: 6574 5f6e 6f64 655f 6465 6628 7365 6c66  et_node_def(self
+00012870: 2920 2d3e 204e 6f64 6544 6566 496e 666f  ) -> NodeDefInfo
+00012880: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00012890: 2073 656c 662e 5f63 6c69 656e 742e 6765   self._client.ge
+000128a0: 745f 6e6f 6465 5f64 6566 7328 295b 7365  t_node_defs()[se
+000128b0: 6c66 2e67 6574 5f74 7970 6528 295d 0a0a  lf.get_type()]..
+000128c0: 2020 2020 6465 6620 6765 745f 696e 7075      def get_inpu
+000128d0: 7473 2873 656c 6629 202d 3e20 5365 745b  ts(self) -> Set[
+000128e0: 7374 725d 3a0a 2020 2020 2020 2020 7265  str]:.        re
+000128f0: 7475 726e 2073 6574 2873 656c 662e 5f69  turn set(self._i
+00012900: 6e70 7574 732e 6b65 7973 2829 290a 0a20  nputs.keys()).. 
+00012910: 2020 2064 6566 2067 6574 5f69 6e70 7574     def get_input
+00012920: 2873 656c 662c 206b 6579 3a20 7374 7229  (self, key: str)
+00012930: 202d 3e20 5475 706c 655b 274e 6f64 6548   -> Tuple['NodeH
+00012940: 616e 646c 6527 2c20 7374 725d 3a0a 2020  andle', str]:.  
+00012950: 2020 2020 2020 6e6f 6465 5f69 642c 206f        node_id, o
+00012960: 7574 5f6b 6579 203d 2073 656c 662e 5f69  ut_key = self._i
+00012970: 6e70 7574 735b 6b65 795d 0a20 2020 2020  nputs[key].     
+00012980: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
+00012990: 6574 5f64 6167 2829 2e67 6574 5f6e 6f64  et_dag().get_nod
+000129a0: 6528 6e6f 6465 5f69 6429 2c20 6f75 745f  e(node_id), out_
+000129b0: 6b65 790a 0a20 2020 2064 6566 2067 6574  key..    def get
+000129c0: 5f73 7461 7475 7328 7365 6c66 2920 2d3e  _status(self) ->
+000129d0: 2054 6173 6b53 7461 7475 733a 0a20 2020   TaskStatus:.   
+000129e0: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
+000129f0: 284e 6f64 6553 7461 7475 732c 2073 656c  (NodeStatus, sel
+00012a00: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+00012a10: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+00012a20: 2020 2020 4d45 5448 4f44 5f47 4554 2c20      METHOD_GET, 
+00012a30: 222f 6e6f 6465 5f73 7461 7475 7322 2c20  "/node_status", 
+00012a40: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00012a50: 2020 2264 6167 223a 2073 656c 662e 6765    "dag": self.ge
+00012a60: 745f 6461 6728 292e 6765 745f 7572 6928  t_dag().get_uri(
+00012a70: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00012a80: 2020 2022 6e6f 6465 223a 2073 656c 662e     "node": self.
+00012a90: 6765 745f 6964 2829 2c0a 2020 2020 2020  get_id(),.      
+00012aa0: 2020 2020 2020 7d29 295b 2273 7461 7475        }))["statu
+00012ab0: 7322 5d0a 0a20 2020 2064 6566 2068 6173  s"]..    def has
+00012ac0: 5f63 6f6e 6669 675f 6572 726f 7228 7365  _config_error(se
+00012ad0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00012ae0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012af0: 2e5f 636f 6e66 6967 5f65 7272 6f72 2069  ._config_error i
+00012b00: 7320 6e6f 7420 4e6f 6e65 0a0a 2020 2020  s not None..    
+00012b10: 6465 6620 6765 745f 636f 6e66 6967 5f65  def get_config_e
+00012b20: 7272 6f72 2873 656c 6629 202d 3e20 4f70  rror(self) -> Op
+00012b30: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
+00012b40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012b50: 2e5f 636f 6e66 6967 5f65 7272 6f72 0a0a  ._config_error..
+00012b60: 2020 2020 6465 6620 6765 745f 7665 7273      def get_vers
+00012b70: 696f 6e5f 6f76 6572 7269 6465 2873 656c  ion_override(sel
+00012b80: 6629 202d 3e20 4f70 7469 6f6e 616c 5b73  f) -> Optional[s
+00012b90: 7472 5d3a 0a20 2020 2020 2020 2072 6574  tr]:.        ret
+00012ba0: 7572 6e20 7365 6c66 2e5f 7665 7273 696f  urn self._versio
+00012bb0: 6e5f 6f76 6572 7269 6465 0a0a 2020 2020  n_override..    
+00012bc0: 6465 6620 6765 745f 626c 6f62 7328 7365  def get_blobs(se
+00012bd0: 6c66 2920 2d3e 204c 6973 745b 7374 725d  lf) -> List[str]
+00012be0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00012bf0: 2073 6f72 7465 6428 7365 6c66 2e5f 626c   sorted(self._bl
+00012c00: 6f62 732e 6b65 7973 2829 290a 0a20 2020  obs.keys())..   
+00012c10: 2064 6566 2067 6574 5f62 6c6f 625f 6861   def get_blob_ha
+00012c20: 6e64 6c65 7328 7365 6c66 2920 2d3e 2044  ndles(self) -> D
+00012c30: 6963 745b 7374 722c 2027 426c 6f62 4861  ict[str, 'BlobHa
+00012c40: 6e64 6c65 275d 3a0a 2020 2020 2020 2020  ndle']:.        
+00012c50: 7265 7475 726e 2073 656c 662e 5f62 6c6f  return self._blo
+00012c60: 6273 0a0a 2020 2020 6465 6620 6765 745f  bs..    def get_
+00012c70: 626c 6f62 5f68 616e 646c 6528 7365 6c66  blob_handle(self
+00012c80: 2c20 6b65 793a 2073 7472 2920 2d3e 2027  , key: str) -> '
+00012c90: 426c 6f62 4861 6e64 6c65 273a 0a20 2020  BlobHandle':.   
+00012ca0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012cb0: 2e5f 626c 6f62 735b 6b65 795d 0a0a 2020  ._blobs[key]..  
+00012cc0: 2020 6465 6620 7365 745f 626c 6f62 5f75    def set_blob_u
+00012cd0: 7269 2873 656c 662c 206b 6579 3a20 7374  ri(self, key: st
+00012ce0: 722c 2062 6c6f 625f 7572 693a 2073 7472  r, blob_uri: str
+00012cf0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00012d00: 2020 7265 7475 726e 2063 6173 7428 5075    return cast(Pu
+00012d10: 744e 6f64 6542 6c6f 622c 2073 656c 662e  tNodeBlob, self.
+00012d20: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
+00012d30: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
+00012d40: 2020 4d45 5448 4f44 5f50 5554 2c20 222f    METHOD_PUT, "/
+00012d50: 6e6f 6465 5f62 6c6f 6222 2c20 7b0a 2020  node_blob", {.  
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00012d70: 6167 223a 2073 656c 662e 6765 745f 6461  ag": self.get_da
+00012d80: 6728 292e 6765 745f 7572 6928 292c 0a20  g().get_uri(),. 
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012da0: 6e6f 6465 223a 2073 656c 662e 6765 745f  node": self.get_
+00012db0: 6964 2829 2c0a 2020 2020 2020 2020 2020  id(),.          
+00012dc0: 2020 2020 2020 2262 6c6f 625f 6b65 7922        "blob_key"
+00012dd0: 3a20 6b65 792c 0a20 2020 2020 2020 2020  : key,.         
+00012de0: 2020 2020 2020 2022 626c 6f62 5f75 7269         "blob_uri
+00012df0: 223a 2062 6c6f 625f 7572 692c 0a20 2020  ": blob_uri,.   
+00012e00: 2020 2020 2020 2020 207d 2929 5b22 6e65           }))["ne
+00012e10: 775f 7572 6922 5d0a 0a20 2020 2064 6566  w_uri"]..    def
+00012e20: 2067 6574 5f69 6e5f 6375 7273 6f72 5f73   get_in_cursor_s
+00012e30: 7461 7465 7328 7365 6c66 2920 2d3e 2044  tates(self) -> D
+00012e40: 6963 745b 7374 722c 2069 6e74 5d3a 0a20  ict[str, int]:. 
+00012e50: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
+00012e60: 7374 2849 6e43 7572 736f 7273 2c20 7365  st(InCursors, se
+00012e70: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
+00012e80: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
+00012e90: 2020 2020 204d 4554 484f 445f 4745 542c       METHOD_GET,
+00012ea0: 2022 2f6e 6f64 655f 696e 5f63 7572 736f   "/node_in_curso
+00012eb0: 7273 222c 207b 0a20 2020 2020 2020 2020  rs", {.         
+00012ec0: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
+00012ed0: 6c66 2e67 6574 5f64 6167 2829 2e67 6574  lf.get_dag().get
+00012ee0: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
+00012ef0: 2020 2020 2020 2020 226e 6f64 6522 3a20          "node": 
+00012f00: 7365 6c66 2e67 6574 5f69 6428 292c 0a20  self.get_id(),. 
+00012f10: 2020 2020 2020 2020 2020 207d 2929 5b22             }))["
+00012f20: 6375 7273 6f72 7322 5d0a 0a20 2020 2064  cursors"]..    d
+00012f30: 6566 2067 6574 5f68 6967 6865 7374 5f63  ef get_highest_c
+00012f40: 6875 6e6b 2873 656c 6629 202d 3e20 696e  hunk(self) -> in
+00012f50: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+00012f60: 6e20 6361 7374 284e 6f64 6543 6875 6e6b  n cast(NodeChunk
+00012f70: 2c20 7365 6c66 2e5f 636c 6965 6e74 2e72  , self._client.r
+00012f80: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
+00012f90: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+00012fa0: 4745 542c 2022 2f6e 6f64 655f 6368 756e  GET, "/node_chun
+00012fb0: 6b22 2c20 7b0a 2020 2020 2020 2020 2020  k", {.          
+00012fc0: 2020 2020 2020 2264 6167 223a 2073 656c        "dag": sel
+00012fd0: 662e 6765 745f 6461 6728 292e 6765 745f  f.get_dag().get_
+00012fe0: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
+00012ff0: 2020 2020 2020 2022 6e6f 6465 223a 2073         "node": s
+00013000: 656c 662e 6765 745f 6964 2829 2c0a 2020  elf.get_id(),.  
+00013010: 2020 2020 2020 2020 2020 7d29 295b 2263            }))["c
+00013020: 6875 6e6b 225d 0a0a 2020 2020 6465 6620  hunk"]..    def 
+00013030: 6765 745f 7368 6f72 745f 7374 6174 7573  get_short_status
+00013040: 2873 656c 662c 2061 6c6c 6f77 5f75 6e69  (self, allow_uni
+00013050: 636f 6465 3a20 626f 6f6c 203d 2054 7275  code: bool = Tru
+00013060: 6529 202d 3e20 7374 723a 0a20 2020 2020  e) -> str:.     
+00013070: 2020 2073 7461 7475 735f 6d61 703a 2044     status_map: D
+00013080: 6963 745b 5461 736b 5374 6174 7573 2c20  ict[TaskStatus, 
+00013090: 7374 725d 203d 207b 0a20 2020 2020 2020  str] = {.       
+000130a0: 2020 2020 2022 626c 6f63 6b65 6422 3a20       "blocked": 
+000130b0: 2242 222c 0a20 2020 2020 2020 2020 2020  "B",.           
+000130c0: 2022 7761 6974 696e 6722 3a20 2257 222c   "waiting": "W",
+000130d0: 0a20 2020 2020 2020 2020 2020 2022 7275  .            "ru
+000130e0: 6e6e 696e 6722 3a20 22e2 8692 2220 6966  nning": "..." if
+000130f0: 2061 6c6c 6f77 5f75 6e69 636f 6465 2065   allow_unicode e
+00013100: 6c73 6520 2252 222c 0a20 2020 2020 2020  lse "R",.       
+00013110: 2020 2020 2022 636f 6d70 6c65 7465 223a       "complete":
+00013120: 2022 e29c 9322 2069 6620 616c 6c6f 775f   "..." if allow_
+00013130: 756e 6963 6f64 6520 656c 7365 2022 4322  unicode else "C"
+00013140: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00013150: 6f73 223a 2022 5822 2c0a 2020 2020 2020  os": "X",.      
+00013160: 2020 2020 2020 2270 6175 7365 6422 3a20        "paused": 
+00013170: 2250 222c 0a20 2020 2020 2020 2020 2020  "P",.           
+00013180: 2022 6572 726f 7222 3a20 2221 222c 0a20   "error": "!",. 
+00013190: 2020 2020 2020 2020 2020 2022 756e 6b6e             "unkn
+000131a0: 6f77 6e22 3a20 223f 222c 0a20 2020 2020  own": "?",.     
+000131b0: 2020 2020 2020 2022 7669 7274 7561 6c22         "virtual"
+000131c0: 3a20 22e2 88b4 2220 6966 2061 6c6c 6f77  : "..." if allow
+000131d0: 5f75 6e69 636f 6465 2065 6c73 6520 2256  _unicode else "V
+000131e0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000131f0: 7175 6575 6522 3a20 223d 222c 0a20 2020  queue": "=",.   
+00013200: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
+00013210: 6574 7572 6e20 7374 6174 7573 5f6d 6170  eturn status_map
+00013220: 5b73 656c 662e 6765 745f 7374 6174 7573  [self.get_status
+00013230: 2829 5d0a 0a20 2020 2064 6566 2067 6574  ()]..    def get
+00013240: 5f6c 6f67 7328 7365 6c66 2920 2d3e 2073  _logs(self) -> s
+00013250: 7472 3a0a 2020 2020 2020 2020 7769 7468  tr:.        with
+00013260: 2073 656c 662e 5f63 6c69 656e 742e 5f72   self._client._r
+00013270: 6177 5f72 6571 7565 7374 5f73 7472 280a  aw_request_str(.
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013290: 4d45 5448 4f44 5f47 4554 2c20 222f 6e6f  METHOD_GET, "/no
+000132a0: 6465 5f6c 6f67 7322 2c20 7b0a 2020 2020  de_logs", {.    
+000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132c0: 2264 6167 223a 2073 656c 662e 6765 745f  "dag": self.get_
+000132d0: 6461 6728 292e 6765 745f 7572 6928 292c  dag().get_uri(),
+000132e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132f0: 2020 2020 2022 6e6f 6465 223a 2073 656c       "node": sel
+00013300: 662e 6765 745f 6964 2829 2c0a 2020 2020  f.get_id(),.    
+00013310: 2020 2020 2020 2020 2020 2020 7d29 2061              }) a
+00013320: 7320 6669 6e3a 0a20 2020 2020 2020 2020  s fin:.         
+00013330: 2020 2072 6574 7572 6e20 6669 6e2e 7265     return fin.re
+00013340: 6164 2829 0a0a 2020 2020 6465 6620 6765  ad()..    def ge
+00013350: 745f 7469 6d69 6e67 2873 656c 6629 202d  t_timing(self) -
+00013360: 3e20 4c69 7374 5b54 696d 696e 675d 3a0a  > List[Timing]:.
+00013370: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00013380: 6173 7428 5469 6d69 6e67 732c 2073 656c  ast(Timings, sel
+00013390: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+000133a0: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+000133b0: 2020 2020 4d45 5448 4f44 5f47 4554 2c20      METHOD_GET, 
+000133c0: 222f 6e6f 6465 5f70 6572 6622 2c20 7b0a  "/node_perf", {.
+000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133e0: 2264 6167 223a 2073 656c 662e 6765 745f  "dag": self.get_
+000133f0: 6461 6728 292e 6765 745f 7572 6928 292c  dag().get_uri(),
+00013400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013410: 2022 6e6f 6465 223a 2073 656c 662e 6765   "node": self.ge
+00013420: 745f 6964 2829 2c0a 2020 2020 2020 2020  t_id(),.        
+00013430: 2020 2020 7d29 295b 2274 696d 6573 225d      }))["times"]
+00013440: 0a0a 2020 2020 6465 6620 7265 6164 5f62  ..    def read_b
+00013450: 6c6f 6228 0a20 2020 2020 2020 2020 2020  lob(.           
+00013460: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00013470: 2020 206b 6579 3a20 7374 722c 0a20 2020     key: str,.   
+00013480: 2020 2020 2020 2020 2063 6875 6e6b 3a20           chunk: 
+00013490: 4f70 7469 6f6e 616c 5b69 6e74 5d2c 0a20  Optional[int],. 
+000134a0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+000134b0: 5f72 6566 7265 7368 3a20 626f 6f6c 2920  _refresh: bool) 
+000134c0: 2d3e 2027 426c 6f62 4861 6e64 6c65 273a  -> 'BlobHandle':
+000134d0: 0a20 2020 2020 2020 2023 2046 4958 4d45  .        # FIXME
+000134e0: 3a20 2121 2121 2121 2065 7870 6c69 6369  : !!!!!! explici
+000134f0: 746c 7920 7265 7065 6174 206f 6e20 7469  tly repeat on ti
+00013500: 6d65 6f75 740a 2020 2020 2020 2020 6461  meout.        da
+00013510: 6720 3d20 7365 6c66 2e67 6574 5f64 6167  g = self.get_dag
+00013520: 2829 0a20 2020 2020 2020 2072 6573 203d  ().        res =
+00013530: 2063 6173 7428 5265 6164 4e6f 6465 2c20   cast(ReadNode, 
+00013540: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
+00013550: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00013560: 2020 2020 2020 204d 4554 484f 445f 504f         METHOD_PO
+00013570: 5354 2c20 222f 7265 6164 5f6e 6f64 6522  ST, "/read_node"
+00013580: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
+00013590: 2020 2020 2264 6167 223a 2064 6167 2e67      "dag": dag.g
+000135a0: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
+000135b0: 2020 2020 2020 2020 2020 226e 6f64 6522            "node"
+000135c0: 3a20 7365 6c66 2e67 6574 5f69 6428 292c  : self.get_id(),
+000135d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000135e0: 2022 6b65 7922 3a20 6b65 792c 0a20 2020   "key": key,.   
+000135f0: 2020 2020 2020 2020 2020 2020 2022 6368               "ch
+00013600: 756e 6b22 3a20 6368 756e 6b2c 0a20 2020  unk": chunk,.   
+00013610: 2020 2020 2020 2020 2020 2020 2022 6973               "is
+00013620: 5f62 6c6f 636b 696e 6722 3a20 5472 7565  _blocking": True
+00013630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013640: 2020 2266 6f72 6365 5f72 6566 7265 7368    "force_refresh
+00013650: 223a 2066 6f72 6365 5f72 6566 7265 7368  ": force_refresh
+00013660: 2c0a 2020 2020 2020 2020 2020 2020 7d29  ,.            })
+00013670: 290a 2020 2020 2020 2020 7572 6920 3d20  ).        uri = 
+00013680: 7265 735b 2272 6573 756c 745f 7572 6922  res["result_uri"
+00013690: 5d0a 2020 2020 2020 2020 6966 2075 7269  ].        if uri
+000136a0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000136b0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000136c0: 6545 7272 6f72 2866 2275 7269 2069 7320  eError(f"uri is 
+000136d0: 4e6f 6e65 3a20 7b72 6573 7d22 290a 2020  None: {res}").  
+000136e0: 2020 2020 2020 7265 7475 726e 2042 6c6f        return Blo
+000136f0: 6248 616e 646c 6528 7365 6c66 2e5f 636c  bHandle(self._cl
+00013700: 6965 6e74 2c20 7572 692c 2069 735f 6675  ient, uri, is_fu
+00013710: 6c6c 3d54 7275 6529 0a0a 2020 2020 6465  ll=True)..    de
+00013720: 6620 6765 745f 696e 6465 785f 636f 6c28  f get_index_col(
+00013730: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+00013740: 2020 2020 2020 7265 7475 726e 2022 5f69        return "_i
+00013750: 6e64 6578 2220 6966 2073 656c 662e 5f63  ndex" if self._c
+00013760: 6c69 656e 742e 6861 735f 7665 7273 696f  lient.has_versio
+00013770: 6e28 342c 2031 2920 656c 7365 2022 696e  n(4, 1) else "in
+00013780: 6465 7822 0a0a 2020 2020 6465 6620 6765  dex"..    def ge
+00013790: 745f 726f 775f 6964 5f63 6f6c 2873 656c  t_row_id_col(sel
+000137a0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+000137b0: 2020 2072 6574 7572 6e20 225f 726f 775f     return "_row_
+000137c0: 6964 2220 6966 2073 656c 662e 5f63 6c69  id" if self._cli
+000137d0: 656e 742e 6861 735f 7665 7273 696f 6e28  ent.has_version(
+000137e0: 342c 2031 2920 656c 7365 2022 726f 775f  4, 1) else "row_
+000137f0: 6964 220a 0a20 2020 2064 6566 2072 6561  id"..    def rea
+00013800: 6428 0a20 2020 2020 2020 2020 2020 2073  d(.            s
+00013810: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00013820: 206b 6579 3a20 7374 722c 0a20 2020 2020   key: str,.     
+00013830: 2020 2020 2020 2063 6875 6e6b 3a20 4f70         chunk: Op
+00013840: 7469 6f6e 616c 5b69 6e74 5d2c 0a20 2020  tional[int],.   
+00013850: 2020 2020 2020 2020 2066 6f72 6365 5f72           force_r
+00013860: 6566 7265 7368 3a20 626f 6f6c 203d 2046  efresh: bool = F
+00013870: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00013880: 2020 6669 6c74 6572 5f69 643a 2062 6f6f    filter_id: boo
+00013890: 6c20 3d20 5472 7565 2920 2d3e 204f 7074  l = True) -> Opt
+000138a0: 696f 6e61 6c5b 4279 7465 5265 7370 6f6e  ional[ByteRespon
+000138b0: 7365 5d3a 0a20 2020 2020 2020 2063 6f6e  se]:.        con
+000138c0: 7465 6e74 203d 2073 656c 662e 7265 6164  tent = self.read
+000138d0: 5f62 6c6f 6228 6b65 792c 2063 6875 6e6b  _blob(key, chunk
+000138e0: 2c20 666f 7263 655f 7265 6672 6573 6829  , force_refresh)
+000138f0: 2e67 6574 5f63 6f6e 7465 6e74 2829 0a20  .get_content(). 
+00013900: 2020 2020 2020 2069 6620 6669 6c74 6572         if filter
+00013910: 5f69 6420 616e 6420 6973 696e 7374 616e  _id and isinstan
+00013920: 6365 2863 6f6e 7465 6e74 2c20 7064 2e44  ce(content, pd.D
+00013930: 6174 6146 7261 6d65 293a 0a20 2020 2020  ataFrame):.     
+00013940: 2020 2020 2020 2064 663a 2070 642e 4461         df: pd.Da
+00013950: 7461 4672 616d 6520 3d20 636f 6e74 656e  taFrame = conten
+00013960: 740a 2020 2020 2020 2020 2020 2020 6466  t.            df
+00013970: 203d 2064 665b 6466 5b73 656c 662e 6765   = df[df[self.ge
+00013980: 745f 726f 775f 6964 5f63 6f6c 2829 5d20  t_row_id_col()] 
+00013990: 3e3d 2030 5d0a 2020 2020 2020 2020 2020  >= 0].          
+000139a0: 2020 6466 203d 2064 662e 7365 745f 696e    df = df.set_in
+000139b0: 6465 7828 7365 6c66 2e67 6574 5f69 6e64  dex(self.get_ind
+000139c0: 6578 5f63 6f6c 2829 2c20 6472 6f70 3d54  ex_col(), drop=T
+000139d0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+000139e0: 2064 662e 696e 6465 782e 6e61 6d65 203d   df.index.name =
+000139f0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00013a00: 2020 636f 6e74 656e 7420 3d20 6466 2e63    content = df.c
+00013a10: 6f70 7928 290a 2020 2020 2020 2020 7265  opy().        re
+00013a20: 7475 726e 2063 6f6e 7465 6e74 0a0a 2020  turn content..  
+00013a30: 2020 6465 6620 7265 6164 5f61 6c6c 280a    def read_all(.
+00013a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013a50: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+00013a60: 793a 2073 7472 2c0a 2020 2020 2020 2020  y: str,.        
+00013a70: 2020 2020 666f 7263 655f 7265 6672 6573      force_refres
+00013a80: 683a 2062 6f6f 6c20 3d20 4661 6c73 652c  h: bool = False,
+00013a90: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00013aa0: 7465 725f 6964 3a20 626f 6f6c 203d 2054  ter_id: bool = T
+00013ab0: 7275 6529 202d 3e20 4f70 7469 6f6e 616c  rue) -> Optional
+00013ac0: 5b42 7974 6552 6573 706f 6e73 655d 3a0a  [ByteResponse]:.
+00013ad0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+00013ae0: 6428 0a20 2020 2020 2020 2020 2020 206b  d(.            k
+00013af0: 6579 2c20 6368 756e 6b3d 4e6f 6e65 2c20  ey, chunk=None, 
+00013b00: 666f 7263 655f 7265 6672 6573 683d 666f  force_refresh=fo
+00013b10: 7263 655f 7265 6672 6573 682c 2066 696c  rce_refresh, fil
+00013b20: 7465 725f 6964 3d46 616c 7365 290a 2020  ter_id=False).  
+00013b30: 2020 2020 2020 7265 733a 204c 6973 745b        res: List[
+00013b40: 4279 7465 5265 7370 6f6e 7365 5d20 3d20  ByteResponse] = 
+00013b50: 5b5d 0a20 2020 2020 2020 2063 7479 7065  [].        ctype
+00013b60: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00013b70: 3d20 4e6f 6e65 0a20 2020 2020 2020 2077  = None.        w
+00013b80: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+00013b90: 2020 2020 2020 2062 6c6f 6220 3d20 7365         blob = se
+00013ba0: 6c66 2e72 6561 645f 626c 6f62 286b 6579  lf.read_blob(key
+00013bb0: 2c20 6368 756e 6b3d 6c65 6e28 7265 7329  , chunk=len(res)
+00013bc0: 2c20 666f 7263 655f 7265 6672 6573 683d  , force_refresh=
+00013bd0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00013be0: 2020 2063 7572 203d 2062 6c6f 622e 6765     cur = blob.ge
+00013bf0: 745f 636f 6e74 656e 7428 290a 2020 2020  t_content().    
+00013c00: 2020 2020 2020 2020 6966 2063 7572 2069          if cur i
+00013c10: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00013c20: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+00013c30: 2020 2020 2020 2020 2020 6375 725f 6374            cur_ct
+00013c40: 7970 6520 3d20 626c 6f62 2e67 6574 5f63  ype = blob.get_c
+00013c50: 7479 7065 2829 0a20 2020 2020 2020 2020  type().         
+00013c60: 2020 2069 6620 6374 7970 6520 6973 204e     if ctype is N
+00013c70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013c80: 2020 2020 2063 7479 7065 203d 2063 7572       ctype = cur
+00013c90: 5f63 7479 7065 0a20 2020 2020 2020 2020  _ctype.         
+00013ca0: 2020 2065 6c69 6620 6374 7970 6520 213d     elif ctype !=
+00013cb0: 2063 7572 5f63 7479 7065 3a0a 2020 2020   cur_ctype:.    
+00013cc0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00013cd0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cf0: 2020 6622 696e 636f 6e73 6973 7465 6e74    f"inconsistent
+00013d00: 2072 6574 7572 6e20 7479 7065 7320 7b63   return types {c
+00013d10: 7479 7065 7d20 213d 207b 6375 725f 6374  type} != {cur_ct
+00013d20: 7970 657d 2229 0a20 2020 2020 2020 2020  ype}").         
+00013d30: 2020 2072 6573 2e61 7070 656e 6428 6375     res.append(cu
+00013d40: 7229 0a20 2020 2020 2020 2069 6620 6e6f  r).        if no
+00013d50: 7420 7265 7320 6f72 2063 7479 7065 2069  t res or ctype i
+00013d60: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00013d70: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00013d80: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
+00013d90: 3d20 6d65 7267 655f 6374 7970 6528 7265  = merge_ctype(re
+00013da0: 732c 2063 7479 7065 290a 2020 2020 2020  s, ctype).      
+00013db0: 2020 6966 2066 696c 7465 725f 6964 2061    if filter_id a
+00013dc0: 6e64 2069 7369 6e73 7461 6e63 6528 636f  nd isinstance(co
+00013dd0: 6e74 656e 742c 2070 642e 4461 7461 4672  ntent, pd.DataFr
+00013de0: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
+00013df0: 2020 6466 3a20 7064 2e44 6174 6146 7261    df: pd.DataFra
+00013e00: 6d65 203d 2063 6f6e 7465 6e74 0a20 2020  me = content.   
+00013e10: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
+00013e20: 5b64 665b 7365 6c66 2e67 6574 5f72 6f77  [df[self.get_row
+00013e30: 5f69 645f 636f 6c28 295d 203e 3d20 305d  _id_col()] >= 0]
+00013e40: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+00013e50: 3d20 6466 2e73 6574 5f69 6e64 6578 2873  = df.set_index(s
+00013e60: 656c 662e 6765 745f 696e 6465 785f 636f  elf.get_index_co
+00013e70: 6c28 292c 2064 726f 703d 5472 7565 290a  l(), drop=True).
+00013e80: 2020 2020 2020 2020 2020 2020 6466 2e69              df.i
+00013e90: 6e64 6578 2e6e 616d 6520 3d20 4e6f 6e65  ndex.name = None
+00013ea0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00013eb0: 7465 6e74 203d 2064 662e 636f 7079 2829  tent = df.copy()
+00013ec0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013ed0: 636f 6e74 656e 740a 0a20 2020 2064 6566  content..    def
+00013ee0: 2063 6c65 6172 2873 656c 6629 202d 3e20   clear(self) -> 
+00013ef0: 4e6f 6465 5374 6174 653a 0a20 2020 2020  NodeState:.     
+00013f00: 2020 2072 6574 7572 6e20 6361 7374 284e     return cast(N
+00013f10: 6f64 6553 7461 7465 2c20 7365 6c66 2e5f  odeState, self._
+00013f20: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
+00013f30: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00013f40: 204d 4554 484f 445f 5055 542c 2022 2f6e   METHOD_PUT, "/n
+00013f50: 6f64 655f 7374 6174 6522 2c20 7b0a 2020  ode_state", {.  
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00013f70: 6167 223a 2073 656c 662e 6765 745f 6461  ag": self.get_da
+00013f80: 6728 292e 6765 745f 7572 6928 292c 0a20  g().get_uri(),. 
+00013f90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013fa0: 6e6f 6465 223a 2073 656c 662e 6765 745f  node": self.get_
+00013fb0: 6964 2829 2c0a 2020 2020 2020 2020 2020  id(),.          
+00013fc0: 2020 2020 2020 2261 6374 696f 6e22 3a20        "action": 
+00013fd0: 2272 6573 6574 222c 0a20 2020 2020 2020  "reset",.       
+00013fe0: 2020 2020 207d 2929 0a0a 2020 2020 6465       }))..    de
+00013ff0: 6620 7265 7175 6575 6528 7365 6c66 2920  f requeue(self) 
+00014000: 2d3e 204e 6f64 6553 7461 7465 3a0a 2020  -> NodeState:.  
+00014010: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00014020: 7428 4e6f 6465 5374 6174 652c 2073 656c  t(NodeState, sel
+00014030: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+00014040: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+00014050: 2020 2020 4d45 5448 4f44 5f50 5554 2c20      METHOD_PUT, 
+00014060: 222f 6e6f 6465 5f73 7461 7465 222c 207b  "/node_state", {
+00014070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014080: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
+00014090: 5f64 6167 2829 2e67 6574 5f75 7269 2829  _dag().get_uri()
+000140a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000140b0: 2020 226e 6f64 6522 3a20 7365 6c66 2e67    "node": self.g
+000140c0: 6574 5f69 6428 292c 0a20 2020 2020 2020  et_id(),.       
+000140d0: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
+000140e0: 223a 2022 7265 7175 6575 6522 2c0a 2020  ": "requeue",.  
+000140f0: 2020 2020 2020 2020 2020 7d29 290a 0a20            })).. 
+00014100: 2020 2064 6566 2066 6978 5f65 7272 6f72     def fix_error
+00014110: 2873 656c 6629 202d 3e20 4e6f 6465 5374  (self) -> NodeSt
+00014120: 6174 653a 0a20 2020 2020 2020 2072 6574  ate:.        ret
+00014130: 7572 6e20 6361 7374 284e 6f64 6553 7461  urn cast(NodeSta
+00014140: 7465 2c20 7365 6c66 2e5f 636c 6965 6e74  te, self._client
+00014150: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+00014160: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+00014170: 445f 5055 542c 2022 2f6e 6f64 655f 7374  D_PUT, "/node_st
+00014180: 6174 6522 2c20 7b0a 2020 2020 2020 2020  ate", {.        
+00014190: 2020 2020 2020 2020 2264 6167 223a 2073          "dag": s
+000141a0: 656c 662e 6765 745f 6461 6728 292e 6765  elf.get_dag().ge
+000141b0: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
+000141c0: 2020 2020 2020 2020 2022 6e6f 6465 223a           "node":
+000141d0: 2073 656c 662e 6765 745f 6964 2829 2c0a   self.get_id(),.
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141f0: 2261 6374 696f 6e22 3a20 2266 6978 5f65  "action": "fix_e
+00014200: 7272 6f72 222c 0a20 2020 2020 2020 2020  rror",.         
+00014210: 2020 207d 2929 0a0a 2020 2020 6465 6620     }))..    def 
+00014220: 6765 745f 626c 6f62 5f75 7269 280a 2020  get_blob_uri(.  
+00014230: 2020 2020 2020 2020 2020 7365 6c66 2c20            self, 
+00014240: 626c 6f62 5f6b 6579 3a20 7374 722c 2062  blob_key: str, b
+00014250: 6c6f 625f 7479 7065 3a20 7374 7229 202d  lob_type: str) -
+00014260: 3e20 5475 706c 655b 7374 722c 2042 6c6f  > Tuple[str, Blo
+00014270: 624f 776e 6572 5d3a 0a20 2020 2020 2020  bOwner]:.       
+00014280: 2072 6573 203d 2063 6173 7428 426c 6f62   res = cast(Blob
+00014290: 5552 4952 6573 706f 6e73 652c 2073 656c  URIResponse, sel
+000142a0: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+000142b0: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+000142c0: 2020 2020 4d45 5448 4f44 5f47 4554 2c20      METHOD_GET, 
+000142d0: 222f 626c 6f62 5f75 7269 222c 207b 0a20  "/blob_uri", {. 
+000142e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000142f0: 6461 6722 3a20 7365 6c66 2e67 6574 5f64  dag": self.get_d
+00014300: 6167 2829 2e67 6574 5f75 7269 2829 2c0a  ag().get_uri(),.
+00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014320: 226e 6f64 6522 3a20 7365 6c66 2e67 6574  "node": self.get
+00014330: 5f69 6428 292c 0a20 2020 2020 2020 2020  _id(),.         
+00014340: 2020 2020 2020 2022 6b65 7922 3a20 626c         "key": bl
+00014350: 6f62 5f6b 6579 2c0a 2020 2020 2020 2020  ob_key,.        
+00014360: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00014370: 626c 6f62 5f74 7970 652c 0a20 2020 2020  blob_type,.     
+00014380: 2020 2020 2020 207d 2929 0a20 2020 2020         })).     
+00014390: 2020 2072 6574 7572 6e20 7265 735b 2275     return res["u
+000143a0: 7269 225d 2c20 7265 735b 226f 776e 6572  ri"], res["owner
+000143b0: 225d 0a0a 2020 2020 6465 6620 6765 745f  "]..    def get_
+000143c0: 6373 765f 626c 6f62 2873 656c 662c 206b  csv_blob(self, k
+000143d0: 6579 3a20 7374 7220 3d20 226f 7269 6722  ey: str = "orig"
+000143e0: 2920 2d3e 2027 4353 5642 6c6f 6248 616e  ) -> 'CSVBlobHan
+000143f0: 646c 6527 3a0a 2020 2020 2020 2020 7572  dle':.        ur
+00014400: 692c 206f 776e 6572 203d 2073 656c 662e  i, owner = self.
+00014410: 6765 745f 626c 6f62 5f75 7269 286b 6579  get_blob_uri(key
+00014420: 2c20 2263 7376 2229 0a20 2020 2020 2020  , "csv").       
+00014430: 2062 6c6f 6220 3d20 4353 5642 6c6f 6248   blob = CSVBlobH
+00014440: 616e 646c 6528 7365 6c66 2e5f 636c 6965  andle(self._clie
+00014450: 6e74 2c20 7572 692c 2069 735f 6675 6c6c  nt, uri, is_full
+00014460: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00014470: 626c 6f62 2e73 6574 5f6c 6f63 616c 5f6f  blob.set_local_o
+00014480: 776e 6572 286f 776e 6572 290a 2020 2020  wner(owner).    
+00014490: 2020 2020 7265 7475 726e 2062 6c6f 620a      return blob.
+000144a0: 0a20 2020 2064 6566 2067 6574 5f74 6f72  .    def get_tor
+000144b0: 6368 5f62 6c6f 6228 7365 6c66 2c20 6b65  ch_blob(self, ke
+000144c0: 793a 2073 7472 203d 2022 6f72 6967 2229  y: str = "orig")
+000144d0: 202d 3e20 2754 6f72 6368 426c 6f62 4861   -> 'TorchBlobHa
+000144e0: 6e64 6c65 273a 0a20 2020 2020 2020 2075  ndle':.        u
+000144f0: 7269 2c20 6f77 6e65 7220 3d20 7365 6c66  ri, owner = self
+00014500: 2e67 6574 5f62 6c6f 625f 7572 6928 6b65  .get_blob_uri(ke
+00014510: 792c 2022 746f 7263 6822 290a 2020 2020  y, "torch").    
+00014520: 2020 2020 626c 6f62 203d 2054 6f72 6368      blob = Torch
+00014530: 426c 6f62 4861 6e64 6c65 2873 656c 662e  BlobHandle(self.
+00014540: 5f63 6c69 656e 742c 2075 7269 2c20 6973  _client, uri, is
+00014550: 5f66 756c 6c3d 4661 6c73 6529 0a20 2020  _full=False).   
+00014560: 2020 2020 2062 6c6f 622e 7365 745f 6c6f       blob.set_lo
+00014570: 6361 6c5f 6f77 6e65 7228 6f77 6e65 7229  cal_owner(owner)
+00014580: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014590: 626c 6f62 0a0a 2020 2020 6465 6620 6765  blob..    def ge
+000145a0: 745f 6a73 6f6e 5f62 6c6f 6228 7365 6c66  t_json_blob(self
+000145b0: 2c20 6b65 793a 2073 7472 203d 2022 6a73  , key: str = "js
+000145c0: 6f6e 735f 696e 2229 202d 3e20 274a 534f  ons_in") -> 'JSO
+000145d0: 4e42 6c6f 6248 616e 646c 6527 3a0a 2020  NBlobHandle':.  
+000145e0: 2020 2020 2020 7572 692c 206f 776e 6572        uri, owner
+000145f0: 203d 2073 656c 662e 6765 745f 626c 6f62   = self.get_blob
+00014600: 5f75 7269 286b 6579 2c20 226a 736f 6e22  _uri(key, "json"
+00014610: 290a 2020 2020 2020 2020 626c 6f62 203d  ).        blob =
+00014620: 204a 534f 4e42 6c6f 6248 616e 646c 6528   JSONBlobHandle(
+00014630: 7365 6c66 2e5f 636c 6965 6e74 2c20 7572  self._client, ur
+00014640: 692c 2069 735f 6675 6c6c 3d46 616c 7365  i, is_full=False
+00014650: 290a 2020 2020 2020 2020 626c 6f62 2e73  ).        blob.s
+00014660: 6574 5f6c 6f63 616c 5f6f 776e 6572 286f  et_local_owner(o
+00014670: 776e 6572 290a 2020 2020 2020 2020 7265  wner).        re
+00014680: 7475 726e 2062 6c6f 620a 0a20 2020 2064  turn blob..    d
+00014690: 6566 2067 6574 5f63 7573 746f 6d5f 636f  ef get_custom_co
+000146a0: 6465 5f62 6c6f 6228 0a20 2020 2020 2020  de_blob(.       
+000146b0: 2020 2020 2073 656c 662c 206b 6579 3a20       self, key: 
+000146c0: 7374 7220 3d20 2263 7573 746f 6d5f 636f  str = "custom_co
+000146d0: 6465 2229 202d 3e20 2743 7573 746f 6d43  de") -> 'CustomC
+000146e0: 6f64 6542 6c6f 6248 616e 646c 6527 3a0a  odeBlobHandle':.
+000146f0: 2020 2020 2020 2020 7572 692c 206f 776e          uri, own
+00014700: 6572 203d 2073 656c 662e 6765 745f 626c  er = self.get_bl
+00014710: 6f62 5f75 7269 286b 6579 2c20 2263 7573  ob_uri(key, "cus
+00014720: 746f 6d5f 636f 6465 2229 0a20 2020 2020  tom_code").     
+00014730: 2020 2062 6c6f 6220 3d20 4375 7374 6f6d     blob = Custom
+00014740: 436f 6465 426c 6f62 4861 6e64 6c65 2873  CodeBlobHandle(s
+00014750: 656c 662e 5f63 6c69 656e 742c 2075 7269  elf._client, uri
+00014760: 2c20 6973 5f66 756c 6c3d 4661 6c73 6529  , is_full=False)
+00014770: 0a20 2020 2020 2020 2062 6c6f 622e 7365  .        blob.se
+00014780: 745f 6c6f 6361 6c5f 6f77 6e65 7228 6f77  t_local_owner(ow
+00014790: 6e65 7229 0a20 2020 2020 2020 2072 6574  ner).        ret
+000147a0: 7572 6e20 626c 6f62 0a0a 2020 2020 6465  urn blob..    de
+000147b0: 6620 6368 6563 6b5f 6375 7374 6f6d 5f63  f check_custom_c
+000147c0: 6f64 655f 6e6f 6465 2873 656c 6629 202d  ode_node(self) -
+000147d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000147e0: 6966 206e 6f74 2073 656c 662e 6765 745f  if not self.get_
+000147f0: 7479 7065 2829 2069 6e20 4355 5354 4f4d  type() in CUSTOM
+00014800: 5f4e 4f44 455f 5459 5045 533a 0a20 2020  _NODE_TYPES:.   
+00014810: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00014820: 616c 7565 4572 726f 7228 6622 7b73 656c  alueError(f"{sel
+00014830: 667d 2069 7320 6e6f 7420 6120 6375 7374  f} is not a cust
+00014840: 6f6d 2063 6f64 6520 6e6f 6465 2e22 290a  om code node.").
+00014850: 0a20 2020 2064 6566 2073 6574 5f63 7573  .    def set_cus
+00014860: 746f 6d5f 696d 706f 7274 7328 0a20 2020  tom_imports(.   
+00014870: 2020 2020 2020 2020 2073 656c 662c 206d           self, m
+00014880: 6f64 756c 6573 3a20 4c69 7374 5b4c 6973  odules: List[Lis
+00014890: 745b 7374 725d 5d29 202d 3e20 4e6f 6465  t[str]]) -> Node
+000148a0: 4375 7374 6f6d 496d 706f 7274 733a 0a20  CustomImports:. 
+000148b0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+000148c0: 6b5f 6375 7374 6f6d 5f63 6f64 655f 6e6f  k_custom_code_no
+000148d0: 6465 2829 0a20 2020 2020 2020 2072 6574  de().        ret
+000148e0: 7572 6e20 6361 7374 284e 6f64 6543 7573  urn cast(NodeCus
+000148f0: 746f 6d49 6d70 6f72 7473 2c20 7365 6c66  tomImports, self
+00014900: 2e5f 636c 6965 6e74 2e72 6571 7565 7374  ._client.request
+00014910: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
+00014920: 2020 204d 4554 484f 445f 5055 542c 2022     METHOD_PUT, "
+00014930: 2f63 7573 746f 6d5f 696d 706f 7274 7322  /custom_imports"
+00014940: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
+00014950: 2020 2020 2264 6167 223a 2073 656c 662e      "dag": self.
+00014960: 6765 745f 6461 6728 292e 6765 745f 7572  get_dag().get_ur
+00014970: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
+00014980: 2020 2020 2022 6e6f 6465 223a 2073 656c       "node": sel
+00014990: 662e 6765 745f 6964 2829 2c0a 2020 2020  f.get_id(),.    
+000149a0: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
+000149b0: 756c 6573 223a 206d 6f64 756c 6573 2c0a  ules": modules,.
+000149c0: 2020 2020 2020 2020 2020 2020 7d29 290a              })).
+000149d0: 0a20 2020 2064 6566 2067 6574 5f63 7573  .    def get_cus
+000149e0: 746f 6d5f 696d 706f 7274 7328 7365 6c66  tom_imports(self
+000149f0: 2920 2d3e 204e 6f64 6543 7573 746f 6d49  ) -> NodeCustomI
+00014a00: 6d70 6f72 7473 3a0a 2020 2020 2020 2020  mports:.        
+00014a10: 7365 6c66 2e63 6865 636b 5f63 7573 746f  self.check_custo
+00014a20: 6d5f 636f 6465 5f6e 6f64 6528 290a 2020  m_code_node().  
+00014a30: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00014a40: 7428 4e6f 6465 4375 7374 6f6d 496d 706f  t(NodeCustomImpo
+00014a50: 7274 732c 2073 656c 662e 5f63 6c69 656e  rts, self._clien
+00014a60: 742e 7265 7175 6573 745f 6a73 6f6e 280a  t.request_json(.
+00014a70: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00014a80: 4f44 5f47 4554 2c20 222f 6375 7374 6f6d  OD_GET, "/custom
+00014a90: 5f69 6d70 6f72 7473 222c 207b 0a20 2020  _imports", {.   
+00014aa0: 2020 2020 2020 2020 2020 2020 2022 6461               "da
+00014ab0: 6722 3a20 7365 6c66 2e67 6574 5f64 6167  g": self.get_dag
+00014ac0: 2829 2e67 6574 5f75 7269 2829 2c0a 2020  ().get_uri(),.  
+00014ad0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00014ae0: 6f64 6522 3a20 7365 6c66 2e67 6574 5f69  ode": self.get_i
+00014af0: 6428 292c 0a20 2020 2020 2020 2020 2020  d(),.           
+00014b00: 207d 2929 0a0a 2020 2020 6465 6620 7365   }))..    def se
+00014b10: 745f 6573 5f71 7565 7279 2873 656c 662c  t_es_query(self,
+00014b20: 2071 7565 7279 3a20 4469 6374 5b73 7472   query: Dict[str
+00014b30: 2c20 416e 795d 2920 2d3e 2045 5351 7565  , Any]) -> ESQue
+00014b40: 7279 5265 7370 6f6e 7365 3a0a 2020 2020  ryResponse:.    
+00014b50: 2020 2020 6966 2073 656c 662e 6765 745f      if self.get_
+00014b60: 7479 7065 2829 2021 3d20 2265 735f 7265  type() != "es_re
+00014b70: 6164 6572 223a 0a20 2020 2020 2020 2020  ader":.         
+00014b80: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00014b90: 726f 7228 6622 7b73 656c 667d 2069 7320  ror(f"{self} is 
+00014ba0: 6e6f 7420 616e 2045 5320 7265 6164 6572  not an ES reader
+00014bb0: 206e 6f64 6522 290a 0a20 2020 2020 2020   node")..       
+00014bc0: 2072 6574 7572 6e20 6361 7374 2845 5351   return cast(ESQ
+00014bd0: 7565 7279 5265 7370 6f6e 7365 2c20 7365  ueryResponse, se
+00014be0: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
+00014bf0: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
+00014c00: 2020 2020 204d 4554 484f 445f 504f 5354       METHOD_POST
+00014c10: 2c20 222f 6573 5f71 7565 7279 222c 207b  , "/es_query", {
+00014c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c30: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
+00014c40: 5f64 6167 2829 2e67 6574 5f75 7269 2829  _dag().get_uri()
+00014c50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014c60: 2020 2262 6c6f 6222 3a20 7365 6c66 2e67    "blob": self.g
+00014c70: 6574 5f62 6c6f 625f 6861 6e64 6c65 2822  et_blob_handle("
+00014c80: 6573 2229 2e67 6574 5f75 7269 2829 2c0a  es").get_uri(),.
+00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ca0: 2265 735f 7175 6572 7922 3a20 7175 6572  "es_query": quer
+00014cb0: 792c 0a20 2020 2020 2020 2020 2020 207d  y,.            }
+00014cc0: 2c0a 2020 2020 2020 2020 2929 0a0a 2020  ,.        ))..  
+00014cd0: 2020 6465 6620 6765 745f 6573 5f71 7565    def get_es_que
+00014ce0: 7279 2873 656c 6629 202d 3e20 4553 5175  ry(self) -> ESQu
+00014cf0: 6572 7952 6573 706f 6e73 653a 0a20 2020  eryResponse:.   
+00014d00: 2020 2020 2069 6620 7365 6c66 2e67 6574       if self.get
+00014d10: 5f74 7970 6528 2920 213d 2022 6573 5f72  _type() != "es_r
+00014d20: 6561 6465 7222 3a0a 2020 2020 2020 2020  eader":.        
+00014d30: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00014d40: 7272 6f72 2866 227b 7365 6c66 7d20 6973  rror(f"{self} is
+00014d50: 206e 6f74 2061 6e20 4553 2072 6561 6465   not an ES reade
+00014d60: 7220 6e6f 6465 2229 0a0a 2020 2020 2020  r node")..      
+00014d70: 2020 7265 7475 726e 2063 6173 7428 4553    return cast(ES
+00014d80: 5175 6572 7952 6573 706f 6e73 652c 2073  QueryResponse, s
+00014d90: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
+00014da0: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
+00014db0: 2020 2020 2020 4d45 5448 4f44 5f47 4554        METHOD_GET
+00014dc0: 2c20 222f 6573 5f71 7565 7279 222c 207b  , "/es_query", {
+00014dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014de0: 2022 6461 6722 3a20 7365 6c66 2e67 6574   "dag": self.get
+00014df0: 5f64 6167 2829 2e67 6574 5f75 7269 2829  _dag().get_uri()
+00014e00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014e10: 2020 2262 6c6f 6222 3a20 7365 6c66 2e67    "blob": self.g
+00014e20: 6574 5f62 6c6f 625f 6861 6e64 6c65 2822  et_blob_handle("
+00014e30: 6573 2229 2e67 6574 5f75 7269 2829 2c0a  es").get_uri(),.
+00014e40: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00014e50: 2020 2020 2020 2029 290a 0a20 2020 2064         ))..    d
+00014e60: 6566 2067 6574 5f75 7365 725f 636f 6c75  ef get_user_colu
+00014e70: 6d6e 7328 7365 6c66 2c20 6b65 793a 2073  mns(self, key: s
+00014e80: 7472 2920 2d3e 204e 6f64 6555 7365 7243  tr) -> NodeUserC
+00014e90: 6f6c 756d 6e73 5265 7370 6f6e 7365 3a0a  olumnsResponse:.
+00014ea0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00014eb0: 6173 7428 4e6f 6465 5573 6572 436f 6c75  ast(NodeUserColu
+00014ec0: 6d6e 7352 6573 706f 6e73 652c 2073 656c  mnsResponse, sel
+00014ed0: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+00014ee0: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+00014ef0: 2020 2020 4d45 5448 4f44 5f47 4554 2c20      METHOD_GET, 
+00014f00: 222f 7573 6572 5f63 6f6c 756d 6e73 222c  "/user_columns",
+00014f10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00014f20: 2020 2022 6461 6722 3a20 7365 6c66 2e67     "dag": self.g
+00014f30: 6574 5f64 6167 2829 2e67 6574 5f75 7269  et_dag().get_uri
+00014f40: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00014f50: 2020 2020 226e 6f64 6522 3a20 7365 6c66      "node": self
+00014f60: 2e67 6574 5f69 6428 292c 0a20 2020 2020  .get_id(),.     
+00014f70: 2020 2020 2020 2020 2020 2022 6b65 7922             "key"
+00014f80: 3a20 6b65 792c 0a20 2020 2020 2020 2020  : key,.         
+00014f90: 2020 207d 2929 0a0a 2020 2020 6465 6620     }))..    def 
+00014fa0: 6765 745f 696e 7075 745f 6578 616d 706c  get_input_exampl
+00014fb0: 6528 7365 6c66 2920 2d3e 2044 6963 745b  e(self) -> Dict[
+00014fc0: 7374 722c 204f 7074 696f 6e61 6c5b 4279  str, Optional[By
+00014fd0: 7465 5265 7370 6f6e 7365 5d5d 3a0a 2020  teResponse]]:.  
+00014fe0: 2020 2020 2020 7265 7320 3d20 7b7d 0a20        res = {}. 
+00014ff0: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
+00015000: 6e20 7365 6c66 2e67 6574 5f69 6e70 7574  n self.get_input
+00015010: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00015020: 2069 6e70 7574 5f6e 6f64 652c 206f 7574   input_node, out
+00015030: 5f6b 6579 203d 2073 656c 662e 6765 745f  _key = self.get_
+00015040: 696e 7075 7428 6b65 7929 0a20 2020 2020  input(key).     
+00015050: 2020 2020 2020 2064 6620 3d20 696e 7075         df = inpu
+00015060: 745f 6e6f 6465 2e72 6561 6428 6f75 745f  t_node.read(out_
+00015070: 6b65 792c 2030 290a 2020 2020 2020 2020  key, 0).        
+00015080: 2020 2020 6966 2064 6620 6973 206e 6f74      if df is not
+00015090: 204e 6f6e 6520 616e 6420 6973 696e 7374   None and isinst
+000150a0: 616e 6365 2864 662c 2070 642e 4461 7461  ance(df, pd.Data
+000150b0: 4672 616d 6529 3a0a 2020 2020 2020 2020  Frame):.        
+000150c0: 2020 2020 2020 2020 7573 6572 5f63 6f6c          user_col
+000150d0: 756d 6e73 203d 205c 0a20 2020 2020 2020  umns = \.       
+000150e0: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+000150f0: 7574 5f6e 6f64 652e 6765 745f 7573 6572  ut_node.get_user
+00015100: 5f63 6f6c 756d 6e73 286f 7574 5f6b 6579  _columns(out_key
+00015110: 295b 2275 7365 725f 636f 6c75 6d6e 7322  )["user_columns"
+00015120: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00015130: 2020 726d 6170 203d 207b 636f 6c3a 2063    rmap = {col: c
+00015140: 6f6c 2e72 6570 6c61 6365 2822 7573 6572  ol.replace("user
+00015150: 5f22 2c20 2222 2920 666f 7220 636f 6c20  _", "") for col 
+00015160: 696e 2075 7365 725f 636f 6c75 6d6e 737d  in user_columns}
+00015170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015180: 2064 6620 3d20 6466 2e6c 6f63 5b3a 2c20   df = df.loc[:, 
+00015190: 7573 6572 5f63 6f6c 756d 6e73 5d2e 7265  user_columns].re
+000151a0: 6e61 6d65 2863 6f6c 756d 6e73 3d72 6d61  name(columns=rma
+000151b0: 7029 0a20 2020 2020 2020 2020 2020 2072  p).            r
+000151c0: 6573 5b6b 6579 5d20 3d20 6466 0a20 2020  es[key] = df.   
+000151d0: 2020 2020 2072 6574 7572 6e20 7265 730a       return res.
+000151e0: 0a20 2020 2064 6566 2067 6574 5f64 6566  .    def get_def
+000151f0: 2873 656c 6629 202d 3e20 4e6f 6465 4465  (self) -> NodeDe
+00015200: 663a 0a20 2020 2020 2020 2072 6574 7572  f:.        retur
+00015210: 6e20 6361 7374 284e 6f64 6544 6566 2c20  n cast(NodeDef, 
+00015220: 7365 6c66 2e5f 636c 6965 6e74 2e72 6571  self._client.req
+00015230: 7565 7374 5f6a 736f 6e28 0a20 2020 2020  uest_json(.     
+00015240: 2020 2020 2020 204d 4554 484f 445f 4745         METHOD_GE
+00015250: 542c 2022 2f6e 6f64 655f 6465 6622 2c20  T, "/node_def", 
+00015260: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00015270: 2020 2264 6167 223a 2073 656c 662e 6765    "dag": self.ge
+00015280: 745f 6461 6728 292e 6765 745f 7572 6928  t_dag().get_uri(
+00015290: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000152a0: 2020 2022 6e6f 6465 223a 2073 656c 662e     "node": self.
+000152b0: 6765 745f 6964 2829 2c0a 2020 2020 2020  get_id(),.      
+000152c0: 2020 2020 2020 7d29 290a 0a20 2020 2023        }))..    #
+000152d0: 204d 6f64 656c 4c69 6b65 204e 6f64 6573   ModelLike Nodes
+000152e0: 206f 6e6c 790a 0a20 2020 2064 6566 2069   only..    def i
+000152f0: 735f 6d6f 6465 6c28 7365 6c66 2920 2d3e  s_model(self) ->
+00015300: 2062 6f6f 6c3a 0a20 2020 2020 2020 2069   bool:.        i
+00015310: 6620 7365 6c66 2e5f 6973 5f6d 6f64 656c  f self._is_model
+00015320: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00015330: 2020 2020 2020 7365 6c66 2e5f 6973 5f6d        self._is_m
+00015340: 6f64 656c 203d 2063 6173 7428 4e6f 6465  odel = cast(Node
+00015350: 5479 7065 5265 7370 6f6e 7365 2c20 7365  TypeResponse, se
+00015360: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
+00015370: 7374 5f6a 736f 6e28 0a20 2020 2020 2020  st_json(.       
+00015380: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+00015390: 4745 542c 2022 2f6e 6f64 655f 7479 7065  GET, "/node_type
+000153a0: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+000153b0: 2020 2020 2020 2020 2022 6461 6722 3a20           "dag": 
+000153c0: 7365 6c66 2e67 6574 5f64 6167 2829 2e67  self.get_dag().g
+000153d0: 6574 5f75 7269 2829 2c0a 2020 2020 2020  et_uri(),.      
+000153e0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+000153f0: 6f64 6522 3a20 7365 6c66 2e67 6574 5f69  ode": self.get_i
+00015400: 6428 292c 0a20 2020 2020 2020 2020 2020  d(),.           
+00015410: 2020 2020 207d 2929 5b22 6973 5f6d 6f64       }))["is_mod
+00015420: 656c 225d 0a0a 2020 2020 2020 2020 7265  el"]..        re
+00015430: 7475 726e 2073 656c 662e 5f69 735f 6d6f  turn self._is_mo
+00015440: 6465 6c0a 0a20 2020 2064 6566 2065 6e73  del..    def ens
+00015450: 7572 655f 6973 5f6d 6f64 656c 2873 656c  ure_is_model(sel
+00015460: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00015470: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00015480: 6973 5f6d 6f64 656c 2829 3a0a 2020 2020  is_model():.    
+00015490: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+000154a0: 6c75 6545 7272 6f72 2866 227b 7365 6c66  lueError(f"{self
+000154b0: 7d20 6973 206e 6f74 2061 206d 6f64 656c  } is not a model
+000154c0: 206e 6f64 652e 2229 0a0a 2020 2020 6465   node.")..    de
+000154d0: 6620 7365 7475 705f 6d6f 6465 6c28 7365  f setup_model(se
+000154e0: 6c66 2c20 6f62 6a3a 2044 6963 745b 7374  lf, obj: Dict[st
+000154f0: 722c 2041 6e79 5d29 202d 3e20 4d6f 6465  r, Any]) -> Mode
+00015500: 6c49 6e66 6f3a 0a20 2020 2020 2020 2073  lInfo:.        s
+00015510: 656c 662e 656e 7375 7265 5f69 735f 6d6f  elf.ensure_is_mo
+00015520: 6465 6c28 290a 2020 2020 2020 2020 7265  del().        re
+00015530: 7475 726e 2063 6173 7428 4d6f 6465 6c49  turn cast(ModelI
+00015540: 6e66 6f2c 2073 656c 662e 5f63 6c69 656e  nfo, self._clien
+00015550: 742e 7265 7175 6573 745f 6a73 6f6e 280a  t.request_json(.
+00015560: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00015570: 4f44 5f50 5554 2c20 222f 6d6f 6465 6c5f  OD_PUT, "/model_
+00015580: 7365 7475 7022 2c20 7b0a 2020 2020 2020  setup", {.      
+00015590: 2020 2020 2020 2020 2020 2264 6167 223a            "dag":
+000155a0: 2073 656c 662e 6765 745f 6461 6728 292e   self.get_dag().
+000155b0: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
+000155c0: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
+000155d0: 223a 2073 656c 662e 6765 745f 6964 2829  ": self.get_id()
+000155e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000155f0: 2020 2263 6f6e 6669 6722 3a20 6f62 6a2c    "config": obj,
+00015600: 0a20 2020 2020 2020 2020 2020 207d 2929  .            }))
+00015610: 0a0a 2020 2020 6465 6620 6765 745f 6d6f  ..    def get_mo
+00015620: 6465 6c5f 7061 7261 6d73 2873 656c 6629  del_params(self)
+00015630: 202d 3e20 4d6f 6465 6c50 6172 616d 7352   -> ModelParamsR
+00015640: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00015650: 2073 656c 662e 656e 7375 7265 5f69 735f   self.ensure_is_
+00015660: 6d6f 6465 6c28 290a 2020 2020 2020 2020  model().        
+00015670: 7265 7475 726e 2063 6173 7428 4d6f 6465  return cast(Mode
+00015680: 6c50 6172 616d 7352 6573 706f 6e73 652c  lParamsResponse,
+00015690: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
+000156a0: 7175 6573 745f 6a73 6f6e 280a 2020 2020  quest_json(.    
+000156b0: 2020 2020 2020 2020 4d45 5448 4f44 5f47          METHOD_G
+000156c0: 4554 2c20 222f 6d6f 6465 6c5f 7061 7261  ET, "/model_para
+000156d0: 6d73 222c 207b 0a20 2020 2020 2020 2020  ms", {.         
+000156e0: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
+000156f0: 6c66 2e67 6574 5f64 6167 2829 2e67 6574  lf.get_dag().get
+00015700: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
+00015710: 2020 2020 2020 2020 226e 6f64 6522 3a20          "node": 
+00015720: 7365 6c66 2e67 6574 5f69 6428 292c 0a20  self.get_id(),. 
+00015730: 2020 2020 2020 2020 2020 207d 2929 0a0a             }))..
+00015740: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
+00015750: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00015760: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+00015770: 7368 2828 7365 6c66 2e67 6574 5f64 6167  sh((self.get_dag
+00015780: 2829 2c20 7365 6c66 2e67 6574 5f69 6428  (), self.get_id(
+00015790: 2929 290a 0a20 2020 2064 6566 205f 5f65  )))..    def __e
+000157a0: 715f 5f28 7365 6c66 2c20 6f74 6865 723a  q__(self, other:
+000157b0: 206f 626a 6563 7429 202d 3e20 626f 6f6c   object) -> bool
+000157c0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+000157d0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+000157e0: 722c 2073 656c 662e 5f5f 636c 6173 735f  r, self.__class_
+000157f0: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
+00015800: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00015810: 2020 2020 2069 6620 7365 6c66 2e67 6574       if self.get
+00015820: 5f64 6167 2829 2021 3d20 6f74 6865 722e  _dag() != other.
+00015830: 6765 745f 6461 6728 293a 0a20 2020 2020  get_dag():.     
+00015840: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00015850: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+00015860: 726e 2073 656c 662e 6765 745f 6964 2829  rn self.get_id()
+00015870: 203d 3d20 6f74 6865 722e 6765 745f 6964   == other.get_id
+00015880: 2829 0a0a 2020 2020 6465 6620 5f5f 6e65  ()..    def __ne
+00015890: 5f5f 2873 656c 662c 206f 7468 6572 3a20  __(self, other: 
+000158a0: 6f62 6a65 6374 2920 2d3e 2062 6f6f 6c3a  object) -> bool:
+000158b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000158c0: 6e6f 7420 7365 6c66 2e5f 5f65 715f 5f28  not self.__eq__(
+000158d0: 6f74 6865 7229 0a0a 2020 2020 6465 6620  other)..    def 
+000158e0: 5f5f 7374 725f 5f28 7365 6c66 2920 2d3e  __str__(self) ->
+000158f0: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+00015900: 7475 726e 2073 656c 662e 6765 745f 6964  turn self.get_id
+00015910: 2829 0a0a 2020 2020 6465 6620 5f5f 7265  ()..    def __re
+00015920: 7072 5f5f 2873 656c 6629 202d 3e20 7374  pr__(self) -> st
+00015930: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+00015940: 6e20 6622 7b73 656c 662e 5f5f 636c 6173  n f"{self.__clas
+00015950: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d5b 7b73  s__.__name__}[{s
+00015960: 656c 662e 6765 745f 6964 2829 7d5d 220a  elf.get_id()}]".
+00015970: 0a23 202a 2a2a 204e 6f64 6548 616e 646c  .# *** NodeHandl
+00015980: 6520 2a2a 2a0a 0a0a 454d 5054 595f 424c  e ***...EMPTY_BL
+00015990: 4f42 5f50 5245 4649 5820 3d20 226e 756c  OB_PREFIX = "nul
+000159a0: 6c3a 2f2f 220a 0a0a 636c 6173 7320 426c  l://"...class Bl
+000159b0: 6f62 4861 6e64 6c65 3a0a 2020 2020 6465  obHandle:.    de
+000159c0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000159d0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000159e0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000159f0: 3a20 5859 4d45 436c 6965 6e74 2c0a 2020  : XYMEClient,.  
+00015a00: 2020 2020 2020 2020 2020 7572 693a 2073            uri: s
+00015a10: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00015a20: 6973 5f66 756c 6c3a 2062 6f6f 6c29 202d  is_full: bool) -
+00015a30: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00015a40: 7365 6c66 2e5f 636c 6965 6e74 203d 2063  self._client = c
+00015a50: 6c69 656e 740a 2020 2020 2020 2020 7365  lient.        se
+00015a60: 6c66 2e5f 7572 6920 3d20 7572 690a 2020  lf._uri = uri.  
+00015a70: 2020 2020 2020 7365 6c66 2e5f 6973 5f66        self._is_f
+00015a80: 756c 6c20 3d20 6973 5f66 756c 6c0a 2020  ull = is_full.  
+00015a90: 2020 2020 2020 7365 6c66 2e5f 6374 7970        self._ctyp
+00015aa0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00015ab0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00015ac0: 7365 6c66 2e5f 746d 705f 7572 693a 204f  self._tmp_uri: O
+00015ad0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00015ae0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00015af0: 2e5f 6f77 6e65 723a 204f 7074 696f 6e61  ._owner: Optiona
+00015b00: 6c5b 426c 6f62 4f77 6e65 725d 203d 204e  l[BlobOwner] = N
+00015b10: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00015b20: 2e5f 696e 666f 3a20 4f70 7469 6f6e 616c  ._info: Optional
+00015b30: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00015b40: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00015b50: 7365 6c66 2e5f 7061 7265 6e74 3a20 4f70  self._parent: Op
+00015b60: 7469 6f6e 616c 5b42 6c6f 6248 616e 646c  tional[BlobHandl
+00015b70: 655d 203d 204e 6f6e 650a 0a20 2020 2064  e] = None..    d
+00015b80: 6566 2069 735f 6675 6c6c 2873 656c 6629  ef is_full(self)
+00015b90: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00015ba0: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
+00015bb0: 735f 6675 6c6c 0a0a 2020 2020 6465 6620  s_full..    def 
+00015bc0: 6973 5f65 6d70 7479 2873 656c 6629 202d  is_empty(self) -
+00015bd0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00015be0: 7265 7475 726e 2073 656c 662e 5f75 7269  return self._uri
+00015bf0: 2e73 7461 7274 7377 6974 6828 454d 5054  .startswith(EMPT
+00015c00: 595f 424c 4f42 5f50 5245 4649 5829 0a0a  Y_BLOB_PREFIX)..
+00015c10: 2020 2020 6465 6620 6765 745f 7572 6928      def get_uri(
+00015c20: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+00015c30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00015c40: 662e 5f75 7269 0a0a 2020 2020 6465 6620  f._uri..    def 
+00015c50: 6765 745f 7061 7468 2873 656c 662c 202a  get_path(self, *
+00015c60: 7061 7468 3a20 7374 7229 202d 3e20 2742  path: str) -> 'B
+00015c70: 6c6f 6248 616e 646c 6527 3a0a 2020 2020  lobHandle':.    
+00015c80: 2020 2020 6966 2073 656c 662e 6973 5f66      if self.is_f
+00015c90: 756c 6c28 293a 0a20 2020 2020 2020 2020  ull():.         
+00015ca0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00015cb0: 726f 7228 6622 5552 4920 6d75 7374 206e  ror(f"URI must n
+00015cc0: 6f74 2062 6520 6675 6c6c 3a20 7b73 656c  ot be full: {sel
+00015cd0: 667d 2229 0a20 2020 2020 2020 2072 6574  f}").        ret
+00015ce0: 7572 6e20 426c 6f62 4861 6e64 6c65 280a  urn BlobHandle(.
+00015cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015d00: 2e5f 636c 6965 6e74 2c20 6622 7b73 656c  ._client, f"{sel
+00015d10: 662e 5f75 7269 7d2f 7b27 2f27 2e6a 6f69  f._uri}/{'/'.joi
+00015d20: 6e28 7061 7468 297d 222c 2069 735f 6675  n(path)}", is_fu
+00015d30: 6c6c 3d54 7275 6529 0a0a 2020 2020 6465  ll=True)..    de
+00015d40: 6620 6765 745f 7061 7265 6e74 2873 656c  f get_parent(sel
+00015d50: 6629 202d 3e20 2742 6c6f 6248 616e 646c  f) -> 'BlobHandl
+00015d60: 6527 3a0a 2020 2020 2020 2020 6966 2073  e':.        if s
+00015d70: 656c 662e 5f70 6172 656e 7420 6973 204e  elf._parent is N
+00015d80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00015d90: 2075 7269 203d 2075 726c 7061 7273 6528   uri = urlparse(
+00015da0: 7365 6c66 2e5f 7572 6929 0a20 2020 2020  self._uri).     
+00015db0: 2020 2020 2020 2070 6174 6820 3d20 5075         path = Pu
+00015dc0: 7265 5061 7468 282a 506f 7369 7850 6174  rePath(*PosixPat
+00015dd0: 6828 7572 692e 7061 7468 292e 7061 7274  h(uri.path).part
+00015de0: 735b 3a33 5d29 0a20 2020 2020 2020 2020  s[:3]).         
+00015df0: 2020 206e 6577 5f75 7269 203d 2075 726c     new_uri = url
+00015e00: 756e 7061 7273 6528 0a20 2020 2020 2020  unparse(.       
+00015e10: 2020 2020 2020 2020 2028 7572 692e 7363           (uri.sc
+00015e20: 6865 6d65 2c20 7572 692e 6e65 746c 6f63  heme, uri.netloc
+00015e30: 2c20 7061 7468 2e61 735f 706f 7369 7828  , path.as_posix(
+00015e40: 292c 204e 6f6e 652c 204e 6f6e 652c 204e  ), None, None, N
+00015e50: 6f6e 6529 290a 2020 2020 2020 2020 2020  one)).          
+00015e60: 2020 7265 7320 3d20 426c 6f62 4861 6e64    res = BlobHand
+00015e70: 6c65 2873 656c 662e 5f63 6c69 656e 742c  le(self._client,
+00015e80: 206e 6577 5f75 7269 2c20 6973 5f66 756c   new_uri, is_ful
+00015e90: 6c3d 4661 6c73 6529 0a20 2020 2020 2020  l=False).       
+00015ea0: 2020 2020 2073 656c 662e 5f70 6172 656e       self._paren
+00015eb0: 7420 3d20 7265 730a 2020 2020 2020 2020  t = res.        
+00015ec0: 7265 7475 726e 2073 656c 662e 5f70 6172  return self._par
+00015ed0: 656e 740a 0a20 2020 2064 6566 2067 6574  ent..    def get
+00015ee0: 5f63 7479 7065 2873 656c 6629 202d 3e20  _ctype(self) -> 
+00015ef0: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
+00015f00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00015f10: 6c66 2e5f 6374 7970 650a 0a20 2020 2064  lf._ctype..    d
+00015f20: 6566 2063 6c65 6172 5f69 6e66 6f5f 6361  ef clear_info_ca
+00015f30: 6368 6528 7365 6c66 2920 2d3e 204e 6f6e  che(self) -> Non
+00015f40: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
+00015f50: 5f69 6e66 6f20 3d20 4e6f 6e65 0a0a 2020  _info = None..  
+00015f60: 2020 6465 6620 6765 745f 696e 666f 2873    def get_info(s
+00015f70: 656c 6629 202d 3e20 4469 6374 5b73 7472  elf) -> Dict[str
+00015f80: 2c20 416e 795d 3a0a 2020 2020 2020 2020  , Any]:.        
+00015f90: 6966 2073 656c 662e 6973 5f66 756c 6c28  if self.is_full(
+00015fa0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00015fb0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00015fc0: 6622 5552 4920 6d75 7374 206e 6f74 2062  f"URI must not b
+00015fd0: 6520 6675 6c6c 3a20 7b73 656c 667d 2229  e full: {self}")
+00015fe0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00015ff0: 2e5f 696e 666f 2069 7320 4e6f 6e65 3a0a  ._info is None:.
+00016000: 2020 2020 2020 2020 2020 2020 696e 666f              info
+00016010: 203d 2073 656c 662e 6765 745f 7061 7468   = self.get_path
+00016020: 2822 696e 666f 2e6a 736f 6e22 292e 6765  ("info.json").ge
+00016030: 745f 636f 6e74 656e 7428 290a 2020 2020  t_content().    
+00016040: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00016050: 6e66 6f20 6973 206e 6f74 204e 6f6e 650a  nfo is not None.
+00016060: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016070: 2e5f 696e 666f 203d 2063 6173 7428 4469  ._info = cast(Di
+00016080: 6374 5b73 7472 2c20 416e 795d 2c20 696e  ct[str, Any], in
+00016090: 666f 290a 2020 2020 2020 2020 7265 7475  fo).        retu
+000160a0: 726e 2073 656c 662e 5f69 6e66 6f0a 0a20  rn self._info.. 
+000160b0: 2020 2064 6566 2067 6574 5f63 6f6e 7465     def get_conte
+000160c0: 6e74 2873 656c 6629 202d 3e20 4f70 7469  nt(self) -> Opti
+000160d0: 6f6e 616c 5b42 7974 6552 6573 706f 6e73  onal[ByteRespons
+000160e0: 655d 3a0a 2020 2020 2020 2020 6966 206e  e]:.        if n
+000160f0: 6f74 2073 656c 662e 6973 5f66 756c 6c28  ot self.is_full(
+00016100: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00016110: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00016120: 6622 5552 4920 6d75 7374 2062 6520 6675  f"URI must be fu
+00016130: 6c6c 3a20 7b73 656c 667d 2229 0a20 2020  ll: {self}").   
+00016140: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+00016150: 656d 7074 7928 293a 0a20 2020 2020 2020  empty():.       
+00016160: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00016170: 0a20 2020 2020 2020 2073 6c65 6570 5f74  .        sleep_t
+00016180: 696d 6520 3d20 302e 310a 2020 2020 2020  ime = 0.1.      
+00016190: 2020 736c 6565 705f 6d75 6c20 3d20 312e    sleep_mul = 1.
+000161a0: 310a 2020 2020 2020 2020 736c 6565 705f  1.        sleep_
+000161b0: 6d61 7820 3d20 352e 300a 2020 2020 2020  max = 5.0.      
+000161c0: 2020 746f 7461 6c5f 7469 6d65 203d 2036    total_time = 6
+000161d0: 302e 300a 2020 2020 2020 2020 7374 6172  0.0.        star
+000161e0: 745f 7469 6d65 203d 2074 696d 652e 6d6f  t_time = time.mo
+000161f0: 6e6f 746f 6e69 6328 290a 2020 2020 2020  notonic().      
+00016200: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+00016210: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00016220: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016230: 696e 2c20 6374 7970 6520 3d20 7365 6c66  in, ctype = self
+00016240: 2e5f 636c 6965 6e74 2e72 6571 7565 7374  ._client.request
+00016250: 5f62 7974 6573 280a 2020 2020 2020 2020  _bytes(.        
+00016260: 2020 2020 2020 2020 2020 2020 4d45 5448              METH
+00016270: 4f44 5f50 4f53 542c 2022 2f75 7269 222c  OD_POST, "/uri",
+00016280: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00016290: 2020 2020 2020 2020 2020 2022 7572 6922             "uri"
+000162a0: 3a20 7365 6c66 2e67 6574 5f75 7269 2829  : self.get_uri()
+000162b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000162c0: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
+000162d0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+000162e0: 7479 7065 203d 2063 7479 7065 0a20 2020  type = ctype.   
+000162f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00016300: 7572 6e20 696e 7465 7270 7265 745f 6374  urn interpret_ct
+00016310: 7970 6528 6669 6e2c 2063 7479 7065 290a  ype(fin, ctype).
+00016320: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00016330: 7074 2048 5454 5045 7272 6f72 2061 7320  pt HTTPError as 
+00016340: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00016350: 2020 2069 6620 652e 7265 7370 6f6e 7365     if e.response
+00016360: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
+00016370: 3430 343a 0a20 2020 2020 2020 2020 2020  404:.           
+00016380: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+00016390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000163a0: 2069 6620 7469 6d65 2e6d 6f6e 6f74 6f6e   if time.monoton
+000163b0: 6963 2829 202d 2073 7461 7274 5f74 696d  ic() - start_tim
+000163c0: 6520 3e3d 2074 6f74 616c 5f74 696d 653a  e >= total_time:
+000163d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000163e0: 2020 2020 2072 6169 7365 2065 0a20 2020       raise e.   
+000163f0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+00016400: 652e 736c 6565 7028 736c 6565 705f 7469  e.sleep(sleep_ti
+00016410: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00016420: 2020 2020 736c 6565 705f 7469 6d65 203d      sleep_time =
+00016430: 206d 696e 2873 6c65 6570 5f74 696d 6520   min(sleep_time 
+00016440: 2a20 736c 6565 705f 6d75 6c2c 2073 6c65  * sleep_mul, sle
+00016450: 6570 5f6d 6178 290a 0a20 2020 2064 6566  ep_max)..    def
+00016460: 206c 6973 745f 6669 6c65 7328 7365 6c66   list_files(self
+00016470: 2920 2d3e 204c 6973 745b 2742 6c6f 6248  ) -> List['BlobH
+00016480: 616e 646c 6527 5d3a 0a20 2020 2020 2020  andle']:.       
+00016490: 2069 6620 7365 6c66 2e69 735f 6675 6c6c   if self.is_full
+000164a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000164b0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000164c0: 2866 2255 5249 206d 7573 7420 6e6f 7420  (f"URI must not 
+000164d0: 6265 2066 756c 6c3a 207b 7365 6c66 7d22  be full: {self}"
+000164e0: 290a 2020 2020 2020 2020 7265 7370 203d  ).        resp =
+000164f0: 2063 6173 7428 426c 6f62 4669 6c65 7352   cast(BlobFilesR
+00016500: 6573 706f 6e73 652c 2073 656c 662e 5f63  esponse, self._c
+00016510: 6c69 656e 742e 7265 7175 6573 745f 6a73  lient.request_js
+00016520: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00016530: 4d45 5448 4f44 5f47 4554 2c20 222f 626c  METHOD_GET, "/bl
+00016540: 6f62 5f66 696c 6573 222c 207b 0a20 2020  ob_files", {.   
+00016550: 2020 2020 2020 2020 2020 2020 2022 626c               "bl
+00016560: 6f62 223a 2073 656c 662e 6765 745f 7572  ob": self.get_ur
+00016570: 6928 292c 0a20 2020 2020 2020 2020 2020  i(),.           
+00016580: 207d 2929 0a20 2020 2020 2020 2072 6574   })).        ret
+00016590: 7572 6e20 5b0a 2020 2020 2020 2020 2020  urn [.          
+000165a0: 2020 426c 6f62 4861 6e64 6c65 2873 656c    BlobHandle(sel
+000165b0: 662e 5f63 6c69 656e 742c 2062 6c6f 625f  f._client, blob_
+000165c0: 7572 692c 2069 735f 6675 6c6c 3d54 7275  uri, is_full=Tru
+000165d0: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
+000165e0: 6f72 2062 6c6f 625f 7572 6920 696e 2072  or blob_uri in r
+000165f0: 6573 705b 2266 696c 6573 225d 0a20 2020  esp["files"].   
+00016600: 2020 2020 205d 0a0a 2020 2020 6465 6620       ]..    def 
+00016610: 6173 5f73 7472 2873 656c 6629 202d 3e20  as_str(self) -> 
+00016620: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
+00016630: 7572 6e20 6622 7b73 656c 662e 6765 745f  urn f"{self.get_
+00016640: 7572 6928 297d 220a 0a20 2020 2064 6566  uri()}"..    def
+00016650: 2073 6574 5f6f 776e 6572 2873 656c 662c   set_owner(self,
+00016660: 206f 776e 6572 3a20 4e6f 6465 4861 6e64   owner: NodeHand
+00016670: 6c65 2920 2d3e 2042 6c6f 624f 776e 6572  le) -> BlobOwner
+00016680: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00016690: 662e 6973 5f66 756c 6c28 293a 0a20 2020  f.is_full():.   
+000166a0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000166b0: 616c 7565 4572 726f 7228 6622 5552 4920  alueError(f"URI 
+000166c0: 6d75 7374 206e 6f74 2062 6520 6675 6c6c  must not be full
+000166d0: 3a20 7b73 656c 667d 2229 0a20 2020 2020  : {self}").     
+000166e0: 2020 2072 6574 7572 6e20 6361 7374 2842     return cast(B
+000166f0: 6c6f 624f 776e 6572 2c20 7365 6c66 2e5f  lobOwner, self._
+00016700: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
+00016710: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00016720: 204d 4554 484f 445f 5055 542c 2022 2f62   METHOD_PUT, "/b
+00016730: 6c6f 625f 6f77 6e65 7222 2c20 7b0a 2020  lob_owner", {.  
+00016740: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00016750: 6c6f 6222 3a20 7365 6c66 2e67 6574 5f75  lob": self.get_u
+00016760: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
+00016770: 2020 2020 2020 226f 776e 6572 5f64 6167        "owner_dag
+00016780: 223a 206f 776e 6572 2e67 6574 5f64 6167  ": owner.get_dag
+00016790: 2829 2e67 6574 5f75 7269 2829 2c0a 2020  ().get_uri(),.  
+000167a0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+000167b0: 776e 6572 5f6e 6f64 6522 3a20 6f77 6e65  wner_node": owne
+000167c0: 722e 6765 745f 6964 2829 2c0a 2020 2020  r.get_id(),.    
+000167d0: 2020 2020 2020 2020 7d29 290a 0a20 2020          }))..   
+000167e0: 2064 6566 2067 6574 5f6f 776e 6572 2873   def get_owner(s
+000167f0: 656c 6629 202d 3e20 426c 6f62 4f77 6e65  elf) -> BlobOwne
+00016800: 723a 0a20 2020 2020 2020 2069 6620 7365  r:.        if se
+00016810: 6c66 2e5f 6f77 6e65 7220 6973 204e 6f6e  lf._owner is Non
+00016820: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00016830: 656c 662e 5f6f 776e 6572 203d 2073 656c  elf._owner = sel
+00016840: 662e 5f63 6c69 656e 742e 6765 745f 626c  f._client.get_bl
+00016850: 6f62 5f6f 776e 6572 2873 656c 662e 6765  ob_owner(self.ge
+00016860: 745f 7572 6928 2929 0a20 2020 2020 2020  t_uri()).       
+00016870: 2072 6574 7572 6e20 7365 6c66 2e5f 6f77   return self._ow
+00016880: 6e65 720a 0a20 2020 2064 6566 2073 6574  ner..    def set
+00016890: 5f6c 6f63 616c 5f6f 776e 6572 2873 656c  _local_owner(sel
+000168a0: 662c 206f 776e 6572 3a20 426c 6f62 4f77  f, owner: BlobOw
+000168b0: 6e65 7229 202d 3e20 4e6f 6e65 3a0a 2020  ner) -> None:.  
+000168c0: 2020 2020 2020 7365 6c66 2e5f 6f77 6e65        self._owne
+000168d0: 7220 3d20 6f77 6e65 720a 0a20 2020 2064  r = owner..    d
+000168e0: 6566 2067 6574 5f6f 776e 6572 5f64 6167  ef get_owner_dag
+000168f0: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00016900: 616c 5b73 7472 5d3a 0a20 2020 2020 2020  al[str]:.       
+00016910: 206f 776e 6572 203d 2073 656c 662e 6765   owner = self.ge
+00016920: 745f 6f77 6e65 7228 290a 2020 2020 2020  t_owner().      
+00016930: 2020 7265 7475 726e 206f 776e 6572 5b22    return owner["
+00016940: 6f77 6e65 725f 6461 6722 5d0a 0a20 2020  owner_dag"]..   
+00016950: 2064 6566 2067 6574 5f6f 776e 6572 5f6e   def get_owner_n
+00016960: 6f64 6528 7365 6c66 2920 2d3e 2073 7472  ode(self) -> str
+00016970: 3a0a 2020 2020 2020 2020 6f77 6e65 7220  :.        owner 
+00016980: 3d20 7365 6c66 2e67 6574 5f6f 776e 6572  = self.get_owner
+00016990: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000169a0: 6e20 6f77 6e65 725b 226f 776e 6572 5f6e  n owner["owner_n
+000169b0: 6f64 6522 5d0a 0a20 2020 2064 6566 2073  ode"]..    def s
+000169c0: 6574 5f6d 6f64 656c 5f74 6872 6573 686f  et_model_thresho
+000169d0: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+000169e0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+000169f0: 2020 7468 7265 7368 6f6c 643a 2066 6c6f    threshold: flo
+00016a00: 6174 2c0a 2020 2020 2020 2020 2020 2020  at,.            
+00016a10: 706f 735f 6c61 6265 6c3a 2073 7472 2920  pos_label: str) 
+00016a20: 2d3e 204d 6f64 656c 496e 666f 3a0a 2020  -> ModelInfo:.  
+00016a30: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00016a40: 7428 4d6f 6465 6c49 6e66 6f2c 2073 656c  t(ModelInfo, sel
+00016a50: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+00016a60: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+00016a70: 2020 2020 4d45 5448 4f44 5f50 5554 2c20      METHOD_PUT, 
+00016a80: 222f 7468 7265 7368 6f6c 6422 2c20 7b0a  "/threshold", {.
+00016a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016aa0: 2262 6c6f 6222 3a20 7365 6c66 2e67 6574  "blob": self.get
+00016ab0: 5f75 7269 2829 2c0a 2020 2020 2020 2020  _uri(),.        
+00016ac0: 2020 2020 2020 2020 2274 6872 6573 686f          "thresho
+00016ad0: 6c64 223a 2074 6872 6573 686f 6c64 2c0a  ld": threshold,.
+00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016af0: 2270 6f73 5f6c 6162 656c 223a 2070 6f73  "pos_label": pos
+00016b00: 5f6c 6162 656c 2c0a 2020 2020 2020 2020  _label,.        
+00016b10: 2020 2020 7d29 290a 0a20 2020 2064 6566      }))..    def
+00016b20: 2064 656c 5f6d 6f64 656c 5f74 6872 6573   del_model_thres
+00016b30: 686f 6c64 2873 656c 6629 202d 3e20 4d6f  hold(self) -> Mo
+00016b40: 6465 6c49 6e66 6f3a 0a20 2020 2020 2020  delInfo:.       
+00016b50: 2072 6574 7572 6e20 6361 7374 284d 6f64   return cast(Mod
+00016b60: 656c 496e 666f 2c20 7365 6c66 2e5f 636c  elInfo, self._cl
+00016b70: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
+00016b80: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
+00016b90: 4554 484f 445f 4445 4c45 5445 2c20 222f  ETHOD_DELETE, "/
+00016ba0: 7468 7265 7368 6f6c 6422 2c20 7b0a 2020  threshold", {.  
+00016bb0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00016bc0: 6c6f 6222 3a20 7365 6c66 2e67 6574 5f75  lob": self.get_u
+00016bd0: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
+00016be0: 2020 7d29 290a 0a20 2020 2064 6566 2067    }))..    def g
+00016bf0: 6574 5f6d 6f64 656c 5f69 6e66 6f28 7365  et_model_info(se
+00016c00: 6c66 2920 2d3e 204d 6f64 656c 496e 666f  lf) -> ModelInfo
+00016c10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00016c20: 2063 6173 7428 4d6f 6465 6c49 6e66 6f2c   cast(ModelInfo,
+00016c30: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
+00016c40: 7175 6573 745f 6a73 6f6e 280a 2020 2020  quest_json(.    
+00016c50: 2020 2020 2020 2020 4d45 5448 4f44 5f47          METHOD_G
+00016c60: 4554 2c20 222f 6d6f 6465 6c5f 696e 666f  ET, "/model_info
+00016c70: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+00016c80: 2020 2020 2022 626c 6f62 223a 2073 656c       "blob": sel
+00016c90: 662e 6765 745f 7572 6928 292c 0a20 2020  f.get_uri(),.   
+00016ca0: 2020 2020 2020 2020 207d 2929 0a0a 2020           }))..  
+00016cb0: 2020 6465 6620 636f 7079 5f74 6f28 0a20    def copy_to(. 
+00016cc0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00016cd0: 0a20 2020 2020 2020 2020 2020 2074 6f5f  .            to_
+00016ce0: 7572 693a 2073 7472 2c0a 2020 2020 2020  uri: str,.      
+00016cf0: 2020 2020 2020 6e65 775f 6f77 6e65 723a        new_owner:
+00016d00: 204f 7074 696f 6e61 6c5b 4e6f 6465 4861   Optional[NodeHa
+00016d10: 6e64 6c65 5d20 3d20 4e6f 6e65 2c0a 2020  ndle] = None,.  
+00016d20: 2020 2020 2020 2020 2020 6578 7465 726e            extern
+00016d30: 616c 5f6f 776e 6572 3a20 626f 6f6c 203d  al_owner: bool =
+00016d40: 2046 616c 7365 2920 2d3e 2027 426c 6f62   False) -> 'Blob
+00016d50: 4861 6e64 6c65 273a 0a20 2020 2020 2020  Handle':.       
+00016d60: 2069 6620 7365 6c66 2e69 735f 6675 6c6c   if self.is_full
+00016d70: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00016d80: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00016d90: 2866 2255 5249 206d 7573 7420 6e6f 7420  (f"URI must not 
+00016da0: 6265 2066 756c 6c3a 207b 7365 6c66 7d22  be full: {self}"
+00016db0: 290a 0a20 2020 2020 2020 206f 776e 6572  )..        owner
+00016dc0: 5f64 6167 203d 205c 0a20 2020 2020 2020  _dag = \.       
+00016dd0: 2020 2020 204e 6f6e 6520 6966 206e 6577       None if new
+00016de0: 5f6f 776e 6572 2069 7320 4e6f 6e65 2065  _owner is None e
+00016df0: 6c73 6520 6e65 775f 6f77 6e65 722e 6765  lse new_owner.ge
+00016e00: 745f 6461 6728 292e 6765 745f 7572 6928  t_dag().get_uri(
+00016e10: 290a 2020 2020 2020 2020 6f77 6e65 725f  ).        owner_
+00016e20: 6e6f 6465 203d 204e 6f6e 6520 6966 206e  node = None if n
+00016e30: 6577 5f6f 776e 6572 2069 7320 4e6f 6e65  ew_owner is None
+00016e40: 2065 6c73 6520 6e65 775f 6f77 6e65 722e   else new_owner.
+00016e50: 6765 745f 6964 2829 0a20 2020 2020 2020  get_id().       
+00016e60: 2072 6573 203d 2063 6173 7428 436f 7079   res = cast(Copy
+00016e70: 426c 6f62 2c20 7365 6c66 2e5f 636c 6965  Blob, self._clie
+00016e80: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
+00016e90: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+00016ea0: 484f 445f 504f 5354 2c20 222f 636f 7079  HOD_POST, "/copy
+00016eb0: 5f62 6c6f 6222 2c20 7b0a 2020 2020 2020  _blob", {.      
+00016ec0: 2020 2020 2020 2020 2020 2266 726f 6d5f            "from_
+00016ed0: 7572 6922 3a20 7365 6c66 2e67 6574 5f75  uri": self.get_u
+00016ee0: 7269 2829 2c0a 2020 2020 2020 2020 2020  ri(),.          
+00016ef0: 2020 2020 2020 226f 776e 6572 5f64 6167        "owner_dag
+00016f00: 223a 206f 776e 6572 5f64 6167 2c0a 2020  ": owner_dag,.  
+00016f10: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+00016f20: 776e 6572 5f6e 6f64 6522 3a20 6f77 6e65  wner_node": owne
+00016f30: 725f 6e6f 6465 2c0a 2020 2020 2020 2020  r_node,.        
+00016f40: 2020 2020 2020 2020 2265 7874 6572 6e61          "externa
+00016f50: 6c5f 6f77 6e65 7222 3a20 6578 7465 726e  l_owner": extern
+00016f60: 616c 5f6f 776e 6572 2c0a 2020 2020 2020  al_owner,.      
+00016f70: 2020 2020 2020 2020 2020 2274 6f5f 7572            "to_ur
+00016f80: 6922 3a20 746f 5f75 7269 2c0a 2020 2020  i": to_uri,.    
+00016f90: 2020 2020 2020 2020 7d29 290a 2020 2020          })).    
+00016fa0: 2020 2020 7265 7475 726e 2042 6c6f 6248      return BlobH
+00016fb0: 616e 646c 6528 7365 6c66 2e5f 636c 6965  andle(self._clie
+00016fc0: 6e74 2c20 7265 735b 226e 6577 5f75 7269  nt, res["new_uri
+00016fd0: 225d 2c20 6973 5f66 756c 6c3d 4661 6c73  "], is_full=Fals
+00016fe0: 6529 0a0a 2020 2020 6465 6620 646f 776e  e)..    def down
+00016ff0: 6c6f 6164 5f7a 6970 2873 656c 662c 2074  load_zip(self, t
+00017000: 6f5f 7061 7468 3a20 4f70 7469 6f6e 616c  o_path: Optional
+00017010: 5b73 7472 5d29 202d 3e20 4f70 7469 6f6e  [str]) -> Option
+00017020: 616c 5b69 6f2e 4279 7465 7349 4f5d 3a0a  al[io.BytesIO]:.
+00017030: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00017040: 6973 5f66 756c 6c28 293a 0a20 2020 2020  is_full():.     
+00017050: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00017060: 7565 4572 726f 7228 6622 5552 4920 6d75  ueError(f"URI mu
+00017070: 7374 206e 6f74 2062 6520 6675 6c6c 3a20  st not be full: 
+00017080: 7b73 656c 667d 2229 0a20 2020 2020 2020  {self}").       
+00017090: 2063 7572 5f72 6573 2c20 5f20 3d20 7365   cur_res, _ = se
+000170a0: 6c66 2e5f 636c 6965 6e74 2e72 6571 7565  lf._client.reque
+000170b0: 7374 5f62 7974 6573 280a 2020 2020 2020  st_bytes(.      
+000170c0: 2020 2020 2020 4d45 5448 4f44 5f47 4554        METHOD_GET
+000170d0: 2c20 222f 646f 776e 6c6f 6164 5f7a 6970  , "/download_zip
+000170e0: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+000170f0: 2020 2020 2022 626c 6f62 223a 2073 656c       "blob": sel
+00017100: 662e 6765 745f 7572 6928 292c 0a20 2020  f.get_uri(),.   
+00017110: 2020 2020 2020 2020 207d 290a 2020 2020           }).    
+00017120: 2020 2020 6966 2074 6f5f 7061 7468 2069      if to_path i
+00017130: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00017140: 2020 2020 7265 7475 726e 2069 6f2e 4279      return io.By
+00017150: 7465 7349 4f28 6375 725f 7265 732e 7265  tesIO(cur_res.re
+00017160: 6164 2829 290a 2020 2020 2020 2020 7769  ad()).        wi
+00017170: 7468 206f 7065 6e28 746f 5f70 6174 682c  th open(to_path,
+00017180: 2022 7762 2229 2061 7320 6669 6c65 5f64   "wb") as file_d
+00017190: 6f77 6e6c 6f61 643a 0a20 2020 2020 2020  ownload:.       
+000171a0: 2020 2020 2066 696c 655f 646f 776e 6c6f       file_downlo
+000171b0: 6164 2e77 7269 7465 2863 7572 5f72 6573  ad.write(cur_res
+000171c0: 2e72 6561 6428 2929 0a20 2020 2020 2020  .read()).       
+000171d0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+000171e0: 2020 6465 6620 5f70 6572 666f 726d 5f75    def _perform_u
+000171f0: 706c 6f61 645f 6163 7469 6f6e 280a 2020  pload_action(.  
+00017200: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+00017210: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+00017220: 6f6e 3a20 7374 722c 0a20 2020 2020 2020  on: str,.       
+00017230: 2020 2020 2061 6464 6974 696f 6e61 6c3a       additional:
+00017240: 2044 6963 745b 7374 722c 2055 6e69 6f6e   Dict[str, Union
+00017250: 5b73 7472 2c20 696e 742c 204c 6973 745b  [str, int, List[
+00017260: 696e 745d 5d5d 2c0a 2020 2020 2020 2020  int]]],.        
+00017270: 2020 2020 666f 626a 3a20 4f70 7469 6f6e      fobj: Option
+00017280: 616c 5b49 4f5b 6279 7465 735d 5d29 202d  al[IO[bytes]]) -
+00017290: 3e20 5570 6c6f 6164 4669 6c65 7352 6573  > UploadFilesRes
+000172a0: 706f 6e73 653a 0a20 2020 2020 2020 2061  ponse:.        a
+000172b0: 7267 733a 2044 6963 745b 7374 722c 2055  rgs: Dict[str, U
+000172c0: 6e69 6f6e 5b73 7472 2c20 696e 742c 204c  nion[str, int, L
+000172d0: 6973 745b 696e 745d 5d5d 203d 207b 0a20  ist[int]]] = {. 
+000172e0: 2020 2020 2020 2020 2020 2022 6163 7469             "acti
+000172f0: 6f6e 223a 2061 6374 696f 6e2c 0a20 2020  on": action,.   
+00017300: 2020 2020 207d 0a20 2020 2020 2020 2061       }.        a
+00017310: 7267 732e 7570 6461 7465 2861 6464 6974  rgs.update(addit
+00017320: 696f 6e61 6c29 0a20 2020 2020 2020 2069  ional).        i
+00017330: 6620 666f 626a 2069 7320 6e6f 7420 4e6f  f fobj is not No
+00017340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00017350: 6d65 7468 6f64 203d 204d 4554 484f 445f  method = METHOD_
+00017360: 4649 4c45 0a20 2020 2020 2020 2020 2020  FILE.           
+00017370: 2066 696c 6573 3a20 4f70 7469 6f6e 616c   files: Optional
+00017380: 5b44 6963 745b 7374 722c 2049 4f5b 6279  [Dict[str, IO[by
+00017390: 7465 735d 5d5d 203d 207b 0a20 2020 2020  tes]]] = {.     
+000173a0: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+000173b0: 223a 2066 6f62 6a2c 0a20 2020 2020 2020  ": fobj,.       
+000173c0: 2020 2020 207d 0a20 2020 2020 2020 2065       }.        e
+000173d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000173e0: 206d 6574 686f 6420 3d20 4d45 5448 4f44   method = METHOD
+000173f0: 5f50 4f53 540a 2020 2020 2020 2020 2020  _POST.          
+00017400: 2020 6669 6c65 7320 3d20 4e6f 6e65 0a20    files = None. 
+00017410: 2020 2020 2020 2069 6620 6163 7469 6f6e         if action
+00017420: 203d 3d20 2263 6c65 6172 223a 0a20 2020   == "clear":.   
+00017430: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+00017440: 6d70 5f75 7269 203d 204e 6f6e 650a 2020  mp_uri = None.  
+00017450: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00017460: 7428 5570 6c6f 6164 4669 6c65 7352 6573  t(UploadFilesRes
+00017470: 706f 6e73 652c 2073 656c 662e 5f63 6c69  ponse, self._cli
+00017480: 656e 742e 7265 7175 6573 745f 6a73 6f6e  ent.request_json
+00017490: 280a 2020 2020 2020 2020 2020 2020 6d65  (.            me
+000174a0: 7468 6f64 2c20 222f 7570 6c6f 6164 5f66  thod, "/upload_f
+000174b0: 696c 6522 2c20 6172 6773 2c20 6669 6c65  ile", args, file
+000174c0: 733d 6669 6c65 7329 290a 0a20 2020 2064  s=files))..    d
+000174d0: 6566 205f 7374 6172 745f 7570 6c6f 6164  ef _start_upload
+000174e0: 2873 656c 662c 2073 697a 653a 2069 6e74  (self, size: int
+000174f0: 2c20 6861 7368 5f73 7472 3a20 7374 722c  , hash_str: str,
+00017500: 2065 7874 3a20 7374 7229 202d 3e20 7374   ext: str) -> st
+00017510: 723a 0a20 2020 2020 2020 2072 6573 203d  r:.        res =
+00017520: 2073 656c 662e 5f70 6572 666f 726d 5f75   self._perform_u
+00017530: 706c 6f61 645f 6163 7469 6f6e 280a 2020  pload_action(.  
+00017540: 2020 2020 2020 2020 2020 2273 7461 7274            "start
+00017550: 222c 0a20 2020 2020 2020 2020 2020 207b  ",.            {
+00017560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017570: 2022 7461 7267 6574 223a 2073 656c 662e   "target": self.
+00017580: 6765 745f 7572 6928 292c 0a20 2020 2020  get_uri(),.     
+00017590: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+000175a0: 223a 2068 6173 685f 7374 722c 0a20 2020  ": hash_str,.   
+000175b0: 2020 2020 2020 2020 2020 2020 2022 7369               "si
+000175c0: 7a65 223a 2073 697a 652c 0a20 2020 2020  ze": size,.     
+000175d0: 2020 2020 2020 2020 2020 2022 6578 7422             "ext"
+000175e0: 3a20 6578 742c 0a20 2020 2020 2020 2020  : ext,.         
+000175f0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00017600: 2020 666f 626a 3d4e 6f6e 6529 0a20 2020    fobj=None).   
+00017610: 2020 2020 2061 7373 6572 7420 7265 735b       assert res[
+00017620: 2275 7269 225d 2069 7320 6e6f 7420 4e6f  "uri"] is not No
+00017630: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+00017640: 6e20 7265 735b 2275 7269 225d 0a0a 2020  n res["uri"]..  
+00017650: 2020 6465 6620 5f6c 6567 6163 795f 6170    def _legacy_ap
+00017660: 7065 6e64 5f75 706c 6f61 6428 0a20 2020  pend_upload(.   
+00017670: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00017680: 2020 2020 2020 2020 2020 2075 7269 3a20             uri: 
+00017690: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+000176a0: 2066 6f62 6a3a 2049 4f5b 6279 7465 735d   fobj: IO[bytes]
+000176b0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+000176c0: 2020 7265 7320 3d20 7365 6c66 2e5f 7065    res = self._pe
+000176d0: 7266 6f72 6d5f 7570 6c6f 6164 5f61 6374  rform_upload_act
+000176e0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+000176f0: 2022 6170 7065 6e64 222c 207b 2275 7269   "append", {"uri
+00017700: 223a 2075 7269 7d2c 2066 6f62 6a3d 666f  ": uri}, fobj=fo
+00017710: 626a 290a 2020 2020 2020 2020 7265 7475  bj).        retu
+00017720: 726e 2072 6573 5b22 706f 7322 5d0a 0a20  rn res["pos"].. 
+00017730: 2020 2064 6566 205f 6170 7065 6e64 5f75     def _append_u
+00017740: 706c 6f61 6428 0a20 2020 2020 2020 2020  pload(.         
+00017750: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00017760: 2020 2020 2075 7269 3a20 7374 722c 0a20       uri: str,. 
+00017770: 2020 2020 2020 2020 2020 2066 6f62 6a3a             fobj:
+00017780: 2049 4f5b 6279 7465 735d 2c0a 2020 2020   IO[bytes],.    
+00017790: 2020 2020 2020 2020 6f66 6673 6574 3a20          offset: 
+000177a0: 696e 7429 202d 3e20 696e 743a 0a20 2020  int) -> int:.   
+000177b0: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+000177c0: 5f70 6572 666f 726d 5f75 706c 6f61 645f  _perform_upload_
+000177d0: 6163 7469 6f6e 280a 2020 2020 2020 2020  action(.        
+000177e0: 2020 2020 2261 7070 656e 6422 2c20 7b22      "append", {"
+000177f0: 7572 6922 3a20 7572 692c 2022 6f66 6673  uri": uri, "offs
+00017800: 6574 223a 206f 6666 7365 747d 2c20 666f  et": offset}, fo
+00017810: 626a 3d66 6f62 6a29 0a20 2020 2020 2020  bj=fobj).       
+00017820: 2072 6574 7572 6e20 7265 735b 2270 6f73   return res["pos
+00017830: 225d 0a0a 2020 2020 6465 6620 5f66 696e  "]..    def _fin
+00017840: 6973 685f 7570 6c6f 6164 5f7a 6970 2873  ish_upload_zip(s
+00017850: 656c 6629 202d 3e20 4c69 7374 5b73 7472  elf) -> List[str
+00017860: 5d3a 0a20 2020 2020 2020 2075 7269 203d  ]:.        uri =
+00017870: 2073 656c 662e 5f74 6d70 5f75 7269 0a20   self._tmp_uri. 
+00017880: 2020 2020 2020 2069 6620 7572 6920 6973         if uri is
+00017890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000178a0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000178b0: 726f 7228 2274 6d70 5f75 7269 2069 7320  ror("tmp_uri is 
+000178c0: 4e6f 6e65 2229 0a20 2020 2020 2020 2072  None").        r
+000178d0: 6573 203d 2063 6173 7428 5570 6c6f 6164  es = cast(Upload
+000178e0: 4669 6c65 7352 6573 706f 6e73 652c 2073  FilesResponse, s
+000178f0: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
+00017900: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
+00017910: 2020 2020 2020 4d45 5448 4f44 5f50 4f53        METHOD_POS
+00017920: 542c 2022 2f66 696e 6973 685f 7a69 7022  T, "/finish_zip"
+00017930: 2c20 7b22 7572 6922 3a20 7572 697d 2929  , {"uri": uri}))
+00017940: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017950: 7265 735b 2266 696c 6573 225d 0a0a 2020  res["files"]..  
+00017960: 2020 6465 6620 5f66 696e 6973 685f 6d6f    def _finish_mo
+00017970: 6465 6c5f 7570 6c6f 6164 280a 2020 2020  del_upload(.    
+00017980: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00017990: 2020 2020 2020 2020 2020 7863 6f6c 733a            xcols:
+000179a0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+000179b0: 7472 5d5d 2c0a 2020 2020 2020 2020 2020  tr]],.          
+000179c0: 2020 7963 6f6c 733a 204f 7074 696f 6e61    ycols: Optiona
+000179d0: 6c5b 4c69 7374 5b73 7472 5d5d 2c0a 2020  l[List[str]],.  
+000179e0: 2020 2020 2020 2020 2020 6973 5f63 6c66            is_clf
+000179f0: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
+00017a00: 2020 2020 6d6f 6465 6c5f 6e61 6d65 3a20      model_name: 
+00017a10: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+00017a20: 2076 6572 7369 6f6e 3a20 696e 742c 0a20   version: int,. 
+00017a30: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+00017a40: 5f70 6172 616d 733a 2044 6963 745b 7374  _params: Dict[st
+00017a50: 722c 2041 6e79 5d2c 0a20 2020 2020 2020  r, Any],.       
+00017a60: 2020 2020 2064 656c 6574 655f 6c61 7465       delete_late
+00017a70: 725f 7665 7273 696f 6e73 3a20 626f 6f6c  r_versions: bool
+00017a80: 2c0a 2020 2020 2020 2020 2020 2020 6675  ,.            fu
+00017a90: 6c6c 5f69 6e69 743a 2062 6f6f 6c29 202d  ll_init: bool) -
+00017aa0: 3e20 5570 6c6f 6164 4669 6c65 7352 6573  > UploadFilesRes
+00017ab0: 706f 6e73 653a 0a20 2020 2020 2020 2075  ponse:.        u
+00017ac0: 7269 203d 2073 656c 662e 5f74 6d70 5f75  ri = self._tmp_u
+00017ad0: 7269 0a20 2020 2020 2020 2069 6620 7572  ri.        if ur
+00017ae0: 6920 6973 204e 6f6e 653a 0a20 2020 2020  i is None:.     
+00017af0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00017b00: 7565 4572 726f 7228 2274 6d70 5f75 7269  ueError("tmp_uri
+00017b10: 2069 7320 4e6f 6e65 2229 0a20 2020 2020   is None").     
+00017b20: 2020 2072 6574 7572 6e20 6361 7374 2855     return cast(U
+00017b30: 706c 6f61 6446 696c 6573 5265 7370 6f6e  ploadFilesRespon
+00017b40: 7365 2c20 7365 6c66 2e5f 636c 6965 6e74  se, self._client
+00017b50: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+00017b60: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+00017b70: 445f 504f 5354 2c20 222f 6669 6e69 7368  D_POST, "/finish
+00017b80: 5f6d 6f64 656c 5f75 706c 6f61 6422 2c20  _model_upload", 
+00017b90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00017ba0: 2020 226d 6f64 656c 5f70 6172 616d 7322    "model_params"
+00017bb0: 3a20 6d6f 6465 6c5f 7061 7261 6d73 2c0a  : model_params,.
+00017bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bd0: 2266 756c 6c5f 696e 6974 223a 2066 756c  "full_init": ful
+00017be0: 6c5f 696e 6974 2c0a 2020 2020 2020 2020  l_init,.        
+00017bf0: 2020 2020 2020 2020 2269 735f 636c 6622          "is_clf"
+00017c00: 3a20 6973 5f63 6c66 2c0a 2020 2020 2020  : is_clf,.      
+00017c10: 2020 2020 2020 2020 2020 226d 6f64 656c            "model
+00017c20: 5f75 7269 223a 2073 656c 662e 6765 745f  _uri": self.get_
+00017c30: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
+00017c40: 2020 2020 2020 2022 6d6f 6465 6c5f 6e61         "model_na
+00017c50: 6d65 223a 206d 6f64 656c 5f6e 616d 652c  me": model_name,
+00017c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c70: 2022 7665 7273 696f 6e22 3a20 7665 7273   "version": vers
+00017c80: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00017c90: 2020 2020 2022 6f77 6e65 725f 6461 6722       "owner_dag"
+00017ca0: 3a20 7365 6c66 2e67 6574 5f6f 776e 6572  : self.get_owner
+00017cb0: 5f64 6167 2829 2c0a 2020 2020 2020 2020  _dag(),.        
+00017cc0: 2020 2020 2020 2020 226f 776e 6572 5f6e          "owner_n
+00017cd0: 6f64 6522 3a20 7365 6c66 2e67 6574 5f6f  ode": self.get_o
+00017ce0: 776e 6572 5f6e 6f64 6528 292c 0a20 2020  wner_node(),.   
+00017cf0: 2020 2020 2020 2020 2020 2020 2022 746d               "tm
+00017d00: 705f 7572 6922 3a20 7572 692c 0a20 2020  p_uri": uri,.   
+00017d10: 2020 2020 2020 2020 2020 2020 2022 7863               "xc
+00017d20: 6f6c 7322 3a20 7863 6f6c 732c 0a20 2020  ols": xcols,.   
+00017d30: 2020 2020 2020 2020 2020 2020 2022 7963               "yc
+00017d40: 6f6c 7322 3a20 7963 6f6c 732c 0a20 2020  ols": ycols,.   
+00017d50: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00017d60: 6c65 7465 5f6c 6174 6572 5f76 6572 7369  lete_later_versi
+00017d70: 6f6e 7322 3a20 6465 6c65 7465 5f6c 6174  ons": delete_lat
+00017d80: 6572 5f76 6572 7369 6f6e 732c 0a20 2020  er_versions,.   
+00017d90: 2020 2020 2020 2020 207d 2929 0a0a 2020           }))..  
+00017da0: 2020 6465 6620 5f63 6c65 6172 5f75 706c    def _clear_upl
+00017db0: 6f61 6428 7365 6c66 2920 2d3e 204e 6f6e  oad(self) -> Non
+00017dc0: 653a 0a20 2020 2020 2020 2075 7269 203d  e:.        uri =
+00017dd0: 2073 656c 662e 5f74 6d70 5f75 7269 0a20   self._tmp_uri. 
+00017de0: 2020 2020 2020 2069 6620 7572 6920 6973         if uri is
+00017df0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00017e00: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00017e10: 726f 7228 2274 6d70 5f75 7269 2069 7320  ror("tmp_uri is 
+00017e20: 4e6f 6e65 2229 0a20 2020 2020 2020 2073  None").        s
+00017e30: 656c 662e 5f70 6572 666f 726d 5f75 706c  elf._perform_upl
+00017e40: 6f61 645f 6163 7469 6f6e 2822 636c 6561  oad_action("clea
+00017e50: 7222 2c20 7b22 7572 6922 3a20 7572 697d  r", {"uri": uri}
+00017e60: 2c20 666f 626a 3d4e 6f6e 6529 0a0a 2020  , fobj=None)..  
+00017e70: 2020 6465 6620 5f6c 6567 6163 795f 7570    def _legacy_up
+00017e80: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
+00017e90: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00017ea0: 2020 2020 2020 2020 2066 696c 655f 636f           file_co
+00017eb0: 6e74 656e 743a 2049 4f5b 6279 7465 735d  ntent: IO[bytes]
+00017ec0: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00017ed0: 743a 2073 7472 2c0a 2020 2020 2020 2020  t: str,.        
+00017ee0: 2020 2020 7072 6f67 7265 7373 5f62 6172      progress_bar
+00017ef0: 3a20 4f70 7469 6f6e 616c 5b49 4f5b 416e  : Optional[IO[An
+00017f00: 795d 5d20 3d20 7379 732e 7374 646f 7574  y]] = sys.stdout
+00017f10: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00017f20: 2020 2069 6e69 745f 706f 7320 3d20 6669     init_pos = fi
+00017f30: 6c65 5f63 6f6e 7465 6e74 2e73 6565 6b28  le_content.seek(
+00017f40: 302c 2069 6f2e 5345 454b 5f43 5552 290a  0, io.SEEK_CUR).
+00017f50: 2020 2020 2020 2020 6669 6c65 5f68 6173          file_has
+00017f60: 6820 3d20 6765 745f 6669 6c65 5f68 6173  h = get_file_has
+00017f70: 6828 6669 6c65 5f63 6f6e 7465 6e74 290a  h(file_content).
+00017f80: 2020 2020 2020 2020 746f 7461 6c5f 7369          total_si
+00017f90: 7a65 203d 2066 696c 655f 636f 6e74 656e  ze = file_conten
+00017fa0: 742e 7365 656b 2830 2c20 696f 2e53 4545  t.seek(0, io.SEE
+00017fb0: 4b5f 454e 4429 202d 2069 6e69 745f 706f  K_END) - init_po
+00017fc0: 730a 2020 2020 2020 2020 6669 6c65 5f63  s.        file_c
+00017fd0: 6f6e 7465 6e74 2e73 6565 6b28 696e 6974  ontent.seek(init
+00017fe0: 5f70 6f73 2c20 696f 2e53 4545 4b5f 5345  _pos, io.SEEK_SE
+00017ff0: 5429 0a20 2020 2020 2020 2069 6620 7072  T).        if pr
+00018000: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+00018010: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00018020: 2020 2020 7072 6f67 7265 7373 5f62 6172      progress_bar
+00018030: 2e77 7269 7465 2822 5570 6c6f 6164 696e  .write("Uploadin
+00018040: 6720 6669 6c65 3a5c 6e22 290a 2020 2020  g file:\n").    
+00018050: 2020 2020 7072 696e 745f 7072 6f67 7265      print_progre
+00018060: 7373 203d 2067 6574 5f70 726f 6772 6573  ss = get_progres
+00018070: 735f 6261 7228 6f75 743d 7072 6f67 7265  s_bar(out=progre
+00018080: 7373 5f62 6172 290a 2020 2020 2020 2020  ss_bar).        
+00018090: 746d 705f 7572 6920 3d20 7365 6c66 2e5f  tmp_uri = self._
+000180a0: 7374 6172 745f 7570 6c6f 6164 2874 6f74  start_upload(tot
+000180b0: 616c 5f73 697a 652c 2066 696c 655f 6861  al_size, file_ha
+000180c0: 7368 2c20 6578 7429 0a20 2020 2020 2020  sh, ext).       
+000180d0: 2073 656c 662e 5f74 6d70 5f75 7269 203d   self._tmp_uri =
+000180e0: 2074 6d70 5f75 7269 0a20 2020 2020 2020   tmp_uri.       
+000180f0: 2063 7572 5f73 697a 6520 3d20 300a 2020   cur_size = 0.  
+00018100: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+00018110: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00018120: 696e 745f 7072 6f67 7265 7373 2863 7572  int_progress(cur
+00018130: 5f73 697a 6520 2f20 746f 7461 6c5f 7369  _size / total_si
+00018140: 7a65 2c20 4661 6c73 6529 0a20 2020 2020  ze, False).     
+00018150: 2020 2020 2020 2062 7566 6620 3d20 6669         buff = fi
+00018160: 6c65 5f63 6f6e 7465 6e74 2e72 6561 6428  le_content.read(
+00018170: 6765 745f 6669 6c65 5f75 706c 6f61 645f  get_file_upload_
+00018180: 6368 756e 6b5f 7369 7a65 2829 290a 2020  chunk_size()).  
+00018190: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000181a0: 2062 7566 663a 0a20 2020 2020 2020 2020   buff:.         
+000181b0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+000181c0: 2020 2020 2020 2020 206e 6577 5f73 697a           new_siz
+000181d0: 6520 3d20 7365 6c66 2e5f 6c65 6761 6379  e = self._legacy
+000181e0: 5f61 7070 656e 645f 7570 6c6f 6164 2874  _append_upload(t
+000181f0: 6d70 5f75 7269 2c20 4279 7465 7349 4f28  mp_uri, BytesIO(
+00018200: 6275 6666 2929 0a20 2020 2020 2020 2020  buff)).         
+00018210: 2020 2069 6620 6e65 775f 7369 7a65 202d     if new_size -
+00018220: 2063 7572 5f73 697a 6520 213d 206c 656e   cur_size != len
+00018230: 2862 7566 6629 3a0a 2020 2020 2020 2020  (buff):.        
+00018240: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00018250: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00018260: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00018270: 696e 636f 6d70 6c65 7465 2063 6875 6e6b  incomplete chunk
+00018280: 2075 706c 6f61 6420 6e3a 7b6e 6577 5f73   upload n:{new_s
+00018290: 697a 657d 2022 0a20 2020 2020 2020 2020  ize} ".         
+000182a0: 2020 2020 2020 2020 2020 2066 226f 3a7b             f"o:{
+000182b0: 6375 725f 7369 7a65 7d20 623a 7b6c 656e  cur_size} b:{len
+000182c0: 2862 7566 6629 7d22 290a 2020 2020 2020  (buff)}").      
+000182d0: 2020 2020 2020 6375 725f 7369 7a65 203d        cur_size =
+000182e0: 206e 6577 5f73 697a 650a 2020 2020 2020   new_size.      
+000182f0: 2020 7072 696e 745f 7072 6f67 7265 7373    print_progress
+00018300: 2863 7572 5f73 697a 6520 2f20 746f 7461  (cur_size / tota
+00018310: 6c5f 7369 7a65 2c20 5472 7565 290a 0a20  l_size, True).. 
+00018320: 2020 2064 6566 205f 7570 6c6f 6164 5f66     def _upload_f
+00018330: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+00018340: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00018350: 2020 2066 696c 655f 636f 6e74 656e 743a     file_content:
+00018360: 2049 4f5b 6279 7465 735d 2c0a 2020 2020   IO[bytes],.    
+00018370: 2020 2020 2020 2020 6d61 785f 7468 7265          max_thre
+00018380: 6164 733a 2069 6e74 2c0a 2020 2020 2020  ads: int,.      
+00018390: 2020 2020 2020 6578 743a 2073 7472 2c0a        ext: str,.
+000183a0: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
+000183b0: 7265 7373 5f62 6172 3a20 4f70 7469 6f6e  ress_bar: Option
+000183c0: 616c 5b49 4f5b 416e 795d 5d20 3d20 7379  al[IO[Any]] = sy
+000183d0: 732e 7374 646f 7574 2920 2d3e 204e 6f6e  s.stdout) -> Non
+000183e0: 653a 0a20 2020 2020 2020 2069 6620 7365  e:.        if se
+000183f0: 6c66 2e5f 636c 6965 6e74 2e5f 6170 695f  lf._client._api_
+00018400: 7665 7273 696f 6e20 3c20 353a 0a20 2020  version < 5:.   
+00018410: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+00018420: 6567 6163 795f 7570 6c6f 6164 5f66 696c  egacy_upload_fil
+00018430: 6528 6669 6c65 5f63 6f6e 7465 6e74 2c20  e(file_content, 
+00018440: 6578 743d 227a 6970 2229 0a20 2020 2020  ext="zip").     
+00018450: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00018460: 2020 2020 2020 696e 6974 5f70 6f73 203d        init_pos =
+00018470: 2066 696c 655f 636f 6e74 656e 742e 7365   file_content.se
+00018480: 656b 2830 2c20 696f 2e53 4545 4b5f 4355  ek(0, io.SEEK_CU
+00018490: 5229 0a20 2020 2020 2020 2066 696c 655f  R).        file_
+000184a0: 6861 7368 203d 2067 6574 5f66 696c 655f  hash = get_file_
+000184b0: 6861 7368 2866 696c 655f 636f 6e74 656e  hash(file_conten
+000184c0: 7429 0a20 2020 2020 2020 2074 6f74 616c  t).        total
+000184d0: 5f73 697a 6520 3d20 6669 6c65 5f63 6f6e  _size = file_con
+000184e0: 7465 6e74 2e73 6565 6b28 302c 2069 6f2e  tent.seek(0, io.
+000184f0: 5345 454b 5f45 4e44 2920 2d20 696e 6974  SEEK_END) - init
+00018500: 5f70 6f73 0a20 2020 2020 2020 2066 696c  _pos.        fil
+00018510: 655f 636f 6e74 656e 742e 7365 656b 2869  e_content.seek(i
+00018520: 6e69 745f 706f 732c 2069 6f2e 5345 454b  nit_pos, io.SEEK
+00018530: 5f53 4554 290a 2020 2020 2020 2020 6966  _SET).        if
+00018540: 2070 726f 6772 6573 735f 6261 7220 6973   progress_bar is
+00018550: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00018560: 2020 2020 2020 2070 726f 6772 6573 735f         progress_
+00018570: 6261 722e 7772 6974 6528 2255 706c 6f61  bar.write("Uploa
+00018580: 6469 6e67 2066 696c 653a 5c6e 2229 0a20  ding file:\n"). 
+00018590: 2020 2020 2020 2070 7269 6e74 5f70 726f         print_pro
+000185a0: 6772 6573 7320 3d20 6765 745f 7072 6f67  gress = get_prog
+000185b0: 7265 7373 5f62 6172 286f 7574 3d70 726f  ress_bar(out=pro
+000185c0: 6772 6573 735f 6261 7229 0a20 2020 2020  gress_bar).     
+000185d0: 2020 2074 6d70 5f75 7269 203d 2073 656c     tmp_uri = sel
+000185e0: 662e 5f73 7461 7274 5f75 706c 6f61 6428  f._start_upload(
+000185f0: 746f 7461 6c5f 7369 7a65 2c20 6669 6c65  total_size, file
+00018600: 5f68 6173 682c 2065 7874 290a 2020 2020  _hash, ext).    
+00018610: 2020 2020 7365 6c66 2e5f 746d 705f 7572      self._tmp_ur
+00018620: 6920 3d20 746d 705f 7572 690a 2020 2020  i = tmp_uri.    
+00018630: 2020 2020 7570 6c6f 6164 5f63 6875 6e6b      upload_chunk
+00018640: 5f73 697a 6520 3d20 6765 745f 6669 6c65  _size = get_file
+00018650: 5f75 706c 6f61 645f 6368 756e 6b5f 7369  _upload_chunk_si
+00018660: 7a65 2829 0a20 2020 2020 2020 2074 6f74  ze().        tot
+00018670: 616c 5f63 6875 6e6b 7320 3d20 6d61 7468  al_chunks = math
+00018680: 2e63 6569 6c28 746f 7461 6c5f 7369 7a65  .ceil(total_size
+00018690: 202f 2075 706c 6f61 645f 6368 756e 6b5f   / upload_chunk_
+000186a0: 7369 7a65 290a 0a20 2020 2020 2020 2062  size)..        b
+000186b0: 6567 696e 7320 3d20 5b63 6875 6e6b 202a  egins = [chunk *
+000186c0: 2075 706c 6f61 645f 6368 756e 6b5f 7369   upload_chunk_si
+000186d0: 7a65 2066 6f72 2063 6875 6e6b 2069 6e20  ze for chunk in 
+000186e0: 7261 6e67 6528 746f 7461 6c5f 6368 756e  range(total_chun
+000186f0: 6b73 295d 0a0a 2020 2020 2020 2020 6465  ks)]..        de
+00018700: 6620 636f 6d70 7574 655f 7570 6c6f 6164  f compute_upload
+00018710: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018720: 2020 6f66 6673 6574 3a20 696e 742c 0a20    offset: int,. 
+00018730: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00018740: 6f6d 7075 7465 5f6c 6f63 6b3a 2074 6872  ompute_lock: thr
+00018750: 6561 6469 6e67 2e52 4c6f 636b 2920 2d3e  eading.RLock) ->
+00018760: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018770: 2020 2061 7373 6572 7420 7365 6c66 2e5f     assert self._
+00018780: 746d 705f 7572 6920 6973 206e 6f74 204e  tmp_uri is not N
+00018790: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000187a0: 7769 7468 2063 6f6d 7075 7465 5f6c 6f63  with compute_loc
+000187b0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+000187c0: 2020 2066 696c 655f 636f 6e74 656e 742e     file_content.
+000187d0: 7365 656b 286f 6666 7365 742c 2069 6f2e  seek(offset, io.
+000187e0: 5345 454b 5f53 4554 290a 2020 2020 2020  SEEK_SET).      
+000187f0: 2020 2020 2020 2020 2020 6275 6666 203d            buff =
+00018800: 2066 696c 655f 636f 6e74 656e 742e 7265   file_content.re
+00018810: 6164 2875 706c 6f61 645f 6368 756e 6b5f  ad(upload_chunk_
+00018820: 7369 7a65 290a 2020 2020 2020 2020 2020  size).          
+00018830: 2020 6e65 775f 7369 7a65 203d 2073 656c    new_size = sel
+00018840: 662e 5f61 7070 656e 645f 7570 6c6f 6164  f._append_upload
+00018850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018860: 2020 7365 6c66 2e5f 746d 705f 7572 692c    self._tmp_uri,
+00018870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018880: 2042 7974 6573 494f 2862 7566 6629 2c0a   BytesIO(buff),.
+00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188a0: 6f66 6673 6574 290a 2020 2020 2020 2020  offset).        
+000188b0: 2020 2020 6966 206e 6577 5f73 697a 6520      if new_size 
+000188c0: 213d 206c 656e 2862 7566 6629 3a0a 2020  != len(buff):.  
+000188d0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000188e0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018900: 2020 2020 6622 696e 636f 6d70 6c65 7465      f"incomplete
+00018910: 2063 6875 6e6b 2075 706c 6f61 6420 6e3a   chunk upload n:
+00018920: 7b6e 6577 5f73 697a 657d 2022 0a20 2020  {new_size} ".   
+00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018940: 2066 2262 3a7b 6c65 6e28 6275 6666 297d   f"b:{len(buff)}
+00018950: 206f 6666 7365 743a 207b 6f66 6673 6574   offset: {offset
+00018960: 7d22 290a 0a20 2020 2020 2020 2063 6f6d  }")..        com
+00018970: 7075 7465 5f70 6172 616c 6c65 6c28 6265  pute_parallel(be
+00018980: 6769 6e73 2c20 636f 6d70 7574 655f 7570  gins, compute_up
+00018990: 6c6f 6164 2c20 7072 696e 745f 7072 6f67  load, print_prog
+000189a0: 7265 7373 2c20 6d61 785f 7468 7265 6164  ress, max_thread
+000189b0: 7329 0a0a 2020 2020 6465 6620 7570 6c6f  s)..    def uplo
+000189c0: 6164 5f7a 6970 280a 2020 2020 2020 2020  ad_zip(.        
+000189d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000189e0: 2020 2020 2020 736f 7572 6365 3a20 556e        source: Un
+000189f0: 696f 6e5b 7374 722c 2069 6f2e 4279 7465  ion[str, io.Byte
+00018a00: 7349 4f5d 2c0a 2020 2020 2020 2020 2020  sIO],.          
+00018a10: 2020 6d61 785f 7468 7265 6164 733a 2069    max_threads: i
+00018a20: 6e74 203d 2031 3029 202d 3e20 4c69 7374  nt = 10) -> List
+00018a30: 5b27 426c 6f62 4861 6e64 6c65 275d 3a0a  ['BlobHandle']:.
+00018a40: 2020 2020 2020 2020 6669 6c65 733a 204c          files: L
+00018a50: 6973 745b 7374 725d 203d 205b 5d0a 2020  ist[str] = [].  
+00018a60: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00018a70: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00018a80: 616e 6365 2873 6f75 7263 652c 2073 7472  ance(source, str
+00018a90: 2920 6f72 206e 6f74 2068 6173 6174 7472  ) or not hasattr
+00018aa0: 2873 6f75 7263 652c 2022 7265 6164 2229  (source, "read")
+00018ab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018ac0: 2020 7769 7468 206f 7065 6e28 6622 7b73    with open(f"{s
+00018ad0: 6f75 7263 657d 222c 2022 7262 2229 2061  ource}", "rb") a
+00018ae0: 7320 6669 6e3a 0a20 2020 2020 2020 2020  s fin:.         
+00018af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018b00: 5f75 706c 6f61 645f 6669 6c65 2866 696e  _upload_file(fin
+00018b10: 2c20 6d61 785f 7468 7265 6164 732c 2065  , max_threads, e
+00018b20: 7874 3d22 7a69 7022 290a 2020 2020 2020  xt="zip").      
+00018b30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00018b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018b50: 2e5f 7570 6c6f 6164 5f66 696c 6528 736f  ._upload_file(so
+00018b60: 7572 6365 2c20 6d61 785f 7468 7265 6164  urce, max_thread
+00018b70: 732c 2065 7874 3d22 7a69 7022 290a 2020  s, ext="zip").  
+00018b80: 2020 2020 2020 2020 2020 6669 6c65 7320            files 
+00018b90: 3d20 7365 6c66 2e5f 6669 6e69 7368 5f75  = self._finish_u
+00018ba0: 706c 6f61 645f 7a69 7028 290a 2020 2020  pload_zip().    
+00018bb0: 2020 2020 6669 6e61 6c6c 793a 0a20 2020      finally:.   
+00018bc0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00018bd0: 6c65 6172 5f75 706c 6f61 6428 290a 2020  lear_upload().  
+00018be0: 2020 2020 2020 7265 7475 726e 205b 0a20        return [. 
+00018bf0: 2020 2020 2020 2020 2020 2042 6c6f 6248             BlobH
+00018c00: 616e 646c 6528 7365 6c66 2e5f 636c 6965  andle(self._clie
+00018c10: 6e74 2c20 626c 6f62 5f75 7269 2c20 6973  nt, blob_uri, is
+00018c20: 5f66 756c 6c3d 5472 7565 290a 2020 2020  _full=True).    
+00018c30: 2020 2020 2020 2020 666f 7220 626c 6f62          for blob
+00018c40: 5f75 7269 2069 6e20 6669 6c65 730a 2020  _uri in files.  
+00018c50: 2020 2020 2020 5d0a 0a20 2020 2064 6566        ]..    def
+00018c60: 2075 706c 6f61 645f 6d6f 6465 6c5f 6669   upload_model_fi
+00018c70: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00018c80: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00018c90: 2020 6d6f 6465 6c5f 6f62 6a3a 2049 4f5b    model_obj: IO[
+00018ca0: 6279 7465 735d 2c0a 2020 2020 2020 2020  bytes],.        
+00018cb0: 2020 2020 7863 6f6c 733a 204f 7074 696f      xcols: Optio
+00018cc0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 2c0a  nal[List[str]],.
+00018cd0: 2020 2020 2020 2020 2020 2020 7963 6f6c              ycol
+00018ce0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00018cf0: 5b73 7472 5d5d 2c0a 2020 2020 2020 2020  [str]],.        
+00018d00: 2020 2020 6973 5f63 6c66 3a20 626f 6f6c      is_clf: bool
+00018d10: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+00018d20: 6465 6c5f 6e61 6d65 3a20 7374 722c 0a20  del_name: str,. 
+00018d30: 2020 2020 2020 2020 2020 2076 6572 7369             versi
+00018d40: 6f6e 3a20 696e 7420 3d20 2d31 2c0a 2020  on: int = -1,.  
+00018d50: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00018d60: 7061 7261 6d73 3a20 4f70 7469 6f6e 616c  params: Optional
+00018d70: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00018d80: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00018d90: 2020 2020 2064 656c 6574 655f 6c61 7465       delete_late
+00018da0: 725f 7665 7273 696f 6e73 3a20 626f 6f6c  r_versions: bool
+00018db0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00018dc0: 2020 2020 2020 6d61 785f 7468 7265 6164        max_thread
+00018dd0: 733a 2069 6e74 203d 2031 302c 0a20 2020  s: int = 10,.   
+00018de0: 2020 2020 2020 2020 2066 756c 6c5f 696e           full_in
+00018df0: 6974 3a20 626f 6f6c 203d 2054 7275 6529  it: bool = True)
+00018e00: 202d 3e20 5570 6c6f 6164 4669 6c65 7352   -> UploadFilesR
+00018e10: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00018e20: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00018e30: 2020 7365 6c66 2e5f 7570 6c6f 6164 5f66    self._upload_f
+00018e40: 696c 6528 6d6f 6465 6c5f 6f62 6a2c 206d  ile(model_obj, m
+00018e50: 6178 5f74 6872 6561 6473 2c20 6578 743d  ax_threads, ext=
+00018e60: 2270 6b6c 2229 0a20 2020 2020 2020 2020  "pkl").         
+00018e70: 2020 2069 6620 6d6f 6465 6c5f 7061 7261     if model_para
+00018e80: 6d73 2069 7320 4e6f 6e65 3a0a 2020 2020  ms is None:.    
+00018e90: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00018ea0: 6c5f 7061 7261 6d73 203d 207b 7d0a 2020  l_params = {}.  
+00018eb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00018ec0: 2073 656c 662e 5f66 696e 6973 685f 6d6f   self._finish_mo
+00018ed0: 6465 6c5f 7570 6c6f 6164 280a 2020 2020  del_upload(.    
+00018ee0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00018ef0: 6c5f 6e61 6d65 3d6d 6f64 656c 5f6e 616d  l_name=model_nam
+00018f00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00018f10: 2020 2076 6572 7369 6f6e 3d76 6572 7369     version=versi
+00018f20: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00018f30: 2020 2020 6d6f 6465 6c5f 7061 7261 6d73      model_params
+00018f40: 3d6d 6f64 656c 5f70 6172 616d 732c 0a20  =model_params,. 
+00018f50: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00018f60: 636f 6c73 3d78 636f 6c73 2c0a 2020 2020  cols=xcols,.    
+00018f70: 2020 2020 2020 2020 2020 2020 7963 6f6c              ycol
+00018f80: 733d 7963 6f6c 732c 0a20 2020 2020 2020  s=ycols,.       
+00018f90: 2020 2020 2020 2020 2069 735f 636c 663d           is_clf=
+00018fa0: 6973 5f63 6c66 2c0a 2020 2020 2020 2020  is_clf,.        
+00018fb0: 2020 2020 2020 2020 6465 6c65 7465 5f6c          delete_l
+00018fc0: 6174 6572 5f76 6572 7369 6f6e 733d 6465  ater_versions=de
+00018fd0: 6c65 7465 5f6c 6174 6572 5f76 6572 7369  lete_later_versi
+00018fe0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+00018ff0: 2020 2020 2066 756c 6c5f 696e 6974 3d66       full_init=f
+00019000: 756c 6c5f 696e 6974 290a 2020 2020 2020  ull_init).      
+00019010: 2020 6669 6e61 6c6c 793a 0a20 2020 2020    finally:.     
+00019020: 2020 2020 2020 2073 656c 662e 5f63 6c65         self._cle
+00019030: 6172 5f75 706c 6f61 6428 290a 0a20 2020  ar_upload()..   
+00019040: 2064 6566 2075 706c 6f61 645f 736b 6c69   def upload_skli
+00019050: 6b65 5f6d 6f64 656c 280a 2020 2020 2020  ke_model(.      
+00019060: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00019070: 2020 2020 2020 2020 6d6f 6465 6c3a 2041          model: A
+00019080: 6e79 2c0a 2020 2020 2020 2020 2020 2020  ny,.            
+00019090: 7863 6f6c 733a 204c 6973 745b 7374 725d  xcols: List[str]
+000190a0: 2c0a 2020 2020 2020 2020 2020 2020 7963  ,.            yc
+000190b0: 6f6c 733a 204f 7074 696f 6e61 6c5b 4c69  ols: Optional[Li
+000190c0: 7374 5b73 7472 5d5d 2c0a 2020 2020 2020  st[str]],.      
+000190d0: 2020 2020 2020 6973 5f63 6c66 3a20 626f        is_clf: bo
+000190e0: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
+000190f0: 6d6f 6465 6c5f 6e61 6d65 3a20 4f70 7469  model_name: Opti
+00019100: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00019110: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+00019120: 7273 696f 6e3a 2069 6e74 203d 202d 312c  rsion: int = -1,
+00019130: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+00019140: 656c 5f70 6172 616d 733a 204f 7074 696f  el_params: Optio
+00019150: 6e61 6c5b 4469 6374 5b73 7472 2c20 416e  nal[Dict[str, An
+00019160: 795d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  y]] = None,.    
+00019170: 2020 2020 2020 2020 6465 6c65 7465 5f6c          delete_l
+00019180: 6174 6572 5f76 6572 7369 6f6e 733a 2062  ater_versions: b
+00019190: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+000191a0: 2020 2020 2020 2020 2066 756c 6c5f 696e           full_in
+000191b0: 6974 3a20 626f 6f6c 203d 2054 7275 6529  it: bool = True)
+000191c0: 202d 3e20 5570 6c6f 6164 4669 6c65 7352   -> UploadFilesR
+000191d0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+000191e0: 2069 6620 6d6f 6465 6c5f 6e61 6d65 2069   if model_name i
+000191f0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00019200: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00019210: 2020 2020 2020 2020 206d 6f64 656c 5f6e           model_n
+00019220: 616d 6520 3d20 7479 7065 286d 6f64 656c  ame = type(model
+00019230: 292e 5f5f 6e61 6d65 5f5f 0a20 2020 2020  ).__name__.     
+00019240: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00019250: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00019260: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00019270: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00019280: 2263 616e 206e 6f74 2069 6e66 6572 206d  "can not infer m
+00019290: 6f64 656c 206e 616d 6520 7b6d 6f64 656c  odel name {model
+000192a0: 7d22 2920 6672 6f6d 2065 0a20 2020 2020  }") from e.     
+000192b0: 2020 2069 6620 6d6f 6465 6c5f 7061 7261     if model_para
+000192c0: 6d73 2069 7320 4e6f 6e65 3a0a 2020 2020  ms is None:.    
+000192d0: 2020 2020 2020 2020 6d6f 6465 6c5f 7061          model_pa
+000192e0: 7261 6d73 203d 207b 7d0a 2020 2020 2020  rams = {}.      
+000192f0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00019300: 2020 2069 6620 6973 5f63 6c66 2061 6e64     if is_clf and
+00019310: 2022 636c 6173 7365 7322 206e 6f74 2069   "classes" not i
+00019320: 6e20 6d6f 6465 6c5f 7061 7261 6d73 3a0a  n model_params:.
+00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019340: 6d6f 6465 6c5f 7061 7261 6d73 5b22 636c  model_params["cl
+00019350: 6173 7365 7322 5d20 3d20 6d6f 6465 6c2e  asses"] = model.
+00019360: 636c 6173 7365 735f 0a20 2020 2020 2020  classes_.       
+00019370: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00019380: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00019390: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000193a0: 7272 6f72 2866 2263 616e 206e 6f74 2069  rror(f"can not i
+000193b0: 6e66 6572 2063 6c61 7373 6573 2066 726f  nfer classes fro
+000193c0: 6d20 7b6d 6f64 656c 7d22 2920 6672 6f6d  m {model}") from
+000193d0: 2065 0a20 2020 2020 2020 2064 756d 7020   e.        dump 
+000193e0: 3d20 7069 636b 6c65 2e64 756d 7073 286d  = pickle.dumps(m
+000193f0: 6f64 656c 2c20 7069 636b 6c65 2e48 4947  odel, pickle.HIG
+00019400: 4845 5354 5f50 524f 544f 434f 4c29 0a20  HEST_PROTOCOL). 
+00019410: 2020 2020 2020 2077 6974 6820 696f 2e42         with io.B
+00019420: 7974 6573 494f 2864 756d 7029 2061 7320  ytesIO(dump) as 
+00019430: 6275 6666 6572 3a0a 2020 2020 2020 2020  buffer:.        
+00019440: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00019450: 7570 6c6f 6164 5f6d 6f64 656c 5f66 696c  upload_model_fil
+00019460: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00019470: 2020 2062 7566 6665 722c 0a20 2020 2020     buffer,.     
+00019480: 2020 2020 2020 2020 2020 2078 636f 6c73             xcols
+00019490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000194a0: 2020 7963 6f6c 732c 0a20 2020 2020 2020    ycols,.       
+000194b0: 2020 2020 2020 2020 2069 735f 636c 662c           is_clf,
+000194c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000194d0: 206d 6f64 656c 5f6e 616d 652c 0a20 2020   model_name,.   
+000194e0: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+000194f0: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00019500: 2020 2020 2020 6d6f 6465 6c5f 7061 7261        model_para
+00019510: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
+00019520: 2020 2020 6465 6c65 7465 5f6c 6174 6572      delete_later
+00019530: 5f76 6572 7369 6f6e 732c 0a20 2020 2020  _versions,.     
+00019540: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
+00019550: 696e 6974 290a 0a20 2020 2064 6566 2063  init)..    def c
+00019560: 6f6e 7665 7274 5f6d 6f64 656c 280a 2020  onvert_model(.  
+00019570: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+00019580: 2020 2020 2020 2020 2020 2020 7665 7273              vers
+00019590: 696f 6e3a 204f 7074 696f 6e61 6c5b 696e  ion: Optional[in
+000195a0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+000195b0: 2020 2020 2020 2072 656c 6f61 643a 2062         reload: b
+000195c0: 6f6f 6c20 3d20 5472 7565 2920 2d3e 204d  ool = True) -> M
+000195d0: 6f64 656c 5265 6c65 6173 6552 6573 706f  odelReleaseRespo
+000195e0: 6e73 653a 0a20 2020 2020 2020 2072 6574  nse:.        ret
+000195f0: 7572 6e20 6361 7374 284d 6f64 656c 5265  urn cast(ModelRe
+00019600: 6c65 6173 6552 6573 706f 6e73 652c 2073  leaseResponse, s
+00019610: 656c 662e 5f63 6c69 656e 742e 7265 7175  elf._client.requ
+00019620: 6573 745f 6a73 6f6e 280a 2020 2020 2020  est_json(.      
+00019630: 2020 2020 2020 4d45 5448 4f44 5f50 4f53        METHOD_POS
+00019640: 542c 2022 2f63 6f6e 7665 7274 5f6d 6f64  T, "/convert_mod
+00019650: 656c 222c 207b 0a20 2020 2020 2020 2020  el", {.         
+00019660: 2020 2020 2020 2022 626c 6f62 223a 2073         "blob": s
+00019670: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
+00019680: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019690: 7665 7273 696f 6e22 3a20 7665 7273 696f  version": versio
+000196a0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+000196b0: 2020 2022 7265 6c6f 6164 223a 2072 656c     "reload": rel
+000196c0: 6f61 642c 0a20 2020 2020 2020 2020 2020  oad,.           
+000196d0: 207d 2929 0a0a 2020 2020 6465 6620 6465   }))..    def de
+000196e0: 6c65 7465 2873 656c 6629 202d 3e20 4465  lete(self) -> De
+000196f0: 6c65 7465 426c 6f62 5265 7370 6f6e 7365  leteBlobResponse
+00019700: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00019710: 2063 6173 7428 4465 6c65 7465 426c 6f62   cast(DeleteBlob
+00019720: 5265 7370 6f6e 7365 2c20 7365 6c66 2e5f  Response, self._
+00019730: 636c 6965 6e74 2e72 6571 7565 7374 5f6a  client.request_j
+00019740: 736f 6e28 0a20 2020 2020 2020 2020 2020  son(.           
+00019750: 204d 4554 484f 445f 4445 4c45 5445 2c20   METHOD_DELETE, 
+00019760: 222f 626c 6f62 222c 207b 0a20 2020 2020  "/blob", {.     
+00019770: 2020 2020 2020 2020 2020 2022 626c 6f62             "blob
+00019780: 5f75 7269 7322 3a20 5b73 656c 662e 6765  _uris": [self.ge
+00019790: 745f 7572 6928 295d 2c0a 2020 2020 2020  t_uri()],.      
+000197a0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000197b0: 2029 290a 0a20 2020 2064 6566 2067 6574   ))..    def get
+000197c0: 5f6d 6f64 656c 5f72 656c 6561 7365 2873  _model_release(s
+000197d0: 656c 6629 202d 3e20 4d6f 6465 6c52 656c  elf) -> ModelRel
+000197e0: 6561 7365 5265 7370 6f6e 7365 3a0a 2020  easeResponse:.  
+000197f0: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+00019800: 7428 4d6f 6465 6c52 656c 6561 7365 5265  t(ModelReleaseRe
+00019810: 7370 6f6e 7365 2c20 7365 6c66 2e5f 636c  sponse, self._cl
+00019820: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
+00019830: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
+00019840: 4554 484f 445f 4745 542c 2022 2f6d 6f64  ETHOD_GET, "/mod
+00019850: 656c 5f72 656c 6561 7365 222c 207b 0a20  el_release", {. 
+00019860: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019870: 626c 6f62 223a 2073 656c 662e 6765 745f  blob": self.get_
+00019880: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
+00019890: 2020 207d 2929 0a0a 2020 2020 6465 6620     }))..    def 
+000198a0: 6765 745f 6d6f 6465 6c5f 7665 7273 696f  get_model_versio
+000198b0: 6e28 7365 6c66 2920 2d3e 204d 6f64 656c  n(self) -> Model
+000198c0: 5665 7273 696f 6e52 6573 706f 6e73 653a  VersionResponse:
+000198d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000198e0: 6361 7374 284d 6f64 656c 5665 7273 696f  cast(ModelVersio
+000198f0: 6e52 6573 706f 6e73 652c 2073 656c 662e  nResponse, self.
+00019900: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
+00019910: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
+00019920: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
+00019930: 6d6f 6465 6c5f 7665 7273 696f 6e22 2c20  model_version", 
+00019940: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00019950: 2020 226d 6f64 656c 5f75 7269 223a 2073    "model_uri": s
+00019960: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
+00019970: 2020 2020 2020 2020 2020 207d 2929 0a0a             }))..
+00019980: 2020 2020 6465 6620 5f63 6f70 795f 6d6f      def _copy_mo
+00019990: 6465 6c5f 7665 7273 696f 6e28 0a20 2020  del_version(.   
+000199a0: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+000199b0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+000199c0: 5f75 7269 3a20 7374 722c 0a20 2020 2020  _uri: str,.     
+000199d0: 2020 2020 2020 2072 6561 645f 7665 7273         read_vers
+000199e0: 696f 6e3a 204f 7074 696f 6e61 6c5b 696e  ion: Optional[in
+000199f0: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
+00019a00: 7772 6974 655f 7665 7273 696f 6e3a 2069  write_version: i
+00019a10: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00019a20: 6f76 6572 7772 6974 653a 2062 6f6f 6c29  overwrite: bool)
+00019a30: 202d 3e20 4d6f 6465 6c56 6572 7369 6f6e   -> ModelVersion
+00019a40: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00019a50: 2020 7265 7475 726e 2063 6173 7428 4d6f    return cast(Mo
+00019a60: 6465 6c56 6572 7369 6f6e 5265 7370 6f6e  delVersionRespon
+00019a70: 7365 2c20 7365 6c66 2e5f 636c 6965 6e74  se, self._client
+00019a80: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+00019a90: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+00019aa0: 445f 5055 542c 2022 2f6d 6f64 656c 5f76  D_PUT, "/model_v
+00019ab0: 6572 7369 6f6e 222c 207b 0a20 2020 2020  ersion", {.     
+00019ac0: 2020 2020 2020 2020 2020 2022 6d6f 6465             "mode
+00019ad0: 6c5f 7572 6922 3a20 6d6f 6465 6c5f 7572  l_uri": model_ur
+00019ae0: 692c 0a20 2020 2020 2020 2020 2020 2020  i,.             
+00019af0: 2020 2022 7265 6164 5f76 6572 7369 6f6e     "read_version
+00019b00: 223a 2072 6561 645f 7665 7273 696f 6e2c  ": read_version,
+00019b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b20: 2022 7772 6974 655f 7665 7273 696f 6e22   "write_version"
+00019b30: 3a20 7772 6974 655f 7665 7273 696f 6e2c  : write_version,
+00019b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b50: 2022 6f76 6572 7772 6974 6522 3a20 6f76   "overwrite": ov
+00019b60: 6572 7772 6974 652c 0a20 2020 2020 2020  erwrite,.       
+00019b70: 2020 2020 207d 2929 0a0a 2020 2020 6465       }))..    de
+00019b80: 6620 636f 7079 5f6d 6f64 656c 5f76 6572  f copy_model_ver
+00019b90: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+00019ba0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00019bb0: 2020 2020 7265 6164 5f76 6572 7369 6f6e      read_version
+00019bc0: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
+00019bd0: 2020 2077 7269 7465 5f76 6572 7369 6f6e     write_version
+00019be0: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
+00019bf0: 2020 206f 7665 7277 7269 7465 3a20 626f     overwrite: bo
+00019c00: 6f6c 2920 2d3e 204d 6f64 656c 5665 7273  ol) -> ModelVers
+00019c10: 696f 6e52 6573 706f 6e73 653a 0a20 2020  ionResponse:.   
+00019c20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00019c30: 2e5f 636f 7079 5f6d 6f64 656c 5f76 6572  ._copy_model_ver
+00019c40: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+00019c50: 2020 6d6f 6465 6c5f 7572 693d 7365 6c66    model_uri=self
+00019c60: 2e67 6574 5f75 7269 2829 2c0a 2020 2020  .get_uri(),.    
+00019c70: 2020 2020 2020 2020 7265 6164 5f76 6572          read_ver
+00019c80: 7369 6f6e 3d72 6561 645f 7665 7273 696f  sion=read_versio
+00019c90: 6e2c 0a20 2020 2020 2020 2020 2020 2077  n,.            w
+00019ca0: 7269 7465 5f76 6572 7369 6f6e 3d77 7269  rite_version=wri
+00019cb0: 7465 5f76 6572 7369 6f6e 2c0a 2020 2020  te_version,.    
+00019cc0: 2020 2020 2020 2020 6f76 6572 7772 6974          overwrit
+00019cd0: 653d 6f76 6572 7772 6974 6529 0a0a 2020  e=overwrite)..  
+00019ce0: 2020 6465 6620 6465 6c65 7465 5f6d 6f64    def delete_mod
+00019cf0: 656c 5f76 6572 7369 6f6e 2873 656c 662c  el_version(self,
+00019d00: 2076 6572 7369 6f6e 3a20 696e 7429 202d   version: int) -
+00019d10: 3e20 4d6f 6465 6c56 6572 7369 6f6e 5265  > ModelVersionRe
+00019d20: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00019d30: 7265 7475 726e 2073 656c 662e 5f63 6f70  return self._cop
+00019d40: 795f 6d6f 6465 6c5f 7665 7273 696f 6e28  y_model_version(
+00019d50: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+00019d60: 656c 5f75 7269 3d73 656c 662e 6765 745f  el_uri=self.get_
+00019d70: 7572 6928 292c 0a20 2020 2020 2020 2020  uri(),.         
+00019d80: 2020 2072 6561 645f 7665 7273 696f 6e3d     read_version=
+00019d90: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00019da0: 2020 7772 6974 655f 7665 7273 696f 6e3d    write_version=
+00019db0: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
+00019dc0: 2020 2020 206f 7665 7277 7269 7465 3d54       overwrite=T
+00019dd0: 7275 6529 0a0a 2020 2020 6465 6620 5f5f  rue)..    def __
+00019de0: 6861 7368 5f5f 2873 656c 6629 202d 3e20  hash__(self) -> 
+00019df0: 696e 743a 0a20 2020 2020 2020 2072 6574  int:.        ret
+00019e00: 7572 6e20 6861 7368 2873 656c 662e 6173  urn hash(self.as
+00019e10: 5f73 7472 2829 290a 0a20 2020 2064 6566  _str())..    def
+00019e20: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
+00019e30: 6865 723a 206f 626a 6563 7429 202d 3e20  her: object) -> 
+00019e40: 626f 6f6c 3a0a 2020 2020 2020 2020 6966  bool:.        if
+00019e50: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00019e60: 6f74 6865 722c 2073 656c 662e 5f5f 636c  other, self.__cl
+00019e70: 6173 735f 5f29 3a0a 2020 2020 2020 2020  ass__):.        
+00019e80: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00019e90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019ea0: 7365 6c66 2e61 735f 7374 7228 2920 3d3d  self.as_str() ==
+00019eb0: 206f 7468 6572 2e61 735f 7374 7228 290a   other.as_str().
+00019ec0: 0a20 2020 2064 6566 205f 5f6e 655f 5f28  .    def __ne__(
+00019ed0: 7365 6c66 2c20 6f74 6865 723a 206f 626a  self, other: obj
+00019ee0: 6563 7429 202d 3e20 626f 6f6c 3a0a 2020  ect) -> bool:.  
+00019ef0: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
+00019f00: 2073 656c 662e 5f5f 6571 5f5f 286f 7468   self.__eq__(oth
+00019f10: 6572 290a 0a20 2020 2064 6566 205f 5f73  er)..    def __s
+00019f20: 7472 5f5f 2873 656c 6629 202d 3e20 7374  tr__(self) -> st
+00019f30: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+00019f40: 6e20 7365 6c66 2e61 735f 7374 7228 290a  n self.as_str().
+00019f50: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+00019f60: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
+00019f70: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00019f80: 227b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  "{self.__class__
+00019f90: 2e5f 5f6e 616d 655f 5f7d 5b7b 7365 6c66  .__name__}[{self
+00019fa0: 2e61 735f 7374 7228 297d 5d22 0a0a 2320  .as_str()}]"..# 
+00019fb0: 2a2a 2a20 426c 6f62 4861 6e64 6c65 202a  *** BlobHandle *
+00019fc0: 2a2a 0a0a 0a63 6c61 7373 2043 5356 426c  **...class CSVBl
+00019fd0: 6f62 4861 6e64 6c65 2842 6c6f 6248 616e  obHandle(BlobHan
+00019fe0: 646c 6529 3a0a 2020 2020 6465 6620 6669  dle):.    def fi
+00019ff0: 6e69 7368 5f63 7376 5f75 706c 6f61 6428  nish_csv_upload(
+0001a000: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001a010: 662c 0a20 2020 2020 2020 2020 2020 2066  f,.            f
+0001a020: 696c 656e 616d 653a 204f 7074 696f 6e61  ilename: Optiona
+0001a030: 6c5b 7374 725d 203d 204e 6f6e 6529 202d  l[str] = None) -
+0001a040: 3e20 5570 6c6f 6164 4669 6c65 7352 6573  > UploadFilesRes
+0001a050: 706f 6e73 653a 0a20 2020 2020 2020 2074  ponse:.        t
+0001a060: 6d70 5f75 7269 203d 2073 656c 662e 5f74  mp_uri = self._t
+0001a070: 6d70 5f75 7269 0a20 2020 2020 2020 2069  mp_uri.        i
+0001a080: 6620 746d 705f 7572 6920 6973 204e 6f6e  f tmp_uri is Non
+0001a090: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0001a0a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0001a0b0: 2274 6d70 5f75 7269 2069 7320 4e6f 6e65  "tmp_uri is None
+0001a0c0: 2229 0a20 2020 2020 2020 2061 7267 733a  ").        args:
+0001a0d0: 2044 6963 745b 7374 722c 204f 7074 696f   Dict[str, Optio
+0001a0e0: 6e61 6c5b 556e 696f 6e5b 7374 722c 2069  nal[Union[str, i
+0001a0f0: 6e74 5d5d 5d20 3d20 7b0a 2020 2020 2020  nt]]] = {.      
+0001a100: 2020 2020 2020 2274 6d70 5f75 7269 223a        "tmp_uri":
+0001a110: 2074 6d70 5f75 7269 2c0a 2020 2020 2020   tmp_uri,.      
+0001a120: 2020 2020 2020 2263 7376 5f75 7269 223a        "csv_uri":
+0001a130: 2073 656c 662e 6765 745f 7572 6928 292c   self.get_uri(),
+0001a140: 0a20 2020 2020 2020 2020 2020 2022 6f77  .            "ow
+0001a150: 6e65 725f 6461 6722 3a20 7365 6c66 2e67  ner_dag": self.g
+0001a160: 6574 5f6f 776e 6572 5f64 6167 2829 2c0a  et_owner_dag(),.
+0001a170: 2020 2020 2020 2020 2020 2020 226f 776e              "own
+0001a180: 6572 5f6e 6f64 6522 3a20 7365 6c66 2e67  er_node": self.g
+0001a190: 6574 5f6f 776e 6572 5f6e 6f64 6528 292c  et_owner_node(),
+0001a1a0: 0a20 2020 2020 2020 2020 2020 2022 6669  .            "fi
+0001a1b0: 6c65 6e61 6d65 223a 2066 696c 656e 616d  lename": filenam
+0001a1c0: 652c 0a20 2020 2020 2020 207d 0a20 2020  e,.        }.   
+0001a1d0: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
+0001a1e0: 2855 706c 6f61 6446 696c 6573 5265 7370  (UploadFilesResp
+0001a1f0: 6f6e 7365 2c20 7365 6c66 2e5f 636c 6965  onse, self._clie
+0001a200: 6e74 2e72 6571 7565 7374 5f6a 736f 6e28  nt.request_json(
+0001a210: 0a20 2020 2020 2020 2020 2020 204d 4554  .            MET
+0001a220: 484f 445f 504f 5354 2c20 222f 6669 6e69  HOD_POST, "/fini
+0001a230: 7368 5f63 7376 222c 2061 7267 7329 290a  sh_csv", args)).
+0001a240: 0a20 2020 2064 6566 2061 6464 5f66 726f  .    def add_fro
+0001a250: 6d5f 6669 6c65 280a 2020 2020 2020 2020  m_file(.        
+0001a260: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0001a270: 2020 2020 2020 6669 6c65 6e61 6d65 3a20        filename: 
+0001a280: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0001a290: 2070 726f 6772 6573 735f 6261 723a 204f   progress_bar: O
+0001a2a0: 7074 696f 6e61 6c5b 494f 5b41 6e79 5d5d  ptional[IO[Any]]
+0001a2b0: 203d 2073 7973 2e73 7464 6f75 742c 0a20   = sys.stdout,. 
+0001a2c0: 2020 2020 2020 2020 2020 2072 6571 7565             reque
+0001a2d0: 7565 5f6f 6e5f 6669 6e69 7368 3a20 4f70  ue_on_finish: Op
+0001a2e0: 7469 6f6e 616c 5b4e 6f64 6548 616e 646c  tional[NodeHandl
+0001a2f0: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
+0001a300: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
+0001a310: 6473 3a20 696e 7420 3d20 3130 2920 2d3e  ds: int = 10) ->
+0001a320: 204f 7074 696f 6e61 6c5b 5570 6c6f 6164   Optional[Upload
+0001a330: 4669 6c65 7352 6573 706f 6e73 655d 3a0a  FilesResponse]:.
+0001a340: 2020 2020 2020 2020 666e 616d 6520 3d20          fname = 
+0001a350: 6669 6c65 6e61 6d65 0a20 2020 2020 2020  filename.       
+0001a360: 2069 6620 6669 6c65 6e61 6d65 2e65 6e64   if filename.end
+0001a370: 7377 6974 6828 494e 5055 545f 5a49 505f  swith(INPUT_ZIP_
+0001a380: 4558 5429 3a0a 2020 2020 2020 2020 2020  EXT):.          
+0001a390: 2020 666e 616d 6520 3d20 6669 6c65 6e61    fname = filena
+0001a3a0: 6d65 5b3a 2d6c 656e 2849 4e50 5554 5f5a  me[:-len(INPUT_Z
+0001a3b0: 4950 5f45 5854 295d 0a20 2020 2020 2020  IP_EXT)].       
+0001a3c0: 2065 7874 5f70 6f73 203d 2066 6e61 6d65   ext_pos = fname
+0001a3d0: 2e72 6669 6e64 2822 2e22 290a 2020 2020  .rfind(".").    
+0001a3e0: 2020 2020 6966 2065 7874 5f70 6f73 203e      if ext_pos >
+0001a3f0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0001a400: 2065 7874 203d 2066 696c 656e 616d 655b   ext = filename[
+0001a410: 6578 745f 706f 7320 2b20 313a 5d20 2023  ext_pos + 1:]  #
+0001a420: 2066 756c 6c20 6669 6c65 6e61 6d65 0a20   full filename. 
+0001a430: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001a440: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0001a450: 616c 7565 4572 726f 7228 2263 6f75 6c64  alueError("could
+0001a460: 206e 6f74 2064 6574 6572 6d69 6e65 2065   not determine e
+0001a470: 7874 656e 7369 6f6e 2229 0a20 2020 2020  xtension").     
+0001a480: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001a490: 2020 2020 7769 7468 206f 7065 6e28 6669      with open(fi
+0001a4a0: 6c65 6e61 6d65 2c20 2272 6222 2920 6173  lename, "rb") as
+0001a4b0: 2066 6275 6666 3a0a 2020 2020 2020 2020   fbuff:.        
+0001a4c0: 2020 2020 2020 2020 7365 6c66 2e5f 7570          self._up
+0001a4d0: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001a4f0: 6275 6666 2c0a 2020 2020 2020 2020 2020  buff,.          
+0001a500: 2020 2020 2020 2020 2020 6d61 785f 7468            max_th
+0001a510: 7265 6164 732c 0a20 2020 2020 2020 2020  reads,.         
+0001a520: 2020 2020 2020 2020 2020 2065 7874 3d65             ext=e
+0001a530: 7874 2c0a 2020 2020 2020 2020 2020 2020  xt,.            
+0001a540: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
+0001a550: 5f62 6172 3d70 726f 6772 6573 735f 6261  _bar=progress_ba
+0001a560: 7229 0a20 2020 2020 2020 2020 2020 2072  r).            r
+0001a570: 6574 7572 6e20 7365 6c66 2e66 696e 6973  eturn self.finis
+0001a580: 685f 6373 765f 7570 6c6f 6164 2866 696c  h_csv_upload(fil
+0001a590: 656e 616d 6529 0a20 2020 2020 2020 2066  ename).        f
+0001a5a0: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
+0001a5b0: 2020 2020 6966 2072 6571 7565 7565 5f6f      if requeue_o
+0001a5c0: 6e5f 6669 6e69 7368 2069 7320 6e6f 7420  n_finish is not 
+0001a5d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001a5e0: 2020 2020 2020 7265 7175 6575 655f 6f6e        requeue_on
+0001a5f0: 5f66 696e 6973 682e 7265 7175 6575 6528  _finish.requeue(
+0001a600: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001a610: 6c66 2e5f 636c 6561 725f 7570 6c6f 6164  lf._clear_upload
+0001a620: 2829 0a0a 2020 2020 6465 6620 6164 645f  ()..    def add_
+0001a630: 6672 6f6d 5f64 6628 0a20 2020 2020 2020  from_df(.       
+0001a640: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0001a650: 2020 2020 2020 2064 663a 2070 642e 4461         df: pd.Da
+0001a660: 7461 4672 616d 652c 0a20 2020 2020 2020  taFrame,.       
+0001a670: 2020 2020 2070 726f 6772 6573 735f 6261       progress_ba
+0001a680: 723a 204f 7074 696f 6e61 6c5b 494f 5b41  r: Optional[IO[A
+0001a690: 6e79 5d5d 203d 2073 7973 2e73 7464 6f75  ny]] = sys.stdou
+0001a6a0: 742c 0a20 2020 2020 2020 2020 2020 2072  t,.            r
+0001a6b0: 6571 7565 7565 5f6f 6e5f 6669 6e69 7368  equeue_on_finish
+0001a6c0: 3a20 4f70 7469 6f6e 616c 5b4e 6f64 6548  : Optional[NodeH
+0001a6d0: 616e 646c 655d 203d 204e 6f6e 652c 0a20  andle] = None,. 
+0001a6e0: 2020 2020 2020 2020 2020 206d 6178 5f74             max_t
+0001a6f0: 6872 6561 6473 3a20 696e 7420 3d20 3130  hreads: int = 10
+0001a700: 2920 2d3e 204f 7074 696f 6e61 6c5b 5570  ) -> Optional[Up
+0001a710: 6c6f 6164 4669 6c65 7352 6573 706f 6e73  loadFilesRespons
+0001a720: 655d 3a0a 2020 2020 2020 2020 696f 5f69  e]:.        io_i
+0001a730: 6e20 3d20 4e6f 6e65 0a20 2020 2020 2020  n = None.       
+0001a740: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0001a750: 2020 696f 5f69 6e20 3d20 6466 5f74 6f5f    io_in = df_to_
+0001a760: 6373 765f 6279 7465 7328 6466 290a 2020  csv_bytes(df).  
+0001a770: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001a780: 7570 6c6f 6164 5f66 696c 6528 0a20 2020  upload_file(.   
+0001a790: 2020 2020 2020 2020 2020 2020 2069 6f5f               io_
+0001a7a0: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+0001a7b0: 2020 2020 6d61 785f 7468 7265 6164 732c      max_threads,
+0001a7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7d0: 2065 7874 3d22 6373 7622 2c0a 2020 2020   ext="csv",.    
+0001a7e0: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
+0001a7f0: 7265 7373 5f62 6172 3d70 726f 6772 6573  ress_bar=progres
+0001a800: 735f 6261 7229 0a20 2020 2020 2020 2020  s_bar).         
+0001a810: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+0001a820: 696e 6973 685f 6373 765f 7570 6c6f 6164  inish_csv_upload
+0001a830: 2829 0a20 2020 2020 2020 2066 696e 616c  ().        final
+0001a840: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
+0001a850: 6966 2072 6571 7565 7565 5f6f 6e5f 6669  if requeue_on_fi
+0001a860: 6e69 7368 2069 7320 6e6f 7420 4e6f 6e65  nish is not None
+0001a870: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a880: 2020 7265 7175 6575 655f 6f6e 5f66 696e    requeue_on_fin
+0001a890: 6973 682e 7265 7175 6575 6528 290a 2020  ish.requeue().  
+0001a8a0: 2020 2020 2020 2020 2020 6966 2069 6f5f            if io_
+0001a8b0: 696e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  in is not None:.
+0001a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8d0: 696f 5f69 6e2e 636c 6f73 6528 290a 2020  io_in.close().  
+0001a8e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001a8f0: 636c 6561 725f 7570 6c6f 6164 2829 0a0a  clear_upload()..
+0001a900: 2020 2020 6465 6620 6164 645f 6672 6f6d      def add_from
+0001a910: 5f63 6f6e 7465 6e74 280a 2020 2020 2020  _content(.      
+0001a920: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0001a930: 2020 2020 2020 2020 636f 6e74 656e 743a          content:
+0001a940: 2055 6e69 6f6e 5b62 7974 6573 2c20 7374   Union[bytes, st
+0001a950: 722c 2070 642e 4461 7461 4672 616d 655d  r, pd.DataFrame]
+0001a960: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
+0001a970: 6f67 7265 7373 5f62 6172 3a20 4f70 7469  ogress_bar: Opti
+0001a980: 6f6e 616c 5b49 4f5b 416e 795d 5d20 3d20  onal[IO[Any]] = 
+0001a990: 7379 732e 7374 646f 7574 2c0a 2020 2020  sys.stdout,.    
+0001a9a0: 2020 2020 2020 2020 7265 7175 6575 655f          requeue_
+0001a9b0: 6f6e 5f66 696e 6973 683a 204f 7074 696f  on_finish: Optio
+0001a9c0: 6e61 6c5b 4e6f 6465 4861 6e64 6c65 5d20  nal[NodeHandle] 
+0001a9d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0001a9e0: 2020 2020 6d61 785f 7468 7265 6164 733a      max_threads:
+0001a9f0: 2069 6e74 203d 2031 3029 202d 3e20 4f70   int = 10) -> Op
+0001aa00: 7469 6f6e 616c 5b55 706c 6f61 6446 696c  tional[UploadFil
+0001aa10: 6573 5265 7370 6f6e 7365 5d3a 0a20 2020  esResponse]:.   
+0001aa20: 2020 2020 2069 6f5f 696e 203d 204e 6f6e       io_in = Non
+0001aa30: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
+0001aa40: 2020 2020 2020 2020 2020 2069 6f5f 696e             io_in
+0001aa50: 203d 2063 6f6e 7465 6e74 5f74 6f5f 6373   = content_to_cs
+0001aa60: 765f 6279 7465 7328 636f 6e74 656e 7429  v_bytes(content)
+0001aa70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001aa80: 662e 5f75 706c 6f61 645f 6669 6c65 280a  f._upload_file(.
+0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aaa0: 696f 5f69 6e2c 0a20 2020 2020 2020 2020  io_in,.         
+0001aab0: 2020 2020 2020 206d 6178 5f74 6872 6561         max_threa
+0001aac0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+0001aad0: 2020 2020 6578 743d 2263 7376 222c 0a20      ext="csv",. 
+0001aae0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001aaf0: 726f 6772 6573 735f 6261 723d 7072 6f67  rogress_bar=prog
+0001ab00: 7265 7373 5f62 6172 290a 2020 2020 2020  ress_bar).      
+0001ab10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001ab20: 662e 6669 6e69 7368 5f63 7376 5f75 706c  f.finish_csv_upl
+0001ab30: 6f61 6428 290a 2020 2020 2020 2020 6669  oad().        fi
+0001ab40: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+0001ab50: 2020 2069 6620 7265 7175 6575 655f 6f6e     if requeue_on
+0001ab60: 5f66 696e 6973 6820 6973 206e 6f74 204e  _finish is not N
+0001ab70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001ab80: 2020 2020 2072 6571 7565 7565 5f6f 6e5f       requeue_on_
+0001ab90: 6669 6e69 7368 2e72 6571 7565 7565 2829  finish.requeue()
+0001aba0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001abb0: 696f 5f69 6e20 6973 206e 6f74 204e 6f6e  io_in is not Non
+0001abc0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001abd0: 2020 2069 6f5f 696e 2e63 6c6f 7365 2829     io_in.close()
+0001abe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001abf0: 662e 5f63 6c65 6172 5f75 706c 6f61 6428  f._clear_upload(
+0001ac00: 290a 0a23 202a 2a2a 2043 5356 426c 6f62  )..# *** CSVBlob
+0001ac10: 4861 6e64 6c65 202a 2a2a 0a0a 0a63 6c61  Handle ***...cla
+0001ac20: 7373 2054 6f72 6368 426c 6f62 4861 6e64  ss TorchBlobHand
+0001ac30: 6c65 2842 6c6f 6248 616e 646c 6529 3a0a  le(BlobHandle):.
+0001ac40: 2020 2020 6465 6620 6669 6e69 7368 5f74      def finish_t
+0001ac50: 6f72 6368 5f75 706c 6f61 6428 0a20 2020  orch_upload(.   
+0001ac60: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+0001ac70: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+0001ac80: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+0001ac90: 725d 203d 204e 6f6e 6529 202d 3e20 5570  r] = None) -> Up
+0001aca0: 6c6f 6164 4669 6c65 7352 6573 706f 6e73  loadFilesRespons
+0001acb0: 653a 0a20 2020 2020 2020 2074 6d70 5f75  e:.        tmp_u
+0001acc0: 7269 203d 2073 656c 662e 5f74 6d70 5f75  ri = self._tmp_u
+0001acd0: 7269 0a20 2020 2020 2020 2069 6620 746d  ri.        if tm
+0001ace0: 705f 7572 6920 6973 204e 6f6e 653a 0a20  p_uri is None:. 
+0001acf0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0001ad00: 2056 616c 7565 4572 726f 7228 2274 6d70   ValueError("tmp
+0001ad10: 5f75 7269 2069 7320 4e6f 6e65 2229 0a20  _uri is None"). 
+0001ad20: 2020 2020 2020 2061 7267 733a 2044 6963         args: Dic
+0001ad30: 745b 7374 722c 204f 7074 696f 6e61 6c5b  t[str, Optional[
+0001ad40: 556e 696f 6e5b 7374 722c 2069 6e74 5d5d  Union[str, int]]
+0001ad50: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
+0001ad60: 2020 2274 6d70 5f75 7269 223a 2074 6d70    "tmp_uri": tmp
+0001ad70: 5f75 7269 2c0a 2020 2020 2020 2020 2020  _uri,.          
+0001ad80: 2020 2274 6f72 6368 5f75 7269 223a 2073    "torch_uri": s
+0001ad90: 656c 662e 6765 745f 7572 6928 292c 0a20  elf.get_uri(),. 
+0001ada0: 2020 2020 2020 2020 2020 2022 6f77 6e65             "owne
+0001adb0: 725f 6461 6722 3a20 7365 6c66 2e67 6574  r_dag": self.get
+0001adc0: 5f6f 776e 6572 5f64 6167 2829 2c0a 2020  _owner_dag(),.  
+0001add0: 2020 2020 2020 2020 2020 226f 776e 6572            "owner
+0001ade0: 5f6e 6f64 6522 3a20 7365 6c66 2e67 6574  _node": self.get
+0001adf0: 5f6f 776e 6572 5f6e 6f64 6528 292c 0a20  _owner_node(),. 
+0001ae00: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+0001ae10: 6e61 6d65 223a 2066 696c 656e 616d 652c  name": filename,
+0001ae20: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0001ae30: 2020 2072 6574 7572 6e20 6361 7374 2855     return cast(U
+0001ae40: 706c 6f61 6446 696c 6573 5265 7370 6f6e  ploadFilesRespon
+0001ae50: 7365 2c20 7365 6c66 2e5f 636c 6965 6e74  se, self._client
+0001ae60: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+0001ae70: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+0001ae80: 445f 504f 5354 2c20 222f 6669 6e69 7368  D_POST, "/finish
+0001ae90: 5f74 6f72 6368 222c 2061 7267 7329 290a  _torch", args)).
+0001aea0: 0a20 2020 2064 6566 2061 6464 5f66 726f  .    def add_fro
+0001aeb0: 6d5f 6669 6c65 280a 2020 2020 2020 2020  m_file(.        
+0001aec0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0001aed0: 2020 2020 2020 6669 6c65 6e61 6d65 3a20        filename: 
+0001aee0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0001aef0: 2070 726f 6772 6573 735f 6261 723a 204f   progress_bar: O
+0001af00: 7074 696f 6e61 6c5b 494f 5b41 6e79 5d5d  ptional[IO[Any]]
+0001af10: 203d 2073 7973 2e73 7464 6f75 742c 0a20   = sys.stdout,. 
+0001af20: 2020 2020 2020 2020 2020 206d 6178 5f74             max_t
+0001af30: 6872 6561 6473 3a20 696e 7420 3d20 3130  hreads: int = 10
+0001af40: 2920 2d3e 204f 7074 696f 6e61 6c5b 5570  ) -> Optional[Up
+0001af50: 6c6f 6164 4669 6c65 7352 6573 706f 6e73  loadFilesRespons
+0001af60: 655d 3a0a 2020 2020 2020 2020 666e 616d  e]:.        fnam
+0001af70: 6520 3d20 6669 6c65 6e61 6d65 0a20 2020  e = filename.   
+0001af80: 2020 2020 2069 6620 6669 6c65 6e61 6d65       if filename
+0001af90: 2e65 6e64 7377 6974 6828 494e 5055 545f  .endswith(INPUT_
+0001afa0: 5a49 505f 4558 5429 3a0a 2020 2020 2020  ZIP_EXT):.      
+0001afb0: 2020 2020 2020 666e 616d 6520 3d20 6669        fname = fi
+0001afc0: 6c65 6e61 6d65 5b3a 2d6c 656e 2849 4e50  lename[:-len(INP
+0001afd0: 5554 5f5a 4950 5f45 5854 295d 0a20 2020  UT_ZIP_EXT)].   
+0001afe0: 2020 2020 2065 7874 5f70 6f73 203d 2066       ext_pos = f
+0001aff0: 6e61 6d65 2e72 6669 6e64 2822 2e22 290a  name.rfind(".").
+0001b000: 2020 2020 2020 2020 6966 2065 7874 5f70          if ext_p
+0001b010: 6f73 203e 3d20 303a 0a20 2020 2020 2020  os >= 0:.       
+0001b020: 2020 2020 2065 7874 203d 2066 696c 656e       ext = filen
+0001b030: 616d 655b 6578 745f 706f 7320 2b20 313a  ame[ext_pos + 1:
+0001b040: 5d20 2023 2066 756c 6c20 6669 6c65 6e61  ]  # full filena
+0001b050: 6d65 0a20 2020 2020 2020 2065 6c73 653a  me.        else:
+0001b060: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001b070: 7365 2056 616c 7565 4572 726f 7228 2263  se ValueError("c
+0001b080: 6f75 6c64 206e 6f74 2064 6574 6572 6d69  ould not determi
+0001b090: 6e65 2065 7874 656e 7369 6f6e 2229 0a20  ne extension"). 
+0001b0a0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001b0b0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0001b0c0: 6e28 6669 6c65 6e61 6d65 2c20 2272 6222  n(filename, "rb"
+0001b0d0: 2920 6173 2066 6275 6666 3a0a 2020 2020  ) as fbuff:.    
+0001b0e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b0f0: 2e5f 7570 6c6f 6164 5f66 696c 6528 0a20  ._upload_file(. 
+0001b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b110: 2020 2066 6275 6666 2c0a 2020 2020 2020     fbuff,.      
+0001b120: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+0001b130: 785f 7468 7265 6164 732c 0a20 2020 2020  x_threads,.     
+0001b140: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001b150: 7874 3d65 7874 2c0a 2020 2020 2020 2020  xt=ext,.        
+0001b160: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
+0001b170: 7265 7373 5f62 6172 3d70 726f 6772 6573  ress_bar=progres
+0001b180: 735f 6261 7229 0a20 2020 2020 2020 2020  s_bar).         
+0001b190: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+0001b1a0: 696e 6973 685f 746f 7263 685f 7570 6c6f  inish_torch_uplo
+0001b1b0: 6164 2866 696c 656e 616d 6529 0a20 2020  ad(filename).   
+0001b1c0: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
+0001b1d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001b1e0: 636c 6561 725f 7570 6c6f 6164 2829 0a0a  clear_upload()..
+0001b1f0: 2320 2a2a 2a20 546f 7263 6842 6c6f 6248  # *** TorchBlobH
+0001b200: 616e 646c 6520 2a2a 2a0a 0a0a 636c 6173  andle ***...clas
+0001b210: 7320 4a53 4f4e 426c 6f62 4861 6e64 6c65  s JSONBlobHandle
+0001b220: 2842 6c6f 6248 616e 646c 6529 3a0a 2020  (BlobHandle):.  
+0001b230: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0001b240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b250: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+0001b260: 6965 6e74 3a20 5859 4d45 436c 6965 6e74  ient: XYMEClient
+0001b270: 2c0a 2020 2020 2020 2020 2020 2020 7572  ,.            ur
+0001b280: 693a 2073 7472 2c0a 2020 2020 2020 2020  i: str,.        
+0001b290: 2020 2020 6973 5f66 756c 6c3a 2062 6f6f      is_full: boo
+0001b2a0: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+0001b2b0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0001b2c0: 6974 5f5f 2863 6c69 656e 742c 2075 7269  it__(client, uri
+0001b2d0: 2c20 6973 5f66 756c 6c29 0a20 2020 2020  , is_full).     
+0001b2e0: 2020 2073 656c 662e 5f63 6f75 6e74 3a20     self._count: 
+0001b2f0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0001b300: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
+0001b310: 745f 636f 756e 7428 7365 6c66 2920 2d3e  t_count(self) ->
+0001b320: 204f 7074 696f 6e61 6c5b 696e 745d 3a0a   Optional[int]:.
+0001b330: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001b340: 656c 662e 5f63 6f75 6e74 0a0a 2020 2020  elf._count..    
+0001b350: 6465 6620 6170 7065 6e64 5f6a 736f 6e73  def append_jsons
+0001b360: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0001b370: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0001b380: 6a73 6f6e 733a 204c 6973 745b 416e 795d  jsons: List[Any]
+0001b390: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+0001b3a0: 7175 6575 655f 6f6e 5f66 696e 6973 683a  queue_on_finish:
+0001b3b0: 204f 7074 696f 6e61 6c5b 4e6f 6465 4861   Optional[NodeHa
+0001b3c0: 6e64 6c65 5d20 3d20 4e6f 6e65 2c0a 2020  ndle] = None,.  
+0001b3d0: 2020 2020 2020 2020 2020 2920 2d3e 204e            ) -> N
+0001b3e0: 6f6e 653a 0a20 2020 2020 2020 206f 626a  one:.        obj
+0001b3f0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0001b400: 2022 626c 6f62 223a 2073 656c 662e 6765   "blob": self.ge
+0001b410: 745f 7572 6928 292c 0a20 2020 2020 2020  t_uri(),.       
+0001b420: 2020 2020 2022 6a73 6f6e 7322 3a20 6a73       "jsons": js
+0001b430: 6f6e 732c 0a20 2020 2020 2020 207d 0a20  ons,.        }. 
+0001b440: 2020 2020 2020 2069 6620 7265 7175 6575         if requeu
+0001b450: 655f 6f6e 5f66 696e 6973 6820 6973 206e  e_on_finish is n
+0001b460: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0001b470: 2020 2020 206f 626a 5b22 6461 6722 5d20       obj["dag"] 
+0001b480: 3d20 7265 7175 6575 655f 6f6e 5f66 696e  = requeue_on_fin
+0001b490: 6973 682e 6765 745f 6461 6728 292e 6765  ish.get_dag().ge
+0001b4a0: 745f 7572 6928 290a 2020 2020 2020 2020  t_uri().        
+0001b4b0: 2020 2020 6f62 6a5b 226e 6f64 6522 5d20      obj["node"] 
+0001b4c0: 3d20 7265 7175 6575 655f 6f6e 5f66 696e  = requeue_on_fin
+0001b4d0: 6973 682e 6765 745f 6964 2829 0a20 2020  ish.get_id().   
+0001b4e0: 2020 2020 2072 6573 203d 2063 6173 7428       res = cast(
+0001b4f0: 4a53 4f4e 426c 6f62 4170 7065 6e64 5265  JSONBlobAppendRe
+0001b500: 7370 6f6e 7365 2c20 7365 6c66 2e5f 636c  sponse, self._cl
+0001b510: 6965 6e74 2e72 6571 7565 7374 5f6a 736f  ient.request_jso
+0001b520: 6e28 0a20 2020 2020 2020 2020 2020 204d  n(.            M
+0001b530: 4554 484f 445f 5055 542c 2022 2f6a 736f  ETHOD_PUT, "/jso
+0001b540: 6e5f 6170 7065 6e64 222c 206f 626a 2929  n_append", obj))
+0001b550: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+0001b560: 6f75 6e74 203d 2072 6573 5b22 636f 756e  ount = res["coun
+0001b570: 7422 5d0a 0a23 202a 2a2a 204a 534f 4e42  t"]..# *** JSONB
+0001b580: 6c6f 6248 616e 646c 6520 2a2a 2a0a 0a0a  lobHandle ***...
+0001b590: 636c 6173 7320 4375 7374 6f6d 436f 6465  class CustomCode
+0001b5a0: 426c 6f62 4861 6e64 6c65 2842 6c6f 6248  BlobHandle(BlobH
+0001b5b0: 616e 646c 6529 3a0a 2020 2020 6465 6620  andle):.    def 
+0001b5c0: 7365 745f 6375 7374 6f6d 5f69 6d70 6f72  set_custom_impor
+0001b5d0: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
+0001b5e0: 7365 6c66 2c20 6d6f 6475 6c65 733a 204c  self, modules: L
+0001b5f0: 6973 745b 4c69 7374 5b73 7472 5d5d 2920  ist[List[str]]) 
+0001b600: 2d3e 204e 6f64 6543 7573 746f 6d49 6d70  -> NodeCustomImp
+0001b610: 6f72 7473 3a0a 2020 2020 2020 2020 7265  orts:.        re
+0001b620: 7475 726e 2063 6173 7428 4e6f 6465 4375  turn cast(NodeCu
+0001b630: 7374 6f6d 496d 706f 7274 732c 2073 656c  stomImports, sel
+0001b640: 662e 5f63 6c69 656e 742e 7265 7175 6573  f._client.reques
+0001b650: 745f 6a73 6f6e 280a 2020 2020 2020 2020  t_json(.        
+0001b660: 2020 2020 4d45 5448 4f44 5f50 5554 2c20      METHOD_PUT, 
+0001b670: 222f 6375 7374 6f6d 5f69 6d70 6f72 7473  "/custom_imports
+0001b680: 222c 207b 0a20 2020 2020 2020 2020 2020  ", {.           
+0001b690: 2020 2020 2022 6461 6722 3a20 7365 6c66       "dag": self
+0001b6a0: 2e67 6574 5f6f 776e 6572 5f64 6167 2829  .get_owner_dag()
+0001b6b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b6c0: 2020 226e 6f64 6522 3a20 7365 6c66 2e67    "node": self.g
+0001b6d0: 6574 5f6f 776e 6572 5f6e 6f64 6528 292c  et_owner_node(),
+0001b6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b6f0: 2022 6d6f 6475 6c65 7322 3a20 6d6f 6475   "modules": modu
+0001b700: 6c65 732c 0a20 2020 2020 2020 2020 2020  les,.           
+0001b710: 207d 2929 0a0a 2020 2020 6465 6620 6765   }))..    def ge
+0001b720: 745f 6375 7374 6f6d 5f69 6d70 6f72 7473  t_custom_imports
+0001b730: 2873 656c 6629 202d 3e20 4e6f 6465 4375  (self) -> NodeCu
+0001b740: 7374 6f6d 496d 706f 7274 733a 0a20 2020  stomImports:.   
+0001b750: 2020 2020 2072 6574 7572 6e20 6361 7374       return cast
+0001b760: 284e 6f64 6543 7573 746f 6d49 6d70 6f72  (NodeCustomImpor
+0001b770: 7473 2c20 7365 6c66 2e5f 636c 6965 6e74  ts, self._client
+0001b780: 2e72 6571 7565 7374 5f6a 736f 6e28 0a20  .request_json(. 
+0001b790: 2020 2020 2020 2020 2020 204d 4554 484f             METHO
+0001b7a0: 445f 4745 542c 2022 2f63 7573 746f 6d5f  D_GET, "/custom_
+0001b7b0: 696d 706f 7274 7322 2c20 7b0a 2020 2020  imports", {.    
+0001b7c0: 2020 2020 2020 2020 2020 2020 2264 6167              "dag
+0001b7d0: 223a 2073 656c 662e 6765 745f 6f77 6e65  ": self.get_owne
+0001b7e0: 725f 6461 6728 292c 0a20 2020 2020 2020  r_dag(),.       
+0001b7f0: 2020 2020 2020 2020 2022 6e6f 6465 223a           "node":
+0001b800: 2073 656c 662e 6765 745f 6f77 6e65 725f   self.get_owner_
+0001b810: 6e6f 6465 2829 2c0a 2020 2020 2020 2020  node(),.        
+0001b820: 2020 2020 7d29 290a 0a20 2020 2064 6566      }))..    def
+0001b830: 2073 6574 5f63 7573 746f 6d5f 636f 6465   set_custom_code
+0001b840: 2873 656c 662c 2066 756e 633a 2046 554e  (self, func: FUN
+0001b850: 4329 202d 3e20 4e6f 6465 4375 7374 6f6d  C) -> NodeCustom
+0001b860: 436f 6465 3a0a 2020 2020 2020 2020 6672  Code:.        fr
+0001b870: 6f6d 2052 6573 7472 6963 7465 6450 7974  om RestrictedPyt
+0001b880: 686f 6e20 696d 706f 7274 2063 6f6d 7069  hon import compi
+0001b890: 6c65 5f72 6573 7472 6963 7465 640a 0a20  le_restricted.. 
+0001b8a0: 2020 2020 2020 2064 6566 2066 6e5f 6173         def fn_as
+0001b8b0: 5f73 7472 2866 756e 3a20 4655 4e43 2920  _str(fun: FUNC) 
+0001b8c0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+0001b8d0: 2020 2020 626f 6479 203d 2074 6578 7477      body = textw
+0001b8e0: 7261 702e 6465 6465 6e74 2869 6e73 7065  rap.dedent(inspe
+0001b8f0: 6374 2e67 6574 736f 7572 6365 2866 756e  ct.getsource(fun
+0001b900: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0001b910: 6573 203d 2062 6f64 7920 2b20 7465 7874  es = body + text
+0001b920: 7772 6170 2e64 6564 656e 7428 6622 2222  wrap.dedent(f"""
+0001b930: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0001b940: 756c 7420 3d20 7b66 756e 2e5f 5f6e 616d  ult = {fun.__nam
+0001b950: 655f 5f7d 282a 6461 7461 2c20 2a2a 6b77  e__}(*data, **kw
+0001b960: 6172 6773 290a 2020 2020 2020 2020 2020  args).          
+0001b970: 2020 6966 2072 6573 756c 7420 6973 204e    if result is N
+0001b980: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001b990: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0001b9a0: 4572 726f 7228 227b 6675 6e2e 5f5f 6e61  Error("{fun.__na
+0001b9b0: 6d65 5f5f 7d20 6d75 7374 2072 6574 7572  me__} must retur
+0001b9c0: 6e20 6120 7661 6c75 6522 290a 2020 2020  n a value").    
+0001b9d0: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
+0001b9e0: 2020 2020 2020 2020 2063 6f6d 7069 6c65           compile
+0001b9f0: 5f72 6573 7472 6963 7465 6428 7265 732c  _restricted(res,
+0001ba00: 2022 696e 6c69 6e65 222c 2022 6578 6563   "inline", "exec
+0001ba10: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0001ba20: 6574 7572 6e20 7265 730a 0a20 2020 2020  eturn res..     
+0001ba30: 2020 2072 6177 5f63 6f64 6520 3d20 666e     raw_code = fn
+0001ba40: 5f61 735f 7374 7228 6675 6e63 290a 2020  _as_str(func).  
+0001ba50: 2020 2020 2020 7265 7475 726e 2063 6173        return cas
+0001ba60: 7428 4e6f 6465 4375 7374 6f6d 436f 6465  t(NodeCustomCode
+0001ba70: 2c20 7365 6c66 2e5f 636c 6965 6e74 2e72  , self._client.r
+0001ba80: 6571 7565 7374 5f6a 736f 6e28 0a20 2020  equest_json(.   
+0001ba90: 2020 2020 2020 2020 204d 4554 484f 445f           METHOD_
+0001baa0: 5055 542c 2022 2f63 7573 746f 6d5f 636f  PUT, "/custom_co
+0001bab0: 6465 222c 207b 0a20 2020 2020 2020 2020  de", {.         
+0001bac0: 2020 2020 2020 2022 6461 6722 3a20 7365         "dag": se
+0001bad0: 6c66 2e67 6574 5f6f 776e 6572 5f64 6167  lf.get_owner_dag
+0001bae0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+0001baf0: 2020 2020 226e 6f64 6522 3a20 7365 6c66      "node": self
+0001bb00: 2e67 6574 5f6f 776e 6572 5f6e 6f64 6528  .get_owner_node(
+0001bb10: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001bb20: 2020 2022 636f 6465 223a 2072 6177 5f63     "code": raw_c
+0001bb30: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
+0001bb40: 207d 2929 0a0a 2020 2020 6465 6620 6765   }))..    def ge
+0001bb50: 745f 6375 7374 6f6d 5f63 6f64 6528 7365  t_custom_code(se
+0001bb60: 6c66 2920 2d3e 204e 6f64 6543 7573 746f  lf) -> NodeCusto
+0001bb70: 6d43 6f64 653a 0a20 2020 2020 2020 2072  mCode:.        r
+0001bb80: 6574 7572 6e20 6361 7374 284e 6f64 6543  eturn cast(NodeC
+0001bb90: 7573 746f 6d43 6f64 652c 2073 656c 662e  ustomCode, self.
+0001bba0: 5f63 6c69 656e 742e 7265 7175 6573 745f  _client.request_
+0001bbb0: 6a73 6f6e 280a 2020 2020 2020 2020 2020  json(.          
+0001bbc0: 2020 4d45 5448 4f44 5f47 4554 2c20 222f    METHOD_GET, "/
+0001bbd0: 6375 7374 6f6d 5f63 6f64 6522 2c20 7b0a  custom_code", {.
+0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbf0: 2264 6167 223a 2073 656c 662e 6765 745f  "dag": self.get_
+0001bc00: 6f77 6e65 725f 6461 6728 292c 0a20 2020  owner_dag(),.   
+0001bc10: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
+0001bc20: 6465 223a 2073 656c 662e 6765 745f 6f77  de": self.get_ow
+0001bc30: 6e65 725f 6e6f 6465 2829 2c0a 2020 2020  ner_node(),.    
+0001bc40: 2020 2020 2020 2020 7d29 290a 0a23 202a          }))..# *
+0001bc50: 2a2a 2043 7573 746f 6d43 6f64 6542 6c6f  ** CustomCodeBlo
+0001bc60: 6248 616e 646c 6520 2a2a 2a0a 0a0a 636c  bHandle ***...cl
+0001bc70: 6173 7320 436f 6d70 7574 6174 696f 6e48  ass ComputationH
+0001bc80: 616e 646c 653a 0a20 2020 2064 6566 205f  andle:.    def _
+0001bc90: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0001bca0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0001bcb0: 2020 2020 2020 2064 6167 3a20 4461 6748         dag: DagH
+0001bcc0: 616e 646c 652c 0a20 2020 2020 2020 2020  andle,.         
+0001bcd0: 2020 2076 616c 7565 5f69 643a 2073 7472     value_id: str
+0001bce0: 2c0a 2020 2020 2020 2020 2020 2020 6765  ,.            ge
+0001bcf0: 745f 6479 6e5f 6572 726f 723a 2043 616c  t_dyn_error: Cal
+0001bd00: 6c61 626c 655b 5b5d 2c20 4f70 7469 6f6e  lable[[], Option
+0001bd10: 616c 5b73 7472 5d5d 2c0a 2020 2020 2020  al[str]],.      
+0001bd20: 2020 2020 2020 7365 745f 6479 6e5f 6572        set_dyn_er
+0001bd30: 726f 723a 2043 616c 6c61 626c 655b 5b73  ror: Callable[[s
+0001bd40: 7472 5d2c 204e 6f6e 655d 2920 2d3e 204e  tr], None]) -> N
+0001bd50: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
+0001bd60: 662e 5f64 6167 203d 2064 6167 0a20 2020  f._dag = dag.   
+0001bd70: 2020 2020 2073 656c 662e 5f76 616c 7565       self._value
+0001bd80: 5f69 6420 3d20 7661 6c75 655f 6964 0a20  _id = value_id. 
+0001bd90: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+0001bda0: 7565 3a20 4f70 7469 6f6e 616c 5b42 7974  ue: Optional[Byt
+0001bdb0: 6552 6573 706f 6e73 655d 203d 204e 6f6e  eResponse] = Non
+0001bdc0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0001bdd0: 6765 745f 6479 6e5f 6572 726f 7220 3d20  get_dyn_error = 
+0001bde0: 6765 745f 6479 6e5f 6572 726f 720a 2020  get_dyn_error.  
+0001bdf0: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
+0001be00: 6479 6e5f 6572 726f 7220 3d20 7365 745f  dyn_error = set_
+0001be10: 6479 6e5f 6572 726f 720a 0a20 2020 2064  dyn_error..    d
+0001be20: 6566 2068 6173 5f66 6574 6368 6564 2873  ef has_fetched(s
+0001be30: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0001be40: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001be50: 662e 5f76 616c 7565 2069 7320 6e6f 7420  f._value is not 
+0001be60: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
+0001be70: 7428 7365 6c66 2920 2d3e 204f 7074 696f  t(self) -> Optio
+0001be80: 6e61 6c5b 4279 7465 5265 7370 6f6e 7365  nal[ByteResponse
+0001be90: 5d3a 0a20 2020 2020 2020 2074 7279 3a0a  ]:.        try:.
+0001bea0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001beb0: 656c 662e 5f76 616c 7565 2069 7320 4e6f  elf._value is No
+0001bec0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001bed0: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
+0001bee0: 3d20 7365 6c66 2e5f 6461 672e 6765 745f  = self._dag.get_
+0001bef0: 6479 6e61 6d69 635f 7265 7375 6c74 2873  dynamic_result(s
+0001bf00: 656c 662e 5f76 616c 7565 5f69 6429 0a20  elf._value_id). 
+0001bf10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001bf20: 6e20 7365 6c66 2e5f 7661 6c75 650a 2020  n self._value.  
+0001bf30: 2020 2020 2020 6578 6365 7074 2053 6572        except Ser
+0001bf40: 7665 7253 6964 6545 7272 6f72 2061 7320  verSideError as 
+0001bf50: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+0001bf60: 6620 7365 6c66 2e5f 6765 745f 6479 6e5f  f self._get_dyn_
+0001bf70: 6572 726f 7228 2920 6973 204e 6f6e 653a  error() is None:
+0001bf80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bf90: 2073 656c 662e 5f73 6574 5f64 796e 5f65   self._set_dyn_e
+0001bfa0: 7272 6f72 2873 7472 2865 2929 0a20 2020  rror(str(e)).   
+0001bfb0: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+0001bfc0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0001bfd0: 4b65 7945 7272 6f72 2061 7320 653a 0a20  KeyError as e:. 
+0001bfe0: 2020 2020 2020 2020 2020 206d 6179 6265             maybe
+0001bff0: 5f65 7272 6f72 203d 2073 656c 662e 5f67  _error = self._g
+0001c000: 6574 5f64 796e 5f65 7272 6f72 2829 0a20  et_dyn_error(). 
+0001c010: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
+0001c020: 7962 655f 6572 726f 7220 6973 206e 6f74  ybe_error is not
+0001c030: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001c040: 2020 2020 2020 2072 6169 7365 2053 6572         raise Ser
+0001c050: 7665 7253 6964 6545 7272 6f72 286d 6179  verSideError(may
+0001c060: 6265 5f65 7272 6f72 2920 6672 6f6d 2065  be_error) from e
+0001c070: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001c080: 7365 2065 0a0a 2020 2020 6465 6620 6765  se e..    def ge
+0001c090: 745f 6964 2873 656c 6629 202d 3e20 7374  t_id(self) -> st
+0001c0a0: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+0001c0b0: 6e20 7365 6c66 2e5f 7661 6c75 655f 6964  n self._value_id
+0001c0c0: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+0001c0d0: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
+0001c0e0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+0001c0f0: 7365 6c66 2e5f 7661 6c75 650a 2020 2020  self._value.    
+0001c100: 2020 2020 6966 2076 616c 7565 2069 7320      if value is 
+0001c110: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001c120: 2020 7265 7475 726e 2066 2276 616c 7565    return f"value
+0001c130: 5f69 643d 7b73 656c 662e 5f76 616c 7565  _id={self._value
+0001c140: 5f69 647d 220a 2020 2020 2020 2020 7265  _id}".        re
+0001c150: 7475 726e 2066 2276 616c 7565 287b 7479  turn f"value({ty
+0001c160: 7065 2876 616c 7565 297d 293d 7b76 616c  pe(value)})={val
+0001c170: 7565 7d22 0a0a 2020 2020 6465 6620 5f5f  ue}"..    def __
+0001c180: 7265 7072 5f5f 2873 656c 6629 202d 3e20  repr__(self) -> 
+0001c190: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
+0001c1a0: 7572 6e20 6622 7b73 656c 662e 5f5f 636c  urn f"{self.__cl
+0001c1b0: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d5b  ass__.__name__}[
+0001c1c0: 7b73 656c 662e 5f5f 7374 725f 5f28 297d  {self.__str__()}
+0001c1d0: 5d22 0a0a 2020 2020 6465 6620 5f5f 6861  ]"..    def __ha
+0001c1e0: 7368 5f5f 2873 656c 6629 202d 3e20 696e  sh__(self) -> in
+0001c1f0: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+0001c200: 6e20 6861 7368 2873 656c 662e 6765 745f  n hash(self.get_
+0001c210: 6964 2829 290a 0a20 2020 2064 6566 205f  id())..    def _
+0001c220: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
+0001c230: 723a 206f 626a 6563 7429 202d 3e20 626f  r: object) -> bo
+0001c240: 6f6c 3a0a 2020 2020 2020 2020 6966 206e  ol:.        if n
+0001c250: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
+0001c260: 6865 722c 2073 656c 662e 5f5f 636c 6173  her, self.__clas
+0001c270: 735f 5f29 3a0a 2020 2020 2020 2020 2020  s__):.          
+0001c280: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0001c290: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001c2a0: 6c66 2e67 6574 5f69 6428 2920 3d3d 206f  lf.get_id() == o
+0001c2b0: 7468 6572 2e67 6574 5f69 6428 290a 0a20  ther.get_id().. 
+0001c2c0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
+0001c2d0: 6c66 2c20 6f74 6865 723a 206f 626a 6563  lf, other: objec
+0001c2e0: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
+0001c2f0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+0001c300: 656c 662e 5f5f 6571 5f5f 286f 7468 6572  elf.__eq__(other
+0001c310: 290a 0a23 202a 2a2a 2043 6f6d 7075 7461  )..# *** Computa
+0001c320: 7469 6f6e 4861 6e64 6c65 202a 2a2a 0a0a  tionHandle ***..
+0001c330: 0a64 6566 2064 6566 6175 6c74 5f78 796d  .def default_xym
+0001c340: 655f 636c 6965 6e74 2829 202d 3e20 5859  e_client() -> XY
+0001c350: 4d45 436c 6965 6e74 3a0a 2020 2020 7265  MEClient:.    re
+0001c360: 7475 726e 2063 7265 6174 655f 7879 6d65  turn create_xyme
+0001c370: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
+0001c380: 2075 726c 3d44 4546 4155 4c54 5f55 524c   url=DEFAULT_URL
+0001c390: 2c0a 2020 2020 2020 2020 746f 6b65 6e3d  ,.        token=
+0001c3a0: 6f73 2e67 6574 656e 7628 2258 594d 455f  os.getenv("XYME_
+0001c3b0: 5345 5256 4552 5f54 4f4b 454e 2229 2c0a  SERVER_TOKEN"),.
+0001c3c0: 2020 2020 2020 2020 6e61 6d65 7370 6163          namespac
+0001c3d0: 653d 4445 4641 554c 545f 4e41 4d45 5350  e=DEFAULT_NAMESP
+0001c3e0: 4143 4529 0a0a 0a64 6566 2063 7265 6174  ACE)...def creat
+0001c3f0: 655f 7879 6d65 5f63 6c69 656e 7428 0a20  e_xyme_client(. 
+0001c400: 2020 2020 2020 2075 726c 3a20 7374 722c         url: str,
+0001c410: 0a20 2020 2020 2020 2074 6f6b 656e 3a20  .        token: 
+0001c420: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001c430: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e61  None,.        na
+0001c440: 6d65 7370 6163 653a 2073 7472 203d 2044  mespace: str = D
+0001c450: 4546 4155 4c54 5f4e 414d 4553 5041 4345  EFAULT_NAMESPACE
+0001c460: 2920 2d3e 2058 594d 4543 6c69 656e 743a  ) -> XYMEClient:
+0001c470: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+0001c480: 2020 7265 7475 726e 2058 594d 4543 6c69    return XYMECli
+0001c490: 656e 7428 7572 6c2c 2074 6f6b 656e 2c20  ent(url, token, 
+0001c4a0: 6e61 6d65 7370 6163 6529 0a20 2020 2065  namespace).    e
+0001c4b0: 7863 6570 7420 4c65 6761 6379 5665 7273  xcept LegacyVers
+0001c4c0: 696f 6e20 6173 206c 7665 3a0a 2020 2020  ion as lve:.    
+0001c4d0: 2020 2020 6170 695f 7665 7273 696f 6e20      api_version 
+0001c4e0: 3d20 6c76 652e 6765 745f 6170 695f 7665  = lve.get_api_ve
+0001c4f0: 7273 696f 6e28 290a 2020 2020 2020 2020  rsion().        
+0001c500: 6966 2061 7069 5f76 6572 7369 6f6e 203d  if api_version =
+0001c510: 3d20 333a 0a20 2020 2020 2020 2020 2020  = 3:.           
+0001c520: 2066 726f 6d20 6163 6365 726e 5f78 796d   from accern_xym
+0001c530: 652e 7633 2e61 6363 6572 6e5f 7879 6d65  e.v3.accern_xyme
+0001c540: 2069 6d70 6f72 7420 6372 6561 7465 5f78   import create_x
+0001c550: 796d 655f 636c 6965 6e74 5f76 330a 0a20  yme_client_v3.. 
+0001c560: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001c570: 6e20 6372 6561 7465 5f78 796d 655f 636c  n create_xyme_cl
+0001c580: 6965 6e74 5f76 3328 7572 6c2c 2074 6f6b  ient_v3(url, tok
+0001c590: 656e 2920 2023 2074 7970 653a 2069 676e  en)  # type: ign
+0001c5a0: 6f72 650a 2020 2020 2020 2020 7261 6973  ore.        rais
+0001c5b0: 6520 6c76 650a                           e lve.
```

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/types.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,26 @@
     "queue_mng": Optional[str],
 })
 
 
 class UserDagDef(BaseDagDef, total=False):
     default_input_key: Optional[str]
     default_output_key: Optional[str]
+    kafka_input_topic: Optional[str]
+    kafka_output_topic: Optional[str]
     uri_prefix: URIPrefix
     state_uri: str
     version_override: Optional[str]
 
 
 class DagDef(BaseDagDef):
     default_input_key: Optional[str]
     default_output_key: Optional[str]
+    kafka_input_topic: Optional[str]
+    kafka_output_topic: Optional[str]
     uri_prefix: URIPrefix
     state_uri: str
     version_override: Optional[str]
 
 
 NodeDef = TypedDict('NodeDef', {
     "blobs": Dict[str, str],
@@ -224,14 +228,16 @@
     "cur_time": float,
     "blobs": List[Tuple[str, Optional[float]]],
 })
 DagInfo = TypedDict('DagInfo', {
     "company": str,
     "high_priority": bool,
     "ins": List[str],
+    "kafka_input_topic": Optional[str],
+    "kafka_output_topic": Optional[str],
     "name": str,
     "nodes": List[NodeInfo],
     "outs": List[Tuple[str, str]],
     "queue_mng": Optional[str],
     "uri_prefix": URIPrefix,
     "state_uri": str,
     "version_override": Optional[str],
@@ -325,19 +331,21 @@
     "topics": Dict[str, Optional[str]],
     "create": bool,
 })
 KafkaTopicNames = TypedDict('KafkaTopicNames', {
     "input": Optional[str],
     "output": Optional[str],
     "error": Optional[str],
+    "error_msg": Optional[str],
 })
 KafkaMessage = TypedDict('KafkaMessage', {
     "messages": Dict[str, str],
 })
 KafkaOffsets = TypedDict('KafkaOffsets', {
+    "error_msg": int,
     "error": int,
     "input": int,
     "output": int,
 })
 KafkaGroup = TypedDict('KafkaGroup', {
     "group": str,
     "dag": str,
@@ -354,14 +362,15 @@
 })
 KafkaThroughput = TypedDict('KafkaThroughput', {
     "dag": str,
     "input": ThroughputDict,
     "output": ThroughputDict,
     "faster": Literal["input", "output", "both"],
     "errors": int,
+    "error_msgs": int,
 })
 PutNodeBlob = TypedDict('PutNodeBlob', {
     "key": str,
     "new_uri": str,
 })
 BlobOwner = TypedDict('BlobOwner', {
     "owner_dag": Optional[str],
```

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/util.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/util.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/v2/legacy.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/v2/legacy.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/v2/util.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/v2/util.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/v3/accern_xyme.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/v3/accern_xyme.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/v3/types.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/v3/types.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme/v3/util.py` & `accern_xyme-4.2.1/packages/python/accern_xyme/v3/util.py`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/PKG-INFO` & `accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accern-xyme
-Version: 4.2.0
+Version: 4.2.1
 Summary: AccernXYME is a library for easily accessing XYME via python.
 Home-page: https://github.com/Accern/accern-xyme
 Author: Accern Corp.
 Author-email: josua.krause@accern.com
 License: MIT
 Keywords: XYME AI machine learning client
 Classifier: Development Status :: 4 - Beta
@@ -19,18 +19,18 @@
 License-File: LICENSE
 
 Accern-XYME
 ===========
 
 *accern\_xyme* is a python/typescript library for accessing XYME functionality.
 
-|CircleCI|
+|GHAction|
 
-.. |CircleCI| image:: https://circleci.com/gh/Accern/accern-xyme.svg?style=svg
-   :target: https://circleci.com/gh/Accern/accern-xyme
+.. |GHAction| image:: https://github.com/Accern/accern-xyme/actions/workflows/python-app.yaml/badge.svg
+   :target: https://github.com/Accern/accern-xyme/actions/workflows/python-app.yaml/
 
 Python Usage
 ------------
 
 You can install *accern\_xyme* with pip:
 
 .. code:: sh
```

### Comparing `accern_xyme-4.2.0/packages/python/accern_xyme.egg-info/SOURCES.txt` & `accern_xyme-4.2.1/packages/python/accern_xyme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `accern_xyme-4.2.0/setup.cfg` & `accern_xyme-4.2.1/setup.cfg`

 * *Files identical despite different names*

