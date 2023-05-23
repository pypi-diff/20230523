# Comparing `tmp/nonebot_plugin_homo_mathematician-0.0.1.tar.gz` & `tmp/nonebot_plugin_homo_mathematician-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.1.tar", last modified: Tue May 23 18:51:56 2023, max compression
+gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.2.tar", last modified: Tue May 23 19:01:15 2023, max compression
```

## Comparing `nonebot_plugin_homo_mathematician-0.0.1.tar` & `nonebot_plugin_homo_mathematician-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 18:51:56.618306 nonebot_plugin_homo_mathematician-0.0.1/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      434 2023-05-23 18:51:56.617308 nonebot_plugin_homo_mathematician-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 18:51:56.607309 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/
--rw-rw-rw-   0        0        0      890 2023-05-19 04:01:21.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-05-23 18:33:15.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/handle.py
--rw-rw-rw-   0        0        0    12647 2023-05-23 18:30:58.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:51:56.615308 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician.egg-info/
--rw-rw-rw-   0        0        0      434 2023-05-23 18:51:56.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-23 18:51:56.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 18:51:56.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-23 18:51:56.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-05-23 18:51:56.000000 nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 18:51:56.618306 nonebot_plugin_homo_mathematician-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-05-23 18:50:30.000000 nonebot_plugin_homo_mathematician-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:01:15.198795 nonebot_plugin_homo_mathematician-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-05-23 19:01:15.198795 nonebot_plugin_homo_mathematician-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 19:01:15.188792 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/
+-rw-rw-rw-   0        0        0      890 2023-05-19 04:01:21.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-05-23 18:33:15.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/handle.py
+-rw-rw-rw-   0        0        0    12647 2023-05-23 18:30:58.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:01:15.196792 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-23 19:01:15.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-23 19:01:15.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:01:15.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-23 19:01:15.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-05-23 19:01:15.000000 nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 19:01:15.199794 nonebot_plugin_homo_mathematician-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-05-23 19:00:59.000000 nonebot_plugin_homo_mathematician-0.0.2/setup.py
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.1/LICENSE` & `nonebot_plugin_homo_mathematician-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/__init__.py` & `nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/handle.py` & `nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.1/nonebot_plugin_homo_mathematician/utils.py` & `nonebot_plugin_homo_mathematician-0.0.2/nonebot_plugin_homo_mathematician/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.1/setup.py` & `nonebot_plugin_homo_mathematician-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_homo_mathematician'
 
 setup(
     name=name,  
-    version='0.0.1',
+    version='0.0.2',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
     url="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
 
     # 设置依赖包
-    install_requires=["fractions","scipy", "nonebot2","nonebot-adapter-onebot"],
+    install_requires=["scipy", "nonebot2","nonebot-adapter-onebot"],
 )
```

