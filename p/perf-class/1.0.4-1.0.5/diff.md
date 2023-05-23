# Comparing `tmp/perf-class-1.0.4.tar.gz` & `tmp/perf-class-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perf-class-1.0.4.tar", last modified: Mon Jul 19 13:44:57 2021, max compression
+gzip compressed data, was "perf-class-1.0.5.tar", last modified: Tue May 23 08:21:00 2023, max compression
```

## Comparing `perf-class-1.0.4.tar` & `perf-class-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2021-07-19 13:44:57.957399 perf-class-1.0.4/
--rw-r--r--   0 tom       (1001) nslab     (1000)     1069 2020-12-01 14:38:09.000000 perf-class-1.0.4/LICENSE
--rw-r--r--   0 tom       (1001) nslab     (1000)     4335 2021-07-19 13:44:57.957399 perf-class-1.0.4/PKG-INFO
--rw-r--r--   0 tom       (1001) nslab     (1000)     3756 2021-07-19 13:28:23.000000 perf-class-1.0.4/README.md
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2021-07-19 13:44:57.957399 perf-class-1.0.4/perf_class/
--rw-r--r--   0 tom       (1001) nslab     (1000)        0 2020-12-01 14:38:09.000000 perf-class-1.0.4/perf_class/__init__.py
--rwxr-xr-x   0 tom       (1001) nslab     (1000)     7107 2020-12-01 14:38:09.000000 perf-class-1.0.4/perf_class/perf_class.py
-drwxr-xr-x   0 tom       (1001) nslab     (1000)        0 2021-07-19 13:44:57.957399 perf-class-1.0.4/perf_class.egg-info/
--rw-r--r--   0 tom       (1001) nslab     (1000)     4335 2021-07-19 13:44:57.000000 perf-class-1.0.4/perf_class.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1001) nslab     (1000)      247 2021-07-19 13:44:57.000000 perf-class-1.0.4/perf_class.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)        1 2021-07-19 13:44:57.000000 perf-class-1.0.4/perf_class.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)       64 2021-07-19 13:44:57.000000 perf-class-1.0.4/perf_class.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)       11 2021-07-19 13:44:57.000000 perf-class-1.0.4/perf_class.egg-info/top_level.txt
--rw-r--r--   0 tom       (1001) nslab     (1000)       38 2021-07-19 13:44:57.957399 perf-class-1.0.4/setup.cfg
--rw-r--r--   0 tom       (1001) nslab     (1000)      907 2021-07-19 13:44:42.000000 perf-class-1.0.4/setup.py
+drwxr-xr-x   0 tbarbette (108557) stafinfo    (36)        0 2023-05-23 08:21:00.753574 perf-class-1.0.5/
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)     1069 2023-05-23 08:10:47.000000 perf-class-1.0.5/LICENSE
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)     3997 2023-05-23 08:21:00.753574 perf-class-1.0.5/PKG-INFO
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)     3464 2023-05-23 08:10:47.000000 perf-class-1.0.5/README.md
+drwxr-xr-x   0 tbarbette (108557) stafinfo    (36)        0 2023-05-23 08:21:00.747574 perf-class-1.0.5/perf_class/
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)        0 2023-05-23 08:10:47.000000 perf-class-1.0.5/perf_class/__init__.py
+-rwxr-xr-x   0 tbarbette (108557) stafinfo    (36)     7107 2023-05-23 08:20:23.000000 perf-class-1.0.5/perf_class/perf_class.py
+drwxr-xr-x   0 tbarbette (108557) stafinfo    (36)        0 2023-05-23 08:21:00.752574 perf-class-1.0.5/perf_class.egg-info/
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)     3997 2023-05-23 08:21:00.000000 perf-class-1.0.5/perf_class.egg-info/PKG-INFO
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)      247 2023-05-23 08:21:00.000000 perf-class-1.0.5/perf_class.egg-info/SOURCES.txt
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)        1 2023-05-23 08:21:00.000000 perf-class-1.0.5/perf_class.egg-info/dependency_links.txt
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)       63 2023-05-23 08:21:00.000000 perf-class-1.0.5/perf_class.egg-info/entry_points.txt
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)       11 2023-05-23 08:21:00.000000 perf-class-1.0.5/perf_class.egg-info/top_level.txt
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)       38 2023-05-23 08:21:00.753574 perf-class-1.0.5/setup.cfg
+-rw-r--r--   0 tbarbette (108557) stafinfo    (36)      898 2023-05-23 08:20:51.000000 perf-class-1.0.5/setup.py
```

### Comparing `perf-class-1.0.4/LICENSE` & `perf-class-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `perf-class-1.0.4/PKG-INFO` & `perf-class-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: perf-class
-Version: 1.0.4
-Summary: A tool to map perf script events to classes of events using a set of regex
+Version: 1.0.5
+Summary: A tool to mep perf script events to classes of events using regex
 Home-page: https://github.com/tbarbette/perf-class
 Author: Tom Barbette
 Author-email: t.barbette@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # perf-class
 
-This program allows to group the CPU time spent in functions as outputed by perf script into classes. Eg. if your application spend 3% of time in "sort\_down", 5% "sort\_up", 4% "sort\_final", and you give a map like "sort: Sorting", this tool will summarize those as "Sorting 12%".
+This program allows to group the CPU time spent in functions as outputed by perf script into classes. Eg. if your application spend 3% of time in "sort_down", 5% "sort_up", 4% "sort_final", and you give a map like "sort: Sorting", this tool will summarize those as "Sorting 12%".
 
-This program is intended as a post-processor to show where, roughly, a CPU spends its time in various part of an application. The result such as "Sorting : 12%, Computing : 23%" can be given to a pie chart, typically.
+This program is intended as a preprocessor to show where, roughly, a CPU spend its time in various application. The result such as "Sorting : 12%, Computing : 23%" can be given to a pie chart, typically.
 
-The map file, to describe the mapping, is simply a series of "regex : class", one by line. Each symbol will be matched against the regex, and upon match will be considered of the given class. The tool will start with the top of the stack trace, and if no match is found, re-try with the previous function in the stack, etc. This is needed for cases where a lot of time is spent in a generic function like the Linux kernel "raw\_spin\_lock" functions, that cannot be clearly tied to a specific event. However the calling function, or one before can be clearly mapped to a "class" of event. This is why in our case we could not simply use the output of perf top, as it does not make much sense, and there are hundred "top" functions that cannot be mapped to classes manually.
-Only the calling functions of those generic hit points will allow to find the reason of the time spent there, and therefore enables mapping of the class.
+The map file, to describe the mapping, is simply a series of "regex : class", one by line. Each symbol will be matched against the regex, and upon match will be considered of the given class. The tool will start with the top of the stack trace, and if no match is found, re-try with the previous function in the stack, etc. This is needed, and explain why a simple script was not sufficient to achieve the purpose of this script as a lot of time spend in the kernel is in "raw_spin_lock" functions.
+Only the calling functions of those generic hit points will allow to find the reason of the time spent there, and therefore allow a mapping to the class.
 
 # Installation
 This package can be installed with pip, for instance:
 ```bash
 pip3 --user install perf-class
 ```
 
@@ -105,9 +103,7 @@
 read_tsc 0.005070
 rcu_all_qs 0.005068
 __softirqentry_text_start 0.005063
 lapic_next_deadline 0.005061
 ```
 
 See perf-class --help for other options
-
-
```

### Comparing `perf-class-1.0.4/README.md` & `perf-class-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # perf-class
 
-This program allows to group the CPU time spent in functions as outputed by perf script into classes. Eg. if your application spend 3% of time in "sort\_down", 5% "sort\_up", 4% "sort\_final", and you give a map like "sort: Sorting", this tool will summarize those as "Sorting 12%".
+This program allows to group the CPU time spent in functions as outputed by perf script into classes. Eg. if your application spend 3% of time in "sort_down", 5% "sort_up", 4% "sort_final", and you give a map like "sort: Sorting", this tool will summarize those as "Sorting 12%".
 
-This program is intended as a post-processor to show where, roughly, a CPU spends its time in various part of an application. The result such as "Sorting : 12%, Computing : 23%" can be given to a pie chart, typically.
+This program is intended as a preprocessor to show where, roughly, a CPU spend its time in various application. The result such as "Sorting : 12%, Computing : 23%" can be given to a pie chart, typically.
 
-The map file, to describe the mapping, is simply a series of "regex : class", one by line. Each symbol will be matched against the regex, and upon match will be considered of the given class. The tool will start with the top of the stack trace, and if no match is found, re-try with the previous function in the stack, etc. This is needed for cases where a lot of time is spent in a generic function like the Linux kernel "raw\_spin\_lock" functions, that cannot be clearly tied to a specific event. However the calling function, or one before can be clearly mapped to a "class" of event. This is why in our case we could not simply use the output of perf top, as it does not make much sense, and there are hundred "top" functions that cannot be mapped to classes manually.
-Only the calling functions of those generic hit points will allow to find the reason of the time spent there, and therefore enables mapping of the class.
+The map file, to describe the mapping, is simply a series of "regex : class", one by line. Each symbol will be matched against the regex, and upon match will be considered of the given class. The tool will start with the top of the stack trace, and if no match is found, re-try with the previous function in the stack, etc. This is needed, and explain why a simple script was not sufficient to achieve the purpose of this script as a lot of time spend in the kernel is in "raw_spin_lock" functions.
+Only the calling functions of those generic hit points will allow to find the reason of the time spent there, and therefore allow a mapping to the class.
 
 # Installation
 This package can be installed with pip, for instance:
 ```bash
 pip3 --user install perf-class
 ```
```

### Comparing `perf-class-1.0.4/perf_class/perf_class.py` & `perf-class-1.0.5/perf_class/perf_class.py`

 * *Files identical despite different names*

### Comparing `perf-class-1.0.4/perf_class.egg-info/PKG-INFO` & `perf-class-1.0.5/perf_class.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: perf-class
-Version: 1.0.4
-Summary: A tool to map perf script events to classes of events using a set of regex
+Version: 1.0.5
+Summary: A tool to mep perf script events to classes of events using regex
 Home-page: https://github.com/tbarbette/perf-class
 Author: Tom Barbette
 Author-email: t.barbette@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # perf-class
 
-This program allows to group the CPU time spent in functions as outputed by perf script into classes. Eg. if your application spend 3% of time in "sort\_down", 5% "sort\_up", 4% "sort\_final", and you give a map like "sort: Sorting", this tool will summarize those as "Sorting 12%".
+This program allows to group the CPU time spent in functions as outputed by perf script into classes. Eg. if your application spend 3% of time in "sort_down", 5% "sort_up", 4% "sort_final", and you give a map like "sort: Sorting", this tool will summarize those as "Sorting 12%".
 
-This program is intended as a post-processor to show where, roughly, a CPU spends its time in various part of an application. The result such as "Sorting : 12%, Computing : 23%" can be given to a pie chart, typically.
+This program is intended as a preprocessor to show where, roughly, a CPU spend its time in various application. The result such as "Sorting : 12%, Computing : 23%" can be given to a pie chart, typically.
 
-The map file, to describe the mapping, is simply a series of "regex : class", one by line. Each symbol will be matched against the regex, and upon match will be considered of the given class. The tool will start with the top of the stack trace, and if no match is found, re-try with the previous function in the stack, etc. This is needed for cases where a lot of time is spent in a generic function like the Linux kernel "raw\_spin\_lock" functions, that cannot be clearly tied to a specific event. However the calling function, or one before can be clearly mapped to a "class" of event. This is why in our case we could not simply use the output of perf top, as it does not make much sense, and there are hundred "top" functions that cannot be mapped to classes manually.
-Only the calling functions of those generic hit points will allow to find the reason of the time spent there, and therefore enables mapping of the class.
+The map file, to describe the mapping, is simply a series of "regex : class", one by line. Each symbol will be matched against the regex, and upon match will be considered of the given class. The tool will start with the top of the stack trace, and if no match is found, re-try with the previous function in the stack, etc. This is needed, and explain why a simple script was not sufficient to achieve the purpose of this script as a lot of time spend in the kernel is in "raw_spin_lock" functions.
+Only the calling functions of those generic hit points will allow to find the reason of the time spent there, and therefore allow a mapping to the class.
 
 # Installation
 This package can be installed with pip, for instance:
 ```bash
 pip3 --user install perf-class
 ```
 
@@ -105,9 +103,7 @@
 read_tsc 0.005070
 rcu_all_qs 0.005068
 __softirqentry_text_start 0.005063
 lapic_next_deadline 0.005061
 ```
 
 See perf-class --help for other options
-
-
```

### Comparing `perf-class-1.0.4/setup.py` & `perf-class-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="perf-class",
-    version="1.0.4",
+    version="1.0.5",
     author="Tom Barbette",
     author_email="t.barbette@gmail.com",
-    description="A tool to map perf script events to classes of events using a set of regex",
+    description="A tool to mep perf script events to classes of events using regex",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tbarbette/perf-class",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

