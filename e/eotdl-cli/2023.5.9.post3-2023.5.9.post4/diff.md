# Comparing `tmp/eotdl-cli-2023.5.9.post3.tar.gz` & `tmp/eotdl-cli-2023.5.9.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-cli-2023.5.9.post3.tar", max compression
+gzip compressed data, was "eotdl-cli-2023.5.9.post4.tar", max compression
```

## Comparing `eotdl-cli-2023.5.9.post3.tar` & `eotdl-cli-2023.5.9.post4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post3/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post3/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post3/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     2537 2023-05-09 14:49:28.320318 eotdl-cli-2023.5.9.post3/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post3/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     7709 2023-05-09 15:00:49.243575 eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      932 2023-05-09 14:32:14.727109 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      820 2023-05-09 14:38:59.864610 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0      837 2023-05-09 14:50:06.056518 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-05-09 14:26:26.021798 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      148 2023-05-09 14:56:32.370413 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1842 2023-05-09 14:50:08.224530 eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      604 2023-05-09 15:04:18.048486 eotdl-cli-2023.5.9.post3/pyproject.toml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post3/setup.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post3/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post4/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post4/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post4/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     2125 2023-05-09 15:21:02.804320 eotdl-cli-2023.5.9.post4/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post4/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     7709 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      932 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      820 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0      837 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      148 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1842 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      604 2023-05-09 15:31:07.174517 eotdl-cli-2023.5.9.post4/pyproject.toml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post4/setup.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post4/PKG-INFO
```

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/commands/auth.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/commands/datasets.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/commands/datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,54 +57,35 @@
 
 
 @app.command()
 def ingest(
     path: str,
     n: Optional[str] = None,
     d: Optional[str] = None,
-    y: Optional[bool] = False,
+    p: Optional[bool] = False,
 ):
     """
     Ingest a dataset
 
     path: Path to dataset to ingest
+    n: Name of the dataset
+    d: Description of the dataset
+    p: Parallel ingest
     """
     try:
         user = auth()
         name = n or typer.prompt("Dataset name")
         description = d or typer.prompt("Description")
         # confirm
-        if not y:
+        if not n or not d:
             typer.confirm(f"Is the data correct?", abort=True)
-        ingest_large_dataset(name, description, path, user, typer.echo)
-        typer.echo(f"Dataset {name} ingested")
-    except Exception as e:
-        typer.echo(e)
-
-
-@app.command()
-def pingest(
-    path: str,
-    n: Optional[str] = None,
-    d: Optional[str] = None,
-    y: Optional[bool] = False,
-):
-    """
-    Ingest a dataset
-
-    path: Path to dataset to ingest
-    """
-    try:
-        user = auth()
-        name = n or typer.prompt("Dataset name")
-        description = d or typer.prompt("Description")
-        # confirm
-        if not y:
-            typer.confirm(f"Is the data correct?", abort=True)
-        ingest_large_dataset_parallel(name, description, path, user, typer.echo)
+        if p:
+            ingest_large_dataset_parallel(name, description, path, user, typer.echo)
+        else:
+            ingest_large_dataset(name, description, path, user, typer.echo)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/APIRepo.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/repos/AuthRepo.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/auth/main.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/eotdl_cli/src/usecases/datasets/main.py` & `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post3/pyproject.toml` & `eotdl-cli-2023.5.9.post4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.05.09-3"
+version = "2023.05.09-4"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-cli-2023.5.9.post3/setup.py` & `eotdl-cli-2023.5.9.post4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl-cli = eotdl_cli.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl-cli',
-    'version': '2023.5.9.post3',
+    'version': '2023.5.9.post4',
     'description': '',
     'long_description': '# eotdl-cli\n\nThis is the CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-cli-2023.5.9.post3/PKG-INFO` & `eotdl-cli-2023.5.9.post4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.5.9.post3
+Version: 2023.5.9.post4
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

