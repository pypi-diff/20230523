# Comparing `tmp/hypothesis-rdkit-0.1.tar.gz` & `tmp/hypothesis-rdkit-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-rdkit-0.1.tar", last modified: Mon Feb 20 00:21:09 2023, max compression
+gzip compressed data, was "hypothesis-rdkit-0.4.tar", last modified: Tue May 23 15:33:44 2023, max compression
```

## Comparing `hypothesis-rdkit-0.1.tar` & `hypothesis-rdkit-0.4.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/MANIFEST.in
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1269 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      829 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/hypothesis_rdkit/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)   441809 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/fragments.smi
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/hook.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     6131 2023-02-19 23:39:15.000000 hypothesis-rdkit-0.1/hypothesis_rdkit/strategy.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1269 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      386 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/entry_points.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-02-20 00:21:09.000000 hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-20 00:21:09.557101 hypothesis-rdkit-0.1/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      768 2023-02-20 00:20:56.000000 hypothesis-rdkit-0.1/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1081 2023-03-06 20:54:00.000000 hypothesis-rdkit-0.4/LICENSE
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/MANIFEST.in
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1475 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      829 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/README.md
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/hypothesis_rdkit/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)   441809 2023-05-23 15:28:37.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/fragments.smi
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/hook.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     6131 2023-05-23 15:28:37.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/strategy.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1475 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      459 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/entry_points.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       30 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/top_level.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1006 2023-05-23 15:33:30.000000 hypothesis-rdkit-0.4/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      648 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/tests/test_mol_blocks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      665 2023-05-23 15:28:37.000000 hypothesis-rdkit-0.4/tests/test_mols.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      607 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/tests/test_smiles.py
```

### Comparing `hypothesis-rdkit-0.1/PKG-INFO` & `hypothesis-rdkit-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.1
+Version: 0.4
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
+License: MIT
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Framework :: Hypothesis
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # hypothesis-rdkit
 
 ## Installation
 
 ```sh
 pip install -U hypothesis-rdkit
```

### Comparing `hypothesis-rdkit-0.1/README.md` & `hypothesis-rdkit-0.4/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.1/hypothesis_rdkit/fragments.smi` & `hypothesis-rdkit-0.4/hypothesis_rdkit/fragments.smi`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.1/hypothesis_rdkit/strategy.py` & `hypothesis-rdkit-0.4/hypothesis_rdkit/strategy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.1/hypothesis_rdkit.egg-info/PKG-INFO` & `hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.1
+Version: 0.4
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
+License: MIT
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Framework :: Hypothesis
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # hypothesis-rdkit
 
 ## Installation
 
 ```sh
 pip install -U hypothesis-rdkit
```

### Comparing `hypothesis-rdkit-0.1/setup.py` & `hypothesis-rdkit-0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="hypothesis-rdkit",
-    version="0.1",
+    version="0.4",
     maintainer="Steffen Hirte",
     maintainer_email="shirte@users.noreply.github.com",
     packages=find_packages(),
     url="https://github.com/shirte/hypothesis-rdkit",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    install_requires=["hypothesis", "rdkit"],
+    license="MIT",
+    license_files=("LICENSE",),
+    install_requires=["hypothesis"],
+    extras_require={"dev": ["black", "isort"]},
     entry_points={"hypothesis": {"_ = hypothesis_rdkit.hook:_hypothesis_setup_hook"}},
     include_package_data=True,
     classifiers=[
+        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
+        "Topic :: Scientific/Engineering :: Chemistry",
         "Framework :: Hypothesis",
+        "License :: OSI Approved :: MIT License",
     ],
 )
```

