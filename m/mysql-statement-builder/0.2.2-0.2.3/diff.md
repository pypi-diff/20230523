# Comparing `tmp/mysql-statement-builder-0.2.2.tar.gz` & `tmp/mysql-statement-builder-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-statement-builder-0.2.2.tar", last modified: Tue May 23 10:35:18 2023, max compression
+gzip compressed data, was "mysql-statement-builder-0.2.3.tar", last modified: Tue May 23 10:41:27 2023, max compression
```

## Comparing `mysql-statement-builder-0.2.2.tar` & `mysql-statement-builder-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.553022 mysql-statement-builder-0.2.2/
--rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     2107 2023-05-23 10:35:18.549021 mysql-statement-builder-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1502 2023-05-23 08:59:39.000000 mysql-statement-builder-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.347226 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.488369 mysql-statement-builder-0.2.2/mysqlsb/
--rw-rw-rw-   0        0        0      156 2023-05-23 10:30:17.000000 mysql-statement-builder-0.2.2/mysqlsb/__init__.py
--rw-rw-rw-   0        0        0     7560 2023-05-23 09:07:28.000000 mysql-statement-builder-0.2.2/mysqlsb/builder.py
--rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.2.2/mysqlsb/configuration.py
--rw-rw-rw-   0        0        0       59 2023-05-22 15:16:44.000000 mysql-statement-builder-0.2.2/mysqlsb/exceptions.py
--rw-rw-rw-   0        0        0     2259 2023-05-23 08:48:54.000000 mysql-statement-builder-0.2.2/mysqlsb/statements.py
--rw-rw-rw-   0        0        0      612 2021-12-08 13:05:41.000000 mysql-statement-builder-0.2.2/mysqlsb/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-23 10:35:18.557061 mysql-statement-builder-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      949 2023-05-23 10:35:07.000000 mysql-statement-builder-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.536379 mysql-statement-builder-0.2.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.2.2/tests/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-23 08:55:28.000000 mysql-statement-builder-0.2.2/tests/test_builder.py
--rw-rw-rw-   0        0        0      506 2023-05-23 08:49:25.000000 mysql-statement-builder-0.2.2/tests/test_statements.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.212502 mysql-statement-builder-0.2.3/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-05-23 10:41:27.212502 mysql-statement-builder-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-23 10:36:35.000000 mysql-statement-builder-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.195504 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 10:41:27.000000 mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.205496 mysql-statement-builder-0.2.3/mysqlsb/
+-rw-rw-rw-   0        0        0      188 2023-05-23 10:41:12.000000 mysql-statement-builder-0.2.3/mysqlsb/__init__.py
+-rw-rw-rw-   0        0        0     7560 2023-05-23 09:07:28.000000 mysql-statement-builder-0.2.3/mysqlsb/builder.py
+-rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.2.3/mysqlsb/configuration.py
+-rw-rw-rw-   0        0        0       59 2023-05-22 15:16:44.000000 mysql-statement-builder-0.2.3/mysqlsb/exceptions.py
+-rw-rw-rw-   0        0        0     2259 2023-05-23 08:48:54.000000 mysql-statement-builder-0.2.3/mysqlsb/statements.py
+-rw-rw-rw-   0        0        0      612 2021-12-08 13:05:41.000000 mysql-statement-builder-0.2.3/mysqlsb/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 10:41:27.213504 mysql-statement-builder-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-05-23 10:41:17.000000 mysql-statement-builder-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:41:27.210493 mysql-statement-builder-0.2.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.2.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-23 08:55:28.000000 mysql-statement-builder-0.2.3/tests/test_builder.py
+-rw-rw-rw-   0        0        0      506 2023-05-23 08:49:25.000000 mysql-statement-builder-0.2.3/tests/test_statements.py
```

### Comparing `mysql-statement-builder-0.2.2/LICENSE` & `mysql-statement-builder-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.2/PKG-INFO` & `mysql-statement-builder-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MySQL-statement-builder (mysqlsb)
 ...
 
+## Installation
+```pip install mysql-statement-builder```
+
 ## Usage
 ```
 import mysql.connector
 from mysql.connector import pooling
 from contextlib import contextmanager
 
 from mysqlsb import MySQLStatementBuilder, FetchType
```

### Comparing `mysql-statement-builder-0.2.2/README.md` & `mysql-statement-builder-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # MySQL-statement-builder (mysqlsb)
 ...
 
+## Installation
+```pip install mysql-statement-builder```
+
 ## Usage
 ```
 import mysql.connector
 from mysql.connector import pooling
 from contextlib import contextmanager
 
 from mysqlsb import MySQLStatementBuilder, FetchType
```

### Comparing `mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/PKG-INFO` & `mysql-statement-builder-0.2.3/mysql_statement_builder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MySQL-statement-builder (mysqlsb)
 ...
 
+## Installation
+```pip install mysql-statement-builder```
+
 ## Usage
 ```
 import mysql.connector
 from mysql.connector import pooling
 from contextlib import contextmanager
 
 from mysqlsb import MySQLStatementBuilder, FetchType
```

### Comparing `mysql-statement-builder-0.2.2/mysqlsb/builder.py` & `mysql-statement-builder-0.2.3/mysqlsb/builder.py`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.2/mysqlsb/statements.py` & `mysql-statement-builder-0.2.3/mysqlsb/statements.py`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.2/mysqlsb/utils.py` & `mysql-statement-builder-0.2.3/mysqlsb/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.2/setup.py` & `mysql-statement-builder-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'Simplifies writing MySQL statements in non-ORM environments.'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='mysql-statement-builder',
```

