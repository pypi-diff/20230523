# Comparing `tmp/bioino-0.0.1.tar.gz` & `tmp/bioino-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioino-0.0.1.tar", last modified: Wed May 17 09:20:57 2023, max compression
+gzip compressed data, was "bioino-0.0.1.post1.tar", last modified: Tue May 23 10:04:31 2023, max compression
```

## Comparing `bioino-0.0.1.tar` & `bioino-0.0.1.post1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:20:57.103189 bioino-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 09:20:46.000000 bioino-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-17 09:20:57.103189 bioino-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-17 09:20:46.000000 bioino-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:20:57.099189 bioino-0.0.1/bioino/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/gff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/gff2table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/table2fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 09:20:46.000000 bioino-0.0.1/bioino/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:20:57.099189 bioino-0.0.1/bioino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-17 09:20:57.000000 bioino-0.0.1/bioino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-17 09:20:57.000000 bioino-0.0.1/bioino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:20:57.000000 bioino-0.0.1/bioino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 09:20:57.000000 bioino-0.0.1/bioino.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 09:20:57.000000 bioino-0.0.1/bioino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 09:20:57.000000 bioino-0.0.1/bioino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-17 09:20:46.000000 bioino-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:20:57.103189 bioino-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:20:57.099189 bioino-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 09:20:46.000000 bioino-0.0.1/test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:04:31.165371 bioino-0.0.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-23 10:04:31.165371 bioino-0.0.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:04:31.165371 bioino-0.0.1.post1/bioino/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/gff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/gff2table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/table2fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/bioino/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:04:31.165371 bioino-0.0.1.post1/bioino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-23 10:04:31.000000 bioino-0.0.1.post1/bioino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 10:04:31.000000 bioino-0.0.1.post1/bioino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:04:31.000000 bioino-0.0.1.post1/bioino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 10:04:31.000000 bioino-0.0.1.post1/bioino.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 10:04:31.000000 bioino-0.0.1.post1/bioino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 10:04:31.000000 bioino-0.0.1.post1/bioino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:04:31.165371 bioino-0.0.1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:04:31.165371 bioino-0.0.1.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 10:04:14.000000 bioino-0.0.1.post1/test/tests.py
```

### Comparing `bioino-0.0.1/LICENSE` & `bioino-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioino-0.0.1/PKG-INFO` & `bioino-0.0.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioino
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Lightweight IO and conversion for bioinformatics file formats.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
-Project-URL: Homepage, https://github.com/scbirlab/bioin
-Project-URL: Bug Tracker, https://github.com/scbirlab/bioin/issues
+Project-URL: Homepage, https://github.com/scbirlab/bioino
+Project-URL: Bug Tracker, https://github.com/scbirlab/bioino/issues
 Keywords: biology,bioinformatics,science,io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bioino-0.0.1/README.md` & `bioino-0.0.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `bioino-0.0.1/bioino/fasta.py` & `bioino-0.0.1.post1/bioino/fasta.py`

 * *Files identical despite different names*

### Comparing `bioino-0.0.1/bioino/gff.py` & `bioino-0.0.1.post1/bioino/gff.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             
             metadata.append(GffMetadatum(name=this_metadata[0], 
                                          flag=flag, 
                                          values=tuple(this_metadata[1:])))
 
         elif len(line) > 0:  # tab-delimited table
 
-            data = line.split()
+            data = line.split('\t')  # Must be TAB otherwise columns 1-8 get messed up
             
             try:
                 
                 columns = GffColumns(*data[:8])
             
             except TypeError as e:
```

### Comparing `bioino-0.0.1/bioino/gff2table.py` & `bioino-0.0.1.post1/bioino/gff2table.py`

 * *Files identical despite different names*

### Comparing `bioino-0.0.1/bioino/table2fasta.py` & `bioino-0.0.1.post1/bioino/table2fasta.py`

 * *Files identical despite different names*

### Comparing `bioino-0.0.1/bioino/tables.py` & `bioino-0.0.1.post1/bioino/tables.py`

 * *Files identical despite different names*

### Comparing `bioino-0.0.1/bioino.egg-info/PKG-INFO` & `bioino-0.0.1.post1/bioino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioino
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Lightweight IO and conversion for bioinformatics file formats.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
-Project-URL: Homepage, https://github.com/scbirlab/bioin
-Project-URL: Bug Tracker, https://github.com/scbirlab/bioin/issues
+Project-URL: Homepage, https://github.com/scbirlab/bioino
+Project-URL: Bug Tracker, https://github.com/scbirlab/bioino/issues
 Keywords: biology,bioinformatics,science,io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bioino-0.0.1/pyproject.toml` & `bioino-0.0.1.post1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bioino"
-version = "0.0.1"
+version = "0.0.1post1"
 authors = [
   { name="Eachan Johnson", email="eachan.johnson@crick.ac.uk" },
 ]
 description = "Lightweight IO and conversion for bioinformatics file formats."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
@@ -26,16 +26,16 @@
 ]
 
 dependencies = [ 
   "pandas"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/scbirlab/bioin"
-"Bug Tracker" = "https://github.com/scbirlab/bioin/issues"
+"Homepage" = "https://github.com/scbirlab/bioino"
+"Bug Tracker" = "https://github.com/scbirlab/bioino/issues"
 
 [project.scripts] 
 gff2table = "bioino.gff2table:main"
 table2fasta = "bioino.table2fasta:main"
 
 [build-system]
 # These are the assumed default build requirements from pip:
```

