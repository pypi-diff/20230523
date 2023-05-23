# Comparing `tmp/tybase-0.0.9.tar.gz` & `tmp/tybase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.0.9.tar", last modified: Tue May 16 15:44:28 2023, max compression
+gzip compressed data, was "tybase-0.1.0.tar", last modified: Tue May 23 07:01:44 2023, max compression
```

## Comparing `tybase-0.0.9.tar` & `tybase-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-16 15:44:28.407657 tybase-0.0.9/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.0.9/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      584 2023-05-16 15:44:28.407374 tybase-0.0.9/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.0.9/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-16 15:44:28.407810 tybase-0.0.9/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)      920 2023-05-16 15:42:53.000000 tybase-0.0.9/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-16 15:44:28.400823 tybase-0.0.9/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.0.9/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-16 15:44:28.403457 tybase-0.0.9/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.0.9/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.0.9/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.0.9/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-16 15:44:28.405148 tybase-0.0.9/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.0.9/tybase/dbtool/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)     9446 2023-05-16 15:43:22.000000 tybase-0.0.9/tybase/dbtool/data_import.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2206 2023-05-13 03:56:34.000000 tybase-0.0.9/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-16 15:44:28.406509 tybase-0.0.9/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.0.9/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.0.9/tybase/lc/eg1.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.0.9/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-16 15:44:28.402916 tybase-0.0.9/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      584 2023-05-16 15:44:28.000000 tybase-0.0.9/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      401 2023-05-16 15:44:28.000000 tybase-0.0.9/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-05-16 15:44:28.000000 tybase-0.0.9/tybase.egg-info/dependency_links.txt
--rw-r--r--   0 zhangte    (501) staff       (20)       86 2023-05-16 15:44:28.000000 tybase-0.0.9/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-05-16 15:44:28.000000 tybase-0.0.9/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-23 07:01:43.914626 tybase-0.1.0/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.1.0/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      619 2023-05-23 07:01:43.914339 tybase-0.1.0/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.1.0/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-05-23 07:01:43.914740 tybase-0.1.0/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      919 2023-05-23 07:00:58.000000 tybase-0.1.0/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-23 07:01:43.810970 tybase-0.1.0/tybase/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.1.0/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-23 07:01:43.821627 tybase-0.1.0/tybase/baidu/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.1.0/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.1.0/tybase/baidu/kw_tool.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.1.0/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-23 07:01:43.860559 tybase-0.1.0/tybase/dbtool/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.1.0/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9444 2023-05-23 07:00:41.000000 tybase-0.1.0/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2206 2023-05-13 03:56:34.000000 tybase-0.1.0/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-23 07:01:43.877798 tybase-0.1.0/tybase/lc/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.1.0/tybase/lc/__init__.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.1.0/tybase/lc/eg1.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.1.0/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-05-23 07:01:43.820976 tybase-0.1.0/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      619 2023-05-23 07:01:42.000000 tybase-0.1.0/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      401 2023-05-23 07:01:43.000000 tybase-0.1.0/tybase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-05-23 07:01:42.000000 tybase-0.1.0/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       86 2023-05-23 07:01:43.000000 tybase-0.1.0/tybase.egg-info/requires.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-05-23 07:01:43.000000 tybase-0.1.0/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.0.9/PKG-INFO` & `tybase-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.0.9
-Summary: 简单优化了一下导入的方法
+Version: 0.1.0
+Summary: 修复了mysql重复导入的问题
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 ### 新增百度的关键词汇总
 位置 : baidu.kw_tools.py
 1. KeywordSummary
 2. KeywordAggregator
 
 ### Langchain相关工具的封装
 1. eg1-生成prompt
+
```

### Comparing `tybase-0.0.9/setup.py` & `tybase-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.0.9',
+    version='0.1.0',
     include_package_data=True,
-    description='简单优化了一下导入的方法',
+    description='修复了mysql重复导入的问题',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.0.9/tybase/baidu/kw_tool.py` & `tybase-0.1.0/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.0.9/tybase/dbtool/data_import.py` & `tybase-0.1.0/tybase/dbtool/data_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sqlalchemy.inspection import inspect
 import pandas as pd
 import os
 import glob
 from pandas import read_excel
 import shutil
 
-import tybase
+
 
 class DataFrameProcessor:
     """
     DataFrameProcessor 类设计用于根据特定规则处理 CSV 文件中的数据。
 
     属性:
         config_df: 一个 pandas DataFrame 对象，用于存储配置数据。
@@ -167,16 +167,16 @@
                         if result.rowcount > 0:
                             del_stmt = text(f"DELETE FROM {table_name} WHERE {where_condition}")
                             connection.execute(del_stmt)
                     trans.commit()  # 提交事务
                 except:
                     trans.rollback()  # 如果发生错误，则回滚事务
                     raise
-
-        df.to_sql(table_name, self.engine, if_exists='append', index=False)
+        #
+        # df.to_sql(table_name, self.engine, if_exists='append', index=False)
 
 
 class DirectoryProcessor:
     """
     # 使用方式：
         # 导入配置文件
         #configh.csv的字段:
```

### Comparing `tybase-0.0.9/tybase/dbtool/mysql.py` & `tybase-0.1.0/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.0.9/tybase/lc/eg1.py` & `tybase-0.1.0/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.0.9/tybase.egg-info/PKG-INFO` & `tybase-0.1.0/tybase.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.0.9
-Summary: 简单优化了一下导入的方法
+Version: 0.1.0
+Summary: 修复了mysql重复导入的问题
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 ### 新增百度的关键词汇总
 位置 : baidu.kw_tools.py
 1. KeywordSummary
 2. KeywordAggregator
 
 ### Langchain相关工具的封装
 1. eg1-生成prompt
+
```

