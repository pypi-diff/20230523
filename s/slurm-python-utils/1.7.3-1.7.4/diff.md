# Comparing `tmp/slurm-python-utils-1.7.3.tar.gz` & `tmp/slurm-python-utils-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-python-utils-1.7.3.tar", last modified: Wed Feb 22 14:33:13 2023, max compression
+gzip compressed data, was "slurm-python-utils-1.7.4.tar", last modified: Tue May 23 16:15:36 2023, max compression
```

## Comparing `slurm-python-utils-1.7.3.tar` & `slurm-python-utils-1.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:33:13.076769 slurm-python-utils-1.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:33:13.072769 slurm-python-utils-1.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:33:13.076769 slurm-python-utils-1.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-22 14:33:13.076769 slurm-python-utils-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:33:13.076769 slurm-python-utils-1.7.3/job_lock/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/job_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25359 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/job_lock/job_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/job_lock/slurm_tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 14:33:13.076769 slurm-python-utils-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:33:13.076769 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-22 14:33:13.000000 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-22 14:33:13.000000 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 14:33:13.000000 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-22 14:33:13.000000 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-22 14:33:13.000000 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 14:33:13.000000 slurm-python-utils-1.7.3/slurm_python_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-02-22 14:32:52.000000 slurm-python-utils-1.7.3/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:15:36.313295 slurm-python-utils-1.7.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:15:36.309295 slurm-python-utils-1.7.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:15:36.309295 slurm-python-utils-1.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 16:15:36.313295 slurm-python-utils-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:15:36.309295 slurm-python-utils-1.7.4/job_lock/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/job_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25396 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/job_lock/job_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/job_lock/slurm_tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:15:36.313295 slurm-python-utils-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:15:36.313295 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-23 16:15:36.000000 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 16:15:36.000000 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:15:36.000000 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-23 16:15:36.000000 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 16:15:36.000000 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 16:15:36.000000 slurm-python-utils-1.7.4/slurm_python_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-05-23 16:15:19.000000 slurm-python-utils-1.7.4/test.py
```

### Comparing `slurm-python-utils-1.7.3/.github/workflows/ci.yml` & `slurm-python-utils-1.7.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `slurm-python-utils-1.7.3/LICENSE` & `slurm-python-utils-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-python-utils-1.7.3/NOTICE` & `slurm-python-utils-1.7.4/NOTICE`

 * *Files identical despite different names*

### Comparing `slurm-python-utils-1.7.3/job_lock/__init__.py` & `slurm-python-utils-1.7.4/job_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `slurm-python-utils-1.7.3/job_lock/job_lock.py` & `slurm-python-utils-1.7.4/job_lock/job_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import abc, argparse, contextlib, datetime, itertools, logging, os, pathlib, random, re, subprocess, sys, time, uuid
+import abc, argparse, contextlib, datetime, itertools, logging, os, pathlib, random, re, socket, subprocess, sys, time, uuid
 if sys.platform != "cygwin":
   import psutil
 
 logger = logging.getLogger("JobLock")
 logger.setLevel(logging.INFO)
 
 def rm_missing_ok(path):
@@ -278,19 +278,20 @@
 
   @property
   def wouldbevalid(self):
     if self: return True
     with self:
       return bool(self)
 
-  def runningjobinfo(self, exceptions=False):
+  def runningjobinfo(self, *, exceptions=False):
     try:
       with open(self.filename) as f:
         contents = f.read()
-        jobtype, cpuid, jobid = contents.split()
+        firstline = contents.split("\n")[0]
+        jobtype, cpuid, jobid = firstline.split()
         cpuid = int(cpuid)
         jobid = int(jobid)
         return jobtype, cpuid, jobid
     except (IOError, OSError, ValueError):
       if exceptions: raise
       return None, None, None
 
@@ -440,14 +441,15 @@
         return self
       else:
         raise
 
     self.f = os.fdopen(self.fd, 'w')
 
     message = " ".join(str(_) for _ in jobinfo())
+    message += "\n" + socket.gethostname()
     try:
       self.f.write(message+"\n")
     except (IOError, OSError):
       pass
     try:
       self.f.close()
     except (IOError, OSError):
@@ -524,16 +526,15 @@
 class JobLockAndWait(JobLock):
   defaultsilent = False
 
   def __init__(self, name, delay, *, printmessage=None, task="doing this", maxiterations=1000, silent=None, waitforinputs=False, **kwargs):
     super().__init__(name, **kwargs)
     self.delay = delay
     if printmessage is None:
-      printmessage = "Another process is already {task}.  Waiting {delay} seconds."
-    printmessage = printmessage.format(delay=delay, task=task)
+      printmessage = f"Another process is already {task}.  Waiting {delay} seconds."
     self.__printmessage = printmessage
     if silent is None:
       silent = self.defaultsilent
     self.__silent = silent
     self.__waitforinputs = waitforinputs
     self.niterations = 0
     self.maxiterations = maxiterations
```

### Comparing `slurm-python-utils-1.7.3/job_lock/slurm_tmpdir.py` & `slurm-python-utils-1.7.4/job_lock/slurm_tmpdir.py`

 * *Files identical despite different names*

### Comparing `slurm-python-utils-1.7.3/setup.py` & `slurm-python-utils-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `slurm-python-utils-1.7.3/test.py` & `slurm-python-utils-1.7.4/test.py`

 * *Files identical despite different names*

