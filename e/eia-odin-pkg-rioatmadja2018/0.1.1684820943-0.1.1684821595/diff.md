# Comparing `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684820943.tar.gz` & `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684821595.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684820943.tar", last modified: Tue May 23 05:49:04 2023, max compression
+gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684821595.tar", last modified: Tue May 23 05:59:55 2023, max compression
```

## Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943.tar` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.122053 eia-odin-pkg-rioatmadja2018-0.1.1684820943/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 05:49:04.122053 eia-odin-pkg-rioatmadja2018-0.1.1684820943/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.114054 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.114054 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/production.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.118054 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/db/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/db/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     9691 2023-05-23 05:47:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/db/odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.122053 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/aws_resources.py
--rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/browser.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5888 2023-05-22 06:33:23.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/constants.py
--rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/credentials.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/facets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/tools.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.122053 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 05:49:04.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)      780 2023-05-23 05:49:04.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 05:49:04.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-23 05:49:04.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       11 2023-05-23 05:49:04.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 05:49:00.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:49:04.122053 eia-odin-pkg-rioatmadja2018-0.1.1684820943/images/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/images/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 05:49:04.122053 eia-odin-pkg-rioatmadja2018-0.1.1684820943/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)     1613 2023-05-23 01:43:18.000000 eia-odin-pkg-rioatmadja2018-0.1.1684820943/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.251615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 05:59:55.251615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.247615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.247615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/production.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/stocks.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.247615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/db/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/db/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     9777 2023-05-23 05:59:34.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/db/odin_db.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.251615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/aws_resources.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/browser.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5888 2023-05-22 06:33:23.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/constants.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/credentials.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/facets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/tools.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.251615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 05:59:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      780 2023-05-23 05:59:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 05:59:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-23 05:59:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       11 2023-05-23 05:59:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 05:59:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 05:59:55.251615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/images/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/images/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 05:59:55.251615 eia-odin-pkg-rioatmadja2018-0.1.1684821595/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)     1613 2023-05-23 01:43:18.000000 eia-odin-pkg-rioatmadja2018-0.1.1684821595/setup.py
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684820943
+Version: 0.1.1684821595
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/README.md` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/README.md`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/consumption_sales.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/consumption_sales.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/movements.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/movements.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/production.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/production.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/crude_oil/stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/crude_oil/stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/db/odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/db/odin_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                 l.timestamp,
                 l.price,
                 l.review,
                 l.review_date,
                 l.sentiment_score
 
             FROM live_gasoline_prices l
-            WHERE l.state = '{dst_state}'
+            WHERE l.state = '{dst_state}' AND SUBSTRING_INDEX(l.timestamp, 'T', 1) = '{datetime.utcnow().strftime('%Y-%m-%d')}'
         """
         try:
             conn: 'MySQL' = pymysql.connect(host=os.environ["MYSQL_HOST"],
                                             user=os.environ["MYSQL_USER"],
                                             password=os.environ["MYSQL_PASSWD"],
                                             database=os.environ["MYSQL_DB"])
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/aws_resources.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/aws_resources.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/browser.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/browser.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/constants.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/constants.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/facets.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/facets.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia/utils/tools.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684820943
+Version: 0.1.1684821595
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684820943/setup.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684821595/setup.py`

 * *Files identical despite different names*

