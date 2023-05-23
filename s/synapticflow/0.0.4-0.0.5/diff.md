# Comparing `tmp/synapticflow-0.0.4.tar.gz` & `tmp/synapticflow-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapticflow-0.0.4.tar", max compression
+gzip compressed data, was "synapticflow-0.0.5.tar", max compression
```

## Comparing `synapticflow-0.0.4.tar` & `synapticflow-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.4/LICENSE
--rw-r--r--   0        0        0     3224 2023-05-21 04:10:05.738713 synapticflow-0.0.4/README.md
--rw-r--r--   0        0        0     1202 2023-05-21 20:12:27.675134 synapticflow-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      269 2023-05-21 20:12:25.868657 synapticflow-0.0.4/synapticflow/__init__.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.4/synapticflow/decision/__init__.py
--rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.4/synapticflow/decision/decision.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.4/synapticflow/encoding/__init__.py
--rw-r--r--   0        0        0    10258 2023-05-21 04:10:05.739497 synapticflow-0.0.4/synapticflow/encoding/encoders.py
--rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.4/synapticflow/learning/__init__.py
--rw-r--r--   0        0        0    22956 2023-05-21 04:10:05.740070 synapticflow-0.0.4/synapticflow/learning/learning_rules.py
--rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.4/synapticflow/learning/rewards.py
--rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.4/synapticflow/network/__init__.py
--rw-r--r--   0        0        0    12989 2023-05-21 20:08:41.240624 synapticflow-0.0.4/synapticflow/network/connections.py
--rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.4/synapticflow/network/monitors.py
--rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.4/synapticflow/network/network.py
--rw-r--r--   0        0        0    87912 2023-05-21 04:10:05.742433 synapticflow-0.0.4/synapticflow/network/neural_populations.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.4/synapticflow/plotting/__init__.py
--rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.4/synapticflow/plotting/plotting.py
--rw-r--r--   0        0        0    16715 2023-05-21 04:10:05.743240 synapticflow-0.0.4/synapticflow/plotting/visualization.py
--rw-r--r--   0        0        0       19 2023-05-21 04:10:05.743431 synapticflow-0.0.4/synapticflow/synapticflow.py
--rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.4/synapticflow/utils.py
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3224 2023-05-21 21:05:41.548967 synapticflow-0.0.5/README.md
+-rw-r--r--   0        0        0     1202 2023-05-23 10:18:05.706717 synapticflow-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-05-23 10:18:09.049291 synapticflow-0.0.5/synapticflow/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.5/synapticflow/decision/__init__.py
+-rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.5/synapticflow/decision/decision.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.5/synapticflow/encoding/__init__.py
+-rw-r--r--   0        0        0    10258 2023-05-21 21:05:41.550284 synapticflow-0.0.5/synapticflow/encoding/encoders.py
+-rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.5/synapticflow/learning/__init__.py
+-rw-r--r--   0        0        0    22956 2023-05-22 22:05:51.553391 synapticflow-0.0.5/synapticflow/learning/learning_rules.py
+-rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.5/synapticflow/learning/rewards.py
+-rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.5/synapticflow/network/__init__.py
+-rw-r--r--   0        0        0    13001 2023-05-23 08:32:21.373763 synapticflow-0.0.5/synapticflow/network/connections.py
+-rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.5/synapticflow/network/monitors.py
+-rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.5/synapticflow/network/network.py
+-rw-r--r--   0        0        0    87912 2023-05-21 21:05:41.553473 synapticflow-0.0.5/synapticflow/network/neural_populations.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.5/synapticflow/plotting/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.5/synapticflow/plotting/plotting.py
+-rw-r--r--   0        0        0    16715 2023-05-21 21:05:41.554393 synapticflow-0.0.5/synapticflow/plotting/visualization.py
+-rw-r--r--   0        0        0       19 2023-05-21 21:05:41.554724 synapticflow-0.0.5/synapticflow/synapticflow.py
+-rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.5/synapticflow/utils.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.5/PKG-INFO
```

### Comparing `synapticflow-0.0.4/LICENSE` & `synapticflow-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/README.md` & `synapticflow-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/pyproject.toml` & `synapticflow-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "synapticflow"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     "Arsham Gholamzadeh Khoee <arsham.gh97@gmail.com>",
     "Mobin Nesari <mobinnesari81@gmail.com>",
     "Mohammad Mehdi Begmaz <mohammadmehdi.begmaz@gmail.com>",
     "Negar Sourati <negarsourati@gmail.com>"
 ]
 maintainers =[
```

### Comparing `synapticflow-0.0.4/synapticflow/decision/decision.py` & `synapticflow-0.0.5/synapticflow/decision/decision.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/encoding/encoders.py` & `synapticflow-0.0.5/synapticflow/encoding/encoders.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/learning/learning_rules.py` & `synapticflow-0.0.5/synapticflow/learning/learning_rules.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/learning/rewards.py` & `synapticflow-0.0.5/synapticflow/learning/rewards.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/network/connections.py` & `synapticflow-0.0.5/synapticflow/network/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         )
         if w is None:
             if (self.w_min == float('-inf')) or (self.w_max == float('inf')):
                 w = torch.clamp(torch.rand(pre.n, post.n), self.w_min, self.w_max)
             else:
                 w = self.w_min + torch.rand(pre.n, post.n) * (self.w_max - self.w_min)
         else:
-            if (self.w_min != float('-inf')).any() or (self.w_max != float('inf')).any():
+            if (self.w_min != float('-inf')) or (self.w_max != float('inf')):
                 w = torch.clamp(torch.as_tensor(w), self.w_min, self.w_max)
 
         if d is None:
             # if (self.d_min == 0.0) or (self.d_max == 100.0):
             #     d = torch.clamp(torch.rand(pre.n, post.n), self.d_min, self.d_max)
             # else:
                 d = self.d_min + torch.rand(pre.n, post.n) * (self.d_max - self.d_min)
@@ -228,21 +228,23 @@
                          post=post,
                          w=w,
                          d=d,
                          d_min=d_min,
                          d_max=d_max,
                          mask=mask,
                          **kwargs)
+        
+        torch.manual_seed(random_seed)
         if w is None:
             if (self.w_min == float('-inf')) or (self.w_max == float('inf')):
                 w = torch.clamp(torch.rand(pre.n, post.n), self.w_min, self.w_max)
             else:
                 w = self.w_min + torch.rand(pre.n, post.n) * (self.w_max - self.w_min)
         else:
-            if (self.w_min != float('-inf')).any() or (self.w_max != float('inf')).any():
+            if (self.w_min != float('-inf')) or (self.w_max != float('inf')):
                 w = torch.clamp(torch.as_tensor(w), self.w_min, self.w_max)
 
         if d is None:
             # if (self.d_min == 0.0) or (self.d_max == 100.0):
             #     d = torch.clamp(torch.rand(pre.n, post.n), self.d_min, self.d_max)
             # else:
                 d = self.d_min + torch.rand(pre.n, post.n) * (self.d_max - self.d_min)
@@ -324,15 +326,15 @@
         )
         if w is None:
             if (self.w_min == float('-inf')) or (self.w_max == float('inf')):
                 w = torch.clamp(torch.rand(pre.n, post.n), self.w_min, self.w_max)
             else:
                 w = self.w_min + torch.rand(pre.n, post.n) * (self.w_max - self.w_min)
         else:
-            if (self.w_min != float('-inf')).any() or (self.w_max != float('inf')).any():
+            if (self.w_min != float('-inf')) or (self.w_max != float('inf')):
                 w = torch.clamp(torch.as_tensor(w), self.w_min, self.w_max)
 
         if d is None:
             # if (self.d_min == 0.0) or (self.d_max == 100.0):
             #     d = torch.clamp(torch.rand(pre.n, post.n), self.d_min, self.d_max)
             # else:
                 d = self.d_min + torch.rand(pre.n, post.n) * (self.d_max - self.d_min)
```

### Comparing `synapticflow-0.0.4/synapticflow/network/monitors.py` & `synapticflow-0.0.5/synapticflow/network/monitors.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/network/network.py` & `synapticflow-0.0.5/synapticflow/network/network.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/network/neural_populations.py` & `synapticflow-0.0.5/synapticflow/network/neural_populations.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/synapticflow/plotting/visualization.py` & `synapticflow-0.0.5/synapticflow/plotting/visualization.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.4/PKG-INFO` & `synapticflow-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapticflow
-Version: 0.0.4
+Version: 0.0.5
 Summary: A powerful Python package for simulating spiking neural networks (SNNs) using PyTorch with GPU acceleration.
 Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network (SNN)
 Author: Arsham Gholamzadeh Khoee
 Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee
 Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synapticflow Version: 0.0.4 Summary: A powerful
+Metadata-Version: 2.1 Name: synapticflow Version: 0.0.5 Summary: A powerful
 Python package for simulating spiking neural networks (SNNs) using PyTorch with
 GPU acceleration. Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network
 (SNN) Author: Arsham Gholamzadeh Khoee Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
```

