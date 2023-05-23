# Comparing `tmp/miniwdl_lsf-0.1.0.tar.gz` & `tmp/miniwdl_lsf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniwdl_lsf-0.1.0.tar", max compression
+gzip compressed data, was "miniwdl_lsf-0.1.1.tar", max compression
```

## Comparing `miniwdl_lsf-0.1.0.tar` & `miniwdl_lsf-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1057 2023-02-03 13:39:11.291202 miniwdl_lsf-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     2571 2023-04-14 13:07:58.403256 miniwdl_lsf-0.1.0/README.md
--rw-r--r--   0        0        0      686 2023-04-14 13:24:58.887105 miniwdl_lsf-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     5378 2023-04-11 20:40:50.318021 miniwdl_lsf-0.1.0/src/miniwdl_lsf/__init__.py
--rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 miniwdl_lsf-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1057 2023-02-03 13:39:11.291202 miniwdl_lsf-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     2571 2023-04-14 13:07:58.403256 miniwdl_lsf-0.1.1/README.md
+-rw-r--r--   0        0        0      804 2023-05-23 14:25:39.556671 miniwdl_lsf-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     5527 2023-05-23 14:25:39.557173 miniwdl_lsf-0.1.1/src/miniwdl_lsf/__init__.py
+-rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 miniwdl_lsf-0.1.1/PKG-INFO
```

### Comparing `miniwdl_lsf-0.1.0/LICENSE` & `miniwdl_lsf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miniwdl_lsf-0.1.0/README.md` & `miniwdl_lsf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `miniwdl_lsf-0.1.0/pyproject.toml` & `miniwdl_lsf-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "miniwdl-lsf"
-version = "0.1.0"
+version = "0.1.1"
 description = "miniwdl lsf backend using singularity"
 authors = ["Andrew Thrasher <adthrasher@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/adthrasher/miniwdl-lsf/"
+documentation = "https://adthrasher.github.io/miniwdl-lsf/"
 packages = [{include = "miniwdl_lsf", from = "src"}]
 keywords = ["WDL", "miniwdl", "workflow language", "LSF", "Singularity"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Topic :: System :: Distributed Computing"
 ]
```

### Comparing `miniwdl_lsf-0.1.0/src/miniwdl_lsf/__init__.py` & `miniwdl_lsf-0.1.1/src/miniwdl_lsf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,34 +84,35 @@
         bsub_args = [
             "bsub",
             "-K",
             "-J", self.run_id,
         ]
 
         # Redirect LSF logs to files
-        bsub_args.extend(["-o", os.path.join(self.host_dir, "stdout.lsf")])
-        bsub_args.extend(["-e", os.path.join(self.host_dir, "stderr.lsf")])
+        bsub_args.extend(["-o", os.path.join(self.host_dir, f"stdout{self.try_counter if self.try_counter > 1 else ''}.lsf")])
+        bsub_args.extend(["-e", os.path.join(self.host_dir, f"stderr{self.try_counter if self.try_counter > 1 else ''}.lsf")])
 
         cpu = self.runtime_values.get("cpu", None)
         if cpu is not None:
             bsub_args.extend(["-n", str(cpu)])
             bsub_args.extend(["-R span[hosts=1]"])
 
-        memory = self.runtime_values.get("memory_reservation", None)
+        # Get memory reservation for job in bytes
+        memory = self.runtime_values.get("memory_reservation", 0)
         if memory is not None:
             # LSF memory specifications are per-core.
             # WDL (bioinformatics) tasks often specify memory per job.
             # This option divides the memory by the number of cores
             # prior to submission to LSF.
             memory_divisor = 1
             if self.cfg["lsf"].get_bool("memory_per_job") and cpu is not None:
                memory_divisor = cpu
             
             # Round to the nearest megabyte.
-            bsub_args.extend(["-M", f"{round((memory / (1024 ** 2)) / memory_divisor)}M"])
+            bsub_args.extend(["-M", f"{round((memory / (1000 ** 2)) / memory_divisor)}M"])
 
         if self.cfg.has_section("lsf"):
             extra_args = self.cfg.get("lsf", "extra_args")
             if extra_args is not None:
                 bsub_args.extend(shlex.split(extra_args))
         return bsub_args
```

### Comparing `miniwdl_lsf-0.1.0/PKG-INFO` & `miniwdl_lsf-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: miniwdl-lsf
-Version: 0.1.0
+Version: 0.1.1
 Summary: miniwdl lsf backend using singularity
+Home-page: https://github.com/adthrasher/miniwdl-lsf/
 License: MIT
 Keywords: WDL,miniwdl,workflow language,LSF,Singularity
 Author: Andrew Thrasher
 Author-email: adthrasher@gmail.com
 Requires-Python: >3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: miniwdl (>=1.7.0)
+Project-URL: Documentation, https://adthrasher.github.io/miniwdl-lsf/
+Project-URL: Repository, https://github.com/adthrasher/miniwdl-lsf/
 Description-Content-Type: text/markdown
 
 miniwdl-lsf
 =============
 Extends miniwdl to run workflows on LSF clusters in singularity containers.
 
 This [LSF backend](https://miniwdl.readthedocs.io/en/latest/runner_backends.html) plugin for
```

