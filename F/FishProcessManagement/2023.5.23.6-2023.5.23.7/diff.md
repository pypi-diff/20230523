# Comparing `tmp/FishProcessManagement-2023.5.23.6.tar.gz` & `tmp/FishProcessManagement-2023.5.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FishProcessManagement-2023.5.23.6.tar", last modified: Tue May 23 10:06:30 2023, max compression
+gzip compressed data, was "FishProcessManagement-2023.5.23.7.tar", last modified: Tue May 23 10:17:39 2023, max compression
```

## Comparing `FishProcessManagement-2023.5.23.6.tar` & `FishProcessManagement-2023.5.23.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:06:30.016332 FishProcessManagement-2023.5.23.6/
-drwxrwxrwx   0        0        0        0 2023-05-23 10:06:29.997190 FishProcessManagement-2023.5.23.6/FishProcessManagement/
--rw-rw-rw-   0        0        0     2655 2023-05-23 10:05:30.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement/__init__.py
--rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement/child.py
--rw-rw-rw-   0        0        0      214 2023-05-23 08:39:06.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement/test.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:06:30.012338 FishProcessManagement-2023.5.23.6/FishProcessManagement.egg-info/
--rw-rw-rw-   0        0        0     1734 2023-05-23 10:06:29.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-23 10:06:29.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:06:29.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-23 10:06:29.000000 FishProcessManagement-2023.5.23.6/FishProcessManagement.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1734 2023-05-23 10:06:30.014336 FishProcessManagement-2023.5.23.6/PKG-INFO
--rw-rw-rw-   0        0        0     1321 2023-05-23 09:59:04.000000 FishProcessManagement-2023.5.23.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 10:06:30.016332 FishProcessManagement-2023.5.23.6/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-05-23 10:06:04.000000 FishProcessManagement-2023.5.23.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:17:39.290035 FishProcessManagement-2023.5.23.7/
+drwxrwxrwx   0        0        0        0 2023-05-23 10:17:39.274379 FishProcessManagement-2023.5.23.7/FishProcessManagement/
+-rw-rw-rw-   0        0        0     2645 2023-05-23 10:11:14.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement/child.py
+-rw-rw-rw-   0        0        0      204 2023-05-23 10:13:05.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement/test.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:17:39.285032 FishProcessManagement-2023.5.23.7/FishProcessManagement.egg-info/
+-rw-rw-rw-   0        0        0     1820 2023-05-23 10:17:39.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-23 10:17:39.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:17:39.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-23 10:17:39.000000 FishProcessManagement-2023.5.23.7/FishProcessManagement.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1820 2023-05-23 10:17:39.288030 FishProcessManagement-2023.5.23.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1407 2023-05-23 10:15:11.000000 FishProcessManagement-2023.5.23.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 10:17:39.290035 FishProcessManagement-2023.5.23.7/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-05-23 10:17:25.000000 FishProcessManagement-2023.5.23.7/setup.py
```

### Comparing `FishProcessManagement-2023.5.23.6/FishProcessManagement/__init__.py` & `FishProcessManagement-2023.5.23.7/FishProcessManagement/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,12 +67,12 @@
                 进程池[进程名] = (进程, pid, False)
                 print("进程已启动")
                 显示进程池信息(进程池)
             else:
                 print("找不到对应的进程名字")
         else:
             print("无效的命令")
-# 进程列表 = {
-#     '第一个进程': ['python', 'child.py'],
-#     # 其他进程信息
-#     }
-# 进程管理器(进程列表)
+进程列表 = {
+    '第一个进程': ['python', 'child.py'],
+    # 其他进程信息
+    }
+进程管理器(进程列表)
```

### Comparing `FishProcessManagement-2023.5.23.6/FishProcessManagement/child.py` & `FishProcessManagement-2023.5.23.7/FishProcessManagement/child.py`

 * *Files identical despite different names*

### Comparing `FishProcessManagement-2023.5.23.6/FishProcessManagement.egg-info/PKG-INFO` & `FishProcessManagement-2023.5.23.7/FishProcessManagement.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FishProcessManagement
-Version: 2023.5.23.6
+Version: 2023.5.23.7
 Summary: 一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置
 Home-page: https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0
 Author: FishProcessManagement
 Author-email: 2645602049@qq.com
 Description-Content-Type: text/markdown
 
 >它是一个启动python项目的工具
@@ -20,20 +20,23 @@
 
 - 主进程(在进程管理器中使用的代码)
 
 ```
 
 import FishProcessManagement
 
-进程列表 = [
-['第一个进程', ['python', 'child.py']],
-]
+import FishProcessManagement
+进程列表 = {
+    '第一个进程': ['python', 'child.py'],
+    '第二个进程': ['python', 'child.py'],
 
+    }
 FishProcessManagement.进程管理器(进程列表)
 
+
 ```
```

### Comparing `FishProcessManagement-2023.5.23.6/PKG-INFO` & `FishProcessManagement-2023.5.23.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FishProcessManagement
-Version: 2023.5.23.6
+Version: 2023.5.23.7
 Summary: 一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置
 Home-page: https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0
 Author: FishProcessManagement
 Author-email: 2645602049@qq.com
 Description-Content-Type: text/markdown
 
 >它是一个启动python项目的工具
@@ -20,20 +20,23 @@
 
 - 主进程(在进程管理器中使用的代码)
 
 ```
 
 import FishProcessManagement
 
-进程列表 = [
-['第一个进程', ['python', 'child.py']],
-]
+import FishProcessManagement
+进程列表 = {
+    '第一个进程': ['python', 'child.py'],
+    '第二个进程': ['python', 'child.py'],
 
+    }
 FishProcessManagement.进程管理器(进程列表)
 
+
 ```
```

### Comparing `FishProcessManagement-2023.5.23.6/README.md` & `FishProcessManagement-2023.5.23.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 
 - 主进程(在进程管理器中使用的代码)
 
 ```
 
 import FishProcessManagement
 
-进程列表 = [
-['第一个进程', ['python', 'child.py']],
-]
+import FishProcessManagement
+进程列表 = {
+    '第一个进程': ['python', 'child.py'],
+    '第二个进程': ['python', 'child.py'],
 
+    }
 FishProcessManagement.进程管理器(进程列表)
 
+
 ```
```

### Comparing `FishProcessManagement-2023.5.23.6/setup.py` & `FishProcessManagement-2023.5.23.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # python setup.py bdist_wheel # 打包为whl文件
 # python setup.py sdist # 打包为tar.gz文件
 # twine upload dist/*
 
 setup(
     name="FishProcessManagement",
-    version="2023.5.23.6",
+    version="2023.5.23.7",
     author="FishProcessManagement",
     author_email="2645602049@qq.com",
     description="一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置",
 
     # 项目主页
     url="https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0",
     # 长描述
```

