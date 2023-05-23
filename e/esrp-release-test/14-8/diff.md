# Comparing `tmp/esrp-release-test-14.tar.gz` & `tmp/esrp-release-test-8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vsts/work/1/s/dist/.tmp-s9fl_z4q/esrp-release-test-14.tar", last modified: Mon May 22 05:42:36 2023, max compression
+gzip compressed data, was "esrp-release-test-8.tar", last modified: Fri Feb  3 10:10:46 2023, max compression
```

## Comparing `esrp-release-test-14.tar` & `esrp-release-test-8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 05:42:36.000000 esrp-release-test-14/
--rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-05-22 05:42:07.000000 esrp-release-test-14/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      957 2023-05-22 05:42:36.000000 esrp-release-test-14/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-22 05:42:07.000000 esrp-release-test-14/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp-release-test/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 05:42:07.000000 esrp-release-test-14/esrp-release-test/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp-release-test/src/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-22 05:42:07.000000 esrp-release-test-14/esrp-release-test/src/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-05-22 05:42:07.000000 esrp-release-test-14/esrp-release-test/src/esrpreltest.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      957 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       63 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       71 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       18 2023-05-22 05:42:36.000000 esrp-release-test-14/esrp_release_test.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       84 2023-05-22 05:42:07.000000 esrp-release-test-14/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     1125 2023-05-22 05:42:36.000000 esrp-release-test-14/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-05-22 05:42:07.000000 esrp-release-test-14/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-03 10:10:46.017476 esrp-release-test-8/
+-rw-rw-rw-   0        0        0    11526 2023-02-03 10:05:20.000000 esrp-release-test-8/LICENSE
+-rw-rw-rw-   0        0        0      988 2023-02-03 10:10:46.017476 esrp-release-test-8/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-02-03 10:07:52.000000 esrp-release-test-8/README.md
+drwxrwxrwx   0        0        0        0 2023-02-03 10:10:46.002495 esrp-release-test-8/esrp-release-test/
+-rw-rw-rw-   0        0        0        0 2023-02-03 10:05:20.000000 esrp-release-test-8/esrp-release-test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-03 10:10:46.005510 esrp-release-test-8/esrp-release-test/src/
+-rw-rw-rw-   0        0        0        0 2023-02-03 10:05:20.000000 esrp-release-test-8/esrp-release-test/src/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-02-03 10:05:20.000000 esrp-release-test-8/esrp-release-test/src/esrpreltest.py
+drwxrwxrwx   0        0        0        0 2023-02-03 10:10:46.015479 esrp-release-test-8/esrp_release_test.egg-info/
+-rw-rw-rw-   0        0        0      988 2023-02-03 10:10:45.000000 esrp-release-test-8/esrp_release_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-02-03 10:10:45.000000 esrp-release-test-8/esrp_release_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-03 10:10:45.000000 esrp-release-test-8/esrp_release_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-02-03 10:10:45.000000 esrp-release-test-8/esrp_release_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-02-03 10:10:45.000000 esrp-release-test-8/esrp_release_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-02-03 10:10:45.000000 esrp-release-test-8/esrp_release_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-02-03 10:05:20.000000 esrp-release-test-8/pyproject.toml
+-rw-rw-rw-   0        0        0     1171 2023-02-03 10:10:46.019474 esrp-release-test-8/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-02-03 10:05:20.000000 esrp-release-test-8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `esrp-release-test-14/PKG-INFO` & `esrp-release-test-8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: esrp-release-test
-Version: 14
-Summary: ESRP Release is a pathway to many abilities some consider to be, unnatural.
-Home-page: https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
-Author: Vishal Jaishankar
-Author-email: vijaisha@microsoft.com
-Maintainer: Sheshagiri Rao Mallipedhi
-Maintainer-email: shmallip@microsoft.com
-License: This is a new licemse for 5.0
-Project-URL: Bug Tracker, https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
-Platform: windows
-Platform: linux
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: pdf
-License-File: LICENSE
-
-## Project Description
-
-This is a test package used to test the publishing features of esrp release system.
-
-## Requirements
-
-* Python (3.6 or higher)
-* azure-storage-blob
-
-## Installation
-Install using pip
-
-`pip install esrp-release-test`
+Metadata-Version: 2.1
+Name: esrp-release-test
+Version: 8
+Summary: ESRP Release is a pathway to many abilities some consider to be, unnatural.
+Home-page: https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
+Author: Vishal Jaishankar
+Author-email: vijaisha@microsoft.com
+Maintainer: Sheshagiri Rao Mallipedhi
+Maintainer-email: shmallip@microsoft.com
+License: This is a new licemse for 5.0
+Project-URL: Bug Tracker, https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
+Platform: windows
+Platform: linux
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: pdf
+License-File: LICENSE
+
+## Project Description
+
+This is a test package used to test the publishing features of esrp release system.
+
+## Requirements
+
+* Python (3.6 or higher)
+* azure-storage-blob
+
+## Installation
+Install using pip
+
+`pip install esrp-release-test`
```

### Comparing `esrp-release-test-14/esrp_release_test.egg-info/PKG-INFO` & `esrp-release-test-8/esrp_release_test.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: esrp-release-test
-Version: 14
-Summary: ESRP Release is a pathway to many abilities some consider to be, unnatural.
-Home-page: https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
-Author: Vishal Jaishankar
-Author-email: vijaisha@microsoft.com
-Maintainer: Sheshagiri Rao Mallipedhi
-Maintainer-email: shmallip@microsoft.com
-License: This is a new licemse for 5.0
-Project-URL: Bug Tracker, https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
-Platform: windows
-Platform: linux
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: pdf
-License-File: LICENSE
-
-## Project Description
-
-This is a test package used to test the publishing features of esrp release system.
-
-## Requirements
-
-* Python (3.6 or higher)
-* azure-storage-blob
-
-## Installation
-Install using pip
-
-`pip install esrp-release-test`
+Metadata-Version: 2.1
+Name: esrp-release-test
+Version: 8
+Summary: ESRP Release is a pathway to many abilities some consider to be, unnatural.
+Home-page: https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
+Author: Vishal Jaishankar
+Author-email: vijaisha@microsoft.com
+Maintainer: Sheshagiri Rao Mallipedhi
+Maintainer-email: shmallip@microsoft.com
+License: This is a new licemse for 5.0
+Project-URL: Bug Tracker, https://dev.azure.com/arugupta/MS.Ess.Release.VSTS.Extension/_git/esrp-release-test
+Platform: windows
+Platform: linux
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: pdf
+License-File: LICENSE
+
+## Project Description
+
+This is a test package used to test the publishing features of esrp release system.
+
+## Requirements
+
+* Python (3.6 or higher)
+* azure-storage-blob
+
+## Installation
+Install using pip
+
+`pip install esrp-release-test`
```

### Comparing `esrp-release-test-14/setup.cfg` & `esrp-release-test-8/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,74 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6573 7270 2d72 656c 6561 7365 2d74  = esrp-release-t
-00000020: 6573 740a 7665 7273 696f 6e20 3d20 3134  est.version = 14
-00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
-00000040: 5352 5020 5265 6c65 6173 6520 6973 2061  SRP Release is a
-00000050: 2070 6174 6877 6179 2074 6f20 6d61 6e79   pathway to many
-00000060: 2061 6269 6c69 7469 6573 2073 6f6d 6520   abilities some 
-00000070: 636f 6e73 6964 6572 2074 6f20 6265 2c20  consider to be, 
-00000080: 756e 6e61 7475 7261 6c2e 0a6c 6f6e 675f  unnatural..long_
-00000090: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000a0: 6c65 3a20 5245 4144 4d45 2e6d 640a 6c6f  le: README.md.lo
-000000b0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000c0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000d0: 7874 2f6d 6172 6b64 6f77 6e0a 706c 6174  xt/markdown.plat
-000000e0: 666f 726d 7320 3d20 7769 6e64 6f77 732c  forms = windows,
-000000f0: 206c 696e 7578 0a61 7574 686f 7220 3d20   linux.author = 
-00000100: 5669 7368 616c 204a 6169 7368 616e 6b61  Vishal Jaishanka
-00000110: 720a 6175 7468 6f72 5f65 6d61 696c 203d  r.author_email =
-00000120: 2076 696a 6169 7368 6140 6d69 6372 6f73   vijaisha@micros
-00000130: 6f66 742e 636f 6d0a 6d61 696e 7461 696e  oft.com.maintain
-00000140: 6572 203d 2053 6865 7368 6167 6972 6920  er = Sheshagiri 
-00000150: 5261 6f20 4d61 6c6c 6970 6564 6869 0a6d  Rao Mallipedhi.m
-00000160: 6169 6e74 6169 6e65 725f 656d 6169 6c20  aintainer_email 
-00000170: 3d20 7368 6d61 6c6c 6970 406d 6963 726f  = shmallip@micro
-00000180: 736f 6674 2e63 6f6d 0a6c 6963 656e 7365  soft.com.license
-00000190: 203d 2054 6869 7320 6973 2061 206e 6577   = This is a new
-000001a0: 206c 6963 656d 7365 2066 6f72 2035 2e30   licemse for 5.0
-000001b0: 0a63 6c61 7373 6966 6965 7273 203d 200a  .classifiers = .
-000001c0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001e0: 3a3a 2033 0a75 726c 203d 2068 7474 7073  :: 3.url = https
-000001f0: 3a2f 2f64 6576 2e61 7a75 7265 2e63 6f6d  ://dev.azure.com
-00000200: 2f61 7275 6775 7074 612f 4d53 2e45 7373  /arugupta/MS.Ess
-00000210: 2e52 656c 6561 7365 2e56 5354 532e 4578  .Release.VSTS.Ex
-00000220: 7465 6e73 696f 6e2f 5f67 6974 2f65 7372  tension/_git/esr
-00000230: 702d 7265 6c65 6173 652d 7465 7374 0a70  p-release-test.p
-00000240: 726f 6a65 6374 5f75 726c 7320 3d20 0a09  roject_urls = ..
-00000250: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
-00000260: 7470 733a 2f2f 6465 762e 617a 7572 652e  tps://dev.azure.
-00000270: 636f 6d2f 6172 7567 7570 7461 2f4d 532e  com/arugupta/MS.
-00000280: 4573 732e 5265 6c65 6173 652e 5653 5453  Ess.Release.VSTS
-00000290: 2e45 7874 656e 7369 6f6e 2f5f 6769 742f  .Extension/_git/
-000002a0: 6573 7270 2d72 656c 6561 7365 2d74 6573  esrp-release-tes
-000002b0: 740a 0a5b 6f70 7469 6f6e 735d 0a70 7974  t..[options].pyt
-000002c0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002d0: 3d33 2e36 0a69 6e73 7461 6c6c 5f72 6571  =3.6.install_req
-000002e0: 7569 7265 7320 3d20 0a09 617a 7572 652d  uires = ..azure-
-000002f0: 7374 6f72 6167 652d 626c 6f62 3d3d 3132  storage-blob==12
-00000300: 2e31 322e 300a 0972 6571 7565 7374 733e  .12.0..requests>
-00000310: 3d32 2e32 332e 300a 7061 636b 6167 6573  =2.23.0.packages
-00000320: 203d 2066 696e 643a 0a0a 5b6f 7074 696f   = find:..[optio
-00000330: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000340: 0a2a 203d 202a 2e74 7874 2c20 2a2e 7273  .* = *.txt, *.rs
-00000350: 740a 6865 6c6c 6f20 3d20 2a2e 6d73 670a  t.hello = *.msg.
-00000360: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000370: 706f 696e 7473 5d0a 636f 6e73 6f6c 655f  points].console_
-00000380: 7363 7269 7074 7320 3d20 0a09 6578 6563  scripts = ..exec
-00000390: 7574 6162 6c65 2d6e 616d 6520 3d20 6d79  utable-name = my
-000003a0: 5f70 6163 6b61 6765 2e6d 6f64 756c 653a  _package.module:
-000003b0: 6675 6e63 7469 6f6e 0a0a 5b6f 7074 696f  function..[optio
-000003c0: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-000003d0: 655d 0a70 6466 203d 2052 6570 6f72 744c  e].pdf = ReportL
-000003e0: 6162 3e3d 312e 323b 2052 5850 0a0a 5b6f  ab>=1.2; RXP..[o
-000003f0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000400: 6669 6e64 5d0a 6578 636c 7564 6520 3d20  find].exclude = 
-00000410: 0a09 6578 616d 706c 6573 2a0a 0974 6f6f  ..examples*..too
-00000420: 6c73 2a0a 0964 6f63 732a 0a09 6d79 5f70  ls*..docs*..my_p
-00000430: 6163 6b61 6765 2e74 6573 7473 2a0a 0a5b  ackage.tests*..[
-00000440: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
-00000450: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
-00000460: 3d20 300a 0a                             = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2065 7372 702d 7265 6c65 6173 652d   = esrp-release-
+00000020: 7465 7374 0d0a 7665 7273 696f 6e20 3d20  test..version = 
+00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
+00000040: 2045 5352 5020 5265 6c65 6173 6520 6973   ESRP Release is
+00000050: 2061 2070 6174 6877 6179 2074 6f20 6d61   a pathway to ma
+00000060: 6e79 2061 6269 6c69 7469 6573 2073 6f6d  ny abilities som
+00000070: 6520 636f 6e73 6964 6572 2074 6f20 6265  e consider to be
+00000080: 2c20 756e 6e61 7475 7261 6c2e 0d0a 6c6f  , unnatural...lo
+00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000a0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000c0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000d0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000e0: 0a70 6c61 7466 6f72 6d73 203d 2077 696e  .platforms = win
+000000f0: 646f 7773 2c20 6c69 6e75 780d 0a61 7574  dows, linux..aut
+00000100: 686f 7220 3d20 5669 7368 616c 204a 6169  hor = Vishal Jai
+00000110: 7368 616e 6b61 720d 0a61 7574 686f 725f  shankar..author_
+00000120: 656d 6169 6c20 3d20 7669 6a61 6973 6861  email = vijaisha
+00000130: 406d 6963 726f 736f 6674 2e63 6f6d 0d0a  @microsoft.com..
+00000140: 6d61 696e 7461 696e 6572 203d 2053 6865  maintainer = She
+00000150: 7368 6167 6972 6920 5261 6f20 4d61 6c6c  shagiri Rao Mall
+00000160: 6970 6564 6869 0d0a 6d61 696e 7461 696e  ipedhi..maintain
+00000170: 6572 5f65 6d61 696c 203d 2073 686d 616c  er_email = shmal
+00000180: 6c69 7040 6d69 6372 6f73 6f66 742e 636f  lip@microsoft.co
+00000190: 6d0d 0a6c 6963 656e 7365 203d 2054 6869  m..license = Thi
+000001a0: 7320 6973 2061 206e 6577 206c 6963 656d  s is a new licem
+000001b0: 7365 2066 6f72 2035 2e30 0d0a 636c 6173  se for 5.0..clas
+000001c0: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
+000001d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
+00000200: 6465 762e 617a 7572 652e 636f 6d2f 6172  dev.azure.com/ar
+00000210: 7567 7570 7461 2f4d 532e 4573 732e 5265  ugupta/MS.Ess.Re
+00000220: 6c65 6173 652e 5653 5453 2e45 7874 656e  lease.VSTS.Exten
+00000230: 7369 6f6e 2f5f 6769 742f 6573 7270 2d72  sion/_git/esrp-r
+00000240: 656c 6561 7365 2d74 6573 740d 0a70 726f  elease-test..pro
+00000250: 6a65 6374 5f75 726c 7320 3d20 0d0a 0942  ject_urls = ...B
+00000260: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
+00000270: 7073 3a2f 2f64 6576 2e61 7a75 7265 2e63  ps://dev.azure.c
+00000280: 6f6d 2f61 7275 6775 7074 612f 4d53 2e45  om/arugupta/MS.E
+00000290: 7373 2e52 656c 6561 7365 2e56 5354 532e  ss.Release.VSTS.
+000002a0: 4578 7465 6e73 696f 6e2f 5f67 6974 2f65  Extension/_git/e
+000002b0: 7372 702d 7265 6c65 6173 652d 7465 7374  srp-release-test
+000002c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+000002d0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000002e0: 203e 3d33 2e36 0d0a 696e 7374 616c 6c5f   >=3.6..install_
+000002f0: 7265 7175 6972 6573 203d 200d 0a09 617a  requires = ...az
+00000300: 7572 652d 7374 6f72 6167 652d 626c 6f62  ure-storage-blob
+00000310: 3d3d 3132 2e31 322e 300d 0a09 7265 7175  ==12.12.0...requ
+00000320: 6573 7473 3e3d 322e 3233 2e30 0d0a 7061  ests>=2.23.0..pa
+00000330: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000340: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000350: 6765 5f64 6174 615d 0d0a 2a20 3d20 2a2e  ge_data]..* = *.
+00000360: 7478 742c 202a 2e72 7374 0d0a 6865 6c6c  txt, *.rst..hell
+00000370: 6f20 3d20 2a2e 6d73 670d 0a0d 0a5b 6f70  o = *.msg....[op
+00000380: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+00000390: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000003a0: 6970 7473 203d 200d 0a09 6578 6563 7574  ipts = ...execut
+000003b0: 6162 6c65 2d6e 616d 6520 3d20 6d79 5f70  able-name = my_p
+000003c0: 6163 6b61 6765 2e6d 6f64 756c 653a 6675  ackage.module:fu
+000003d0: 6e63 7469 6f6e 0d0a 0d0a 5b6f 7074 696f  nction....[optio
+000003e0: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
+000003f0: 655d 0d0a 7064 6620 3d20 5265 706f 7274  e]..pdf = Report
+00000400: 4c61 623e 3d31 2e32 3b20 5258 500d 0a0d  Lab>=1.2; RXP...
+00000410: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000420: 6573 2e66 696e 645d 0d0a 6578 636c 7564  es.find]..exclud
+00000430: 6520 3d20 0d0a 0965 7861 6d70 6c65 732a  e = ...examples*
+00000440: 0d0a 0974 6f6f 6c73 2a0d 0a09 646f 6373  ...tools*...docs
+00000450: 2a0d 0a09 6d79 5f70 6163 6b61 6765 2e74  *...my_package.t
+00000460: 6573 7473 2a0d 0a0d 0a5b 6567 675f 696e  ests*....[egg_in
+00000470: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000480: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000490: 0a0d 0a                                  ...
```

