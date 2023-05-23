# Comparing `tmp/jcmutils-1.5.6.tar.gz` & `tmp/jcmutils-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.5.6.tar", last modified: Thu May 18 09:30:43 2023, max compression
+gzip compressed data, was "jcmutils-1.5.7.tar", last modified: Tue May 23 08:58:02 2023, max compression
```

## Comparing `jcmutils-1.5.6.tar` & `jcmutils-1.5.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 09:30:43.906537 jcmutils-1.5.6/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.6/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 09:30:43.906537 jcmutils-1.5.6/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.6/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 09:30:43.906537 jcmutils-1.5.6/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.6/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    11474 2023-05-18 09:30:19.000000 jcmutils-1.5.6/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.6/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.6/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.6/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 09:30:43.906537 jcmutils-1.5.6/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 09:30:43.000000 jcmutils-1.5.6/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 09:30:43.000000 jcmutils-1.5.6/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 09:30:43.000000 jcmutils-1.5.6/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 09:30:43.000000 jcmutils-1.5.6/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 09:30:43.000000 jcmutils-1.5.6/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 09:30:43.906537 jcmutils-1.5.6/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 09:30:25.000000 jcmutils-1.5.6/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 08:58:02.324372 jcmutils-1.5.7/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.7/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-23 08:58:02.324372 jcmutils-1.5.7/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.7/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 08:58:02.324372 jcmutils-1.5.7/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.7/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    11549 2023-05-23 08:57:15.000000 jcmutils-1.5.7/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.7/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.7/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.7/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-23 08:58:02.324372 jcmutils-1.5.7/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-23 08:58:02.000000 jcmutils-1.5.7/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-23 08:58:02.000000 jcmutils-1.5.7/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-23 08:58:02.000000 jcmutils-1.5.7/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-23 08:58:02.000000 jcmutils-1.5.7/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-23 08:58:02.000000 jcmutils-1.5.7/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-23 08:58:02.324372 jcmutils-1.5.7/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-23 08:57:24.000000 jcmutils-1.5.7/setup.py
```

### Comparing `jcmutils-1.5.6/LICENSE` & `jcmutils-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.6/README.md` & `jcmutils-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.6/jcmutils/dataset_utils.py` & `jcmutils-1.5.7/jcmutils/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,20 +119,20 @@
 
         gradX = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=1, dy=0, ksize=-1)
         gradY = cv2.Sobel(diff_img, ddepth=cv2.CV_32F, dx=0, dy=1, ksize=-1)
         
         # subtract the y-gradient from the x-gradient
         gradient = cv2.subtract(gradX, gradY)
         gradient = cv2.convertScaleAbs(gradient)
-        blurred = cv2.blur(gradient, (9, 9)) 
-        (_, thresh) = cv2.threshold(blurred, 60 , 255, cv2.THRESH_BINARY)
-        kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (18, 18))
-        closed = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel)
+        blurred = cv2.blur(gradient, (5, 5),borderType=cv2.BORDER_REFLECT) 
+        (_, thresh) = cv2.threshold(blurred, 55 , 255, cv2.THRESH_BINARY)
+        kernel = cv2.getStructuringElement(cv2.MORPH_CROSS, (13, 13))
+        closed = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel,iterations=3,borderType=cv2.BORDER_ISOLATED)
         closed = cv2.erode(closed, None, iterations=6)
-        closed = cv2.dilate(closed, None, iterations=6)
+        closed = cv2.dilate(closed, None, iterations=7)
 
         # 找距离图像中心点最近的一个封闭区域
         (cnts, _) = cv2.findContours(closed.copy(), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
         # c = sorted(cnts, key=cv2.contourArea, reverse=True)[0]
         min_dist = -1
         c = cnts[0]
         for conners in cnts:
```

### Comparing `jcmutils-1.5.6/jcmutils/gen_sources.py` & `jcmutils-1.5.7/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.6/jcmutils/logger.py` & `jcmutils-1.5.7/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.6/jcmutils/solver.py` & `jcmutils-1.5.7/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.6/setup.py` & `jcmutils-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.5.6'
+VERSION = '1.5.7'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

