# Comparing `tmp/cicsim-0.1.2.tar.gz` & `tmp/cicsim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicsim-0.1.2.tar", last modified: Tue May 23 16:41:04 2023, max compression
+gzip compressed data, was "cicsim-0.1.3.tar", last modified: Tue May 23 17:11:51 2023, max compression
```

## Comparing `cicsim-0.1.2.tar` & `cicsim-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-23 16:41:04.962774 cicsim-0.1.2/
--rw-r--r--   0 wulff      (502) staff       (20)     2961 2023-05-23 16:41:04.962516 cicsim-0.1.2/PKG-INFO
--rw-r--r--   0 wulff      (502) staff       (20)     2416 2023-01-22 20:55:26.000000 cicsim-0.1.2/README.md
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-23 16:41:04.960497 cicsim-0.1.2/cicsim/
--rw-r--r--   0 wulff      (502) staff       (20)      419 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)     6800 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cdsconf.py
--rw-r--r--   0 wulff      (502) staff       (20)     4837 2023-03-02 10:27:23.000000 cicsim-0.1.2/cicsim/cicsim.py
--rw-r--r--   0 wulff      (502) staff       (20)     5261 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cmdip.py
--rw-r--r--   0 wulff      (502) staff       (20)     7640 2023-02-10 08:58:13.000000 cicsim-0.1.2/cicsim/cmdresults.py
--rw-r--r--   0 wulff      (502) staff       (20)     7658 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cmdrun.py
--rw-r--r--   0 wulff      (502) staff       (20)    12773 2023-04-21 12:36:15.000000 cicsim-0.1.2/cicsim/cmdrunng.py
--rw-r--r--   0 wulff      (502) staff       (20)     6012 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cmdsimdir.py
--rw-r--r--   0 wulff      (502) staff       (20)     5852 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cmdsimdirng.py
--rw-r--r--   0 wulff      (502) staff       (20)     4407 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cmdspider.py
--rw-r--r--   0 wulff      (502) staff       (20)     4503 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/cmdsummary.py
--rw-r--r--   0 wulff      (502) staff       (20)     3130 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/command.py
--rw-r--r--   0 wulff      (502) staff       (20)     3424 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/ngraw.py
--rw-r--r--   0 wulff      (502) staff       (20)     2089 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/plot.py
--rw-r--r--   0 wulff      (502) staff       (20)     3763 2023-05-01 13:58:23.000000 cicsim-0.1.2/cicsim/simcalc.py
--rw-r--r--   0 wulff      (502) staff       (20)     4208 2023-02-10 09:05:33.000000 cicsim-0.1.2/cicsim/spec.py
--rw-r--r--   0 wulff      (502) staff       (20)     2984 2023-01-22 20:55:26.000000 cicsim-0.1.2/cicsim/spiceparser.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-23 16:41:04.962195 cicsim-0.1.2/cicsim.egg-info/
--rw-r--r--   0 wulff      (502) staff       (20)     2961 2023-05-23 16:41:04.000000 cicsim-0.1.2/cicsim.egg-info/PKG-INFO
--rw-r--r--   0 wulff      (502) staff       (20)      529 2023-05-23 16:41:04.000000 cicsim-0.1.2/cicsim.egg-info/SOURCES.txt
--rw-r--r--   0 wulff      (502) staff       (20)        1 2023-05-23 16:41:04.000000 cicsim-0.1.2/cicsim.egg-info/dependency_links.txt
--rw-r--r--   0 wulff      (502) staff       (20)       45 2023-05-23 16:41:04.000000 cicsim-0.1.2/cicsim.egg-info/entry_points.txt
--rw-r--r--   0 wulff      (502) staff       (20)       36 2023-05-23 16:41:04.000000 cicsim-0.1.2/cicsim.egg-info/requires.txt
--rw-r--r--   0 wulff      (502) staff       (20)        7 2023-05-23 16:41:04.000000 cicsim-0.1.2/cicsim.egg-info/top_level.txt
--rw-r--r--   0 wulff      (502) staff       (20)      573 2023-05-23 16:40:54.000000 cicsim-0.1.2/pyproject.toml
--rw-r--r--   0 wulff      (502) staff       (20)       38 2023-05-23 16:41:04.962872 cicsim-0.1.2/setup.cfg
--rw-r--r--   0 wulff      (502) staff       (20)     1147 2023-01-22 20:55:26.000000 cicsim-0.1.2/setup.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-23 17:11:51.462410 cicsim-0.1.3/
+-rw-r--r--   0 wulff      (502) staff       (20)     2535 2023-05-23 17:11:51.462168 cicsim-0.1.3/PKG-INFO
+-rw-r--r--   0 wulff      (502) staff       (20)     1990 2023-05-23 17:11:23.000000 cicsim-0.1.3/README.md
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-23 17:11:51.460152 cicsim-0.1.3/cicsim/
+-rw-r--r--   0 wulff      (502) staff       (20)      419 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)     6800 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cdsconf.py
+-rw-r--r--   0 wulff      (502) staff       (20)     4837 2023-03-02 10:27:23.000000 cicsim-0.1.3/cicsim/cicsim.py
+-rw-r--r--   0 wulff      (502) staff       (20)     5261 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cmdip.py
+-rw-r--r--   0 wulff      (502) staff       (20)     7640 2023-02-10 08:58:13.000000 cicsim-0.1.3/cicsim/cmdresults.py
+-rw-r--r--   0 wulff      (502) staff       (20)     7658 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cmdrun.py
+-rw-r--r--   0 wulff      (502) staff       (20)    12773 2023-04-21 12:36:15.000000 cicsim-0.1.3/cicsim/cmdrunng.py
+-rw-r--r--   0 wulff      (502) staff       (20)     6012 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cmdsimdir.py
+-rw-r--r--   0 wulff      (502) staff       (20)     5852 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cmdsimdirng.py
+-rw-r--r--   0 wulff      (502) staff       (20)     4407 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cmdspider.py
+-rw-r--r--   0 wulff      (502) staff       (20)     4503 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/cmdsummary.py
+-rw-r--r--   0 wulff      (502) staff       (20)     3130 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/command.py
+-rw-r--r--   0 wulff      (502) staff       (20)     3424 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/ngraw.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2089 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/plot.py
+-rw-r--r--   0 wulff      (502) staff       (20)     3763 2023-05-01 13:58:23.000000 cicsim-0.1.3/cicsim/simcalc.py
+-rw-r--r--   0 wulff      (502) staff       (20)     4208 2023-02-10 09:05:33.000000 cicsim-0.1.3/cicsim/spec.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2984 2023-01-22 20:55:26.000000 cicsim-0.1.3/cicsim/spiceparser.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-23 17:11:51.461847 cicsim-0.1.3/cicsim.egg-info/
+-rw-r--r--   0 wulff      (502) staff       (20)     2535 2023-05-23 17:11:51.000000 cicsim-0.1.3/cicsim.egg-info/PKG-INFO
+-rw-r--r--   0 wulff      (502) staff       (20)      529 2023-05-23 17:11:51.000000 cicsim-0.1.3/cicsim.egg-info/SOURCES.txt
+-rw-r--r--   0 wulff      (502) staff       (20)        1 2023-05-23 17:11:51.000000 cicsim-0.1.3/cicsim.egg-info/dependency_links.txt
+-rw-r--r--   0 wulff      (502) staff       (20)       45 2023-05-23 17:11:51.000000 cicsim-0.1.3/cicsim.egg-info/entry_points.txt
+-rw-r--r--   0 wulff      (502) staff       (20)       36 2023-05-23 17:11:51.000000 cicsim-0.1.3/cicsim.egg-info/requires.txt
+-rw-r--r--   0 wulff      (502) staff       (20)        7 2023-05-23 17:11:51.000000 cicsim-0.1.3/cicsim.egg-info/top_level.txt
+-rw-r--r--   0 wulff      (502) staff       (20)      573 2023-05-23 17:07:24.000000 cicsim-0.1.3/pyproject.toml
+-rw-r--r--   0 wulff      (502) staff       (20)       38 2023-05-23 17:11:51.462486 cicsim-0.1.3/setup.cfg
+-rw-r--r--   0 wulff      (502) staff       (20)     1126 2023-05-23 17:07:31.000000 cicsim-0.1.3/setup.py
```

### Comparing `cicsim-0.1.2/README.md` & `cicsim-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,63 @@
 
 # Custom IC Creator Simulation Tools
 
-
 [![tests](https://github.com/wulffern/cicsim/actions/workflows/main.yml/badge.svg)](https://github.com/wulffern/cicsim/actions/workflows/main.yml)
 
 # Caution
 If you're looking for the cicsim that controlled spectre, then look in the
 cadence branch. From 2022-10-14 I decided to go all in on open source tools like
-ngspice, and thus discontinued support for spectre
+ngspice, and thus discontinued support for spectre.
 
 # Why
 This is a script package I use to control ngspice, it can
 - Run corner simulations
-- Create IPs (used in wulffern/aicex)
+- Create IPs (used in  [wulffern/aicex](https://github.com/wulffern/aicex) )
 - Create simulation directories
 
 # Changelog
 
 | Version | Status                      | Comment                 |
 |:--------|:----------------------------|:------------------------|
-| 0.0.3   | All in on open source tools |                         |
-| 0.0.2   | to be released              | Probably bugfixes       |
 | 0.0.1   | :white_check_mark:          | First version of cicsim |
+| 0.0.3   | All in on open source tools |                         |
+| 0.1.2   | First version on pipy      |                         |
 
 # Install this module
 If you want to follow the latest and greatest
 ``` sh
-mkdir pro
-cd pro
 git clone https://github.com/wulffern/cicsim
 cd cicsim
-python3 -m pip install -r requirements.txt --user
-python3 -m pip install --no-deps -e . --user
+python3 -m pip install --user -e . 
+```
+
+If you want the latest stable
+
+``` bash
+python3 -m pip install cicpy
 ```
+
 # Get started with simulation
-Head over to [wulffern/aicex](https://github.com/wulffern/aicex) to see how it works
+Head over to [Open source analog integrated circuit flow on Skywater
+130nm](https://analogicus.com/rply_ex0_sky130nm/tutorial) to see cicsim in action.
 
 # Commands
 
 ``` 
 Usage: cicsim [OPTIONS] COMMAND [ARGS]...
 
   Custom IC Creator Simulator Tools
 
-  This package provides helper scripts for simulating integrated circuits in
-  ngspice
+  This package provides helper scripts for simulating integrated circuits
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  run      Run a simulation of TESTBENCH
-  simcell  Create a simulation directory for a cell
+  ip           make ip from a YAML template file
+  plot         Plot from rawfile
+  portreplace  Replace ${PORTS} and ${VPORTS} with the subcircuit ports...
+  results      Results of single runfile
+  run          Run a ngspice simulation of TESTBENCH
+  simcell      Create a ngspice simulation directory for a Cell
+  summary      Generate simulation summary for results
 ```
-
-## Know what python you're running
-
-Python is great, however, python exists in many different versions, and you can
-never trust that the right version is installed on the system that you're going
-to use. As such, always know what you're running.
-
-### Option 1: Build yourself
-If you don't control the system, then you can still install locally
-https://randomwalk.in/python/2019/10/27/Install-Python-copy.html
-
-It's not straightforward though, and it can be a rabbit hole that takes some
-time
-
-### Option 2: Check version
-Try 
-
-  python3 --version
-
-Or
-
-  python --version 
-
-### Option 3: Set version
-Sometimes multiple versions can be installed, if so, then you can add the
-following lines to your .bashrc file
-  
-  alias python3='/usr/local/bin/python3.8'
-  alias pip3='/usr/local/bin/pip3.8'
```

### Comparing `cicsim-0.1.2/cicsim/cdsconf.py` & `cicsim-0.1.3/cicsim/cdsconf.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cicsim.py` & `cicsim-0.1.3/cicsim/cicsim.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdip.py` & `cicsim-0.1.3/cicsim/cmdip.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdresults.py` & `cicsim-0.1.3/cicsim/cmdresults.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdrun.py` & `cicsim-0.1.3/cicsim/cmdrun.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdrunng.py` & `cicsim-0.1.3/cicsim/cmdrunng.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdsimdir.py` & `cicsim-0.1.3/cicsim/cmdsimdir.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdsimdirng.py` & `cicsim-0.1.3/cicsim/cmdsimdirng.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdspider.py` & `cicsim-0.1.3/cicsim/cmdspider.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/cmdsummary.py` & `cicsim-0.1.3/cicsim/cmdsummary.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/command.py` & `cicsim-0.1.3/cicsim/command.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/ngraw.py` & `cicsim-0.1.3/cicsim/ngraw.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/plot.py` & `cicsim-0.1.3/cicsim/plot.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/simcalc.py` & `cicsim-0.1.3/cicsim/simcalc.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/spec.py` & `cicsim-0.1.3/cicsim/spec.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim/spiceparser.py` & `cicsim-0.1.3/cicsim/spiceparser.py`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/cicsim.egg-info/SOURCES.txt` & `cicsim-0.1.3/cicsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cicsim-0.1.2/pyproject.toml` & `cicsim-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cicsim"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Carsten Wulff", email="carsten@wulff.no" },
 ]
 description = "Custom IC Creator Simulation Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cicsim-0.1.2/setup.py` & `cicsim-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicsim",
-    version="0.1.1",
     author="Carsten Wulff",
     author_email="carsten@wulff.no",
     description="Custom IC Creator Simulation Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wulffern/cicsim",
     packages=setuptools.find_packages(),
```

