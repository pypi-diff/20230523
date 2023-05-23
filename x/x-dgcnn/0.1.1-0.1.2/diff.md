# Comparing `tmp/x-dgcnn-0.1.1.tar.gz` & `tmp/x-dgcnn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.1.1.tar", last modified: Sun May 21 19:02:41 2023, max compression
+gzip compressed data, was "x-dgcnn-0.1.2.tar", last modified: Tue May 23 17:31:51 2023, max compression
```

## Comparing `x-dgcnn-0.1.1.tar` & `x-dgcnn-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:40.997079 x-dgcnn-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 19:02:29.000000 x-dgcnn-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 19:02:40.997079 x-dgcnn-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-21 19:02:29.000000 x-dgcnn-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:02:40.997079 x-dgcnn-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-21 19:02:29.000000 x-dgcnn-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:40.997079 x-dgcnn-0.1.1/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 19:02:29.000000 x-dgcnn-0.1.1/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-21 19:02:29.000000 x-dgcnn-0.1.1/x_dgcnn/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 19:02:29.000000 x-dgcnn-0.1.1/x_dgcnn/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:40.997079 x-dgcnn-0.1.1/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 19:02:40.000000 x-dgcnn-0.1.1/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-21 19:02:40.000000 x-dgcnn-0.1.1/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:02:40.000000 x-dgcnn-0.1.1/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 19:02:40.000000 x-dgcnn-0.1.1/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 19:02:40.000000 x-dgcnn-0.1.1/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:51.235447 x-dgcnn-0.1.2/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/x_dgcnn/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.1.1/LICENSE` & `x-dgcnn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.1.1/PKG-INFO` & `x-dgcnn-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.1.1/README.md` & `x-dgcnn-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,25 +58,26 @@
 
 ```python
 import torch
 from x_dgcnn import DGCNN_Seg, SpatialTransformNet
 
 # use stn and do part segmentation
 stn = SpatialTransformNet(k=40)
-model = DGCNN_Seg(k=40, in_dim=3, out_dim=4, n_category=10, stn=stn)
+model = DGCNN_Seg(k=40, in_dim=9, out_dim=4, n_category=10, stn=stn)
 x = torch.randn(8, 9, 2048)  # keep xyz at the first 3 channels if using stn
 xyz = x[:, :3].clone()
 category = torch.randint(0, 10, (10,))
 out = model(x, xyz, category)
 ```
 
 ## TODO
 - [ ] Add differentiable subset operator and coordinate descent as another option to fuse features.
 - [ ] Scale up model size and test.
 - [ ] Add sampling to get hierarchical features.
+- [ ] Do tasks on other tasks, e.x. rotation prediction, normal prediction, etc.
 
 ## References
 
 ```bibtex
 @article{wang2019dynamic,
   title={Dynamic graph cnn for learning on point clouds},
   author={Wang, Yue and Sun, Yongbin and Liu, Ziwei and Sarma, Sanjay E and Bronstein, Michael M and Solomon, Justin M},
```

### Comparing `x-dgcnn-0.1.1/x_dgcnn/dgcnn.py` & `x-dgcnn-0.1.2/x_dgcnn/dgcnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,19 +211,19 @@
         self.norm = nn.BatchNorm1d(emb_dim)
         self.act = nn.GELU()
         self.dropout = nn.Dropout(dropout) if dropout > 0 else nn.Identity()
 
         # head
         dim = emb_dim + depth * 64
         self.mlp = nn.Sequential(
-            nn.Conv1d(dim, 256, 1, bias=False),
-            nn.BatchNorm1d(256),
+            nn.Conv1d(dim, 512, 1, bias=False),
+            nn.BatchNorm1d(512),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
-            nn.Conv1d(256, 256, 1, bias=False),
+            nn.Conv1d(512, 256, 1, bias=False),
             nn.BatchNorm1d(256),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
             nn.Conv1d(256, 128, 1, bias=False),
             nn.BatchNorm1d(128),
             nn.GELU(),
         )
```

### Comparing `x-dgcnn-0.1.1/x_dgcnn/route.py` & `x-dgcnn-0.1.2/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.1.1/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.1.2/x_dgcnn.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

