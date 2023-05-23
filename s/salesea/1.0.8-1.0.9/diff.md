# Comparing `tmp/salesea-1.0.8.tar.gz` & `tmp/salesea-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.8.tar", last modified: Mon May 22 05:45:23 2023, max compression
+gzip compressed data, was "salesea-1.0.9.tar", last modified: Tue May 23 07:38:20 2023, max compression
```

## Comparing `salesea-1.0.8.tar` & `salesea-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.385628 salesea-1.0.8/
--rw-rw-rw-   0        0        0     2319 2023-05-22 05:45:23.385628 salesea-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1345 2023-05-22 05:39:22.000000 salesea-1.0.8/README.md
--rw-rw-rw-   0        0        0      111 2023-05-22 05:45:23.386628 salesea-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2298 2023-05-22 03:40:12.000000 salesea-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.368629 salesea-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.378628 salesea-1.0.8/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.8/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.8/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7110 2023-05-22 05:38:19.000000 salesea-1.0.8/src/salesea/app.py
--rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.8/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.8/src/salesea/log.py
--rw-rw-rw-   0        0        0     7716 2023-05-22 03:01:08.000000 salesea-1.0.8/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.8/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.8/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 05:45:23.384628 salesea-1.0.8/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2319 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 05:45:23.000000 salesea-1.0.8/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.782057 salesea-1.0.9/
+-rw-rw-rw-   0        0        0     2587 2023-05-23 07:38:20.782057 salesea-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.9/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-23 07:38:20.783057 salesea-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2298 2023-05-23 07:16:05.000000 salesea-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.757001 salesea-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.775057 salesea-1.0.9/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.9/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.9/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7119 2023-05-23 07:18:06.000000 salesea-1.0.9/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.9/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.9/src/salesea/log.py
+-rw-rw-rw-   0        0        0     7716 2023-05-22 03:01:08.000000 salesea-1.0.9/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.9/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.9/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.781057 salesea-1.0.9/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2587 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.8/PKG-INFO` & `salesea-1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.8
+Version: 1.0.9
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
@@ -24,14 +24,18 @@
 
 # salesea@nginx-log-parser
 
 ## 开始使用
 
 > 网络姻缘一线牵 珍惜这段缘
 
+[![salesea](https://img.shields.io/pypi/v/salesea)](https://pypi.org/project/salesea/)
+[![salesea](https://img.shields.io/pypi/dd/salesea)](https://pypi.org/project/salesea/#files)
+[![salesea](https://img.shields.io/pypi/wheel/salesea)](https://pypi.org/project/salesea/)
+
 ### Nginx要求
 
 - Nginx http配置：
   > 日志格式
 
   ```nginx
   log_format salesea '$remote_addr - $remote_user [$time_local] "$request" '
@@ -45,15 +49,15 @@
     access_log /to/path/access.log salesea;
   ```
 
 ### Python要求
 
 - Python版本：3.6+
 
-- [conf.ini](conf.ini)配置文件
+- salesea.ini配置文件
 
   ```ini
   [nginx]
   server_name = 需要采集的nginx server_name，可以使用*通配符
   nginx_path = 如果你配置了环境变量，可以为空
   [request]
   concurrency = 上传日志并发数
```

### Comparing `salesea-1.0.8/setup.py` & `salesea-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
```

### Comparing `salesea-1.0.8/src/salesea/__main__.py` & `salesea-1.0.9/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.8/src/salesea/app.py` & `salesea-1.0.9/src/salesea/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from .nginx import Nginx, NginxException
 from .log import logger
 from .solution import print_solution
 
 
 def launch():
     # 将PID写入文件
-    pid = os.getpid()
-    with open("salesea.pid", "w") as f:
-        f.write(str(pid))
+    # pid = os.getpid()
+    # with open("salesea.pid", "w") as f:sys
+    #     f.write(str(pid))
     #############################################################################
     #####Global Variable#########################################################
     datetime_format = "%Y-%m-%d %H:%M:%S %z"  # 时间格式
     nginx = None
 
     #############################################################################
     #####Get Access Servers######################################################
```

### Comparing `salesea-1.0.8/src/salesea/config.py` & `salesea-1.0.9/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.8/src/salesea/log.py` & `salesea-1.0.9/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.8/src/salesea/nginx.py` & `salesea-1.0.9/src/salesea/nginx.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.8/src/salesea/solution.py` & `salesea-1.0.9/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.8/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.9/src/salesea.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.8
+Version: 1.0.9
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
@@ -24,14 +24,18 @@
 
 # salesea@nginx-log-parser
 
 ## 开始使用
 
 > 网络姻缘一线牵 珍惜这段缘
 
+[![salesea](https://img.shields.io/pypi/v/salesea)](https://pypi.org/project/salesea/)
+[![salesea](https://img.shields.io/pypi/dd/salesea)](https://pypi.org/project/salesea/#files)
+[![salesea](https://img.shields.io/pypi/wheel/salesea)](https://pypi.org/project/salesea/)
+
 ### Nginx要求
 
 - Nginx http配置：
   > 日志格式
 
   ```nginx
   log_format salesea '$remote_addr - $remote_user [$time_local] "$request" '
@@ -45,15 +49,15 @@
     access_log /to/path/access.log salesea;
   ```
 
 ### Python要求
 
 - Python版本：3.6+
 
-- [conf.ini](conf.ini)配置文件
+- salesea.ini配置文件
 
   ```ini
   [nginx]
   server_name = 需要采集的nginx server_name，可以使用*通配符
   nginx_path = 如果你配置了环境变量，可以为空
   [request]
   concurrency = 上传日志并发数
```

