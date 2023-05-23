# Comparing `tmp/mysql-statement-builder-0.2.1.tar.gz` & `tmp/mysql-statement-builder-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-statement-builder-0.2.1.tar", last modified: Tue May 23 09:31:20 2023, max compression
+gzip compressed data, was "mysql-statement-builder-0.2.2.tar", last modified: Tue May 23 10:35:18 2023, max compression
```

## Comparing `mysql-statement-builder-0.2.1.tar` & `mysql-statement-builder-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:31:20.281899 mysql-statement-builder-0.2.1/
--rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2107 2023-05-23 09:31:20.280580 mysql-statement-builder-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1502 2023-05-23 08:59:39.000000 mysql-statement-builder-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 09:31:20.201873 mysql-statement-builder-0.2.1/mysqlsb/
-drwxrwxrwx   0        0        0        0 2023-05-23 09:31:20.273876 mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-05-23 09:31:19.000000 mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-23 09:31:20.000000 mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:31:19.000000 mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-23 09:31:19.000000 mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 09:31:19.000000 mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 09:31:20.282875 mysql-statement-builder-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      892 2023-05-23 09:30:53.000000 mysql-statement-builder-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.553022 mysql-statement-builder-0.2.2/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 08:20:23.000000 mysql-statement-builder-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2107 2023-05-23 10:35:18.549021 mysql-statement-builder-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1502 2023-05-23 08:59:39.000000 mysql-statement-builder-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.347226 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 10:35:17.000000 mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.488369 mysql-statement-builder-0.2.2/mysqlsb/
+-rw-rw-rw-   0        0        0      156 2023-05-23 10:30:17.000000 mysql-statement-builder-0.2.2/mysqlsb/__init__.py
+-rw-rw-rw-   0        0        0     7560 2023-05-23 09:07:28.000000 mysql-statement-builder-0.2.2/mysqlsb/builder.py
+-rw-rw-rw-   0        0        0      219 2023-05-23 07:45:37.000000 mysql-statement-builder-0.2.2/mysqlsb/configuration.py
+-rw-rw-rw-   0        0        0       59 2023-05-22 15:16:44.000000 mysql-statement-builder-0.2.2/mysqlsb/exceptions.py
+-rw-rw-rw-   0        0        0     2259 2023-05-23 08:48:54.000000 mysql-statement-builder-0.2.2/mysqlsb/statements.py
+-rw-rw-rw-   0        0        0      612 2021-12-08 13:05:41.000000 mysql-statement-builder-0.2.2/mysqlsb/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 10:35:18.557061 mysql-statement-builder-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-05-23 10:35:07.000000 mysql-statement-builder-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:35:18.536379 mysql-statement-builder-0.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 07:33:30.000000 mysql-statement-builder-0.2.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-23 08:55:28.000000 mysql-statement-builder-0.2.2/tests/test_builder.py
+-rw-rw-rw-   0        0        0      506 2023-05-23 08:49:25.000000 mysql-statement-builder-0.2.2/tests/test_statements.py
```

### Comparing `mysql-statement-builder-0.2.1/LICENSE` & `mysql-statement-builder-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.1/PKG-INFO` & `mysql-statement-builder-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mysql-statement-builder-0.2.1/README.md` & `mysql-statement-builder-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mysql-statement-builder-0.2.1/mysqlsb/mysql_statement_builder.egg-info/PKG-INFO` & `mysql-statement-builder-0.2.2/mysql_statement_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: https://github.com/johnmartins/mysql-statement-builder
 Author: Julian Martinsson Bonde
 Author-email: julianm@chalmers.se
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mysql-statement-builder-0.2.1/setup.py` & `mysql-statement-builder-0.2.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-from setuptools import setup
+from setuptools import setup, find_packages
+
+VERSION = '0.2.2'
+DESCRIPTION = 'Simplifies writing MySQL statements in non-ORM environments.'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='mysql-statement-builder',
-    version='0.2.1',
-    description='Simplifies writing MySQL statements in non-ORM environments.',
-    py_modules=["mysqlsb"],
-    package_dir={'': 'mysqlsb'},
+    version=VERSION,
+    description=DESCRIPTION,
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License"
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
+    install_requires=[],
     extras_require={
         "dev": [
-            "pytest>=7.3",
+            "pytest==7.*",
             "twine>=4.0"
         ]
     },
     url="https://github.com/johnmartins/mysql-statement-builder",
     author="Julian Martinsson Bonde",
     author_email="julianm@chalmers.se"
 )
```

