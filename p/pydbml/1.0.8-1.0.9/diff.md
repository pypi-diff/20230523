# Comparing `tmp/pydbml-1.0.8.tar.gz` & `tmp/pydbml-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbml-1.0.8.tar", last modified: Sun May 14 11:55:57 2023, max compression
+gzip compressed data, was "pydbml-1.0.9.tar", last modified: Tue May 23 17:35:36 2023, max compression
```

## Comparing `pydbml-1.0.8.tar` & `pydbml-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/
--rw-r--r--   0 user      (1000) user      (1000)     1056 2022-08-27 12:11:12.000000 pydbml-1.0.8/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3897 2023-05-14 11:55:57.296517 pydbml-1.0.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3211 2023-05-14 11:55:38.000000 pydbml-1.0.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.293184 pydbml-1.0.8/pydbml/
--rw-r--r--   0 user      (1000) user      (1000)      202 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.293184 pydbml-1.0.8/pydbml/classes/
--rw-r--r--   0 user      (1000) user      (1000)      283 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1122 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/base.py
--rw-r--r--   0 user      (1000) user      (1000)     4935 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/column.py
--rw-r--r--   0 user      (1000) user      (1000)     3911 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/enum.py
--rw-r--r--   0 user      (1000) user      (1000)      589 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/expression.py
--rw-r--r--   0 user      (1000) user      (1000)     5009 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/index.py
--rw-r--r--   0 user      (1000) user      (1000)     2563 2022-10-23 09:04:28.000000 pydbml-1.0.8/pydbml/classes/note.py
--rw-r--r--   0 user      (1000) user      (1000)     1447 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/project.py
--rw-r--r--   0 user      (1000) user      (1000)     9058 2022-11-20 08:34:11.000000 pydbml-1.0.8/pydbml/classes/reference.py
--rw-r--r--   0 user      (1000) user      (1000)     8651 2022-12-11 11:12:03.000000 pydbml-1.0.8/pydbml/classes/table.py
--rw-r--r--   0 user      (1000) user      (1000)     1470 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/table_group.py
--rw-r--r--   0 user      (1000) user      (1000)       73 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/constants.py
--rw-r--r--   0 user      (1000) user      (1000)     7738 2022-11-20 08:34:11.000000 pydbml-1.0.8/pydbml/database.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/pydbml/definitions/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3463 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/column.py
--rw-r--r--   0 user      (1000) user      (1000)     1019 2023-05-14 11:55:38.000000 pydbml-1.0.8/pydbml/definitions/common.py
--rw-r--r--   0 user      (1000) user      (1000)     2123 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/enum.py
--rw-r--r--   0 user      (1000) user      (1000)     1137 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/generic.py
--rw-r--r--   0 user      (1000) user      (1000)     2777 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/index.py
--rw-r--r--   0 user      (1000) user      (1000)     1369 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/project.py
--rw-r--r--   0 user      (1000) user      (1000)     4357 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/reference.py
--rw-r--r--   0 user      (1000) user      (1000)     2613 2023-05-14 11:41:15.000000 pydbml-1.0.8/pydbml/definitions/table.py
--rw-r--r--   0 user      (1000) user      (1000)      903 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/table_group.py
--rw-r--r--   0 user      (1000) user      (1000)      389 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/exceptions.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/pydbml/parser/
--rw-r--r--   0 user      (1000) user      (1000)       27 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/parser/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     8642 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/parser/blueprints.py
--rw-r--r--   0 user      (1000) user      (1000)     6616 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/parser/parser.py
--rw-r--r--   0 user      (1000) user      (1000)     1578 2022-12-11 11:28:25.000000 pydbml-1.0.8/pydbml/tools.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.293184 pydbml-1.0.8/pydbml.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3897 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1074 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-14 11:55:57.296517 pydbml-1.0.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-14 11:55:38.000000 pydbml-1.0.8/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/test/
--rw-r--r--   0 user      (1000) user      (1000)    14118 2022-10-23 09:24:06.000000 pydbml-1.0.8/test/test_database.py
--rw-r--r--   0 user      (1000) user      (1000)     9929 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_docs.py
--rw-r--r--   0 user      (1000) user      (1000)      996 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_doctest.py
--rw-r--r--   0 user      (1000) user      (1000)     3073 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_editing.py
--rw-r--r--   0 user      (1000) user      (1000)     3952 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_integration.py
--rw-r--r--   0 user      (1000) user      (1000)     5975 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_parser.py
--rw-r--r--   0 user      (1000) user      (1000)     3515 2022-12-11 11:28:25.000000 pydbml-1.0.8/test/test_tools.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.857257 pydbml-1.0.9/
+-rw-r--r--   0 user       (502) staff       (20)     1056 2022-08-29 11:30:28.000000 pydbml-1.0.9/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)     3899 2023-05-23 17:35:36.856786 pydbml-1.0.9/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)     3211 2023-05-23 17:31:22.000000 pydbml-1.0.9/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.810101 pydbml-1.0.9/pydbml/
+-rw-r--r--   0 user       (502) staff       (20)      202 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.831354 pydbml-1.0.9/pydbml/classes/
+-rw-r--r--   0 user       (502) staff       (20)      283 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1122 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/base.py
+-rw-r--r--   0 user       (502) staff       (20)     4935 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/column.py
+-rw-r--r--   0 user       (502) staff       (20)     3911 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/enum.py
+-rw-r--r--   0 user       (502) staff       (20)      589 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/expression.py
+-rw-r--r--   0 user       (502) staff       (20)     5009 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/index.py
+-rw-r--r--   0 user       (502) staff       (20)     2563 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/note.py
+-rw-r--r--   0 user       (502) staff       (20)     1447 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/project.py
+-rw-r--r--   0 user       (502) staff       (20)     9058 2022-12-11 09:05:50.000000 pydbml-1.0.9/pydbml/classes/reference.py
+-rw-r--r--   0 user       (502) staff       (20)     8651 2023-05-23 17:31:22.000000 pydbml-1.0.9/pydbml/classes/table.py
+-rw-r--r--   0 user       (502) staff       (20)     1470 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/classes/table_group.py
+-rw-r--r--   0 user       (502) staff       (20)       73 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/constants.py
+-rw-r--r--   0 user       (502) staff       (20)     7781 2023-05-23 17:31:22.000000 pydbml-1.0.9/pydbml/database.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.844633 pydbml-1.0.9/pydbml/definitions/
+-rw-r--r--   0 user       (502) staff       (20)        0 2020-04-14 08:48:28.000000 pydbml-1.0.9/pydbml/definitions/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3463 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/column.py
+-rw-r--r--   0 user       (502) staff       (20)     1019 2023-05-23 17:31:22.000000 pydbml-1.0.9/pydbml/definitions/common.py
+-rw-r--r--   0 user       (502) staff       (20)     2123 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/enum.py
+-rw-r--r--   0 user       (502) staff       (20)     1137 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/generic.py
+-rw-r--r--   0 user       (502) staff       (20)     2777 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/index.py
+-rw-r--r--   0 user       (502) staff       (20)     1369 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/project.py
+-rw-r--r--   0 user       (502) staff       (20)     4357 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/reference.py
+-rw-r--r--   0 user       (502) staff       (20)     2613 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/table.py
+-rw-r--r--   0 user       (502) staff       (20)      903 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/definitions/table_group.py
+-rw-r--r--   0 user       (502) staff       (20)      389 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/exceptions.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.848000 pydbml-1.0.9/pydbml/parser/
+-rw-r--r--   0 user       (502) staff       (20)       27 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/parser/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     8642 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/parser/blueprints.py
+-rw-r--r--   0 user       (502) staff       (20)     6616 2022-08-29 11:30:28.000000 pydbml-1.0.9/pydbml/parser/parser.py
+-rw-r--r--   0 user       (502) staff       (20)     1578 2023-05-23 17:31:22.000000 pydbml-1.0.9/pydbml/tools.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.815382 pydbml-1.0.9/pydbml.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)     3899 2023-05-23 17:35:36.000000 pydbml-1.0.9/pydbml.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)     1074 2023-05-23 17:35:36.000000 pydbml-1.0.9/pydbml.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-05-23 17:35:36.000000 pydbml-1.0.9/pydbml.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       17 2023-05-23 17:35:36.000000 pydbml-1.0.9/pydbml.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)        7 2023-05-23 17:35:36.000000 pydbml-1.0.9/pydbml.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-05-23 17:35:36.857515 pydbml-1.0.9/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     1149 2023-05-23 17:31:22.000000 pydbml-1.0.9/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-23 17:35:36.855826 pydbml-1.0.9/test/
+-rw-r--r--   0 user       (502) staff       (20)    14118 2022-11-10 09:04:21.000000 pydbml-1.0.9/test/test_database.py
+-rw-r--r--   0 user       (502) staff       (20)     9929 2022-08-29 11:30:28.000000 pydbml-1.0.9/test/test_docs.py
+-rw-r--r--   0 user       (502) staff       (20)      996 2022-08-29 11:30:28.000000 pydbml-1.0.9/test/test_doctest.py
+-rw-r--r--   0 user       (502) staff       (20)     3073 2022-08-29 11:30:28.000000 pydbml-1.0.9/test/test_editing.py
+-rw-r--r--   0 user       (502) staff       (20)     3952 2022-08-29 11:30:28.000000 pydbml-1.0.9/test/test_integration.py
+-rw-r--r--   0 user       (502) staff       (20)     6283 2023-05-23 17:31:22.000000 pydbml-1.0.9/test/test_parser.py
+-rw-r--r--   0 user       (502) staff       (20)     3515 2023-05-23 17:31:22.000000 pydbml-1.0.9/test/test_tools.py
```

### Comparing `pydbml-1.0.8/LICENSE` & `pydbml-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/PKG-INFO` & `pydbml-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbml
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python parser and builder for DBML
 Home-page: https://github.com/Vanderhoof/PyDBML
 Author: Daniil Minukhin
 Author-email: ddddsa@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -171,7 +171,9 @@
     "order_id" int
     "product_id" int
     "quantity" int [default: 1]
 }
 ...
 
 ```
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydbml Version: 1.0.8 Summary: Python parser and
+Metadata-Version: 2.1 Name: pydbml Version: 1.0.9 Summary: Python parser and
 builder for DBML Home-page: https://github.com/Vanderhoof/PyDBML Author: Daniil
 Minukhin Author-email: ddddsa@gmail.com License: MIT Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Topic :: Documentation Classifier: Topic :: Text
 Processing :: Markup Classifier: Topic :: Utilities Requires-Python: >=3.8
```

### Comparing `pydbml-1.0.8/README.md` & `pydbml-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/base.py` & `pydbml-1.0.9/pydbml/classes/base.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/column.py` & `pydbml-1.0.9/pydbml/classes/column.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/enum.py` & `pydbml-1.0.9/pydbml/classes/enum.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/expression.py` & `pydbml-1.0.9/pydbml/classes/expression.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/index.py` & `pydbml-1.0.9/pydbml/classes/index.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/note.py` & `pydbml-1.0.9/pydbml/classes/note.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/project.py` & `pydbml-1.0.9/pydbml/classes/project.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/reference.py` & `pydbml-1.0.9/pydbml/classes/reference.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/table.py` & `pydbml-1.0.9/pydbml/classes/table.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/classes/table_group.py` & `pydbml-1.0.9/pydbml/classes/table_group.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/database.py` & `pydbml-1.0.9/pydbml/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,16 @@
         self.refs.append(obj)
         return obj
 
     def add_enum(self, obj: Enum) -> Enum:
         if obj in self.enums:
             raise DatabaseValidationError(f'{obj} is already in the database.')
         for enum in self.enums:
-            if enum.name == obj.name:
-                raise DatabaseValidationError(f'Enum {obj.name} is already in the database.')
+            if enum.name == obj.name and enum.schema == obj.schema:
+                raise DatabaseValidationError(f'Enum {obj.schema}.{obj.name} is already in the database.')
 
         self._set_database(obj)
         self.enums.append(obj)
         return obj
 
     def add_table_group(self, obj: TableGroup) -> TableGroup:
         if obj in self.table_groups:
```

### Comparing `pydbml-1.0.8/pydbml/definitions/column.py` & `pydbml-1.0.9/pydbml/definitions/column.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/common.py` & `pydbml-1.0.9/pydbml/definitions/common.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/enum.py` & `pydbml-1.0.9/pydbml/definitions/enum.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/generic.py` & `pydbml-1.0.9/pydbml/definitions/generic.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/index.py` & `pydbml-1.0.9/pydbml/definitions/index.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/project.py` & `pydbml-1.0.9/pydbml/definitions/project.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/reference.py` & `pydbml-1.0.9/pydbml/definitions/reference.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/table.py` & `pydbml-1.0.9/pydbml/definitions/table.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/definitions/table_group.py` & `pydbml-1.0.9/pydbml/definitions/table_group.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/parser/blueprints.py` & `pydbml-1.0.9/pydbml/parser/blueprints.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/parser/parser.py` & `pydbml-1.0.9/pydbml/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml/tools.py` & `pydbml-1.0.9/pydbml/tools.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/pydbml.egg-info/PKG-INFO` & `pydbml-1.0.9/pydbml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbml
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python parser and builder for DBML
 Home-page: https://github.com/Vanderhoof/PyDBML
 Author: Daniil Minukhin
 Author-email: ddddsa@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -171,7 +171,9 @@
     "order_id" int
     "product_id" int
     "quantity" int [default: 1]
 }
 ...
 
 ```
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydbml Version: 1.0.8 Summary: Python parser and
+Metadata-Version: 2.1 Name: pydbml Version: 1.0.9 Summary: Python parser and
 builder for DBML Home-page: https://github.com/Vanderhoof/PyDBML Author: Daniil
 Minukhin Author-email: ddddsa@gmail.com License: MIT Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Topic :: Documentation Classifier: Topic :: Text
 Processing :: Markup Classifier: Topic :: Utilities Requires-Python: >=3.8
```

### Comparing `pydbml-1.0.8/pydbml.egg-info/SOURCES.txt` & `pydbml-1.0.9/pydbml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/setup.py` & `pydbml-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='pydbml',
     python_requires='>=3.8',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='1.0.8',
+    version='1.0.9',
     author='Daniil Minukhin',
     author_email='ddddsa@gmail.com',
     url='https://github.com/Vanderhoof/PyDBML',
     packages=['pydbml', 'pydbml.classes', 'pydbml.definitions', 'pydbml.parser'],
     license='MIT',
     platforms='any',
     install_requires=[
```

### Comparing `pydbml-1.0.8/test/test_database.py` & `pydbml-1.0.9/test/test_database.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/test/test_docs.py` & `pydbml-1.0.9/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/test/test_doctest.py` & `pydbml-1.0.9/test/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/test/test_editing.py` & `pydbml-1.0.9/test/test_editing.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/test/test_integration.py` & `pydbml-1.0.9/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.8/test/test_parser.py` & `pydbml-1.0.9/test/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,22 @@
 
         self.assertEqual(rs[1].col1[0].table, posts2)
         self.assertEqual(rs[1].col1, [posts2['id'], posts2['tag']])
         self.assertEqual(rs[1].col2[0].table, reviews2)
         self.assertEqual(rs[1].col2, [reviews2['post_id'], reviews2['tag']])
 
 
+class TestDBMLReferenceDef(TestCase):
+    def test_dbml_reference_def(self):
+        results = PyDBML.parse_file(TEST_DATA_PATH / 'dbml_schema_def.dbml')
+        self.assertEqual(len(results.tables), 5)
+        self.assertEqual(len(results.table_groups), 1)
+        self.assertEqual(len(results.enums), 3)
+
+
 class TestFaulty(TestCase):
     def test_bad_reference(self) -> None:
         with self.assertRaises(TableNotFoundError):
             PyDBML(TEST_DATA_PATH / 'wrong_inline_ref_table.dbml')
         with self.assertRaises(ColumnNotFoundError):
             PyDBML(TEST_DATA_PATH / 'wrong_inline_ref_column.dbml')
```

### Comparing `pydbml-1.0.8/test/test_tools.py` & `pydbml-1.0.9/test/test_tools.py`

 * *Files identical despite different names*

