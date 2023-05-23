# Comparing `tmp/easytqdm-1.0.tar.gz` & `tmp/easytqdm-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytqdm-1.0.tar", last modified: Tue May 23 08:09:05 2023, max compression
+gzip compressed data, was "easytqdm-1.3.tar", last modified: Tue May 23 09:23:46 2023, max compression
```

## Comparing `easytqdm-1.0.tar` & `easytqdm-1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:09:05.147537 easytqdm-1.0/
--rw-rw-rw-   0        0        0      229 2023-05-23 08:09:05.147537 easytqdm-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 08:09:05.145558 easytqdm-1.0/easytqdm.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-23 08:09:03.000000 easytqdm-1.0/easytqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-23 08:09:04.000000 easytqdm-1.0/easytqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:09:04.000000 easytqdm-1.0/easytqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 08:09:04.000000 easytqdm-1.0/easytqdm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1711 2023-05-23 08:03:32.000000 easytqdm-1.0/easytqdm.py
--rw-rw-rw-   0        0        0       42 2023-05-23 08:09:05.148550 easytqdm-1.0/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-05-23 08:06:27.000000 easytqdm-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:23:46.688107 easytqdm-1.3/
+-rw-rw-rw-   0        0        0      229 2023-05-23 09:23:46.687107 easytqdm-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 09:23:46.683109 easytqdm-1.3/easytqdm.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-05-23 09:23:45.000000 easytqdm-1.3/easytqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-23 09:23:46.000000 easytqdm-1.3/easytqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:23:45.000000 easytqdm-1.3/easytqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 09:23:46.000000 easytqdm-1.3/easytqdm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1848 2023-05-23 09:18:42.000000 easytqdm-1.3/easytqdm.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:23:46.689106 easytqdm-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      543 2023-05-23 09:20:35.000000 easytqdm-1.3/setup.py
```

### Comparing `easytqdm-1.0/easytqdm.py` & `easytqdm-1.3/easytqdm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import time
 
 
 class EasyTqdm:
     def __init__(self, iterable, total=None):
-        self.iterable = iterable
-        self.total = total
+        if isinstance(iterable, EasyTqdm):
+            self.iterable = iterable.iterable
+        else:
+            self.iterable = iterable
+
+        if total is None:
+            self.total = len(self.iterable)
+        else:
+            self.total = total
+
         self.start_time = time.time()
         self.progress = 0
         self.description = ""
 
         if self.total is None:
             try:
-                self.total = len(iterable)
+                self.total = len(self.iterable)
             except TypeError:
                 self.total = None
 
     def __iter__(self):
         for item in self.iterable:
             yield item
             self.progress += 1
@@ -35,18 +43,16 @@
             RED = '\033[91m'  # ANSI 转义序列，表示红色文本
             RESET = '\033[0m'  # 重置文本颜色
             g = GREEN + '\u2501' * int(round(self.progress / self.total, 2) * 30) + RESET
 
             r = RED + '\u2501' * int(round((self.total - self.progress) / self.total, 2) * 30) + RESET
 
             print(self.description, g + r,
-                  f" {self.progress}/{self.total+1}, [{elapsed_time:.2f}s -> {estimated_time:.2f}s] ", end='\r')
+                  f" {self.progress}/{self.total + 1}, [{elapsed_time:.2f}s -> {estimated_time:.2f}s] ", end='\r')
 
     def dec(self, epoch):
         self.description = epoch
 
     def __len__(self):
         return self.total
 
-def easytqdm(iterable, total=None):
-    return EasyTqdm(iterable, total)
```

### Comparing `easytqdm-1.0/setup.py` & `easytqdm-1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='easytqdm',# 需要打包的名字,即本模块要发布的名字
-    version='v1.0',#版本
+    version='v1.3',#版本
     description='easytqdm', # 简要描述
     py_modules=['easytqdm'],   #  需要打包的模块
     author='LXD', # 作者名
     author_email='clearlyzero@stu.cqut.edu.cn',   # 作者邮件
     url='https://github.com/clearlyzerolxd/easytqdm', # 项目地址,一般是代码托管的网站
     # requires=['requests','urllib3'], # 依赖包,如果没有,可以不要
     license='MIT'
```

