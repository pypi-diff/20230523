# Comparing `tmp/smoltools-1.0.8.tar.gz` & `tmp/smoltools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smoltools-1.0.8.tar", last modified: Wed Feb 15 07:00:10 2023, max compression
+gzip compressed data, was "smoltools-1.0.9.tar", last modified: Thu Feb 16 01:08:03 2023, max compression
```

## Comparing `smoltools-1.0.8.tar` & `smoltools-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.156442 smoltools-1.0.8/
--rw-r--r--   0 aysung     (502) staff       (20)     1068 2022-06-15 04:46:04.000000 smoltools-1.0.8/LICENSE
--rw-r--r--   0 aysung     (502) staff       (20)      601 2023-02-15 07:00:10.156523 smoltools-1.0.8/PKG-INFO
--rw-r--r--   0 aysung     (502) staff       (20)       72 2022-06-15 04:46:04.000000 smoltools-1.0.8/README.md
--rw-r--r--   0 aysung     (502) staff       (20)      103 2022-05-13 20:02:23.000000 smoltools-1.0.8/pyproject.toml
--rw-r--r--   0 aysung     (502) staff       (20)      735 2023-02-15 07:00:10.156830 smoltools-1.0.8/setup.cfg
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.149452 smoltools-1.0.8/smoltools/
--rw-r--r--   0 aysung     (502) staff       (20)      170 2023-02-15 06:59:35.000000 smoltools-1.0.8/smoltools/__init__.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.150077 smoltools-1.0.8/smoltools/calculate/
--rw-r--r--   0 aysung     (502) staff       (20)      115 2022-07-09 17:06:33.000000 smoltools-1.0.8/smoltools/calculate/__init__.py
--rw-r--r--   0 aysung     (502) staff       (20)     2525 2022-07-09 17:06:33.000000 smoltools-1.0.8/smoltools/calculate/distance.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.151970 smoltools-1.0.8/smoltools/fret0/
--rw-r--r--   0 aysung     (502) staff       (20)      309 2022-07-10 15:26:50.000000 smoltools-1.0.8/smoltools/fret0/__init__.py
--rw-r--r--   0 aysung     (502) staff       (20)     1983 2022-07-09 18:18:04.000000 smoltools-1.0.8/smoltools/fret0/efficiency.py
--rw-r--r--   0 aysung     (502) staff       (20)     1857 2022-07-09 17:06:33.000000 smoltools-1.0.8/smoltools/fret0/main.py
--rw-r--r--   0 aysung     (502) staff       (20)     6772 2022-07-15 18:23:41.000000 smoltools-1.0.8/smoltools/fret0/plots.py
--rw-r--r--   0 aysung     (502) staff       (20)      364 2022-07-09 17:06:33.000000 smoltools-1.0.8/smoltools/fret0/utils.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.153058 smoltools-1.0.8/smoltools/noesy_neighbors/
--rw-r--r--   0 aysung     (502) staff       (20)      509 2023-02-15 03:04:35.000000 smoltools-1.0.8/smoltools/noesy_neighbors/__init__.py
--rw-r--r--   0 aysung     (502) staff       (20)     4231 2023-02-15 03:04:35.000000 smoltools-1.0.8/smoltools/noesy_neighbors/main.py
--rw-r--r--   0 aysung     (502) staff       (20)     8687 2023-02-15 06:59:35.000000 smoltools-1.0.8/smoltools/noesy_neighbors/plots.py
--rw-r--r--   0 aysung     (502) staff       (20)     2143 2023-02-15 03:04:35.000000 smoltools-1.0.8/smoltools/noesy_neighbors/utils.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.154638 smoltools-1.0.8/smoltools/pdbtools/
--rw-r--r--   0 aysung     (502) staff       (20)      193 2022-07-09 17:06:33.000000 smoltools-1.0.8/smoltools/pdbtools/__init__.py
--rw-r--r--   0 aysung     (502) staff       (20)     1049 2022-07-09 17:06:33.000000 smoltools-1.0.8/smoltools/pdbtools/coordinates.py
--rw-r--r--   0 aysung     (502) staff       (20)      547 2022-07-10 15:26:50.000000 smoltools-1.0.8/smoltools/pdbtools/exceptions.py
--rw-r--r--   0 aysung     (502) staff       (20)     1167 2022-07-08 18:27:08.000000 smoltools-1.0.8/smoltools/pdbtools/load.py
--rw-r--r--   0 aysung     (502) staff       (20)     3524 2022-07-10 15:26:50.000000 smoltools-1.0.8/smoltools/pdbtools/select.py
--rw-r--r--   0 aysung     (502) staff       (20)      565 2022-07-15 18:16:20.000000 smoltools-1.0.8/smoltools/pdbtools/utils.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.155359 smoltools-1.0.8/smoltools/rate_my_plate/
--rw-r--r--   0 aysung     (502) staff       (20)      214 2023-02-15 06:59:35.000000 smoltools-1.0.8/smoltools/rate_my_plate/__init__.py
--rw-r--r--   0 aysung     (502) staff       (20)     3268 2023-02-15 06:59:35.000000 smoltools-1.0.8/smoltools/rate_my_plate/main.py
--rw-r--r--   0 aysung     (502) staff       (20)     2157 2023-02-15 06:59:35.000000 smoltools-1.0.8/smoltools/rate_my_plate/plots.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.155657 smoltools-1.0.8/smoltools/resources/
--rw-r--r--   0 aysung     (502) staff       (20)        0 2022-06-17 03:28:00.000000 smoltools-1.0.8/smoltools/resources/__init__.py
--rw-r--r--   0 aysung     (502) staff       (20)       79 2022-06-19 15:05:54.000000 smoltools-1.0.8/smoltools/resources/colors.py
-drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-15 07:00:10.156316 smoltools-1.0.8/smoltools.egg-info/
--rw-r--r--   0 aysung     (502) staff       (20)      601 2023-02-15 07:00:10.000000 smoltools-1.0.8/smoltools.egg-info/PKG-INFO
--rw-r--r--   0 aysung     (502) staff       (20)      925 2023-02-15 07:00:10.000000 smoltools-1.0.8/smoltools.egg-info/SOURCES.txt
--rw-r--r--   0 aysung     (502) staff       (20)        1 2023-02-15 07:00:10.000000 smoltools-1.0.8/smoltools.egg-info/dependency_links.txt
--rw-r--r--   0 aysung     (502) staff       (20)       10 2023-02-15 07:00:10.000000 smoltools-1.0.8/smoltools.egg-info/top_level.txt
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.413770 smoltools-1.0.9/
+-rw-r--r--   0 aysung     (502) staff       (20)     1068 2022-06-15 04:46:04.000000 smoltools-1.0.9/LICENSE
+-rw-r--r--   0 aysung     (502) staff       (20)      601 2023-02-16 01:08:03.413926 smoltools-1.0.9/PKG-INFO
+-rw-r--r--   0 aysung     (502) staff       (20)       72 2022-06-15 04:46:04.000000 smoltools-1.0.9/README.md
+-rw-r--r--   0 aysung     (502) staff       (20)      103 2022-05-13 20:02:23.000000 smoltools-1.0.9/pyproject.toml
+-rw-r--r--   0 aysung     (502) staff       (20)      742 2023-02-16 01:08:03.414404 smoltools-1.0.9/setup.cfg
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.406806 smoltools-1.0.9/smoltools/
+-rw-r--r--   0 aysung     (502) staff       (20)      170 2023-02-15 06:59:35.000000 smoltools-1.0.9/smoltools/__init__.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.407612 smoltools-1.0.9/smoltools/calculate/
+-rw-r--r--   0 aysung     (502) staff       (20)      115 2022-07-09 17:06:33.000000 smoltools-1.0.9/smoltools/calculate/__init__.py
+-rw-r--r--   0 aysung     (502) staff       (20)     2525 2022-07-09 17:06:33.000000 smoltools-1.0.9/smoltools/calculate/distance.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.409060 smoltools-1.0.9/smoltools/fret0/
+-rw-r--r--   0 aysung     (502) staff       (20)      309 2022-07-10 15:26:50.000000 smoltools-1.0.9/smoltools/fret0/__init__.py
+-rw-r--r--   0 aysung     (502) staff       (20)     1983 2022-07-09 18:18:04.000000 smoltools-1.0.9/smoltools/fret0/efficiency.py
+-rw-r--r--   0 aysung     (502) staff       (20)     1857 2022-07-09 17:06:33.000000 smoltools-1.0.9/smoltools/fret0/main.py
+-rw-r--r--   0 aysung     (502) staff       (20)     6772 2022-07-15 18:23:41.000000 smoltools-1.0.9/smoltools/fret0/plots.py
+-rw-r--r--   0 aysung     (502) staff       (20)      364 2022-07-09 17:06:33.000000 smoltools-1.0.9/smoltools/fret0/utils.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.410197 smoltools-1.0.9/smoltools/noesy_neighbors/
+-rw-r--r--   0 aysung     (502) staff       (20)      509 2023-02-15 03:04:35.000000 smoltools-1.0.9/smoltools/noesy_neighbors/__init__.py
+-rw-r--r--   0 aysung     (502) staff       (20)     4231 2023-02-15 03:04:35.000000 smoltools-1.0.9/smoltools/noesy_neighbors/main.py
+-rw-r--r--   0 aysung     (502) staff       (20)     8687 2023-02-15 06:59:35.000000 smoltools-1.0.9/smoltools/noesy_neighbors/plots.py
+-rw-r--r--   0 aysung     (502) staff       (20)     2143 2023-02-15 03:04:35.000000 smoltools-1.0.9/smoltools/noesy_neighbors/utils.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.411589 smoltools-1.0.9/smoltools/pdbtools/
+-rw-r--r--   0 aysung     (502) staff       (20)      193 2022-07-09 17:06:33.000000 smoltools-1.0.9/smoltools/pdbtools/__init__.py
+-rw-r--r--   0 aysung     (502) staff       (20)     1049 2022-07-09 17:06:33.000000 smoltools-1.0.9/smoltools/pdbtools/coordinates.py
+-rw-r--r--   0 aysung     (502) staff       (20)      547 2022-07-10 15:26:50.000000 smoltools-1.0.9/smoltools/pdbtools/exceptions.py
+-rw-r--r--   0 aysung     (502) staff       (20)     1167 2022-07-08 18:27:08.000000 smoltools-1.0.9/smoltools/pdbtools/load.py
+-rw-r--r--   0 aysung     (502) staff       (20)     3524 2022-07-10 15:26:50.000000 smoltools-1.0.9/smoltools/pdbtools/select.py
+-rw-r--r--   0 aysung     (502) staff       (20)      565 2022-07-15 18:16:20.000000 smoltools-1.0.9/smoltools/pdbtools/utils.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.412450 smoltools-1.0.9/smoltools/rate_my_plate/
+-rw-r--r--   0 aysung     (502) staff       (20)      214 2023-02-15 06:59:35.000000 smoltools-1.0.9/smoltools/rate_my_plate/__init__.py
+-rw-r--r--   0 aysung     (502) staff       (20)     3030 2023-02-15 18:38:47.000000 smoltools-1.0.9/smoltools/rate_my_plate/main.py
+-rw-r--r--   0 aysung     (502) staff       (20)     2162 2023-02-15 18:38:52.000000 smoltools-1.0.9/smoltools/rate_my_plate/plots.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.412837 smoltools-1.0.9/smoltools/resources/
+-rw-r--r--   0 aysung     (502) staff       (20)        0 2022-06-17 03:28:00.000000 smoltools-1.0.9/smoltools/resources/__init__.py
+-rw-r--r--   0 aysung     (502) staff       (20)       79 2022-06-19 15:05:54.000000 smoltools-1.0.9/smoltools/resources/colors.py
+drwxr-xr-x   0 aysung     (502) staff       (20)        0 2023-02-16 01:08:03.413617 smoltools-1.0.9/smoltools.egg-info/
+-rw-r--r--   0 aysung     (502) staff       (20)      601 2023-02-16 01:08:03.000000 smoltools-1.0.9/smoltools.egg-info/PKG-INFO
+-rw-r--r--   0 aysung     (502) staff       (20)      925 2023-02-16 01:08:03.000000 smoltools-1.0.9/smoltools.egg-info/SOURCES.txt
+-rw-r--r--   0 aysung     (502) staff       (20)        1 2023-02-16 01:08:03.000000 smoltools-1.0.9/smoltools.egg-info/dependency_links.txt
+-rw-r--r--   0 aysung     (502) staff       (20)       10 2023-02-16 01:08:03.000000 smoltools-1.0.9/smoltools.egg-info/top_level.txt
```

### Comparing `smoltools-1.0.8/LICENSE` & `smoltools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/PKG-INFO` & `smoltools-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smoltools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Collection of tools for various single-molecule experiments.
 Home-page: https://github.com/AYSung/smoltools/
 Author: Andrew Sung
 Author-email: aysung300@gmail.com
 Project-URL: Bug Tracker, https://github.com/AYSung/smoltools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `smoltools-1.0.8/setup.cfg` & `smoltools-1.0.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smoltools
-version = 1.0.8
+version = 1.0.9
 author = Andrew Sung
 author_email = aysung300@gmail.com
 description = Collection of tools for various single-molecule experiments.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AYSung/smoltools/
 project_urls = 
@@ -14,15 +14,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 install_requires = 
 	pandas>=1.4.0
 	numpy>=1.22.2
 	altair>=4.2.0
 	scipy>=1.8.0
-	xlrd
+	xlrd>=2.0.1
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >=3.10.4
```

### Comparing `smoltools-1.0.8/smoltools/calculate/distance.py` & `smoltools-1.0.9/smoltools/calculate/distance.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/fret0/efficiency.py` & `smoltools-1.0.9/smoltools/fret0/efficiency.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/fret0/main.py` & `smoltools-1.0.9/smoltools/fret0/main.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/fret0/plots.py` & `smoltools-1.0.9/smoltools/fret0/plots.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/noesy_neighbors/main.py` & `smoltools-1.0.9/smoltools/noesy_neighbors/main.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/noesy_neighbors/plots.py` & `smoltools-1.0.9/smoltools/noesy_neighbors/plots.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/noesy_neighbors/utils.py` & `smoltools-1.0.9/smoltools/noesy_neighbors/utils.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/pdbtools/coordinates.py` & `smoltools-1.0.9/smoltools/pdbtools/coordinates.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/pdbtools/exceptions.py` & `smoltools-1.0.9/smoltools/pdbtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/pdbtools/load.py` & `smoltools-1.0.9/smoltools/pdbtools/load.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/pdbtools/select.py` & `smoltools-1.0.9/smoltools/pdbtools/select.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/pdbtools/utils.py` & `smoltools-1.0.9/smoltools/pdbtools/utils.py`

 * *Files identical despite different names*

### Comparing `smoltools-1.0.8/smoltools/rate_my_plate/main.py` & `smoltools-1.0.9/smoltools/rate_my_plate/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,29 +58,22 @@
 ) -> tuple[float, float]:
     max_value = df.nadh_consumed.max()
     lower_threshold = lower_percent * max_value
     upper_threshold = upper_percent * max_value
     return lower_threshold, upper_threshold
 
 
-def filter_data(df: pd.DataFrame, lower_percent, upper_percent) -> pd.DataFrame:
-    def _get_linear_range(df: pd.DataFrame) -> pd.DataFrame:
-        lower_threshold, upper_threshold = _get_thresholds(
-            df, lower_percent=lower_percent, upper_percent=upper_percent
-        )
-        return df.loc[
-            lambda x: (x.nadh_consumed > lower_threshold)
-            & (x.nadh_consumed < upper_threshold)
-        ]
-
-    return (
-        df.groupby('well', as_index=False)
-        .apply(_get_linear_range)
-        .reset_index(drop=True)
-    )
+def filter_data(
+    df: pd.DataFrame, lower_percent: float, upper_percent: float
+) -> pd.DataFrame:
+    lower_threshold, upper_threshold = _get_thresholds(df, lower_percent, upper_percent)
+    return df.loc[
+        lambda x: (x.nadh_consumed >= lower_threshold)
+        & (x.nadh_consumed <= upper_threshold)
+    ]
 
 
 def _estimate_slope(df: pd.DataFrame) -> float:
     slope = linregress(df.time, df.nadh_consumed)[0]
     return slope
```

### Comparing `smoltools-1.0.8/smoltools/rate_my_plate/plots.py` & `smoltools-1.0.9/smoltools/rate_my_plate/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,46 +18,45 @@
     )
 
 
 def consumption_curve(
     df: pd.DataFrame, lower_percent: float, upper_percent: float
 ) -> alt.Chart:
 
-    df_with_thresholds = df.groupby('well', as_index=False).apply(
-        _add_thresholds, lower_percent=lower_percent, upper_percent=upper_percent
-    )
+    lower_threshold, upper_threshold = _get_thresholds(df, lower_percent, upper_percent)
+
     scatter = (
         alt.Chart()
         .mark_circle(size=60)
         .encode(
             x=alt.X('time', title='Time (minutes)'),
             y=alt.Y('nadh_consumed', title='NADH consumed'),
             opacity=alt.condition(
-                (alt.datum.nadh_consumed > alt.datum.lower_threshold)
-                & (alt.datum.nadh_consumed < alt.datum.upper_threshold),
+                (alt.datum.nadh_consumed >= lower_threshold)
+                & (alt.datum.nadh_consumed <= upper_threshold),
                 alt.value(0.8),
                 alt.value(0.2),
             ),
         )
     ).properties(
         height=100,
         width=150,
     )
 
     upper_rule = (
-        alt.Chart()
+        alt.Chart(pd.DataFrame({'upper_threshold': [upper_threshold]}))
         .mark_rule()
         .encode(y=alt.Y('upper_threshold', title='NADH consumed'))
     )
     lower_rule = (
-        alt.Chart()
+        alt.Chart(pd.DataFrame({'lower_threshold': [lower_threshold]}))
         .mark_rule()
         .encode(y=alt.Y('lower_threshold', title='NADH consumed'))
     )
-    return alt.layer(scatter, upper_rule, lower_rule, data=df_with_thresholds).facet(
+    return alt.layer(scatter, upper_rule, lower_rule, data=df).facet(
         facet=alt.Facet('well:N', title='well', sort=PLATE_ORDER),
         columns=6,
     )
 
 
 def kinetics_curves(df: pd.DataFrame) -> alt.Chart:
     return (
```

### Comparing `smoltools-1.0.8/smoltools.egg-info/PKG-INFO` & `smoltools-1.0.9/smoltools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smoltools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Collection of tools for various single-molecule experiments.
 Home-page: https://github.com/AYSung/smoltools/
 Author: Andrew Sung
 Author-email: aysung300@gmail.com
 Project-URL: Bug Tracker, https://github.com/AYSung/smoltools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `smoltools-1.0.8/smoltools.egg-info/SOURCES.txt` & `smoltools-1.0.9/smoltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

