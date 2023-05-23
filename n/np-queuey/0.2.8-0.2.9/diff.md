# Comparing `tmp/np_queuey-0.2.8.tar.gz` & `tmp/np_queuey-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.2.8.tar", last modified: Tue May  9 17:42:11 2023, max compression
+gzip compressed data, was "np_queuey-0.2.9.tar", last modified: Tue May  9 20:00:18 2023, max compression
```

## Comparing `np_queuey-0.2.8.tar` & `np_queuey-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.8/README.md
--rw-r--r--   0        0        0     2560 2023-05-09 17:42:11.922048 np_queuey-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.8/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.8/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.8/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.8/src/np_queuey/hueys/qc.py
--rw-r--r--   0        0        0     4602 2023-05-09 05:18:07.449224 np_queuey-0.2.8/src/np_queuey/hueys/sorting.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.8/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.8/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.8/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.8/src/np_queuey/jobs/run_sorting.py
--rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.8/src/np_queuey/jobs/sorting.py
--rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.8/src/np_queuey/queues/__init__.py
--rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.8/src/np_queuey/queues/huey_job_queue.py
--rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.8/src/np_queuey/queues/peewee_job_queue.py
--rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.8/src/np_queuey/queues/pipeline_qc_queue.py
--rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.8/src/np_queuey/queues/pipeline_sorting_queue.py
--rw-r--r--   0        0        0    11550 2023-05-09 17:39:26.303806 np_queuey-0.2.8/src/np_queuey/queues/sqlite_isilon_queue.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.8/src/np_queuey/tasks.py
--rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.8/src/np_queuey/types.py
--rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.8/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.8/tests/test_huey.py
--rw-r--r--   0        0        0     1708 1970-01-01 00:00:00.000000 np_queuey-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.9/README.md
+-rw-r--r--   0        0        0     2560 2023-05-09 20:00:18.850869 np_queuey-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.9/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.9/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.9/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0     2773 2023-05-09 19:34:28.870717 np_queuey-0.2.9/src/np_queuey/hueys/npexp_upload.py
+-rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.9/src/np_queuey/hueys/qc.py
+-rw-r--r--   0        0        0     4608 2023-05-09 18:05:11.294040 np_queuey-0.2.9/src/np_queuey/hueys/sorting.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.9/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.9/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.9/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.9/src/np_queuey/jobs/run_sorting.py
+-rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.9/src/np_queuey/jobs/sorting.py
+-rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.9/src/np_queuey/queues/__init__.py
+-rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.9/src/np_queuey/queues/huey_job_queue.py
+-rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.9/src/np_queuey/queues/peewee_job_queue.py
+-rw-r--r--   0        0        0      152 2023-05-09 17:52:13.458363 np_queuey-0.2.9/src/np_queuey/queues/pipeline_npexp_upload_queue.py
+-rw-r--r--   0        0        0      133 2023-05-09 17:51:36.934753 np_queuey-0.2.9/src/np_queuey/queues/pipeline_qc_queue.py
+-rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.9/src/np_queuey/queues/pipeline_sorting_queue.py
+-rw-r--r--   0        0        0    11550 2023-05-09 17:39:26.303806 np_queuey-0.2.9/src/np_queuey/queues/sqlite_isilon_queue.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.9/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.9/src/np_queuey/types.py
+-rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.9/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.9/tests/test_huey.py
+-rw-r--r--   0        0        0     1708 1970-01-01 00:00:00.000000 np_queuey-0.2.9/PKG-INFO
```

### Comparing `np_queuey-0.2.8/pyproject.toml` & `np_queuey-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.2.8"
+version = "0.2.9"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "np-config>=0.4.17",
```

### Comparing `np_queuey-0.2.8/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.9/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/hueys/qc.py` & `np_queuey-0.2.9/src/np_queuey/hueys/qc.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/hueys/sorting.py` & `np_queuey-0.2.9/src/np_queuey/hueys/sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     job = get_job(session_or_job, SortingJob)
     for probe_folder in probe_folders(job):
         src = pathlib.Path(f'D:/{probe_folder}')
         dest = np_session.Session(job.session).npexp_path / probe_folder
         logger.info(f'Moving {src} to {dest}')
         subprocess.run([
             'robocopy', f'{src}', f'{dest}',
-             '/MOVE', '/E', '/COPYALL', '/R:0', '/W:0', '/MT:32'
+             '/MOVE', '/E', '/J', '/COPYALL', '/R:0', '/W:0', '/MT:32'
              ], check=False) # return code from robocopy doesn't signal failure      
         if src.exists():
             np_tools.move(src, dest, ignore_errors=True)
             
 def remove_raw_data_on_acq_drives(session_or_job: SortingJob | SessionArgs) -> None:
     session = get_session(session_or_job)
     for drive in ('A:', 'B:'):
```

### Comparing `np_queuey-0.2.8/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.9/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/jobs/sorting.py` & `np_queuey-0.2.9/src/np_queuey/jobs/sorting.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/queues/huey_job_queue.py` & `np_queuey-0.2.9/src/np_queuey/queues/huey_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/queues/peewee_job_queue.py` & `np_queuey-0.2.9/src/np_queuey/queues/peewee_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/queues/sqlite_isilon_queue.py` & `np_queuey-0.2.9/src/np_queuey/queues/sqlite_isilon_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/types.py` & `np_queuey-0.2.9/src/np_queuey/types.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/src/np_queuey/utils.py` & `np_queuey-0.2.9/src/np_queuey/utils.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/tests/test_huey.py` & `np_queuey-0.2.9/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.8/PKG-INFO` & `np_queuey-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

