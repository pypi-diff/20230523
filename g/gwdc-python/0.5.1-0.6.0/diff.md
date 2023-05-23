# Comparing `tmp/gwdc_python-0.5.1.tar.gz` & `tmp/gwdc_python-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdc_python-0.5.1.tar", max compression
+gzip compressed data, was "gwdc_python-0.6.0.tar", max compression
```

## Comparing `gwdc_python-0.5.1.tar` & `gwdc_python-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1076 2021-07-19 20:27:11.070554 gwdc_python-0.5.1/LICENSE
--rw-r--r--   0        0        0      195 2021-07-19 20:27:11.070554 gwdc_python-0.5.1/README.rst
--rw-r--r--   0        0        0       67 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/__init__.py
--rw-r--r--   0        0        0       47 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/gwdc_python/constants.py
--rw-r--r--   0        0        0     1091 2022-08-09 17:58:23.302425 gwdc_python-0.5.1/gwdc_python/exceptions.py
--rw-r--r--   0        0        0       61 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/__init__.py
--rw-r--r--   0        0        0     3980 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/file_reference.py
--rw-r--r--   0        0        0     2598 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/filters.py
--rw-r--r--   0        0        0      659 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/identifiers.py
--rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/__init__.py
--rw-r--r--   0        0        0     4897 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/test_file_reference.py
--rw-r--r--   0        0        0     4444 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/test_filters.py
--rw-r--r--   0        0        0     3296 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/test_identifiers.py
--rw-r--r--   0        0        0     5626 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/gwdc_python/gwdc.py
--rw-r--r--   0        0        0      541 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/helpers.py
--rw-r--r--   0        0        0       26 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/__init__.py
--rw-r--r--   0        0        0     1421 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/base.py
--rw-r--r--   0        0        0     3298 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/meta.py
--rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/tests/__init__.py
--rw-r--r--   0        0        0      789 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/tests/test_base.py
--rw-r--r--   0        0        0      830 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/tests/test_meta.py
--rw-r--r--   0        0        0      227 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/logger.py
--rw-r--r--   0        0        0        0 2021-06-30 01:51:45.372719 gwdc_python-0.5.1/gwdc_python/tests/__init__.py
--rw-r--r--   0        0        0     5422 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/gwdc_python/tests/test_gwdc_python.py
--rw-r--r--   0        0        0      112 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/tests/__init__.py
--rw-r--r--   0        0        0     2244 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1337 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/typed_list.py
--rw-r--r--   0        0        0     2709 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/utils.py
--rw-r--r--   0        0        0      898 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 gwdc_python-0.5.1/setup.py
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 gwdc_python-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-07-19 20:27:11.070554 gwdc_python-0.6.0/LICENSE
+-rw-r--r--   0        0        0      195 2021-07-19 20:27:11.070554 gwdc_python-0.6.0/README.rst
+-rw-r--r--   0        0        0       67 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-04 01:13:40.935287 gwdc_python-0.6.0/gwdc_python/constants.py
+-rw-r--r--   0        0        0     1091 2022-08-09 17:58:23.302425 gwdc_python-0.6.0/gwdc_python/exceptions.py
+-rw-r--r--   0        0        0       61 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/files/__init__.py
+-rw-r--r--   0        0        0      229 2023-05-23 06:20:39.338727 gwdc_python-0.6.0/gwdc_python/files/constants.py
+-rw-r--r--   0        0        0     4304 2023-05-23 06:20:39.338727 gwdc_python-0.6.0/gwdc_python/files/file_reference.py
+-rw-r--r--   0        0        0     2598 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/files/filters.py
+-rw-r--r--   0        0        0      659 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/files/identifiers.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/files/tests/__init__.py
+-rw-r--r--   0        0        0     5780 2023-05-23 06:20:39.338727 gwdc_python-0.6.0/gwdc_python/files/tests/test_file_reference.py
+-rw-r--r--   0        0        0     4444 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/files/tests/test_filters.py
+-rw-r--r--   0        0        0     3296 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/files/tests/test_identifiers.py
+-rw-r--r--   0        0        0     5626 2023-05-04 01:13:40.935287 gwdc_python-0.6.0/gwdc_python/gwdc.py
+-rw-r--r--   0        0        0      541 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/helpers.py
+-rw-r--r--   0        0        0       26 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/jobs/__init__.py
+-rw-r--r--   0        0        0     1407 2023-05-23 06:20:39.338727 gwdc_python-0.6.0/gwdc_python/jobs/base.py
+-rw-r--r--   0        0        0     3298 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/jobs/meta.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/jobs/tests/__init__.py
+-rw-r--r--   0        0        0      789 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/jobs/tests/test_base.py
+-rw-r--r--   0        0        0      830 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/jobs/tests/test_meta.py
+-rw-r--r--   0        0        0      227 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/logger.py
+-rw-r--r--   0        0        0        0 2021-06-30 01:51:45.372719 gwdc_python-0.6.0/gwdc_python/tests/__init__.py
+-rw-r--r--   0        0        0     5422 2023-05-04 01:13:40.935287 gwdc_python-0.6.0/gwdc_python/tests/test_gwdc_python.py
+-rw-r--r--   0        0        0      112 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2244 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1337 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/utils/typed_list.py
+-rw-r--r--   0        0        0     2709 2022-06-17 01:28:34.516404 gwdc_python-0.6.0/gwdc_python/utils/utils.py
+-rw-r--r--   0        0        0      913 2023-05-23 06:20:39.338727 gwdc_python-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 gwdc_python-0.6.0/PKG-INFO
```

### Comparing `gwdc_python-0.5.1/LICENSE` & `gwdc_python-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/exceptions.py` & `gwdc_python-0.6.0/gwdc_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/files/file_reference.py` & `gwdc_python-0.6.0/gwdc_python/files/file_reference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+import urllib.parse
 from dataclasses import dataclass, field
 from pathlib import Path
 from . import filters
+from .constants import JobType
 from ..utils import remove_path_anchor, TypedList
 
 
 @dataclass
 class FileReference:
     """Object used to facilitate simpler downloading of files.
     """
+
     path: str
     file_size: int = field(repr=False)
     download_token: str = field(repr=False)
     job_id: int = field(repr=False)
-    uploaded: bool = field(repr=False, default=False)
+    job_type: int = field(repr=False, default=JobType.NORMAL_JOB)
 
     def __post_init__(self):
-        self.path = remove_path_anchor(Path(self.path))
+        if self.job_type != JobType.GWOSC_JOB:
+            self.path = remove_path_anchor(Path(self.path))
+
         self.file_size = int(self.file_size)
 
 
 class FileReferenceList(TypedList):
     def __init__(self, data=[]):
         super().__init__(item_type=FileReference, data=data)
 
@@ -96,23 +101,23 @@
         Returns
         -------
         list
             List of file paths
         """
         return [ref.path for ref in self.data]
 
-    def get_uploaded(self):
-        """Get whether the files are from an uploaded job in a list
+    def get_job_type(self):
+        """Get the job type for each job in a list
 
         Returns
         -------
         list
-            List of True for uploaded jobs, False for submitted jobs
+            List of JobType for jobs
         """
-        return [ref.uploaded for ref in self.data]
+        return [ref.job_type for ref in self.data]
 
     def get_output_paths(self, root_path, preserve_directory_structure=True):
         """Get all the file paths modified to give them a base directory.
         Can also optionally remove any existing directory structure
 
         Parameters
         ----------
@@ -124,12 +129,20 @@
         Returns
         -------
         list
             List of output file paths
         """
         paths = []
         for ref in self.data:
+            if ref.job_type == JobType.GWOSC_JOB:
+                path = urllib.parse.urlparse(ref.path).path
+                path = Path(path.rsplit('/', 1).pop())
+                path = remove_path_anchor(path)
+            else:
+                path = ref.path
+
             if preserve_directory_structure:
-                paths.append(root_path / ref.path)
+                paths.append(root_path / path)
             else:
-                paths.append(root_path / Path(ref.path.name))
+                paths.append(root_path / Path(path.name))
+
         return paths
```

### Comparing `gwdc_python-0.5.1/gwdc_python/files/filters.py` & `gwdc_python-0.6.0/gwdc_python/files/filters.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/files/identifiers.py` & `gwdc_python-0.6.0/gwdc_python/files/identifiers.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/files/tests/test_file_reference.py` & `gwdc_python-0.6.0/gwdc_python/files/tests/test_file_reference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,106 @@
 import pytest
 from pathlib import Path
 from collections import OrderedDict
+
+from gwdc_python.files.constants import JobType
 from gwdc_python.files.file_reference import FileReference, FileReferenceList
 from gwdc_python.utils import remove_path_anchor
 
 
 @pytest.fixture
 def setup_dicts():
     return [
         {
             'path': 'data/dir/test1.png',
             'file_size': '1',
             'download_token': 'test_token_1',
             'job_id': 'id1',
-            'uploaded': False
+            'job_type': JobType.NORMAL_JOB
         },
         {
             'path': 'data/dir/test2.png',
             'file_size': '1',
             'download_token': 'test_token_2',
             'job_id': 'id1',
-            'uploaded': False
+            'job_type': JobType.NORMAL_JOB
         },
         {
             'path': 'result/dir/test1.txt',
             'file_size': '1',
             'download_token': 'test_token_3',
             'job_id': 'id2',
-            'uploaded': True
+            'job_type': JobType.UPLOADED_JOB
         },
         {
             'path': 'result/dir/test2.txt',
             'file_size': '1',
             'download_token': 'test_token_4',
             'job_id': 'id2',
-            'uploaded': True
+            'job_type': JobType.UPLOADED_JOB
         },
         {
             'path': 'test1.json',
             'file_size': '1',
             'download_token': 'test_token_5',
             'job_id': 'id3',
-            'uploaded': False
+            'job_type': JobType.NORMAL_JOB
         },
         {
             'path': 'test2.json',
             'file_size': '1',
             'download_token': 'test_token_6',
             'job_id': 'id3',
-            'uploaded': False
+            'job_type': JobType.NORMAL_JOB
+        },
+        {
+            'path': 'https://myurl.com/test/file1.h5',
+            'file_size': '1',
+            'download_token': 'test_token_8',
+            'job_id': 'id4',
+            'job_type': JobType.GWOSC_JOB
+        },
+        {
+            'path': 'https://anotherurl.net/test/whatever/file2.h5?download=1',
+            'file_size': '1',
+            'download_token': 'test_token_9',
+            'job_id': 'id4',
+            'job_type': JobType.GWOSC_JOB
         },
     ]
 
 
 def test_file_reference(setup_dicts):
     for file_dict in setup_dicts:
         ref = FileReference(**file_dict)
-        assert ref.path == remove_path_anchor(Path(file_dict['path']))
+        if ref.job_type == JobType.GWOSC_JOB:
+            assert ref.path == file_dict['path']
+        else:
+            assert ref.path == remove_path_anchor(Path(file_dict['path']))
         assert ref.file_size == int(file_dict['file_size'])
         assert ref.download_token == file_dict['download_token']
         assert ref.job_id == file_dict['job_id']
-        assert ref.uploaded == file_dict['uploaded']
+        assert ref.job_type == file_dict['job_type']
 
 
 def test_file_reference_list(setup_dicts):
     file_references = [FileReference(**file_dict) for file_dict in setup_dicts]
     file_reference_list = FileReferenceList(file_references)
 
     for i, ref in enumerate(file_reference_list):
         assert ref.path == file_references[i].path
         assert ref.file_size == file_references[i].file_size
         assert ref.download_token == file_references[i].download_token
         assert ref.job_id == file_references[i].job_id
-        assert ref.uploaded == file_references[i].uploaded
+        assert ref.job_type == file_references[i].job_type
 
     assert file_reference_list.get_total_bytes() == sum([ref.file_size for ref in file_references])
     assert file_reference_list.get_tokens() == [ref.download_token for ref in file_references]
     assert file_reference_list.get_paths() == [ref.path for ref in file_references]
-    assert file_reference_list.get_uploaded() == [ref.uploaded for ref in file_references]
+    assert file_reference_list.get_job_type() == [ref.job_type for ref in file_references]
 
 
 def test_file_reference_list_types(setup_dicts):
     # FileReferenceList can be created from list of FileReference objects
     file_references = [FileReference(**file_dict) for file_dict in setup_dicts]
     file_reference_list = FileReferenceList(file_references)
 
@@ -112,31 +131,36 @@
     root_path = Path('test_dir')
     output_paths = [
         root_path / 'data/dir/test1.png',
         root_path / 'data/dir/test2.png',
         root_path / 'result/dir/test1.txt',
         root_path / 'result/dir/test2.txt',
         root_path / 'test1.json',
-        root_path / 'test2.json'
+        root_path / 'test2.json',
+        root_path / 'file1.h5',
+        root_path / 'file2.h5'
     ]
     output_paths_flat = [
         root_path / 'test1.png',
         root_path / 'test2.png',
         root_path / 'test1.txt',
         root_path / 'test2.txt',
         root_path / 'test1.json',
-        root_path / 'test2.json'
+        root_path / 'test2.json',
+        root_path / 'file1.h5',
+        root_path / 'file2.h5'
     ]
     assert output_paths == file_reference_list.get_output_paths(root_path)
     assert output_paths_flat == file_reference_list.get_output_paths(root_path, preserve_directory_structure=False)
 
 
 def test_batch_file_reference_list(setup_dicts):
     file_reference_list = FileReferenceList([FileReference(**file_dict) for file_dict in setup_dicts])
 
     batched = OrderedDict(
         id1=file_reference_list[0:2],
         id2=file_reference_list[2:4],
         id3=file_reference_list[4:6],
+        id4=file_reference_list[6:8],
     )
 
     assert file_reference_list.batched == batched
```

### Comparing `gwdc_python-0.5.1/gwdc_python/files/tests/test_filters.py` & `gwdc_python-0.6.0/gwdc_python/files/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/files/tests/test_identifiers.py` & `gwdc_python-0.6.0/gwdc_python/files/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/gwdc.py` & `gwdc_python-0.6.0/gwdc_python/gwdc.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/helpers.py` & `gwdc_python-0.6.0/gwdc_python/helpers.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/jobs/base.py` & `gwdc_python-0.6.0/gwdc_python/jobs/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, client, job_id, name, description, user, job_status):
         self.client = client
         self.job_id = job_id
         self.name = name
         self.description = description
         self.user = user
         self.status = JobStatus(status=job_status['name'], date=job_status['date'])
-        self.is_uploaded_job = None
+        self.job_type = None
 
     def __repr__(self):
         return f"{self.__class__.__name__}(name={self.name}, job_id={self.job_id})"
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return (
@@ -32,9 +32,9 @@
         """Get information for all files associated with this job
 
         Returns
         -------
         ~gwdc_python.files.file_reference.FileReferenceList
             Contains FileReference instances for each of the files associated with this job
         """
-        result, self.is_uploaded_job = self.client._get_files_by_job_id(self.job_id)
+        result, self.job_type = self.client._get_files_by_job_id(self.job_id)
         return result
```

### Comparing `gwdc_python-0.5.1/gwdc_python/jobs/meta.py` & `gwdc_python-0.6.0/gwdc_python/jobs/meta.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/jobs/tests/test_base.py` & `gwdc_python-0.6.0/gwdc_python/jobs/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/jobs/tests/test_meta.py` & `gwdc_python-0.6.0/gwdc_python/jobs/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/tests/test_gwdc_python.py` & `gwdc_python-0.6.0/gwdc_python/tests/test_gwdc_python.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/utils/tests/test_utils.py` & `gwdc_python-0.6.0/gwdc_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/utils/typed_list.py` & `gwdc_python-0.6.0/gwdc_python/utils/typed_list.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/gwdc_python/utils/utils.py` & `gwdc_python-0.6.0/gwdc_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.1/pyproject.toml` & `gwdc_python-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwdc-python"
-version = "0.5.1"
+version = "0.6.0"
 description = "API for GWDC modules"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwdc_python"
 include = ["LICENSE",]
 
@@ -15,14 +15,15 @@
 requests-toolbelt = "^0.9.1"
 tqdm = "^4.61.2"
 importlib-metadata = "^4.5.0"
 Sphinx = {version = "^4.0.2", optional = true}
 sphinx-rtd-theme = {version = "^0.5.2", optional = true}
 pyhumps = "^3.7.1"
 appdirs = "^1.4.4"
+urllib3 = "^1"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3"
 requests-mock = "^1.8.0"
```

### Comparing `gwdc_python-0.5.1/PKG-INFO` & `gwdc_python-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdc-python
-Version: 0.5.1
+Version: 0.6.0
 Summary: API for GWDC modules
 Home-page: https://github.com/gravitationalwavedc/gwdc_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,15 @@
 Requires-Dist: importlib-metadata (>=4.5.0,<5.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.1,<4.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
+Requires-Dist: urllib3 (>=1,<2)
 Project-URL: Repository, https://github.com/gravitationalwavedc/gwdc_python
 Description-Content-Type: text/x-rst
 
 GWDC Python API
 ===============
 
 This package handles requests for the GWDC modules. Presently, it primarily handles the requests for `gwcloud-python <https://pypi.org/project/gwcloud-python/>`_.
```

