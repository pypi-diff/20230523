# Comparing `tmp/PrusaLinkPy-1.0.0.tar.gz` & `tmp/PrusaLinkPy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrusaLinkPy-1.0.0.tar", last modified: Tue May 23 19:50:53 2023, max compression
+gzip compressed data, was "PrusaLinkPy-1.0.1.tar", last modified: Tue May 23 19:55:14 2023, max compression
```

## Comparing `PrusaLinkPy-1.0.0.tar` & `PrusaLinkPy-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 19:50:53.883609 PrusaLinkPy-1.0.0/
--rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 PrusaLinkPy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    10399 2023-05-23 19:50:53.883609 PrusaLinkPy-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 19:50:53.858980 PrusaLinkPy-1.0.0/PrusaLinkPy/
--rw-rw-rw-   0        0        0     4469 2023-05-23 19:34:19.000000 PrusaLinkPy-1.0.0/PrusaLinkPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:50:53.883609 PrusaLinkPy-1.0.0/PrusaLinkPy.egg-info/
--rw-rw-rw-   0        0        0    10399 2023-05-23 19:50:53.000000 PrusaLinkPy-1.0.0/PrusaLinkPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-23 19:50:53.000000 PrusaLinkPy-1.0.0/PrusaLinkPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 19:50:53.000000 PrusaLinkPy-1.0.0/PrusaLinkPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 19:50:53.000000 PrusaLinkPy-1.0.0/PrusaLinkPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8479 2023-05-23 19:50:15.000000 PrusaLinkPy-1.0.0/README.md
--rw-rw-rw-   0        0        0      685 2023-05-23 19:33:42.000000 PrusaLinkPy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 19:50:53.883609 PrusaLinkPy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      206 2023-05-23 19:32:56.000000 PrusaLinkPy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:50:53.883609 PrusaLinkPy-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 PrusaLinkPy-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 PrusaLinkPy-1.0.0/tests/test_PrusaLinkPy.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:55:14.750947 PrusaLinkPy-1.0.1/
+-rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 PrusaLinkPy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10323 2023-05-23 19:55:14.750947 PrusaLinkPy-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 19:55:14.718587 PrusaLinkPy-1.0.1/PrusaLinkPy/
+-rw-rw-rw-   0        0        0     4469 2023-05-23 19:34:19.000000 PrusaLinkPy-1.0.1/PrusaLinkPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:55:14.734384 PrusaLinkPy-1.0.1/PrusaLinkPy.egg-info/
+-rw-rw-rw-   0        0        0    10323 2023-05-23 19:55:14.000000 PrusaLinkPy-1.0.1/PrusaLinkPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-23 19:55:14.000000 PrusaLinkPy-1.0.1/PrusaLinkPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:55:14.000000 PrusaLinkPy-1.0.1/PrusaLinkPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 19:55:14.000000 PrusaLinkPy-1.0.1/PrusaLinkPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8397 2023-05-23 19:54:44.000000 PrusaLinkPy-1.0.1/README.md
+-rw-rw-rw-   0        0        0      691 2023-05-23 19:54:31.000000 PrusaLinkPy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 19:55:14.750947 PrusaLinkPy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      206 2023-05-23 19:54:55.000000 PrusaLinkPy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:55:14.750947 PrusaLinkPy-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 PrusaLinkPy-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 PrusaLinkPy-1.0.1/tests/test_PrusaLinkPy.py
```

### Comparing `PrusaLinkPy-1.0.0/LICENSE` & `PrusaLinkPy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PrusaLinkPy-1.0.0/PKG-INFO` & `PrusaLinkPy-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrusaLinkPy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library to interface with the PrusaLink API
 Author: Guillaume RICO
 Author-email: Guillaume RICO <guillaume.rico@alpesmesures.fr>
 License: Copyright (c) 2023 Guillaume RICO
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -19,17 +19,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/guillaume-rico/prusaLink
-Project-URL: Bug Tracker, https://github.com/guillaume-rico/prusaLink/issues
-Project-URL: repository, https://github.com/guillaume-rico/prusaLink.git
+Project-URL: Homepage, https://github.com/guillaume-rico/PrusaLinkPy
+Project-URL: Bug Tracker, https://github.com/guillaume-rico/PrusaLinkPy/issues
+Project-URL: repository, https://github.com/guillaume-rico/PrusaLinkPy.git
 Keywords: Prusalink,API,Mini
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -304,22 +304,18 @@
 **[Link to Buddy code](https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/master/lib/WUI/link_content/prusa_link_api.cpp#L276)**
 
 GET/POST /api/download 
 **[Link to Buddy code](https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/master/lib/WUI/link_content/prusa_link_api.cpp#L289)**
 
 # Change Log 
 
-0.1.0 :
+1.0.0 :
 
  - First Release
 
-0.1.1 :
-
- - get_files : Bug correction in default dir
- - rm : add rm function
 
 # Inspiration
 
 An other lib : 
 
 https://github.com/home-assistant-libs/PrusaLinkPy/blob/main/PrusaLinkPy/
```

### Comparing `PrusaLinkPy-1.0.0/PrusaLinkPy/__init__.py` & `PrusaLinkPy-1.0.1/PrusaLinkPy/__init__.py`

 * *Files identical despite different names*

### Comparing `PrusaLinkPy-1.0.0/PrusaLinkPy.egg-info/PKG-INFO` & `PrusaLinkPy-1.0.1/PrusaLinkPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrusaLinkPy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library to interface with the PrusaLink API
 Author: Guillaume RICO
 Author-email: Guillaume RICO <guillaume.rico@alpesmesures.fr>
 License: Copyright (c) 2023 Guillaume RICO
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -19,17 +19,17 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/guillaume-rico/prusaLink
-Project-URL: Bug Tracker, https://github.com/guillaume-rico/prusaLink/issues
-Project-URL: repository, https://github.com/guillaume-rico/prusaLink.git
+Project-URL: Homepage, https://github.com/guillaume-rico/PrusaLinkPy
+Project-URL: Bug Tracker, https://github.com/guillaume-rico/PrusaLinkPy/issues
+Project-URL: repository, https://github.com/guillaume-rico/PrusaLinkPy.git
 Keywords: Prusalink,API,Mini
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -304,22 +304,18 @@
 **[Link to Buddy code](https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/master/lib/WUI/link_content/prusa_link_api.cpp#L276)**
 
 GET/POST /api/download 
 **[Link to Buddy code](https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/master/lib/WUI/link_content/prusa_link_api.cpp#L289)**
 
 # Change Log 
 
-0.1.0 :
+1.0.0 :
 
  - First Release
 
-0.1.1 :
-
- - get_files : Bug correction in default dir
- - rm : add rm function
 
 # Inspiration
 
 An other lib : 
 
 https://github.com/home-assistant-libs/PrusaLinkPy/blob/main/PrusaLinkPy/
```

### Comparing `PrusaLinkPy-1.0.0/README.md` & `PrusaLinkPy-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -484,47 +484,42 @@
 00001e30: 6875 622e 636f 6d2f 7072 7573 6133 642f  hub.com/prusa3d/
 00001e40: 5072 7573 612d 4669 726d 7761 7265 2d42  Prusa-Firmware-B
 00001e50: 7564 6479 2f62 6c6f 622f 6d61 7374 6572  uddy/blob/master
 00001e60: 2f6c 6962 2f57 5549 2f6c 696e 6b5f 636f  /lib/WUI/link_co
 00001e70: 6e74 656e 742f 7072 7573 615f 6c69 6e6b  ntent/prusa_link
 00001e80: 5f61 7069 2e63 7070 234c 3238 3929 2a2a  _api.cpp#L289)**
 00001e90: 0d0a 0d0a 2320 4368 616e 6765 204c 6f67  ....# Change Log
-00001ea0: 200d 0a0d 0a30 2e31 2e30 203a 0d0a 0d0a   ....0.1.0 :....
+00001ea0: 200d 0a0d 0a31 2e30 2e30 203a 0d0a 0d0a   ....1.0.0 :....
 00001eb0: 202d 2046 6972 7374 2052 656c 6561 7365   - First Release
-00001ec0: 0d0a 0d0a 302e 312e 3120 3a0d 0a0d 0a20  ....0.1.1 :.... 
-00001ed0: 2d20 6765 745f 6669 6c65 7320 3a20 4275  - get_files : Bu
-00001ee0: 6720 636f 7272 6563 7469 6f6e 2069 6e20  g correction in 
-00001ef0: 6465 6661 756c 7420 6469 720d 0a20 2d20  default dir.. - 
-00001f00: 726d 203a 2061 6464 2072 6d20 6675 6e63  rm : add rm func
-00001f10: 7469 6f6e 0d0a 0d0a 2320 496e 7370 6972  tion....# Inspir
-00001f20: 6174 696f 6e0d 0a0d 0a41 6e20 6f74 6865  ation....An othe
-00001f30: 7220 6c69 6220 3a20 0d0a 0d0a 6874 7470  r lib : ....http
-00001f40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00001f50: 6f6d 652d 6173 7369 7374 616e 742d 6c69  ome-assistant-li
-00001f60: 6273 2f50 7275 7361 4c69 6e6b 5079 2f62  bs/PrusaLinkPy/b
-00001f70: 6c6f 622f 6d61 696e 2f50 7275 7361 4c69  lob/main/PrusaLi
-00001f80: 6e6b 5079 2f0d 0a0d 0a0d 0a4c 6573 2063  nkPy/......Les c
-00001f90: 6f6d 6d61 6e64 6573 2064 616e 7320 6c61  ommandes dans la
-00001fa0: 206d 696e 6920 3a0d 0a68 7474 7073 3a2f   mini :..https:/
-00001fb0: 2f67 6974 6875 622e 636f 6d2f 7072 7573  /github.com/prus
-00001fc0: 6133 642f 5072 7573 612d 4669 726d 7761  a3d/Prusa-Firmwa
-00001fd0: 7265 2d42 7564 6479 2f62 6c6f 622f 6d61  re-Buddy/blob/ma
-00001fe0: 7374 6572 2f6c 6962 2f57 5549 2f6c 696e  ster/lib/WUI/lin
-00001ff0: 6b5f 636f 6e74 656e 742f 6261 7369 635f  k_content/basic_
-00002000: 6765 7473 2e63 7070 0d0a 0d0a 0d0a 0d0a  gets.cpp........
-00002010: 2320 436f 6e73 7472 7569 7265 206c 6120  # Construire la 
-00002020: 6c69 620d 0a0d 0a20 2020 2070 7920 2d6d  lib....    py -m
-00002030: 2062 7569 6c64 0d0a 0d0a 546f 2075 706c   build....To upl
-00002040: 6f61 6420 746f 2074 6573 7470 6920 7265  oad to testpi re
-00002050: 706f 203a 0d0a 0d0a 2020 2020 7079 202d  po :....    py -
-00002060: 6d20 7477 696e 6520 7570 6c6f 6164 202d  m twine upload -
-00002070: 2d72 6570 6f73 6974 6f72 7920 7465 7374  -repository test
-00002080: 7069 2064 6973 742f 2a0d 0a0d 0a54 6f20  pi dist/*....To 
-00002090: 7570 6c6f 6164 2074 6f20 7079 7069 2072  upload to pypi r
-000020a0: 6570 6f20 3a0d 0a0d 0a20 2020 2070 7920  epo :....    py 
-000020b0: 2d6d 2074 7769 6e65 2075 706c 6f61 6420  -m twine upload 
-000020c0: 6469 7374 2f2a 0d0a 0d0a 0d0a 6874 7470  dist/*......http
-000020d0: 733a 2f2f 6d65 6469 756d 2e63 6f6d 2f61  s://medium.com/a
-000020e0: 6e61 6c79 7469 6373 2d76 6964 6879 612f  nalytics-vidhya/
-000020f0: 686f 772d 746f 2d63 7265 6174 652d 612d  how-to-create-a-
-00002100: 7079 7468 6f6e 2d6c 6962 7261 7279 2d37  python-library-7
-00002110: 6435 6165 6138 3063 6333 660d 0a0d 0a    d5aea80cc3f....
+00001ec0: 0d0a 0d0a 0d0a 2320 496e 7370 6972 6174  ......# Inspirat
+00001ed0: 696f 6e0d 0a0d 0a41 6e20 6f74 6865 7220  ion....An other 
+00001ee0: 6c69 6220 3a20 0d0a 0d0a 6874 7470 733a  lib : ....https:
+00001ef0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6f6d  //github.com/hom
+00001f00: 652d 6173 7369 7374 616e 742d 6c69 6273  e-assistant-libs
+00001f10: 2f50 7275 7361 4c69 6e6b 5079 2f62 6c6f  /PrusaLinkPy/blo
+00001f20: 622f 6d61 696e 2f50 7275 7361 4c69 6e6b  b/main/PrusaLink
+00001f30: 5079 2f0d 0a0d 0a0d 0a4c 6573 2063 6f6d  Py/......Les com
+00001f40: 6d61 6e64 6573 2064 616e 7320 6c61 206d  mandes dans la m
+00001f50: 696e 6920 3a0d 0a68 7474 7073 3a2f 2f67  ini :..https://g
+00001f60: 6974 6875 622e 636f 6d2f 7072 7573 6133  ithub.com/prusa3
+00001f70: 642f 5072 7573 612d 4669 726d 7761 7265  d/Prusa-Firmware
+00001f80: 2d42 7564 6479 2f62 6c6f 622f 6d61 7374  -Buddy/blob/mast
+00001f90: 6572 2f6c 6962 2f57 5549 2f6c 696e 6b5f  er/lib/WUI/link_
+00001fa0: 636f 6e74 656e 742f 6261 7369 635f 6765  content/basic_ge
+00001fb0: 7473 2e63 7070 0d0a 0d0a 0d0a 0d0a 2320  ts.cpp........# 
+00001fc0: 436f 6e73 7472 7569 7265 206c 6120 6c69  Construire la li
+00001fd0: 620d 0a0d 0a20 2020 2070 7920 2d6d 2062  b....    py -m b
+00001fe0: 7569 6c64 0d0a 0d0a 546f 2075 706c 6f61  uild....To uploa
+00001ff0: 6420 746f 2074 6573 7470 6920 7265 706f  d to testpi repo
+00002000: 203a 0d0a 0d0a 2020 2020 7079 202d 6d20   :....    py -m 
+00002010: 7477 696e 6520 7570 6c6f 6164 202d 2d72  twine upload --r
+00002020: 6570 6f73 6974 6f72 7920 7465 7374 7069  epository testpi
+00002030: 2064 6973 742f 2a0d 0a0d 0a54 6f20 7570   dist/*....To up
+00002040: 6c6f 6164 2074 6f20 7079 7069 2072 6570  load to pypi rep
+00002050: 6f20 3a0d 0a0d 0a20 2020 2070 7920 2d6d  o :....    py -m
+00002060: 2074 7769 6e65 2075 706c 6f61 6420 6469   twine upload di
+00002070: 7374 2f2a 0d0a 0d0a 0d0a 6874 7470 733a  st/*......https:
+00002080: 2f2f 6d65 6469 756d 2e63 6f6d 2f61 6e61  //medium.com/ana
+00002090: 6c79 7469 6373 2d76 6964 6879 612f 686f  lytics-vidhya/ho
+000020a0: 772d 746f 2d63 7265 6174 652d 612d 7079  w-to-create-a-py
+000020b0: 7468 6f6e 2d6c 6962 7261 7279 2d37 6435  thon-library-7d5
+000020c0: 6165 6138 3063 6333 660d 0a0d 0a         aea80cc3f....
```

