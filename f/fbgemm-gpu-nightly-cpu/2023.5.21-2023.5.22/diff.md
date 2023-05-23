# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.5.21-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.5.22-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,39 @@
-Zip file size: 3830634 bytes, number of entries: 37
--rw-r--r--  2.0 unx      567 b- defN 23-May-21 12:57 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14800 b- defN 23-May-21 12:57 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-May-21 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-21 12:57 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 13773960 b- defN 23-May-21 12:57 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-May-21 12:57 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-May-21 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2477 b- defN 23-May-21 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-May-21 12:57 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-May-21 12:57 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5727 b- defN 23-May-21 12:57 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     8738 b- defN 23-May-21 12:57 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    20503 b- defN 23-May-21 12:57 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx   134040 b- defN 23-May-21 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx    39018 b- defN 23-May-21 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-21 12:57 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1912 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4163 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     4465 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6474 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     4501 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     3710 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
--rw-r--r--  2.0 unx     1533 b- defN 23-May-21 12:51 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     4401 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4451 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6460 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     4487 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4407 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3696 b- defN 23-May-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     2934 b- defN 23-May-21 12:57 fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/METADATA
--rw-r--r--  2.0 unx      102 b- defN 23-May-21 12:57 fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-21 12:57 fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4129 b- defN 23-May-21 12:57 fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/RECORD
-37 files, 14105607 bytes uncompressed, 3823658 bytes compressed:  72.9%
+Zip file size: 3830633 bytes, number of entries: 37
+-rw-r--r--  2.0 unx      567 b- defN 23-May-22 13:03 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14800 b- defN 23-May-22 13:03 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-May-22 13:03 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-22 13:03 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 13773960 b- defN 23-May-22 13:03 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-May-22 13:03 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-May-22 13:03 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2477 b- defN 23-May-22 13:03 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-May-22 13:03 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-May-22 13:03 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5727 b- defN 23-May-22 13:03 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     8738 b- defN 23-May-22 13:03 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    20503 b- defN 23-May-22 13:03 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx   134040 b- defN 23-May-22 13:03 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx    39018 b- defN 23-May-22 13:03 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-22 13:03 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4163 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     4465 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6474 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     3710 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-May-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4451 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6460 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     4487 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3696 b- defN 23-May-22 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-May-22 13:03 fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/METADATA
+-rw-r--r--  2.0 unx      102 b- defN 23-May-22 13:03 fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-22 13:03 fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4129 b- defN 23-May-22 13:03 fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/RECORD
+37 files, 14105607 bytes uncompressed, 3823657 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -93,20 +93,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.5.21
+Version: 2023.5.22
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=fBw0hDYHVaob9Pc2IC_XnpQ0jRStbG9R-IZqBnMywRM,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=z_INEdVlMxPi-rrq4W7oma6YnJF6EqHFIJeD1VdJNh0,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=YO8izH_FCVjxnhlf-Rx3uwTYrKJeERYEGki-QwnWmag,4451
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=5NeEd5Vx-cEpJMLTXFbJqlUtbKptFtx6lFpTSrd6xKA,6460
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=aL3HeCkQw88kBm685hn1QQJpEtQvKha_XAki6GtzpUU,4487
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=qOeMzSHbEm74uOWD4W5r5UPZ1NpBqZefvYZS41_9kbE,4407
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=IjeKrN7_9l5SZppuc2WbOR8sv6JtRew5geHKKRIRexY,3696
-fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/METADATA,sha256=dWmuQlOodDOmVJq6pNf8OPiZOH42VMCLnB1_jbSF8lo,2934
-fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
-fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.5.21.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/METADATA,sha256=XCmgTb9pbnzMgz9LKWDMqqw-uhqEEThZNxVrwmzFELI,2934
+fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
+fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.5.22.dist-info/RECORD,,
```

