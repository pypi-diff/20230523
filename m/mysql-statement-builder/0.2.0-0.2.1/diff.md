# Comparing `tmp/mysql_statement_builder-0.2.0-py3-none-any.whl.zip` & `tmp/mysql_statement_builder-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2828 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1101 b- defN 23-May-23 08:57 mysql_statement_builder-0.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2038 b- defN 23-May-23 08:57 mysql_statement_builder-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 08:57 mysql_statement_builder-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-23 08:57 mysql_statement_builder-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      465 b- defN 23-May-23 08:57 mysql_statement_builder-0.2.0.dist-info/RECORD
-5 files, 3704 bytes uncompressed, 1948 bytes compressed:  47.4%
+Zip file size: 2810 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1101 b- defN 23-May-23 09:00 mysql_statement_builder-0.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2019 b- defN 23-May-23 09:00 mysql_statement_builder-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 09:00 mysql_statement_builder-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-23 09:00 mysql_statement_builder-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      465 b- defN 23-May-23 09:00 mysql_statement_builder-0.2.1.dist-info/RECORD
+5 files, 3685 bytes uncompressed, 1930 bytes compressed:  47.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: mysql_statement_builder-0.2.0.dist-info/LICENSE
+Filename: mysql_statement_builder-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: mysql_statement_builder-0.2.0.dist-info/METADATA
+Filename: mysql_statement_builder-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: mysql_statement_builder-0.2.0.dist-info/WHEEL
+Filename: mysql_statement_builder-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: mysql_statement_builder-0.2.0.dist-info/top_level.txt
+Filename: mysql_statement_builder-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mysql_statement_builder-0.2.0.dist-info/RECORD
+Filename: mysql_statement_builder-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mysql_statement_builder-0.2.0.dist-info/LICENSE` & `mysql_statement_builder-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mysql_statement_builder-0.2.0.dist-info/METADATA` & `mysql_statement_builder-0.2.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-statement-builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simplifies writing MySQL statements in non-ORM environments.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 
 ## Usage
 ```
 import mysql.connector
 from mysql.connector import pooling
 from contextlib import contextmanager
 
-from sedbackend.libs.mysqlutils import MySQLStatementBuilder, FetchType
+from mysqlsb import MySQLStatementBuilder, FetchType
 
 # Setup a connection pool using the MySQL python connector
 connection_pool = mysql.connector.pooling.MySQLConnectionPool(
     user='user',
     password='password',
     host='host',
     database='database',
```

