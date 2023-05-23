# Comparing `tmp/kronbinations-1.8.tar.gz` & `tmp/kronbinations-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kronbinations-1.8.tar", last modified: Fri Apr 28 08:47:36 2023, max compression
+gzip compressed data, was "kronbinations-1.9.tar", last modified: Fri Apr 28 09:04:59 2023, max compression
```

## Comparing `kronbinations-1.8.tar` & `kronbinations-1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:47:36.480310 kronbinations-1.8/
--rw-rw-rw-   0        0        0     1096 2023-04-28 08:47:26.000000 kronbinations-1.8/LICENSE
--rw-rw-rw-   0        0        0     6395 2023-04-28 08:47:36.481322 kronbinations-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5867 2023-04-28 08:47:26.000000 kronbinations-1.8/README.md
--rw-rw-rw-   0        0        0      523 2023-04-28 08:47:36.487902 kronbinations-1.8/setup.cfg
--rw-rw-rw-   0        0        0      880 2023-04-28 08:47:26.000000 kronbinations-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:47:36.310546 kronbinations-1.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 08:47:36.384424 kronbinations-1.8/src/kronbinations/
--rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.8/src/kronbinations/JIT_Array.py
--rw-rw-rw-   0        0        0    17596 2023-04-28 08:47:16.000000 kronbinations-1.8/src/kronbinations/JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.8/src/kronbinations/Kron_Array.py
--rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.8/src/kronbinations/Kron_Fun_Modifier.py
--rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.8/src/kronbinations/__init__.py
--rw-rw-rw-   0        0        0    12796 2023-04-28 08:20:15.000000 kronbinations-1.8/src/kronbinations/kronbinations.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:47:36.468219 kronbinations-1.8/src/kronbinations.egg-info/
--rw-rw-rw-   0        0        0     6395 2023-04-28 08:47:35.000000 kronbinations-1.8/src/kronbinations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-04-28 08:47:35.000000 kronbinations-1.8/src/kronbinations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:47:35.000000 kronbinations-1.8/src/kronbinations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 08:47:35.000000 kronbinations-1.8/src/kronbinations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 08:47:35.000000 kronbinations-1.8/src/kronbinations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 08:47:36.477782 kronbinations-1.8/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.8/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.8/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:59.969977 kronbinations-1.9/
+-rw-rw-rw-   0        0        0     1096 2023-04-28 09:04:55.000000 kronbinations-1.9/LICENSE
+-rw-rw-rw-   0        0        0     6395 2023-04-28 09:04:59.971507 kronbinations-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5867 2023-04-28 09:04:55.000000 kronbinations-1.9/README.md
+-rw-rw-rw-   0        0        0      523 2023-04-28 09:04:59.975552 kronbinations-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-04-28 09:04:55.000000 kronbinations-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:59.895738 kronbinations-1.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:59.927321 kronbinations-1.9/src/kronbinations/
+-rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.9/src/kronbinations/JIT_Array.py
+-rw-rw-rw-   0        0        0    17596 2023-04-28 08:47:16.000000 kronbinations-1.9/src/kronbinations/JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.9/src/kronbinations/Kron_Array.py
+-rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.9/src/kronbinations/Kron_Fun_Modifier.py
+-rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.9/src/kronbinations/__init__.py
+-rw-rw-rw-   0        0        0    12796 2023-04-28 08:20:15.000000 kronbinations-1.9/src/kronbinations/kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:59.963447 kronbinations-1.9/src/kronbinations.egg-info/
+-rw-rw-rw-   0        0        0     6395 2023-04-28 09:04:59.000000 kronbinations-1.9/src/kronbinations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-28 09:04:59.000000 kronbinations-1.9/src/kronbinations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:04:59.000000 kronbinations-1.9/src/kronbinations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 09:04:59.000000 kronbinations-1.9/src/kronbinations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 09:04:59.000000 kronbinations-1.9/src/kronbinations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:59.967962 kronbinations-1.9/test/
+-rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.9/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.9/test/test_kronbinations.py
```

### Comparing `kronbinations-1.8/LICENSE` & `kronbinations-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/PKG-INFO` & `kronbinations-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.8
+Version: 1.9
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.8.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.9.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kronbinations-1.8/README.md` & `kronbinations-1.9/README.md`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/setup.cfg` & `kronbinations-1.9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 380d  ..version = 1.8.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 390d  ..version = 1.9.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6b72  description = kr
 00000080: 6f6e 6269 6e61 7469 6f6e 7320 6973 2075  onbinations is u
 00000090: 7365 6420 746f 2072 656d 6f76 6520 6e65  sed to remove ne
@@ -16,15 +16,15 @@
 000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
 00000110: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
 00000120: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 00000130: 622e 636f 6d2f 4e74 726f 7069 632f 6b72  b.com/Ntropic/kr
 00000140: 6f6e 6269 6e61 7469 6f6e 732f 6172 6368  onbinations/arch
 00000150: 6976 652f 7265 6673 2f74 6167 732f 7631  ive/refs/tags/v1
-00000160: 2e38 2e74 6172 2e67 7a0d 0a50 726f 6772  .8.tar.gz..Progr
+00000160: 2e39 2e74 6172 2e67 7a0d 0a50 726f 6772  .9.tar.gz..Progr
 00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000180: 3d20 3a20 5079 7468 6f6e 203a 3a20 330d  = : Python :: 3.
 00000190: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001a0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
 000001b0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
 000001c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
 000001d0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
```

### Comparing `kronbinations-1.8/setup.py` & `kronbinations-1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "kronbinations",
-    version              = "1.8",
+    version               = "1.9",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "kronbinations is used to remove nested loops and perform parameter sweeps.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.8.tar.gz",
+    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.9.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    install_requires=["numpy", "tqdm"],
+    install_requires=["numpy", "weighted_tqdm"],
     python_requires=">=3.6",
 )
```

### Comparing `kronbinations-1.8/src/kronbinations/JIT_Array.py` & `kronbinations-1.9/src/kronbinations/JIT_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/src/kronbinations/JIT_kronbinations.py` & `kronbinations-1.9/src/kronbinations/JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/src/kronbinations/Kron_Array.py` & `kronbinations-1.9/src/kronbinations/Kron_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/src/kronbinations/Kron_Fun_Modifier.py` & `kronbinations-1.9/src/kronbinations/Kron_Fun_Modifier.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/src/kronbinations/kronbinations.py` & `kronbinations-1.9/src/kronbinations/kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/src/kronbinations.egg-info/PKG-INFO` & `kronbinations-1.9/src/kronbinations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.8
+Version: 1.9
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.8.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.9.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kronbinations-1.8/test/test_JIT_kronbinations.py` & `kronbinations-1.9/test/test_JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.8/test/test_kronbinations.py` & `kronbinations-1.9/test/test_kronbinations.py`

 * *Files identical despite different names*

