# Comparing `tmp/finlogic-0.4.7.tar.gz` & `tmp/finlogic-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.7.tar", last modified: Mon May 22 11:46:10 2023, max compression
+gzip compressed data, was "finlogic-0.4.8.tar", last modified: Mon May 22 22:51:30 2023, max compression
```

## Comparing `finlogic-0.4.7.tar` & `finlogic-0.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.7/LICENSE
--rw-r--r--   0        0        0     9216 2023-05-22 11:45:26.558019 finlogic-0.4.7/README.md
--rw-r--r--   0        0        0      423 2023-05-22 11:32:57.010081 finlogic-0.4.7/finlogic/__init__.py
--rw-r--r--   0        0        0    23964 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.7/finlogic/config.py
--rw-r--r--   0        0        0    11456 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/cvm.py
--rw-r--r--   0        0        0     4637 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/database.py
--rw-r--r--   0        0        0     2987 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/fduckdb.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.7/finlogic/fprint.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.7/finlogic/language.py
--rw-r--r--   0        0        0     1039 2023-05-22 11:46:10.598431 finlogic-0.4.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.7/tests/test_company.py
--rw-r--r--   0        0        0      900 2023-05-22 11:25:57.287389 finlogic-0.4.7/tests/test_database.py
--rw-r--r--   0        0        0    11325 1970-01-01 00:00:00.000000 finlogic-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.8/LICENSE
+-rw-r--r--   0        0        0     9216 2023-05-22 22:49:10.801399 finlogic-0.4.8/README.md
+-rw-r--r--   0        0        0      423 2023-05-22 22:42:54.448718 finlogic-0.4.8/finlogic/__init__.py
+-rw-r--r--   0        0        0    23696 2023-05-22 22:42:54.448718 finlogic-0.4.8/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.8/finlogic/config.py
+-rw-r--r--   0        0        0    11931 2023-05-22 22:43:42.677190 finlogic-0.4.8/finlogic/cvm.py
+-rw-r--r--   0        0        0     4637 2023-05-22 11:25:57.286389 finlogic-0.4.8/finlogic/database.py
+-rw-r--r--   0        0        0     3044 2023-05-22 22:42:54.448718 finlogic-0.4.8/finlogic/fduckdb.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.8/finlogic/fprint.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.8/finlogic/language.py
+-rw-r--r--   0        0        0     1039 2023-05-22 22:51:30.874768 finlogic-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.8/tests/__init__.py
+-rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.8/tests/test_company.py
+-rw-r--r--   0        0        0      900 2023-05-22 22:42:54.448718 finlogic-0.4.8/tests/test_database.py
+-rw-r--r--   0        0        0    11325 1970-01-01 00:00:00.000000 finlogic-0.4.8/PKG-INFO
```

### Comparing `finlogic-0.4.7/LICENSE` & `finlogic-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.7/README.md` & `finlogic-0.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 # Show database info:
 >>> fl.database_info()
 ```
 
 | FinLogic Database Info |                         Value |
 | :--------------------- | ----------------------------: |
 | db_path                | .../finlogic/data/finlogic.db |
-| db_size                |                      301.0 MB |
+| db_size                |                       76.0 MB |
 | db_last_modified       |           2023-04-20 07:29:08 |
 | number_of_companies    |                         1,139 |
-| number_of_rows         |                     4,379,496 |
-| number_of_reports      |                        13,770 |
+| number_of_rows         |                     2,806,635 |
+| number_of_reports      |                         9,422 |
 | first_report           |                    2009-01-31 |
 | last_report            |                    2023-03-31 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
```

### Comparing `finlogic-0.4.7/finlogic/company.py` & `finlogic-0.4.8/finlogic/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,22 +285,14 @@
         annual_df = df.query('report_type == "ANNUAL"')
         self._first_annual = annual_df["period_end"].min()
         self._last_annual = annual_df["period_end"].max()
         quarterly_df = df.query('report_type == "QUARTERLY"')
         self._last_quarterly = quarterly_df["period_end"].max()
         self._last_period = df["period_end"].max()
 
-        # Keep last quarterly report only if it is after the last annual report
-        # for calculating TTM values
-        df.query(
-            'report_type == "ANNUAL" or \
-             period_reference == @self._last_period',
-            inplace=True,
-        )
-
         # Drop columns that are already company attributes or will not be used
         df.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
 
         # Set company data frame
         self._df = df
 
     def info(self) -> dict:
```

### Comparing `finlogic-0.4.7/finlogic/cvm.py` & `finlogic-0.4.8/finlogic/cvm.py`

 * *Files 6% similar despite different names*

```diff
@@ -219,16 +219,16 @@
         'DF Individual - Demonstração de Valor Adicionado',
         'DF Individual - Demonstração do Fluxo de Caixa (Método Indireto)',
         'DF Individual - Demonstração do Resultado',
     Hence, with string position 3:6 we can make:
     if == 'Con' -> consolidated statement
     if == 'Ind' -> separate statement
     """
-    map_dic = {"DF C": "CONSOLIDATED", "DF I": "SEPARATE"}
-    df.insert(9, "acc_method", df["report_group"].str[:4].map(map_dic))
+    map_dic = {"Con": "CONSOLIDATED", "Ind": "SEPARATE"}
+    df.insert(4, "acc_method", df["report_group"].str[3:6].map(map_dic))
     # 'report_group' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
 
     # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
     # Few of them have different values in "acc_value". Only one them will be kept.
     # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
@@ -258,24 +258,25 @@
 
 def read_all_processed_files() -> pd.DataFrame:
     """Read all processed CVM files."""
     # list filepaths in processed folder
     filepaths = sorted(cfg.CVM_PROCESSED_DIR.glob("*.pickle"))
     df = pd.concat([pd.read_pickle(f, compression="zstd") for f in filepaths])
     columns = df.columns
-    cat_cols = [c for c in columns if df[c].dtype in ["object", "datetime64[ns]"]]
+    cat_cols = [c for c in columns if df[c].dtype in ["object"]]
     df[cat_cols] = df[cat_cols].astype("category")
     return df
 
 
-def drop_duplicates(df: pd.DataFrame) -> pd.DataFrame:
-    """Drop duplicates from a before building database
-    Because PREVIOUS value == LAST value for the year before, we can keep only
-    the most recent values by dropping duplicates. By doing this, we guarantee
-    that there is only one valid accounting value in database -> the last one
+def drop_not_last_entries(df: pd.DataFrame) -> pd.DataFrame:
+    """Drop duplicated accounting entries before building database
+
+    Because the report holds accounting entries for the year before, we can keep only
+    the most recent one in the database. By doing this, we guarantee
+    that there is only one valid accounting value in the database -> the last one
     """
     sort_cols = [
         "cvm_id",
         "acc_method",
         "acc_code",
         "period_reference",
         "report_type",
@@ -290,7 +291,20 @@
         "acc_code",
         "period_begin",
         "period_end",
     ]
     df.drop_duplicates(subset=subset_cols, keep="last", inplace=True, ignore_index=True)
 
     return df
+
+
+def drop_unecessary_quarterly_entries(df: pd.DataFrame) -> pd.DataFrame:
+    """Keep the last QUARTERLY report for each company only when necessary."""
+    df["max_period"] = df.groupby("cvm_id")["period_reference"].transform("max")
+
+    condition1 = df["report_type"] == "QUARTERLY"
+    condition2 = df["period_reference"] < df["max_period"]
+    df = df[~(condition1 & condition2)].reset_index(drop=True)
+
+    df.drop(columns=["max_period"], inplace=True)
+
+    return df
```

### Comparing `finlogic-0.4.7/finlogic/database.py` & `finlogic-0.4.8/finlogic/database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.7/finlogic/fduckdb.py` & `finlogic-0.4.8/finlogic/fduckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
 def build():
     """Build FinLogic Database from processed CVM files."""
     print("Building FinLogic Database...")
     # Reset database
     reset()
     df = cvm.read_all_processed_files()
-    df = cvm.drop_duplicates(df)
+    df = cvm.drop_not_last_entries(df)
+    df = cvm.drop_unecessary_quarterly_entries(df)
     # Create a table with all processed CVM files
     execute("CREATE TABLE reports AS SELECT * FROM df")
 
 
 def is_empty() -> bool:
     """Return True if database is considered empty."""
     return FINLOGIC_DB_PATH.stat().st_size / 1024**2 < 10
```

### Comparing `finlogic-0.4.7/finlogic/fprint.py` & `finlogic-0.4.8/finlogic/fprint.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.7/finlogic/language.py` & `finlogic-0.4.8/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.7/pyproject.toml` & `finlogic-0.4.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 dependencies = [
     "pandas>=1.5.0",
     "requests>=2.30.0",
     "duckdb>=0.8.0",
     "rich>=13.0.0",
     "zstandard>=0.21.0",
 ]
-version = "0.4.7"
+version = "0.4.8"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.4.7/tests/test_company.py` & `finlogic-0.4.8/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.7/tests/test_database.py` & `finlogic-0.4.8/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TestDatabase(unittest.TestCase):
     def test_info(self):
         """Test the info method of the Database module."""
         db_info = fdb.get_info()
         self.assertEqual(db_info["first_report"], "2009-01-31")
-        self.assertTrue(db_info["number_of_rows"] > 4_000_000)
+        self.assertTrue(db_info["number_of_rows"] > 2_000_000)
 
     def test_search_company(self):
         """Test the search_company method of the Database module."""
         search_result = fl.search_company("petrobras")
         """
             name_id                            cvm_id  tax_id
         0   PETROBRAS DISTRIBUIDORA S/A         24295  34.274.233/0001-02
```

### Comparing `finlogic-0.4.7/PKG-INFO` & `finlogic-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.7
+Version: 0.4.8
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -99,19 +99,19 @@
 # Show database info:
 >>> fl.database_info()
 ```
 
 | FinLogic Database Info |                         Value |
 | :--------------------- | ----------------------------: |
 | db_path                | .../finlogic/data/finlogic.db |
-| db_size                |                      301.0 MB |
+| db_size                |                       76.0 MB |
 | db_last_modified       |           2023-04-20 07:29:08 |
 | number_of_companies    |                         1,139 |
-| number_of_rows         |                     4,379,496 |
-| number_of_reports      |                        13,770 |
+| number_of_rows         |                     2,806,635 |
+| number_of_reports      |                         9,422 |
 | first_report           |                    2009-01-31 |
 | last_report            |                    2023-03-31 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
```

