# Comparing `tmp/easytqdm-1.3.tar.gz` & `tmp/easytqdm-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytqdm-1.3.tar", last modified: Tue May 23 09:23:46 2023, max compression
+gzip compressed data, was "easytqdm-1.4.tar", last modified: Tue May 23 09:30:43 2023, max compression
```

## Comparing `easytqdm-1.3.tar` & `easytqdm-1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:23:46.688107 easytqdm-1.3/
--rw-rw-rw-   0        0        0      229 2023-05-23 09:23:46.687107 easytqdm-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 09:23:46.683109 easytqdm-1.3/easytqdm.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-23 09:23:45.000000 easytqdm-1.3/easytqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-23 09:23:46.000000 easytqdm-1.3/easytqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:23:45.000000 easytqdm-1.3/easytqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 09:23:46.000000 easytqdm-1.3/easytqdm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1848 2023-05-23 09:18:42.000000 easytqdm-1.3/easytqdm.py
--rw-rw-rw-   0        0        0       42 2023-05-23 09:23:46.689106 easytqdm-1.3/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-05-23 09:20:35.000000 easytqdm-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:30:43.938433 easytqdm-1.4/
+-rw-rw-rw-   0        0        0      229 2023-05-23 09:30:43.937433 easytqdm-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 09:30:43.935433 easytqdm-1.4/easytqdm.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-05-23 09:30:42.000000 easytqdm-1.4/easytqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-23 09:30:43.000000 easytqdm-1.4/easytqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:30:42.000000 easytqdm-1.4/easytqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 09:30:43.000000 easytqdm-1.4/easytqdm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1923 2023-05-23 09:30:12.000000 easytqdm-1.4/easytqdm.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:30:43.939443 easytqdm-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      543 2023-05-23 09:30:39.000000 easytqdm-1.4/setup.py
```

### Comparing `easytqdm-1.3/easytqdm.py` & `easytqdm-1.4/easytqdm.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,7 +52,9 @@
     def dec(self, epoch):
         self.description = epoch
 
     def __len__(self):
         return self.total
 
 
+def easytqdm(iterable, total=None):
+    return EasyTqdm(iterable, total)
```

### Comparing `easytqdm-1.3/setup.py` & `easytqdm-1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='easytqdm',# 需要打包的名字,即本模块要发布的名字
-    version='v1.3',#版本
+    version='v1.4',#版本
     description='easytqdm', # 简要描述
     py_modules=['easytqdm'],   #  需要打包的模块
     author='LXD', # 作者名
     author_email='clearlyzero@stu.cqut.edu.cn',   # 作者邮件
     url='https://github.com/clearlyzerolxd/easytqdm', # 项目地址,一般是代码托管的网站
     # requires=['requests','urllib3'], # 依赖包,如果没有,可以不要
     license='MIT'
```

