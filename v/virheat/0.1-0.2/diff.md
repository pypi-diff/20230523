# Comparing `tmp/virheat-0.1.tar.gz` & `tmp/virheat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virheat-0.1.tar", last modified: Mon May 22 14:05:25 2023, max compression
+gzip compressed data, was "virheat-0.2.tar", last modified: Tue May 23 14:27:02 2023, max compression
```

## Comparing `virheat-0.1.tar` & `virheat-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:05:25.277989 virheat-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-22 14:05:25.277989 virheat-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-22 14:05:08.000000 virheat-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:05:25.277989 virheat-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 14:05:08.000000 virheat-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:05:25.273989 virheat-0.1/virheat/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 14:05:08.000000 virheat-0.1/virheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 14:05:08.000000 virheat-0.1/virheat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-22 14:05:08.000000 virheat-0.1/virheat/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:05:25.277989 virheat-0.1/virheat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:05:08.000000 virheat-0.1/virheat/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-22 14:05:08.000000 virheat-0.1/virheat/scripts/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-22 14:05:08.000000 virheat-0.1/virheat/scripts/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:05:25.277989 virheat-0.1/virheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 14:05:25.000000 virheat-0.1/virheat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-23 14:27:02.112931 virheat-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-23 14:26:44.000000 virheat-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:27:02.112931 virheat-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-23 14:26:44.000000 virheat-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/virheat/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 14:26:44.000000 virheat-0.2/virheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 14:26:44.000000 virheat-0.2/virheat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-23 14:26:44.000000 virheat-0.2/virheat/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/virheat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:26:44.000000 virheat-0.2/virheat/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-23 14:26:44.000000 virheat-0.2/virheat/scripts/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-23 14:26:44.000000 virheat-0.2/virheat/scripts/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:27:02.112931 virheat-0.2/virheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:27:01.000000 virheat-0.2/virheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:27:02.000000 virheat-0.2/virheat.egg-info/top_level.txt
```

### Comparing `virheat-0.1/PKG-INFO` & `virheat-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: virheat
-Version: 0.1
+Version: 0.2
 Summary: virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.
 Home-page: https://github.com/jonas-fuchs/virHEAT
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-<img src="https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png" alt="virHEAT logo" />
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/virheat/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/virheat)
+[![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
+[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
+[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
+[![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+
+[![Logo](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)
+
 
 
 **virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
 
 
 
 Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
 
 ## SARS-CoV-2 example:
 
-<img src="https://github.com/jonas-fuchs/virHEAT/blob/master/example.png" alt="example plot" />
-
+[![Example](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)
 
 ## Installation
 
 ### via pip (recommened):
 ```shell
 pip install virheat
 ```
```

### Comparing `virheat-0.1/README.md` & `virheat-0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-<img src="https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png" alt="virHEAT logo" />
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/virheat/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/virheat)
+[![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
+[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
+[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
+[![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+
+[![Logo](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)
+
 
 
 **virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
 
 
 
 Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
 
 ## SARS-CoV-2 example:
 
-<img src="https://github.com/jonas-fuchs/virHEAT/blob/master/example.png" alt="example plot" />
-
+[![Example](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)
 
 ## Installation
 
 ### via pip (recommened):
 ```shell
 pip install virheat
 ```
```

### Comparing `virheat-0.1/setup.py` & `virheat-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     version=__version__,
     python_requires=">=3.9",
     license_files=('LICENSE'),
     packages=find_packages(),
     install_requires=[
         "matplotlib>=3.5.1",
         "numpy>=1.23.3",
-        "vcfpy>=0.13.6"
     ],
     description='virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.',
     url='https://github.com/jonas-fuchs/virHEAT',
     author='Dr. Jonas Fuchs',
     author_email='jonas.fuchs@uniklinik-freiburg.de',
     classifiers=[
         "Programming Language :: Python :: 3.9",
```

### Comparing `virheat-0.1/virheat/command.py` & `virheat-0.2/virheat/command.py`

 * *Files identical despite different names*

### Comparing `virheat-0.1/virheat/scripts/data_prep.py` & `virheat-0.2/virheat/scripts/data_prep.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # BUILT-INS
 import os
 import re
 import pathlib
 
 # LIBS
 import numpy as np
-import vcfpy as vcf
 
 
 def get_vcf_files(path):
     """
     returns a list of vcf files in a paticular folder
     """
     return list(pathlib.Path(path).glob('*.vcf'))
@@ -29,40 +28,106 @@
         alpha = re.sub(r'\d+', '', filename)
     else:
         digit = ''
         alpha = filename
     return (alpha, int(digit) if digit else float('inf'))
 
 
+def convert_string(string):
+    """
+    converts string to its right type
+    """
+    string = string.replace("\n", "")
+    if string.isdecimal():
+        return(int(string))
+    elif string.replace('.', '', 1).isdecimal():
+        return(float(string))
+    else:
+        return string
+
+
+def read_vcf(vcf_file):
+    """
+    parse vcf files to dictionary
+    """
+    vcf_dict = {}
+
+    # get header and values
+    with open(vcf_file, "r") as f:
+        header = [l.split("\t") for l in f if l.startswith('#CHROM')][0]
+    # get each line as frequency_lists
+    with open(vcf_file, "r") as f:
+        lines = [l.split("\t") for l in f if not l.startswith('#')]
+    # check if vcf is empty
+    if not lines:
+        print(f"WARNING: {vcf_file} is empty!")
+    # get standard headers as keys
+    for key in header[0:6]:
+        vcf_dict[key] = []
+    # functional effect
+    vcf_dict["TYPE"] = []
+    # info field
+    for line in lines:
+        for info in line[7].split(";"):
+            if "=" in info:
+                vcf_dict[info.split("=")[0]] = []
+    # fill in dictionary
+    for line in lines:
+        # remember keys that have an entry already
+        visited_keys = []
+        for idx, key in enumerate(header[0:6]):
+            vcf_dict[key].append(convert_string(line[idx]))
+        # get mutation type
+        if len(line[3]) == len(line[4]):
+            vcf_dict["TYPE"].append("SNV")
+        elif len(line[3]) < len(line[4]):
+            vcf_dict["TYPE"].append("INS")
+        elif len(line[3]) > len(line[4]):
+            vcf_dict["TYPE"].append("DEL")
+        visited_keys.extend(header[0:6])
+        visited_keys.append("TYPE")
+        # get data from info field
+        for info in line[7].split(";"):
+            if "=" in info:
+                key, val = info.split("=")
+                vcf_dict[key].append(convert_string(val))
+                visited_keys.append(key)
+        # append none for ech none vistited key
+        for key in [k for k in vcf_dict.keys() if k not in visited_keys]:
+            vcf_dict[key].append(None)
+
+    return vcf_dict
+
+
 def extract_vcf_data(vcf_files, threshold=0):
     """
     extract relevant vcf data
     """
 
     file_names = []
     frequency_lists = []
 
     for file in vcf_files:
         file_names.append(os.path.splitext(os.path.basename(file))[0])
-        vcf_reader = vcf.Reader.from_path(file)
+        vcf_dict = read_vcf(file)
         frequency_list = []
         # write all mutation info in a '_' sep string
-        for line in vcf_reader:
-            if not line.INFO["AF"] >= threshold:
+        for idx in range(0, len(vcf_dict["#CHROM"])):
+            if not vcf_dict["AF"][idx] >= threshold:
                 continue
             frequency_list.append(
-                (f"{line.POS}_{line.REF}_{[alt.value for alt in line.ALT][0]}_{[alt.type for alt in line.ALT][0]}", line.INFO["AF"])
+                (f"{vcf_dict['POS'][idx]}_{vcf_dict['REF'][idx]}_{vcf_dict['ALT'][idx]}_{vcf_dict['TYPE'][idx]}", vcf_dict['AF'][idx])
             )
         frequency_lists.append(frequency_list)
     # sort by mutation index
     unique_mutations = sorted(
         {x[0] for li in frequency_lists for x in li}, key=lambda x: int(x.split("_")[0])
     )
 
-    return line.CHROM, frequency_lists, unique_mutations, file_names
+    return vcf_dict["#CHROM"][0], frequency_lists, unique_mutations, file_names
 
 
 def create_freq_array(unique_mutations, frequency_lists):
     """
     create an np array of the mutation frequencies
     """
```

### Comparing `virheat-0.1/virheat/scripts/plotting.py` & `virheat-0.2/virheat/scripts/plotting.py`

 * *Files identical despite different names*

### Comparing `virheat-0.1/virheat.egg-info/PKG-INFO` & `virheat-0.2/virheat.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: virheat
-Version: 0.1
+Version: 0.2
 Summary: virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.
 Home-page: https://github.com/jonas-fuchs/virHEAT
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-<img src="https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png" alt="virHEAT logo" />
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/virheat/badge)](https://www.codefactor.io/repository/github/jonas-fuchs/virheat)
+[![DOI](https://zenodo.org/badge/639918477.svg)](https://zenodo.org/badge/latestdoi/639918477)
+[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
+[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/virheat)](https://www.gnu.org/licenses/gpl-3.0)
+[![pypi version](https://img.shields.io/pypi/v/virheat)](https://pypi.org/project/virheat/)
+
+[![Logo](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/virheat.png)
+
 
 
 **virHEAT is a tool to visualize vcfs as a heatmap and map mutations to respective genes.**
 
 
 
 Ever wanted to have a condensed look at variant frequencies after mapping your raw reads to a viral/bacterial reference genome and compare multiple vcf files at the same time? Than virHEAT is for you. You can not only visualize the heatmap but also read in a gff3 file that lets you display genes harboring a mutation. This lightweight script was inspired by [snipit](https://github.com/aineniamh/snipit) and my [variant frequency plot](https://github.com/jonas-fuchs/SARS-CoV-2-analyses/tree/main/Heatmap), getting the best visualization features of both.
 
 ## SARS-CoV-2 example:
 
-<img src="https://github.com/jonas-fuchs/virHEAT/blob/master/example.png" alt="example plot" />
-
+[![Example](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)](https://github.com/jonas-fuchs/virHEAT/blob/master/example.png)
 
 ## Installation
 
 ### via pip (recommened):
 ```shell
 pip install virheat
 ```
```

