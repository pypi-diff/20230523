# Comparing `tmp/mlforecast-0.7.2.tar.gz` & `tmp/mlforecast-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.7.2.tar", last modified: Tue May 16 02:10:05 2023, max compression
+gzip compressed data, was "mlforecast-0.7.3.tar", last modified: Tue May 23 01:55:50 2023, max compression
```

## Comparing `mlforecast-0.7.2.tar` & `mlforecast-0.7.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.265344 mlforecast-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-16 02:09:54.000000 mlforecast-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-05-16 02:09:54.000000 mlforecast-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 02:09:54.000000 mlforecast-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-16 02:10:05.265344 mlforecast-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-05-16 02:09:54.000000 mlforecast-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.257344 mlforecast-0.7.2/mlforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28756 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.261344 mlforecast-0.7.2/mlforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.261344 mlforecast-0.7.2/mlforecast/distributed/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.261344 mlforecast-0.7.2/mlforecast/distributed/models/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/dask/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/dask/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.265344 mlforecast-0.7.2/mlforecast/distributed/models/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/ray/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/ray/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.265344 mlforecast-0.7.2/mlforecast/distributed/models/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/spark/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/distributed/models/spark/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    25865 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/lgb_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-16 02:09:54.000000 mlforecast-0.7.2/mlforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:10:05.261344 mlforecast-0.7.2/mlforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-16 02:10:05.000000 mlforecast-0.7.2/mlforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 02:10:05.000000 mlforecast-0.7.2/mlforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:10:05.000000 mlforecast-0.7.2/mlforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:10:05.000000 mlforecast-0.7.2/mlforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-16 02:10:05.000000 mlforecast-0.7.2/mlforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 02:10:05.000000 mlforecast-0.7.2/mlforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-16 02:09:54.000000 mlforecast-0.7.2/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:10:05.265344 mlforecast-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-16 02:09:54.000000 mlforecast-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-23 01:55:41.000000 mlforecast-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-05-23 01:55:41.000000 mlforecast-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:55:41.000000 mlforecast-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-23 01:55:50.569450 mlforecast-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-05-23 01:55:41.000000 mlforecast-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.565450 mlforecast-0.7.3/mlforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28756 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/dask/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/dask/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/ray/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/ray/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast/distributed/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/spark/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/distributed/models/spark/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25865 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/lgb_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-23 01:55:41.000000 mlforecast-0.7.3/mlforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:55:50.569450 mlforecast-0.7.3/mlforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 01:55:50.000000 mlforecast-0.7.3/mlforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-23 01:55:41.000000 mlforecast-0.7.3/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:55:50.569450 mlforecast-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-23 01:55:41.000000 mlforecast-0.7.3/setup.py
```

### Comparing `mlforecast-0.7.2/CONTRIBUTING.md` & `mlforecast-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/LICENSE` & `mlforecast-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/PKG-INFO` & `mlforecast-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.7.2
+Version: 0.7.3
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.7.2/README.md` & `mlforecast-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/_modidx.py` & `mlforecast-0.7.3/mlforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/core.py` & `mlforecast-0.7.3/mlforecast/core.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/distributed/forecast.py` & `mlforecast-0.7.3/mlforecast/distributed/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/distributed/models/dask/lgb.py` & `mlforecast-0.7.3/mlforecast/distributed/models/dask/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/distributed/models/dask/xgb.py` & `mlforecast-0.7.3/mlforecast/distributed/models/dask/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/distributed/models/ray/xgb.py` & `mlforecast-0.7.3/mlforecast/distributed/models/ray/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/distributed/models/spark/lgb.py` & `mlforecast-0.7.3/mlforecast/distributed/models/spark/lgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/distributed/models/spark/xgb.py` & `mlforecast-0.7.3/mlforecast/distributed/models/spark/xgb.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/forecast.py` & `mlforecast-0.7.3/mlforecast/forecast.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/grouped_array.py` & `mlforecast-0.7.3/mlforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/lgb_cv.py` & `mlforecast-0.7.3/mlforecast/lgb_cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,31 +21,22 @@
     Lags,
     TimeSeries,
 )
 from .utils import backtest_splits
 from .target_transforms import BaseTargetTransform
 
 # %% ../nbs/lgb_cv.ipynb 5
-def _mape(y_true, y_pred):
+def _mape(y_true, y_pred, ids, _dates):
     abs_pct_err = abs(y_true - y_pred) / y_true
-    return (
-        abs_pct_err.groupby(y_true.index.get_level_values(0), observed=True)
-        .mean()
-        .mean()
-    )
+    return abs_pct_err.groupby(ids, observed=True).mean().mean()
 
 
-def _rmse(y_true, y_pred):
+def _rmse(y_true, y_pred, ids, _dates):
     sq_err = (y_true - y_pred) ** 2
-    return (
-        sq_err.groupby(y_true.index.get_level_values(0), observed=True)
-        .mean()
-        .pow(0.5)
-        .mean()
-    )
+    return sq_err.groupby(ids, observed=True).mean().pow(0.5).mean()
 
 
 _metric2fn = {"mape": _mape, "rmse": _rmse}
 
 
 def _update(bst, n):
     for _ in range(n):
@@ -196,15 +187,15 @@
             self.weights = np.full(n_windows, 1 / n_windows)
         elif len(weights) != n_windows:
             raise ValueError("Must specify as many weights as the number of windows")
         else:
             self.weights = np.asarray(weights)
         if callable(metric):
             self.metric_fn = metric
-            self.metric_name = "custom_metric"
+            self.metric_name = metric.__name__
         else:
             if metric not in _metric2fn:
                 raise ValueError(
                     f'{metric} is not one of the implemented metrics: ({", ".join(_metric2fn.keys())})'
                 )
             self.metric_fn = _metric2fn[metric]
             self.metric_name = metric
@@ -260,15 +251,20 @@
                 bst=bst,
                 valid=valid,
                 n=num_iterations,
                 h=self.window_size,
                 before_predict_callback=before_predict_callback,
                 after_predict_callback=after_predict_callback,
             )
-            metric_values[j] = self.metric_fn(preds[self.target_col], preds["Booster"])
+            metric_values[j] = self.metric_fn(
+                preds[self.target_col],
+                preds["Booster"],
+                preds[self.id_col],
+                preds[self.time_col],
+            )
 
     def _multithreaded_partial_fit(
         self,
         metric_values,
         num_iterations,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
@@ -285,15 +281,20 @@
                     h=self.window_size,
                     before_predict_callback=before_predict_callback,
                     after_predict_callback=after_predict_callback,
                 )
                 futures.append(future)
             cv_preds = [f.result() for f in futures]
         metric_values[:] = [
-            self.metric_fn(preds[self.target_col], preds["Booster"])
+            self.metric_fn(
+                preds[self.target_col],
+                preds["Booster"],
+                preds[self.id_col],
+                preds[self.time_col],
+            )
             for preds in cv_preds
         ]
 
     def partial_fit(
         self,
         num_iterations: int,
         before_predict_callback: Optional[Callable] = None,
```

### Comparing `mlforecast-0.7.2/mlforecast/target_transforms.py` & `mlforecast-0.7.3/mlforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast/utils.py` & `mlforecast-0.7.3/mlforecast/utils.py`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.7.3/mlforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.7.2
+Version: 0.7.3
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mlforecast-0.7.2/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.7.3/mlforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlforecast-0.7.2/settings.ini` & `mlforecast-0.7.3/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.7.2
+version = 0.7.3
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
 requirements = numba pandas scikit-learn window-ops
```

### Comparing `mlforecast-0.7.2/setup.py` & `mlforecast-0.7.3/setup.py`

 * *Files identical despite different names*

