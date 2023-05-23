# Comparing `tmp/qufit-1.1.8.tar.gz` & `tmp/qufit-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qufit-1.1.8.tar", last modified: Thu May 18 10:55:43 2023, max compression
+gzip compressed data, was "qufit-1.1.9.tar", last modified: Thu May 18 14:55:43 2023, max compression
```

## Comparing `qufit-1.1.8.tar` & `qufit-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:55:43.504061 qufit-1.1.8/
--rw-rw-rw-   0        0        0      820 2023-05-18 10:55:43.503070 qufit-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:55:43.473146 qufit-1.1.8/qufit/
--rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.8/qufit/__init__.py
--rw-rw-rw-   0        0        0    27114 2023-05-18 10:55:24.000000 qufit-1.1.8/qufit/dataTools.py
--rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.8/qufit/opt.py
--rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.8/qufit/optimize.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:55:43.501070 qufit-1.1.8/qufit.egg-info/
--rw-rw-rw-   0        0        0      820 2023-05-18 10:55:43.000000 qufit-1.1.8/qufit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-18 10:55:43.000000 qufit-1.1.8/qufit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 10:55:43.000000 qufit-1.1.8/qufit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 10:55:43.000000 qufit-1.1.8/qufit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 10:55:43.505059 qufit-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-18 10:55:31.000000 qufit-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:55:43.646407 qufit-1.1.9/
+-rw-rw-rw-   0        0        0      820 2023-05-18 14:55:43.645409 qufit-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 14:55:43.602524 qufit-1.1.9/qufit/
+-rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.9/qufit/__init__.py
+-rw-rw-rw-   0        0        0    27176 2023-05-18 11:08:08.000000 qufit-1.1.9/qufit/dataTools.py
+-rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.9/qufit/opt.py
+-rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.9/qufit/optimize.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:55:43.639428 qufit-1.1.9/qufit.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-05-18 14:55:43.000000 qufit-1.1.9/qufit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-18 14:55:43.000000 qufit-1.1.9/qufit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 14:55:43.000000 qufit-1.1.9/qufit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 14:55:43.000000 qufit-1.1.9/qufit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 14:55:43.647405 qufit-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-18 14:55:24.000000 qufit-1.1.9/setup.py
```

### Comparing `qufit-1.1.8/PKG-INFO` & `qufit-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.1.8
+Version: 1.1.9
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.1.8/qufit/dataTools.py` & `qufit-1.1.9/qufit/dataTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,14 +335,15 @@
     cLst_m, num0Lst, num1Lst = [], [], []
     cLst, pLst = [], []
     for i,qi in enumerate(range(dim)):
         ax0 = axes[i][0] if dim>1 else axes[0]
         ax1 = axes[i][1] if dim>1 else axes[1]
         if qi not in target:
             s_off, s_on = s_st[0,:,qi], s_st[1,:,qi]
+            center1, center0 = np.mean(s_off), np.mean(s_on)
             sdiff = complex((center1-center0))
             s0 = s_off / (sdiff/np.abs(sdiff))
             s1 = s_on / (sdiff/np.abs(sdiff))
             s0 = np.real(s0)
             s1 = np.real(s1)
             bins = 120
```

### Comparing `qufit-1.1.8/qufit/opt.py` & `qufit-1.1.9/qufit/opt.py`

 * *Files identical despite different names*

### Comparing `qufit-1.1.8/qufit/optimize.py` & `qufit-1.1.9/qufit/optimize.py`

 * *Files identical despite different names*

### Comparing `qufit-1.1.8/qufit.egg-info/PKG-INFO` & `qufit-1.1.9/qufit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.1.8
+Version: 1.1.9
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.1.8/setup.py` & `qufit-1.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qufit",
-    version="1.1.8",
+    version="1.1.9",
     author="赵寿宽(sk zhao)",
     author_email="2396776980@qq.com",
     description="本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/",
     packages=setuptools.find_packages(),
```

