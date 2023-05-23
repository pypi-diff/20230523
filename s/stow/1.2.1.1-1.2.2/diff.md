# Comparing `tmp/stow-1.2.1.1.tar.gz` & `tmp/stow-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stow-1.2.1.1.tar", last modified: Mon Apr  3 10:47:22 2023, max compression
+gzip compressed data, was "stow-1.2.2.tar", last modified: Tue May 23 00:00:00 2023, max compression
```

## Comparing `stow-1.2.1.1.tar` & `stow-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.571423 stow-1.2.1.1/
--rw-rw-rw-   0        0        0    10756 2023-03-26 22:44:13.000000 stow-1.2.1.1/LICENSE
--rw-rw-rw-   0        0        0    20306 2023-04-03 10:47:22.571423 stow-1.2.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.540606 stow-1.2.1.1/docs/
--rw-rw-rw-   0        0        0    19244 2023-03-17 15:18:32.000000 stow-1.2.1.1/docs/index.md
--rw-rw-rw-   0        0        0       86 2023-03-26 22:44:13.000000 stow-1.2.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1012 2023-04-03 10:47:22.575423 stow-1.2.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.545607 stow-1.2.1.1/stow/
--rw-rw-rw-   0        0        0     1631 2023-04-03 10:28:37.000000 stow-1.2.1.1/stow/__init__.py
--rw-rw-rw-   0        0        0     4119 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/_utils.py
--rw-rw-rw-   0        0        0    19608 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/artefacts.py
--rw-rw-rw-   0        0        0     3617 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/callbacks.py
--rw-rw-rw-   0        0        0      830 2023-03-17 15:18:32.000000 stow-1.2.1.1/stow/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.564395 stow-1.2.1.1/stow/manager/
--rw-rw-rw-   0        0        0       83 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/manager/__init__.py
--rw-rw-rw-   0        0        0     9750 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/manager/abstract_methods.py
--rw-rw-rw-   0        0        0     6538 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/manager/base_managers.py
--rw-rw-rw-   0        0        0    45447 2023-04-03 10:24:10.000000 stow-1.2.1.1/stow/manager/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.566904 stow-1.2.1.1/stow/managers/
--rw-rw-rw-   0        0        0       53 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/managers/__init__.py
--rw-rw-rw-   0        0        0    21027 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/managers/amazon.py
--rw-rw-rw-   0        0        0     8038 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/managers/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.568425 stow-1.2.1.1/stow/testing/
--rw-rw-rw-   0        0        0       20 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/testing/__init__.py
--rw-rw-rw-   0        0        0      577 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/testing/mock.py
--rw-rw-rw-   0        0        0     2329 2023-03-26 22:44:13.000000 stow-1.2.1.1/stow/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.561394 stow-1.2.1.1/stow.egg-info/
--rw-rw-rw-   0        0        0    20306 2023-04-03 10:47:22.000000 stow-1.2.1.1/stow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2023-04-03 10:47:22.000000 stow-1.2.1.1/stow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 10:47:22.000000 stow-1.2.1.1/stow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-03 10:47:22.000000 stow-1.2.1.1/stow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2023-04-03 10:47:22.000000 stow-1.2.1.1/stow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-03 10:47:22.000000 stow-1.2.1.1/stow.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 10:47:22.570422 stow-1.2.1.1/tests/
--rw-rw-rw-   0        0        0     1414 2023-03-26 22:44:13.000000 stow-1.2.1.1/tests/test_callbacks.py
--rw-rw-rw-   0        0        0    26887 2023-04-03 10:23:35.000000 stow-1.2.1.1/tests/test_stateless.py
--rw-rw-rw-   0        0        0     2832 2023-03-26 22:44:13.000000 stow-1.2.1.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.817089 stow-1.2.2/
+-rw-rw-rw-   0        0        0    10756 2023-03-26 22:44:13.000000 stow-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0    20304 2023-05-23 00:00:00.817089 stow-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-05-22 22:46:32.000000 stow-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.783471 stow-1.2.2/docs/
+-rw-rw-rw-   0        0        0    19244 2023-03-17 15:18:32.000000 stow-1.2.2/docs/index.md
+-rw-rw-rw-   0        0        0       86 2023-03-26 22:44:13.000000 stow-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1024 2023-05-23 00:00:00.822243 stow-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.787984 stow-1.2.2/stow/
+-rw-rw-rw-   0        0        0     1650 2023-05-22 22:46:32.000000 stow-1.2.2/stow/__init__.py
+-rw-rw-rw-   0        0        0     4119 2023-03-26 22:44:13.000000 stow-1.2.2/stow/_utils.py
+-rw-rw-rw-   0        0        0    18852 2023-05-22 22:46:32.000000 stow-1.2.2/stow/artefacts.py
+-rw-rw-rw-   0        0        0     3617 2023-03-26 22:44:13.000000 stow-1.2.2/stow/callbacks.py
+-rw-rw-rw-   0        0        0      830 2023-03-17 15:18:32.000000 stow-1.2.2/stow/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.809091 stow-1.2.2/stow/manager/
+-rw-rw-rw-   0        0        0       83 2023-03-26 22:44:13.000000 stow-1.2.2/stow/manager/__init__.py
+-rw-rw-rw-   0        0        0    10054 2023-05-22 22:46:32.000000 stow-1.2.2/stow/manager/abstract_methods.py
+-rw-rw-rw-   0        0        0     7368 2023-05-22 22:46:32.000000 stow-1.2.2/stow/manager/base_managers.py
+-rw-rw-rw-   0        0        0    47131 2023-05-22 22:46:32.000000 stow-1.2.2/stow/manager/manager.py
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.812089 stow-1.2.2/stow/managers/
+-rw-rw-rw-   0        0        0       26 2023-05-22 22:46:32.000000 stow-1.2.2/stow/managers/__init__.py
+-rw-rw-rw-   0        0        0    21275 2023-05-22 22:46:32.000000 stow-1.2.2/stow/managers/amazon.py
+-rw-rw-rw-   0        0        0     9212 2023-05-22 22:46:32.000000 stow-1.2.2/stow/managers/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.814091 stow-1.2.2/stow/testing/
+-rw-rw-rw-   0        0        0       20 2023-03-26 22:44:13.000000 stow-1.2.2/stow/testing/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-03-26 22:44:13.000000 stow-1.2.2/stow/testing/mock.py
+-rw-rw-rw-   0        0        0     2329 2023-03-26 22:44:13.000000 stow-1.2.2/stow/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.805937 stow-1.2.2/stow.egg-info/
+-rw-rw-rw-   0        0        0    20304 2023-05-23 00:00:00.000000 stow-1.2.2/stow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-05-23 00:00:00.000000 stow-1.2.2/stow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 00:00:00.000000 stow-1.2.2/stow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-05-23 00:00:00.000000 stow-1.2.2/stow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2023-05-23 00:00:00.000000 stow-1.2.2/stow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 00:00:00.000000 stow-1.2.2/stow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 00:00:00.816091 stow-1.2.2/tests/
+-rw-rw-rw-   0        0        0     1414 2023-03-26 22:44:13.000000 stow-1.2.2/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0    28162 2023-05-22 22:46:32.000000 stow-1.2.2/tests/test_stateless.py
+-rw-rw-rw-   0        0        0     2832 2023-03-26 22:44:13.000000 stow-1.2.2/tests/test_utils.py
```

### Comparing `stow-1.2.1.1/LICENSE` & `stow-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/PKG-INFO` & `stow-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stow
-Version: 1.2.1.1
+Version: 1.2.2
 Summary: stow artefacts anywhere, with ease
 Author: Kieran Bacon
 Author-email: kieran.bacon@outlook.com
 Project-URL: Homepage, https://github.com/Kieran-Bacon/stow
 Project-URL: Documentation, https://stow.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Kieran-Bacon/stow/issues
 Keywords: aws s3 boto3 ssh os
```

### Comparing `stow-1.2.1.1/docs/index.md` & `stow-1.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/setup.cfg` & `stow-1.2.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 746f 770d 0a76 6572 7369 6f6e   = stow..version
-00000020: 203d 2031 2e32 2e31 2e31 0d0a 6175 7468   = 1.2.1.1..auth
-00000030: 6f72 203d 204b 6965 7261 6e20 4261 636f  or = Kieran Baco
-00000040: 6e0d 0a61 7574 686f 725f 656d 6169 6c20  n..author_email 
-00000050: 3d20 6b69 6572 616e 2e62 6163 6f6e 406f  = kieran.bacon@o
-00000060: 7574 6c6f 6f6b 2e63 6f6d 0d0a 6465 7363  utlook.com..desc
-00000070: 7269 7074 696f 6e20 3d20 7374 6f77 2061  ription = stow a
-00000080: 7274 6566 6163 7473 2061 6e79 7768 6572  rtefacts anywher
-00000090: 652c 2077 6974 6820 6561 7365 0d0a 6c6f  e, with ease..lo
-000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-000000b0: 2066 696c 653a 2064 6f63 732f 696e 6465   file: docs/inde
-000000c0: 782e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  x.md..long_descr
-000000d0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-000000e0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-000000f0: 6f77 6e0d 0a74 6573 745f 7375 6974 6520  own..test_suite 
-00000100: 3d20 7465 7374 730d 0a6b 6579 776f 7264  = tests..keyword
-00000110: 7320 3d20 6177 7320 7333 2062 6f74 6f33  s = aws s3 boto3
-00000120: 2073 7368 206f 730d 0a63 6c61 7373 6966   ssh os..classif
-00000130: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000140: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000150: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000160: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000170: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-00000180: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-00000190: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-000001a0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001b0: 7065 6e64 656e 740d 0a70 726f 6a65 6374  pendent..project
-000001c0: 5f75 726c 7320 3d20 0d0a 0948 6f6d 6570  _urls = ...Homep
-000001d0: 6167 6520 3d20 6874 7470 733a 2f2f 6769  age = https://gi
-000001e0: 7468 7562 2e63 6f6d 2f4b 6965 7261 6e2d  thub.com/Kieran-
-000001f0: 4261 636f 6e2f 7374 6f77 0d0a 0944 6f63  Bacon/stow...Doc
-00000200: 756d 656e 7461 7469 6f6e 203d 2068 7474  umentation = htt
-00000210: 7073 3a2f 2f73 746f 772e 7265 6164 7468  ps://stow.readth
-00000220: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000230: 7374 2f0d 0a09 4275 6720 5472 6163 6b65  st/...Bug Tracke
-00000240: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000250: 7562 2e63 6f6d 2f4b 6965 7261 6e2d 4261  ub.com/Kieran-Ba
-00000260: 636f 6e2f 7374 6f77 2f69 7373 7565 730d  con/stow/issues.
-00000270: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 696e  ...[options]..in
-00000280: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000290: 200d 0a09 7471 646d 0d0a 7061 636b 6167   ...tqdm..packag
-000002a0: 655f 6469 7220 3d20 0d0a 0973 746f 7720  e_dir = ...stow 
-000002b0: 3d20 7374 6f77 0d0a 0d0a 5b6f 7074 696f  = stow....[optio
-000002c0: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-000002d0: 655d 0d0a 616c 6c20 3d20 0d0a 0962 6f74  e]..all = ...bot
-000002e0: 6f33 0d0a 7333 203d 200d 0a09 626f 746f  o3..s3 = ...boto
-000002f0: 330d 0a74 6573 7420 3d20 0d0a 0970 7969  3..test = ...pyi
-00000300: 6e69 0d0a 0970 7974 6573 740d 0a09 7079  ni...pytest...py
-00000310: 7465 7374 2d63 6f76 0d0a 096d 6f74 6f5b  test-cov...moto[
-00000320: 7333 5d3e 3d34 2e31 2e35 2e64 6576 3430  s3]>=4.1.5.dev40
-00000330: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000340: 7279 5f70 6f69 6e74 735d 0d0a 7374 6f77  ry_points]..stow
-00000350: 5f6d 616e 6167 6572 7320 3d20 0d0a 0966  _managers = ...f
-00000360: 7320 3d20 7374 6f77 2e6d 616e 6167 6572  s = stow.manager
-00000370: 733a 4653 0d0a 096c 6673 203d 2073 746f  s:FS...lfs = sto
-00000380: 772e 6d61 6e61 6765 7273 3a46 530d 0a09  w.managers:FS...
-00000390: 6177 7320 3d20 7374 6f77 2e6d 616e 6167  aws = stow.manag
-000003a0: 6572 733a 416d 617a 6f6e 0d0a 0973 3320  ers:Amazon...s3 
-000003b0: 3d20 7374 6f77 2e6d 616e 6167 6572 733a  = stow.managers:
-000003c0: 416d 617a 6f6e 0d0a 0d0a 5b65 6767 5f69  Amazon....[egg_i
-000003d0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000003e0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000003f0: 0d0a 0d0a                                ....
+00000020: 203d 2031 2e32 2e32 0d0a 6175 7468 6f72   = 1.2.2..author
+00000030: 203d 204b 6965 7261 6e20 4261 636f 6e0d   = Kieran Bacon.
+00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000050: 6b69 6572 616e 2e62 6163 6f6e 406f 7574  kieran.bacon@out
+00000060: 6c6f 6f6b 2e63 6f6d 0d0a 6465 7363 7269  look.com..descri
+00000070: 7074 696f 6e20 3d20 7374 6f77 2061 7274  ption = stow art
+00000080: 6566 6163 7473 2061 6e79 7768 6572 652c  efacts anywhere,
+00000090: 2077 6974 6820 6561 7365 0d0a 6c6f 6e67   with ease..long
+000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000b0: 696c 653a 2064 6f63 732f 696e 6465 782e  ile: docs/index.
+000000c0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000d0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000000e0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+000000f0: 6e0d 0a74 6573 745f 7375 6974 6520 3d20  n..test_suite = 
+00000100: 7465 7374 730d 0a6b 6579 776f 7264 7320  tests..keywords 
+00000110: 3d20 6177 7320 7333 2062 6f74 6f33 2073  = aws s3 boto3 s
+00000120: 7368 206f 730d 0a63 6c61 7373 6966 6965  sh os..classifie
+00000130: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000140: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000150: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
+00000160: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000170: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
+00000180: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
+00000190: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000001a0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000001b0: 6e64 656e 740d 0a70 726f 6a65 6374 5f75  ndent..project_u
+000001c0: 726c 7320 3d20 0d0a 0948 6f6d 6570 6167  rls = ...Homepag
+000001d0: 6520 3d20 6874 7470 733a 2f2f 6769 7468  e = https://gith
+000001e0: 7562 2e63 6f6d 2f4b 6965 7261 6e2d 4261  ub.com/Kieran-Ba
+000001f0: 636f 6e2f 7374 6f77 0d0a 0944 6f63 756d  con/stow...Docum
+00000200: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
+00000210: 3a2f 2f73 746f 772e 7265 6164 7468 6564  ://stow.readthed
+00000220: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000230: 2f0d 0a09 4275 6720 5472 6163 6b65 7220  /...Bug Tracker 
+00000240: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000250: 2e63 6f6d 2f4b 6965 7261 6e2d 4261 636f  .com/Kieran-Baco
+00000260: 6e2f 7374 6f77 2f69 7373 7565 730d 0a0d  n/stow/issues...
+00000270: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 7374  .[options]..inst
+00000280: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000290: 0a09 7471 646d 0d0a 7061 636b 6167 655f  ..tqdm..package_
+000002a0: 6469 7220 3d20 0d0a 0973 746f 7720 3d20  dir = ...stow = 
+000002b0: 7374 6f77 0d0a 0d0a 5b6f 7074 696f 6e73  stow....[options
+000002c0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+000002d0: 0d0a 616c 6c20 3d20 0d0a 0962 6f74 6f33  ..all = ...boto3
+000002e0: 0d0a 7333 203d 200d 0a09 626f 746f 330d  ..s3 = ...boto3.
+000002f0: 0a74 6573 7420 3d20 0d0a 0970 7969 6e69  .test = ...pyini
+00000300: 0d0a 0970 7974 6573 740d 0a09 7079 7465  ...pytest...pyte
+00000310: 7374 2d63 6f76 0d0a 096d 6f74 6f5b 7333  st-cov...moto[s3
+00000320: 5d3e 3d34 2e31 2e35 2e64 6576 3430 0d0a  ]>=4.1.5.dev40..
+00000330: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000340: 5f70 6f69 6e74 735d 0d0a 7374 6f77 5f6d  _points]..stow_m
+00000350: 616e 6167 6572 7320 3d20 0d0a 0966 7320  anagers = ...fs 
+00000360: 3d20 7374 6f77 2e6d 616e 6167 6572 733a  = stow.managers:
+00000370: 4653 0d0a 096c 6673 203d 2073 746f 772e  FS...lfs = stow.
+00000380: 6d61 6e61 6765 7273 3a46 530d 0a09 6177  managers:FS...aw
+00000390: 7320 3d20 7374 6f77 2e6d 616e 6167 6572  s = stow.manager
+000003a0: 732e 616d 617a 6f6e 3a41 6d61 7a6f 6e0d  s.amazon:Amazon.
+000003b0: 0a09 7333 203d 2073 746f 772e 6d61 6e61  ..s3 = stow.mana
+000003c0: 6765 7273 2e61 6d61 7a6f 6e3a 416d 617a  gers.amazon:Amaz
+000003d0: 6f6e 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  on....[egg_info]
+000003e0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000003f0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `stow-1.2.1.1/stow/__init__.py` & `stow-1.2.2/stow/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .utils import (
     find,
     connect,
     parseURL
 )
 
 env = os.environ
+getcwd = os.getcwd
 
 # Create the stateless manager
 Manager = Manager()
 
 manager = Manager.manager
 artefact = Manager.artefact
 abspath = Manager.abspath
```

### Comparing `stow-1.2.1.1/stow/_utils.py` & `stow-1.2.2/stow/_utils.py`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/stow/artefacts.py` & `stow-1.2.2/stow/artefacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,18 +111,21 @@
     def name(self):
         """ Name of artefact - for `File` this is without extension """
         return self.basename
     @name.setter
     def name(self, name: str):
         self.basename = name
 
-    @abc.abstractmethod
-    @contextlib.contextmanager
     def localise(self):
-        pass
+        """ Localise this artefact
+
+        Returns:
+            Localiser: The context manager object
+        """
+        return self.manager.localise(self)
 
     def save(self, path: str, force: bool = False):
         """ Save the artefact to a local location
 
         Args:
             path: A local path where the Artefact is to be saved
             force: Ignore artefacts at the destination location
@@ -282,29 +285,17 @@
         return self._size
 
     def isLink(self):
         if self._isLink is None:
             self._isLink = self._manager._isLink(self)
         return self._isLink
 
-    @contextlib.contextmanager
-    def localise(self) -> str:
-        """ Localise this File artefact
-
-        Returns:
-            str: the absolute local path to the manager path
-        """
-        with self.manager.localise(self) as abspath:
-            yield abspath
-
-    @contextlib.contextmanager
-    def open(self, mode: str = 'r', **kwargs) -> io.IOBase:
+    def open(self, mode: str = 'r', **kwargs) -> typing.IO[typing.AnyStr]:
         """ Context manager to allow the pulling down and opening of a file """
-        with self._manager.open(self, mode, **kwargs) as handle:
-            yield handle
+        return self._manager.open(self, mode, **kwargs)
 
 class Directory(Artefact):
     """ A directory represents an local filesystems directory or folder. Directories hold references to other
     directories or files
 
     Args:
         manager (stow.Manager): The manager this directory object belongs to
@@ -416,45 +407,30 @@
         #     raise exceptions.ArtefactNotMember(
         #         "Cannot create relative path for Artefact {} as its not a member of {}".format(artefact, self)
         #     )
 
         # Return the path
         return self.manager.relpath(path, self.path, separator=separator)
 
-    @contextlib.contextmanager
-    def localise(self, path: str = None) -> str:
-        """ Localise an artefact this directory or a child artefact with the provided path.
-
-        Args:
-            path: Path of localisation
-
-        Returns:
-            str: the absolute local path to the manager path
-        """
-        with self.manager.localise(self if path is None else self.manager.join(self._path, path, separator='/')) as abspath:
-            yield abspath
-
-    @contextlib.contextmanager
-    def open(self, path: str, mode: str = "r", **kwargs) -> io.IOBase:
+    def open(self, path: str, mode: str = "r", **kwargs) -> typing.IO[typing.AnyStr]:
         """ Open a file and create a stream to that file. Expose interface of `open`
 
         Args:
             path: Path to directory object
             mode: The open method
             kwargs: kwargs to be passed to the interface of open
 
         Yields:
             io.IOBase: An IO object depending on the mode for interacting with the file
         """
-        with self.manager.open(
+        return self.manager.open(
             self.manager.join(self._path, path, separator='/', joinAbsolutes=True),
             mode,
             **kwargs
-            ) as handle:
-            yield handle
+        )
 
     def rm(self, path: str = None, recursive: bool = False):
         """ Remove an artefact at the given location
 
         Args:
             artefact: Path that is to be deleted
             recursive: If the target is a directory, whether to delete recursively the directories contents
```

### Comparing `stow-1.2.1.1/stow/callbacks.py` & `stow-1.2.2/stow/callbacks.py`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/stow/exceptions.py` & `stow-1.2.2/stow/exceptions.py`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/stow/manager/abstract_methods.py` & `stow-1.2.2/stow/manager/abstract_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     """
 
     # @abstractmethod
     # def __repr__(self):
     #     pass
 
     @abstractmethod
+    def _cwd(self) -> str:
+        """ Return the default working directory for the manager - used to default the artefact path if no path provided
+
+        Returns:
+            str: The default path of the manager, the current working directory
+        """
+        pass
+
+    @abstractmethod
     def _abspath(self, managerPath: str) -> str:
         """ Return the absolute path for a manager path, including the managers protocol, hostname, and parameters.
 
         Args:
             managerPath: The manager relative path which is to be converted to an absolute path
 
         Returns:
@@ -155,15 +164,15 @@
         Args:
             source: the manager local source artefact
             destination: a manager abspath path for destination
         """
         pass
 
     @abstractmethod
-    def _mv(self, source: Artefact, destination: str):
+    def _mv(self, source: Artefact, destination: str) -> Artefact:
         """ Move an artefact from its location to another location managed by the same manager class. This method should
         attempt exploit manager implementation to have transfer done remotely, and avoid having data downloaded to be
         pushed.
 
         An example of this could be the s3 mv feature - though an artefact and its destination maybe in different
         buckets, it is possible to transfer artefacts inside s3.
```

### Comparing `stow-1.2.1.1/stow/manager/base_managers.py` & `stow-1.2.2/stow/manager/base_managers.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,190 +3,214 @@
 import abc
 import typing
 import tempfile
 import contextlib
 import datetime
 
 from ..artefacts import Artefact
-from .manager import Manager
+from .manager import Manager, Localiser
 
-class LocalManager(Manager, abc.ABC):
-    """ Abstract Base Class for managers that will be working with local artefacts.
-    """
-
-    def _setArtefactTimes(self, path: str, modified_time: float, accessed_time: float) -> None:
-        return os.utime(path, (accessed_time, modified_time))
+class LocalLocaliser(Localiser):
 
-    def _setmtime(
-        self,
-        artefact: Artefact,
-        _datetime: typing.Union[float, datetime.datetime]
-        ) -> datetime.datetime:
-
-        if isinstance(_datetime, float):
-            timestamp = _datetime
-            _datetime = datetime.datetime.fromtimestamp(_datetime)
-        else:
-            timestamp = _datetime.timestamp()
-
-        self._setArtefactTimes(
-            artefact.abspath,
-            timestamp,
-            artefact.accessedTime.timestamp()
-        )
-
-        return _datetime
-
-    def _setatime(
-        self,
-        artefact: Artefact,
-        _datetime: typing.Union[float, datetime.datetime]
-        ):
+    def __init__(self, abspath: str):
 
-        if isinstance(_datetime, float):
-            timestamp = _datetime
-            _datetime = datetime.datetime.fromtimestamp(_datetime)
-        else:
-            timestamp = _datetime.timestamp()
+        self._abspath = abspath
+        os.makedirs(os.path.dirname(abspath), exist_ok=True)
 
-        self._setArtefactTimes(
-            artefact.abspath,
-            artefact.modifiedTime.timestamp(),
-            timestamp
-        )
+    def start(self):
+        return self._abspath
 
-        return _datetime
+    def close(self):
+        pass
 
-    @contextlib.contextmanager
-    def localise(self, artefact: typing.Union[Artefact, str]):
 
-        _, _, path = self._splitManagerArtefactForm(artefact, load=False)
+class RemoteLocaliser(Localiser):
 
-        abspath = self._abspath(path)
-        os.makedirs(os.path.dirname(abspath), exist_ok=True)
+    def __init__(self, manager: Manager, artefact: typing.Optional[Artefact], path: str):
 
-        try:
-            yield abspath
-        except Exception as e:
-            raise
+        self._manager = manager
+        self._artefact = artefact
+        self._path = path
 
-class RemoteManager(Manager, abc.ABC):
-    """ Abstract Base Class for managers that will be working with remote artefacts so efficiency with fetching and
-    pushing files is important for time and bandwidth
-    """
+        self._local_path = None
+        self._checksum = None
 
     @staticmethod
     def _compare(dict1, dict2, key):
         # Extract the two sets of keys
         keys1, keys2 = set(dict1[key].keys()), set(dict2[key].keys())
         return keys1.difference(keys2), keys1.intersection(keys2), keys2.difference(keys1)
 
-    @classmethod
-    def _parseHierarchy(cls, path, _toplevel=None):
+    def _parseHierarchy(self, path, _toplevel=None):
 
         # Store separately the directories and files of the path
         directories = {}
         files = {}
 
         # For each item process their checksums
         for item in os.listdir(path):
 
             # Identify their absolute path and relative manager path from the temporary local files
             abspath = os.path.join(path, item)
 
             if os.path.isdir(abspath):
-                directories[abspath] = cls._parseHierarchy(abspath, _toplevel=path)
+                directories[abspath] = self._parseHierarchy(abspath, _toplevel=path)
 
             else:
-                files[abspath] = cls.md5(abspath)
+                files[abspath] = self._manager.md5(abspath)
 
         return {"directories": directories, "files": files}
 
-    @classmethod
-    def _compareHierarhy(cls, original, new):
+    def _compareHierarhy(self, original, new):
 
         # Data containers for files and directory comparison
         toPush, toDelete = set(), set()
 
         # Compare the directories
-        removed, editted, added = cls._compare(original, new, "directories")
+        removed, editted, added = self._compare(original, new, "directories")
         for directory in editted:
-            put, delete = cls._compareHierarhy(original['directories'][directory], new['directories'][directory])
+            put, delete = self._compareHierarhy(original['directories'][directory], new['directories'][directory])
 
             # Union the result of the comparison on the sub directory level
             added |= put
             removed |= delete
 
         toPush |= added
         toDelete |= removed
 
         # Compare the files
-        removed, editted, added = cls._compare(original, new, "files")
+        removed, editted, added = self._compare(original, new, "files")
         for file in editted:
             if original['files'][file] != new['files'][file]:
                 # The checksum of the files are not the same, therefore, the file has been editted and needs to be pushed
                 added.add(file)
 
         toPush |= added
         toDelete |= removed
 
         return toPush, toDelete
 
-    @contextlib.contextmanager
-    def localise(self, artefact):
-
-        # Load the artefacts from the remote
-        _, obj, path = self._splitManagerArtefactForm(artefact, require=False)
+    def start(self):
 
         # Setup a location locally to be able to work with the files
-        exception = None
-        with tempfile.TemporaryDirectory() as directory:
+        directory = tempfile.mkdtemp()
+
+        # Generate a temporay path for the file to be downloaded into
+        self._local_path = local_path = os.path.join(directory, self._manager.basename(self._path))
+
+        # Get the contents and put it into the temporay directory
+        if self._artefact is not None:
+            self._manager.get(self._path, local_path)
+
+            if os.path.isdir(local_path):
+                # To collected item is a directory - walk the directory and record its state
+                self._checksum = self._parseHierarchy(local_path)
+
+            else:
+                # Generate a checksum for the file
+                self._checksum = self._manager.md5(local_path)
+
+        else:
+            # No checksum for no object
+            self._checksum = None
+
+        return local_path
 
-            # Generate a temporay path for the file to be downloaded into
-            local_path = os.path.join(directory, self.basename(path))
+    def close(self):
 
-            # Get the contents and put it into the temporay directory
-            if obj is not None:
-                self.get(path, local_path)
-
-                if os.path.isdir(local_path):
-                    # To collected item is a directory - walk the directory and record its state
-                    checksum = self._parseHierarchy(local_path)
-
-                else:
-                    # Generate a checksum for the file
-                    checksum = self.md5(local_path)
+        # The user has stopped interacting with the artefact - resolve any differences with manager
+        if os.path.exists(self._local_path):
+            if self._checksum:
+                if os.path.isdir(self._local_path):
+                    # Compare the new hiearchy - update only affected files/directories
+                    put, delete = self._compareHierarhy(self._checksum, self._parseHierarchy(self._local_path))
+
+                    # Define the method for converting the abspath back to the manager relative path
+                    contexualise = lambda x: self._manager.join(self._path, x[len(self._local_path)+1:], separator=self._manager.SEPARATOR)
+
+                    # Put/delete the affected artefacts
+                    for abspath in put: self._manager.put(abspath, contexualise(abspath))
+                    for abspath in delete: self._manager.rm(contexualise(abspath), recursive=True)
+
+                elif self._manager.md5(self._local_path) != self._checksum:
+                    # The file has been changed - upload the file's contents
+                    self._manager.put(self._local_path, self._path)
 
             else:
-                # No checksum for no object
-                checksum = None
+                # New item - put the artefact into the manager
+                self._manager.put(self._local_path, self._path)
 
-            # Return the local path to the object
-            try:
-                yield local_path
-            except Exception as e:
-                exception = e
-
-            # The user has stopped interacting with the artefact - resolve any differences with manager
-            if os.path.exists(local_path):
-                if checksum:
-                    if os.path.isdir(local_path):
-                        # Compare the new hiearchy - update only affected files/directories
-                        put, delete = self._compareHierarhy(checksum, self._parseHierarchy(local_path))
-
-                        # Define the method for converting the abspath back to the manager relative path
-                        contexualise = lambda x: self.join(path, x[len(local_path)+1:], separator='/')
-
-                        # Put/delete the affected artefacts
-                        for abspath in put: self.put(abspath, contexualise(abspath))
-                        for abspath in delete: self.rm(contexualise(abspath), recursive=True)
-
-                    elif self.md5(local_path) != checksum:
-                        # The file has been changed - upload the file's contents
-                        self.put(self._localLoad(local_path), path)
-
-                else:
-                    # New item - put the artefact into the manager
-                    self.put(self._localLoad(local_path), path)
+class LocalManager(Manager, abc.ABC):
+    """ Abstract Base Class for managers that will be working with local artefacts.
+    """
+
+    def _cwd(self) -> str:
+        """ Return the default working directory for the manager - used to default the artefact path if no path provided
+
+        Returns:
+            str: The default path of the manager, the current working directory
+        """
+        return os.getcwd()
+
+    def _setArtefactTimes(self, path: str, modified_time: float, accessed_time: float) -> None:
+        return os.utime(path, (accessed_time, modified_time))
+
+    def _setmtime(
+        self,
+        artefact: Artefact,
+        _datetime: typing.Union[float, datetime.datetime]
+        ) -> datetime.datetime:
+
+        if isinstance(_datetime, float):
+            timestamp = _datetime
+            _datetime = datetime.datetime.fromtimestamp(_datetime)
+        else:
+            timestamp = _datetime.timestamp()
+
+        self._setArtefactTimes(
+            artefact.abspath,
+            timestamp,
+            artefact.accessedTime.timestamp()
+        )
+
+        return _datetime
+
+    def _setatime(
+        self,
+        artefact: Artefact,
+        _datetime: typing.Union[float, datetime.datetime]
+        ):
 
-        if exception is not None:
-            raise exception
+        if isinstance(_datetime, float):
+            timestamp = _datetime
+            _datetime = datetime.datetime.fromtimestamp(_datetime)
+        else:
+            timestamp = _datetime.timestamp()
+
+        self._setArtefactTimes(
+            artefact.abspath,
+            artefact.modifiedTime.timestamp(),
+            timestamp
+        )
+
+        return _datetime
+
+    def localise(self, artefact: typing.Union[Artefact, str]) -> Localiser:
+        _, _, path = self._splitManagerArtefactForm(artefact, load=False)
+        return LocalLocaliser(self._abspath(path))
+
+class RemoteManager(Manager, abc.ABC):
+    """ Abstract Base Class for managers that will be working with remote artefacts so efficiency with fetching and
+    pushing files is important for time and bandwidth
+    """
+
+    def _cwd(self) -> str:
+        """ Return the default working directory for the manager - used to default the artefact path if no path provided
+
+        Returns:
+            str: The default path of the manager, the current working directory
+        """
+        return '/'
+
+    def localise(self, artefact: typing.Union[Artefact, str]) -> Localiser:
+        _, obj, path = self._splitManagerArtefactForm(artefact, require=False)
+        return RemoteLocaliser(self, obj, path)
```

### Comparing `stow-1.2.1.1/stow/manager/manager.py` & `stow-1.2.2/stow/manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import io
 import typing
+from typing import (Union, Optional)
 import urllib
 import shutil
 import tempfile
 import mimetypes
 import contextlib
 import datetime
 import hashlib
@@ -16,26 +17,48 @@
 from ..callbacks import AbstractCallback
 from .. import _utils as utils
 from .. import exceptions
 
 import logging
 log = logging.getLogger(__name__)
 
+class Localiser(contextlib.AbstractContextManager):
+
+    def __init__(self):
+        pass
+
+    def start(self) -> str:
+        """ Returns path to the localised artefact """
+        pass
+
+    def close(self):
+        pass
+
+    def __enter__(self) -> str:
+        return self.start()
+
+    def __exit__(self, exeception_type, exeception_value, exeception_traceback):
+        self.close()
+
+        if exeception_type:
+            return False
+
 class ManagerReloader:
     """ Class to manage the reloading of a reduced Manager """
     def __new__(cls, config):
         # This will create a new manager if it doesn't exist of fetch the one globally created
         return utils.connect(**config)
 
 class Manager(AbstractManager):
     """ Manager Abstract base class - expressed the interface of a Manager which governs a storage
     option and allows extraction and placement of files in that storage container
 
     """
 
+    SEPARATOR = os.sep
     SEPARATORS = ['\\', '/']
     ISOLATED = False
 
     _READONLYMODES = ["r", "rb"]
     _MULTI_SEP_REGEX = re.compile(r"(\\{2,})|(\/{2,})")
     _RELPATH_REGEX = re.compile(r"^([a-zA-Z0-9]+:)?([/\\\w\.!-_*'() ]*)$")
 
@@ -96,15 +119,16 @@
         if isinstance(artefact, Artefact):
             return artefact.manager, artefact, artefact.path
 
         else:
             obj = None
 
             if artefact is None:
-                manager, path = utils.connect("FS"), self._cwd()
+                manager = utils.connect("FS")
+                path = manager._cwd()
 
             elif isinstance(artefact, str):
                 manager, path = utils.parseURL(artefact)
 
             else:
                 t = type(artefact)
                 raise TypeError(
@@ -137,28 +161,30 @@
             require (str): Require that the object exists. when false return None for yet to be created objects but
 
         Returns:
             Artefact or None: the artefact object or None if it doesn't exists and require is False
             str: The relative path of the object/the passed value
         """
 
-        if isinstance(artefact, Artefact):
+
+        if self.__class__ == Manager:
+            return self._splitExternalArtefactForm(artefact, load=load, require=require)
+
+        elif isinstance(artefact, Artefact):
             return artefact.manager, artefact, artefact.path
 
         else:
             obj = None
 
-            if artefact in [None, '/']:
-                return self, Directory(self, '/'), '/'
+            if artefact is None:
+                cwd = self._cwd()
+                return self, Directory(self, cwd), cwd
 
             elif isinstance(artefact, str):
-                manager, path = utils.parseURL(
-                    artefact,
-                    default_manager=self if type(self) != Manager else None
-                )
+                manager, path = utils.parseURL(artefact, default_manager=self)
 
             else:
                 t = type(artefact)
                 raise TypeError(
                     f"Artefact reference must be either `stow.Artefact` or string not type {t}"
                 )
 
@@ -179,22 +205,14 @@
         contentType = (contentType or 'application/octet-stream')
         return contentType
 
     def _set_content_type(self, path: str, content_type: str) -> str:
         """ Set the content type of the file """
         raise NotImplementedError('Manager does not have an method for changing the content-type for the path given')
 
-    def _cwd(self) -> str:
-        """ Return the default working directory for the manager - used to default the artefact path if no path provided
-
-        Returns:
-            str: The default path of the manager, the current working directory
-        """
-        return os.getcwd()
-
     def manager(self, artefact: typing.Union[Artefact, str]) -> 'Manager':
         """ Fetch the manager object for the artefact
 
         Params:
             artefact: The artefact whose manager is to be returned
 
         Returns:
@@ -538,16 +556,16 @@
             artefact: Artefact or path whose existence is to be checked
 
         Returns:
             bool: True if artefact exists else False
         """
         return os.path.lexists(artefact)
 
-    @classmethod
-    def join(cls, *paths: typing.Iterable[str], separator=os.sep, joinAbsolutes: bool = False) -> str:
+    # @classmethod
+    def join(self, *paths: typing.Iterable[str], separator=None, joinAbsolutes: bool = False) -> str:
         """ Join one or more path components intelligently. The return value is the concatenation of path and any
         members of *paths with exactly one directory separator following each non-empty part except the last,
         meaning that the result will only end in a separator if the last part is empty. If a component is an absolute
         path, all previous components are thrown away and joining continues from the absolute path component.
 
         Protocols/drive letters are perserved in the event that an absolute is passed in.
 
@@ -558,14 +576,16 @@
 
         Returns:
             str: A joined path
         """
         if not paths:
             return ""
 
+        separator = separator or self.SEPARATOR
+
         parsedResult = None  # Store the network information while path is joined
         joined = ""  # Constructed path
 
         for segment in paths:
             if isinstance(segment, Artefact):
                 # Convert artefacts to paths
                 segment = segment.path
@@ -575,23 +595,23 @@
             if presult.scheme:
                 parsedResult = presult
                 segment = presult.path
 
             if joined:
                 # A path is in the midst of being created
 
-                if any(segment.startswith(sep) for sep in cls.SEPARATORS):
+                if any(segment.startswith(sep) for sep in self.SEPARATORS):
                     if joinAbsolutes:
                         joined = joined.rstrip('\\/') + segment
 
                     else:
                         joined = segment
 
                 else:
-                    if any(joined.endswith(sep) for sep in cls.SEPARATORS):
+                    if any(joined.endswith(sep) for sep in self.SEPARATORS):
                         joined += segment
 
                     else:
                         joined += separator + segment
 
             else:
                 joined = segment
@@ -820,23 +840,32 @@
     def put(
         self,
         source: typing.Union[Artefact, str, bytes],
         destination: typing.Union[Artefact, str],
         overwrite: bool = False,
         *,
         metadata: typing.Dict[str, str] = None,
-        callback: typing.Type[AbstractCallback] = None
-        ) -> Artefact:
+        callback: typing.Type[AbstractCallback] = None,
+        modified_time: Optional[datetime.datetime] = None,
+        accessed_time: Optional[datetime.datetime] = None
+        ) -> Union[File, Directory]:
         """ Put a local artefact onto the remote at the location given.
 
         Args:
-            src_local (str): The path to the local artefact that is to be put on the remote
-            dest_remote (Artefact/str): A file object to overwrite or the relative path to a destination on the
-                remote
-            overwrite (bool) = False: Whether to accept the overwriting of a target destination when it is a directory
+            source (Artefact, str, bytes): The artefact to be put, either artefact, path to file or file bytes.
+            destination (Artefact, str): The artefact of the location object or the path to destination.
+            overwrite (bool) = False: Protection against overwritting directories
+            *,
+            metadata (Dict[str,str]): A dictionary of metadata to write with the file artefact
+            callback (AbstractCallback): A callback method to monitor file upload progress
+            modified_time (Optional[datetime.datetime]): The modified time of the new artefact (if manager supports)
+            accessed_time (Optional[datetime.datetime]): The accessed time of the new artefact (if manager supports)
+
+        Returns:
+
         """
 
         # Validate source before deleting destination
         if not isinstance(source, bytes):
             _, sourceObj, _ = self._splitExternalArtefactForm(source)
 
         # Load in the information about the destination
@@ -856,23 +885,27 @@
             callback = callback('put')
 
         if isinstance(source, bytes):
             return destinationManager._putBytes(
                 source,
                 destinationPath,
                 metadata=metadata,
-                callback=callback
+                callback=callback,
+                modified_time=modified_time,
+                accessed_time=accessed_time,
             )
 
         else:
             return destinationManager._put(
                 sourceObj,
                 destinationPath,
                 metadata=metadata,
-                callback=callback
+                callback=callback,
+                modified_time=modified_time,
+                accessed_time=accessed_time,
             )
 
     def cp(
         self,
         source: typing.Union[Artefact, str],
         destination: typing.Union[Artefact, str],
         overwrite: bool = False
@@ -991,47 +1024,57 @@
 
         # Fetch the destination object
         destinationManager, destinationObj, destinationPath = self._splitExternalArtefactForm(destination, require=False)
 
         if destinationObj is None:
             # The destination doesn't exist - sync the entire source
 
-            log.debug("Syncing: No destination therefore putting entire source")
-            self.put(sourceObj, destination)
+            log.debug("Syncing: Destination doesn't exist therefore putting entire source")
+            destinationManager.put(
+                sourceObj,
+                destination
+            )
 
         elif isinstance(destinationObj, File):
             if isinstance(sourceObj, Directory):
                 # The source is a directory - we simply replace the file
-                self.put(sourceObj, destinationObj, overwrite=overwrite)
+                destinationManager.put(sourceObj, destinationObj, overwrite=overwrite)
 
             elif (
                 (not check_modified_times or destinationObj.modifiedTime < sourceObj.modifiedTime) and
                 (digest_comparator is None or not digest_comparator(sourceObj, destinationObj))
                 ):
-                self.put(sourceObj, destinationObj)
+                destinationManager.put(sourceObj, destinationObj)
 
             else:
                 log.debug('%s already synced', destination)
 
         else:
             # Desintation object is a dictionary
             if isinstance(sourceObj, File):
                 # We are trying to sync a file to a directory - this is a put
-                return self.put(sourceObj, destinationObj, overwrite=overwrite)
+                return destinationManager.put(sourceObj, destinationObj, overwrite=overwrite)
 
             # Syncing a source directory to a destination directory
             destinationMap = {artefact.basename: artefact for artefact in destinationObj.ls()}
 
             # Recursively fill in destination at this recursion level
             for artefact in sourceObj.ls():
                 if artefact.basename in destinationMap:
-                    self.sync(artefact, destinationMap.pop(artefact.basename))
+                    self.sync(
+                        artefact,
+                        destinationMap.pop(artefact.basename),
+                        overwrite=overwrite,
+                        delete=delete,
+                        check_modified_times=check_modified_times,
+                        digest_comparator=digest_comparator,
+                    )
 
                 else:
-                    self.put(artefact, self.join(destinationObj.path, artefact.basename))
+                    destinationManager.put(artefact, destinationManager.join(destinationObj.path, artefact.basename))
 
             # Any remaining destionation objects were not targets of sync - delete if argument passed
             if delete:
                 for artefact in destinationMap.values():
                     destinationManager.rm(artefact, recursive=overwrite)
 
     def iterls(
@@ -1149,35 +1192,42 @@
         if artefact is not None:
             return self.cp(artefact, artefact)
 
         return self.put(b'', relpath)
 
     _READONLYMODES = ["r", "rb"]
 
-    @contextlib.contextmanager
-    def open(self, artefact: typing.Union[File, str], mode: str = "r", **kwargs) -> io.IOBase:
+    def open(self, artefact: typing.Union[File, str], mode: str = "r", **kwargs) -> typing.IO[typing.AnyStr]:
         """ Open a file and create a stream to that file. Expose interface of `open`
 
         Args:
             artefact: The object that represents the file (or path to the file) to be openned by this manager
             mode: The open method
             kwargs: kwargs to be passed to the interface of open
 
         Yields:
             io.IOBase: An IO object depending on the mode for interacting with the file
         """
 
+        # Parse the artefact
         manager, obj, path = self._splitManagerArtefactForm(artefact, load=mode in self._READONLYMODES)
 
-        with manager.localise(path) as abspath:
-            with open(abspath, mode, **kwargs) as handle:
-                yield handle
+        # Setup a localiser for the artefact
+        localiser = manager.localise(obj or path)
+        abspath = localiser.start()
+
+        # Create a handle to the file - update the close to close the localiser
+        handle = open(abspath, mode, **kwargs)
+        _close = handle.close
+        def closer():
+            _close()
+            localiser.close()
+        handle.close = closer
+
+        return handle
 
-    @contextlib.contextmanager
-    def localise(self, artefact: typing.Union[Artefact, str]) -> str:
+    def localise(self, artefact: typing.Union[Artefact, str]) -> Localiser:
 
         # Get the manager instance to handle the localise method
         manager, obj, path = self._splitManagerArtefactForm(artefact, load=False)
 
-        # Call localise on the manager with the path
-        with manager.localise(path) as handle:
-            yield handle
+        return manager.localise(obj or path)
```

### Comparing `stow-1.2.1.1/stow/managers/amazon.py` & `stow-1.2.2/stow/managers/amazon.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 from ..artefacts import Artefact, PartialArtefact, File, Directory, HashingAlgorithm
 from ..manager import RemoteManager
 from ..callbacks import AbstractCallback
 from .. import exceptions
 
 log = logging.getLogger(__name__)
 
-def getS3ETag(bytes_readable):
-    """
+def calculateBytesS3ETag(bytes_readable: typing.BinaryIO) -> str:
+    """ For a given set of bytes, calculate their AWS's etag value.
 
     The ETag of multipart uploads is not MD5 - each part has a md5 calculated and then
     they are concaticated before they are MD5'd for the final etag. It is then followed
     by a -xxxx that stored the number of parts that made up the upload.
 
     Args:
-        bytes_readable (_type_): _description_
+        bytes_readable (typing.BinaryIO): A readable object containing the file bytes
 
     Returns:
-        _type_: _description_
+        str: the string literal ETag value as found in aws api responses.
     """
 
     md5s = []
     while True:
         data = bytes_readable.read(8 * 1024 * 1024)
         if not data:
             break
@@ -70,15 +70,15 @@
     digests = []
     for f in files:
         if isinstance(f._manager, Amazon):
             digests.append(f.metadata['ETag'])
 
         else:
             with f.open('rb') as handle:
-                digests.append(getS3ETag(handle))
+                digests.append(calculateBytesS3ETag(handle))
 
     return digests[0] == digests[1]
 
 class Amazon(RemoteManager):
     """ Connect to an amazon s3 bucket using an IAM user credentials or environment variables
 
     Params:
@@ -87,14 +87,16 @@
         aws_secret_access_key (None): The secret key for a IAM user that has permissions to the bucket
         region_name (None): The region of the user/bucket
         storage_class (STANDARD): The storage class type name e.g. STANDARD, REDUCED_REDUDANCY
         TODO
 
     """
 
+    SEPARATOR = '/'
+
     # Define regex for the object key
     _LINE_SEP = "/"
     _S3_OBJECT_KEY = re.compile(r"^[a-zA-Z0-9!_.*'()\- ]+(/[a-zA-Z0-9!_.*'()\- ]+)*$")
     _S3_DISALLOWED_CHARACTERS = "{}^%`]'`\"<>[~#|"
     _S3_MAX_KEYS = os.environ.get('STOW_AMAZON_MAX_KEYS', 100)
 
     class StorageClass(enum.Enum):
@@ -390,15 +392,15 @@
                     "StorageClass": self._storageClass.value,
                     "ContentType": (mimetypes.guess_type(destination)[0] or 'application/octet-stream'),
                     **extra_args
                 },
                 Callback=self._s3Callback(callback, source)
             )
 
-    def _put(self, source: Artefact, destination: str, *, metadata = None, callback = None):
+    def _put(self, source: Artefact, destination: str, *, metadata = None, callback = None, **kwargs):
 
         # Setup metadata about the objects being put
         extra_args = {}
         if metadata is not None:
             extra_args['Metadata'] = {str(k): str(v) for k, v in metadata.items()}
 
         if isinstance(source, Directory):
@@ -471,15 +473,16 @@
 
     def _putBytes(
         self,
         fileBytes: bytes,
         destination: str,
         *,
         metadata: typing.Dict[str, str] = None,
-        callback = None
+        callback = None,
+        **kwargs
         ):
 
 
         self._s3.upload_fileobj(
             io.BytesIO(fileBytes),
             self._bucketName,
             self._managerPath(destination),
@@ -559,15 +562,15 @@
 
     def _mv(self, source: Artefact, destination: str):
 
         # Copy the source objects to the destination
         copied_artefact = self._cp(source, destination)
 
         # Delete the source objects now it has been entirely copied
-        self._rm(source)
+        source.manager._rm(source)
 
         return copied_artefact
 
     def _ls(self, directory: str, recursive: bool = False):
 
         for metadata, is_file in self._list_objects(
             self._bucketName,
```

### Comparing `stow-1.2.1.1/stow/managers/filesystem.py` & `stow-1.2.2/stow/managers/filesystem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import datetime
 import shutil
 import urllib
-import typing
+from typing import Optional
 
 import binascii
 import hashlib
 
 if os.name == 'nt':
     import ctypes
 
@@ -135,32 +135,72 @@
         method(sourceAbspath, destination)
 
     def _getBytes(self, source: Artefact, *, callback = None) -> bytes:
 
         with open(self._abspath(source.path), "rb") as handle:
             return handle.read()
 
-    def _put(self, source: str, destination: str, *, metadata = None, callback = None):
+    def _put(
+        self,
+        source: str,
+        destination: str,
+        *,
+        metadata = None,
+        callback = None,
+        modified_time: Optional[datetime.datetime] = None,
+        accessed_time: Optional[datetime.datetime] = None,
+        **kwargs
+        ):
 
         # Convert destination path
         destinationAbspath = self._abspath(destination)
 
         # Ensure the destination
         os.makedirs(os.path.dirname(destinationAbspath), exist_ok=True)
 
+        fileUpdators = []
+        if modified_time is not None or accessed_time is not None:
+            def updateFileTimes(artefact: Artefact):
+                self._setArtefactTimes(
+                    modified_time=(modified_time or artefact.modifiedTime.timestamp()),
+                    accessed_time=(accessed_time or artefact.accessedTime.timestamp())
+                )
+            fileUpdators.append(updateFileTimes)
+
         # Select the put method
         with source.localise() as sourceAbspath:
-            method = shutil.copytree if os.path.isdir(sourceAbspath) else shutil.copy
 
-            # Perform the putting
-            method(sourceAbspath, destinationAbspath)
+            if os.path.isdir(sourceAbspath):
+                shutil.copytree(sourceAbspath, destinationAbspath)
+
+                if fileUpdators:
+                    for artefact in self._ls(destinationAbspath):
+                        for updator in fileUpdators:
+                            updator(artefact)
+
+            else:
+                shutil.copy(sourceAbspath, destinationAbspath)
+
+                if fileUpdators:
+                    for updator in fileUpdators:
+                        updator(destinationAbspath)
 
         return PartialArtefact(self, destination)
 
-    def _putBytes(self, fileBytes: bytes, destination: str, *, metadata = None, callback = None):
+    def _putBytes(
+        self,
+        fileBytes: bytes,
+        destination: str,
+        *,
+        metadata = None,
+        callback = None,
+        modified_time: Optional[datetime.datetime] = None,
+        accessed_time: Optional[datetime.datetime] = None,
+        **kwargs
+        ):
 
         # Convert destination path
         destinationAbspath = self._abspath(destination)
 
         # Makesure the destination exists
         os.makedirs(os.path.dirname(destinationAbspath), exist_ok=True)
 
@@ -190,15 +230,15 @@
 
         # Get a path to the folder
         abspath = self._abspath(directory)
 
         # Iterate over the folder and identify every object - add the created
         for art in os.listdir(abspath):
             artefact = self._identifyPath(
-                self.join(directory, art, separator='/')
+                self.join(directory, art)
             )
 
             if artefact is not None:
                 yield artefact
 
     def _rm(self, artefact: Artefact):
 
@@ -240,14 +280,14 @@
 class SubdirectoryFS(FS):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._rootLength = len(self._root)
 
     def _cwd(self):
-        return self._root
+        return self.SEPARATOR
 
     def _abspath(self, managerPath: str) -> str:
         return os.path.abspath(self.join(self._root, managerPath, joinAbsolutes=True))
 
     def _relative(self, abspath: str) -> str:
         return abspath[self._rootLength:] or os.sep
```

### Comparing `stow-1.2.1.1/stow/testing/mock.py` & `stow-1.2.2/stow/testing/mock.py`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/stow/utils.py` & `stow-1.2.2/stow/utils.py`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/stow.egg-info/PKG-INFO` & `stow-1.2.2/stow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stow
-Version: 1.2.1.1
+Version: 1.2.2
 Summary: stow artefacts anywhere, with ease
 Author: Kieran Bacon
 Author-email: kieran.bacon@outlook.com
 Project-URL: Homepage, https://github.com/Kieran-Bacon/stow
 Project-URL: Documentation, https://stow.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Kieran-Bacon/stow/issues
 Keywords: aws s3 boto3 ssh os
```

### Comparing `stow-1.2.1.1/stow.egg-info/SOURCES.txt` & `stow-1.2.2/stow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 pyproject.toml
 setup.cfg
 docs/index.md
 stow/__init__.py
 stow/_utils.py
 stow/artefacts.py
 stow/callbacks.py
```

### Comparing `stow-1.2.1.1/tests/test_callbacks.py` & `stow-1.2.2/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stow-1.2.1.1/tests/test_stateless.py` & `stow-1.2.2/tests/test_stateless.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,42 @@
 import os
 import tempfile
 import uuid
 import datetime
 import time
 
 import stow
-import stow.managers
+from stow.managers.filesystem import FS
+from stow.managers.amazon import Amazon
 
 class Test_Stateless(unittest.TestCase):
 
+    def test_open_object(self):
+        """ Use stow open like a normal file handle """
+
+        with tempfile.TemporaryDirectory() as directory:
+            file_path = stow.join(directory, 'new_file.txt')
+            fileDescriptor = stow.open(file_path, 'w')
+            fileDescriptor.write("Hello there")
+            fileDescriptor.close()
+
+            fileDescriptor2 = open(file_path)
+            self.assertEqual(os.path.splitdrive(fileDescriptor.name)[1], os.path.splitdrive(fileDescriptor2.name)[1])
+
+            self.assertEqual(fileDescriptor2.read(), 'Hello there')
+
+            fileDescriptor2.close()
+
     def test_find(self):
 
         filesystemManager = stow.find("FS")
-        self.assertTrue(filesystemManager, stow.managers.FS)
+        self.assertTrue(filesystemManager, FS)
 
         amazonS3 = stow.find("s3")
-        self.assertTrue(amazonS3, stow.managers.Amazon)
+        self.assertTrue(amazonS3, Amazon)
 
         with self.assertRaises(ValueError):
             stow.find("missing")
 
     def test_connect(self):
 
         with tempfile.TemporaryDirectory() as directory:
@@ -123,15 +140,15 @@
         self.assertEqual(stow.dirname("s3://bucket/there"), "s3://bucket/")
         self.assertEqual(stow.dirname("s3://bucket/hello/there"), "s3://bucket/hello")
         self.assertEqual(stow.dirname("s3://hello/there?param1=value1"), "s3://hello/?param1=value1")
 
     def test_dirname_with_artefact(self):
 
         test_file = stow.artefact(__file__)
-        self.assertEqual(stow.dirname(test_file), os.path.dirname(__file__))
+        self.assertEqual(os.path.splitdrive(stow.dirname(test_file))[1], os.path.splitdrive(os.path.dirname(__file__))[1])
 
     def test_expandusers(self):
 
         self.assertEqual(stow.expanduser("~/Documents"), os.path.expanduser("~/Documents"))
         self.assertEqual(stow.expanduser("~/${MODELS}/Documents"), os.path.expanduser("~/${MODELS}/Documents"))
 
     def test_expandvars(self):
@@ -500,14 +517,20 @@
 
 
     def test_ls(self):
         arts = {os.path.basename(art.path) for art in stow.ls(".")}
         files = {filename for filename in os.listdir()}
         self.assertEqual(arts, files)
 
+    def test_ls_none(self):
+        arts = {os.path.basename(art.path) for art in stow.ls()}
+        files = {filename for filename in os.listdir()}
+        self.assertEqual(arts, files)
+
+
     def test_join(self):
 
         for s in [
             ("hello//there", "buddy/"),
             ("hello", "/", "there"),
             ("hello"),
             ("", "hello"),
@@ -746,14 +769,29 @@
             )
 
             self.assertEqual(stow.artefact(stow.join(directory, "dir2", "file1.txt")).content, b"content")
             self.assertEqual(stow.artefact(stow.join(directory, "dir2", "file2.txt")).content, b"file2")
             self.assertEqual(stow.artefact(stow.join(directory, "dir2", "file3.txt")).content, b"Original")
             self.assertEqual(stow.artefact(stow.join(directory, "dir2", "file4.txt")).content, b"copied")
 
+    def test_sync_to_non_existent_location(self):
+
+        with tempfile.TemporaryDirectory() as directory:
+
+            stow.touch(stow.join(directory, 'dir1', 'hello.txt'))
+
+            stow.sync(
+                stow.join(directory, 'dir1'),
+                stow.join(directory, 'dir2')
+            )
+
+            self.assertTrue(stow.exists(stow.join(directory, 'dir2', 'hello.txt')))
+
+
+
     def test_rm(self):
 
         with tempfile.TemporaryDirectory() as directory:
 
             filepath1 = stow.join(directory, "file1.txt")
             filepath2 = stow.join(directory, "file2.txt")
```

### Comparing `stow-1.2.1.1/tests/test_utils.py` & `stow-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

