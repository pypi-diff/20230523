# Comparing `tmp/algorithmadts-0.1.5.tar.gz` & `tmp/algorithmadts-0.1.6.tar.gz`

## Comparing `algorithmadts-0.1.5.tar` & `algorithmadts-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/src/AlgorithmADTs/.DS_Store
--rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/src/AlgorithmADTs/AbstractDataTypes.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/src/AlgorithmADTs/GraphAlgorithms.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/src/AlgorithmADTs/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/tests/experimenting.ipynb
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/tests/test_GraphAlgorithms.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/LICENSE
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/README.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 algorithmadts-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.DS_Store
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/src/AlgorithmADTs/.DS_Store
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/src/AlgorithmADTs/AbstractDataTypes.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/src/AlgorithmADTs/GraphAlgorithms.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/src/AlgorithmADTs/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/tests/experimenting.ipynb
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/tests/test_GraphAlgorithms.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/README.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 algorithmadts-0.1.6/PKG-INFO
```

### Comparing `algorithmadts-0.1.5/.DS_Store` & `algorithmadts-0.1.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/src/.DS_Store` & `algorithmadts-0.1.6/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/src/AlgorithmADTs/.DS_Store` & `algorithmadts-0.1.6/src/AlgorithmADTs/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/src/AlgorithmADTs/AbstractDataTypes.py` & `algorithmadts-0.1.6/src/AlgorithmADTs/AbstractDataTypes.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/src/AlgorithmADTs/GraphAlgorithms.py` & `algorithmadts-0.1.6/src/AlgorithmADTs/GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/tests/experimenting.ipynb` & `algorithmadts-0.1.6/tests/experimenting.ipynb`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/tests/test_GraphAlgorithms.py` & `algorithmadts-0.1.6/tests/test_GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/LICENSE` & `algorithmadts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/README.md` & `algorithmadts-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.5/PKG-INFO` & `algorithmadts-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgorithmADTs
-Version: 0.1.5
+Version: 0.1.6
 Summary: General purpose Abstract Data Types for Algorithmics
 Author-email: Finlay <finlay3.141@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

