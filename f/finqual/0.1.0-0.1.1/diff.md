# Comparing `tmp/finqual-0.1.0.tar.gz` & `tmp/finqual-0.1.1.tar.gz`

## Comparing `finqual-0.1.0.tar` & `finqual-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0   118637 2020-02-02 00:00:00.000000 finqual-0.1.0/src/FinQual/FinQual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.0/src/FinQual/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 finqual-0.1.0/README.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 finqual-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 finqual-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0   118637 2020-02-02 00:00:00.000000 finqual-0.1.1/src/FinQual/FinQual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.1/src/FinQual/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 finqual-0.1.1/README.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 finqual-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 finqual-0.1.1/PKG-INFO
```

### Comparing `finqual-0.1.0/src/FinQual/FinQual.py` & `finqual-0.1.1/src/FinQual/FinQual.py`

 * *Files identical despite different names*

### Comparing `finqual-0.1.0/LICENSE.txt` & `finqual-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.0/README.md` & `finqual-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `finqual-0.1.0/PKG-INFO` & `finqual-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: FinQual
-Version: 0.1.0
-Summary: A WIP package to retrieve financial information
+Name: finqual
+Version: 0.1.1
+Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet and cashflow statement
 Author: Myztika
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

