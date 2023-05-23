# Comparing `tmp/modified-thompson-tau-test-0.1.2.tar.gz` & `tmp/modified-thompson-tau-test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modified-thompson-tau-test-0.1.2.tar", last modified: Mon Oct  4 05:45:13 2021, max compression
+gzip compressed data, was "modified-thompson-tau-test-0.1.3.tar", last modified: Tue May 23 18:50:39 2023, max compression
```

## Comparing `modified-thompson-tau-test-0.1.2.tar` & `modified-thompson-tau-test-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-10-04 05:45:13.031829 modified-thompson-tau-test-0.1.2/
--rw-rw-rw-   0        0        0     1083 2021-10-04 05:44:41.000000 modified-thompson-tau-test-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1079 2021-10-04 05:45:13.031829 modified-thompson-tau-test-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      556 2021-10-04 05:44:41.000000 modified-thompson-tau-test-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2021-10-04 05:45:13.031829 modified-thompson-tau-test-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      796 2021-10-04 05:44:41.000000 modified-thompson-tau-test-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-04 05:45:13.016189 modified-thompson-tau-test-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2021-10-04 05:45:13.031829 modified-thompson-tau-test-0.1.2/src/Modified_Thompson_Tau_Test/
--rw-rw-rw-   0        0        0       70 2021-10-04 05:44:41.000000 modified-thompson-tau-test-0.1.2/src/Modified_Thompson_Tau_Test/__init__.py
--rw-rw-rw-   0        0        0     6290 2021-10-04 05:44:41.000000 modified-thompson-tau-test-0.1.2/src/Modified_Thompson_Tau_Test/modified_thompson_tau_test.py
-drwxrwxrwx   0        0        0        0 2021-10-04 05:45:13.031829 modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/
--rw-rw-rw-   0        0        0     1079 2021-10-04 05:45:12.000000 modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2021-10-04 05:45:13.000000 modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-04 05:45:12.000000 modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-10-04 05:45:12.000000 modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2021-10-04 05:45:12.000000 modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 18:50:39.565354 modified-thompson-tau-test-0.1.3/
+-rw-rw-rw-   0        0        0     1062 2023-05-23 18:49:46.000000 modified-thompson-tau-test-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1038 2023-05-23 18:50:39.565354 modified-thompson-tau-test-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-05-23 18:49:46.000000 modified-thompson-tau-test-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 18:50:39.565354 modified-thompson-tau-test-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-05-23 18:49:46.000000 modified-thompson-tau-test-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:50:39.549729 modified-thompson-tau-test-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 18:50:39.565354 modified-thompson-tau-test-0.1.3/src/Modified_Thompson_Tau_Test/
+-rw-rw-rw-   0        0        0       70 2023-05-23 18:49:46.000000 modified-thompson-tau-test-0.1.3/src/Modified_Thompson_Tau_Test/__init__.py
+-rw-rw-rw-   0        0        0     6185 2023-05-23 18:49:46.000000 modified-thompson-tau-test-0.1.3/src/Modified_Thompson_Tau_Test/modified_thompson_tau_test.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:50:39.565354 modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/
+-rw-rw-rw-   0        0        0     1038 2023-05-23 18:50:39.000000 modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-23 18:50:39.000000 modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 18:50:39.000000 modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 18:50:39.000000 modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-23 18:50:39.000000 modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/top_level.txt
```

### Comparing `modified-thompson-tau-test-0.1.2/PKG-INFO` & `modified-thompson-tau-test-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: modified-thompson-tau-test
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of Modified Thompson Tau Test in Python
 Home-page: https://github.com/vvaezian/modified_thompson_tau_test
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Installation
@@ -21,20 +19,18 @@
 ```python
 from Modified_Thompson_Tau_Test.modified_thompson_tau_test import run_modified_thompson_tau_test
 ```
 You can pass a list, a Pandas Series or a Pandas DataFrame to the function:
 ```python
 run_modified_thompson_tau_test([2, 3, -50, 1, 0, 10, 1000])
 ```
-The function returns the results as a Pandas DataFrame where the column `is_outlier` shows the result.
+The function returns the results as a Pandas DataFrame where the column `is_outlier` shows the result:
 ```
  	0 	is_outlier
 2 	-50 	1
 4 	0 	0
 3 	1 	0
 0 	2 	0
 1 	3 	0
 5 	10 	1
 6 	1000 	1
 ```
-
-
```

### Comparing `modified-thompson-tau-test-0.1.2/src/Modified_Thompson_Tau_Test/modified_thompson_tau_test.py` & `modified-thompson-tau-test-0.1.3/src/Modified_Thompson_Tau_Test/modified_thompson_tau_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-
-def run_modified_thompson_tau_test(data, target_column_index=None, target_column_name=None, strictness=3, is_sorted=False):
-  '''
-  Run the Modified Thompson Tau Test on the given data to determine which elements are outliers.
-  
-  Keyword arguments:
-  data -- a list, Series, or DataFrame that containes the data that needs to be evaluated
-  target_column_index -- index of the column that needs to be evaluated
-  target_column_name -- name of the column that needs to be evaluated
-  strictness -- how aggresive the outlier detection should be.
-  is_sorted -- indicating whether data is already sorted (useful for large datasets)
-  '''
-  import pandas as pd
-  assert type(data) in [ pd.DataFrame, pd.Series, list ]
-  
-  ######## making sure we have the data we need ########
-  if type(data) == pd.DataFrame:
-    if target_column_index is None:
-      if target_column_name is None:
-        if len(data.columns) > 1:
-          raise ValueError('Either the name or index of the target column needs to be provided.')
-        else:
-          target_column_index = 0
-      else:
-        target_column_index = data.columns.index(target_column_name)
-    df = data
-    
-  if type(data) == pd.Series:
-    target_column_index = 0
-    df = pd.DataFrame(data)
-    
-  if type(data) == list:
-    if target_column_index is None:
-      # assuming the list is one-dimentional
-      target_column_index = 0
-    df = pd.DataFrame(data)
-  
-  
-  ######## Helper Functions ########
-  def get_T_critical_value(n, strictness=3):
-    '''Get the value from the t-Student distribution for the given n.'''
-    mapping = {
-      1:[ { 1:3.078,2:1.886,3:1.638,4:1.533,5:1.476,6:1.440,7:1.415,8:1.397,9:1.383,10:1.372,11:1.363,12:1.356,
-            13:1.350,14:1.345,15:1.341,16:1.337,17:1.333,18:1.330,19:1.328,20:1.325,21:1.323,22:1.321,23:1.319,
-            24:1.318,25:1.316,26:1.315,27:1.314,28:1.313,29:1.311,30:1.310,40:1.303,50:1.299,60:1.296,80:1.292,
-            100:1.290,120:1.289}, 1.282 ],
-      2:[ { 1:6.314,2:2.920,3:2.353,4:2.132,5:2.015,6:1.943,7:1.895,8:1.860,9:1.833,10:1.812,11:1.796,12:1.782,
-            13:1.771,14:1.761,15:1.753,16:1.746,17:1.740,18:1.734,19:1.729,20:1.725,21:1.721,22:1.717,23:1.714,
-            24:1.711,25:1.708,26:1.706,27:1.703,28:1.701,29:1.699,30:1.697,40:1.684,50:1.676,60:1.671,80:1.664,
-            100:1.660,120:1.658}, 1.645 ],
-      3:[ { 1:12.71, 2:4.303, 3:3.182, 4:2.776, 5:2.571, 6:2.447, 7:2.365, 8:2.306, 9:2.262, 10:2.228, 11:2.201, 
-            12:2.179, 13:2.160, 14:2.145, 15:2.131, 16:2.120, 17:2.110, 18:2.101, 19:2.093, 20:2.086, 21:2.080, 
-            22:2.074, 23:2.069, 24:2.064, 25:2.060, 26:2.056, 27:2.052, 28:2.048, 29:2.045, 30:2.042, 40:2.021, 
-            50:2.009, 60:2.000, 80:1.990, 100:1.984, 120:1.980}, 1.96 ],
-      4:[ { 1:31.82 ,2:6.965,3:4.541,4:3.747,5:3.365,6:3.143,7:2.998,8:2.896,9:2.821,10:2.764,11:2.718,12:2.681,
-            13:2.650,14:2.624,15:2.602,16:2.583,17:2.567,18:2.552,19:2.539,20:2.528,21:2.518,22:2.508,23:2.500,
-            24:2.492,25:2.485,26:2.479,27:2.473,28:2.467,29:2.462,30:2.457,40:2.423,50:2.403,60:2.390,80:2.374,
-            100:2.364,120:2.358}, 2.326 ],
-      5:[ { 1:63.66,2:9.925,3:5.841,4:4.604,5:4.032,6:3.707,7:3.499,8:3.355,9:3.250,10:3.169,11:3.106,12:3.055,
-            13:3.012,14:2.977,15:2.947,16:2.921,17:2.898,18:2.878,19:2.861,20:2.845,21:2.831,22:2.819,23:2.807,
-            24:2.797,25:2.787,26:2.779,27:2.771,28:2.763,29:2.756,30:2.750,40:2.704,50:2.678,60:2.660,80:2.639,
-            100:2.626,120:2.617}, 2.576 ]
-    }
-    t, inf_val = mapping[strictness]
-    for key, val in t.items():
-      if n <= key:
-        return val
-    return inf_val
-
-
-
-  def calc_tau(n, strictness=3):
-    '''Calculate the rejection threshold.'''
-    if n < 3:
-      raise ValueError
-    import math
-    t = get_T_critical_value(n - 2, strictness=strictness)
-    return (t * (n - 1))/(math.sqrt(n) * math.sqrt(n - 2 + t**2)) 
-
-
-
-  def run_alg_one_step(sorted_series, strictness=3):
-    '''
-    Determine whether the biggest (absolute value) element of the given series is an outlier or not
-    using the Modified Thompson Tau Test.
-    '''
-    n = len(sorted_series)
-    if n < 3:
-      return (0, None)
-
-    sample_mean = sorted_series.mean()
-    first_element = sorted_series.iloc[0]
-    last_element = sorted_series.iloc[-1]
-
-    if abs(first_element) > abs(last_element):
-      candidate_position = 0  # first
-      outlier_candidate = first_element
-    else:
-      candidate_position = -1  # last
-      outlier_candidate = last_element
-
-    rejection_region = calc_tau(n, strictness=strictness)
-    sample_std = sorted_series.std()
-    delta = abs(outlier_candidate - sample_mean)/sample_std
-    return (1, candidate_position) if delta > rejection_region else (0, None)
-  
-  
-
-  ######## Processing ########
-  # adding is_outlier column to hold the data for output
-  df_with_outlier_col = df
-  df_with_outlier_col['is_outlier'] = 0
-  df_with_outlier_col_sorted = df_with_outlier_col if is_sorted else df_with_outlier_col.sort_values(by=target_column_index)
-  
-  # deep-copying the target column (sorted) to be used by the alg
-  import copy
-  target_column_sorted_copy = copy.deepcopy(df_with_outlier_col_sorted[df_with_outlier_col_sorted.columns[target_column_index]])
-  
-  # running the algorithm on the sorted target column 
-  while True:
-    # run the alg for the biggest element (absolute value), get the result and update the data accordingly
-    res, position = run_alg_one_step(target_column_sorted_copy, strictness=strictness)
-    if res == 0:  # The current records is not an outlier, so the rest of the records are not outlier either.
-      break
-    else: # The current records is an outlier. Remove it and run the test on the rest of the dataset
-      if position == 0:
-        df_with_outlier_col_sorted.loc[target_column_sorted_copy.index[0], 'is_outlier'] = 1
-        target_column_sorted_copy = target_column_sorted_copy.iloc[1:]
-      else:
-        df_with_outlier_col_sorted.loc[target_column_sorted_copy.index[-1], 'is_outlier'] = 1
-        target_column_sorted_copy = target_column_sorted_copy.iloc[:-1]
-  
-  return df_with_outlier_col_sorted
+
+def run_modified_thompson_tau_test(data, target_column_index=None, target_column_name=None, strictness=3, is_sorted=False):
+  '''
+  Run the Modified Thompson Tau Test on the given data to determine which elements are outliers.
+  
+  Keyword arguments:
+  data -- a list, Series, or DataFrame that containes the data that needs to be evaluated
+  target_column_index -- index of the column that needs to be evaluated
+  target_column_name -- name of the column that needs to be evaluated
+  strictness -- how aggresive the outlier detection should be.
+  is_sorted -- indicating whether data is already sorted (useful for large datasets)
+  '''
+  import pandas as pd
+  assert type(data) in [ pd.DataFrame, pd.Series, list ]
+  
+  ######## making sure we have the data we need ########
+  if type(data) == pd.DataFrame:
+    if target_column_index is None:
+      if target_column_name is None:
+        if len(data.columns) > 1:
+          raise ValueError('Either the name or index of the target column needs to be provided.')
+        else:
+          target_column_index = 0
+      else:
+        target_column_index = data.columns.index(target_column_name)
+    df = data
+    
+  if type(data) == pd.Series:
+    target_column_index = 0
+    df = pd.DataFrame(data)
+    
+  if type(data) == list:
+    if target_column_index is None:
+      # assuming the list is one-dimentional
+      target_column_index = 0
+    df = pd.DataFrame(data)
+  
+  
+  ######## Helper Functions ########
+  def get_T_critical_value(n, strictness=3):
+    '''Get the value from the t-Student distribution for the given n.'''
+    mapping = {
+      1:[ { 1:3.078,2:1.886,3:1.638,4:1.533,5:1.476,6:1.440,7:1.415,8:1.397,9:1.383,10:1.372,11:1.363,12:1.356,
+            13:1.350,14:1.345,15:1.341,16:1.337,17:1.333,18:1.330,19:1.328,20:1.325,21:1.323,22:1.321,23:1.319,
+            24:1.318,25:1.316,26:1.315,27:1.314,28:1.313,29:1.311,30:1.310,40:1.303,50:1.299,60:1.296,80:1.292,
+            100:1.290,120:1.289}, 1.282 ],
+      2:[ { 1:6.314,2:2.920,3:2.353,4:2.132,5:2.015,6:1.943,7:1.895,8:1.860,9:1.833,10:1.812,11:1.796,12:1.782,
+            13:1.771,14:1.761,15:1.753,16:1.746,17:1.740,18:1.734,19:1.729,20:1.725,21:1.721,22:1.717,23:1.714,
+            24:1.711,25:1.708,26:1.706,27:1.703,28:1.701,29:1.699,30:1.697,40:1.684,50:1.676,60:1.671,80:1.664,
+            100:1.660,120:1.658}, 1.645 ],
+      3:[ { 1:12.71, 2:4.303, 3:3.182, 4:2.776, 5:2.571, 6:2.447, 7:2.365, 8:2.306, 9:2.262, 10:2.228, 11:2.201, 
+            12:2.179, 13:2.160, 14:2.145, 15:2.131, 16:2.120, 17:2.110, 18:2.101, 19:2.093, 20:2.086, 21:2.080, 
+            22:2.074, 23:2.069, 24:2.064, 25:2.060, 26:2.056, 27:2.052, 28:2.048, 29:2.045, 30:2.042, 40:2.021, 
+            50:2.009, 60:2.000, 80:1.990, 100:1.984, 120:1.980}, 1.96 ],
+      4:[ { 1:31.82 ,2:6.965,3:4.541,4:3.747,5:3.365,6:3.143,7:2.998,8:2.896,9:2.821,10:2.764,11:2.718,12:2.681,
+            13:2.650,14:2.624,15:2.602,16:2.583,17:2.567,18:2.552,19:2.539,20:2.528,21:2.518,22:2.508,23:2.500,
+            24:2.492,25:2.485,26:2.479,27:2.473,28:2.467,29:2.462,30:2.457,40:2.423,50:2.403,60:2.390,80:2.374,
+            100:2.364,120:2.358}, 2.326 ],
+      5:[ { 1:63.66,2:9.925,3:5.841,4:4.604,5:4.032,6:3.707,7:3.499,8:3.355,9:3.250,10:3.169,11:3.106,12:3.055,
+            13:3.012,14:2.977,15:2.947,16:2.921,17:2.898,18:2.878,19:2.861,20:2.845,21:2.831,22:2.819,23:2.807,
+            24:2.797,25:2.787,26:2.779,27:2.771,28:2.763,29:2.756,30:2.750,40:2.704,50:2.678,60:2.660,80:2.639,
+            100:2.626,120:2.617}, 2.576 ]
+    }
+    t, inf_val = mapping[strictness]
+    for key, val in t.items():
+      if n <= key:
+        return val
+    return inf_val
+
+
+
+  def calc_tau(n, strictness=3):
+    '''Calculate the rejection threshold.'''
+    if n < 3:
+      raise ValueError
+    import math
+    t = get_T_critical_value(n - 2, strictness=strictness)
+    return (t * (n - 1))/(math.sqrt(n) * math.sqrt(n - 2 + t**2)) 
+
+
+
+  def run_alg_one_step(sorted_series, strictness=3):
+    '''
+    Determine whether the biggest (absolute value) element of the given series is an outlier or not
+    using the Modified Thompson Tau Test.
+    '''
+    n = len(sorted_series)
+    if n < 3:
+      return (0, None)
+
+    sample_mean = sorted_series.mean()
+    first_element = sorted_series.iloc[0]
+    last_element = sorted_series.iloc[-1]
+
+    if abs(first_element - sample_mean) > abs(last_element - sample_mean):
+      candidate_position = 0  # first
+      outlier_candidate = first_element
+    else:
+      candidate_position = -1  # last
+      outlier_candidate = last_element
+
+    rejection_region = calc_tau(n, strictness=strictness)
+    sample_std = sorted_series.std()
+    delta = abs(outlier_candidate - sample_mean)/sample_std
+    return (1, candidate_position) if delta > rejection_region else (0, None)
+  
+  
+
+  ######## Processing ########
+  # adding is_outlier column to hold the data for output
+  df_with_outlier_col = df
+  df_with_outlier_col['is_outlier'] = 0
+  df_with_outlier_col_sorted = df_with_outlier_col if is_sorted else df_with_outlier_col.sort_values(by=target_column_index)
+  
+  # deep-copying the target column (sorted) to be used by the alg
+  import copy
+  target_column_sorted_copy = copy.deepcopy(df_with_outlier_col_sorted[df_with_outlier_col_sorted.columns[target_column_index]])
+  
+  # running the algorithm on the sorted target column 
+  while True:
+    # run the alg for the biggest element (absolute value), get the result and update the data accordingly
+    res, position = run_alg_one_step(target_column_sorted_copy, strictness=strictness)
+    if res == 0:  # The current records is not an outlier, so the rest of the records are not outlier either.
+      break
+    else: # The current records is an outlier. Remove it and run the test on the rest of the dataset
+      if position == 0:
+        df_with_outlier_col_sorted.loc[target_column_sorted_copy.index[0], 'is_outlier'] = 1
+        target_column_sorted_copy = target_column_sorted_copy.iloc[1:]
+      else:
+        df_with_outlier_col_sorted.loc[target_column_sorted_copy.index[-1], 'is_outlier'] = 1
+        target_column_sorted_copy = target_column_sorted_copy.iloc[:-1]
+  
+  return df_with_outlier_col_sorted
```

### Comparing `modified-thompson-tau-test-0.1.2/src/modified_thompson_tau_test.egg-info/PKG-INFO` & `modified-thompson-tau-test-0.1.3/src/modified_thompson_tau_test.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: modified-thompson-tau-test
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of Modified Thompson Tau Test in Python
 Home-page: https://github.com/vvaezian/modified_thompson_tau_test
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Installation
@@ -21,20 +19,18 @@
 ```python
 from Modified_Thompson_Tau_Test.modified_thompson_tau_test import run_modified_thompson_tau_test
 ```
 You can pass a list, a Pandas Series or a Pandas DataFrame to the function:
 ```python
 run_modified_thompson_tau_test([2, 3, -50, 1, 0, 10, 1000])
 ```
-The function returns the results as a Pandas DataFrame where the column `is_outlier` shows the result.
+The function returns the results as a Pandas DataFrame where the column `is_outlier` shows the result:
 ```
  	0 	is_outlier
 2 	-50 	1
 4 	0 	0
 3 	1 	0
 0 	2 	0
 1 	3 	0
 5 	10 	1
 6 	1000 	1
 ```
-
-
```

