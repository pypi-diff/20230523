# Comparing `tmp/FishProcessManagement-2023.5.23.tar.gz` & `tmp/FishProcessManagement-2023.5.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FishProcessManagement-2023.5.23.tar", last modified: Tue May 23 07:38:23 2023, max compression
+gzip compressed data, was "FishProcessManagement-2023.5.23.1.tar", last modified: Tue May 23 08:17:25 2023, max compression
```

## Comparing `FishProcessManagement-2023.5.23.tar` & `FishProcessManagement-2023.5.23.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 07:38:23.539370 FishProcessManagement-2023.5.23/
-drwxrwxrwx   0        0        0        0 2023-05-23 07:38:23.536377 FishProcessManagement-2023.5.23/FishProcessManagement.egg-info/
--rw-rw-rw-   0        0        0      976 2023-05-23 07:38:23.000000 FishProcessManagement-2023.5.23/FishProcessManagement.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-23 07:38:23.000000 FishProcessManagement-2023.5.23/FishProcessManagement.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 07:38:23.000000 FishProcessManagement-2023.5.23/FishProcessManagement.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 07:38:23.000000 FishProcessManagement-2023.5.23/FishProcessManagement.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      976 2023-05-23 07:38:23.539370 FishProcessManagement-2023.5.23/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-05-23 07:13:28.000000 FishProcessManagement-2023.5.23/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 07:38:23.540367 FishProcessManagement-2023.5.23/setup.cfg
--rw-rw-rw-   0        0        0      820 2023-05-23 07:37:50.000000 FishProcessManagement-2023.5.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:17:25.813351 FishProcessManagement-2023.5.23.1/
+drwxrwxrwx   0        0        0        0 2023-05-23 08:17:25.794926 FishProcessManagement-2023.5.23.1/FishProcessManagement/
+-rw-rw-rw-   0        0        0       28 2023-05-23 07:52:21.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement/child.py
+-rw-rw-rw-   0        0        0     2264 2023-05-23 08:13:12.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement/main.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:17:25.810352 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/
+-rw-rw-rw-   0        0        0     1765 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1765 2023-05-23 08:17:25.812350 FishProcessManagement-2023.5.23.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2023-05-23 07:58:30.000000 FishProcessManagement-2023.5.23.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:17:25.813351 FishProcessManagement-2023.5.23.1/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-05-23 08:15:50.000000 FishProcessManagement-2023.5.23.1/setup.py
```

### Comparing `FishProcessManagement-2023.5.23/setup.py` & `FishProcessManagement-2023.5.23.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 filepath = 'README.md'
 
 
 setup(
     name="FishProcessManagement",
-    version="2023.5.23",
+    version="2023.5.23.1",
     author="FishProcessManagement",
     author_email="2645602049@qq.com",
     description="一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置",
 
     # 项目主页
     url="https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0",
     # 长描述
@@ -18,8 +18,11 @@
     long_description_content_type='text/markdown',
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     packages=find_packages(),
 
 
     # 依赖包，没有将会自动下载
     install_requires=[],
+        package_data={
+        'my_package': ['main.py','child.py'],
+    },
 )
```

