# Comparing `tmp/vector_quantize_pytorch-1.5.3.tar.gz` & `tmp/vector_quantize_pytorch-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.3.tar", last modified: Sat May 20 14:30:19 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.4.tar", last modified: Tue May 23 20:27:28 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.3.tar` & `vector_quantize_pytorch-1.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:30:19.344693 vector_quantize_pytorch-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-20 14:30:19.344693 vector_quantize_pytorch-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:30:19.344693 vector_quantize_pytorch-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:30:19.344693 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-20 14:30:09.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:30:19.344693 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-20 14:30:19.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-20 14:30:19.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:30:19.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 14:30:19.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-20 14:30:19.000000 vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-23 20:27:14.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:27:28.290620 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 20:27:28.000000 vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.3/LICENSE` & `vector_quantize_pytorch-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.3/PKG-INFO` & `vector_quantize_pytorch-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.3
+Version: 1.5.4
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.3/README.md` & `vector_quantize_pytorch-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.3/setup.py` & `vector_quantize_pytorch-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.3',
+  version = '1.5.4',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.3/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -290,16 +290,14 @@
 
         dist = -torch.cdist(flatten, embed, p = 2)
 
         embed_ind = gumbel_sample(dist, dim = -1, temperature = self.sample_codebook_temp)
         embed_onehot = F.one_hot(embed_ind, self.codebook_size).type(dtype)
         embed_ind = embed_ind.view(*shape[:-1])
 
-        quantize = batched_embedding(embed_ind, self.embed)
-
         if self.training:
             cluster_size = embed_onehot.sum(dim = 1)
 
             self.all_reduce_fn(cluster_size)
             self.cluster_size.data.lerp_(cluster_size, 1 - self.decay)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
@@ -308,14 +306,16 @@
 
             cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum(dim = -1, keepdim = True)
 
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             self.embed.data.copy_(embed_normalized)
             self.expire_codes_(x)
 
+        quantize = batched_embedding(embed_ind, self.embed)
+
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
         dist = unpack_one(dist, ps, 'h * d')
 
         return quantize, embed_ind, dist
 
@@ -432,16 +432,14 @@
         embed = l2norm(embed)
 
         dist = einsum('h n d, h c d -> h n c', flatten, embed)
         embed_ind = gumbel_sample(dist, dim = -1, temperature = self.sample_codebook_temp)
         embed_onehot = F.one_hot(embed_ind, self.codebook_size).type(dtype)
         embed_ind = embed_ind.view(*shape[:-1])
 
-        quantize = batched_embedding(embed_ind, self.embed)
-
         if self.training:
             bins = embed_onehot.sum(dim = 1)
             self.all_reduce_fn(bins)
 
             self.cluster_size.data.lerp_(bins, 1 - self.decay)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
@@ -452,14 +450,16 @@
 
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             embed_normalized = l2norm(embed_normalized)
 
             self.embed.data.copy_(l2norm(embed_normalized))
             self.expire_codes_(x)
 
+        quantize = batched_embedding(embed_ind, self.embed)
+
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
         dist = unpack_one(dist, ps, 'h * d')
         return quantize, embed_ind, dist
 
 # main class
```

### Comparing `vector_quantize_pytorch-1.5.3/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.4/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.3
+Version: 1.5.4
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

