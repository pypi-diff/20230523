# Comparing `tmp/dicomselect-0.1.0.tar.gz` & `tmp/dicomselect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomselect-0.1.0.tar", last modified: Thu May  4 10:52:25 2023, max compression
+gzip compressed data, was "dicomselect-0.3.0.tar", last modified: Tue May 23 11:51:08 2023, max compression
```

## Comparing `dicomselect-0.1.0.tar` & `dicomselect-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:52:25.482298 dicomselect-0.1.0/
--rw-rw-rw-   0        0        0     1082 2023-04-18 16:33:48.000000 dicomselect-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      798 2023-05-04 10:52:25.482298 dicomselect-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-18 16:33:48.000000 dicomselect-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 10:52:25.463300 dicomselect-0.1.0/dicomselect/
--rw-rw-rw-   0        0        0       92 2023-05-02 16:40:21.000000 dicomselect-0.1.0/dicomselect/__init__.py
--rw-rw-rw-   0        0        0     1358 2023-05-02 11:37:54.000000 dicomselect-0.1.0/dicomselect/constants.py
--rw-rw-rw-   0        0        0     5350 2023-05-03 08:13:30.000000 dicomselect-0.1.0/dicomselect/database.py
--rw-rw-rw-   0        0        0     2239 2023-05-04 10:50:11.000000 dicomselect-0.1.0/dicomselect/dicom.py
--rw-rw-rw-   0        0        0     1470 2023-05-01 13:30:45.000000 dicomselect-0.1.0/dicomselect/info.py
--rw-rw-rw-   0        0        0     8189 2023-05-02 16:40:16.000000 dicomselect-0.1.0/dicomselect/query.py
--rw-rw-rw-   0        0        0     2740 2023-05-02 16:40:11.000000 dicomselect-0.1.0/dicomselect/queryfactory.py
--rw-rw-rw-   0        0        0    15090 2023-05-02 16:40:07.000000 dicomselect-0.1.0/dicomselect/reader.py
--rw-rw-rw-   0        0        0   203115 2023-05-02 16:33:47.000000 dicomselect-0.1.0/dicomselect/tags_generated.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:52:25.480798 dicomselect-0.1.0/dicomselect.egg-info/
--rw-rw-rw-   0        0        0      798 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 08:03:05.000000 dicomselect-0.1.0/dicomselect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      255 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-04 10:52:25.000000 dicomselect-0.1.0/dicomselect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      930 2023-05-04 10:52:25.486799 dicomselect-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-03 13:10:14.000000 dicomselect-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.559170 dicomselect-0.3.0/
+-rw-rw-rw-   0        0        0     1082 2023-04-26 08:15:15.000000 dicomselect-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2814 2023-05-23 11:51:08.559170 dicomselect-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2045 2023-05-23 11:32:18.000000 dicomselect-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.527418 dicomselect-0.3.0/dicomselect/
+-rw-rw-rw-   0        0        0      133 2023-05-23 11:44:09.000000 dicomselect-0.3.0/dicomselect/__init__.py
+-rw-rw-rw-   0        0        0     1358 2023-05-09 08:19:32.000000 dicomselect-0.3.0/dicomselect/constants.py
+-rw-rw-rw-   0        0        0    13063 2023-05-23 11:44:09.000000 dicomselect-0.3.0/dicomselect/convert.py
+-rw-rw-rw-   0        0        0     9048 2023-05-23 11:44:09.000000 dicomselect-0.3.0/dicomselect/database.py
+-rw-rw-rw-   0        0        0     2315 2023-05-09 15:05:34.000000 dicomselect-0.3.0/dicomselect/dicom.py
+-rw-rw-rw-   0        0        0     1580 2023-05-23 11:32:18.000000 dicomselect-0.3.0/dicomselect/info.py
+-rw-rw-rw-   0        0        0     6689 2023-05-09 09:17:00.000000 dicomselect-0.3.0/dicomselect/query.py
+-rw-rw-rw-   0        0        0     2759 2023-05-09 09:17:00.000000 dicomselect-0.3.0/dicomselect/queryfactory.py
+-rw-rw-rw-   0        0        0    15428 2023-05-23 11:32:18.000000 dicomselect-0.3.0/dicomselect/reader.py
+-rw-rw-rw-   0        0        0   203115 2023-05-09 08:19:32.000000 dicomselect-0.3.0/dicomselect/tags_generated.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.543433 dicomselect-0.3.0/dicomselect.egg-info/
+-rw-rw-rw-   0        0        0     2814 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 11:37:02.000000 dicomselect-0.3.0/dicomselect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      263 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2023-05-23 11:51:08.574819 dicomselect-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-23 11:32:18.000000 dicomselect-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.559170 dicomselect-0.3.0/tests/
+-rw-rw-rw-   0        0        0     1604 2023-05-23 11:44:09.000000 dicomselect-0.3.0/tests/test_convert.py
+-rw-rw-rw-   0        0        0      903 2023-05-09 15:12:16.000000 dicomselect-0.3.0/tests/test_create.py
+-rw-rw-rw-   0        0        0     2669 2023-05-09 15:11:33.000000 dicomselect-0.3.0/tests/test_select.py
+-rw-rw-rw-   0        0        0      141 2023-05-09 15:06:15.000000 dicomselect-0.3.0/tests/test_version.py
```

### Comparing `dicomselect-0.1.0/LICENSE` & `dicomselect-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomselect-0.1.0/dicomselect/constants.py` & `dicomselect-0.3.0/dicomselect/constants.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.1.0/dicomselect/database.py` & `dicomselect-0.3.0/dicomselect/database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,136 @@
+import binascii
 import os
+import re
 import shutil
-import binascii
 import sqlite3
 import tempfile
+import warnings
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from os import PathLike
 from pathlib import Path
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 
 import pandas as pd
 from tqdm import tqdm
 
+from dicomselect.convert import Convert, Plan
 from dicomselect.query import Query
 from dicomselect.queryfactory import QueryFactory
 from dicomselect.reader import DICOMImageReader
 
+database_version = '0.3.0'
+
 
 class Database:
     def __init__(self, db_path: PathLike):
         self._db_path = Path(db_path).absolute()
+        if self._db_path.is_dir() or self._db_path.suffix != '.db':
+            raise IsADirectoryError('Provide a file path with as extension, .db')
         self._errors = []
-        self._conn = None
-        self._query_factory = None
+        self._conn: sqlite3.Connection = None
+        self._query_factory: QueryFactory = None
+        self._db_dir: Path = None
+
+    @property
+    def source_dir(self) -> Path:
+        if not self._db_dir:
+            try:
+                with self:
+                    self._db_dir = Path(self._conn.execute('SELECT datadir FROM meta').fetchone()[0])
+            except:
+                raise sqlite3.DataError(f'No source directory found! Did you create a database at {self._db_path}?')
+        return self._db_dir
+
+    @property
+    def version(self) -> str:
+        if self._db_path.exists():
+            cursor = sqlite3.connect(self._db_path, timeout=10)
+            return cursor.execute('SELECT version FROM meta').fetchone()[0]
+        return database_version
 
     def __enter__(self) -> Query:
         return self.open()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def open(self) -> Query:
         with open(self._db_path, "rb") as f:
             file_header = binascii.hexlify(f.read(16)).decode("utf-8")
         # official sqlite3 file header
         if not file_header.startswith("53514c69746520666f726d6174203300"):
             sqlite3.DatabaseError(f'{self._db_path} does not appear to be a valid database')
 
+        db_version = database_version.split('.')
+        this_db_version = self.version.split('.')
+        if db_version[0] != this_db_version[0]:
+            raise RuntimeError(f'this database ({this_db_version}) is outdated by a major revision {db_version}')
+        if db_version[1] > this_db_version[1]:
+            warnings.warn(f'this database ({this_db_version}) is outdated by a minor revision {db_version}')
+
         self._conn = sqlite3.connect(self._db_path)
         self._query_factory = QueryFactory(self._conn)
+
         return self._query_factory.create_query(None)
 
     def close(self):
         self._conn.close()
 
+    def plan(self, filepath: str, *queries: Query) -> Plan:
+        """
+        Prepare a conversion plan, which can convert the results of queries to MHA files.
+
+        Parameters
+        ----------
+        filepath: PathLike
+            Dictates the form of the directory and filename structure, omitting the suffix.
+            Use braces along with column names to replace with that column value.
+            Use forward slash to create a directory structure.
+            (see Query.columns for a full list of available columns).
+            A unique id will be appended at the end.
+
+            Illegal characters will be replaced with '#'.
+            Blank column values will be replaced with '(column_name)=blank'
+        queries: Query
+            The combined results of the query object will be converted to MHA.
+
+        Returns
+        -------
+        A conversion plan.
+        """
+        with self as query:
+            cols = query.columns
+            requested_cols = [r.group(1) for r in re.finditer(r'{(.+?)}', filepath)]
+            QueryFactory.check_if_exists('column', cols, *requested_cols)
+
+            ids = set()
+            for q in queries:
+                ids = ids.union(q._ids)
+            self._conn.execute('CREATE TEMPORARY TABLE convert_ids (id INTEGER)')
+            self._conn.executemany('INSERT INTO convert_ids (id) VALUES (?)', [(i,) for i in ids])
+            converts_fetched = self._conn.execute(
+                f'SELECT dicomselect_uid, path, {", ".join(requested_cols)} FROM data JOIN convert_ids ON data.id = convert_ids.id').fetchall()
+            converts = [Convert(fetched[0], fetched[1], filepath, requested_cols, fetched[2:]) for fetched in converts_fetched]
+
+        return Plan(self.source_dir, converts)
+
     def create(self, data_dir: PathLike, max_workers: int = 4, *additional_dicom_tags: str):
-        """Build a database from DICOMs in subdirectories of data_dir.
+        """
+        Build a database from DICOMs in subdirectories of data_dir.
 
         Parameters
         ----------
-        data_dir
+        data_dir: PathLike
+            Directory containing .dcm data or dicom.zip data.
         max_workers
+            Max number of workers for parallel execution of database creation.
         additional_dicom_tags
+            See https://www.dicomlibrary.com/dicom/dicom-tags/, input any additional tags that are not included by default
+            Each tag should be formatted as shown in the DICOM tag library, eg. '(0002,0000)'.
         """
         self._errors = []
 
         data_dir = Path(data_dir).absolute()
         with tempfile.TemporaryDirectory(ignore_cleanup_errors=True) as temp_dir:
             temp_db = Path(temp_dir) / 'temp.db'
             subdirectories = [data_dir / path for path in os.listdir(data_dir)]
@@ -72,37 +148,39 @@
             if example_metadata is None:
                 raise sqlite3.DataError(f'No dicom data found in {data_dir}')
 
             cursor = sqlite3.connect(temp_db)
             cursor.execute(f'CREATE TABLE data (id INTEGER PRIMARY KEY AUTOINCREMENT, series_length INTEGER, path TEXT, {columns});')
             cursor.close()
 
-            print(f"Creating database from DICOMs subdirectories of {data_dir}. Collecting all subdirectories...")
+            print(f"Creating database from DICOMs subdirectories of {data_dir}.")
+            print("Collecting all subdirectories...")
 
             subdirectories = [data_dir / path for path in os.listdir(data_dir)]
             with tqdm(total=len(subdirectories)) as pbar, ThreadPoolExecutor(max_workers=max_workers) as pool:
                 futures = [pool.submit(self._thread_execute_dir, temp_db, path.absolute(), additional_dicom_tags) for path in subdirectories]
                 for future in as_completed(futures):
                     self._errors.append(future.exception())
                     pbar.update()
 
             cursor = sqlite3.connect(temp_db, timeout=10)
-            df_meta = pd.DataFrame({'DataDirectory': str(data_dir)}, index=[0])
+            df_meta = pd.DataFrame({'datadir': str(data_dir), 'version': database_version}, index=[0])
             df_meta.to_sql(name='meta', con=cursor, if_exists='replace')
             cursor.close()
 
             if self._db_path.exists():
                 os.remove(self._db_path)
             shutil.copy(temp_db, self._db_path)
 
             self._errors = [err for err in self._errors if err]
             print(f"Database created at {self._db_path} with {len(self._errors)} errors.")
-            for e in self._errors:
-                if e:
-                    print('\t' + str(e))
+            print(self._format_errors())
+
+    def _format_errors(self):
+        return "\t" + "\n\t".join([str(e) for e in self._errors if e])
 
     def _dicoms_in_dir(self, subdir: Path) -> Tuple[Path, Path]:
         for root, _, filenames in os.walk(subdir, onerror=lambda err: self._errors.append(err)):
             if any([file.endswith('.dcm') for file in filenames]) or 'dicom.zip' in filenames:
                 rel_path = Path(root).relative_to(subdir.parent)
                 yield root, rel_path
```

### Comparing `dicomselect-0.1.0/dicomselect/dicom.py` & `dicomselect-0.3.0/dicomselect/dicom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import re
 from typing import Callable
 
 from dicomselect.tags_generated import tags_generated, version
 from dicomselect.constants import DEFAULT_DICOM_TAGS
 
 
+class InvalidTagError(ValueError):
+    pass
+
+
 def convert_AS(value: str):
     t = value[3]
     value = int(value[:3])
     if t == 'D':
         value /= 365
     elif t == 'M':
         value /= 12
@@ -40,20 +44,20 @@
 }
 
 
 class DICOMTag:
     def __init__(self, tag: str):
         r = re.search(r'(.{4})[,| ]+(.{4})', tag.upper())
         if not r:
-            raise ValueError(f'Invalid tag, could not parse {tag}')
+            raise InvalidTagError(f'Invalid tag, could not parse {tag}')
         self._tag = r.groups()
 
-        from_generated_tags = tags_generated.get(self.key, None)
+        from_generated_tags = tags_generated.get(self.key.upper(), None)
         if from_generated_tags is None:
-            raise ValueError(f'Invalid tag, does not exist in {version}')
+            raise InvalidTagError(f'Invalid tag, does not exist in {version}')
 
         self._name = from_generated_tags[0]
         vr = VR.get(from_generated_tags[1], "TEXT")
         if isinstance(vr, str):
             vr = (vr, lambda v: v)
 
         self._datatype = vr[0]
@@ -66,15 +70,15 @@
 
     @property
     def name(self) -> str:
         return re.sub(r'\W+', '', self._name.replace(' ', '_')).lower()
 
     @property
     def key(self) -> str:
-        return f'{self._tag[0]}|{self._tag[1]}'
+        return f'{self._tag[0]}|{self._tag[1]}'.lower()
 
     @property
     def column_type(self) -> str:
         return self._datatype
 
     def convert(self, value: str):
         return self._convert_func(value)
```

### Comparing `dicomselect-0.1.0/dicomselect/info.py` & `dicomselect-0.3.0/dicomselect/info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from typing import List, Dict
+from typing import TYPE_CHECKING, Dict, List
+
+if TYPE_CHECKING:
+    from dicomselect.query import Query
 
 
 class Info:
-    def __init__(self, rows: List[tuple], cols: Dict[str, Dict[str, int]]):
-        # self._query_parent = parent
+    def __init__(self, parent: 'Query', rows: List[tuple], cols: Dict[str, Dict[str, int]]):
+        self._query_parent = parent
         self._rows = rows
         self._cols = cols
 
     @property
     def count(self) -> int:
         return len(self._rows)
 
-    # def query(self) -> 'Query':
-    #     return self._query_parent
+    def query(self) -> 'Query':
+        return self._query_parent
 
     def print(self, sort_by_homogeneous: bool = True) -> 'Info':
         """
         Print the current results of a query
 
         Parameters
         ----------
@@ -34,12 +37,13 @@
         print('=' * len(header))
         for key in sort_by_similarity:
             print(key)
             items = sorted(self._cols[key].items(), key=lambda a: a[1], reverse=True)
             for value, count in items:
                 count: str = f'({count})'.ljust(len(str(len(self._rows))) + 2)
                 print(f'\t{count} {value}')
+
         return self
 
     def filter(self, *columns: str) -> 'Info':
         filtered_cols = {key: value for key, value in self._cols.items() if key in columns}
-        return Info(self._rows, filtered_cols)
+        return Info(self._query_parent, self._rows, filtered_cols)
```

### Comparing `dicomselect-0.1.0/dicomselect/queryfactory.py` & `dicomselect-0.3.0/dicomselect/queryfactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import sqlite3
-from typing import Tuple, Optional, Iterable
+from typing import Tuple, Optional, Iterable, Dict, List
 
 import rapidfuzz
 
 
 class QueryFactory:
     def __init__(self, connection: sqlite3.Connection):
         self._conn = connection
         self._cursor = connection.cursor()
         column_info = self.execute('PRAGMA TABLE_INFO(data)').fetchall()
         self.columns: Tuple[str] = tuple([c[1] for c in column_info if c[1] != 'id'])
-        self.temp_tables = dict()
+        self.temp_tables: Dict[str, Tuple[List[int], int]] = dict()
+        self._update_temp_tables('data')
         self._count = -1
 
-    @property
-    def count(self) -> int:
-        if self._count == -1:
-            self._count = self.execute('SELECT COUNT(id) FROM data').fetchone()[0]
-        return self._count
-
     def execute(self, sql: str) -> sqlite3.Cursor:
         return self._cursor.execute(sql)
 
     def create_query(self, parent: Optional[str]):
         from dicomselect.query import Query
         return Query(self, parent)
 
     def _update_temp_tables(self, new_temp_table: str):
-        self.temp_tables[new_temp_table] = self.execute(f'SELECT COUNT(id) FROM {new_temp_table};').fetchone()[0]
-        self.temp_tables = dict(sorted(self.temp_tables.items(), key=lambda x: x[1]))
+        ids = self.select_ids(new_temp_table)
+        self.temp_tables[new_temp_table] = (ids, len(ids))
+        self.temp_tables = dict(sorted(self.temp_tables.items(), key=lambda x: x[1][1]))
 
     def create_query_from_sql(self, sql: str, parent_temp_table: str):
         new_temp_table = __package__ + str(len(self.temp_tables))
         if parent_temp_table:
             self.execute(
                 f'CREATE TEMP TABLE {new_temp_table} AS SELECT id FROM {parent_temp_table} WHERE id IN (SELECT id FROM data {sql});')
         else:
@@ -47,14 +43,17 @@
 
         new_temp_table = __package__ + str(len(self.temp_tables))
         self.execute(f'CREATE TEMP TABLE {new_temp_table} AS SELECT id FROM {temp_tables[0]} {operation} SELECT id FROM {temp_tables[1]};')
 
         self._update_temp_tables(new_temp_table)
         return self.create_query(new_temp_table)
 
+    def select_ids(self, table: str):
+        return [i[0] for i in self.execute(f'SELECT id FROM {table};').fetchall()]
+
     @staticmethod
     def check_if_exists(item_type: str, possible_items: Iterable, *items):
         for item in items:
             if item is not None and item not in possible_items:
                 suggest = rapidfuzz.process.extractOne(item, possible_items, score_cutoff=25)
                 suggest = f', did you mean {suggest[0]}?' if suggest else ''
                 raise ValueError(f'{item_type} "{item}" does not exist{suggest}')
```

### Comparing `dicomselect-0.1.0/dicomselect/reader.py` & `dicomselect-0.3.0/dicomselect/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import tempfile
+import hashlib
 import zipfile
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import SimpleITK as sitk
 import numpy as np
 import pydicom
 import pydicom.errors
 
-from dicomselect.dicom import DICOMTag, DEFAULT_DICOM_TAGS
+from dicomselect.dicom import DICOMTag, DEFAULT_DICOM_TAGS, InvalidTagError
 
 PathLike = os.PathLike
 
 
 class UnreadableDICOMError(BaseException):
     """Exception raised when a DICOM series could not be loaded"""
 
@@ -88,14 +89,16 @@
             self._image = self._read_image()
         return self._image
 
     @property
     def metadata(self) -> Dict[str, str]:
         if self._metadata is None:
             self._metadata = self._read_metadata()
+            uid_str = '_'.join([str(self.metadata[tag.name]) for tag in DEFAULT_DICOM_TAGS])
+            self._metadata['dicomselect_uid'] = hashlib.blake2b(uid_str.encode()).hexdigest()
         return self._metadata
 
     def column_info(self):
         columns = {tag.name: tag.column_type for tag in self._dcm_tags}
         for key in self.metadata.keys():
             if key not in columns:
                 columns[key] = "TEXT"
@@ -290,30 +293,34 @@
             except pydicom.errors.InvalidDicomError:
                 raise UnreadableDICOMError(path)
 
     def _collect_metadata_sitk(self, ref: Union[sitk.Image, sitk.ImageFileReader]) -> Dict[str, str]:
         metadata = {}
         for tag in self._dcm_tags:
             # collect metadata with DICOM names, e.g. patientsage, as keys)
-            metadata[tag.name] = tag.convert(ref.GetMetaData(tag.key).strip() if ref.HasMetaDataKey(tag.key) else '')
+            metadata[tag.name] = tag.convert(ref.GetMetaData(tag.key.lower()).strip() if ref.HasMetaDataKey(tag.key) else '')
         if self._allow_raw_tags:
             for key in ref.GetMetaDataKeys():
                 # collect all available metadata (with DICOM tags, e.g. 0010|1010, as keys)
-                tag = DICOMTag(key)
-                if tag not in self._dcm_tags:
-                    metadata[tag.name] = tag.convert(ref.GetMetaData(tag.key).strip())
+                try:
+                    tag = DICOMTag(key)
+                    if tag not in self._dcm_tags:
+                        metadata[tag.name] = tag.convert(ref.GetMetaData(tag.key).strip())
+                except InvalidTagError:
+                    continue
 
         metadata["spacing_in_plane"] = str(ref.GetSpacing()[0:2])
         metadata["image_direction"] = str(ref.GetDirection())
+
         return metadata
 
     def _collect_metadata_pydicom(self, ds: "pydicom.dataset.Dataset") -> Dict[str, str]:
         metadata = {}
         for tag in self._dcm_tags:
-            # collect metadata with DICOM names, e.g. patientsage, as keys)
+            # collect metadata with DICOM names, e.g. patients_age, as keys)
             value = self.get_pydicom_value(ds, tag.key)
             metadata[tag.name] = tag.convert(value if value is not None else '')
         if self._allow_raw_tags:
             for key in ds.keys():
                 # collect all available metadata (with DICOM tags, e.g. 0010|1010, as keys)
                 tag = DICOMTag('|'.join([str(x).zfill(4) for x in [key.group, key.elem]]))
                 if tag not in self._dcm_tags:
```

### Comparing `dicomselect-0.1.0/dicomselect/tags_generated.py` & `dicomselect-0.3.0/dicomselect/tags_generated.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.1.0/dicomselect.egg-info/SOURCES.txt` & `dicomselect-0.3.0/dicomselect.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 ./dicomselect/__init__.py
 ./dicomselect/constants.py
+./dicomselect/convert.py
 ./dicomselect/database.py
 ./dicomselect/dicom.py
 ./dicomselect/info.py
 ./dicomselect/query.py
 ./dicomselect/queryfactory.py
 ./dicomselect/reader.py
 ./dicomselect/tags_generated.py
 dicomselect/__init__.py
 dicomselect/constants.py
+dicomselect/convert.py
 dicomselect/database.py
 dicomselect/dicom.py
 dicomselect/info.py
 dicomselect/query.py
 dicomselect/queryfactory.py
 dicomselect/reader.py
 dicomselect/tags_generated.py
 dicomselect.egg-info/PKG-INFO
 dicomselect.egg-info/SOURCES.txt
 dicomselect.egg-info/dependency_links.txt
 dicomselect.egg-info/not-zip-safe
 dicomselect.egg-info/requires.txt
-dicomselect.egg-info/top_level.txt
+dicomselect.egg-info/top_level.txt
+tests/test_convert.py
+tests/test_create.py
+tests/test_select.py
+tests/test_version.py
```

### Comparing `dicomselect-0.1.0/setup.cfg` & `dicomselect-0.3.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -33,27 +33,27 @@
 00000200: 0d0a 0970 796c 6962 6a70 6567 7e3d 312e  ...pylibjpeg~=1.
 00000210: 342e 300d 0a09 7079 6c69 626a 7065 672d  4.0...pylibjpeg-
 00000220: 6c69 626a 7065 677e 3d31 2e33 2e34 0d0a  libjpeg~=1.3.4..
 00000230: 0970 6963 6169 5f70 7265 707e 3d32 2e31  .picai_prep~=2.1
 00000240: 2e36 0d0a 0972 6170 6964 6675 7a7a 7e3d  .6...rapidfuzz~=
 00000250: 332e 302e 300d 0a09 7079 7468 6f6e 2d4c  3.0.0...python-L
 00000260: 6576 656e 7368 7465 696e 7e3d 302e 3231  evenshtein~=0.21
-00000270: 2e30 0d0a 7079 7468 6f6e 5f72 6571 7569  .0..python_requi
-00000280: 7265 7320 3d20 3e3d 332e 370d 0a70 6163  res = >=3.7..pac
-00000290: 6b61 6765 5f64 6972 203d 200d 0a09 3d2e  kage_dir = ...=.
-000002a0: 0d0a 7a69 705f 7361 6665 203d 206e 6f0d  ..zip_safe = no.
-000002b0: 0a0d 0a5b 6f70 7469 6f6e 732e 6578 7472  ...[options.extr
-000002c0: 6173 5f72 6571 7569 7265 5d0d 0a74 6573  as_require]..tes
-000002d0: 7469 6e67 203d 200d 0a09 7079 7465 7374  ting = ...pytest
-000002e0: 3e3d 362e 300d 0a09 7079 7465 7374 2d63  >=6.0...pytest-c
-000002f0: 6f76 3e3d 322e 300d 0a09 6d79 7079 3e3d  ov>=2.0...mypy>=
-00000300: 302e 3931 300d 0a09 666c 616b 6538 3e3d  0.910...flake8>=
-00000310: 332e 390d 0a09 746f 783e 3d33 2e32 340d  3.9...tox>=3.24.
-00000320: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000330: 6167 655f 6461 7461 5d0d 0a64 6963 6f6d  age_data]..dicom
-00000340: 7365 6c65 6374 203d 2070 792e 7479 7065  select = py.type
-00000350: 640d 0a0d 0a5b 666c 616b 6538 5d0d 0a6d  d....[flake8]..m
-00000360: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-00000370: 2031 3630 0d0a 0d0a 5b65 6767 5f69 6e66   160....[egg_inf
-00000380: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000390: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000003a0: 0d0a                                     ..
+00000270: 2e30 0d0a 0974 7265 656c 6962 0d0a 7079  .0...treelib..py
+00000280: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000290: 3e3d 332e 370d 0a70 6163 6b61 6765 5f64  >=3.7..package_d
+000002a0: 6972 203d 200d 0a09 3d2e 0d0a 7a69 705f  ir = ...=...zip_
+000002b0: 7361 6665 203d 206e 6f0d 0a0d 0a5b 6f70  safe = no....[op
+000002c0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000002d0: 7569 7265 5d0d 0a74 6573 7469 6e67 203d  uire]..testing =
+000002e0: 200d 0a09 7079 7465 7374 3e3d 362e 300d   ...pytest>=6.0.
+000002f0: 0a09 7079 7465 7374 2d63 6f76 3e3d 322e  ..pytest-cov>=2.
+00000300: 300d 0a09 6d79 7079 3e3d 302e 3931 300d  0...mypy>=0.910.
+00000310: 0a09 666c 616b 6538 3e3d 332e 390d 0a09  ..flake8>=3.9...
+00000320: 746f 783e 3d33 2e32 340d 0a0d 0a5b 6f70  tox>=3.24....[op
+00000330: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000340: 7461 5d0d 0a64 6963 6f6d 7365 6c65 6374  ta]..dicomselect
+00000350: 203d 2070 792e 7479 7065 640d 0a0d 0a5b   = py.typed....[
+00000360: 666c 616b 6538 5d0d 0a6d 6178 2d6c 696e  flake8]..max-lin
+00000370: 652d 6c65 6e67 7468 203d 2031 3630 0d0a  e-length = 160..
+00000380: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000390: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000003a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `dicomselect-0.1.0/setup.py` & `dicomselect-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import setuptools
 
+version = '0.3.0'
+
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name='dicomselect',
-        version='0.1.0',
+        version=version,
         author_email='Stan.Noordman@radboudumc.nl',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/DIAGNijmegen/dicomselect',
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/dicomselect"
         },
```

