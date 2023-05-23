# Comparing `tmp/scinumtools-0.1.0.tar.gz` & `tmp/scinumtools-0.2.0.tar.gz`

## Comparing `scinumtools-0.1.0.tar` & `scinumtools-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scinumtools-0.1.0/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-0.1.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scinumtools-0.1.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 scinumtools-0.1.0/src/scinumtools/structs/RowCollectorClass.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scinumtools-0.1.0/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 scinumtools-0.1.0/tests/test_struct.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-0.1.0/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-0.1.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scinumtools-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-0.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scinumtools-0.2.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scinumtools-0.2.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 scinumtools-0.2.0/src/scinumtools/structs/RowCollectorClass.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scinumtools-0.2.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 scinumtools-0.2.0/tests/test_struct.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-0.2.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-0.2.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-0.2.0/PKG-INFO
```

### Comparing `scinumtools-0.1.0/.github/workflows/python-publish.yml` & `scinumtools-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-0.1.0/src/scinumtools/structs/RowCollectorClass.py` & `scinumtools-0.2.0/src/scinumtools/structs/RowCollectorClass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 import numpy as np
 import pandas as pd
+from typing import Union
 
 @dataclass
 class RowCollector:
-    """ Initialization of RowCollector
+    """ RowCollector class collect table rows and transform them into one of available formats
 
     Example of use:
 
     ..code-block::
     
         import scinumtools as snt
         
@@ -24,15 +25,15 @@
     
     def __enter__(self):
         return self
     
     def __exit__(self, type, value, tb):
         pass
     
-    def __init__(self, columns):
+    def __init__(self, columns: Union[list,dict]):
         self._columns = []
         if isinstance(columns,list):
             # Columns are standard python lists
             self._numpy = False
             for column in columns:
                 setattr(self,column,[])
                 self._columns.append(column)
@@ -41,15 +42,15 @@
             self._numpy = True
             for column, kwargs in columns.items():
                 setattr(self,column,np.array([],**kwargs))
                 self._columns.append(column)
         else:
             raise Exception("Columns parameter can be either a list of column names or a dictionary of column numpy settings.")
         
-    def append(self, values):
+    def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         if self._numpy:
             for n, name in enumerate(self._columns):
                 data = getattr(self,name)
@@ -63,23 +64,25 @@
         """ Convert class data to a dictionary of lists/arrays
         """
         data = {}
         for name in self._columns:
             data[name] = getattr(self,name)
         return data
     
-    def to_dataframe(self, columns=None):
+    def to_dataframe(self, columns: Union[list,dict]=None):
         """ Convert class data to a pandas data frame
 
         :param columns: This can be either a list of columns or a dictionary of column:title pairs. If not set, all coumns are being taken.
         """
         if isinstance(columns,dict):
             return pd.DataFrame({title:getattr(self,name) for name,title in columns.items()})
         elif isinstance(columns,list):
             return pd.DataFrame({name:getattr(self,name) for name in columns})
         else:
             return pd.DataFrame({name:getattr(self,name) for name in self._columns})
         
-    def to_string(self, index=True):
-        """ Convert class data to a string using pandas dataframe
+    def to_text(self, **kwargs):
+        """ Convert class data to a text using pandas dataframe
+
+        :param kwargs: kwargs of DataFrame's to_string() method
         """
-        return self.to_dataframe().to_string(index=index)
+        return self.to_dataframe().to_string(**kwargs)
```

### Comparing `scinumtools-0.1.0/.gitignore` & `scinumtools-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-0.1.0/pyproject.toml` & `scinumtools-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-0.1.0/PKG-INFO` & `scinumtools-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

