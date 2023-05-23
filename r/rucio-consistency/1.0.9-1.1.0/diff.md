# Comparing `tmp/rucio-consistency-1.0.9.tar.gz` & `tmp/rucio-consistency-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.9.tar", last modified: Thu Apr 13 19:15:48 2023, max compression
+gzip compressed data, was "rucio-consistency-1.1.0.tar", last modified: Tue May 23 17:50:56 2023, max compression
```

## Comparing `rucio-consistency-1.0.9.tar` & `rucio-consistency-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.561073 rucio-consistency-1.0.9/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.9/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 19:15:48.560642 rucio-consistency-1.0.9/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.9/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.554672 rucio-consistency-1.0.9/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.0.9/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.559180 rucio-consistency-1.0.9/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.9/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 19:15:45.000000 rucio-consistency-1.0.9/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.560263 rucio-consistency-1.0.9/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27445 2023-04-13 19:14:40.000000 rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.557038 rucio-consistency-1.0.9/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 19:15:48.561190 rucio-consistency-1.0.9/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.9/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.120522 rucio-consistency-1.1.0/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.1.0/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-05-23 17:50:56.120147 rucio-consistency-1.1.0/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)    12399 2023-05-19 14:17:54.000000 rucio-consistency-1.1.0/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.113993 rucio-consistency-1.1.0/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4635 2023-04-21 14:37:25.000000 rucio-consistency-1.1.0/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.1.0/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     5417 2023-04-21 14:37:27.000000 rucio-consistency-1.1.0/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.118488 rucio-consistency-1.1.0/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3532 2023-04-13 22:36:38.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3596 2023-04-13 22:34:51.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4317 2023-04-13 22:36:42.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    10323 2023-05-23 15:56:13.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.1.0/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.1.0/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-05-23 17:49:31.000000 rucio-consistency-1.1.0/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.119561 rucio-consistency-1.1.0/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.1.0/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27445 2023-04-13 19:31:22.000000 rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-23 17:50:56.116348 rucio-consistency-1.1.0/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      850 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      388 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-05-23 17:50:56.000000 rucio-consistency-1.1.0/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-05-23 17:50:56.120624 rucio-consistency-1.1.0/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.1.0/setup.py
```

### Comparing `rucio-consistency-1.0.9/LICENSE` & `rucio-consistency-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/rucio_consistency/config.py` & `rucio-consistency-1.1.0/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.1.0/rucio_consistency/scripts/cmp2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import sys, glob, time, os
 
 from rucio_consistency import PartitionedList, Stats
 
 Version = "1.0"
 
 Usage = """
-python cmp2.py [-z] [-s <stats file> [-S <stats key>]]    (join|minus|xor|or) <A prefix> <B prefix> <output prefix>
-python cmp2.py [-z] [-s <stats file> [-S <stats key>]] -f (join|minus|xor|or) <A file> <B file> <output file>
+%(cmd)s [-z] [-s <stats file> [-S <stats key>]]    (join|minus|xor|or) <A prefix> <B prefix> <output prefix>
+%(cmd)s [-z] [-s <stats file> [-S <stats key>]] -f (join|minus|xor|or) <A file> <B file> <output file>
 """
 
 def main():
     import getopt
 
     t0 = time.time()
 
     opts, args = getopt.getopt(sys.argv[1:], "s:S:zf")
     opts = dict(opts)
     
 
 
     if len(args) < 4:
-            print (Usage)
-            sys.exit(2)
+        cmd = sys.argv[0].rsplit("/", 1)[-1]
+        if cmd.endswith(".py"):
+            cmd = "python " + cmd
+        print(Usage % {"cmd":cmd})
+        sys.exit(2)
 
     stats_file = opts.get("-s")
     stats_key = opts.get("-S", "join")
     compress = "-z" in opts
     single_file = "-f" in opts
 
     my_stats = stats = None
```

### Comparing `rucio-consistency-1.0.9/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.1.0/rucio_consistency/scripts/cmp3.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
         if len(args) < 5:
             cmd = sys.argv[0].rsplit("/", 1)[-1]
             if cmd.endswith(".py"):
                 cmd = "python " + cmd
             print(Usage % (cmd,))
             sys.exit(2)
+
         compress = "-z" in opts
         stats_file = opts.get("-s")
         stats_key = opts.get("-S", "cmp3")
         stats = Stats(stats_file) if stats_file else None
 
         b_prefix, r_prefix, a_prefix, out_dark, out_missing = args
```

### Comparing `rucio-consistency-1.0.9/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.1.0/rucio_consistency/scripts/cmp5.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         opts = dict(opts)
 
         if len(args) < 5:
             cmd = sys.argv[0].rsplit("/", 1)[-1]
             if cmd.endswith(".py"):
                 cmd = "python " + cmd
             print(Usage % (cmd,))
-        sys.exit(2)
+            sys.exit(2)
+
         compress = "-z" in opts
         stats_file = opts.get("-s")
         stats_key = opts.get("-S", "cmp3")
         if stats_file:
             stats = Stats(stats_file) if stats_file else None
 
         b_m_prefix, b_d_prefix, r_prefix, a_m_prefix, a_d_prefix, out_dark, out_missing = args
```

### Comparing `rucio-consistency-1.0.9/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.1.0/rucio_consistency/scripts/db_dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sqlalchemy.exc import ArgumentError
 
 from rucio_consistency import PartitionedList, DBConfig, CEConfiguration, Stats
 
 Version = "2.0"
 
 Usage = """
-python db_dump.py [options] -c <config.yaml> <rse_name>
+%(cmd)s [options] -c <config.yaml> <rse_name>
     -c <config file> -- required
     -d <db config file> -- required - uses rucio.cfg format. Must contain "default" and "schema" under [databse]
     -v -- verbose
     -n <nparts>
     -f <state>:<prefix> -- filter files with given state to the files set with prefix
         state can be either combination of capital letters or "*" 
         can be repeated  ( -f A:/path1 -f CD:/path2 )
@@ -106,16 +106,19 @@
             states, prefix = val.split(':')
             filters[states] = prefix
             all_states |= set(states)
 
     opts = dict(opts)
 
     if not args or (not "-c" in opts and not "-d" in opts):
-            print (Usage)
-            sys.exit(2)
+        cmd = sys.argv[0].rsplit("/", 1)[-1]
+        if cmd.endswith(".py"):
+            cmd = "python " + cmd
+        print(Usage % {"cmd":cmd})
+        sys.exit(2)
 
     verbose = "-v" in opts
     long_output = "-l" in opts
     out_prefix = opts.get("-o")
     zout = "-z" in opts
     stats_file = opts.get("-s")
     stats_key = opts.get("-S", "db_dump")
@@ -212,15 +215,15 @@
 
         if all_replicas:
                 sys.stderr.write("including all replias\n")
         else:            
                 print("including replicas in states:", list(all_states), file=sys.stderr)
                 replicas = replicas.filter(Replica.state.in_(list(all_states)))
         dirs = set()
-        n = 0
+        ntotal = 0
         filter_re = None    #config.dbdump_param(rse, "filter")
         ignored_files = 0
         if filter_re:
             filter_re = re.compile(filter_re)
         root_file_counts = {root: 0 for root in config.RootList}
         for r in replicas:
             path = r.name
@@ -233,42 +236,46 @@
                 if not filter_re.search(path):
                     continue
             
             if any(path.startswith(ignore_prefix) for ignore_prefix in ignore_list):
                 ignored_files += 1
                 continue
 
-            for r, n in list(root_file_counts.items()):
-                prefix = r + '/' if not r.endswith('/') else r
+            matched_root = None
+
+            for root, root_count in list(root_file_counts.items()):
+                prefix = root + '/' if not root.endswith('/') else root
                 if path.startswith(prefix):
-                    root_file_counts[r] = n + 1
+                    root_file_counts[root] = root_count + 1
+                    matched_root = root
                     break
 
+            if not matched_root:
+                continue                # not under any root
+
             words = path.rsplit("/", 1)
             if len(words) == 1:
                     dirp = "/"
             else:
                     dirp = words[0]
             dirs.add(dirp)
 
             for s, out_list in outputs.items():
                 if state in s or s == '*':
                     if long_output:
                         out_list.add("%s\t%s\t%s\t%s\t%s" % (rse_name, r.scope, r.name, path or "null", r.state))
                     else:
                         out_list.add(path or "null")
-            n += 1
-            if n % batch == 0:
-                    print(n)
-            if stop_after is not None and n >= stop_after:
+            ntotal += 1
+            if stop_after is not None and ntotal >= stop_after:
                 print(f"stopped after {stop_after} files", file=sys.stderr)
                 break
         for out_list in outputs.values():
             out_list.close()
-        sys.stderr.write("Found %d files in %d directories\n" % (n, len(dirs)))
+        sys.stderr.write("Found %d files in %d directories\n" % (ntotal, len(dirs)))
         t1 = time.time()
         t = int(t1 - t0)
         s = t % 60
         m = t // 60
         sys.stderr.write("Elapsed time: %dm%02ds\n" % (m, s))
     except:
         lines = traceback.format_exc().split("\n")
@@ -282,15 +289,15 @@
             })
         raise
     else:    
         if stats is not None:
             stats.update_section(stats_key, {
                 "status":"done",
                 "end_time":t1,
-                "files":n,
+                "files":ntotal,
                 "ignored_files":ignored_files,
                 "elapsed":t1-t0,
                 "directories":len(dirs),
                 "ignore_list":ignore_list
             })
         if root_file_counts_out is not None:
             root_file_counts_out.write(json.dumps(root_file_counts, indent=4, sort_keys=True))
```

### Comparing `rucio-consistency-1.0.9/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.1.0/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.1.0/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/rucio_consistency/stats.py` & `rucio-consistency-1.1.0/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.1.0/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pythreader import TaskQueue, Task, DEQueue, PyThread, synchronized, ShellCommand, Primitive
 import re, json, os, os.path, traceback, sys
 import subprocess, time, random, gzip
 
 from rucio_consistency import to_str, Stats, PartitionedList, ScannerConfiguration
 from .xrootd_client import XRootDClient
 
-Version = "3.1"
+Version = "4.0"
 
 GB = 1024*1024*1024
 
 try:
     import tqdm
     Use_tqdm = True
 except:
```

### Comparing `rucio-consistency-1.0.9/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.1.0/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.9/setup.py` & `rucio-consistency-1.1.0/setup.py`

 * *Files identical despite different names*

