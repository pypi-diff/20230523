# Comparing `tmp/huhangkai-1.1.4.tar.gz` & `tmp/huhangkai-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.4.tar", last modified: Tue May 16 11:15:23 2023, max compression
+gzip compressed data, was "huhangkai-1.1.5.tar", last modified: Tue May 23 08:46:19 2023, max compression
```

## Comparing `huhangkai-1.1.4.tar` & `huhangkai-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:15:23.026404 huhangkai-1.1.4/
--rw-rw-rw-   0        0        0      228 2023-05-16 11:15:23.025407 huhangkai-1.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 11:15:23.013438 huhangkai-1.1.4/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.4/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/unit_dict.py
--rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.4/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-16 11:14:52.000000 huhangkai-1.1.4/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:15:23.024409 huhangkai-1.1.4/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 11:15:23.026404 huhangkai-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-05-16 11:15:17.000000 huhangkai-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:46:19.553175 huhangkai-1.1.5/
+-rw-rw-rw-   0        0        0      228 2023-05-23 08:46:19.552180 huhangkai-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 08:46:19.540985 huhangkai-1.1.5/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.5/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3475 2023-05-23 08:44:54.000000 huhangkai-1.1.5/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.5/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.5/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-16 11:14:52.000000 huhangkai-1.1.5/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:46:19.550183 huhangkai-1.1.5/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 08:46:19.000000 huhangkai-1.1.5/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:46:19.553175 huhangkai-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-05-23 08:46:16.000000 huhangkai-1.1.5/setup.py
```

### Comparing `huhangkai-1.1.4/commen/__init__.py` & `huhangkai-1.1.5/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/commen/init_project.py` & `huhangkai-1.1.5/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/commen/unit_dict.py` & `huhangkai-1.1.5/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/commen/unit_fun.py` & `huhangkai-1.1.5/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/commen/unit_logger.py` & `huhangkai-1.1.5/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/commen/unit_request.py` & `huhangkai-1.1.5/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/commen/unit_tasks.py` & `huhangkai-1.1.5/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.4/setup.py` & `huhangkai-1.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.1.4',  # 版本号
+    version='1.1.5',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.bat'],},
     python_requires=">=3.0",
     install_requires=[
-        "faker",
-        "requests",
-        "openpyxl",
-        "apscheduler"
+        "faker==15.1.3",
+        "openpyxl==3.0.10",
+        "apscheduler",
+        "rsa==4.9",
+        "pyDes==2.0.1",
+        "pycryptodome==3.17",
     ],
 )
```

