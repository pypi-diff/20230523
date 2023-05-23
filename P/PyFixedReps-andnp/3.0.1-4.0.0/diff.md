# Comparing `tmp/PyFixedReps-andnp-3.0.1.tar.gz` & `tmp/PyFixedReps-andnp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFixedReps-andnp-3.0.1.tar", last modified: Wed Jan 18 17:35:06 2023, max compression
+gzip compressed data, was "PyFixedReps-andnp-4.0.0.tar", last modified: Tue May 23 03:16:48 2023, max compression
```

## Comparing `PyFixedReps-andnp-3.0.1.tar` & `PyFixedReps-andnp-4.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-18 17:34:36.485315 PyFixedReps-andnp-3.0.1/PyFixedReps/BaseRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-01-18 17:34:36.485315 PyFixedReps-andnp-3.0.1/PyFixedReps/RBF.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-01-18 17:34:36.485315 PyFixedReps-andnp-3.0.1/PyFixedReps/TileCoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-18 17:34:36.485315 PyFixedReps-andnp-3.0.1/PyFixedReps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-18 17:34:36.485315 PyFixedReps-andnp-3.0.1/PyFixedReps/_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-01-18 17:35:04.873303 PyFixedReps-andnp-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-18 17:35:04.881303 PyFixedReps-andnp-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 17:34:36.489315 PyFixedReps-andnp-3.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-01-18 17:34:36.489315 PyFixedReps-andnp-3.0.1/tests/test_RBF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-01-18 17:34:36.489315 PyFixedReps-andnp-3.0.1/tests/test_TileCoder.py
--rw-------   0 runner    (1001) docker     (123)     3800 2023-01-18 17:35:06.149303 PyFixedReps-andnp-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      181 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/BaseRepresentation.py
+-rw-r--r--   0        0        0      751 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/RBF.py
+-rw-r--r--   0        0        0     2856 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/TileCoder.py
+-rw-r--r--   0        0        0      220 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/__init__.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/_jit.py
+-rw-r--r--   0        0        0     2931 2023-05-23 03:16:46.383080 PyFixedReps-andnp-4.0.0/README.md
+-rw-r--r--   0        0        0      942 2023-05-23 03:16:46.395080 PyFixedReps-andnp-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/tests/test_RBF.py
+-rw-r--r--   0        0        0     3907 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/tests/test_TileCoder.py
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.0.0/PKG-INFO
```

### Comparing `PyFixedReps-andnp-3.0.1/PyFixedReps/RBF.py` & `PyFixedReps-andnp-4.0.0/PyFixedReps/RBF.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-3.0.1/README.md` & `PyFixedReps-andnp-4.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+Metadata-Version: 2.1
+Name: PyFixedReps-andnp
+Version: 4.0.0
+License: MIT
+Author-email: Andy Patterson <andnpatterson@gmail.com>
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==3.0.1
+pip install PyFixedReps-andnp==4.0.0
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
@@ -17,15 +25,14 @@
 tc = TileCoder({
     # [required]
     'tiles': 2, # how many tiles in each tiling
     'tilings': 4,
     'dims': 2, # shape of the state-vector
 
     # [optional]
-    'actions': 2, # offset the representation by which action was taken (more details below)
     'random_offset': True, # instead of using the default fixed-width offset, randomly generate offsets between tilings
     'input_ranges': [(-1.2, 0.5), (-0.07, 0.07)], # a vector of same length as 'dims' containing (min, max) tuples to rescale inputs
     'scale_output': True, # scales the output by number of active features
 })
 
 state = [-1.1, 0.03]
 # returns an n-hot numpy array for active tiles
@@ -40,11 +47,11 @@
 print(indices) # -> [4, 12, 31, 89]
 
 num_features = tc.features()
 print(num_features) # -> 16, the length of the vector generated by "encode"
 ```
 
 ### Options
- * `actions` - by specifying the number of actions, the tile-coder will expect that you include the action which was taken in the `encode` function. For example, `tc.encode(state, action)`. This will offset the entire representation so that each action gets its own portion of the feature vector. The size of the feature vector is the size of the usual state feature vector times the total number of actions. Personally, I do not like this convention and find it to be rather computationally inefficient, but it is commonly used so I decided to support it (though not by default).
  * `random_offset` - In most cases, having a uniform even offset is sufficient to have uncorrelated and high coverage of the statespace. Occasionally, it becomes important that the offsets are randomly generated to break any correlations or structure in the statespace.
  * `input_ranges` - It's important that the inputs are scaled between `[0, 1]` for this tile-coder to be most effective. When not scaled, we can potentially get into bad failure cases where only a small percentage of the tiles are ever active. This is true of all current tile-coder implementations. This implementation is robust to imperfect scaling by wrapping values larger than 1 back around to 0 (modular arithmetic), so as long as the units are _roughly_ correct then good performance can still be achieved.
  * `scale_output` - Has the `encode` function scale the outputs by the norm of the feature vector so that every feature vector has unit norm. This is simply a scalar multiple of every feature vector, which is often perfectly absorbed into the stepsize parameter, the effect of this option is to make it easier to find good stepsize by decoupling number of tilings from applicable stepsize range.
+
```

### Comparing `PyFixedReps-andnp-3.0.1/pyproject.toml` & `PyFixedReps-andnp-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.1"
+version = "4.0.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
     "README.md",
 ]
 
 [tool.pdm]
@@ -24,22 +24,23 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyFixedReps-andnp"
-version = "3.0.1"
+version = "4.0.0"
 description = ""
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numpy>=1.23.5",
     "numba>=0.56.4",
+    "tile-coder==0.1.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `PyFixedReps-andnp-3.0.1/tests/test_TileCoder.py` & `PyFixedReps-andnp-4.0.0/tests/test_TileCoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,162 +4,130 @@
 
 class TestTileCoder(unittest.TestCase):
     def test_get_indices_1d_1tiling(self):
         config = TileCoderConfig(
             tiles=2,
             tilings=1,
             dims=1,
-            actions=2,
         )
         tc = TileCoder(config)
 
-        indices = tc.get_indices([0], 0)
+        indices = tc.get_indices([0])
         self.assertListEqual(list(indices), [0])
 
-        indices = tc.get_indices([0.4], 0)
+        indices = tc.get_indices([0.4])
         self.assertListEqual(list(indices), [0])
 
-        indices = tc.get_indices([0.5], 0)
+        indices = tc.get_indices([0.5])
         self.assertListEqual(list(indices), [1])
 
-        indices = tc.get_indices([1.0], 0)
-        self.assertListEqual(list(indices), [0])
-
-        indices = tc.get_indices([0], 1)
-        self.assertListEqual(list(indices), [2])
-
-        indices = tc.get_indices([0.4], 1)
-        self.assertListEqual(list(indices), [2])
-
-        indices = tc.get_indices([0.5], 1)
-        self.assertListEqual(list(indices), [3])
-
-        indices = tc.get_indices([1.0], 1)
-        self.assertListEqual(list(indices), [2])
-
-        # test out of bounds
-        indices = tc.get_indices([1.1], 0)
-        self.assertListEqual(list(indices), [0])
-
-        indices = tc.get_indices([1.1], 1)
-        self.assertListEqual(list(indices), [2])
+        indices = tc.get_indices([1.0])
+        self.assertListEqual(list(indices), [1])
 
     def test_get_indices_2d_1tiling(self):
         config = TileCoderConfig(
             dims=2,
             tilings=1,
             tiles=2,
-            actions=2,
         )
         tc = TileCoder(config)
 
-        indices = tc.get_indices([0, 0], 0)
+        indices = tc.get_indices([0, 0])
         self.assertListEqual(list(indices), [0])
 
-        indices = tc.get_indices([0.99, 0], 0)
+        indices = tc.get_indices([0.99, 0])
         self.assertListEqual(list(indices), [1])
 
-        indices = tc.get_indices([0, 0.99], 0)
+        indices = tc.get_indices([0, 0.99])
         self.assertListEqual(list(indices), [2])
 
-        indices = tc.get_indices([0.6, 0.8], 0)
+        indices = tc.get_indices([0.6, 0.8])
         self.assertListEqual(list(indices), [3])
 
-        indices = tc.get_indices([0, 0], 1)
-        self.assertListEqual(list(indices), [4])
-
-        indices = tc.get_indices([0.99, 0], 1)
-        self.assertListEqual(list(indices), [5])
-
     def test_get_indices_1d_2tiling(self):
         config = TileCoderConfig(
             dims=1,
             tilings=2,
             tiles=2,
-            actions=2,
         )
         tc = TileCoder(config)
 
-        indices = tc.get_indices([0], 0)
+        indices = tc.get_indices([0])
         self.assertListEqual(list(indices), [0, 2])
 
-        indices = tc.get_indices([0.99], 0)
-        self.assertListEqual(list(indices), [1, 2])
+        indices = tc.get_indices([0.99])
+        self.assertListEqual(list(indices), [1, 3])
 
-        indices = tc.get_indices([.3], 0)
+        indices = tc.get_indices([.3])
         self.assertListEqual(list(indices), [0, 3])
 
-        indices = tc.get_indices([.51], 0)
+        indices = tc.get_indices([.51])
         self.assertListEqual(list(indices), [1, 3])
 
     def test_get_indices_2d_2tiling(self):
         config = TileCoderConfig(
             bound='clip',
             dims=2,
             tilings=2,
             tiles=2,
-            actions=1,
         )
         tc = TileCoder(config)
 
-        indices = tc.get_indices([0, 0], 0)
+        indices = tc.get_indices([0, 0])
         self.assertListEqual(list(indices), [0, 4])
 
-        indices = tc.get_indices([0.99, 0.99], 0)
+        indices = tc.get_indices([0.99, 0.99])
         self.assertListEqual(list(indices), [3, 7])
 
-        indices = tc.get_indices([.3, .2], 0)
+        indices = tc.get_indices([.3, .2])
         self.assertListEqual(list(indices), [0, 5])
 
-        indices = tc.get_indices([.51, .51], 0)
+        indices = tc.get_indices([.51, .51])
         self.assertListEqual(list(indices), [3, 7])
 
     def test_get_indices_2d_2tiling_random(self):
 
         config = TileCoderConfig(
             dims=2,
             tilings=2,
             tiles=2,
-            actions=1,
             offset='random',
         )
 
         rng = np.random.RandomState(42)
         tc = TileCoder(config, rng=rng)
 
-        indices = tc.get_indices([0, 0], 0)
+        indices = tc.get_indices([0, 0])
         self.assertListEqual(list(indices), [2, 7])
 
     def test_encode(self):
         config = TileCoderConfig(
             dims=2,
             tilings=2,
             tiles=2,
-            actions=2,
             scale_output=False,
         )
         tc = TileCoder(config)
 
-        rep = tc.encode([0, 0.2], 1)
-        expected = [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0]
+        rep = tc.encode([0, 0.2])
+        expected = [1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0]
 
         self.assertListEqual(list(rep), expected)
 
     def test_scaling(self):
         config = TileCoderConfig(
             dims=2,
             tilings=2,
             tiles=2,
-            actions=2,
             input_ranges=[(-1, 1), (2.1, 4.1)],
         )
         tc = TileCoder(config)
 
-        rep = tc.encode([-1, 2.5], 1)
-        expected = [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.0, 0.0, 0.0, 0.5, 0.0, 0.0, 0.0]
+        rep = tc.encode([-1, 2.5])
+        expected = [0.5, 0.0, 0.0, 0.0, 0.5, 0.0, 0.0, 0.0]
         self.assertListEqual(list(rep), expected)
 
     def test_tabular(self):
         config = TileCoderConfig(
             dims=2,
             tiles=7,
             tilings=1,
```

