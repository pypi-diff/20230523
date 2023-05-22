# Comparing `tmp/pytorch-calibrated-0.0.2.tar.gz` & `tmp/pytorch-calibrated-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-calibrated-0.0.2.tar", last modified: Tue Apr 11 01:27:17 2023, max compression
+gzip compressed data, was "pytorch-calibrated-0.1.1.tar", last modified: Mon May 22 23:07:55 2023, max compression
```

## Comparing `pytorch-calibrated-0.0.2.tar` & `pytorch-calibrated-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/pytorch_calibrated/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/layers/numerical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/pytorch_calibrated/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 01:27:17.000000 pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:27:17.933414 pytorch-calibrated-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_categorical_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-04-11 01:27:06.000000 pytorch-calibrated-0.0.2/tests/test_numerical_calibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:07:55.913112 pytorch-calibrated-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-22 23:07:55.913112 pytorch-calibrated-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:07:55.905112 pytorch-calibrated-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:07:55.909112 pytorch-calibrated-0.1.1/pytorch_calibrated/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:07:55.909112 pytorch-calibrated-0.1.1/pytorch_calibrated/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/layers/categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/layers/numerical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/pytorch_calibrated/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:07:55.909112 pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-22 23:07:55.000000 pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-22 23:07:55.000000 pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:07:55.000000 pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 23:07:55.000000 pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 23:07:55.000000 pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:07:55.913112 pytorch-calibrated-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:07:55.913112 pytorch-calibrated-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/tests/test_categorical_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-05-22 23:07:44.000000 pytorch-calibrated-0.1.1/tests/test_numerical_calibrator.py
```

### Comparing `pytorch-calibrated-0.0.2/LICENSE` & `pytorch-calibrated-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/PKG-INFO` & `pytorch-calibrated-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-calibrated
-Version: 0.0.2
+Version: 0.1.1
 Summary: A PyTorch Library For Interpretable Machine Learning
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SOTAI-Labs/pytorch-calibrated
 Project-URL: Documentation, https://github.com/SOTAI-Labs/pytorch-calibrated/tree/dev/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytorch-calibrated Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: pytorch-calibrated Version: 0.1.1 Summary: A
 PyTorch Library For Interpretable Machine Learning Author-email: SOTAI
 sotai.ai> Maintainer-email: SOTAI
 sotai.ai> License: Apache-2.0 Project-URL: Source, https://github.com/SOTAI-
 Labs/pytorch-calibrated Project-URL: Documentation, https://github.com/SOTAI-
 Labs/pytorch-calibrated/tree/dev/docs Project-URL: Feature Requests, https://
 github.com/SOTAI-Labs/pytorch-calibrated/issues Project-URL: Bug Reports,
 https://github.com/SOTAI-Labs/pytorch-calibrated/issues Classifier: Development
```

### Comparing `pytorch-calibrated-0.0.2/docs/README.md` & `pytorch-calibrated-0.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pyproject.toml` & `pytorch-calibrated-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "pytorch-calibrated"
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release.
 #
 # NOTE: as part of the release flow, update this version immediately after release.
-version = "0.0.2"
+version = "0.1.1"
 description = "A PyTorch Library For Interpretable Machine Learning"
 readme = "docs/README.md"
 license = {text = "Apache-2.0"}
 authors = [
   {name = "SOTAI", email = "support@sotai.ai"},
 ]
 maintainers = [
```

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/__init__.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 # limitations under the License.
 """PyTorch implementation of calibrated modeling."""
 # This version must always be one version ahead of the current release, so it
 # matches the current state of development, which will always be ahead of the
 # current release.
 #
 # NOTE: as part of the release flow, update this version immediately after release.
-__version__ = "0.0.2"
+__version__ = "0.1.1"
 
 from pytorch_calibrated import configs, data, enums, layers, models
 
 __all__ = ["configs", "data", "enums", "layers", "models"]
```

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/configs.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/configs.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/data.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/data.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/enums.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/enums.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,70 +8,81 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Enums used throughout the PyTorch Calibrated library."""
-from enum import Enum
+from enum import Enum, EnumMeta
+from typing import Any
 
 
-class Monotonicity(Enum):
+class _Metaclass(EnumMeta):
+    """Base `EnumMeta` subclass for accessing enum members directly."""
+
+    def __getattribute__(cls, __name: str) -> Any:
+        value = super().__getattribute__(__name)
+        if isinstance(value, Enum):
+            value = value.value
+        return value
+
+
+class Monotonicity(str, Enum, metaclass=_Metaclass):
     """Type of monotonicity constraint.
 
     - NONE: no monotonicity constraint.
     - INCREASING: increasing monotonicity i.e. increasing input increases output.
     - DECREASING: decreasing monotonicity i.e. increasing input decreases output.
     """
 
-    NONE = 0
-    INCREASING = 1
-    DECREASING = -1
+    NONE = "none"
+    INCREASING = "increasing"
+    DECREASING = "decreasing"
 
 
-class NumericalCalibratorInit(Enum):
+class NumericalCalibratorInit(str, Enum, metaclass=_Metaclass):
     """Type of kernel initialization to use for NumericalCalibrator.
 
     - EQUAL_HEIGHTS: initialize the kernel such that all segments have the same height.
     - EQUAL_SLOPES: initialize the kernel such that all segments have the same slope.
     """
 
-    EQUAL_HEIGHTS = 0
-    EQUAL_SLOPES = 1
+    EQUAL_HEIGHTS = "equal_heights"
+    EQUAL_SLOPES = "equal_slopes"
 
 
-class CategoricalCalibratorInit(Enum):
+class CategoricalCalibratorInit(str, Enum, metaclass=_Metaclass):
     """Type of kernel initialization to use for CategoricalCalibrator.
 
     - UNIFORM: initialize the kernel with uniformly distributed values. The sample range
         will be [`output_min`, `output_max`] if both are provided.
     - CONSTANT: initialize the kernel with a constant value for all categories. This
         value will be `(output_min + output_max) / 2` if both are provided.
     """
 
-    UNIFORM = 0
-    CONSTANT = 1
+    UNIFORM = "uniform"
+    CONSTANT = "constant"
 
 
-class InputKeypointsInit(Enum):
+class InputKeypointsInit(str, Enum, metaclass=_Metaclass):
     """Type of initialization to use for NumericalCalibrator input keypoints.
 
     - QUANTILES: initialize the input keypoints such that each segment will see the same
         number of examples.
     - UNIFORM: initialize the input keypoints uniformly spaced in the feature range.
     """
 
-    QUANTILES = 0
-    UNIFORM = 1
+    QUANTILES = "quantiles"
+    UNIFORM = "uniform"
 
 
-class FeatureType(Enum):
+class FeatureType(str, Enum, metaclass=_Metaclass):
     """Type of feature.
 
     - NUMERICAL: a numerical feature that should be calibrated using an instance of
         `NumericalCalibrator`.
     - CATEGORICAL: a categorical feature that should be calibrated using an instance of
         `CategoricalCalibrator`.
     """
 
-    NUMERICAL = 0
-    CATEGORICAL = 1
+    NUMERICAL = "numerical"
+    CATEGORICAL = "categorical"
```

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/__init__.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/categorical_calibrator.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/layers/categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/linear.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/layers/linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/layers/numerical_calibrator.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/layers/numerical_calibrator.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated/models.py` & `pytorch-calibrated-0.1.1/pytorch_calibrated/models.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/PKG-INFO` & `pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-calibrated
-Version: 0.0.2
+Version: 0.1.1
 Summary: A PyTorch Library For Interpretable Machine Learning
 Author-email: SOTAI <support@sotai.ai>
 Maintainer-email: SOTAI <support@sotai.ai>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SOTAI-Labs/pytorch-calibrated
 Project-URL: Documentation, https://github.com/SOTAI-Labs/pytorch-calibrated/tree/dev/docs
 Project-URL: Feature Requests, https://github.com/SOTAI-Labs/pytorch-calibrated/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytorch-calibrated Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: pytorch-calibrated Version: 0.1.1 Summary: A
 PyTorch Library For Interpretable Machine Learning Author-email: SOTAI
 sotai.ai> Maintainer-email: SOTAI
 sotai.ai> License: Apache-2.0 Project-URL: Source, https://github.com/SOTAI-
 Labs/pytorch-calibrated Project-URL: Documentation, https://github.com/SOTAI-
 Labs/pytorch-calibrated/tree/dev/docs Project-URL: Feature Requests, https://
 github.com/SOTAI-Labs/pytorch-calibrated/issues Project-URL: Bug Reports,
 https://github.com/SOTAI-Labs/pytorch-calibrated/issues Classifier: Development
```

### Comparing `pytorch-calibrated-0.0.2/pytorch_calibrated.egg-info/SOURCES.txt` & `pytorch-calibrated-0.1.1/pytorch_calibrated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/tests/test_categorical_calibrator.py` & `pytorch-calibrated-0.1.1/tests/test_categorical_calibrator.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/tests/test_configs.py` & `pytorch-calibrated-0.1.1/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/tests/test_data.py` & `pytorch-calibrated-0.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/tests/test_linear.py` & `pytorch-calibrated-0.1.1/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/tests/test_models.py` & `pytorch-calibrated-0.1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pytorch-calibrated-0.0.2/tests/test_numerical_calibrator.py` & `pytorch-calibrated-0.1.1/tests/test_numerical_calibrator.py`

 * *Files identical despite different names*

