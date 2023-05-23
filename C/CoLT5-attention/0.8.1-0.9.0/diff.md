# Comparing `tmp/CoLT5-attention-0.8.1.tar.gz` & `tmp/CoLT5-attention-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.8.1.tar", last modified: Mon May 15 22:02:02 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.9.0.tar", last modified: Mon May 22 16:46:17 2023, max compression
```

## Comparing `CoLT5-attention-0.8.1.tar` & `CoLT5-attention-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:02:02.031594 CoLT5-attention-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:02:02.031594 CoLT5-attention-0.8.1/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 22:02:02.000000 CoLT5-attention-0.8.1/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-15 22:02:02.000000 CoLT5-attention-0.8.1/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:02:02.000000 CoLT5-attention-0.8.1/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 22:02:02.000000 CoLT5-attention-0.8.1/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:02:02.000000 CoLT5-attention-0.8.1/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 22:02:02.031594 CoLT5-attention-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:02:02.031594 CoLT5-attention-0.8.1/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    35704 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:02:02.031594 CoLT5-attention-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 22:01:49.000000 CoLT5-attention-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:17.826324 CoLT5-attention-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:17.822323 CoLT5-attention-0.9.0/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 16:46:17.000000 CoLT5-attention-0.9.0/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-22 16:46:17.000000 CoLT5-attention-0.9.0/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:46:17.000000 CoLT5-attention-0.9.0/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-22 16:46:17.000000 CoLT5-attention-0.9.0/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 16:46:17.000000 CoLT5-attention-0.9.0/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 16:46:17.826324 CoLT5-attention-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:46:17.826324 CoLT5-attention-0.9.0/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36039 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:46:17.826324 CoLT5-attention-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 16:46:06.000000 CoLT5-attention-0.9.0/setup.py
```

### Comparing `CoLT5-attention-0.8.1/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.9.0/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.8.1
+Version: 0.9.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.8.1/LICENSE` & `CoLT5-attention-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.8.1/PKG-INFO` & `CoLT5-attention-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.8.1
+Version: 0.9.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.8.1/README.md` & `CoLT5-attention-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -228,7 +228,17 @@
 @inproceedings{dao2022flashattention,
     title     = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
     author    = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
     booktitle = {Advances in Neural Information Processing Systems},
     year      = {2022}
 }
 ```
+
+```bibtex
+@article{Lei2023ConditionalAP,
+    title   = {Conditional Adapters: Parameter-efficient Transfer Learning with Fast Inference},
+    author  = {Tao Lei and Junwen Bai and Siddhartha Brahma and Joshua Ainslie and Kenton Lee and Yanqi Zhou and Nan Du and Vincent Zhao and Yuexin Wu and Bo Li and Yu Zhang and Ming-Wei Chang},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2304.04947}
+}
+```
```

#### html2text {}

```diff
@@ -126,8 +126,13 @@
 tiled neural network computations}, author = {Philippe Tillet and H. Kung and
 D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
 on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
 @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
 Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
 Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ```
+} ``` ```bibtex @article{Lei2023ConditionalAP, title = {Conditional Adapters:
+Parameter-efficient Transfer Learning with Fast Inference}, author = {Tao Lei
+and Junwen Bai and Siddhartha Brahma and Joshua Ainslie and Kenton Lee and
+Yanqi Zhou and Nan Du and Vincent Zhao and Yuexin Wu and Bo Li and Yu Zhang and
+Ming-Wei Chang}, journal = {ArXiv}, year = {2023}, volume = {abs/2304.04947} }
+```
```

### Comparing `CoLT5-attention-0.8.1/colt5_attention/attend.py` & `CoLT5-attention-0.9.0/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.8.1/colt5_attention/coor_descent.py` & `CoLT5-attention-0.9.0/colt5_attention/coor_descent.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,50 +2,68 @@
 import torch.nn.functional as F
 
 from einops import rearrange
 
 def exists(val):
     return val is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
 def log(t, eps = 1e-20):
     return torch.log(t.clamp(min = eps))
 
 def coor_descent(
     s,
     *,
     n_iters,
     k,
     eps = 1e-1,
+    eps_init = None,
+    eps_decay = 1.,
     mask = None
 ):
+    """
+    coordinate descent  - https://arxiv.org/abs/1502.04759, utilized in https://arxiv.org/abs/2303.09752
+    ε-scaling           - https://arxiv.org/abs/1610.06519, utilized in https://arxiv.org/abs/2304.04947
+
+    in a follow up paper applying coordinate descent routing to efficient fine tuning
+    they were able to cut n_iters from 50 -> 20 by setting eps_init = 4 and eps_decay = 0.7
+    eps was dependent on the task, and ranged from 0.02 to 1
+    """
+
     assert n_iters > 0
 
     mask_value = -torch.finfo(s.dtype).max
 
     if not isinstance(k, torch.Tensor):
         k = torch.Tensor([k]).to(s)
     else:
         k = rearrange(k, '... -> ... 1')
 
-    constant = eps * log(k)
+    logk = log(k)
 
     if exists(mask):
         s = s.masked_fill(~mask, mask_value)
 
     a = 0
     b = -s
 
+    current_eps = max(default(eps_init, eps), eps)
+
     for _ in range(n_iters):
-        sb = ((s + b) / eps)
+        sb = ((s + b) / current_eps)
 
         if exists(mask):
             sb = sb.masked_fill(~mask, mask_value)
 
-        a = constant - eps * sb.logsumexp(dim = -1, keepdim = True)
+        a = current_eps * (logk - sb.logsumexp(dim = -1, keepdim = True))
         b = -F.relu(s + a)
 
-    scores = ((s + a + b) / eps).exp()
+        current_eps = max(current_eps * eps_decay, eps)
+
+    scores = ((s + a + b) / current_eps).exp()
 
     if exists(mask):
         scores = scores.masked_fill(~mask, 0.)
 
     return scores
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CoLT5-attention-0.8.1/colt5_attention/transformer_block.py` & `CoLT5-attention-0.9.0/colt5_attention/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,32 +245,39 @@
     finally, used successfully by this paper for routing to heavy branch attention / feedforward
     """
 
     def __init__(
         self,
         dim,
         straight_through = True,
-        n_iters = 50,                   # 50 iterations in the paper
+        n_iters = 20,                   # 20 iterations in a new paper, utilizing ε-scaling
         fetch_k_ratio = 9 / 8,          # in the paper, they do a bit slightly higher k (times this ratio) for better learning
-        eps = 1.,                       # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
+        eps = 0.03,                     # the epsilon for coordinate descent. in a recent paper, they used 0.03 for text and 1.0 for speech
+        eps_decay = 0.7,
+        eps_init = 4.,
         num_routing_tokens = 1,
         learned_routing_tokens = False,
         use_triton = False,
         route_block_size = None,
         triton_checkpoint_segments = None # whether to recompute the coordinate descent in segments, with 4 and 50 iterations, backwards is sped up 3x times at the expense of forwards and some memory for saving initial a and b
     ):
         super().__init__()
         assert fetch_k_ratio >= 1.
-        self.eps = eps
 
         self.n_iters = n_iters
         self.fetch_k_ratio = fetch_k_ratio
 
         self.coor_descent = coor_descent
 
+        # epsilon related hparams, for ε-scaling
+
+        self.eps = eps
+        self.eps_decay = eps_decay
+        self.eps_init = eps_init
+
         if use_triton:
             from colt5_attention.triton_coor_descent import triton_coor_descent
             triton_checkpoint_segments = default(triton_checkpoint_segments, n_iters // 10)
             self.coor_descent = partial(triton_coor_descent, checkpoint_segments = triton_checkpoint_segments)
 
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
@@ -290,15 +297,15 @@
         x,
         *,
         num_tokens,
         mask = None,
         random_route = False,
         routing_tokens = None
     ):
-        n, device, eps, num_routes, route_block_size = x.shape[-2], x.device, self.eps, self.num_routing_tokens, self.route_block_size
+        n, device, eps, eps_init, eps_decay, num_routes, route_block_size = x.shape[-2], x.device, self.eps, self.eps_init, self.eps_decay, self.num_routing_tokens, self.route_block_size
 
         # do not route if the sequence length is less than the number of tokens
 
         if n < num_tokens:
             b = x.shape[0]
             r = self.num_routing_tokens
 
@@ -365,15 +372,17 @@
         # coordinate descent
 
         scores = self.coor_descent(
             s,
             n_iters = self.n_iters,
             mask = mask,
             k = k,
-            eps = eps
+            eps = eps,
+            eps_init = eps_init,
+            eps_decay = eps_decay
         )
 
         # force random routing, if negative control
 
         if random_route:
             scores = torch.randn_like(scores)
             scores = scores.masked_fill(~mask, -torch.finfo(scores.dtype).max)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CoLT5-attention-0.8.1/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.9.0/colt5_attention/triton_coor_descent.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     k_ptr,
     a_iter_stride,
     b_row_stride,
     b_iter_stride,
     input_row_stride,
     mask_row_stride,
     n_iters,
+    current_eps,
+    eps_decay,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
     col_offsets = tl.arange(0, BLOCK_SIZE)
     col_mask = col_offsets < n_cols
@@ -101,38 +103,43 @@
     # load k - controls the sparsity of output
 
     k_ptr = k_ptr + row_idx
     k = tl.load(k_ptr)
 
     # initialize some constants
 
-    constant = tl.log(k) * eps
-
-    inv_eps = 1. / eps
+    logk = tl.log(k)
 
     for _ in range(n_iters):        
 
-        a = (s + b) * inv_eps
+        a = (s + b) / current_eps
         a = tl.where(mask, a, -float('inf'))
 
         # stable log sum exp
 
         a_max = tl.max(a, axis = 0)
         a_minus_max = a - a_max
         exp = tl.exp(a_minus_max)
         sum_exp = tl.sum(exp, axis = 0)
         log_sum_exp = tl.log(sum_exp) + a_max
 
-        a = constant - eps * log_sum_exp
+        a = current_eps * (logk - log_sum_exp)
 
         # update b
 
         b = s + a
         b = tl.where(b >= 0., -b, 0.)
 
+        # decay epsilon, from epsilon-scaling
+
+        current_eps *= eps_decay
+
+        if current_eps < eps:
+            current_eps = eps
+
     # store a and b for next round
 
     next_a_ptrs = a_ptr + a_iter_stride
     next_b_ptrs = b_ptrs + b_iter_stride
 
     tl.store(next_a_ptrs, a)
     tl.store(next_b_ptrs, b, mask = col_mask)
@@ -151,14 +158,16 @@
     k_ptr,
     input_row_stride,
     b_row_stride,
     mask_row_stride,
     ds_row_stride,
     db_row_stride,
     n_iters,
+    eps_init,
+    eps_decay,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
     col_offsets = tl.arange(0, BLOCK_SIZE)
 
@@ -191,15 +200,15 @@
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
 
     # load k - controls the sparsity of output
 
     k_ptr = k_ptr + row_idx
 
     k = tl.load(k_ptr)
-    constant = tl.log(k) * eps
+    logk = tl.log(k)
 
     # load initial ds
 
     ds_row_start_ptr = ds_ptr + row_idx * ds_row_stride
     ds_ptrs = ds_row_start_ptr + col_offsets
 
     ds = tl.load(ds_ptrs, mask = mask, other = 0.)
@@ -214,58 +223,69 @@
     # load initial dk
 
     dk_ptr = dk_ptr + row_idx
     dk = tl.load(dk_ptr)
 
     # temp variables
 
-    inv_eps = 1. / eps
     last_da = tl.sum(ds, axis = 0)
 
     # backwards
 
     for ind in range(n_iters):
         a = init_a
         b = init_b
 
         sa = s * 0
         softmax = s * 0
 
+        # calculate epsilon
+
+        current_eps = eps_init / eps_decay
+
         # recompute
 
         for _ in range(n_iters - ind):
+            # update epsilon
+
+            current_eps *= eps_decay
 
-            sb = (s + b) * inv_eps
+            if current_eps < eps:
+                current_eps = eps
+
+            # updating a
+
+            sb = (s + b) / current_eps
             sb = tl.where(mask, sb, -float('inf'))
 
             # stable log sum exp
 
             sb_max = tl.max(sb, axis = 0)
             sb_minus_max = sb - sb_max
             exp = tl.exp(sb_minus_max)
             sum_exp = tl.sum(exp, axis = 0)
             softmax = exp / sum_exp
             log_sum_exp = tl.log(sum_exp) + sb_max
 
-            a = constant - eps * log_sum_exp
+            a = current_eps * (logk - log_sum_exp)
 
             # update b
 
             sa = s + a
             b = tl.where(sa > 0., -sa, 0.)
 
         # go backwards
 
         dsa = db * tl.where(sa > 0, -1., 0.)
 
         ds += dsa
 
         da = tl.sum(dsa, axis = 0) + last_da
 
-        dk += da
+        dk += da * current_eps
 
         dsb = da * -softmax
 
         ds += dsb
         db = dsb
 
         last_da = 0.
@@ -291,14 +311,16 @@
     def forward(
         self,
         ctx,
         x,
         n_iters,
         k,
         eps,
+        eps_init,
+        eps_decay,
         mask,
         checkpoint_segments
     ):
         assert n_iters > 0
         assert x.is_cuda, 'triton coordinate descent must be on cuda'
 
         batch, requires_grad, device, dtype = x.shape[0], x.requires_grad, x.device, x.dtype
@@ -308,14 +330,18 @@
 
         x, shape = pack_one(x, '* n')
         mask, _ = pack_one(mask, '* n')
 
         x = x.masked_fill(~mask, -torch.finfo(x.dtype).max)
         mask_ints = mask.int()
 
+        epsilons = []
+        eps_init = default(eps_init, eps)
+        current_eps = float(max(eps_init, eps))
+
         n_rows, n_cols = x.shape
 
         if isinstance(k, (int, float)):
             k = torch.full((n_rows,), k)
         elif k.ndim == 1:
             k = repeat(k, 'n -> (b n)', b = x.shape[0] // k.shape[0])
 
@@ -332,40 +358,49 @@
 
         checkpointed_a[0] = torch.zeros_like(k)
         checkpointed_b[0] = -x
 
         for ind, segment_iters in enumerate(num_to_groups(n_iters, checkpoint_segments)):
             is_last = ind == (checkpoint_segments - 1)
 
+            epsilons.append(current_eps)
+
             coor_descent_kernel_forward[(n_rows,)](
                 checkpointed_a[ind],
                 checkpointed_b[ind],
                 x,
                 mask_ints,
                 k,
                 checkpointed_a.stride(0),
                 n_cols,
                 checkpointed_b.stride(0),
                 x.stride(0),
                 mask_ints.stride(0),
                 segment_iters,
+                current_eps,
+                eps_decay,
                 eps,
                 n_cols,
                 num_warps = num_warps,
                 BLOCK_SIZE = BLOCK_SIZE,
             )
 
+            current_eps *= (eps_decay ** segment_iters)
+            current_eps = max(current_eps, eps)
+
         last_a, last_b = map(lambda t: t[-1], (checkpointed_a, checkpointed_b))
-        y = torch.exp((last_a[..., None] + last_b + x) / eps)
+        y = torch.exp((last_a[..., None] + last_b + x) / current_eps)
+
+        epsilons.append(current_eps)
 
         if requires_grad:
             checkpointed_a = checkpointed_a[:-1]
             checkpointed_b = checkpointed_b[:-1]
 
-            ctx.args = (n_iters, checkpoint_segments, eps)
+            ctx.args = (n_iters, checkpoint_segments, epsilons, eps_decay, eps)
             ctx.save_for_backward(x, y, k, mask, checkpointed_a, checkpointed_b)
 
         y = unpack_one(y, shape, '* n')
 
         return y
 
     @classmethod
@@ -374,40 +409,43 @@
         ctx,
         grad_probs
     ):
         assert grad_probs.is_cuda
 
         batch = grad_probs.shape[0]
 
-        n_iters, checkpoint_segments, eps = ctx.args
+        n_iters, checkpoint_segments, epsilons, eps_decay, eps = ctx.args
         x, y, k, mask, checkpointed_a, checkpointed_b = ctx.saved_tensors
 
         grad_probs, shape = pack_one(grad_probs, '* n')
 
         if exists(mask):
             grad_probs = grad_probs.masked_fill(~mask, 0.)
 
         n_rows, n_cols = grad_probs.shape
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
         num_warps = calc_num_warps(BLOCK_SIZE)
 
-        ds = grad_probs * y / eps
+        *epsilons, last_eps = epsilons
+
+        ds = grad_probs * y / last_eps
         db = ds.clone()
         dk = torch.zeros_like(k)
 
         mask_int = mask.int()
 
         items = zip(
             reversed(checkpointed_a.unbind(dim = 0)),
             reversed(checkpointed_b.unbind(dim = 0)),
-            reversed(num_to_groups(n_iters, checkpoint_segments))
+            reversed(num_to_groups(n_iters, checkpoint_segments)),
+            reversed(epsilons)
         )
 
-        for init_a, init_b, segment_iters, in items:
+        for init_a, init_b, segment_iters, eps_init, in items:
             coor_descent_kernel_backward[(n_rows,)](
                 dk,
                 x,
                 init_a,
                 init_b,
                 mask_int,
                 ds,
@@ -415,36 +453,40 @@
                 k,
                 x.stride(0),
                 init_b.stride(0),
                 mask_int.stride(0),
                 ds.stride(0),
                 db.stride(0),
                 segment_iters,
+                eps_init,
+                eps_decay,
                 eps,
                 n_cols,
                 num_warps = num_warps,
                 BLOCK_SIZE = BLOCK_SIZE
             )
 
         ds += -db
         ds = unpack_one(ds, shape, '* n')
 
         if not k.requires_grad:
             dk = None
         else:
-            dk *= eps / k
+            dk /= k
 
-        return ds, None, dk, None, None, None
+        return ds, None, dk, None, None, None, None, None
 
 def triton_coor_descent(
     s,
     *,
     n_iters,
     k,
     eps = 1e-1,
+    eps_init = None,
+    eps_decay = 1.,
     mask = None,
     checkpoint_segments = 1
 ):
     if not s.is_cuda:
-        return coor_descent(s, n_iters = n_iters, k = k, eps = eps, mask = mask)
+        return coor_descent(s, n_iters = n_iters, k = k, eps = eps, eps_init = eps_init, eps_decay = eps_decay, mask = mask)
 
-    return _coor_descent.apply(s, n_iters, k, eps, mask, checkpoint_segments)
+    return _coor_descent.apply(s, n_iters, k, eps, eps_init, eps_decay, mask, checkpoint_segments)
```

### Comparing `CoLT5-attention-0.8.1/setup.py` & `CoLT5-attention-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.8.1',
+  version = '0.9.0',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

