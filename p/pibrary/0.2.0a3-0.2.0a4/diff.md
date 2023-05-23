# Comparing `tmp/pibrary-0.2.0a3.tar.gz` & `tmp/pibrary-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibrary-0.2.0a3.tar", max compression
+gzip compressed data, was "pibrary-0.2.0a4.tar", max compression
```

## Comparing `pibrary-0.2.0a3.tar` & `pibrary-0.2.0a4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-05-15 09:17:40.380475 pibrary-0.2.0a3/LICENSE
--rw-r--r--   0        0        0     2054 2023-05-15 09:17:40.380475 pibrary-0.2.0a3/README.md
--rw-r--r--   0        0        0        0 2023-05-15 09:17:40.384475 pibrary-0.2.0a3/pibrary/__init__.py
--rw-r--r--   0        0        0     4446 2023-05-15 09:17:40.384475 pibrary-0.2.0a3/pibrary/file.py
--rw-r--r--   0        0        0      939 2023-05-15 09:17:40.384475 pibrary-0.2.0a3/pibrary/logger.py
--rw-r--r--   0        0        0     1435 2023-05-15 09:17:40.384475 pibrary-0.2.0a3/pibrary/string.py
--rw-r--r--   0        0        0      487 2023-05-15 09:17:40.384475 pibrary-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 pibrary-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-08 15:05:56.342612 pibrary-0.2.0a4/LICENSE
+-rw-r--r--   0        0        0     2053 2023-05-23 16:06:08.329944 pibrary-0.2.0a4/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 08:01:06.111923 pibrary-0.2.0a4/pibrary/__init__.py
+-rw-r--r--   0        0        0     4446 2023-05-12 02:16:45.133836 pibrary-0.2.0a4/pibrary/file.py
+-rw-r--r--   0        0        0      939 2023-05-08 15:05:56.343483 pibrary-0.2.0a4/pibrary/logger.py
+-rw-r--r--   0        0        0     1435 2023-05-14 14:59:23.553176 pibrary-0.2.0a4/pibrary/string.py
+-rw-r--r--   0        0        0      486 2023-05-23 16:06:15.222301 pibrary-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2724 1970-01-01 00:00:00.000000 pibrary-0.2.0a4/PKG-INFO
```

### Comparing `pibrary-0.2.0a3/LICENSE` & `pibrary-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a3/README.md` & `pibrary-0.2.0a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 # String Class
 new_text = String(text).lower().remove_digits().remove_punctuation().strip()
 ```
 
 ## Documentation
 
-The full documentation for Pibrary is available at https://pibrary.readthedocs.io/en/latest/.
+The full documentation of Pibrary is available at https://pibrary.readthedocs.io/en/latest/.
 
 ## Contributing
 Contributions are welcome! Please read [CONTRIBUTING](CONTRIBUTING) for details on how to contribute to this project.
 
 
 # License
 This project is licensed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -6,11 +6,11 @@
 pibrary.file import File from pibrary.logger import timeit from pibrary.string
 import String # File Class dataframe = File(file_path).read().csv() File
 (file_path).write(dataframe).csv() json_data = File(file_path).read().json()
 File(file_path).write(json_data).csv() pickle_data = File(file_path).read
 ().pickle() File(file_path).write(pickle_data).csv() # Logger @timeit def
 some_function(...): ... # String Class new_text = String(text).lower
 ().remove_digits().remove_punctuation().strip() ``` ## Documentation The full
-documentation for Pibrary is available at https://pibrary.readthedocs.io/en/
+documentation of Pibrary is available at https://pibrary.readthedocs.io/en/
 latest/. ## Contributing Contributions are welcome! Please read [CONTRIBUTING]
 (CONTRIBUTING) for details on how to contribute to this project. # License This
 project is licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `pibrary-0.2.0a3/pibrary/file.py` & `pibrary-0.2.0a4/pibrary/file.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a3/pibrary/logger.py` & `pibrary-0.2.0a4/pibrary/logger.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a3/pibrary/string.py` & `pibrary-0.2.0a4/pibrary/string.py`

 * *Files identical despite different names*

### Comparing `pibrary-0.2.0a3/PKG-INFO` & `pibrary-0.2.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pibrary
-Version: 0.2.0a3
-Summary: A package for reusable code for ML projects.
+Version: 0.2.0a4
+Summary: A package of reusable code for ML projects.
 License: MIT
 Author: Prakash Chaudhary
 Author-email: connectwithprakash@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -69,15 +69,15 @@
 
 # String Class
 new_text = String(text).lower().remove_digits().remove_punctuation().strip()
 ```
 
 ## Documentation
 
-The full documentation for Pibrary is available at https://pibrary.readthedocs.io/en/latest/.
+The full documentation of Pibrary is available at https://pibrary.readthedocs.io/en/latest/.
 
 ## Contributing
 Contributions are welcome! Please read [CONTRIBUTING](CONTRIBUTING) for details on how to contribute to this project.
 
 
 # License
 This project is licensed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pibrary Version: 0.2.0a3 Summary: A package for
+Metadata-Version: 2.1 Name: pibrary Version: 0.2.0a4 Summary: A package of
 reusable code for ML projects. License: MIT Author: Prakash Chaudhary Author-
 email: connectwithprakash@gmail.com Requires-Python: >=3.8 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: joblib
 (>=1.2.0,<2.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: pandas
@@ -14,11 +14,11 @@
 pibrary.file import File from pibrary.logger import timeit from pibrary.string
 import String # File Class dataframe = File(file_path).read().csv() File
 (file_path).write(dataframe).csv() json_data = File(file_path).read().json()
 File(file_path).write(json_data).csv() pickle_data = File(file_path).read
 ().pickle() File(file_path).write(pickle_data).csv() # Logger @timeit def
 some_function(...): ... # String Class new_text = String(text).lower
 ().remove_digits().remove_punctuation().strip() ``` ## Documentation The full
-documentation for Pibrary is available at https://pibrary.readthedocs.io/en/
+documentation of Pibrary is available at https://pibrary.readthedocs.io/en/
 latest/. ## Contributing Contributions are welcome! Please read [CONTRIBUTING]
 (CONTRIBUTING) for details on how to contribute to this project. # License This
 project is licensed under the terms of the [MIT license](LICENSE).
```

