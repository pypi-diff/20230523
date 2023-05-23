# Comparing `tmp/exergenics-etl-0.5.0.tar.gz` & `tmp/exergenics-etl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-0.5.0.tar", last modified: Mon May 22 07:07:59 2023, max compression
+gzip compressed data, was "exergenics-etl-1.0.0.tar", last modified: Tue May 23 02:54:02 2023, max compression
```

## Comparing `exergenics-etl-0.5.0.tar` & `exergenics-etl-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45201 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/src/exergenics_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-05-22 07:07:56.000000 exergenics-etl-0.5.0/app/exergenics_etl/test/test_exergenics_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:07:59.335723 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 07:07:59.000000 exergenics-etl-0.5.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:07:59.339724 exergenics-etl-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-22 07:07:58.000000 exergenics-etl-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.563222 exergenics-etl-1.0.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.563222 exergenics-etl-1.0.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47357 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/src/exergenics_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33594 2023-05-23 02:54:00.000000 exergenics-etl-1.0.0/app/exergenics_etl/test/test_exergenics_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 02:54:02.000000 exergenics-etl-1.0.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 02:54:02.567221 exergenics-etl-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 02:54:01.000000 exergenics-etl-1.0.0/setup.py
```

### Comparing `exergenics-etl-0.5.0/LICENSE` & `exergenics-etl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-0.5.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.0.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 LENGTH_THRESHOLD = 10
 # The maximum distance between two timestamp column headers that are considered similar
 TIMESTAMP_HEADER_DISTANCE = 4
 LOG_HEADER = ['timepretty', 'observation', 'datapoint']
 TIME, NAME, VALUE = LOG_HEADER
 N_COLUMN_LONG_DATA = 3  # The number of columns in a long-format data table
 DEFAULT_POSITION_DAY = 0  # The default position of the day of month in timestamps
+SUMMARY_COLUMNS = ['count', 'mean', 'std',
+                   'min', '25%', '50%', '75%', 'max']
 
 
 logger = Logger(loggerName='Exergenics-ETL',
                 component='data_modules', subComponent='pre_merged')
 
 
 def hello(name: str) -> None:
@@ -1105,14 +1107,88 @@
 
         assert point not in dfDictFile.keys(), f'Duplicate column header in a single data file.'
         dfDictFile[point] = tempDf
 
     return dfDictFile, filesWithNanColumn
 
 
+def get_point_summary(point: str, df: pd.DataFrame) -> pd.DataFrame:
+    """Generate summary statistics of a point based on its trend log.
+
+    Args:
+        point (str): Point name of the data.
+        df (pd.DataFrame): Trend log of the point.
+
+    Returns:
+        pd.DataFrame: Summary statistics of the given trend log.
+    """
+
+    logger = Logger()
+
+    try:
+
+        # Reformat and transform data
+        df.rename(columns={'datapoint': point}, inplace=True)
+        df[point] = pd.to_numeric(df[point], errors='coerce')
+
+        # Calculate statistics
+        df_summary = df[[point]].describe()
+        # df_summary.loc['count'] = df[point].gt(0).sum()
+        df_summary = df_summary.transpose().round(3)
+
+        # Drop columns that are not in SUMMARY_COLUMNS
+        df_summary = df_summary[df_summary.columns.intersection(
+            SUMMARY_COLUMNS)]
+
+        # Replace pd.NaN with empty string
+        df_summary.fillna(value="", inplace=True)
+
+    except Exception as e:
+        df_summary = pd.DataFrame(
+            data={j: "" for j in SUMMARY_COLUMNS}, index=[point])
+        msg = f"Exception occurred: {e}. Added empty strings as summary statistics instead."
+        logger.warn(msg)
+
+    return df_summary
+
+
+def get_statistical_summary(dfDict: dict) -> pd.DataFrame:
+    """Generate a summary statistics table for the dataframe(s) in the input dictionary.
+
+    Args:
+        dfDict (dict): Dictionary of dataframe(s).
+
+    Raises:
+        Exception: For unknown errors.
+
+    Returns:
+        pd.DataFrame: A summary statistics table.
+    """
+
+    logger = Logger()
+
+    try:
+        summaryList = []
+        for point, df in dfDict.items():
+            pointSummary = get_point_summary(point, df)
+            summaryList.append(pointSummary)
+
+        statSummaryDf = pd.concat(summaryList)
+
+        # Replace pd.NaN with empty string
+        statSummaryDf.fillna(value="", inplace=True)
+
+    except Exception as e:
+        msg = f'Unknown error: {e}'
+        logger.error(msg)
+        raise Exception(msg)
+
+    return statSummaryDf
+
+
 def merge_long_dataframes(dfList: list, freq: int) -> pd.DataFrame:
     """Merge a list of long dataframes to wide format after rounding timestamp for a given time interval
 
     Args:
         dfList (list): A list of pandas DataFrames containing the trend log. (length upto 100)
         freq (int): Value of given time interval.
```

### Comparing `exergenics-etl-0.5.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.0.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     get_file_name_list,
     SkipRowsMachine,
     InputValidation,
     calculate_time_interval,
     DatetimeParser,
     DEFAULT_POSITION_DAY,
     transform_columns_to_long_dataframes,
+    get_point_summary,
+    get_statistical_summary,
     merge_long_dataframes,
     merge_wide_dataframes,
     save_file_to_portal
 )
 
 
 load_dotenv()
@@ -588,16 +590,60 @@
         assert dfDict.keys() == expectedDfDictOutput.keys()
 
         # Compare DataFrames for each key
         for key in dfDict.keys():
             df1 = dfDict[key]
             df2 = expectedDfDictOutput[key]
             assert df1.equals(df2)
-            
-            
+
+
+class TestGetPointSummary:
+
+    @pytest.mark.parametrize("my_get_point_summary_test_case", ['my_summary_statistics_table_test_case1', 'my_summary_statistics_table_test_case2', 'my_summary_statistics_table_test_case3'])
+    def test_get_point_summary(self, my_get_point_summary_test_case, request):
+        myTestPoint, myTestDf, expectedPointSummary = request.getfixturevalue(
+            my_get_point_summary_test_case)
+        assert get_point_summary(
+            myTestPoint, myTestDf).equals(expectedPointSummary)
+
+
+class TestGetStatisticalSummary:
+    def test_get_statistical_summary(self, my_summary_statistics_table_test_case1, my_summary_statistics_table_test_case2, my_summary_statistics_table_test_case3):
+        myTestPoint1, myTestDf1, expectedPointSummary = my_summary_statistics_table_test_case1
+        myTestPoint2, myTestDf2, expectedPointSummary = my_summary_statistics_table_test_case2
+        myTestPoint3, myTestDf3, expectedPointSummary = my_summary_statistics_table_test_case3
+        expectedStatisticalSummaryTable = pd.DataFrame({'count': {'Test data point1': 2.0,
+                                                                  'Test data point2': 3.0,
+                                                                  'Test data point3': 0.0},
+                                                        'mean': {'Test data point1': 1.0,
+                                                                 'Test data point2': '',
+                                                                 'Test data point3': ''},
+                                                        'std': {'Test data point1': 1.414,
+                                                                'Test data point2': '',
+                                                                'Test data point3': ''},
+                                                        'min': {'Test data point1': 0.0,
+                                                                'Test data point2': '',
+                                                                'Test data point3': ''},
+                                                        '25%': {'Test data point1': 0.5,
+                                                                'Test data point2': '',
+                                                                'Test data point3': ''},
+                                                        '50%': {'Test data point1': 1.0,
+                                                                'Test data point2': '',
+                                                                'Test data point3': ''},
+                                                        '75%': {'Test data point1': 1.5,
+                                                                'Test data point2': '',
+                                                                'Test data point3': ''},
+                                                        'max': {'Test data point1': 2.0,
+                                                                'Test data point2': '',
+                                                                'Test data point3': ''}})
+
+        assert get_statistical_summary(
+            {myTestPoint1: myTestDf1, myTestPoint2: myTestDf2, myTestPoint3: myTestDf3}).equals(expectedStatisticalSummaryTable)
+
+
 class TestMergeLongDataframesClass:
 
     @pytest.fixture(scope='class')
     def my_df_list(self):
         df = pd.DataFrame(np.array([['01/01/2023 00:00', 'a', 7], ['01/01/2023 00:08', 'a', 8], ['01/01/2023 00:16', 'a', 9]]),
                           columns=['t', 'd', 'v'])
         df1 = pd.DataFrame(np.array([['01/01/2023 00:00', 'b', 9], ['01/01/2023 00:08', 'b', 8], ['01/01/2023 00:16', 'b', 9]]),
```

### Comparing `exergenics-etl-0.5.0/setup.py` & `exergenics-etl-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v0.5.0",
+    version="v1.0.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

