# Comparing `tmp/MicroLIA-2.1.0.tar.gz` & `tmp/MicroLIA-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicroLIA-2.1.0.tar", last modified: Mon May 22 20:42:30 2023, max compression
+gzip compressed data, was "MicroLIA-2.2.0.tar", last modified: Mon May 22 22:02:21 2023, max compression
```

## Comparing `MicroLIA-2.1.0.tar` & `MicroLIA-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.682300 MicroLIA-2.1.0/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.1.0/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.1.0/MANIFEST.in
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.668140 MicroLIA-2.1.0/MicroLIA/
--rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.1.0/MicroLIA/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.1.0/MicroLIA/cnn_model.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.680612 MicroLIA-2.1.0/MicroLIA/data/
--rw-r--r--   0 daniel     (501) staff       (20)     6148 2023-05-22 19:33:40.000000 MicroLIA-2.1.0/MicroLIA/data/.DS_Store
--rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.1.0/MicroLIA/data/Miras_vo.xml
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2022-07-17 06:13:15.000000 MicroLIA-2.1.0/MicroLIA/data/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.1.0/MicroLIA/data_augmentation.py
--rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.1.0/MicroLIA/data_processing.py
--rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.1.0/MicroLIA/ensemble_model.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.1.0/MicroLIA/extract_features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.1.0/MicroLIA/features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.1.0/MicroLIA/noise_models.py
--rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.1.0/MicroLIA/optimization.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.1.0/MicroLIA/quality_check.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    20101 2023-05-22 20:37:04.000000 MicroLIA-2.1.0/MicroLIA/simulate.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    25740 2023-05-22 20:21:37.000000 MicroLIA-2.1.0/MicroLIA/training_set.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 20:42:30.671665 MicroLIA-2.1.0/MicroLIA.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      593 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-22 20:42:30.000000 MicroLIA-2.1.0/MicroLIA.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 20:42:30.681843 MicroLIA-2.1.0/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.1.0/README.md
--rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.1.0/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-22 20:42:30.682558 MicroLIA-2.1.0/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1162 2023-05-22 20:32:10.000000 MicroLIA-2.1.0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.854395 MicroLIA-2.2.0/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.2.0/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.2.0/MANIFEST.in
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.838681 MicroLIA-2.2.0/MicroLIA/
+-rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.2.0/MicroLIA/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.2.0/MicroLIA/cnn_model.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.852569 MicroLIA-2.2.0/MicroLIA/data/
+-rw-r--r--   0 daniel     (501) staff       (20)     6148 2023-05-22 20:44:02.000000 MicroLIA-2.2.0/MicroLIA/data/.DS_Store
+-rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.2.0/MicroLIA/data/Miras_vo.xml
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2022-07-17 06:13:15.000000 MicroLIA-2.2.0/MicroLIA/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.2.0/MicroLIA/data_augmentation.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.2.0/MicroLIA/data_processing.py
+-rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.2.0/MicroLIA/ensemble_model.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.2.0/MicroLIA/extract_features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.2.0/MicroLIA/features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.2.0/MicroLIA/noise_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.2.0/MicroLIA/optimization.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.2.0/MicroLIA/quality_check.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    20101 2023-05-22 20:37:04.000000 MicroLIA-2.2.0/MicroLIA/simulate.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    25956 2023-05-22 21:13:10.000000 MicroLIA-2.2.0/MicroLIA/training_set.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.843628 MicroLIA-2.2.0/MicroLIA.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      593 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 22:02:21.853793 MicroLIA-2.2.0/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.2.0/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.2.0/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-22 22:02:21.854576 MicroLIA-2.2.0/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1162 2023-05-22 22:00:17.000000 MicroLIA-2.2.0/setup.py
```

### Comparing `MicroLIA-2.1.0/LICENSE.txt` & `MicroLIA-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/cnn_model.py` & `MicroLIA-2.2.0/MicroLIA/cnn_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/data/.DS_Store` & `MicroLIA-2.2.0/MicroLIA/data/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0002 0000 0009  ................
 00000210: 0053 0065 0073 0061 0072 0032 0030 0031  .S.e.s.a.r.2.0.1
-00000220: 0030 6277 7370 626c 6f62 0000 00b7 6270  .0bwspblob....bp
+00000220: 0030 6277 7370 626c 6f62 0000 00b8 6270  .0bwspblob....bp
 00000230: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
 00000240: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 00000250: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 00000260: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 00000270: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 00000280: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00000290: 6f77 5369 6465 6261 7208 0908 095f 1017  owSidebar...._..
-000002a0: 7b7b 3134 2c20 3232 357d 2c20 7b39 3230  {{14, 225}, {920
-000002b0: 2c20 3436 347d 7d09 0815 232f 3b52 5f6b  , 464}}...#/;R_k
-000002c0: 6c6d 6e6f 8900 0000 0000 0001 0100 0000  lmno............
-000002d0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 8a00 0000 0900 5300 6500 7300  ..........S.e.s.
-000002f0: 6100 7200 3200 3000 3100 3076 5372 6e6c  a.r.2.0.1.0vSrnl
-00000300: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
+00000290: 6f77 5369 6465 6261 7208 0908 095f 1018  owSidebar...._..
+000002a0: 7b7b 3632 342c 2034 3237 7d2c 207b 3932  {{624, 427}, {92
+000002b0: 302c 2034 3336 7d7d 0908 1523 2f3b 525f  0, 436}}...#/;R_
+000002c0: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
+000002d0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 008b 0000 0009 0053 0065 0073  ...........S.e.s
+000002f0: 0061 0072 0032 0030 0031 0030 7653 726e  .a.r.2.0.1.0vSrn
+00000300: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `MicroLIA-2.1.0/MicroLIA/data/Miras_vo.xml` & `MicroLIA-2.2.0/MicroLIA/data/Miras_vo.xml`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/data_augmentation.py` & `MicroLIA-2.2.0/MicroLIA/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/data_processing.py` & `MicroLIA-2.2.0/MicroLIA/data_processing.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/ensemble_model.py` & `MicroLIA-2.2.0/MicroLIA/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/extract_features.py` & `MicroLIA-2.2.0/MicroLIA/extract_features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/features.py` & `MicroLIA-2.2.0/MicroLIA/features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/noise_models.py` & `MicroLIA-2.2.0/MicroLIA/noise_models.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/optimization.py` & `MicroLIA-2.2.0/MicroLIA/optimization.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/quality_check.py` & `MicroLIA-2.2.0/MicroLIA/quality_check.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/simulate.py` & `MicroLIA-2.2.0/MicroLIA/simulate.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/MicroLIA/training_set.py` & `MicroLIA-2.2.0/MicroLIA/training_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,20 @@
     stats_list = []
 
     progess_bar = bar.FillingSquaresBar('Simulating variables......', max=n_class)
     for k in range(1,n_class+1):
         time = random.choice(timestamps)
         baseline = np.random.uniform(min_mag,max_mag)
         mag, amplitude, period = simulate.rrlyr_variable(time, baseline)
-           
+        
+        #Incorrect template fitting yields negative mag! 
+        if np.min(mag) < 0:
+            while np.min(mag) < 0:
+                mag, amplitude, period = simulate.rrlyr_variable(time, baseline)
+                
         if noise is not None:
             mag, magerr = noise_models.add_noise(mag, noise, zp=zp, exptime=exptime)
         if noise is None:
            mag, magerr = noise_models.add_gaussian_noise(mag, zp=zp, exptime=exptime)
            
         source_class = ['VARIABLE']*len(time)
         source_class_list.append(source_class)
```

### Comparing `MicroLIA-2.1.0/MicroLIA.egg-info/PKG-INFO` & `MicroLIA-2.2.0/MicroLIA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.1.0
+Version: 2.2.0
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.1.0/MicroLIA.egg-info/SOURCES.txt` & `MicroLIA-2.2.0/MicroLIA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/PKG-INFO` & `MicroLIA-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.1.0
+Version: 2.2.0
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.1.0/README.md` & `MicroLIA-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.1.0/setup.py` & `MicroLIA-2.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="MicroLIA",
-    version="2.1.0",
+    version="2.2.0",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Machine learning classifier for microlensing",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/MicroLIA",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
```

