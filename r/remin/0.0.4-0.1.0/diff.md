# Comparing `tmp/remin-0.0.4.tar.gz` & `tmp/remin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remin-0.0.4.tar", last modified: Wed Apr 26 12:00:54 2023, max compression
+gzip compressed data, was "remin-0.1.0.tar", last modified: Tue May 23 18:44:01 2023, max compression
```

## Comparing `remin-0.0.4.tar` & `remin-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.0.4/.gitignore
--rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.4/LICENSE
--rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.0.4/Makefile
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-26 12:00:54.042894 remin-0.0.4/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.0.4/README.md
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.038894 remin-0.0.4/examples/
--rw-rw-r--   0 salih     (1000) salih     (1000)    78602 2023-04-17 09:08:31.000000 remin-0.0.4/examples/example_heat_problem.ipynb
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.038894 remin-0.0.4/examples/heat/
--rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.0.4/examples/heat/model.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/examples/heat/outputs/
--rw-rw-r--   0 salih     (1000) salih     (1000)   217061 2023-04-25 20:35:40.000000 remin-0.0.4/examples/heat/outputs/heat.png
--rw-rw-r--   0 salih     (1000) salih     (1000)    52733 2023-04-24 20:50:29.000000 remin-0.0.4/examples/heat/outputs/heat_best_model.pt
--rw-rw-r--   0 salih     (1000) salih     (1000)    52733 2023-04-21 02:09:04.000000 remin-0.0.4/examples/heat/outputs/heat_best_model_full_batch.pt
--rw-rw-r--   0 salih     (1000) salih     (1000)    52733 2023-04-21 01:56:00.000000 remin-0.0.4/examples/heat/outputs/heat_best_model_fully_loaded.pt
--rw-rw-r--   0 salih     (1000) salih     (1000)    52775 2023-04-21 02:09:04.000000 remin-0.0.4/examples/heat/outputs/heat_final_model_full_batch.pt
--rw-rw-r--   0 salih     (1000) salih     (1000)    52775 2023-04-21 01:56:00.000000 remin-0.0.4/examples/heat/outputs/heat_final_model_fully_loaded.pt
--rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.0.4/examples/heat/postprocess.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1495 2023-04-25 20:42:55.000000 remin-0.0.4/examples/heat/training.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-04-26 11:59:10.000000 remin-0.0.4/pyproject.toml
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.4/requirements.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-26 12:00:54.042894 remin-0.0.4/setup.cfg
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.034894 remin-0.0.4/src/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/src/remin/
--rw-rw-r--   0 salih     (1000) salih     (1000)       22 2023-04-26 11:59:09.000000 remin-0.0.4/src/remin/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1180 2023-04-24 20:56:05.000000 remin-0.0.4/src/remin/domain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      809 2023-04-17 01:46:30.000000 remin-0.0.4/src/remin/func.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     4031 2023-04-26 11:55:58.000000 remin-0.0.4/src/remin/residual.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     4336 2023-04-24 20:56:05.000000 remin-0.0.4/src/remin/solver.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/src/remin.egg-info/
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)      735 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/SOURCES.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/dependency_links.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/requires.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/top_level.txt
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.779185 remin-0.1.0/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.1.0/.gitignore
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.1.0/LICENSE
+-rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.1.0/Makefile
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-05-23 18:44:01.775185 remin-0.1.0/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.1.0/README.md
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.775185 remin-0.1.0/examples/
+-rw-rw-r--   0 salih     (1000) salih     (1000)    78602 2023-04-17 09:08:31.000000 remin-0.1.0/examples/example_heat_problem.ipynb
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.775185 remin-0.1.0/examples/heat/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.1.0/examples/heat/model.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.1.0/examples/heat/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1515 2023-05-06 19:07:30.000000 remin-0.1.0/examples/heat/training.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-05-23 18:42:25.000000 remin-0.1.0/pyproject.toml
+-rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.1.0/requirements.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-05-23 18:44:01.779185 remin-0.1.0/setup.cfg
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.775185 remin-0.1.0/src/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.775185 remin-0.1.0/src/remin/
+-rw-rw-r--   0 salih     (1000) salih     (1000)       22 2023-05-23 18:42:11.000000 remin-0.1.0/src/remin/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     5795 2023-05-23 18:09:37.000000 remin-0.1.0/src/remin/callbacks.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1294 2023-05-15 12:29:55.000000 remin-0.1.0/src/remin/domain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1045 2023-05-11 10:55:40.000000 remin-0.1.0/src/remin/func.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     5229 2023-05-23 18:13:40.000000 remin-0.1.0/src/remin/residual.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.775185 remin-0.1.0/src/remin/solver/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      117 2023-05-08 21:15:07.000000 remin-0.1.0/src/remin/solver/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1794 2023-05-11 14:29:44.000000 remin-0.1.0/src/remin/solver/residual_loss.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3456 2023-05-23 18:12:53.000000 remin-0.1.0/src/remin/solver/solver.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3475 2023-05-11 14:29:36.000000 remin-0.1.0/src/remin/solver/trainer.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-05-23 18:44:01.775185 remin-0.1.0/src/remin.egg-info/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-05-23 18:44:01.000000 remin-0.1.0/src/remin.egg-info/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)      570 2023-05-23 18:44:01.000000 remin-0.1.0/src/remin.egg-info/SOURCES.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-05-23 18:44:01.000000 remin-0.1.0/src/remin.egg-info/dependency_links.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-05-23 18:44:01.000000 remin-0.1.0/src/remin.egg-info/requires.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-05-23 18:44:01.000000 remin-0.1.0/src/remin.egg-info/top_level.txt
```

### Comparing `remin-0.0.4/.gitignore` & `remin-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `remin-0.0.4/LICENSE` & `remin-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remin-0.0.4/PKG-INFO` & `remin-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.0.4
+Version: 0.1.0
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `remin-0.0.4/README.md` & `remin-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `remin-0.0.4/examples/example_heat_problem.ipynb` & `remin-0.1.0/examples/example_heat_problem.ipynb`

 * *Files identical despite different names*

### Comparing `remin-0.0.4/examples/heat/model.py` & `remin-0.1.0/examples/heat/model.py`

 * *Files identical despite different names*

### Comparing `remin-0.0.4/examples/heat/postprocess.py` & `remin-0.1.0/examples/heat/postprocess.py`

 * *Files identical despite different names*

### Comparing `remin-0.0.4/examples/heat/training.py` & `remin-0.1.0/examples/heat/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from remin.solver import Solver
-from remin.residual import Residual, ResidualLoader
+from remin.solver import Solver, make_trainer
+from remin.residual import Residual, make_loader
 from remin import func, domain
 import torch
 from torch import nn
 from model import Heat
 
 torch.set_default_device('cuda')
 torch.set_float32_matmul_precision('high')
@@ -31,24 +31,25 @@
 
 pde_res = Residual(pde_col, pde_residual)
 ic_res = Residual(ic_col, ic_residual)
 bc0_res = Residual(bc0_col, bc_residual)
 bc1_res = Residual(bc1_col, bc_residual)
 
 if __name__ == '__main__':
-    loader = ResidualLoader(
+    loader = make_loader(
         [pde_res, ic_res, bc0_res, bc1_res],
         fully_loaded=True,
         #batched=False,
         #pin_memory=True,
         #num_workers=1
     )
 
     epochs = 35000
     lr = 2e-4
     optimizer = torch.optim.Adam(model.parameters(), lr=lr)
     lossfunc = nn.MSELoss()
-    heat = Solver('outputs/heat', model, loader, optimizer, lossfunc)
+    trainer = make_trainer(model, loader, optimizer, lossfunc)
+    heat = Solver('heat', 'outputs',trainer=trainer)
 
     heat.compile(backend='inductor', fullgraph=True)
 
-    heat.fit(epochs, log_epoch=1000, log_progress=100)
+    heat.fit(epochs)
```

### Comparing `remin-0.0.4/pyproject.toml` & `remin-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "remin"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
     { name="Salih Taşdelen", email="salih.tasdelen@hotmail.com"},
 ]
 description = "PINN solver implemented in Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `remin-0.0.4/src/remin/domain.py` & `remin-0.1.0/src/remin/domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 def Line(pt1, pt2, n_coll):
     ndim = len(pt1)
     scale = np.array([x2 - x1 for x1, x2 in zip(pt1, pt2)])
     shift = np.array(pt1)
     return lhs(ndim, n_coll) * scale + shift
 
 
+def Point(pt):
+    return np.array([pt])
+
+
 def Ring(center, radius, n_coll):
     center = np.array(center)
     theta = 2 * np.pi * lhs(1, n_coll)
     return radius * np.hstack((np.cos(theta), np.sin(theta))) + center
 
 
 def cut(domain_from, constraints):
@@ -36,7 +40,12 @@
     for constraint in constraints:
         cond = np.logical_and(cond, constraint(domain_from))
     return domain_from[cond]
 
 
 def union(*args):
     return np.vstack(args)
+
+
+def shuffle(domain):
+    np.random.shuffle(domain)
+    return domain
```

### Comparing `remin-0.0.4/src/remin/func.py` & `remin-0.1.0/src/remin/func.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import wraps
-from torch import func
+from torch import func, autograd
 from torch import _dynamo as dynamo
 
 
 def make_sum(f):
 
     @wraps(f)
     def _sum(*args, **kwargs):
@@ -35,13 +35,20 @@
 
     def _call(params, *args):
         return func.functional_call(model, dict(params), args)
 
     return _call
 
 
-def grad(f, argnum=0):
+def fgrad(f, argnum=1):
     return func.grad(make_sum(f), argnums=argnum)
 
 
-def gradi(f, i, argnum=0):
+def fgradi(f, i, argnum=1):
     return func.grad(take_col_sum(f, i), argnums=argnum)
+
+
+def grad(u, xs, create_graph=True, retain_graph=True):
+    return autograd.grad(u.sum(),
+                         xs,
+                         create_graph=create_graph,
+                         retain_graph=retain_graph)
```

### Comparing `remin-0.0.4/src/remin.egg-info/PKG-INFO` & `remin-0.1.0/src/remin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.0.4
+Version: 0.1.0
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

