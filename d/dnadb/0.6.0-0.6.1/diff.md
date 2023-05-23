# Comparing `tmp/dnadb-0.6.0.tar.gz` & `tmp/dnadb-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.6.0.tar", last modified: Sun May 21 18:38:17 2023, max compression
+gzip compressed data, was "dnadb-0.6.1.tar", last modified: Tue May 23 04:50:58 2023, max compression
```

## Comparing `dnadb-0.6.0.tar` & `dnadb-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.0/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-21 18:38:17.236162 dnadb-0.6.0/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.0/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-21 18:37:54.000000 dnadb-0.6.0/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-21 18:38:17.236162 dnadb-0.6.0/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-21 18:37:47.000000 dnadb-0.6.0/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.0/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.0/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.0/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.0/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.0/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.0/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.6.0/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7774 2023-05-21 15:17:15.000000 dnadb-0.6.0/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5991 2023-05-21 14:19:54.000000 dnadb-0.6.0/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    10992 2023-05-21 18:28:55.000000 dnadb-0.6.0/src/dnadb/sample.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.0/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.0/src/dnadb/types.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.0/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      541 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.1/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 04:50:58.193070 dnadb-0.6.1/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.1/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-23 04:50:32.000000 dnadb-0.6.1/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-23 04:50:58.193070 dnadb-0.6.1/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-23 04:50:25.000000 dnadb-0.6.1/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.1/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.1/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.1/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.1/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.1/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.1/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.6.1/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7774 2023-05-21 15:17:15.000000 dnadb-0.6.1/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5991 2023-05-21 14:19:54.000000 dnadb-0.6.1/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    11003 2023-05-23 04:49:42.000000 dnadb-0.6.1/src/dnadb/sample.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.1/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.1/src/dnadb/types.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.1/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      541 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.6.0/LICENSE` & `dnadb-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/PKG-INFO` & `dnadb-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.0/pyproject.toml` & `dnadb-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.6.0/src/dnadb/datasets/dataset.py` & `dnadb-0.6.1/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/datasets/greengenes.py` & `dnadb-0.6.1/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.6.1/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.6.1/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/db.py` & `dnadb-0.6.1/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/dna.py` & `dnadb-0.6.1/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/fasta.py` & `dnadb-0.6.1/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/fastq.py` & `dnadb-0.6.1/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/sample.py` & `dnadb-0.6.1/src/dnadb/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,36 +255,34 @@
             for _ in range(abundance):
                 yield entry
 
 # Utility functions for loading/wrapping FASTA/FASTQ databases with sample interfaces.
 
 def load_fasta(
     fasta_db_or_path: Union[FastaDb, Union[str, Path]],
-    name: Optional[str]
+    name: Optional[str] = None
 ) -> FastaSample:
     if not isinstance(fasta_db_or_path, FastaDb):
         fasta_db_or_path = FastaDb(fasta_db_or_path)
     return FastaSample(fasta_db_or_path, name)
 
 
 def load_fastq(
     fastq_db_or_path: Union[FastqDb, Union[str, Path]],
-    name: Optional[str]
+    name: Optional[str] = None
 ) -> FastqSample:
     if not isinstance(fastq_db_or_path, FastqDb):
         fastq_db_or_path = FastqDb(fastq_db_or_path)
     return FastqSample(fastq_db_or_path, name)
 
 
 def load_multiplexed_fasta(
     fasta_db_or_path: Union[FastaDb, Union[str, Path]],
     sample_mapping_db_or_path: Union[SampleMappingDb, Union[str, Path]],
-    fasta_index_db_or_path: Optional[Union[FastaIndexDb, Union[str, Path]]] = None,
-
-
+    fasta_index_db_or_path: Optional[Union[FastaIndexDb, Union[str, Path]]] = None
 ) -> Tuple[DemultiplexedFastaSample, ...]:
     if not isinstance(fasta_db_or_path, FastaDb):
         fasta_db_or_path = FastaDb(fasta_db_or_path)
     if not isinstance(sample_mapping_db_or_path, SampleMappingDb):
         if fasta_index_db_or_path is None:
             assert str(sample_mapping_db_or_path).endswith(".mapping.db"), \
                 "Unable to automatically resolve the index path."
```

### Comparing `dnadb-0.6.0/src/dnadb/taxonomy.py` & `dnadb-0.6.1/src/dnadb/taxonomy.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb/utils.py` & `dnadb-0.6.1/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.0/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.6.1/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.0/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.6.1/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

