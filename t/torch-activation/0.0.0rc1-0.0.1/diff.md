# Comparing `tmp/torch_activation-0.0.0rc1.tar.gz` & `tmp/torch_activation-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_activation-0.0.0rc1.tar", max compression
+gzip compressed data, was "torch_activation-0.0.1.tar", max compression
```

## Comparing `torch_activation-0.0.0rc1.tar` & `torch_activation-0.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      469 2023-05-12 06:50:06.750078 torch_activation-0.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2876 2023-05-17 00:39:29.643764 torch_activation-0.0.0rc1/README.md
--rw-r--r--   0        0        0      331 2023-05-16 09:31:55.118465 torch_activation-0.0.0rc1/torch_activation/__init__.py
--rw-r--r--   0        0        0     6628 2023-05-16 09:24:07.573583 torch_activation-0.0.0rc1/torch_activation/non_linear.py
--rw-r--r--   0        0        0     4744 2023-05-16 09:24:06.329563 torch_activation-0.0.0rc1/torch_activation/relu_family.py
--rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 torch_activation-0.0.0rc1/setup.py
--rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 torch_activation-0.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3203 2023-05-23 01:48:14.729010 torch_activation-0.0.1/README.md
+-rw-r--r--   0        0        0      449 2023-05-23 01:48:14.729010 torch_activation-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      372 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/__init__.py
+-rw-r--r--   0        0        0     3363 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/glu_family.py
+-rw-r--r--   0        0        0     6402 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/non_linear.py
+-rw-r--r--   0        0        0     4571 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/relu_family.py
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 torch_activation-0.0.1/PKG-INFO
```

### Comparing `torch_activation-0.0.0rc1/README.md` & `torch_activation-0.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,98 @@
-# PyTorch Activation Collection
-
-A collection of new, un-implemented activation functions for the PyTorch library. This project is designed for ease of use during experimentation with different activation functions (or simply for fun!). 
-
-
-## Installation
-
-```bash
-$ pip install torch_activation
-```
-
-## Usage
-
-To use the activation functions, simply import from `torch_activation`:
-
-```python
-from torch_activation import ShiLU
-
-m = ShiLU(inplace=True)
-x = torch.rand(1, 2, 2, 3)
-m(x)
-```
-
-
-## Available Functions
-
-- ShiLU [[1]](#1)
-
-  ![ShiLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/ShiLU.png "ShiLU")
-
-- DELU [[1]](#1)
-
-  ![DELU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/DELU.png "DELU")
-
-- CReLU [[2]](#2)
-
-- GCU [[3]](#3)
-
-  ![GCU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/GCU.png "GCU")
-
-- CosLU [[1]](#1)
-
-  ![CosLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/CosLU.png "CosLU")
-
-- CoLU [[4]](#4)
-
-  ![CoLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/CoLU.png "CoLU")
-
-- ReLUN [[1]](#1)
-
-  ![ReLUN Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/ReLUN.png "ReLUN")
-
-
-- SquaredReLU [[5]](#5)
-
-  ![SquaredReLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/SquaredReLU.png "SquaredReLU")
-
-- ScaledSoftSign [[1]](#1)
-
-  ![ScaledSoftSign Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/ScaledSoftSign.png "ScaledSoftSign")
-
-  
-## Future features
-* Activations:
-  * LinComb
-  * NormLinComb
-  * ReGLU
-  * GeGLU
-  * SwiGLU
-  * SinLU
-  * DReLUs
-  * ...
-* Layers:
-  * Depth-wise Convolution
-  * ...
-
-## References
-<a id="1">[1]</a>
-Pishchik, E. (2023). Trainable Activations for Image Classification. Preprints.org, 2023010463. DOI: 10.20944/preprints202301.0463.v1.
-
-<a id="2">[2]</a>
-Shang, W., Sohn, K., Almeida, D., Lee, H. (2016). Understanding and Improving Convolutional Neural Networks via Concatenated Rectified Linear Units. arXiv:1603.05201v2 (cs).
-
-<a id="3">[3]</a>
-Noel, M. M., Arunkumar, L., Trivedi, A., Dutta, P. (2023). Growing Cosine Unit: A Novel Oscillatory Activation Function That Can Speedup Training and Reduce Parameters in Convolutional Neural Networks. arXiv:2108.12943v3 (cs).
-
-<a id="4">[4]</a>
-Vagerwal, A. (2021). Deeper Learning with CoLU Activation. arXiv:2112.12078v1 (cs).
-
-<a id="5">[5]</a>
-So, D. R., Mańke, W., Liu, H., Dai, Z., Shazeer, N., Le, Q. V. (2022). Primer: Searching for Efficient Transformers for Language Modeling. arXiv:2109.08668v2 (cs)
+# PyTorch Activation Collection
+
+A collection of new, un-implemented activation functions for the PyTorch library. This project is designed for ease of use during experimentation with different activation functions (or simply for fun!). 
+
+
+## Installation
+
+```bash
+$ pip install torch-activation
+```
+
+## Usage
+
+To use the activation functions, simply import from `torch_activation`:
+
+```python
+from torch_activation import ShiLU
+
+m = ShiLU(inplace=True)
+x = torch.rand(1, 2, 2, 3)
+m(x)
+```
+
+
+## Available Functions
+
+- ShiLU [[1]](#1)
+
+  ![ShiLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/ShiLU.png "ShiLU")
+
+- DELU [[1]](#1)
+
+  ![DELU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/DELU.png "DELU")
+
+- CReLU [[2]](#2)
+
+- GCU [[3]](#3)
+
+  ![GCU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/GCU.png "GCU")
+
+- CosLU [[1]](#1)
+
+  ![CosLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/CosLU.png "CosLU")
+
+- CoLU [[4]](#4)
+
+  ![CoLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/CoLU.png "CoLU")
+
+- ReLUN [[1]](#1)
+
+  ![ReLUN Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/ReLUN.png "ReLUN")
+
+
+- SquaredReLU [[5]](#5)
+
+  ![SquaredReLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/SquaredReLU.png "SquaredReLU")
+
+- ScaledSoftSign [[1]](#1)
+
+  ![ScaledSoftSign Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/ScaledSoftSign.png "ScaledSoftSign")
+
+- ReGLU [[6]](#6)
+
+- GeGLU [[6]](#6)
+
+- SwiGLU [[6]](#6)
+
+- SeGLU
+  
+## Future features
+* Activations:
+  * LinComb
+  * NormLinComb
+  * SinLU
+  * DReLUs
+  * ...
+* Layers:
+  * Depth-wise Convolution
+  * ...
+
+## References
+<a id="1">[1]</a>
+Pishchik, E. (2023). Trainable Activations for Image Classification. Preprints.org, 2023010463. DOI: 10.20944/preprints202301.0463.v1.
+
+<a id="2">[2]</a>
+Shang, W., Sohn, K., Almeida, D., Lee, H. (2016). Understanding and Improving Convolutional Neural Networks via Concatenated Rectified Linear Units. arXiv:1603.05201v2 (cs).
+
+<a id="3">[3]</a>
+Noel, M. M., Arunkumar, L., Trivedi, A., Dutta, P. (2023). Growing Cosine Unit: A Novel Oscillatory Activation Function That Can Speedup Training and Reduce Parameters in Convolutional Neural Networks. arXiv:2108.12943v3 (cs).
+
+<a id="4">[4]</a>
+Vagerwal, A. (2021). Deeper Learning with CoLU Activation. arXiv:2112.12078v1 (cs).
+
+<a id="5">[5]</a>
+So, D. R., Mańke, W., Liu, H., Dai, Z., Shazeer, N., Le, Q. V. (2022). Primer: Searching for Efficient Transformers for Language Modeling. arXiv:2109.08668v2 (cs)
+
+<a id="6">[6]</a>
+Noam, S. (2020). GLU Variants Improve Transformer. arXiv:2002.05202v1 (cs)
```

### Comparing `torch_activation-0.0.0rc1/torch_activation/non_linear.py` & `torch_activation-0.0.1/torch_activation/non_linear.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from torch import Tensor
-
-
-class CoLU(nn.Module):
-    r"""
-    Applies the Collapsing Linear Unit activation function:
-
-    :math:`\text{CoLU}(x) = \frac{x}{1-x \mul e^{-(x+e^x)}}`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-
-    .. image:: ../images/activation_images/CoLU.png
-
-    Examples::
-
-        >>> m = nn.CoLU()
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = nn.CoLU(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-    """
-
-    def __init__(self, inplace=False):
-        super(CoLU, self).__init__()
-        self.inplace = inplace
-
-    def forward(self, x) -> Tensor:
-        if self.inplace:
-            return x.div_(1 - x * torch.exp(-1 * (x + torch.exp(x))))
-        else:
-            return x / (1 - x * torch.exp(-1 * (x + torch.exp(x))))
-
-
-class DELU(nn.Module):
-    r"""
-    Applies the DELU activation function:
-
-    :math:`\text{DELU}(x) = \begin{cases} \text{SiLU}(x), x \leqslant 0 \\x(n-1), \text{otherwise} \end{cases}`
-
-    Args:
-        n: Scaling factor for the positive part of the input. Default: 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        n: Scaling factor for the positive part of the input. Default: 1.0.
-
-    Examples:
-        >>> m = nn.DELU()
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = nn.DELU(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-    """
-
-    def __init__(self, n=1.0, inplace=False):
-        super(DELU, self).__init__()
-        self.n = torch.nn.Parameter(torch.tensor(n))
-        self.inplace = inplace
-
-    def forward(self, x) -> Tensor:
-        return self._forward_inplace(x) if self.inplace else self._forward(x)
-
-    def _forward(self, x):
-        return torch.where(x <= 0, 
-            F.silu(x), 
-            (self.n + 0.5) * x + torch.abs(torch.exp(-x) - 1))
-        
-    def _forward_inplace(self, x):
-        x[x <= 0] = F.silu(x[x <= 0])
-        x[x > 0] = (self.n + 0.5) * x[x > 0] + torch.abs(torch.exp(-x[x > 0]) - 1)
-        return x
-
-
-class GCU(nn.Module):
-    r"""
-    Applies the Growing Cosine Unit activation function:
-
-    :math:`\text{GCU}(x) = x \cos (x)`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-
-    .. image:: ../images/activation_images/GCU.png
-
-    Examples::
-
-        >>> m = nn.GCU()
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = nn.GCU(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-    """
-
-    def __init__(self, inplace=False):
-        super(GCU, self).__init__()
-        self.inplace = inplace
-
-    def forward(self, x) -> Tensor:
-        if self.inplace:            
-            return x.mul_(torch.cos(x))
-        else:
-            return x * torch.cos(x)
-
-
-class CosLU(nn.Module):
-    r"""
-    Applies the Cosine Linear Unit function:
-    
-    :math:`\text{CosLU}(x) = (x + \alpha \cdot \cos(\beta x)) \cdot \sigma(x)`
-
-    Args:
-        alpha: Scaling factor for the cosine term. Default is 1.0.
-        beta: Frequency factor for the cosine term. Default is 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-    
-    Attributes:
-        alpha: Scaling factor for the cosine term. Default is 1.0.
-        beta: Frequency factor for the cosine term. Default is 1.0.
-        
-    .. image:: ../images/activation_images/CosLU.png
-
-    Examples::
-
-        >>> m = CosLU(alpha=2.0, beta=1.0)
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = CosLU(inplace=True)
-        >>> x = torch.randn(2, 3, 4)
-        >>> m(x) 
-    """
-
-    def __init__(self, alpha=1.0, beta=1.0, inplace=False):
-        super(CosLU, self).__init__()
-        self.alpha = nn.Parameter(torch.tensor(alpha))
-        self.beta  = nn.Parameter(torch.tensor(beta))
-        self.inplace = inplace
-
-    def forward(self, x) -> Tensor:
-        return self._forward_inplace(x) if self.inplace else self._forward(x)
-
-    def _forward(self, x):
-        result = x + self.alpha * torch.cos(self.beta * x)
-        result *= torch.sigmoid(x)
-        return result
-    
-    def _forward_inplace(self, x):
-        s_x = torch.sigmoid(x)
-        x.add_(self.alpha * torch.cos(self.beta * x))
-        x.mul_(s_x)
-        del s_x
-        return x
-
-
-class ScaledSoftSign(torch.nn.Module):
-    r"""
-    Applies the ScaledSoftSign activation function:
-
-    :math:`\text{ScaledSoftSign}(x) = \frac{\alpha \mul x}{\beta + |x|}`
-
-    Args:
-        alpha: The initial value of the alpha parameter.
-        beta: The initial value of the beta parameter.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-    
-    Attributes:
-        alpha (nn.Parameter): The alpha scaling parameter.
-        beta (nn.Parameter): The beta scaling parameter.
-        
-    .. image:: ../images/activation_images/ScaledSoftSign.png
-
-    Examples:
-        >>> m = ScaledSoftSign(alpha=0.5, beta=1.0)
-        >>> x = torch.randn(2, 3)
-        >>> output = m(x)
-        
-        >>> m = ScaledSoftSign(inplace=True)
-        >>> x = torch.randn(2, 3)
-        >>> m(x)
-    """
-    def __init__(self, alpha=1.0, beta=1.0):
-        super(ScaledSoftSign, self).__init__()
-        
-        self.alpha = torch.nn.Parameter(torch.tensor(alpha))
-        self.beta = torch.nn.Parameter(torch.tensor(beta))
-
-    def forward(self, x) -> Tensor:
-        abs_x = x.abs()
-        alpha_x = self.alpha * x
-        denom = self.beta + abs_x
-        result = alpha_x / denom
-        return result
-
-
-if __name__ == "__main__":
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from torch import Tensor
+
+
+class CoLU(nn.Module):
+    r"""
+    Applies the Collapsing Linear Unit activation function:
+
+    :math:`\text{CoLU}(x) = \frac{x}{1-x \mul e^{-(x+e^x)}}`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+
+    .. image:: ../images/activation_images/CoLU.png
+
+    Examples::
+
+        >>> m = nn.CoLU()
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = nn.CoLU(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+    """
+
+    def __init__(self, inplace=False):
+        super(CoLU, self).__init__()
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:
+            return x.div_(1 - x * torch.exp(-1 * (x + torch.exp(x))))
+        else:
+            return x / (1 - x * torch.exp(-1 * (x + torch.exp(x))))
+
+
+class DELU(nn.Module):
+    r"""
+    Applies the DELU activation function:
+
+    :math:`\text{DELU}(x) = \begin{cases} \text{SiLU}(x), x \leqslant 0 \\x(n-1), \text{otherwise} \end{cases}`
+
+    Args:
+        n: Scaling factor for the positive part of the input. Default: 1.0.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    Attributes:
+        n: Scaling factor for the positive part of the input. Default: 1.0.
+
+    Examples:
+        >>> m = nn.DELU()
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = nn.DELU(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+    """
+
+    def __init__(self, n=1.0, inplace=False):
+        super(DELU, self).__init__()
+        self.n = torch.nn.Parameter(torch.tensor(n))
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        return self._forward_inplace(x) if self.inplace else self._forward(x)
+
+    def _forward(self, x):
+        return torch.where(x <= 0, 
+            F.silu(x), 
+            (self.n + 0.5) * x + torch.abs(torch.exp(-x) - 1))
+        
+    def _forward_inplace(self, x):
+        x[x <= 0] = F.silu(x[x <= 0])
+        x[x > 0] = (self.n + 0.5) * x[x > 0] + torch.abs(torch.exp(-x[x > 0]) - 1)
+        return x
+
+
+class GCU(nn.Module):
+    r"""
+    Applies the Growing Cosine Unit activation function:
+
+    :math:`\text{GCU}(x) = x \cos (x)`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+
+    .. image:: ../images/activation_images/GCU.png
+
+    Examples::
+
+        >>> m = nn.GCU()
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = nn.GCU(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+    """
+
+    def __init__(self, inplace=False):
+        super(GCU, self).__init__()
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:            
+            return x.mul_(torch.cos(x))
+        else:
+            return x * torch.cos(x)
+
+
+class CosLU(nn.Module):
+    r"""
+    Applies the Cosine Linear Unit function:
+    
+    :math:`\text{CosLU}(x) = (x + \alpha \cdot \cos(\beta x)) \cdot \sigma(x)`
+
+    Args:
+        alpha: Scaling factor for the cosine term. Default is 1.0.
+        beta: Frequency factor for the cosine term. Default is 1.0.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+    
+    Attributes:
+        alpha: Scaling factor for the cosine term. Default is 1.0.
+        beta: Frequency factor for the cosine term. Default is 1.0.
+        
+    .. image:: ../images/activation_images/CosLU.png
+
+    Examples::
+
+        >>> m = CosLU(alpha=2.0, beta=1.0)
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = CosLU(inplace=True)
+        >>> x = torch.randn(2, 3, 4)
+        >>> m(x) 
+    """
+
+    def __init__(self, alpha=1.0, beta=1.0, inplace=False):
+        super(CosLU, self).__init__()
+        self.alpha = nn.Parameter(torch.tensor(alpha))
+        self.beta  = nn.Parameter(torch.tensor(beta))
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        return self._forward_inplace(x) if self.inplace else self._forward(x)
+
+    def _forward(self, x):
+        result = x + self.alpha * torch.cos(self.beta * x)
+        result *= torch.sigmoid(x)
+        return result
+    
+    def _forward_inplace(self, x):
+        s_x = torch.sigmoid(x)
+        x.add_(self.alpha * torch.cos(self.beta * x))
+        x.mul_(s_x)
+        del s_x
+        return x
+
+
+class ScaledSoftSign(torch.nn.Module):
+    r"""
+    Applies the ScaledSoftSign activation function:
+
+    :math:`\text{ScaledSoftSign}(x) = \frac{\alpha \mul x}{\beta + |x|}`
+
+    Args:
+        alpha: The initial value of the alpha parameter.
+        beta: The initial value of the beta parameter.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+    
+    Attributes:
+        alpha (nn.Parameter): The alpha scaling parameter.
+        beta (nn.Parameter): The beta scaling parameter.
+        
+    .. image:: ../images/activation_images/ScaledSoftSign.png
+
+    Examples:
+        >>> m = ScaledSoftSign(alpha=0.5, beta=1.0)
+        >>> x = torch.randn(2, 3)
+        >>> output = m(x)
+        
+        >>> m = ScaledSoftSign(inplace=True)
+        >>> x = torch.randn(2, 3)
+        >>> m(x)
+    """
+    def __init__(self, alpha=1.0, beta=1.0):
+        super(ScaledSoftSign, self).__init__()
+        
+        self.alpha = torch.nn.Parameter(torch.tensor(alpha))
+        self.beta = torch.nn.Parameter(torch.tensor(beta))
+
+    def forward(self, x) -> Tensor:
+        abs_x = x.abs()
+        alpha_x = self.alpha * x
+        denom = self.beta + abs_x
+        result = alpha_x / denom
+        return result
+
+
+if __name__ == "__main__":
     pass
```

### Comparing `torch_activation-0.0.0rc1/torch_activation/relu_family.py` & `torch_activation-0.0.1/torch_activation/relu_family.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from torch import Tensor
-
-
-class ShiLU(nn.Module):
-    r"""
-    Applies the ShiLU activation function:
-
-    :math:`\text{ShiLU}(x) = \alpha * \max(0,x) + \beta`
-
-    Args:
-        alpha : Scaling factor for the positive part of the input. Default: 1.0.
-        beta : Bias term added to the output. Default: 0.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        alpha : Scaling factor for the positive part of the input. Default: 1.0.
-        beta : Bias term added to the output. Default: 0.0.
-
-    .. image:: ../images/activation_images/ShiLU.png
-
-    Examples::
-    
-        >>> m = ShiLU(alpha=2.0, beta=1.0)
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = ShiLU(inplace=True)
-        >>> x = torch.randn(2, 3, 4)
-        >>> m(x)
-    """
-
-    def __init__(self, alpha=1.0, beta=0.0, inplace=False):
-        super().__init__()
-        self.alpha = nn.Parameter(torch.tensor(alpha))
-        self.beta  = nn.Parameter(torch.tensor(beta))
-        self.inplace = inplace
-
-    def forward(self, x):
-        if self.inplace:
-            F.relu_(x)
-            x.mul_(self.alpha)
-            x.add_(self.beta)
-            return x
-        else:    
-            return self.alpha * F.relu(x) + self.beta
-        
-
-class CReLU(nn.Module):
-    r"""
-    Applies the Concatenated Rectified Linear Unit activation function.
-
-    :math:`\text{CReLU}(x) = \max(0,x) \oplus \max(0,-x)`
-
-    Args:
-        dim: Dimension along which to concatenate in the output tensor. Default: 1
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*, C, *)` where :math:`*` means any number of additional dimensions
-        - Output: :math:`(*, 2C, *)`
-
-    .. image:: ../images/activation_images/CReLU.png
-
-    Examples::
-
-        >>> m = nn.CReLU()
-        >>> x = torch.randn(2, 3)
-        >>> output = m(x)
-        
-        >>> m = CReLU(inplace=True)
-        >>> x = torch.randn(2, 3, 4)
-        >>> m(x)
-    """
-    
-    
-    def __init__(self, dim=0):
-        super(CReLU, self).__init__()
-        self.dim = dim
-
-    def forward(self, x):
-        return F.relu(torch.cat((x, -x), dim=self.dim))
-        
-        
-class ReLUN(nn.Module):
-    r"""Applies the element-wise function:
-
-    :math:`\text{ReLUN}(x) = \min(\max(0,x), n)`
-
-    Args:
-        n: Upper bound for the function's output. Default is 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        n: Upper bound for the function's output. Default is 1.0.
-        
-    .. image:: ../images/activation_images/ReLUN.png
-
-    Examples::
-
-        >>> m = nn.ReLUN(n=6.0) # ReLU6
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-        
-        >>> m = nn.ReLUN(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-
-    """
-    def __init__(self, n=1.0, inplace=False):
-        super(ReLUN, self).__init__()
-        self.n = nn.Parameter(torch.tensor(n))
-        self.inplace = inplace
-
-    def forward(self, x):
-        if self.inplace:
-            x.clamp_max_(self.n.data)
-            x.relu_()
-            return x
-        else:
-            return torch.clamp(x, 0, self.n.data)
-        
-        
-class SquaredReLU(nn.Module):
-    r"""
-    Applies the element-wise function:
-
-    :math:`\text{SquaredReLU}(x) = \text{ReLU}(x)^2`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    .. image:: ../images/activation_images/SquaredReLU.png
-
-    Examples::
-
-        >>> m = nn.SquaredReLU()
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = nn.SquaredReLU(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-    """
-    
-    
-    def __init__(self, inplace=False):
-        super().__init__()
-        self.inplace = inplace
-
-    def forward(self, x) -> Tensor:
-        if self.inplace:
-            return F.relu_(x).pow_(2)
-        else:
-            return F.relu(x).pow(2)
-    
-    
-if __name__ == '__main__':
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from torch import Tensor
+
+
+class ShiLU(nn.Module):
+    r"""
+    Applies the ShiLU activation function:
+
+    :math:`\text{ShiLU}(x) = \alpha * \max(0,x) + \beta`
+
+    Args:
+        alpha : Scaling factor for the positive part of the input. Default: 1.0.
+        beta : Bias term added to the output. Default: 0.0.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    Attributes:
+        alpha : Scaling factor for the positive part of the input. Default: 1.0.
+        beta : Bias term added to the output. Default: 0.0.
+
+    .. image:: ../images/activation_images/ShiLU.png
+
+    Examples::
+    
+        >>> m = ShiLU(alpha=2.0, beta=1.0)
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = ShiLU(inplace=True)
+        >>> x = torch.randn(2, 3, 4)
+        >>> m(x)
+    """
+
+    def __init__(self, alpha=1.0, beta=0.0, inplace=False):
+        super().__init__()
+        self.alpha = nn.Parameter(torch.tensor(alpha))
+        self.beta  = nn.Parameter(torch.tensor(beta))
+        self.inplace = inplace
+
+    def forward(self, x):
+        if self.inplace:
+            F.relu_(x)
+            x.mul_(self.alpha)
+            x.add_(self.beta)
+            return x
+        else:    
+            return self.alpha * F.relu(x) + self.beta
+        
+
+class CReLU(nn.Module):
+    r"""
+    Applies the Concatenated Rectified Linear Unit activation function.
+
+    :math:`\text{CReLU}(x) = \max(0,x) \oplus \max(0,-x)`
+
+    Args:
+        dim: Dimension along which to concatenate in the output tensor. Default: 1
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*, C, *)` where :math:`*` means any number of additional dimensions
+        - Output: :math:`(*, 2C, *)`
+
+    .. image:: ../images/activation_images/CReLU.png
+
+    Examples::
+
+        >>> m = nn.CReLU()
+        >>> x = torch.randn(2, 3)
+        >>> output = m(x)
+        
+        >>> m = CReLU(inplace=True)
+        >>> x = torch.randn(2, 3, 4)
+        >>> m(x)
+    """
+    
+    
+    def __init__(self, dim=0):
+        super(CReLU, self).__init__()
+        self.dim = dim
+
+    def forward(self, x):
+        return F.relu(torch.cat((x, -x), dim=self.dim))
+        
+        
+class ReLUN(nn.Module):
+    r"""Applies the element-wise function:
+
+    :math:`\text{ReLUN}(x) = \min(\max(0,x), n)`
+
+    Args:
+        n: Upper bound for the function's output. Default is 1.0.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    Attributes:
+        n: Upper bound for the function's output. Default is 1.0.
+        
+    .. image:: ../images/activation_images/ReLUN.png
+
+    Examples::
+
+        >>> m = nn.ReLUN(n=6.0) # ReLU6
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+        
+        >>> m = nn.ReLUN(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+
+    """
+    def __init__(self, n=1.0, inplace=False):
+        super(ReLUN, self).__init__()
+        self.n = nn.Parameter(torch.tensor(n))
+        self.inplace = inplace
+
+    def forward(self, x):
+        if self.inplace:
+            x.clamp_max_(self.n.data)
+            x.relu_()
+            return x
+        else:
+            return torch.clamp(x, 0, self.n.data)
+        
+        
+class SquaredReLU(nn.Module):
+    r"""
+    Applies the element-wise function:
+
+    :math:`\text{SquaredReLU}(x) = \text{ReLU}(x)^2`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    .. image:: ../images/activation_images/SquaredReLU.png
+
+    Examples::
+
+        >>> m = nn.SquaredReLU()
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = nn.SquaredReLU(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+    """
+    
+    
+    def __init__(self, inplace=False):
+        super().__init__()
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:
+            return F.relu_(x).pow_(2)
+        else:
+            return F.relu(x).pow(2)
+    
+    
+if __name__ == '__main__':
     pass
```

### Comparing `torch_activation-0.0.0rc1/setup.py` & `torch_activation-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: torch-activation
+Version: 0.0.1
+Summary: A library of new activation function implement in PyTorch to save time in experiment and have fun
+License: MIT
+Author: Alan Huynh
+Author-email: hdmquan@outlook.com
+Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: torch (>=1.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['torch_activation']
+# PyTorch Activation Collection
 
-package_data = \
-{'': ['*']}
+A collection of new, un-implemented activation functions for the PyTorch library. This project is designed for ease of use during experimentation with different activation functions (or simply for fun!). 
 
-install_requires = \
-['torch>=1.0.0']
-
-setup_kwargs = {
-    'name': 'torch-activation',
-    'version': '0.0.0rc1',
-    'description': 'A library of new activation function implement in PyTorch to save time in experiment and have fun',
-    'long_description': '# PyTorch Activation Collection\n\nA collection of new, un-implemented activation functions for the PyTorch library. This project is designed for ease of use during experimentation with different activation functions (or simply for fun!). \n\n\n## Installation\n\n```bash\n$ pip install torch_activation\n```\n\n## Usage\n\nTo use the activation functions, simply import from `torch_activation`:\n\n```python\nfrom torch_activation import ShiLU\n\nm = ShiLU(inplace=True)\nx = torch.rand(1, 2, 2, 3)\nm(x)\n```\n\n\n## Available Functions\n\n- ShiLU [[1]](#1)\n\n  ![ShiLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/ShiLU.png "ShiLU")\n\n- DELU [[1]](#1)\n\n  ![DELU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/DELU.png "DELU")\n\n- CReLU [[2]](#2)\n\n- GCU [[3]](#3)\n\n  ![GCU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/GCU.png "GCU")\n\n- CosLU [[1]](#1)\n\n  ![CosLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/CosLU.png "CosLU")\n\n- CoLU [[4]](#4)\n\n  ![CoLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/CoLU.png "CoLU")\n\n- ReLUN [[1]](#1)\n\n  ![ReLUN Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/ReLUN.png "ReLUN")\n\n\n- SquaredReLU [[5]](#5)\n\n  ![SquaredReLU Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/SquaredReLU.png "SquaredReLU")\n\n- ScaledSoftSign [[1]](#1)\n\n  ![ScaledSoftSign Activation](https://github.com/alan191006/torch_activation/blob/main/images/activation_images/ScaledSoftSign.png "ScaledSoftSign")\n\n  \n## Future features\n* Activations:\n  * LinComb\n  * NormLinComb\n  * ReGLU\n  * GeGLU\n  * SwiGLU\n  * SinLU\n  * DReLUs\n  * ...\n* Layers:\n  * Depth-wise Convolution\n  * ...\n\n## References\n<a id="1">[1]</a>\nPishchik, E. (2023). Trainable Activations for Image Classification. Preprints.org, 2023010463. DOI: 10.20944/preprints202301.0463.v1.\n\n<a id="2">[2]</a>\nShang, W., Sohn, K., Almeida, D., Lee, H. (2016). Understanding and Improving Convolutional Neural Networks via Concatenated Rectified Linear Units. arXiv:1603.05201v2 (cs).\n\n<a id="3">[3]</a>\nNoel, M. M., Arunkumar, L., Trivedi, A., Dutta, P. (2023). Growing Cosine Unit: A Novel Oscillatory Activation Function That Can Speedup Training and Reduce Parameters in Convolutional Neural Networks. arXiv:2108.12943v3 (cs).\n\n<a id="4">[4]</a>\nVagerwal, A. (2021). Deeper Learning with CoLU Activation. arXiv:2112.12078v1 (cs).\n\n<a id="5">[5]</a>\nSo, D. R., Mańke, W., Liu, H., Dai, Z., Shazeer, N., Le, Q. V. (2022). Primer: Searching for Efficient Transformers for Language Modeling. arXiv:2109.08668v2 (cs)',
-    'author': 'Alan Huynh',
-    'author_email': 'hdmquan@outlook.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6',
-}
 
+## Installation
 
-setup(**setup_kwargs)
+```bash
+$ pip install torch-activation
+```
+
+## Usage
+
+To use the activation functions, simply import from `torch_activation`:
+
+```python
+from torch_activation import ShiLU
+
+m = ShiLU(inplace=True)
+x = torch.rand(1, 2, 2, 3)
+m(x)
+```
+
+
+## Available Functions
+
+- ShiLU [[1]](#1)
+
+  ![ShiLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/ShiLU.png "ShiLU")
+
+- DELU [[1]](#1)
+
+  ![DELU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/DELU.png "DELU")
+
+- CReLU [[2]](#2)
+
+- GCU [[3]](#3)
+
+  ![GCU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/GCU.png "GCU")
+
+- CosLU [[1]](#1)
+
+  ![CosLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/CosLU.png "CosLU")
+
+- CoLU [[4]](#4)
+
+  ![CoLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/CoLU.png "CoLU")
+
+- ReLUN [[1]](#1)
+
+  ![ReLUN Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/ReLUN.png "ReLUN")
+
+
+- SquaredReLU [[5]](#5)
+
+  ![SquaredReLU Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/SquaredReLU.png "SquaredReLU")
+
+- ScaledSoftSign [[1]](#1)
+
+  ![ScaledSoftSign Activation](https://github.com/alan191006/torch_activation/blob/63d8db5d4a2ef19e382fc8175bf47b0a5173df3e/images/activation_images/ScaledSoftSign.png "ScaledSoftSign")
+
+- ReGLU [[6]](#6)
+
+- GeGLU [[6]](#6)
+
+- SwiGLU [[6]](#6)
+
+- SeGLU
+  
+## Future features
+* Activations:
+  * LinComb
+  * NormLinComb
+  * SinLU
+  * DReLUs
+  * ...
+* Layers:
+  * Depth-wise Convolution
+  * ...
+
+## References
+<a id="1">[1]</a>
+Pishchik, E. (2023). Trainable Activations for Image Classification. Preprints.org, 2023010463. DOI: 10.20944/preprints202301.0463.v1.
+
+<a id="2">[2]</a>
+Shang, W., Sohn, K., Almeida, D., Lee, H. (2016). Understanding and Improving Convolutional Neural Networks via Concatenated Rectified Linear Units. arXiv:1603.05201v2 (cs).
+
+<a id="3">[3]</a>
+Noel, M. M., Arunkumar, L., Trivedi, A., Dutta, P. (2023). Growing Cosine Unit: A Novel Oscillatory Activation Function That Can Speedup Training and Reduce Parameters in Convolutional Neural Networks. arXiv:2108.12943v3 (cs).
+
+<a id="4">[4]</a>
+Vagerwal, A. (2021). Deeper Learning with CoLU Activation. arXiv:2112.12078v1 (cs).
+
+<a id="5">[5]</a>
+So, D. R., Mańke, W., Liu, H., Dai, Z., Shazeer, N., Le, Q. V. (2022). Primer: Searching for Efficient Transformers for Language Modeling. arXiv:2109.08668v2 (cs)
+
+<a id="6">[6]</a>
+Noam, S. (2020). GLU Variants Improve Transformer. arXiv:2002.05202v1 (cs)
```

