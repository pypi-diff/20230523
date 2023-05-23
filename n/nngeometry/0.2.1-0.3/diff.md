# Comparing `tmp/nngeometry-0.2.1.tar.gz` & `tmp/nngeometry-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tfjgeorge/repos/nngeometry/dist/tmpcksocim6/nngeometry-0.2.1.tar", last modified: Wed Feb 24 14:44:51 2021, max compression
+gzip compressed data, was "nngeometry-0.3.tar", last modified: Tue May 23 21:15:43 2023, max compression
```

## Comparing `nngeometry-0.2.1.tar` & `nngeometry-0.3.tar`

### file list

```diff
@@ -1,26 +1,44 @@
-drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-02-24 14:44:51.513433 nngeometry-0.2.1/
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      258 2021-02-24 14:44:51.513433 nngeometry-0.2.1/PKG-INFO
-drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-02-24 14:44:51.505433 nngeometry-0.2.1/nngeometry/
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/__init__.py
-drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-02-24 14:44:51.509433 nngeometry-0.2.1/nngeometry/generator/
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       31 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/generator/__init__.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    48433 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/generator/jacobian.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     6939 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/layercollection.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      185 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/maths.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     5546 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/metrics.py
-drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-02-24 14:44:51.513433 nngeometry-0.2.1/nngeometry/object/
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      324 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/object/__init__.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     2362 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/object/fspace.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     1613 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/object/map.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    33380 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/object/pspace.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    11002 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/object/vector.py
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      766 2021-02-24 14:43:01.000000 nngeometry-0.2.1/nngeometry/utils.py
-drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-02-24 14:44:51.509433 nngeometry-0.2.1/nngeometry.egg-info/
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      258 2021-02-24 14:44:51.000000 nngeometry-0.2.1/nngeometry.egg-info/PKG-INFO
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      530 2021-02-24 14:44:51.000000 nngeometry-0.2.1/nngeometry.egg-info/SOURCES.txt
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)        1 2021-02-24 14:44:51.000000 nngeometry-0.2.1/nngeometry.egg-info/dependency_links.txt
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)        1 2021-02-24 14:43:59.000000 nngeometry-0.2.1/nngeometry.egg-info/not-zip-safe
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       13 2021-02-24 14:44:51.000000 nngeometry-0.2.1/nngeometry.egg-info/requires.txt
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       11 2021-02-24 14:44:51.000000 nngeometry-0.2.1/nngeometry.egg-info/top_level.txt
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       38 2021-02-24 14:44:51.513433 nngeometry-0.2.1/setup.cfg
--rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      452 2021-02-24 14:44:20.000000 nngeometry-0.2.1/setup.py
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.177204 nngeometry-0.3/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     1070 2021-11-17 09:28:18.000000 nngeometry-0.3/LICENSE
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      239 2023-05-23 21:15:43.177204 nngeometry-0.3/PKG-INFO
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.169204 nngeometry-0.3/nngeometry/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/__init__.py
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.169204 nngeometry-0.3/nngeometry/generator/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       31 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/generator/__init__.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      274 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/generator/dummy.py
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.173204 nngeometry-0.3/nngeometry/generator/jacobian/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    29147 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/generator/jacobian/__init__.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    12821 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/generator/jacobian/grads.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     5942 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/generator/jacobian/grads_conv.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    11979 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/layercollection.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     3383 2021-11-22 10:21:37.000000 nngeometry-0.3/nngeometry/layers.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      185 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/maths.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     6421 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/metrics.py
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.173204 nngeometry-0.3/nngeometry/object/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      324 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/object/__init__.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     2464 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/object/fspace.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     1761 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/object/map.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    38232 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/object/pspace.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    12580 2021-11-17 09:28:18.000000 nngeometry-0.3/nngeometry/object/vector.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     1706 2023-05-23 21:13:12.000000 nngeometry-0.3/nngeometry/utils.py
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.169204 nngeometry-0.3/nngeometry.egg-info/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      239 2023-05-23 21:15:43.000000 nngeometry-0.3/nngeometry.egg-info/PKG-INFO
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      942 2023-05-23 21:15:43.000000 nngeometry-0.3/nngeometry.egg-info/SOURCES.txt
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)        1 2023-05-23 21:15:43.000000 nngeometry-0.3/nngeometry.egg-info/dependency_links.txt
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)        1 2021-11-22 10:24:57.000000 nngeometry-0.3/nngeometry.egg-info/not-zip-safe
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       13 2023-05-23 21:15:43.000000 nngeometry-0.3/nngeometry.egg-info/requires.txt
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       11 2023-05-23 21:15:43.000000 nngeometry-0.3/nngeometry.egg-info/top_level.txt
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)       38 2023-05-23 21:15:43.177204 nngeometry-0.3/setup.cfg
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      499 2023-05-23 21:13:12.000000 nngeometry-0.3/setup.py
+drwxrwxr-x   0 tfjgeorge  (1000) tfjgeorge  (1000)        0 2023-05-23 21:15:43.177204 nngeometry-0.3/tests/
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      867 2023-05-23 21:13:12.000000 nngeometry-0.3/tests/test_conv_switch.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    33160 2023-05-23 21:13:12.000000 nngeometry-0.3/tests/test_jacobian.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     3930 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_jacobian_ekfac.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)    10215 2023-05-23 21:13:12.000000 nngeometry-0.3/tests/test_jacobian_kfac.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     2776 2021-11-22 10:21:37.000000 nngeometry-0.3/tests/test_layers.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)      573 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_maths.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     6528 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_metrics.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     1915 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_pickle.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     3650 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_representations.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     1005 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_utils.py
+-rw-rw-r--   0 tfjgeorge  (1000) tfjgeorge  (1000)     7771 2021-11-17 09:28:18.000000 nngeometry-0.3/tests/test_vector.py
```

### Comparing `nngeometry-0.2.1/nngeometry/metrics.py` & `nngeometry-0.3/nngeometry/metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         The parameter matrix representation that will be used to store
         the matrix
     variants : string 'classif_logits' or 'regression', optional
             (default='classif_logits')
         Variant to use depending on how you interpret your function.
         Possible choices are:
          - 'classif_logits' when using logits for classification
-         - 'regression' when using a gaussian regression model
+         - 'classif_logsoftmax' when using log_softmax values for classification
+         - 'segmentation_logits' when using logits in a segmentation task
     trials : int, optional (default=1)
         Number of trials for Monte Carlo sampling
     device : string, optional (default='cpu')
         Target device for the returned matrix
     function : function, optional (default=None)
         An optional function if different from `model(input)`. If
         it is different from None, it will override the device
@@ -60,30 +61,45 @@
             probabilities = torch.exp(log_softmax)
             sampled_targets = torch.multinomial(probabilities, trials,
                                                 replacement=True)
             return trials ** -.5 * torch.gather(log_softmax, 1,
                                                 sampled_targets)
     elif variant == 'classif_logsoftmax':
 
-        def fim_function(input, target):
+        def fim_function(*d):
             log_softmax = function(*d)
             probabilities = torch.exp(log_softmax)
             sampled_targets = torch.multinomial(probabilities, trials,
                                                 replacement=True)
             return trials ** -.5 * torch.gather(log_softmax, 1,
                                                 sampled_targets)
+    elif variant == 'segmentation_logits':
+
+        def fim_function(*d):
+            log_softmax = torch.log_softmax(function(*d), dim=1)
+            s_mb, s_c, s_h, s_w = log_softmax.size()
+            log_softmax = log_softmax.permute(0, 2, 3, 1).contiguous() \
+                .view(s_mb * s_h * s_w, s_c)
+            probabilities = torch.exp(log_softmax)
+            sampled_indices = torch.multinomial(probabilities, trials,
+                                                replacement=True)
+            sampled_targets = torch.gather(log_softmax, 1,
+                                        sampled_indices)
+            sampled_targets = sampled_targets.view(s_mb, s_h * s_w, trials) \
+                .sum(dim=1)
+            return trials ** -.5 * sampled_targets
+                                                
     else:
         raise NotImplementedError
 
     generator = Jacobian(layer_collection=layer_collection,
                          model=model,
-                         loader=loader,
                          function=fim_function,
                          n_output=trials)
-    return representation(generator)
+    return representation(generator=generator, examples=loader)
 
 
 def FIM(model,
         loader,
         representation,
         n_output,
         variant='classif_logits',
@@ -143,11 +159,10 @@
             estimates = function(*d)
             return estimates
     else:
         raise NotImplementedError
 
     generator = Jacobian(layer_collection=layer_collection,
                          model=model,
-                         loader=loader,
                          function=function_fim,
                          n_output=n_output)
-    return representation(generator)
+    return representation(generator=generator, examples=loader)
```

### Comparing `nngeometry-0.2.1/nngeometry/object/fspace.py` & `nngeometry-0.3/nngeometry/object/fspace.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 
     @abstractmethod
     def __init__(self, generator):
         return NotImplementedError
 
 
 class FMatDense(FMatAbstract):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_gram_matrix()
+            self.data = generator.get_gram_matrix(examples)
 
-    def compute_eigendecomposition(self, impl='symeig'):
-        # TODO: test
-        if impl == 'symeig':
-            self.evals, self.evecs = torch.symeig(self.data, eigenvectors=True)
+    def compute_eigendecomposition(self, impl='eigh'):
+        s = self.data.size()
+        M = self.data.view(s[0] * s[1], s[2] * s[3])
+        if impl == 'eigh':
+            self.evals, self.evecs = torch.linalg.eigh(M)
         elif impl == 'svd':
-            _, self.evals, self.evecs = torch.svd(self.data, some=False)
+            _, self.evals, self.evecs = torch.svd(M, some=False)
+        else:
+            raise NotImplementedError
 
     def mv(self, v):
         # TODO: test
         v_flat = torch.mv(self.data, v.get_flat_representation())
         return FVector(vector_repr=v_flat)
 
     def vTMv(self, v):
```

### Comparing `nngeometry-0.2.1/nngeometry/object/map.py` & `nngeometry-0.3/nngeometry/object/map.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,53 +7,55 @@
 
     @abstractmethod
     def __init__(self, generator):
         return NotImplementedError
 
 
 class PushForwardDense(AbstractPushForward):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_jacobian()
+            self.data = generator.get_jacobian(examples)
 
     def get_dense_tensor(self):
         return self.data
 
     def mv(self, v):
         v_flat = torch.mv(self.data.view(-1, self.data.size(-1)),
                           v.get_flat_representation())
         v_flat = v_flat.view(self.data.size(0), self.data.size(1))
         return FVector(vector_repr=v_flat)
 
 
 class PushForwardImplicit(AbstractPushForward):
-    def __init__(self, generator):
+    def __init__(self, generator, data=None, examples=None):
         self.generator = generator
+        self.examples = examples
+        assert data is None
 
     def mv(self, v):
-        return self.generator.implicit_Jv(v)
+        return self.generator.implicit_Jv(v, self.examples)
 
 
 class PullBackAbstract(ABC):
 
     @abstractmethod
     def __init__(self, generator):
         return NotImplementedError
 
 
 class PullBackDense(PullBackAbstract):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_jacobian()
+            self.data = generator.get_jacobian(examples)
 
     def get_dense_tensor(self):
         return self.data
 
     def mv(self, v):
         v_flat = torch.mv(self.data.view(-1, self.data.size(-1)).t(),
                           v.get_flat_representation().view(-1))
```

### Comparing `nngeometry-0.2.1/nngeometry/object/pspace.py` & `nngeometry-0.3/nngeometry/object/pspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import torch
 from abc import ABC, abstractmethod
 from ..maths import kronecker
 from .vector import PVector
+from nngeometry.generator.dummy import DummyGenerator
 
 
 class PMatAbstract(ABC):
     """
     A :math:`d \\times d` matrix in parameter space. This abstract class
     defines common methods used in concrete representations.
 
     :param generator: The generator
     :type generator: :class:`nngeometry.generator.jacobian.Jacobian`
-    :param data: if None, uses the generator to populate the matrix data.
+    :param data: if None, it requires examples to be different from None, and
+        it uses the generator to populate the matrix data
+    :param examples: if data is None, it uses these examples to populate the
+        matrix using the generator. `examples` is either a Dataloader, or a
+        single mini-batch of (inputs, targets) from a Dataloader
+
+    Note:
+        Either `data` or `examples` has to be different from None, and both
+        cannot be not None at the same time.
     """
 
     @abstractmethod
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
         raise NotImplementedError
 
     @abstractmethod
     def get_dense_tensor(self):
         raise NotImplementedError
 
     @abstractmethod
@@ -83,43 +92,62 @@
         if dim == 0 or dim == 1:
             return s
         elif dim is None:
             return (s, s)
         else:
             raise IndexError
 
+    def _check_data_examples(self, data, examples):
+        """
+        Either data or examples has to be not None in order
+        to populate the matrix. If both are not None, then
+        it is ambiguous, then the following test will fail
+        """
+        assert (data is not None) ^ (examples is not None)
+
+    def __getstate__(self):
+        return {'layer_collection': self.generator.layer_collection,
+                'data': self.data,
+                'device': self.generator.get_device()}
+
+    def __setstate__(self, state_dict):
+        self.data = state_dict['data']
+        self.generator = DummyGenerator(state_dict['layer_collection'],
+                                        state_dict['device'])
+
 
 class PMatDense(PMatAbstract):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_covariance_matrix()
+            self.data = generator.get_covariance_matrix(examples)
 
-    def compute_eigendecomposition(self, impl='symeig'):
-        # TODO: test
-        if impl == 'symeig':
-            self.evals, self.evecs = torch.symeig(self.data, eigenvectors=True)
+    def compute_eigendecomposition(self, impl='eigh'):
+        if impl == 'eigh':
+            self.evals, self.evecs = torch.linalg.eigh(self.data)
         elif impl == 'svd':
             _, self.evals, self.evecs = torch.svd(self.data, some=False)
         else:
             raise NotImplementedError
 
     def solve(self, v, regul=1e-8, impl='solve'):
         """
         solves v = Ax in x
         """
         # TODO: test
         if impl == 'solve':
             # TODO: reuse LU decomposition once it is computed
-            inv_v, _ = torch.solve(v.get_flat_representation().view(-1, 1),
-                                   self.data +
-                                   regul * torch.eye(self.size(0),
-                                                     device=self.data.device))
+            inv_v = torch.linalg.solve(self.data + 
+                                       regul * torch.eye(self.size(0),
+                                                         device=self.data.device),
+                                       v.get_flat_representation().view(-1, 1))
             return PVector(v.layer_collection, vector_repr=inv_v[:, 0])
         elif impl == 'eigendecomposition':
             v_eigenbasis = self.project_to_diag(v)
             inv_v_eigenbasis = v_eigenbasis / (self.evals + regul)
             return self.project_from_diag(inv_v_eigenbasis)
         else:
             raise NotImplementedError
@@ -174,22 +202,38 @@
         return PMatDense(generator=self.generator,
                          data=sub_data)
 
     def __rmul__(self, x):
         return PMatDense(generator=self.generator,
                          data=x * self.data)
 
+    def mm(self, other):
+        """
+        Matrix-matrix product where `other` is another 
+        instance of PMatDense
+
+        :param other: Other FIM matrix
+        :type other: :class:`nngeometry.object.PMatDense`
+
+        :return: The matrix-matrix product
+        :rtype: :class:`nngeometry.object.PMatDense`
+        """
+        return PMatDense(self.generator,
+                         data=torch.mm(self.data, other.data))
+
 
 class PMatDiag(PMatAbstract):
-    def __init__(self, generator=None, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_covariance_diag()
+            self.data = generator.get_covariance_diag(examples)
 
     def inverse(self, regul=1e-8):
         inv_tensor = 1. / (self.data + regul)
         return PMatDiag(generator=self.generator,
                         data=inv_tensor)
 
     def mv(self, v):
@@ -231,22 +275,38 @@
         return PMatDiag(generator=self.generator,
                         data=sub_diags)
 
     def __rmul__(self, x):
         return PMatDiag(generator=self.generator,
                         data=x * self.data)
 
+    def mm(self, other):
+        """
+        Matrix-matrix product where `other` is another 
+        instance of PMatDiag
+
+        :param other: Other FIM matrix
+        :type other: :class:`nngeometry.object.PMatDiag`
+
+        :return: The matrix-matrix product
+        :rtype: :class:`nngeometry.object.PMatDiag`
+        """
+        return PMatDiag(self.generator,
+                         data=self.data * other.data)
+
 
 class PMatBlockDiag(PMatAbstract):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_covariance_layer_blocks()
+            self.data = generator.get_covariance_layer_blocks(examples)
 
     def trace(self):
         # TODO test
         return sum([torch.trace(b) for b in self.data.values()])
 
     def get_dense_tensor(self):
         s = self.generator.layer_collection.numel()
@@ -285,18 +345,18 @@
         out_dict = dict()
         for layer_id, layer in self.generator.layer_collection.layers.items():
             v = vs_dict[layer_id][0].view(-1)
             if layer.bias is not None:
                 v = torch.cat([v, vs_dict[layer_id][1].view(-1)])
             block = self.data[layer_id]
 
-            inv_v, _ = torch.solve(v.view(-1, 1),
-                                   block +
-                                   regul * torch.eye(block.size(0),
-                                                     device=block.device))
+            inv_v = torch.linalg.solve(block +
+                                       regul * torch.eye(block.size(0),
+                                                         device=block.device),
+                                       v.view(-1, 1))
             inv_v_tuple = (inv_v[:layer.weight.numel()]
                            .view(*layer.weight.size),)
             if layer.bias is not None:
                 inv_v_tuple = (inv_v_tuple[0],
                                inv_v[layer.weight.numel():]
                                .view(*layer.bias.size),)
 
@@ -343,20 +403,40 @@
                              data=sum_data)
 
     def __rmul__(self, x):
         sum_data = {l_id: x * d for l_id, d in self.data.items()}
         return PMatBlockDiag(generator=self.generator,
                              data=sum_data)
 
+    def mm(self, other):
+        """
+        Matrix-matrix product where `other` is another 
+        instance of PMatBlockDiag
+
+        :param other: Other FIM matrix
+        :type other: :class:`nngeometry.object.PMatBlockDiag`
+
+        :return: The matrix-matrix product
+        :rtype: :class:`nngeometry.object.PMatBlockDiag`
+        """
+        prod = dict()
+        for layer_id, block in self.data.items():
+            block_other = other.data[layer_id]
+            prod[layer_id] = torch.mm(block, block_other)
+        return PMatBlockDiag(self.generator,
+                             data=prod)
+
 
 class PMatKFAC(PMatAbstract):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is None:
-            self.data = generator.get_kfac_blocks()
+            self.data = generator.get_kfac_blocks(examples)
         else:
             self.data = data
 
     def trace(self):
         return sum([torch.trace(a) * torch.trace(g)
                     for a, g in self.data.values()])
 
@@ -393,16 +473,16 @@
                 pi = (torch.trace(a) / torch.trace(g) *
                       g.size(0) / a.size(0))**.5
             else:
                 pi = 1
             a_reg = a + regul**.5 * pi * torch.eye(a.size(0), device=g.device)
             g_reg = g + regul**.5 / pi * torch.eye(g.size(0), device=g.device)
 
-            solve_g, _ = torch.solve(v, g_reg)
-            solve_a, _ = torch.solve(solve_g.t(), a_reg)
+            solve_g, _, _, _ = torch.linalg.lstsq(g_reg, v)
+            solve_a, _, _, _ = torch.linalg.lstsq(a_reg, solve_g.t())
             solve_a = solve_a.t()
             if layer.bias is None:
                 solve_tuple = (solve_a.view(*sw),)
             else:
                 solve_tuple = (solve_a[:, :-1].contiguous().view(*sw),
                                solve_a[:, -1].contiguous())
             out_dict[layer_id] = solve_tuple
@@ -486,50 +566,70 @@
                                v.view(-1))
         return norm2
 
     def frobenius_norm(self):
         return sum([torch.trace(torch.mm(a, a)) * torch.trace(torch.mm(g, g))
                     for a, g in self.data.values()])**.5
 
-    def compute_eigendecomposition(self, impl='symeig'):
+    def compute_eigendecomposition(self, impl='eigh'):
         self.evals = dict()
         self.evecs = dict()
-        if impl == 'symeig':
+        if impl == 'eigh':
             for layer_id in self.generator.layer_collection.layers.keys():
                 a, g = self.data[layer_id]
-                evals_a, evecs_a = torch.symeig(a, eigenvectors=True)
-                evals_g, evecs_g = torch.symeig(g, eigenvectors=True)
+                evals_a, evecs_a = torch.linalg.eigh(a)
+                evals_g, evecs_g = torch.linalg.eigh(g)
                 self.evals[layer_id] = (evals_a, evals_g)
                 self.evecs[layer_id] = (evecs_a, evecs_g)
         else:
             raise NotImplementedError
 
     def get_eigendecomposition(self):
         return self.evals, self.evecs
 
+    def mm(self, other):
+        """
+        Matrix-matrix product where `other` is another 
+        instance of PMatKFAC
+
+        :param other: Other FIM matrix
+        :type other: :class:`nngeometry.object.PMatKFAC`
+
+        :return: The matrix-matrix product
+        :rtype: :class:`nngeometry.object.PMatKFAC`
+        """
+        prod = dict()
+        for layer_id, (a, g) in self.data.items():
+            (a_other, g_other) = other.data[layer_id]
+            prod[layer_id] = (torch.mm(a, a_other),
+                              torch.mm(g, g_other))
+        return PMatKFAC(self.generator, data=prod)
+
 
 class PMatEKFAC(PMatAbstract):
     """
     EKFAC representation from
     *George, Laurent et al., Fast Approximate Natural Gradient Descent
     in a Kronecker-factored Eigenbasis, NIPS 2018*
 
     """
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is None:
             evecs = dict()
             diags = dict()
 
-            kfac_blocks = generator.get_kfac_blocks()
+            kfac_blocks = generator.get_kfac_blocks(examples)
             for layer_id, layer in \
                     self.generator.layer_collection.layers.items():
                 a, g = kfac_blocks[layer_id]
-                evals_a, evecs_a = torch.symeig(a, eigenvectors=True)
-                evals_g, evecs_g = torch.symeig(g, eigenvectors=True)
+                evals_a, evecs_a = torch.linalg.eigh(a)
+                evals_g, evecs_g = torch.linalg.eigh(g)
                 evecs[layer_id] = (evecs_a, evecs_g)
                 diags[layer_id] = kronecker(evals_g.view(-1, 1),
                                             evals_a.view(-1, 1))
                 del a, g, kfac_blocks[layer_id]
             self.data = (evecs, diags)
         else:
             self.data = data
@@ -537,40 +637,58 @@
     def get_dense_tensor(self, split_weight_bias=True):
         """
         - split_weight_bias (bool): if True then the parameters are ordered in
         the same way as in the dense or blockdiag representation, but it
         involves more operations. Otherwise the coefficients corresponding
         to the bias are mixed between coefficients of the weight matrix
         """
-        evecs, diags = self.data
+        _, diags = self.data
         s = self.generator.layer_collection.numel()
         M = torch.zeros((s, s), device=self.generator.get_device())
-        for layer_id, layer in self.generator.layer_collection.layers.items():
-            evecs_a, evecs_g = evecs[layer_id]
+        KFE_layers = self.get_KFE(split_weight_bias=split_weight_bias)
+        for layer_id, _ in self.generator.layer_collection.layers.items():
             diag = diags[layer_id]
             start = self.generator.layer_collection.p_pos[layer_id]
             sAG = diag.numel()
+            KFE = KFE_layers[layer_id]
+            M[start:start+sAG, start:start+sAG].add_(
+                    torch.mm(KFE, torch.mm(torch.diag(diag.view(-1)),
+                                           KFE.t())))
+        return M
+
+    def get_KFE(self, split_weight_bias=True):
+        """
+        Returns a dict index by layers, of dense eigenvectors constructed from
+        Kronecker-factored eigenvectors
+
+        - split_weight_bias (bool): if True then the parameters are ordered in
+        the same way as in the dense or blockdiag representation, but it
+        involves more operations. Otherwise the coefficients corresponding
+        to the bias are mixed between coefficients of the weight matrix
+        """
+        evecs, _ = self.data
+        KFE = dict()
+        for layer_id, _ in self.generator.layer_collection.layers.items():
+            evecs_a, evecs_g = evecs[layer_id]
+            start = self.generator.layer_collection.p_pos[layer_id]
             if split_weight_bias:
                 kronecker(evecs_g, evecs_a[:-1, :])
                 kronecker(evecs_g, evecs_a[-1:, :].contiguous())
-                KFE = torch.cat([kronecker(evecs_g, evecs_a[:-1, :]),
+                KFE[layer_id] = torch.cat([kronecker(evecs_g, evecs_a[:-1, :]),
                                  kronecker(evecs_g, evecs_a[-1:, :])], dim=0)
             else:
-                KFE = kronecker(evecs_g, evecs_a)
-            M[start:start+sAG, start:start+sAG].add_(
-                    torch.mm(KFE, torch.mm(torch.diag(diag.view(-1)),
-                                           KFE.t())))
-        return M
+                KFE[layer_id] = kronecker(evecs_g, evecs_a)
+        return KFE
 
-    def update_diag(self):
+    def update_diag(self, examples):
         """
         Will update the diagonal in the KFE (aka the approximate eigenvalues)
         using current values of the model's parameters
         """
-        self.data = (self.data[0], self.generator.get_kfe_diag(self.data[0]))
+        self.data = (self.data[0], self.generator.get_kfe_diag(self.data[0], examples))
 
     def mv(self, vs):
         vs_dict = vs.get_dict_representation()
         out_dict = dict()
         evecs, diags = self.data
         for l_id, l in self.generator.layer_collection.layers.items():
             diag = diags[l_id]
@@ -661,25 +779,29 @@
     various linear algebra operations are performed implicitely
     using efficient tricks.
 
     The computations are done exactly, meaning that there is
     no approximation involved. This is useful for networks too big
     to fit in memory.
     """
-    def __init__(self, generator):
+    def __init__(self, generator, data=None, examples=None):
         self.generator = generator
 
+        assert data is None
+
+        self.examples = examples
+
     def mv(self, v):
-        return self.generator.implicit_mv(v)
+        return self.generator.implicit_mv(v, self.examples)
 
     def vTMv(self, v):
-        return self.generator.implicit_vTMv(v)
+        return self.generator.implicit_vTMv(v, self.examples)
 
     def trace(self):
-        return self.generator.implicit_trace()
+        return self.generator.implicit_trace(self.examples)
 
     def frobenius_norm(self):
         raise NotImplementedError
 
     def get_dense_tensor(self):
         raise NotImplementedError
 
@@ -687,20 +809,22 @@
         raise NotImplementedError
 
     def get_diag(self):
         raise NotImplementedError
 
 
 class PMatLowRank(PMatAbstract):
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_jacobian()
+            self.data = generator.get_jacobian(examples)
             self.data /= self.data.size(1)**.5
 
     def vTMv(self, v):
         data_mat = self.data.view(-1, self.data.size(2))
         Av = torch.mv(data_mat, v.get_flat_representation())
         return torch.dot(Av, Av)
 
@@ -714,20 +838,19 @@
 
     def mv(self, v):
         data_mat = self.data.view(-1, self.data.size(2))
         v_flat = torch.mv(data_mat.t(),
                           torch.mv(data_mat, v.get_flat_representation()))
         return PVector(v.layer_collection, vector_repr=v_flat)
 
-    def compute_eigendecomposition(self, impl='symeig'):
-        if impl == 'symeig':
-            self.evals, V = torch.symeig(torch.mm(self.data, self.data.t()),
-                                         eigenvectors=True)
-            self.evecs = torch.mm(self.data.t(), V) / \
-                (self.evals**.5).unsqueeze(0)
+    def compute_eigendecomposition(self, impl='svd'):
+        data_mat = self.data.view(-1, self.data.size(2))
+        if impl == 'svd':
+            _, sqrt_evals, self.evecs = torch.svd(data_mat, some=True)
+            self.evals = sqrt_evals**2
         else:
             raise NotImplementedError
 
     def get_eigendecomposition(self):
         return self.evals, self.evecs
 
     def trace(self):
@@ -736,16 +859,19 @@
         return torch.trace(A)
 
     def frobenius_norm(self):
         A = torch.mm(self.data.view(-1, self.data.size(2)),
                      self.data.view(-1, self.data.size(2)).t())
         return torch.norm(A)
 
-    def solve(self, v):
-        raise NotImplementedError
+    def solve(self, b, regul=1e-8):
+        u, s, v = torch.svd(self.data.view(-1, self.data.size(2)))
+        x = torch.mv(v, torch.mv(v.t(), b.get_flat_representation()) /
+                     (s**2 + regul))
+        return PVector(b.layer_collection, vector_repr=x)
 
     def get_diag(self):
         return (self.data**2).sum(dim=(0, 1))
 
     def __rmul__(self, x):
         return PMatLowRank(generator=self.generator,
                            data=x**.5 * self.data)
@@ -753,20 +879,22 @@
 
 class PMatQuasiDiag(PMatAbstract):
     """
     Quasidiagonal approximation as decribed in Ollivier,
     Riemannian metrics for neural networks I: feedforward networks,
     Information and Inference: A Journal of the IMA, 2015
     """
-    def __init__(self, generator, data=None):
+    def __init__(self, generator, data=None, examples=None):
+        self._check_data_examples(data, examples)
+
         self.generator = generator
         if data is not None:
             self.data = data
         else:
-            self.data = generator.get_covariance_quasidiag()
+            self.data = generator.get_covariance_quasidiag(examples)
 
     def get_dense_tensor(self):
         s = self.generator.layer_collection.numel()
         device = self.generator.get_device()
         M = torch.zeros((s, s), device=device)
         for layer_id in self.generator.layer_collection.layers.keys():
             diag, cross = self.data[layer_id]
```

### Comparing `nngeometry-0.2.1/nngeometry/object/vector.py` & `nngeometry-0.3/nngeometry/object/vector.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     v_dict = dict()
     for layer_id, layer in layer_collection.layers.items():
         if layer.bias is not None:
             v_dict[layer_id] = (torch.normal(0, 1, layer.weight.size, device=device),
                                 torch.normal(0, 1, layer.bias.size, device=device))
         else:
-            v_dict[layer_id] = (torch.normal(0, 1, layer.weight.size, device=device))
+            v_dict[layer_id] = (torch.normal(0, 1, layer.weight.size, device=device),)
     return PVector(layer_collection, dict_repr=v_dict)
 
 
 def random_pvector(layer_collection, device=None):
     """
     Returns a random :class:`nngeometry.object.PVector` object using
     the structure defined by the `layer_collection` parameter, with 
@@ -87,16 +87,30 @@
         dict_repr = self.get_dict_representation()
         layer_collection = LayerCollection.from_model(model)
         l_to_m, _ = layer_collection.get_layerid_module_maps(model)
         for layer_id, layer in layer_collection.layers.items():
             mod = l_to_m[layer_id]
             if layer.bias is not None:
                 mod.bias.data.copy_(dict_repr[layer_id][1])
-            else:
-                mod.weight.data.copy_(dict_repr[layer_id][0])
+            mod.weight.data.copy_(dict_repr[layer_id][0])
+
+    def add_to_model(self, model):
+        """
+        Updates `model` parameter values by adding the current PVector
+
+        Note. This is an inplace operation
+        """
+        dict_repr = self.get_dict_representation()
+        layer_collection = LayerCollection.from_model(model)
+        l_to_m, _ = layer_collection.get_layerid_module_maps(model)
+        for layer_id, layer in layer_collection.layers.items():
+            mod = l_to_m[layer_id]
+            if layer.bias is not None:
+                mod.bias.data.add_(dict_repr[layer_id][1])
+            mod.weight.data.add_(dict_repr[layer_id][0])
 
     @staticmethod
     def from_model_grad(model):
         """
         Creates a PVector using the current values of the `.grad`
         fields of parameters of the given model
         """
@@ -198,15 +212,15 @@
         """
         Computes the Lp norm of the PVector
         """
         if self.dict_repr is not None:
             sum_p = 0
             for l_id, l in self.layer_collection.layers.items():
                 sum_p += (self.dict_repr[l_id][0]**p).sum()
-                if l.bias:
+                if l.bias is not None:
                     sum_p += (self.dict_repr[l_id][1]**p).sum()
             return sum_p ** (1/p)
         else:
             return torch.norm(self.vector_repr, p=p)
 
     def __rmul__(self, x):
         # TODO: test
@@ -262,14 +276,40 @@
             return PVector(self.layer_collection,
                            vector_repr=self.vector_repr-other.vector_repr)
         else:
             return PVector(self.layer_collection,
                            vector_repr=(self.get_flat_representation() -
                                         other.get_flat_representation()))
 
+    def dot(self, other):
+        """
+        Computes the dot product between `self` and `other`
+
+        :param other: The other `PVector`
+        """
+        if self.vector_repr is not None or other.vector_repr is not None:
+            return torch.dot(self.get_flat_representation(),
+                             other.get_flat_representation())
+        else:
+            dot_ = 0
+            for l_id, l in self.layer_collection.layers.items():
+                if l.bias is not None:
+                    dot_ += torch.dot(self.dict_repr[l_id][1],
+                                      other.dict_repr[l_id][1])
+                dot_ += torch.dot(self.dict_repr[l_id][0].view(-1),
+                                  other.dict_repr[l_id][0].view(-1))
+            return dot_
+
+    def size(self):
+        """
+        The size of the PVector, or equivalently the number of
+        parameters of the layer collection
+        """
+        return (self.layer_collection.numel(), )
+
 
 class FVector:
     """
     A vector in function space
     """
     def __init__(self, vector_repr=None):
         self.vector_repr = vector_repr
```

