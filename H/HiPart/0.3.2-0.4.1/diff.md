# Comparing `tmp/HiPart-0.3.2.tar.gz` & `tmp/HiPart-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiPart-0.3.2.tar", last modified: Tue Apr 25 14:00:39 2023, max compression
+gzip compressed data, was "HiPart-0.4.1.tar", last modified: Tue May 23 12:53:46 2023, max compression
```

## Comparing `HiPart-0.3.2.tar` & `HiPart-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 14:00:22.000000 HiPart-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:00:22.000000 HiPart-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-25 14:00:39.615010 HiPart-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-25 14:00:22.000000 HiPart-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 14:00:23.000000 HiPart-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:00:39.615010 HiPart-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-25 14:00:23.000000 HiPart-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.611010 HiPart-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/src/HiPart/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23326 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/__utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/src/HiPart/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/assets/int_viz.css
--rw-r--r--   0 runner    (1001) docker     (123)    72232 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/interactive_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/src/HiPart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-04-25 14:00:23.000000 HiPart-0.3.2/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.335885 HiPart-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 12:53:24.000000 HiPart-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 12:53:24.000000 HiPart-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-23 12:53:46.331885 HiPart-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-23 12:53:24.000000 HiPart-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 12:53:24.000000 HiPart-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:53:46.335885 HiPart-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-23 12:53:24.000000 HiPart-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/HiPart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31954 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/__utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/HiPart/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/assets/int_viz.css
+-rw-r--r--   0 runner    (1001) docker     (123)    88495 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/interactive_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/HiPart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-05-23 12:53:24.000000 HiPart-0.4.1/tests/test_package.py
```

### Comparing `HiPart-0.3.2/LICENSE` & `HiPart-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.2/PKG-INFO` & `HiPart-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.3.2
+Version: 0.4.1
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
 Project-URL: Documentation, https://hipart.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/panagiotisanagnostou/HiPart/
```

### Comparing `HiPart-0.3.2/README.md` & `HiPart-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.2/setup.py` & `HiPart-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "0.3.2"
+__version__ = "0.4.1"
 
 setuptools.setup(
     name="HiPart",
     version=__version__,
     url="https://github.com/panagiotisanagnostou/HiPart",
     author="Panagiotis Anagnostou",
     author_email="panagno@uth.gr",
```

### Comparing `HiPart-0.3.2/src/HiPart/__init__.py` & `HiPart-0.4.1/src/HiPart/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 
 """
 
 from KDEpy.NaiveKDE import NaiveKDE
 from KDEpy.TreeKDE import TreeKDE
 from KDEpy.FFTKDE import FFTKDE
 
-__version__ = "0.3.2"
+__version__ = "0.4.1"
 __author__ = "Panagiotis Anagnostou"
 
 TreeKDE = TreeKDE
 NaiveKDE = NaiveKDE
 FFTKDE = FFTKDE
```

### Comparing `HiPart-0.3.2/src/HiPart/__utility_functions.py` & `HiPart-0.4.1/src/HiPart/__utility_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,28 +17,48 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
 Utility functions of the HiPart package.
 
 @author: Panagiotis Anagnostou
+@author: Nicos Pavlidis
 """
 
 import copy
 import math
 import matplotlib
 import numpy as np
 import statsmodels.api as sm
 import warnings
 
 from KDEpy import FFTKDE
+from scipy import stats as st
+from scipy.optimize import Bounds, minimize, NonlinearConstraint, SR1
 from sklearn.manifold import TSNE
 from sklearn.decomposition import PCA, KernelPCA, FastICA
 
 
+def band_const(d):
+    """
+    Calculate the data bandwidth based in their dimensions.
+
+    Parameters
+    ----------
+    d : int
+        Number of dimensions
+
+    Returns
+    -------
+    float
+        Bandwidth
+    """
+    return 0.45 / np.power(d, 0.2)
+
+
 def execute_decomposition_method(
         data_matrix,
         decomposition_method,
         two_dimentions,
         decomposition_args,
 ):
     """
@@ -101,14 +121,284 @@
             + decomposition_method
             + ") is not supported!"
         )
 
     return two_dimensions
 
 
+def initialize_b(x0, X, depth_init=True):
+    """
+    Initialize the b parameter of the MDH algorithm. The initialization is done
+    by finding the minimum density point of the projection of the data matrix
+    onto the vector v.
+
+    Parameters
+    ----------
+    x0 : numpy.ndarray (1D)
+        The vector v in the first d position of x0 vector and the point b in the
+        last one. The vector v is the projection direction of the data matrix
+        and b is a random estimation of the minimum density point.
+    X : numpy.ndarray (2D)
+        The data matrix.
+    depth_init : bool (default=True)
+        If (True) the b parameter is initialized by finding the maximum depth of
+        the curve created by the projection of the data matrix onto the vector
+        v. If (False) the b parameter is initialized by finding the lowest local
+        minimum density point of the projection of the data matrix onto the
+        vector v.
+
+    Returns
+    -------
+    b : float
+        The initialized b parameter on the local minimum density point of the
+        projection of the data matrix onto the vector v.
+
+    """
+    v = x0[:-1] / np.linalg.norm(x0[:-1])
+    xv = np.sort(np.dot(X, v))
+    # Bandwidth calculation
+    h = np.std(xv) * band_const(X.shape[0])
+
+    # The unitization of vector v produces a vector field with nans due to the norm
+    try:
+        x_ticks, y = FFTKDE(kernel="gaussian", bw=h).fit(xv).evaluate()
+    except ValueError:
+        return np.array([])
+
+    # find all local maxima of the projection's density
+    maxima = np.where(np.diff(1 * (np.diff(y) > 0)) == -1)[0]
+
+    # RuntimeErrors are raised if there are no local maxima this is not possibl
+    # by the definition of the KDE.
+    if len(maxima) == 0:
+        raise RuntimeError("MDH: no local maximum: This shouldn't be possible!")
+    # If there is only one maximum, then the distribution is uni-modal and there
+    # is no need for further searching for a local minimum.
+    elif len(maxima) == 1:
+        warnings.warn(
+            "MDH: uni-modal distribution there is no need for further processing!")
+        return np.array([])
+
+    # locations of maxima in original y array
+    # maxima += 1  # #$$# den exei shmasia an einai maxima h maxima+1 kanonika
+    # #$$# tha prepei an einai sthn mesh outos h allos
+
+    if depth_init:
+        # find minima between every pair of peaks
+        depth = np.inf
+        p = None
+        for i in np.arange(len(maxima) - 1):
+            pos = maxima[i] + np.argmin(y[maxima[i]:maxima[i + 1]])
+            # inverse of depth (to avoid numerical difficulties)
+            tmp_depth = np.amin(
+                [np.amax(y[maxima[:i + 1]]), np.amax(y[maxima[i + 1:]])]) - y[
+                            pos]
+            # No divisions by zero
+            if tmp_depth:
+                d = y[pos] / tmp_depth
+            else:
+                continue
+
+            # Find the minimum depth
+            if d < depth:
+                depth = d
+                p = pos
+
+        # Return, if exists, the location of the minimum density point of the projection
+        if p:
+            return x_ticks[p]
+        else:
+            return None
+
+    else:
+        # Find the lowest minimum between any peaks
+        pos = maxima[0] + np.argmin(y[maxima[0]:maxima[-1] + 1])
+        return x_ticks[pos]
+
+
+def md_sqp(x0, X, k):
+    """
+    MDH through SQP in Python
+
+    Parameters
+    ----------
+    x0 : numpy.ndarray, shape (d,)
+        Initial point (v,b) for optimisation algorithm .The vector v is the
+        projection direction of the data matrix and b is a random estimation of
+        the minimum density point.
+    X : ndarray, shape (n,d)
+        N times D Input data matrix. Must be centred
+    k : float
+        Range parameter
+
+    Returns
+    -------
+    res : OptimizeResult
+        Output from the minimizer.
+    depth : float
+        The depth of the minimum density point of the projection of the data.
+
+    """
+
+    # I need this to avoid division by zero in the Jacobian
+    # kern = np.sqrt(np.finfo("float").eps)
+
+    ub = np.ones(len(x0))
+    lb = np.full(len(x0), -1, dtype=float)
+    lb[0] = 0
+
+    if k == 0:
+        # pad last entry with a zero
+        def Fx(x):
+            return fx(np.append(x, 0), X)
+
+        # remove last derivative
+        def JacF(x):
+            return (dKdeDvb(np.append(x, 0), X))[:-1]
+
+        def cons_f(x):
+            return np.sum(x ** 2)
+
+        def cons_J(x):
+            return 2 * x
+
+        def cons_H(x, v):
+            return v[0] * 2 * np.eye(len(x))
+    else:
+        def Fx(x):
+            return fx(x, X)
+
+        def JacF(x):
+            return dKdeDvb(x, X)
+
+        # l2_norm = 1 constraint
+        def cons_f(x):
+            return np.sum(x[:-1] ** 2)
+
+        def cons_J(x):
+            return np.append(2 * x[:-1], 0)
+
+        def cons_H(x, v):
+            return v[0] * 2 * np.diag(
+                np.append(np.ones(len(x) - 1), 0))
+
+        ub[-1] = k
+        lb[-1] = -k
+
+    nlc = NonlinearConstraint(cons_f, 1, 1, jac=cons_J, hess=cons_H)
+
+    x0 = x0 if x0[0] > 0 else -x0
+    res = minimize(
+        Fx, x0,
+        method="trust-constr",
+        jac=JacF,
+        hess=SR1(),
+        constraints=nlc,
+        options={"verbose": 0},
+        bounds=Bounds(lb, ub),
+    )
+
+    if res:
+        return res, Fx(res.x)
+    else:
+        return res, None
+
+
+def fx(xcur, X):
+    """
+    Evaluate the 1D KDE at xcur[-1] after projecting the data matrix X onto the
+    unit-vector xcur[:-1].
+
+    Parameters
+    ----------
+    xcur: numpy.ndarray, shape (d,)
+        Point (v,b). The vector v is the projection direction of the data matrix
+        X and b is a random estimation of the minimum density point.
+    X: numpy.ndarray, shape (n,d)
+        N times D Input data matrix.
+
+    Returns
+    -------
+    float
+        The value of the 1D KDE at b after projecting the data matrix X onto the
+        unit-vector v.
+
+    """
+    # evaluate 1D kde at xcur[-1] after projecting onto unit-vector xcur[:-1]
+    v = xcur[:-1]
+    b = xcur[-1]
+
+    # compute projections
+    xv = np.dot(X, v)
+    band = np.std(xv) * band_const(len(xv))
+
+    return np.mean(st.norm.pdf(xv, b, band))
+
+
+def dKdeDvb(xcur, X):
+    """
+    Evaluate the derivative of the 1D KDE at v after projecting the data
+    matrix X onto the unit-vector b.
+
+    Parameters
+    ----------
+    xcur : numpy.ndarray, shape (d,)
+        Point (v,b). The vector v (xcur[:-1]) is the projection direction of the
+        data matrix X and b (xcur[-1]) is a random estimation of the minimum
+        density point.
+    X : numpy.ndarray, shape (n,d)
+        N times D Input data matrix.
+
+    Returns
+    -------
+    numpy.ndarray, shape (d,)
+        The derivative of the 1D KDE at v after projecting the data matrix X.
+
+    """
+
+    v = xcur[:-1]
+    b = xcur[-1]
+
+    # compute projection of X onto v
+    proj = np.dot(X, v)
+    N = proj.shape[0]
+    bn = band_const(N)
+
+    # Bandwidth calculation
+    h = np.std(proj) * bn
+
+    # ==========================================================================
+    # Derivative of fx w.r.t. projected points and bandwidth
+    DgF = np.empty(N + 1, dtype=float)
+    # first N entries are derivatives w.r.t. each projected point
+    kde = st.norm.pdf(proj, b, h)
+    DgF[:-1] = kde * (b - proj) / (h * h * N)
+    # derivative w.r.t. bandwidth
+    DgF[-1] = -np.mean(kde) / h + np.mean(kde * (np.power((b - proj), 2))) / (
+            h * h * h)
+
+    # ==========================================================================
+    # Derivative of g = (p_1,p_2, ... p_N,h) w.r.t. full-dimensional projection vector!
+    # Data is CENTRED and X stores observations in rows: Thoroughly debugged
+    # get std of projected data
+    dhdv = (bn ** 2) / (h * (N - 1))
+
+    # last parenthesis: De-means all columns of X
+    last_row = dhdv * (proj @ X)
+    DvG = np.vstack((X, last_row))
+
+    # ==========================================================================
+    # derivative of fx w.r.t to xcur = (v,b)
+    out = np.empty(len(xcur), dtype=float)
+    out[:-1] = DgF @ DvG
+    out[-1] = np.sum((proj - b) * kde) / (h * h * len(proj))
+
+    return out
+
+
 def center_data(data):
     """
     Center the data on all its dimensions (subtract the mean of each variable,
     from each variable).
 
     Parameters
     ----------
@@ -230,15 +520,15 @@
     scatter.set_yticks([])
     scatter.grid()
     scatter.xaxis.grid(which="minor")
 
     if scaler is None:
         hist.plot(s, e)
     else:
-        hist.plot(s, e*(PP.shape[0]/scaler))
+        hist.plot(s, e * (PP.shape[0] / scaler))
     hist.axvline(x=splitPoint, color="red", lw=1)
     hist.set_xticks([])
     hist.set_yticks([])
     hist.grid()
     hist.autoscale_view()
 
 
@@ -398,41 +688,41 @@
     sub_grid_size = 2 if with_marginal else 1
 
     # Change the last row of the visualization to have the subplot always in
     # the middle of the plot
     if curRow != math.ceil(splits / rows) - 1:
         row_from = curRow * num_of_subgrid_elements
         row_to = (
-            (curRow * num_of_subgrid_elements) + num_of_subgrid_elements
+                (curRow * num_of_subgrid_elements) + num_of_subgrid_elements
         )
         col_from = curCol * num_of_subgrid_elements
         col_to = (curCol * num_of_subgrid_elements) + num_of_subgrid_elements
     else:
         if splits % rows == 0:
             row_from = curRow * num_of_subgrid_elements
             row_to = (
-                (curRow * num_of_subgrid_elements) + num_of_subgrid_elements
+                    (curRow * num_of_subgrid_elements) + num_of_subgrid_elements
             )
             col_from = curCol * num_of_subgrid_elements
             col_to = (
-                (curCol * num_of_subgrid_elements) + num_of_subgrid_elements
+                    (curCol * num_of_subgrid_elements) + num_of_subgrid_elements
             )
 
         elif splits % rows != 0:
             position_corection = (rows - 1) / (splits % rows) * sub_grid_size
             row_from = curRow * num_of_subgrid_elements
             row_to = (
-                (curRow * num_of_subgrid_elements) + num_of_subgrid_elements
+                    (curRow * num_of_subgrid_elements) + num_of_subgrid_elements
             )
             col_from = (
                 int((curCol * num_of_subgrid_elements) + position_corection)
             )
             col_to = (
-                int((curCol * num_of_subgrid_elements) + position_corection)
-                + num_of_subgrid_elements
+                    int((curCol * num_of_subgrid_elements) + position_corection)
+                    + num_of_subgrid_elements
             )
 
     return row_from, row_to, col_from, col_to
 
 
 def _get_node_depth(path_to_leaves, i):
     """
@@ -525,23 +815,25 @@
                 # a new node on the dendrogram tree
                 children = tree.children(i)
                 Z = np.vstack(
                     [Z, [
                         children[-1].data["unlinked_nodes"][0],
                         children[-2].data["unlinked_nodes"][0],
                         max_distance - _get_node_depth(path_to_leaves, i),
-                        children[-1].data["counts"] + children[-2].data["counts"],
+                        children[-1].data["counts"] + children[-2].data[
+                            "counts"],
                     ]]
                 )
                 # Update of the data of the algorithm execution tree node
                 tree.get_node(
                     i
                 ).data["dendromgram_indicator"] = dendrogram_counts
                 tree.get_node(i).data["counts"] = (
-                    children[-1].data["counts"] + children[-2].data["counts"]
+                        children[-1].data["counts"]
+                        + children[-2].data["counts"]
                 )
                 tree.get_node(i).data["unlinked_nodes"] = [dendrogram_counts]
                 dendrogram_counts += 1
 
     # Remove the first row of the linkage matrix because it is the
     # initialization`s row of zeros
     Z = Z[1:, :]
```

### Comparing `HiPart-0.3.2/src/HiPart/assets/int_viz.css` & `HiPart-0.4.1/src/HiPart/assets/int_viz.css`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.2/src/HiPart/clustering.py` & `HiPart-0.4.1/src/HiPart/clustering.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
 Implementation of the clustering algorithms, members of the HiPart package.
+
+@author Panagiotis Anagnostou
+@author Nicos Pavlidis
 """
 
 import HiPart.__utility_functions as util
 import numpy as np
 import statsmodels.api as sm
 
 from KDEpy import FFTKDE
+from scipy import stats
 from sklearn.cluster import KMeans
 from treelib import Tree
 
 
 class DePDDP:
     """
     Class dePDDP. It executes the dePDDP algorithm.
@@ -2128,7 +2132,472 @@
             labels_[i.data["indices"]] = i.identifier
         self.labels_ = labels_
         return self._labels_
 
     @labels_.setter
     def labels_(self, v):
         self._labels_ = v
+
+
+class MDH:
+    """
+    Class MDH. It executes the MDH algorithm.
+
+    References
+    ----------
+    Pavlidis, N. G., Hofmeyr, D. P., & Tasoulis, S. K. (2016). Minimum density
+    hyperplanes. Journal of Machine Learning Research, 17 (156), 1-33.
+
+    Parameters
+    ----------
+    max_clusters_number : int, optional
+        Desired maximum number of clusters to find the MDH algorithm.
+    max_iterations : int, optional
+        Maximum number of iterations on the search for the minimum density
+        hyperplane.
+    k : float, optional
+        The multiples of the standard deviation which the existence of a
+        splitting hyperplane is allowed. The default value is 2.3.
+    percentile : float, optional
+        The percentile distance from the dataset's edge in which a split can
+        not occur. [0,0.5) values are allowed.
+    min_sample_split : int, optional
+        The minimum number of points needed in a cluster for a split to occur.
+    random_seed : int, optional
+        The random seed to be used in the algorithm's execution.
+
+    Attributes
+    ----------
+    output_matrix : numpy.ndarray
+        Model's step by step execution output.
+    labels_ : numpy.ndarray
+        Extracted clusters from the algorithm.
+    tree : treelib.Tree
+        The object which contains all the information about the execution of
+        the MDH algorithm.
+    samples_number : int
+        The number of samples contained in the data.
+
+    """
+
+    def __init__(
+        self,
+        max_clusters_number=100,
+        max_iterations=10,
+        k=2.3,
+        percentile=0.1,
+        min_sample_split=5,
+        random_state=None,
+    ):
+        self.max_clusters_number = max_clusters_number
+        self.k = k
+        self.max_iterations = max_iterations
+        self.percentile = percentile
+        self.min_sample_split = min_sample_split
+        self.random_state = random_state
+
+    def fit(self, X):
+        """
+        Execute the MDH algorithm and return all the execution data in the form
+        of a MDH class object.
+
+        Parameters
+        ----------
+        X : numpy.ndarray
+            Data matrix with the samples on the rows and the variables on the
+            columns.
+
+        Returns
+        -------
+        self
+            A MDH class type object, with complete results on the algorithm's
+            analysis.
+
+        """
+
+        # initialize the random seed
+        np.random.seed(self.random_state)
+
+        # initialize the data matrix and the number of samples
+        self.X = X
+        self.samples_number = np.size(X, 0)
+
+        # create an id vector for the samples of X
+        indices = np.array([int(i) for i in range(self.samples_number)])
+
+        # initialize the tree and root node                           # step (0)
+        den_tree = Tree()
+        # nodes unique IDs indicator
+        self.node_ids = 0
+        # nodes next color indicator (necessary for visualization purposes)
+        self.cluster_color = 0
+        den_tree.create_node(
+            tag="density_cluster_" + str(self.node_ids),
+            identifier=self.node_ids,
+            data=self.calculate_node_data(indices, self.cluster_color),
+        )
+        # indicator for the next node to split
+        selected_node = 0
+
+        # if no possibility of split exists on the data                  # (ST2)
+        if not den_tree.get_node(0).data["split_permission"]:
+            raise RuntimeError("MDH: cannot split the data at all!!!")
+
+        # Initialize the ST1 stopping criterion counter that count the number
+        # of clusters                                                    # (ST1)
+        found_clusters = 1
+        while (found_clusters < self.max_clusters_number) and (
+            selected_node is not None
+        ):  # (ST1) or (ST2)
+
+            self.split_function(den_tree, selected_node)  # step (1, 2)
+
+            # select the next kid for split based on the local minimum density
+            selected_node = self.select_kid(den_tree.leaves())  # step (3)
+            found_clusters = found_clusters + 1  # (ST1)
+
+        self.tree = den_tree
+        return self
+
+    def fit_predict(self, X):
+        """
+        Execute the MDH algorithm and return the results of the execution in the
+        form of labels.
+
+        Parameters
+        ----------
+        X : numpy.ndarray
+            Data matrix with the samples on the rows and the variables on the
+            columns.
+
+        Returns
+        -------
+        labels_ : numpy.ndarray
+            Extracted clusters from the algorithm.
+
+        """
+
+        return self.fit(X).labels_
+
+    def split_function(self, den_tree, selected_node):
+        """
+        Split the indicated node on the minimum of the local minimum density
+        of the data projected on the first principal component.
+
+        Because python passes by reference data this function doesn't need a
+        return statement.
+
+        Parameters
+        ----------
+        den_tree : treelib.tree.Tree
+            The tree build by the MDH algorithm, in order to cluster the
+            input data.
+        selected_node : int
+            The numerical identifier for the tree node that i about to be split.
+
+        Returns
+        -------
+            There no returns in this function. The results of this function
+            pass to execution by utilizing the python's pass-by-reference
+            nature.
+
+        """
+        node = den_tree.get_node(selected_node)
+        node.data["split_permission"] = False
+
+        # left child indices extracted from the nodes split-point and the
+        # indices included in the parent node
+        left_kid_index = node.data["indices"][
+            np.where(node.data["projection"][:, 0] < node.data["splitpoint"])[0]
+        ]
+        # right child indices
+        right_kid_index = node.data["indices"][
+            np.where(node.data["projection"][:, 0] >= node.data["splitpoint"])[0]
+        ]
+
+        # Nodes and data creation for the children
+        # Uses the calculate_node_data function to create the data for the node
+        den_tree.create_node(
+            tag="density_cluster_" + str(self.node_ids + 1),
+            identifier=self.node_ids + 1,
+            parent=node.identifier,
+            data=self.calculate_node_data(left_kid_index, node.data["color_key"]),
+        )
+        den_tree.create_node(
+            tag="density_cluster_" + str(self.node_ids + 2),
+            identifier=self.node_ids + 2,
+            parent=node.identifier,
+            data=self.calculate_node_data(right_kid_index, self.cluster_color + 1),
+        )
+
+        self.cluster_color += 1
+        self.node_ids += 2
+
+    def select_kid(self, possible_splits):
+        """
+        The clusters each time exist in the leaves of the trees. From those
+        leaves select the next leave to split based on the algorithm's
+        specifications.
+
+        This function creates the necessary cause for the stopping criterion
+        ST1.
+
+        Parameters
+        ----------
+        possible_splits : list of treelib.node.Node
+            The list of nodes needed to exam to select the next Node to split.
+
+        Returns
+        -------
+        next_split : int
+            The identifier of the next node to split by the algorithm.
+
+        """
+        min_density_node = None
+
+        # Remove the nodes that can not split further
+        possible_splits = list(
+            np.array(possible_splits)[
+                [
+                    True if i.data["split_criterion"] is not None else False
+                    for i in possible_splits
+                ]
+            ]
+        )
+
+        if len(possible_splits) > 0:
+            for i in sorted(
+                enumerate(possible_splits), key=lambda x: x[1].data["split_criterion"],
+                reverse=True,
+            ):
+                if i[1].data["split_permission"]:
+                    min_density_node = i[1].identifier
+                    break
+
+        return min_density_node
+
+    def calculate_node_data(self, indices, key):
+        """
+        Find a minimum density hyperplane to bisect the data. The determination
+        of the minimum density hyperplane is based on the minimization is found
+        by minimizing the first derivative of the density function. This is made
+        possible through the use of "Sequential Quadratic Programming" (SQP)
+        method, which is used to simultaneously find the optimal projection
+        vector v and minimum density point b.
+
+        This function leads to the second Stopping criterion 2 of the
+        algorithm.
+
+        Parameters
+        ----------
+        indices : numpy.ndarray
+            The index of the samples in the original data matrix.
+        key : int
+            The value of the color for each node.
+
+        Returns
+        -------
+        data : dict
+            The necessary data for each node which are splitting point.
+
+        """
+
+        # Initialization of the return variables
+        projection = None
+        splitpoint = None
+        split_criterion = None
+        flag = False
+        split_vector = None
+
+        # If the number of samples in the node is greater than the minimum allowed for split
+        if indices.shape[0] > self.min_sample_split:
+            node_data = self.X[indices, :]
+            node_size = node_data.shape[0]
+            # Normalize the data of the node to zero mean and unit standard deviation
+            node_data = (node_data - np.mean(node_data, 0)) / np.std(node_data, 0)
+
+            minC = 100 if node_size * self.percentile > 100 else node_size * self.percentile
+
+            solutions = []
+            for i in range(0, self.max_iterations):
+
+                # Generate a random vector in the space of the node's data and
+                # normalize it to unit length
+                # v_n_b: vector v and point b
+                initial_v_n_b = stats.norm.rvs(size=np.shape(node_data)[1])
+                initial_v_n_b = initial_v_n_b / np.linalg.norm(initial_v_n_b)
+                initial_v_n_b = np.append(initial_v_n_b, 0)
+
+                # Find the minimum density point of the data on the projection
+                # direction
+                minimum_b = util.initialize_b(initial_v_n_b, node_data, depth_init=True)
+
+                if minimum_b:
+                    initial_v_n_b[-1] = minimum_b
+                    # res has the following fields that are of interest:
+                    #   1. success (whether algorithm terminated successfully)
+                    #   2. x (solution)
+                    #   3. nfev (number of function evaluations)
+                    #   4. njev (number of jacobian/ gradient evaluations)
+                    results, depth = util.md_sqp(initial_v_n_b, node_data, self.k)
+
+                    # If the algorithm terminated successfully try appending the append the solution
+                    if results.success:
+                        v = results.x[:-1] / np.linalg.norm(results.x[:-1])
+                        projection = np.dot(node_data, v).reshape(-1, 1)
+                        b = results.x[-1]
+                        c0 = np.sum(projection > b)
+                        # Solutions in the edges of the projection are not acceptable
+                        if min(c0, node_size - c0) >= minC:
+                            solutions.append((v, b, depth))
+
+            # Find the solution with the minimum depth
+            if solutions:
+                split = min(solutions, key=lambda x: x[2])
+                if split:
+                    splitpoint = split[1]
+                    projection = np.dot(node_data, split[0]).reshape(-1, 1)
+                    split_criterion = indices.shape[0]
+                    flag = True
+                    split_vector = split[0]
+
+        return {
+            "indices": indices,
+            "projection": projection,
+            "splitpoint": splitpoint,
+            "split_criterion": split_criterion,
+            "split_permission": flag,
+            "split_vector": split_vector,
+            "color_key": key,
+            "dendrogram_check": False,
+        }
+
+    @property
+    def max_clusters_number(self):
+        return self._max_clusters_number
+
+    @max_clusters_number.setter
+    def max_clusters_number(self, v):
+        if v < 0 or (not isinstance(v, int)):
+            raise ValueError(
+                "MDH: min_sample_split: Invalid value it should be int and > 1"
+            )
+        self._max_clusters_number = v
+
+    @property
+    def max_iterations(self):
+        return self._max_iterations
+
+    @max_iterations.setter
+    def max_iterations(self, v):
+        if v < 0 or (not isinstance(v, int)):
+            raise ValueError(
+                "MDH: max_iteration: Invalid value it should be int and > 1"
+            )
+        self._max_iterations = v
+
+    @property
+    def k(self):
+        return self._k
+
+    @k.setter
+    def k(self, v):
+        if v < 0 or (not isinstance(v, float)):
+            raise ValueError(
+                "MDH: k: Invalid value it should be float and > 1"
+            )
+        self._k = v
+
+    @property
+    def percentile(self):
+        return self._percentile
+
+    @percentile.setter
+    def percentile(self, v):
+        if v >= 0.5 or v < 0:
+            raise ValueError("MDH: percentile: Should be between [0,0.5) interval")
+        self._percentile = v
+
+    @property
+    def min_sample_split(self):
+        return self._min_sample_split
+
+    @min_sample_split.setter
+    def min_sample_split(self, v):
+        if v < 0 or (not isinstance(v, int)):
+            raise ValueError(
+                "MDH: min_sample_split: Invalid value it should be int and > 1"
+            )
+        self._min_sample_split = v
+
+    @property
+    def random_state(self):
+        return self._random_state
+
+    @random_state.setter
+    def random_state(self, v):
+        if v is not None and (not isinstance(v, int)):
+            raise ValueError(
+                "MDH: min_sample_split: Invalid value it should be int and > 1"
+            )
+        self._random_state = v
+
+    @property
+    def tree(self):
+        return self._tree
+
+    @tree.setter
+    def tree(self, v):
+        self._tree = v
+
+    @property
+    def output_matrix(self):
+        nd_dict = self.tree.nodes
+        output_matrix = [np.zeros(np.size(self.X, 0))]
+
+        # the dictionary of nodes contains the created node from the MDH
+        # algorithm sorted from the root to the last split
+        for i in nd_dict:
+            # For the output matrix we don't want the leaves of the tree. Each
+            # level of the output matrix represents a split the split exist in
+            # the internal nodes of the tree. Only by checking the children of
+            # those nodes we can extract the data for the current split.
+            if not nd_dict[i].is_leaf():
+                # create output cluster splitting matrix
+                tmp = np.copy(output_matrix[-1])
+                # Left child according to the tree creation process
+                tmp[self.tree.children(i)[0].data["indices"]] = self.tree.children(i)[
+                    0
+                ].identifier
+                # Right child according to the tree creation process
+                tmp[self.tree.children(i)[1].data["indices"]] = self.tree.children(i)[
+                    1
+                ].identifier
+
+                # The output_matrix is created transposed
+                output_matrix.append(tmp)
+        # the first row contains only zeros
+        del output_matrix[0]
+
+        # transpose the output_matrix to be extracted
+        output_matrix = np.array(output_matrix).transpose()
+
+        return output_matrix
+
+    @output_matrix.setter
+    def output_matrix(self, v):
+        raise RuntimeError(
+            "MDH: output_matrix: can only be generated and not to be assigned!"
+        )
+
+    @property
+    def labels_(self):
+        labels_ = np.ones(np.size(self.X, 0))
+        for i in self.tree.leaves():
+            labels_[i.data["indices"]] = i.identifier
+        return labels_
+
+    @labels_.setter
+    def labels_(self, v):
+        raise RuntimeError(
+            "MDH: labels_: can only be generated and not to be assigned!"
+        )
```

### Comparing `HiPart-0.3.2/src/HiPart/interactive_visualization.py` & `HiPart-0.4.1/src/HiPart/interactive_visualization.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.2/src/HiPart/visualizations.py` & `HiPart-0.4.1/src/HiPart/visualizations.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,30 +17,36 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
 Implementation module for the static visualization of the algorithms implemented
 in the HiPart package.
 
+@author: Panagiotis Anagnostou
+@author: Nicos Pavlidis
 """
 
 import HiPart.__utility_functions as util
 import math
 import matplotlib.gridspec as gridspec
 import matplotlib.pyplot as plt
+import numpy as np
 
-from scipy.cluster.hierarchy import dendrogram
 from HiPart.clustering import BisectingKmeans
 from HiPart.clustering import DePDDP
 from HiPart.clustering import IPDDP
 from HiPart.clustering import KMPDDP
 from HiPart.clustering import PDDP
+from HiPart.clustering import MDH
+from scipy.cluster.hierarchy import dendrogram
+from sklearn.decomposition import PCA
+from sklearn.neighbors import KernelDensity
 
 
-def split_visualization(hipart_object, color_map="tab20"):
+def split_visualization(hipart_object, color_map="tab20", mdh_split_plot=True):
     """
     Create the visualization of each of the splits generated by one of the
     divisive hierarchical clustering algorithms, members of HiPart package.
     For each split, we visualize the data on the first two principal
     components, while the color of each sample is chosen depending on the
     cluster it belongs to. The colors throughout the separate split represent
     the same cluster each time.
@@ -64,27 +70,34 @@
     principal component. That is the information the iPDDP algorithm utilizes
     to split each cluster.
 
     4. BisectingKmeans object does not include additional information in the
     visualization. That is because of the nature of the algorithm it
     implements.
 
+    5. MDH object does not include additional information in the visualization.
+    That is because of the nature of the algorithm it implements.
+
     Finally, for all the objects the visualization adds the selected split
     point for each split by each algorithm. This way one can validate the
     execution and the results of each algorithm. Moreover, examining this
     visualization can help the parametrization of the algorithms.
 
     Parameters
     ----------
     hipart_object : dePDDP or iPDDP or kM_PDDP or PDDP or BisectingKmeans
         The object member of HiPart package that we want to manipulate on the
         premiss of this function.
     color_map : string
         The name of the matplotlib color map to be used for the data
         visualization.
+    mdh_split_plot : bool
+        If True, the visualization of the MDH object will include the projection
+        vector and the splitting hyperplane visualization. See
+        visualization.mdh_visualization for more information.
 
     Raises
     ------
     TypeError
         If the hipart_object is not a member of the HiPart package raise an
         error for the possibility of unexpected errors that will be raised
         if the elements of the object are not correctly structured.
@@ -96,14 +109,17 @@
     Returns
     -------
     plt : pyplot (module)
         The created visualization by this function.
 
     """
 
+    if isinstance(hipart_object, MDH) and mdh_split_plot:
+        return mdh_visualization(hipart_object, color_map)
+
     # Check data compatibility with the function
     if isinstance(hipart_object, DePDDP):
         if not hipart_object.visualization_utility:
             raise ValueError(
                 """The visualization of the data cannot be archived because the
                 visualization_utility is False."""
             )
@@ -119,15 +135,18 @@
             raise ValueError(
                 """The visualization of the data cannot be archived because the
                 visualization_utility is False."""
             )
         with_hist = False
         with_marginal_scatter = True
         grid_size = 4
-    elif isinstance(hipart_object, BisectingKmeans):
+    elif (
+        isinstance(hipart_object, BisectingKmeans)
+        or isinstance(hipart_object, MDH)
+    ):
         with_hist = False
         with_marginal_scatter = False
         grid_size = 2
     else:
         raise TypeError("can only process objects of the 'HiPart' package.")
 
     # prepare the necessary data for this visualization
@@ -246,15 +265,18 @@
                 "Split no. "
                 + str(i + 1)
             )
 
         else:
             # Bisecting k-Means doesn't execute PCA, so we execute it here for
             # the visualization
-            if isinstance(hipart_object, BisectingKmeans):
+            if (
+                isinstance(hipart_object, BisectingKmeans)
+                or isinstance(hipart_object, MDH)
+            ):
                 principal_projections = util.execute_decomposition_method(
                     data_matrix=hipart_object.X[
                         dictionary_of_nodes[internal_nodes[i]].data["indices"]
                     ],
                     decomposition_method="pca",
                     two_dimentions=True,
                     decomposition_args={},
@@ -285,14 +307,195 @@
                 "Original data with 1st split"
             ) if i == 0 else ax.title.set_text("Split no. " + str(i + 1))
 
     plt.subplots_adjust(wspace=0.2, hspace=0.6)
     return plt
 
 
+def mdh_visualization(mdh_obj, color_map="tab20"):
+    """
+    Create the visualization of each of the splits generated by MDH algorithm,
+    members of HiPart package. For each split, we visualize the data on the
+    first two principal components, while the color of each sample is chosen
+    depending on the cluster it belongs to. The colors throughout the separate
+    split represent the same cluster each time.
+
+    Moreover, we add the line of the projection vector projected onto the first
+    two principal components, as well as a dashed line representing the
+    splitting hyperplane. The splitting hyperplane a line that is perpendicular
+    to the projection vector and passes through the minimum density point of the
+    data on the projection direction. In addition, we create add the density of
+    the data onto the projection vector in the form of a blue line, projected
+    onto the projection vector. With this information one can validate the
+    execution and the results of each algorithm and examining this visualization
+    can help the parametrization of the algorithms.
+
+    Warning: the projection vector and the splitting hyperplane in the plot may
+    not seem perpendicular to each other. This is because the projection vector
+    is projected onto the first two principal components, and we can't predict
+    the viewing angle of the plot, in the tuple of dimensions. For the same
+    reason, dotted line representing the splitting hyperplane may seem misplaced
+    from the data it splits.
+
+    Parameters
+    ----------
+    mdh_obj : MDH
+        The object member of HiPart package that we want to manipulate on the
+        premiss of this function.
+    color_map : string
+        The name of the matplotlib color map to be used for the data
+        visualization.
+
+    Raises
+    ------
+    TypeError
+        If the hipart_object is not a member of the HiPart package raise an
+        error for the possibility of unexpected errors that will be raised
+        if the elements of the object are not correctly structured.
+    ValueError
+        If the "visualization_utility" attribute of the imported object is
+        False, this causes some needed for this visualization data not
+        to be created.
+
+    Returns
+    -------
+    plt : pyplot (module)
+        The created visualization by this function.
+
+    """
+    grid_size = 2
+
+    # prepare the necessary data for this visualization
+    (
+        dictionary_of_nodes,
+        internal_nodes,
+        _,
+        sample_color,
+    ) = util.visualization_preparation(mdh_obj, color_map)
+    number_of_splits = len(internal_nodes)
+
+    # Ensure that the root node will be always an internal node while is the
+    # only node in the tree
+    if number_of_splits == 0:
+        internal_nodes = [0]
+
+    # select the number of plot sub-figures
+    row_plots = 3 if math.ceil(number_of_splits) > 4 else 2
+
+    # set figure size
+    fig = plt.figure(
+        figsize=(4 * row_plots, 3.5 * math.ceil(number_of_splits / row_plots)),
+    )
+
+    # create grid for sub-figures
+    gs = gridspec.GridSpec(
+        math.ceil(number_of_splits / row_plots) * grid_size,
+        row_plots * grid_size,
+        fig,
+    )
+
+    for i in range(number_of_splits):
+        # Extract the subplot position
+        row_from, row_to, col_from, col_to = util.grid_position(
+            current=i,
+            rows=row_plots,
+            splits=number_of_splits,
+            with_marginal=False,
+        )
+
+        # create each individual visualization
+        ax = plt.subplot(gs[row_from:row_to, col_from:col_to])
+
+        # get the color of the sample that belong to the i internal node
+        pr_col = sample_color[
+            mdh_obj.tree.get_node(internal_nodes[i]).data["indices"]
+        ]
+
+        node_data = mdh_obj.X[
+            dictionary_of_nodes[internal_nodes[i]].data["indices"]
+        ]
+        node_data = (node_data - np.mean(node_data, 0)) / np.std(node_data, 0)
+
+        pca = PCA(n_components=2)
+        pcaproj = pca.fit_transform(node_data)
+        v = dictionary_of_nodes[internal_nodes[i]].data["split_vector"]
+        b = dictionary_of_nodes[internal_nodes[i]].data["splitpoint"]
+
+        v_norm = np.linalg.norm(v)
+        # convert v to unit vector
+        v = v / v_norm
+
+        pv = pca.transform(v.reshape(1, -1))[0]
+        pv = pv / np.linalg.norm(pv)  # $$
+        b = b / np.linalg.norm(pv)
+
+        proj = np.dot(pcaproj, pv)
+        h = util.band_const(mdh_obj.samples_number) * np.std(proj)
+
+        x_grid = np.linspace(-3.5 * np.std(proj), 3.5 * np.std(proj), 1000)
+
+        if np.abs(np.abs(pv[1]) - 1) <= 1.0e-8:
+            ax.vlines(
+                x=0, ymin=np.amin(x_grid), ymax=np.amax(x_grid), colors="cyan",
+                zorder=2
+            )
+            phi = np.sign(pv[1]) * 0.5 * np.pi
+        else:
+            phi = np.arctan2(pv[1], pv[0])
+            ax.plot(x_grid, np.tan(phi) * x_grid, c="cyan", zorder=2)
+
+        ax.plot(np.cos(phi) * proj, np.sin(phi) * proj, c="r", alpha=0.7,
+                zorder=3)
+
+        ax.scatter(
+            np.cos(phi) * b, np.sin(phi) * b, marker="o", c="r", alpha=1,
+            zorder=4
+        )
+        ax.plot(
+            x_grid,
+            np.sin(phi) * b + np.tan(phi + np.pi / 2) * (
+                        x_grid - np.cos(phi) * b),
+            ":r",
+            zorder=4,
+        )
+
+        kde = KernelDensity(kernel="gaussian", bandwidth=h)
+        kde.fit(proj[:, np.newaxis])
+        out = np.exp(kde.score_samples(x_grid[:, np.newaxis]))
+
+        # plot kde
+        P = phi
+        R = np.matrix([[np.cos(P), -np.sin(P)], [np.sin(P), np.cos(P)]])
+        Y = np.matmul(R, np.row_stack((x_grid, out)))
+        ax.plot(Y.A[0], Y.A[1], c="DarkBlue", lw=1, label="kde", zorder=4)
+
+        ax.scatter(pcaproj[:, 0], pcaproj[:, 1], c=pr_col, s=5, marker=".",
+                   zorder=1)
+        ax.set_xticks([])
+        ax.set_yticks([])
+        ax.set_xlim(
+            min(pcaproj[:, 0]) - np.std(pcaproj[:, 0]) / 2,
+            max(pcaproj[:, 0]) + np.std(pcaproj[:, 0]) / 2,
+        )
+        ax.set_ylim(
+            min(pcaproj[:, 1]) - np.std(pcaproj[:, 1]) / 2,
+            max(pcaproj[:, 1]) + np.std(pcaproj[:, 1]) / 2,
+        )
+        ax.grid(False)
+        ax.margins(0.03)
+
+        # title the subplot
+        ax.title.set_text(
+            "Original data with 1st split"
+        ) if i == 0 else ax.title.set_text("Split no. " + str(i + 1))
+
+    plt.subplots_adjust(wspace=0.2, hspace=0.6)
+    return plt
+
+
 def dendrogram_visualization(hipart_object, **dendrogram_parameters):
     """
     Create a dendrogram visualization of the divisive clustering based on the
     HiPart`s algorithm execution. The characteristic of this dendrogram is that
     the distance of the clusters is not the one depicted on the graph, but it
     represents the distance of each node from the base of the tree, also known
     as leaves.
@@ -326,14 +529,15 @@
 
     if not (
         isinstance(hipart_object, DePDDP)
         or isinstance(hipart_object, IPDDP)
         or isinstance(hipart_object, KMPDDP)
         or isinstance(hipart_object, PDDP)
         or isinstance(hipart_object, BisectingKmeans)
+        or isinstance(hipart_object, MDH)
     ):
         raise TypeError("can only process objects of the 'HiPart' package.")
 
     Z = util.create_linkage(hipart_object.tree)
     dn = dendrogram(Z, color_threshold=0.3, **dendrogram_parameters)
 
     return dn
@@ -363,11 +567,12 @@
 
     if not (
         isinstance(hipart_object, DePDDP)
         or isinstance(hipart_object, IPDDP)
         or isinstance(hipart_object, KMPDDP)
         or isinstance(hipart_object, PDDP)
         or isinstance(hipart_object, BisectingKmeans)
+        or isinstance(hipart_object, MDH)
     ):
         raise TypeError("can only process objects of the 'HiPart' package.")
 
     return util.create_linkage(hipart_object.tree)
```

### Comparing `HiPart-0.3.2/src/HiPart.egg-info/PKG-INFO` & `HiPart-0.4.1/src/HiPart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.3.2
+Version: 0.4.1
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
 Project-URL: Documentation, https://hipart.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/panagiotisanagnostou/HiPart/
```

### Comparing `HiPart-0.3.2/tests/test_package.py` & `HiPart-0.4.1/tests/test_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from distutils import dir_util
 from HiPart import visualizations as viz
 from HiPart.clustering import DePDDP
 from HiPart.clustering import IPDDP
 from HiPart.clustering import KMPDDP
 from HiPart.clustering import PDDP
 from HiPart.clustering import BisectingKmeans
+from HiPart.clustering import MDH
 
 import numpy as np
 import os
 import pickle
 import pytest
 
 
@@ -65,14 +66,22 @@
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     new_obj = BisectingKmeans(max_clusters_number=5).fit(data_import["data"])
     assert isinstance(new_obj, BisectingKmeans)
 
 
+def test_mdh_return_type(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    new_obj = MDH(max_clusters_number=5).fit(data_import["data"])
+    assert isinstance(new_obj, MDH)
+
+
 def test_depddp_parameter_errors():
     success_score = 0
 
     algorithm = DePDDP()
     success_score += 1 if isinstance(algorithm.decomposition_method, str) else 0
     success_score += 1 if isinstance(algorithm.max_clusters_number, int) else 0
     success_score += 1 if isinstance(algorithm.bandwidth_scale, float) else 0
@@ -209,14 +218,53 @@
         BisectingKmeans(min_sample_split=-5)
     except Exception:
         success_score += 1
 
     assert success_score == 6
 
 
+def test_mdh_parameter_errors():
+    success_score = 0
+
+    algorithm = MDH(random_state=5)
+    success_score += 1 if isinstance(algorithm.max_clusters_number, int) else 0
+    success_score += 1 if isinstance(algorithm.max_iterations, int) else 0
+    success_score += 1 if isinstance(algorithm.k, float) else 0
+    success_score += 1 if isinstance(algorithm.percentile, float) else 0
+    success_score += 1 if isinstance(algorithm.min_sample_split, int) else 0
+    success_score += 1 if isinstance(algorithm.random_state, int) else 0
+
+    try:
+        MDH(max_clusters_number=-5)
+    except Exception:
+        success_score += 1
+    try:
+        MDH(max_iterations=-5)
+    except Exception:
+        success_score += 1
+    try:
+        MDH(k=-.8)
+    except Exception:
+        success_score += 1
+    try:
+        MDH(percentile=.8)
+    except Exception:
+        success_score += 1
+    try:
+        MDH(random_state=.8)
+    except Exception:
+        success_score += 1
+    try:
+        MDH(min_sample_split=-5)
+    except Exception:
+        success_score += 1
+
+    assert success_score == 12
+
+
 def test_depddp_labels__return_type_and_form(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     results = DePDDP(max_clusters_number=5).fit_predict(data_import["data"])
     assert isinstance(results, np.ndarray) and results.ndim == 1
 
@@ -241,37 +289,60 @@
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     results = PDDP(max_clusters_number=5).fit_predict(data_import["data"])
     assert isinstance(results, np.ndarray) and results.ndim == 1
 
 
-def test_bicecting_kmeans_labels__return_type_and_form(datadir):
+def test_bicecting_kmeans_labels_return_type_and_form(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     results = BisectingKmeans(
         max_clusters_number=5,
     ).fit_predict(data_import["data"])
     assert isinstance(results, np.ndarray) and results.ndim == 1
 
 
+def test_mdh_labels_return_type_and_form(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    results = MDH(
+        max_clusters_number=5,
+    ).fit_predict(data_import["data"])
+    assert isinstance(results, np.ndarray) and results.ndim == 1
+
+
 def test_bicecting_kmeans_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     matrix_control = data_import["BisectingKmeans"]
 
     matrix_test = BisectingKmeans(
         max_clusters_number=5,
         random_seed=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
+def test_mdh_results(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    matrix_control = data_import["MDH"]
+
+    matrix_test = MDH(
+        max_clusters_number=5,
+        random_state=1256,
+    ).fit(data_import["data"]).output_matrix
+    assert np.sum(matrix_test == matrix_control) == 6000
+
+
 def test_depddp_pca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     matrix_control = data_import["DePDDP_pca"]
 
     matrix_test = DePDDP(
@@ -574,14 +645,44 @@
     try:
         viz.split_visualization(clustering)
         assert True
     except Exception:
         assert False
 
 
+def test_split_visualization_plot_8(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    clustering = MDH(
+        max_clusters_number=5,
+        random_state=1256,
+    ).fit(data_import["data"])
+    try:
+        viz.split_visualization(clustering, mdh_split_plot=True)
+        assert True
+    except Exception:
+        assert False
+
+
+def test_split_visualization_plot_9(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    clustering = MDH(
+        max_clusters_number=5,
+        random_state=1256,
+    ).fit(data_import["data"])
+    try:
+        viz.split_visualization(clustering, mdh_split_plot=False)
+        assert True
+    except Exception:
+        assert False
+
+
 def test_split_visualization_typeerror(datadir):
     try:
         viz.split_visualization(np.array([1, 2, 3]))
         assert False
     except Exception:
         assert True
```

