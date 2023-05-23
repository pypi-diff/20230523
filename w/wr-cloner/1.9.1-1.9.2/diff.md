# Comparing `tmp/wr-cloner-1.9.1.tar.gz` & `tmp/wr-cloner-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wr-cloner-1.9.1.tar", last modified: Sun Mar 19 14:53:58 2023, max compression
+gzip compressed data, was "wr-cloner-1.9.2.tar", last modified: Tue May 23 15:25:57 2023, max compression
```

## Comparing `wr-cloner-1.9.1.tar` & `wr-cloner-1.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 14:53:58.404681 wr-cloner-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-19 14:53:58.404681 wr-cloner-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 14:53:58.404681 wr-cloner-1.9.1/cloner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/clone_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/cloner_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/cpu_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/obtain_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/put_repos_in_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/cloner/split_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-19 14:53:58.404681 wr-cloner-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 14:53:58.404681 wr-cloner-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/tests/test_cloner_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/tests/test_obtain_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/tests/test_put_repos_in_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-19 14:53:47.000000 wr-cloner-1.9.1/tests/test_split_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 14:53:58.404681 wr-cloner-1.9.1/wr_cloner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-19 14:53:58.000000 wr-cloner-1.9.1/wr_cloner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-19 14:53:58.000000 wr-cloner-1.9.1/wr_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 14:53:58.000000 wr-cloner-1.9.1/wr_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-19 14:53:58.000000 wr-cloner-1.9.1/wr_cloner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-19 14:53:58.000000 wr-cloner-1.9.1/wr_cloner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-19 14:53:58.000000 wr-cloner-1.9.1/wr_cloner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:57.786708 wr-cloner-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-23 15:25:57.786708 wr-cloner-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:57.782708 wr-cloner-1.9.2/cloner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/clone_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/cloner_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/cpu_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/obtain_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/put_repos_in_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/cloner/split_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 15:25:57.786708 wr-cloner-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:57.786708 wr-cloner-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/tests/test_cloner_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/tests/test_obtain_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/tests/test_put_repos_in_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-23 15:25:45.000000 wr-cloner-1.9.2/tests/test_split_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:25:57.786708 wr-cloner-1.9.2/wr_cloner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-23 15:25:57.000000 wr-cloner-1.9.2/wr_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 15:25:57.000000 wr-cloner-1.9.2/wr_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:25:57.000000 wr-cloner-1.9.2/wr_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 15:25:57.000000 wr-cloner-1.9.2/wr_cloner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 15:25:57.000000 wr-cloner-1.9.2/wr_cloner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 15:25:57.000000 wr-cloner-1.9.2/wr_cloner.egg-info/top_level.txt
```

### Comparing `wr-cloner-1.9.1/LICENSE` & `wr-cloner-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/PKG-INFO` & `wr-cloner-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wr-cloner
-Version: 1.9.1
+Version: 1.9.2
 Summary: A tool to clone efficiently all the repos in an organization
 Author: w0rmr1d3r
 License: MIT
 Project-URL: Homepage, https://github.com/w0rmr1d3r/cloner
 Project-URL: Repository, https://github.com/w0rmr1d3r/cloner
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/cloner/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/cloner
```

### Comparing `wr-cloner-1.9.1/README.md` & `wr-cloner-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/cli.py` & `wr-cloner-1.9.2/cloner/cli.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/clone_repos.py` & `wr-cloner-1.9.2/cloner/clone_repos.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/cloner_process.py` & `wr-cloner-1.9.2/cloner/cloner_process.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/cpu_config.py` & `wr-cloner-1.9.2/cloner/cpu_config.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/obtain_repos.py` & `wr-cloner-1.9.2/cloner/obtain_repos.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/put_repos_in_queue.py` & `wr-cloner-1.9.2/cloner/put_repos_in_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/repository.py` & `wr-cloner-1.9.2/cloner/repository.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/cloner/split_queue.py` & `wr-cloner-1.9.2/cloner/split_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/pyproject.toml` & `wr-cloner-1.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Topic :: Software Development :: Version Control",
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: System",
 ]
 # Make sure this matches the keywords in GitHub
 keywords = ["github", "python", "git", "clone", "organization", "multiprocessing", "multithreading", "python3"]
 # Make sure this matches the version in __version__.py
-version = "1.9.1"
+version = "1.9.2"
 # Supported Python 3.9 and above
 # If supporting newer versions, update ->  CI and classifiers
 # If minimum version supported changes, update -> CI, coverage, classifiers, pylint, release, contributing.
 requires-python = ">=3.9.0"
 
 # Always try to be compatible with these versions and above
 dependencies = [
```

### Comparing `wr-cloner-1.9.1/tests/test_cloner_process.py` & `wr-cloner-1.9.2/tests/test_cloner_process.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/tests/test_obtain_repos.py` & `wr-cloner-1.9.2/tests/test_obtain_repos.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/tests/test_put_repos_in_queue.py` & `wr-cloner-1.9.2/tests/test_put_repos_in_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/tests/test_repository.py` & `wr-cloner-1.9.2/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/tests/test_split_queue.py` & `wr-cloner-1.9.2/tests/test_split_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.1/wr_cloner.egg-info/PKG-INFO` & `wr-cloner-1.9.2/wr_cloner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wr-cloner
-Version: 1.9.1
+Version: 1.9.2
 Summary: A tool to clone efficiently all the repos in an organization
 Author: w0rmr1d3r
 License: MIT
 Project-URL: Homepage, https://github.com/w0rmr1d3r/cloner
 Project-URL: Repository, https://github.com/w0rmr1d3r/cloner
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/cloner/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/cloner
```

### Comparing `wr-cloner-1.9.1/wr_cloner.egg-info/SOURCES.txt` & `wr-cloner-1.9.2/wr_cloner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

