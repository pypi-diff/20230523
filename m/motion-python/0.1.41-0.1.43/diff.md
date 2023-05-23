# Comparing `tmp/motion_python-0.1.41.tar.gz` & `tmp/motion_python-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.41.tar", max compression
+gzip compressed data, was "motion_python-0.1.43.tar", max compression
```

## Comparing `motion_python-0.1.41.tar` & `motion_python-0.1.43.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2752 2023-05-14 23:33:39.859564 motion_python-0.1.41/README.md
--rw-r--r--   0        0        0      187 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/__init__.py
--rw-r--r--   0        0        0     1818 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/cli.py
--rw-r--r--   0        0        0    20577 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/component.py
--rw-r--r--   0        0        0     5733 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/execute.py
--rw-r--r--   0        0        0     6823 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/route.py
--rw-r--r--   0        0        0     3734 2023-05-14 23:33:39.863563 motion_python-0.1.41/motion/utils.py
--rw-r--r--   0        0        0     1657 2023-05-14 23:33:59.775864 motion_python-0.1.41/pyproject.toml
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 motion_python-0.1.41/PKG-INFO
+-rw-r--r--   0        0        0     2752 2023-05-23 16:50:57.023610 motion_python-0.1.43/README.md
+-rw-r--r--   0        0        0      187 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/cli.py
+-rw-r--r--   0        0        0    20577 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/component.py
+-rw-r--r--   0        0        0     5733 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/execute.py
+-rw-r--r--   0        0        0     6823 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/route.py
+-rw-r--r--   0        0        0     3734 2023-05-23 16:50:57.027610 motion_python-0.1.43/motion/utils.py
+-rw-r--r--   0        0        0     1657 2023-05-23 16:51:19.371545 motion_python-0.1.43/pyproject.toml
+-rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 motion_python-0.1.43/PKG-INFO
```

### Comparing `motion_python-0.1.41/README.md` & `motion_python-0.1.43/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/motion/cli.py` & `motion_python-0.1.43/motion/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,12 +64,12 @@
     # Dump the graph to a file with the date
     ts = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
     out_filename = f"{ts}_{instance}_{output}"
     checkmark = "\u2705"  # Unicode code point for checkmark emoji
 
     with open(out_filename, "w") as f:
         json.dump(graph, f, indent=4)
-        click.echo(f"{checkmark} Graph dumped to {out_filename}.")
+        click.echo(f"{checkmark} Graph dumped to {out_filename}")
 
 
 if __name__ == "__main__":
     motioncli()
```

### Comparing `motion_python-0.1.41/motion/component.py` & `motion_python-0.1.43/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/motion/execute.py` & `motion_python-0.1.43/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/motion/instance.py` & `motion_python-0.1.43/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.43/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/motion/route.py` & `motion_python-0.1.43/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/motion/utils.py` & `motion_python-0.1.43/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.41/pyproject.toml` & `motion_python-0.1.43/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.41"
+version = "0.1.43"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.41/PKG-INFO` & `motion_python-0.1.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.41
+Version: 0.1.43
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

