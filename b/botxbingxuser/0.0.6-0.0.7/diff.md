# Comparing `tmp/botxbingxuser-0.0.6.tar.gz` & `tmp/botxbingxuser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botxbingxuser-0.0.6.tar", last modified: Wed May 17 17:40:31 2023, max compression
+gzip compressed data, was "botxbingxuser-0.0.7.tar", last modified: Tue May 23 18:04:30 2023, max compression
```

## Comparing `botxbingxuser-0.0.6.tar` & `botxbingxuser-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:40:31.560840 botxbingxuser-0.0.6/
--rw-rw-rw-   0        0        0      566 2023-05-17 17:40:31.559839 botxbingxuser-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 17:40:31.552832 botxbingxuser-0.0.6/botxbingxuser.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 17:40:31.557838 botxbingxuser-0.0.6/botxbinxuser/
--rw-rw-rw-   0        0        0     6630 2023-05-17 17:07:47.000000 botxbingxuser-0.0.6/botxbinxuser/PrincipalMetodos.py
--rw-rw-rw-   0        0        0        0 2023-05-17 15:51:27.000000 botxbingxuser-0.0.6/botxbinxuser/__init__.py
--rw-rw-rw-   0        0        0     4021 2023-05-17 17:07:33.000000 botxbingxuser-0.0.6/botxbinxuser/symbols.py
--rw-rw-rw-   0        0        0       42 2023-05-17 17:40:31.560840 botxbingxuser-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-05-17 17:39:52.000000 botxbingxuser-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:04:30.846798 botxbingxuser-0.0.7/
+-rw-rw-rw-   0        0        0      566 2023-05-23 18:04:30.845798 botxbingxuser-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 18:04:30.819776 botxbingxuser-0.0.7/botxbingxuser.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-23 18:04:29.000000 botxbingxuser-0.0.7/botxbingxuser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-23 18:04:30.000000 botxbingxuser-0.0.7/botxbingxuser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 18:04:29.000000 botxbingxuser-0.0.7/botxbingxuser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 18:04:29.000000 botxbingxuser-0.0.7/botxbingxuser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 18:04:30.844797 botxbingxuser-0.0.7/botxbinxuser/
+-rw-rw-rw-   0        0        0    20504 2023-05-23 18:00:44.000000 botxbingxuser-0.0.7/botxbinxuser/PrincipalMetodos.py
+-rw-rw-rw-   0        0        0        0 2023-05-17 15:51:27.000000 botxbingxuser-0.0.7/botxbinxuser/__init__.py
+-rw-rw-rw-   0        0        0     2140 2023-05-22 19:08:12.000000 botxbingxuser-0.0.7/botxbinxuser/responses.py
+-rw-rw-rw-   0        0        0     4021 2023-05-17 17:07:33.000000 botxbingxuser-0.0.7/botxbinxuser/symbols.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 18:04:30.846798 botxbingxuser-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2023-05-23 18:04:22.000000 botxbingxuser-0.0.7/setup.py
```

### Comparing `botxbingxuser-0.0.6/PKG-INFO` & `botxbingxuser-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.6
+Version: 0.0.7
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.6/botxbingxuser.egg-info/PKG-INFO` & `botxbingxuser-0.0.7/botxbingxuser.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.6
+Version: 0.0.7
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.6/botxbinxuser/symbols.py` & `botxbingxuser-0.0.7/botxbinxuser/symbols.py`

 * *Files identical despite different names*

### Comparing `botxbingxuser-0.0.6/setup.py` & `botxbingxuser-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'API de acesso a Xbinx'
 LONG_DESCRIPTION = """ API de acesso a corretora XBINGX
                         Para automatizar os traders"""
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
```

