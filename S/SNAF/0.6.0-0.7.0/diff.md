# Comparing `tmp/SNAF-0.6.0.tar.gz` & `tmp/SNAF-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SNAF-0.6.0.tar", last modified: Mon Jul 11 07:02:24 2022, max compression
+gzip compressed data, was "dist/SNAF-0.7.0.tar", last modified: Tue May 23 14:57:14 2023, max compression
```

## Comparing `SNAF-0.6.0.tar` & `SNAF-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/
--rw-r--r--   0 ligk2e     (503) staff       (20)     2846 2022-07-11 07:02:24.000000 SNAF-0.6.0/PKG-INFO
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/SNAF.egg-info/
--rw-r--r--   0 ligk2e     (503) staff       (20)     2846 2022-07-11 07:02:23.000000 SNAF-0.6.0/SNAF.egg-info/PKG-INFO
--rw-r--r--   0 ligk2e     (503) staff       (20)      918 2022-07-11 07:02:23.000000 SNAF-0.6.0/SNAF.egg-info/SOURCES.txt
--rw-r--r--   0 ligk2e     (503) staff       (20)      366 2022-07-11 07:02:23.000000 SNAF-0.6.0/SNAF.egg-info/requires.txt
--rw-r--r--   0 ligk2e     (503) staff       (20)       48 2022-07-11 07:02:23.000000 SNAF-0.6.0/SNAF.egg-info/top_level.txt
--rw-r--r--   0 ligk2e     (503) staff       (20)        1 2022-07-11 07:02:23.000000 SNAF-0.6.0/SNAF.egg-info/dependency_links.txt
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/
--rwx------   0 ligk2e     (503) staff       (20)    55216 2022-07-11 06:32:17.000000 SNAF-0.6.0/snaf/snaf.py
--rwx------   0 ligk2e     (503) staff       (20)    10709 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/proteomics.py
--rwx------   0 ligk2e     (503) staff       (20)     2102 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/data_io.py
--rwx------   0 ligk2e     (503) staff       (20)     1516 2022-07-02 02:06:13.000000 SNAF-0.6.0/snaf/__init__.py
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/surface/
--rwx------   0 ligk2e     (503) staff       (20)     3018 2022-06-05 18:43:15.000000 SNAF-0.6.0/snaf/surface/alignment.py
--rwx------   0 ligk2e     (503) staff       (20)     2642 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/surface/data_io.py
--rwx------   0 ligk2e     (503) staff       (20)      166 2022-07-04 13:26:55.000000 SNAF-0.6.0/snaf/surface/__init__.py
--rwx------   0 ligk2e     (503) staff       (20)    25939 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/surface/emboss.py
--rwx------   0 ligk2e     (503) staff       (20)     1427 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/surface/api.py
--rwx------   0 ligk2e     (503) staff       (20)     4464 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/surface/orf_finder.py
--rwx------   0 ligk2e     (503) staff       (20)    78590 2022-07-11 06:23:33.000000 SNAF-0.6.0/snaf/surface/main.py
--rwx------   0 ligk2e     (503) staff       (20)     4718 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/surface/orf_check.py
--rwx------   0 ligk2e     (503) staff       (20)     6900 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/gtex_viewer.py
--rwx------   0 ligk2e     (503) staff       (20)     6489 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/visualize.py
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/dash_app/
--rwx------   0 ligk2e     (503) staff       (20)       73 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/dash_app/__init__.py
--rwx------   0 ligk2e     (503) staff       (20)     2111 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/dash_app/pweblogo.py
--rwx------   0 ligk2e     (503) staff       (20)     7063 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/dash_app/app.py
--rwx------   0 ligk2e     (503) staff       (20)     1331 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/dash_app/schema.py
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/deepimmuno/
--rwx------   0 ligk2e     (503) staff       (20)     7534 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/deepimmuno.py
--rwx------   0 ligk2e     (503) staff       (20)       54 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/__init__.py
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/deepimmuno/models/
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/deepimmuno/models/cnn_model_331_3_7/
--rwx------   0 ligk2e     (503) staff       (20)       59 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/models/cnn_model_331_3_7/checkpoint
--rwx------   0 ligk2e     (503) staff       (20)     4870 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/models/cnn_model_331_3_7/.index
--rwx------   0 ligk2e     (503) staff       (20)   517339 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/models/cnn_model_331_3_7/.data-00000-of-00001
-drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2022-07-11 07:02:24.000000 SNAF-0.6.0/snaf/deepimmuno/data/
--rwx------   0 ligk2e     (503) staff       (20)     3607 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/data/hla2paratopeTable_aligned.txt
--rwx------   0 ligk2e     (503) staff       (20)     6444 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/deepimmuno/data/after_pca.txt
--rwx------   0 ligk2e     (503) staff       (20)     9246 2022-06-19 01:12:48.000000 SNAF-0.6.0/snaf/gtex.py
--rwx------   0 ligk2e     (503) staff       (20)    18502 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/mqpar.xml
--rwx------   0 ligk2e     (503) staff       (20)     6118 2022-05-26 13:22:51.000000 SNAF-0.6.0/snaf/binding.py
--rwx------   0 ligk2e     (503) staff       (20)    21057 2022-06-30 01:42:51.000000 SNAF-0.6.0/snaf/downstream.py
--rw-r--r--   0 ligk2e     (503) staff       (20)     1953 2022-07-11 06:55:14.000000 SNAF-0.6.0/README.md
--rw-r--r--   0 ligk2e     (503) staff       (20)     1940 2022-07-11 06:59:01.000000 SNAF-0.6.0/setup.py
--rw-r--r--   0 ligk2e     (503) staff       (20)       38 2022-07-11 07:02:24.000000 SNAF-0.6.0/setup.cfg
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/
+-rw-r--r--   0 ligk2e     (503) staff       (20)     2892 2023-05-23 14:57:14.000000 SNAF-0.7.0/PKG-INFO
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/SNAF.egg-info/
+-rw-r--r--   0 ligk2e     (503) staff       (20)     2892 2023-05-23 14:57:13.000000 SNAF-0.7.0/SNAF.egg-info/PKG-INFO
+-rw-r--r--   0 ligk2e     (503) staff       (20)      963 2023-05-23 14:57:13.000000 SNAF-0.7.0/SNAF.egg-info/SOURCES.txt
+-rw-r--r--   0 ligk2e     (503) staff       (20)      366 2023-05-23 14:57:13.000000 SNAF-0.7.0/SNAF.egg-info/requires.txt
+-rw-r--r--   0 ligk2e     (503) staff       (20)       48 2023-05-23 14:57:13.000000 SNAF-0.7.0/SNAF.egg-info/top_level.txt
+-rw-r--r--   0 ligk2e     (503) staff       (20)        1 2023-05-23 14:57:13.000000 SNAF-0.7.0/SNAF.egg-info/dependency_links.txt
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/
+-rwx------   0 ligk2e     (503) staff       (20)    70070 2023-04-14 11:24:12.000000 SNAF-0.7.0/snaf/snaf.py
+-rwx------   0 ligk2e     (503) staff       (20)    18302 2023-02-09 17:22:15.000000 SNAF-0.7.0/snaf/proteomics.py
+-rwx------   0 ligk2e     (503) staff       (20)   346869 2023-04-13 15:58:18.000000 SNAF-0.7.0/snaf/HLA_Allele_frequency_21_populations.csv
+-rwx------   0 ligk2e     (503) staff       (20)     2494 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/data_io.py
+-rwx------   0 ligk2e     (503) staff       (20)     5607 2023-01-31 22:46:14.000000 SNAF-0.7.0/snaf/__init__.py
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/surface/
+-rwx------   0 ligk2e     (503) staff       (20)     3018 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/surface/alignment.py
+-rwx------   0 ligk2e     (503) staff       (20)     2642 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/surface/data_io.py
+-rwx------   0 ligk2e     (503) staff       (20)      189 2022-11-05 15:53:48.000000 SNAF-0.7.0/snaf/surface/__init__.py
+-rwx------   0 ligk2e     (503) staff       (20)    25939 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/surface/emboss.py
+-rwx------   0 ligk2e     (503) staff       (20)     1427 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/surface/api.py
+-rwx------   0 ligk2e     (503) staff       (20)     4464 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/surface/orf_finder.py
+-rwx------   0 ligk2e     (503) staff       (20)    88248 2023-01-10 21:32:23.000000 SNAF-0.7.0/snaf/surface/main.py
+-rwx------   0 ligk2e     (503) staff       (20)     4718 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/surface/orf_check.py
+-rwx------   0 ligk2e     (503) staff       (20)    13841 2023-04-30 15:22:51.000000 SNAF-0.7.0/snaf/gtex_viewer.py
+-rwx------   0 ligk2e     (503) staff       (20)     6529 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/visualize.py
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/dash_app/
+-rwx------   0 ligk2e     (503) staff       (20)       73 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/dash_app/__init__.py
+-rwx------   0 ligk2e     (503) staff       (20)     2111 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/dash_app/pweblogo.py
+-rwx------   0 ligk2e     (503) staff       (20)     7063 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/dash_app/app.py
+-rwx------   0 ligk2e     (503) staff       (20)     1331 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/dash_app/schema.py
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/deepimmuno/
+-rwx------   0 ligk2e     (503) staff       (20)     7534 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/deepimmuno.py
+-rwx------   0 ligk2e     (503) staff       (20)       54 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/__init__.py
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/deepimmuno/models/
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/deepimmuno/models/cnn_model_331_3_7/
+-rwx------   0 ligk2e     (503) staff       (20)       59 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/models/cnn_model_331_3_7/checkpoint
+-rwx------   0 ligk2e     (503) staff       (20)     4870 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/models/cnn_model_331_3_7/.index
+-rwx------   0 ligk2e     (503) staff       (20)   517339 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/models/cnn_model_331_3_7/.data-00000-of-00001
+drwxr-xr-x   0 ligk2e     (503) staff       (20)        0 2023-05-23 14:57:14.000000 SNAF-0.7.0/snaf/deepimmuno/data/
+-rwx------   0 ligk2e     (503) staff       (20)     3607 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/data/hla2paratopeTable_aligned.txt
+-rwx------   0 ligk2e     (503) staff       (20)     6444 2022-08-13 20:33:25.000000 SNAF-0.7.0/snaf/deepimmuno/data/after_pca.txt
+-rwx------   0 ligk2e     (503) staff       (20)    21880 2022-11-02 15:32:43.000000 SNAF-0.7.0/snaf/gtex.py
+-rwx------   0 ligk2e     (503) staff       (20)    23963 2022-12-08 22:15:48.000000 SNAF-0.7.0/snaf/mqpar.xml
+-rwx------   0 ligk2e     (503) staff       (20)     6118 2023-01-30 18:48:31.000000 SNAF-0.7.0/snaf/binding.py
+-rwx------   0 ligk2e     (503) staff       (20)    53266 2023-04-28 22:47:55.000000 SNAF-0.7.0/snaf/downstream.py
+-rw-r--r--   0 ligk2e     (503) staff       (20)     1991 2022-08-13 20:33:25.000000 SNAF-0.7.0/README.md
+-rw-r--r--   0 ligk2e     (503) staff       (20)     1982 2023-05-23 14:53:05.000000 SNAF-0.7.0/setup.py
+-rw-r--r--   0 ligk2e     (503) staff       (20)       38 2023-05-23 14:57:14.000000 SNAF-0.7.0/setup.cfg
```

### Comparing `SNAF-0.6.0/PKG-INFO` & `SNAF-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNAF
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python package to predict, prioritize and visualize splicing derived neoantigens, including MHC-bound peptides (T cell antigen) and altered surface protein (B cell antigen)
 Home-page: https://github.com/frankligy/SNAF
 Author: Guangyuan(Frank) Li
 Author-email: li2g2@mail.uc.edu
 Maintainer: Guangyuan(Frank) Li
 Maintainer-email: li2g2@mail.uc.edu
 License: UNKNOWN
@@ -18,25 +18,26 @@
         ![workflow](./images/fig1.png)
         
         
         # Tutorial and documentation
         
         [Full Documentation](https://snaf.readthedocs.io)
         
-        # Input and Output
-        
-        Simply put, user needs to supply ``a folder with bam files``, and the ``HLA type`` assciated with each patient (using your favorite HLA typing tool). And it will generate predicted immunogenic MHC-bound peptides and altered surface protein. Moreover, there's a myriad of convenient function that enables users to conduct survival analysis, association analysis and publication-quality visualiztion. Check our tutorials for more detail.
-        
-        # Interactive Viewers
+        # Interactive Viewers (below, take a few seconds to load)
         
         <p float="left">
           <img src="images/T_viewer.gif" width="45%" />
           <img src="images/B_viewer.gif" width="45%" /> 
         </p>
         
+        # Input and Output 
+        
+        Simply put, user needs to supply ``a folder with bam files``, and the ``HLA type`` assciated with each patient (using your favorite HLA typing tool). And it will generate predicted immunogenic MHC-bound peptides and altered surface protein. Moreover, there's a myriad of convenient function that enables users to conduct survival analysis, association analysis and publication-quality visualiztion. Check our tutorials for more detail.
+        
+        
         # Citation
         
         [Guangyuan Li, Nathan Salomonis. SNAF: Accurate and compatible computational framework for identifying splicing derived neoantigens [abstract]. Cancer Res 2022;82(12_Suppl)](https://aacrjournals.org/cancerres/article/82/12_Supplement/1898/701846/Abstract-1898-SNAF-Accurate-and-compatible)
         
         A preprint will be released soon.
         
         # Contact
```

### Comparing `SNAF-0.6.0/SNAF.egg-info/PKG-INFO` & `SNAF-0.7.0/SNAF.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNAF
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python package to predict, prioritize and visualize splicing derived neoantigens, including MHC-bound peptides (T cell antigen) and altered surface protein (B cell antigen)
 Home-page: https://github.com/frankligy/SNAF
 Author: Guangyuan(Frank) Li
 Author-email: li2g2@mail.uc.edu
 Maintainer: Guangyuan(Frank) Li
 Maintainer-email: li2g2@mail.uc.edu
 License: UNKNOWN
@@ -18,25 +18,26 @@
         ![workflow](./images/fig1.png)
         
         
         # Tutorial and documentation
         
         [Full Documentation](https://snaf.readthedocs.io)
         
-        # Input and Output
-        
-        Simply put, user needs to supply ``a folder with bam files``, and the ``HLA type`` assciated with each patient (using your favorite HLA typing tool). And it will generate predicted immunogenic MHC-bound peptides and altered surface protein. Moreover, there's a myriad of convenient function that enables users to conduct survival analysis, association analysis and publication-quality visualiztion. Check our tutorials for more detail.
-        
-        # Interactive Viewers
+        # Interactive Viewers (below, take a few seconds to load)
         
         <p float="left">
           <img src="images/T_viewer.gif" width="45%" />
           <img src="images/B_viewer.gif" width="45%" /> 
         </p>
         
+        # Input and Output 
+        
+        Simply put, user needs to supply ``a folder with bam files``, and the ``HLA type`` assciated with each patient (using your favorite HLA typing tool). And it will generate predicted immunogenic MHC-bound peptides and altered surface protein. Moreover, there's a myriad of convenient function that enables users to conduct survival analysis, association analysis and publication-quality visualiztion. Check our tutorials for more detail.
+        
+        
         # Citation
         
         [Guangyuan Li, Nathan Salomonis. SNAF: Accurate and compatible computational framework for identifying splicing derived neoantigens [abstract]. Cancer Res 2022;82(12_Suppl)](https://aacrjournals.org/cancerres/article/82/12_Supplement/1898/701846/Abstract-1898-SNAF-Accurate-and-compatible)
         
         A preprint will be released soon.
         
         # Contact
```

### Comparing `SNAF-0.6.0/SNAF.egg-info/SOURCES.txt` & `SNAF-0.7.0/SNAF.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 SNAF.egg-info/PKG-INFO
 SNAF.egg-info/SOURCES.txt
 SNAF.egg-info/dependency_links.txt
 SNAF.egg-info/requires.txt
 SNAF.egg-info/top_level.txt
+snaf/HLA_Allele_frequency_21_populations.csv
 snaf/__init__.py
 snaf/binding.py
 snaf/data_io.py
 snaf/downstream.py
 snaf/gtex.py
 snaf/gtex_viewer.py
 snaf/mqpar.xml
```

### Comparing `SNAF-0.6.0/snaf/snaf.py` & `SNAF-0.7.0/snaf/snaf.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import re
 import requests
 import xmltodict
 import multiprocessing as mp
 import functools
 from tqdm import tqdm
 from itertools import compress
+from ast import literal_eval
+from bisect import bisect, bisect_left
 
 
 # for biopython, pip install biopython
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from Bio.Seq import Seq
 
 # other modules
@@ -40,49 +42,219 @@
 import matplotlib as mpl
 mpl.rcParams['pdf.fonttype'] = 42
 mpl.rcParams['ps.fonttype'] = 42
 mpl.rcParams['font.family'] = 'Arial'
 
 
 # configuration
-def snaf_configuration(exon_table,fasta,software_path_arg=None,binding_method_arg=None):
+def snaf_configuration(exon_table,transcript_db,db_dir,fasta,software_path_arg=None,binding_method_arg=None):
     global dict_exonCoords
     global dict_fa
     global software_path
     global binding_method
+    global dict_exonlist
+    global dict_start_codon
+    global phase_inferer_gtf_dict
     dict_exonCoords = exonCoords_to_dict(exon_table)
+    dict_exonlist = construct_dict_exonlist(transcript_db)
     dict_fa = fasta_to_dict(fasta)
     software_path = software_path_arg
     binding_method = binding_method_arg
 
+    df_start_codon = pd.read_csv(os.path.join(db_dir,'Alt91_db','df_start_codon.txt'),sep='\t',index_col=0)
+    df_start_codon['start_codon'] = [literal_eval(item) for item in df_start_codon['start_codon']]
+    df_start_codon['non_redundant'] = [literal_eval(item) for item in df_start_codon['non_redundant']]
+    dict_start_codon = df_start_codon['start_codon'].to_dict()
+
+    phase_inferer_gtf_dict = process_gtf(os.path.join(db_dir,'Alt91_db','Homo_sapiens.GRCh38.91.gtf'))
+
+    
+
+
+def process_gtf(gtf):
+    # any official ensembl release gtf format
+    '''
+    gtf_dict['ENSG00000186092']
+
+        {'ENST00000641515': [(65419, 65433), (65520, 65573), (69037, 71585)],
+        'ENST00000335137': [(69055, 70108)]}
+    '''
+    gtf_dict = {}
+    with open(gtf,'r') as f:
+        for line in f:
+            try:
+                chrom, source, typ, start, end, score, strand, phase, attrs = line.rstrip('\n').split('\t')
+            except ValueError:  # the header line
+                continue
+            if typ == 'gene':
+                ensg = attrs.split(';')[0].split(' ')[1].strip('"')
+                gtf_dict[ensg] = {}
+            elif typ == 'transcript':
+                enst = attrs.split(';')[2].split(' ')[2].strip('"')
+                gtf_dict[ensg][enst] = []
+            elif typ == 'exon':
+                gtf_dict[ensg][enst].append((int(start),int(end)))
+    return gtf_dict
+
+def get_support_phase(ensg, coord_first_exon_last_base, pssc, strand, length_first):
+    coord_first_exon_last_base, pssc, length_first = int(coord_first_exon_last_base), int(pssc), int(length_first)
+    all_trans = phase_inferer_gtf_dict[ensg]
+    supports = []
+    if strand == '+':
+        for enst, tran in all_trans.items():
+            lis = []
+            [lis.extend(list(exon)) for exon in tran]
+            pssc_insert_pos = bisect(lis, pssc)
+            coord_first_exon_first_base = coord_first_exon_last_base - length_first + 1
+            junction_insert_pos = bisect(lis, coord_first_exon_first_base)
+
+            if junction_insert_pos % 2 == 1 and pssc_insert_pos % 2 == 1:
+                if junction_insert_pos == pssc_insert_pos:
+                    n_bases = coord_first_exon_first_base - pssc + 1
+                elif junction_insert_pos > pssc_insert_pos:
+                    start_exon_index = (pssc_insert_pos - 1) // 2
+                    end_exon_index = (junction_insert_pos - 1) // 2
+                    n_bases = 0
+                    for i, exon in enumerate(tran):
+                        if i == start_exon_index:
+                            n_bases += (exon[1] - pssc + 1)
+                        elif i == end_exon_index:
+                            n_bases += (coord_first_exon_first_base - exon[0] + 1)
+                        else:
+                            if i > start_exon_index and i < end_exon_index:
+                                n_bases += (exon[1] - exon[0] + 1)
+                else:
+                    continue
+            else:
+                continue
+
+
+            remainder = n_bases % 3
+            '''
+            *   *   *   *   |*   *   *    *    *
+                            |6   7   8    9    10
+
+            remainder means a fragment including the first base in the first exon, how many left. 1 left means 6 should be the first base of new codon
+            2 left means 6 should be 6 is the second in last codon, 7 will be the last base in the last codon, have to start with 8
+            0 left means 6 should be the last base in the last codon, so that we start with 7
+            '''
+            if remainder == 1:
+                phase = 0
+            elif remainder == 2:
+                phase = 2
+            elif remainder == 0:
+                phase = 1
+            supports.append((phase, pssc, enst,strand))
+
+    elif strand == '-':
+        for enst, tran in all_trans.items():
+            tran.sort(
+                key=lambda x: x[0])  # because negative strand looks like [(5,7),(2,4)], we change it to [(2,4),(5,7)]
+            lis = []
+            [lis.extend(list(exon)) for exon in tran]
+            pssc_insert_pos = bisect_left(lis, pssc)
+            coord_first_exon_first_base = coord_first_exon_last_base + length_first - 1
+            junction_insert_pos = bisect_left(lis, coord_first_exon_first_base)
+
+            if junction_insert_pos % 2 == 1 and pssc_insert_pos % 2 == 1:
+                if junction_insert_pos == pssc_insert_pos:
+                    n_bases = pssc - coord_first_exon_first_base + 1
+                elif junction_insert_pos < pssc_insert_pos:
+                    start_exon_index = (pssc_insert_pos - 1) // 2
+                    end_exon_index = (junction_insert_pos - 1) // 2
+                    n_bases = 0
+                    for i, exon in enumerate(tran):
+                        if i == start_exon_index:
+                            n_bases += (pssc - exon[0] + 1)
+                        elif i == end_exon_index:
+                            n_bases += (exon[1] - coord_first_exon_first_base + 1)
+                        else:
+                            if i > end_exon_index and i < start_exon_index:
+                                n_bases += (exon[1] - exon[0] + 1)
+                else:
+                    continue
+            else:
+                continue
+
+
+
+            remainder = n_bases % 3  # same idea as above forward strand, see explanation above
+            if remainder == 1:
+                phase = 0
+            elif remainder == 2:
+                phase = 2
+            elif remainder == 0:
+                phase = 1
+            supports.append((phase, pssc, enst, strand))
+
+    return supports   
+
+
+
+    
+def is_in_db(valid):
+    # provide a list with uid without repeats
+    mapping = {}
+    for uid in tqdm(valid):
+        ensg = uid.split(':')[0]
+        exons = ':'.join(uid.split(':')[1:])
+        if '_' in exons or 'U' in exons or 'ENSG' in exons or 'I' in exons:
+            mapping[uid] = False
+        else:
+            exonlist = dict_exonlist[ensg]
+            exonstring = '|'.join(exonlist)
+            e1,e2 = exons.split('-')
+            pattern1 = re.compile(r'^{}\|{}\|'.format(e1,e2))  # ^E1.1|E2.3|
+            pattern2 = re.compile(r'\|{}\|{}$'.format(e1,e2))  # |E1.1|E2.3$
+            pattern3 = re.compile(r'\|{}\|{}\|'.format(e1,e2)) # |E1.1|E2.3|
+            if re.search(pattern3,exonstring) or re.search(pattern2,exonstring) or re.search(pattern1,exonstring):   # as long as match one pattern, should be eliminated
+                mapping[uid] = True
+            else:
+                mapping[uid] = False
+    return mapping
+
+
+
+
+
+
 
 
 class JunctionCountMatrixQuery():
 
     '''
     Instantiate the JunctionCountMatrixQuery class
 
     :param junction_count_matrix: The pandas dataframe for the junction_count_matrix, outputted by AltAnalyze
     :param cores: int, how many cores you'd like to use, if None, then will automatically detect the maximum amount of cores in the OS
-    :param add_control: None or pandas dataframe, SNAF will determine tumor specific junction using GTEx dataset in the downloaded reference folder,
-                        however, if you have additional matched control you want to add, please add that, it is the same format as the junction count matrix, 
-                        but the samples will all be normal control samples.
+    :param add_control: None or a dictionary containing additional controls, additional controls can a dataframe or anndata, for instance, if adding two controls asides from internal GTEx,
+                        {'tcga_matched_control':df,'gtex_skin':adata}, when added database contains multiple tissue types, it is recommended to pass as a AnnData with the tissue
+                        information stored as adata.var['tissue'], otherwise, if passed as a dataframe, or samples will be recognized as a single tissue type, it will affect tumor specifcity
+                        score calculation if using MLE or bayesian hierarchical models.
+    :param not_in_db: boolean, whether to remove junctions that are present in any Ensembl documented transcript, remember some of the documented transcript in
+                      Ensembl are tumor-specific as well, doing so may remove some bona fide hits. But good for reducing number of neoantigens for validation.
+    :param outdir: string, the output folder for storing results
+    :param filter_mode: string, either 'maxmin' or 'prevalance', this correspond to the parameters that will be used in snaf.initialize, if maxmin, use t_min and n_max, 
+                        if prevalance, use normal and tumor cutoff
 
     Example::
 
-        jcmq = JunctionCountMatrixQuery(junction_count_matrix=df,cores=50,add_control=control_df)
+        jcmq = JunctionCountMatrixQuery(junction_count_matrix=df,cores=50,add_control=control_df,not_in_db=True)
         
     '''
 
-    def __init__(self,junction_count_matrix,cores=None,add_control=None):
+    def __init__(self,junction_count_matrix,cores=None,add_control=None,not_in_db=False,outdir='.',filter_mode='maxmin'):
         self.junction_count_matrix = junction_count_matrix
         if cores is None:
             cores = mp.cpu_count()
         self.cores = cores
-        self.get_neojunctions(add_control=add_control)
+        if not_in_db:
+            self.get_neojunctions(add_control=add_control,dict_exonlist=dict_exonlist,outdir=outdir,filter_mode=filter_mode)
+        else:
+            self.get_neojunctions(add_control=add_control,dict_exonlist=None,outdir=outdir,filter_mode=filter_mode)
         
 
     def __str__(self):
         try:
             len_translated = len(self.translated)
         except AttributeError:
             len_translated = None
@@ -101,47 +273,50 @@
                'cond_df: {}\n'\
                'subset: {}\n'\
                'translated: list of {} nj objects\n'\
                'cond_subset_df: {}\n'\
                'results: list of length {}'.format(self.junction_count_matrix.shape,self.cores,len(self.valid),len(self.invalid),
                                                self.cond_df.shape,self.subset.shape,len_translated,shape_cond_subset_df,len_results)
     
-    def get_neojunctions(self,add_control):
-        self.valid, self.invalid, self.cond_df = multiple_crude_sifting(self.junction_count_matrix,add_control)
+    def get_neojunctions(self,add_control,dict_exonlist,outdir,filter_mode):
+        self.valid, self.invalid, self.cond_df = multiple_crude_sifting(self.junction_count_matrix,add_control,dict_exonlist,outdir,filter_mode)
         self.subset = self.junction_count_matrix.loc[self.valid,:]
         self.cond_subset_df = self.cond_df.loc[self.valid,:]
 
     def get_neojunction_info(self,event):  # more for B cell antigen, since we design it in a way that B cell pipeline completely rely on T pipeline for GTEx check
         ed = self.subset.loc[event,:].to_dict()
         freq = np.count_nonzero(np.array(list(ed.values())))/len(ed)
         return ed,freq
 
 
     @staticmethod
-    def get_membrane_tuples(df):
+    def get_membrane_tuples(df,**kwargs):
         '''
         this function is used by SurfaceAntigen pipeline to filter out splicing evnets that are not tumor-specific and also compute
         useful informations for each membrane protein.
 
         :param df: pandas dataframe, the junction count matrix
+        :param **kwargs: will be passed to __init__ of JunctionCountMatrixQuery class function
+
         :return membrane_tuples: a list, in which each item is a tuple (uid,mean_gtex,df_gtex,ed,freq). 
 
             * uid: the uid of the splicing evnet
             * mean_gtex: the mean raw read count across GTEx
             * df_gtex: a dataframe of gtex sample name, tissue types and read count values
             * ed: expression dictionary for tumor samples
             * freq: expression frequency for tumor samples
 
         Example::
 
             membrane_tuples = snaf.JunctionCountMatrixQuery.get_membrane_tuples(df)
 
         '''
         from .surface import filter_to_membrane_protein
-        jcmq = JunctionCountMatrixQuery(junction_count_matrix=df)
+        jcmq = JunctionCountMatrixQuery(junction_count_matrix=df,**kwargs)
+        print(jcmq)
         neojunctions = jcmq.valid
         membrane_uid = filter_to_membrane_protein(neojunctions)
         membrane_tuples = []
         for uid in membrane_uid:
             mean_gtex, df_gtex = tumor_specificity(uid,method='mean',return_df=True)
             ed, freq = jcmq.get_neojunction_info(uid)
             membrane_tuples.append((uid,mean_gtex,df_gtex,ed,freq))
@@ -172,22 +347,22 @@
             for i in sub_index:
                 item_in_group.append(array[i])
             sub_arrays.append(item_in_group)
         return sub_arrays
         
             
     @staticmethod
-    def each_chunk_func(input_,kind,hlas=None,sub_cond_df=None,binding_method=None):
+    def each_chunk_func(input_,kind,hlas=None,strict=False,sub_cond_df=None,binding_method=None):
         if kind == 1:
             nj_list = []
             for uid in input_.index:
                 nj = NeoJunction(uid=uid,count=50,check_gtex=False)
                 nj.detect_type()
                 nj.retrieve_junction_seq()
-                nj.in_silico_translation()    
+                nj.in_silico_translation(strict=strict)    
                 nj_list.append(nj) 
         elif kind == 2:   # out of development
             nj_list = []
             for uid in input_.index:
                 nj = NeoJunction(uid=uid,count=50,check_gtex=False)
                 nj.detect_type()
                 nj.retrieve_junction_seq()
@@ -234,27 +409,28 @@
                     nj.immunogenicity_prediction()
                 except Exception as e:
                     nj_list.append(None)
                     continue
                 nj_list.append(nj)                 
         return nj_list
 
-    def run(self,hlas,outdir='.',name='after_prediction.p'):
+    def run(self,hlas,strict=False,outdir='.',name='after_prediction.p'):
         '''
         main function to run mhc bound peptide T antigen pipeline
 
         :param hlas: list, each item is a list of 6 HLA types associated with each sample, the order of this list must be consistent with the sample name in the df column
+        :param strict: boolean, default is False, determine whether to filter out peptide which doesn't have canonical start codon support
         :param outdir: string, the path where all the results will go into
         :param name: string, the name of the generated pickle result object
 
         Example::
 
             jcmq.run(hlas=hlas,outdir='result',name='after_prediction.p')
         '''
-        self.parallelize_run(kind=1)
+        self.parallelize_run(kind=1,strict=strict)
         print(self)
         self.parallelize_run(kind=3,hlas=hlas)
         self.serialize(outdir=outdir,name=name)
 
     @staticmethod
     def generate_results(path,outdir,criterion=None):
         '''
@@ -271,31 +447,55 @@
 
         jcmq = JunctionCountMatrixQuery.deserialize(name=path)
         stage0_compatible_results(jcmq,outdir=outdir)
         for stage in [3,2,1]:
             jcmq.show_neoantigen_burden(outdir=outdir,name='burden_stage{}.txt'.format(stage),stage=stage,verbosity=1,contain_uid=False,criterion=criterion)
             jcmq.show_neoantigen_frequency(outdir=outdir,name='frequency_stage{}.txt'.format(stage),stage=stage,verbosity=1,contain_uid=False,plot=True,plot_name='frequency_stage{}.pdf'.format(stage),criterion=criterion)
             jcmq.show_neoantigen_frequency(outdir=outdir,name='frequency_stage{}_verbosity1_uid.txt'.format(stage),stage=stage,verbosity=1,contain_uid=True,plot=False,criterion=criterion)
+            # add additional attributes
+            df = pd.read_csv(os.path.join(outdir,'frequency_stage{}_verbosity1_uid.txt'.format(stage)),sep='\t',index_col=0)
+            enhance_frequency_table(df,True,True,outdir,'frequency_stage{}_verbosity1_uid_gene_symbol_coord_mean_mle.txt'.format(stage))
+            # report candidates
+            if stage == 3:
+                dff = pd.read_csv(os.path.join(outdir,'frequency_stage{}_verbosity1_uid_gene_symbol_coord_mean_mle.txt'.format(stage)),sep='\t',index_col=0)
+                for sample in tqdm(jcmq.junction_count_matrix.columns,total=jcmq.junction_count_matrix.shape[1]):
+                    report_candidates(jcmq,dff,sample,os.path.join(outdir,'T_candidates'),True)
+                print('concatenating all T antigen files into one & indicate whether in AltAnalyze database')
+                df_list = []
+                for sample in jcmq.junction_count_matrix.columns:
+                    df_list.append(pd.read_csv(os.path.join(outdir,'T_candidates','T_antigen_candidates_{}.txt'.format(sample)),sep='\t',index_col=0))
+                final_df = pd.concat(df_list,axis=0)
+                all_uid = final_df['uid'].unique().tolist()
+                mapping = is_in_db(all_uid)
+                final_df['in_db'] = final_df['uid'].map(mapping).values
+                final_df.to_csv(os.path.join(outdir,'T_candidates','T_antigen_candidates_all.txt'),sep='\t')
+
+        # add additional attributes to stage0
+        df = pd.read_csv(os.path.join(outdir,'frequency_stage0.txt'),sep='\t',index_col=0)
+        df.index = [','.join([item,item]) for item in df.index]
+        df.to_csv(os.path.join(outdir,'frequency_stage0_verbosity1_uid.txt'),sep='\t')
+        df = pd.read_csv(os.path.join(outdir,'frequency_stage0_verbosity1_uid.txt'),sep='\t',index_col=0)
+        enhance_frequency_table(df,True,True,outdir,'frequency_stage0_verbosity1_uid_gene_symbol_coord_mean_mle.txt')        
 
-    def parallelize_run(self,kind,hlas=None):
+    def parallelize_run(self,kind,hlas=None,strict=False):
         pool = mp.Pool(processes=self.cores)
         if kind == 1 or kind == 2:
             sub_dfs = JunctionCountMatrixQuery.split_df_to_chunks(self.subset,self.cores)
-            r = [pool.apply_async(func=JunctionCountMatrixQuery.each_chunk_func,args=(sub_df,kind,)) for sub_df in sub_dfs]
+            r = [pool.apply_async(func=JunctionCountMatrixQuery.each_chunk_func,args=(sub_df,kind,None,strict,)) for sub_df in sub_dfs]
             pool.close()
             pool.join()
             results = []
             for collect in r:
                 result = collect.get()
                 results.extend(result)
             self.translated = results
         elif kind == 3:
             sub_arrays = JunctionCountMatrixQuery.split_array_to_chunks(self.translated,self.cores)
             sub_cond_dfs = JunctionCountMatrixQuery.split_df_to_chunks(self.cond_subset_df,self.cores)
-            r = [pool.apply_async(func=JunctionCountMatrixQuery.each_chunk_func,args=(sub_array,kind,hlas,sub_cond_df,binding_method,)) for sub_array,sub_cond_df in zip(sub_arrays,sub_cond_dfs)]
+            r = [pool.apply_async(func=JunctionCountMatrixQuery.each_chunk_func,args=(sub_array,kind,hlas,False,sub_cond_df,binding_method,)) for sub_array,sub_cond_df in zip(sub_arrays,sub_cond_dfs)]
             pool.close()
             pool.join()
             results = []
             for collect in r:
                 result = collect.get()
                 results.extend(result)
             self.results = (results,hlas)
@@ -341,14 +541,15 @@
         '''
         Visualize certain Neojunction in certain sample
 
         :param uid: string, the uid for the event you want to check
         :param sample: string, the sample name
         :param outdir: string, where to deposite the figure
         :param tumor: bool, whether to show the expression level in tumor sample as well, default is not
+        :param criterion: a nested tuple, if none of the neoantigens are bound and immunogenic, no candidates will be plotted, so you can relax the criterion a bit based on the format specified.
 
         Example::
 
             jcmq.visualize(uid='ENSG00000167291:E38.6-E39.1',sample='TCGA-DA-A1I1-06A-12R-A18U-07.bed',outdir='./result')
         '''
         if not os.path.exists(outdir):
             os.mkdir(outdir)
@@ -450,23 +651,45 @@
             ax.bar(x=np.arange(df.shape[0]),height=df['n_sample'].values,edgecolor='k')
             ax.set_xlabel('Neoantigen rank by its occurence (descending order)')
             ax.set_ylabel('Occurence (n_sample)')
             ax.set_title('Neoantigen Occurence')
             plt.savefig(os.path.join(outdir,'x_neoantigen_{}'.format(plot_name)),bbox_inches='tight')
             plt.close()
             fig,ax = plt.subplots()
-            sns.histplot(df['n_sample'].values,binwidth=1,kde=True,ax=ax)
-            ax.set_yscale(yscale)
-            plt.savefig(os.path.join(outdir,'x_occurence_{}'.format(plot_name)),bbox_inches='tight')
-            plt.close()
+            try:
+                sns.histplot(df['n_sample'].values,binwidth=1,kde=True,ax=ax)
+                ax.set_yscale(yscale)
+                plt.savefig(os.path.join(outdir,'x_occurence_{}'.format(plot_name)),bbox_inches='tight')
+                plt.close()
+            except ValueError:
+                print('All neoantigens are present in same amount of patients, seaborn histplot can not properly figure out binedge, no occurence plot generated')
+
 
 
 
 
     def show_neoantigen_as_fasta(self,outdir,name,stage,verbosity,contain_uid,sample=None,criterion=None):
+        '''
+        write the neoantigen as a fasta file for MS validation or other purpose
+
+        :param outdir: string ,the output directory for the generated fasta file
+        :param name: string, the name of the output fasta file
+        :param stage: int, either 0,1,2,3, the stage of neoantigen you want to report
+        :param verbosity: int, either 1,2,3, the verbosity of candidates
+        :param contain_uid: boolean, whether you want to contain the junction UID along with the neoantigen
+        :param sample: string, the name of the sample in which you want to extract the neoantigen
+        :param criterion: nested list, the criterion for filtering out the candidate
+
+        Examples::
+
+            jcmq = snaf.JunctionCountMatrixQuery.deserialize('result/after_prediction.p')
+            sample = 'SRR5933735.Aligned.sortedByCoord.out'
+            jcmq.show_neoantigen_as_fasta(outdir='./fasta',name='neoantigen_{}.fasta'.format(sample),stage=2,verbosity=1,contain_uid=True,sample=sample)
+
+        '''
         if not os.path.exists(outdir):
             os.mkdir(outdir)
             
         sub_arrays = JunctionCountMatrixQuery.split_array_to_chunks(self.results[0],self.cores)
         sub_conds = JunctionCountMatrixQuery.split_df_to_chunks(self.cond_subset_df,self.cores)
         hlas = self.results[1]
         column_names = self.subset.columns
@@ -543,36 +766,36 @@
                             dic[cand] = []
                             dic[cand].append(column_name)       
         return dic   
 
 class EnhancedPeptides():
     def __init__(self,peptides,hlas,kind):
         # kind means how to instantiate the EnhancedPeptides object
-        if kind == 2:  # hla-reduced enhanced peptide
+        if kind == 2:  # hla-reduced enhanced peptide, this mode is used when filtsre_based_on_hla
             self.mers = peptides
             self.info = hlas
         else:
             self.mers = []
             self.info = []
             for k,v in peptides.items():
                 self.mers.append(k)
-                phlas = {}  # {pep1:{origin:(extra,n_from_first),hla1:{},hla2:{}}}
+                phlas = {}  # {pep1:{origin:(extra,n_from_first,phase,evidences),hla1:{},hla2:{}}}
                 for pep in v:
-                    if kind == 0:  # each pep is (pep,extra,n_from_first)
+                    if kind == 0:  # each pep is (pep,extra,n_from_first,phase,evidences), this mode is used before binding_prediction
                         pairs = {}
-                        pairs['origin'] = (pep[1],pep[2])
+                        pairs['origin'] = (pep[1],pep[2],pep[3],pep[4])
                         for hla in hlas:
                             pairs[hla] = {}
                         phlas[pep[0]] = pairs
-                    elif kind == 1:   # each pep is (pep,extra,n_from_first,hla)
+                    elif kind == 1:   # each pep is (pep,extra,n_from_first,hla,phase,evidences), this mode is used when filter_based_on_criterion
                         try:
-                            phlas[pep[0]]['origin'] = (pep[1],pep[2])
+                            phlas[pep[0]]['origin'] = (pep[1],pep[2],pep[4],pep[5])
                         except KeyError:
                             phlas[pep[0]] = {}
-                            phlas[pep[0]]['origin'] = (pep[1],pep[2])
+                            phlas[pep[0]]['origin'] = (pep[1],pep[2],pep[4],pep[5])
                         phlas[pep[0]][pep[3]] = {}
                 self.info.append(phlas)
 
     def __str__(self):
         return str(self.info)
 
     def __getitem__(self,key):
@@ -601,15 +824,15 @@
                     for hla in hla_complex.keys():
                         if hla != 'origin':
                             result_list.append((pep,hla))
         elif verbosity==3:
             result_list = []
             for mer in self.mers:
                 for pep,hla_complex in self[mer].items():
-                    extra,n_from_first = hla_complex['origin']
+                    extra,n_from_first,phase,evidences = hla_complex['origin']
                     for hla in hla_complex.keys():
                         if hla != 'origin':
                             result_list.append((pep,hla,extra,n_from_first))
         return result_list
 
     def register_attr(self,df,attr_name):
         '''
@@ -649,15 +872,15 @@
 
 
     def filter_based_on_criterion(self,criteria,reinstantiate=True):
         # criterion: [(net),], ['netMHCpan_el',1,==,SB]
         peptides = {k:[] for k in self.mers}
         for i,k in enumerate(self.mers):
             for pep,hla_complex in self.info[i].items():
-                extra,n_from_first = hla_complex['origin']
+                extra,n_from_first,phase,evidences = hla_complex['origin']
                 for hla,attrs in hla_complex.items():
                     if hla == 'origin':
                         continue
                     boolean_list = []
                     for criterion in criteria:
                         if criterion[1] == 1:   # matched is not a number
                             eval_string = 'attrs[\'{}\'][{}] {} \'{}\''.format(criterion[0],criterion[1],criterion[2],criterion[3])
@@ -666,15 +889,15 @@
                         try:
                             boolean = eval(eval_string)                            
                         except KeyError:
                             boolean = False
                         boolean_list.append(boolean)
                     boolean_final = all(boolean_list)
                     if boolean_final:
-                        peptides[k].append((pep,extra,n_from_first,hla))   # if not reinstantiate, this format is called reduced form
+                        peptides[k].append((pep,extra,n_from_first,hla,phase,evidences))   # if not reinstantiate, this format is called reduced form
         if reinstantiate:
             return EnhancedPeptides(peptides,None,1)
         else:
             return peptides
 
 
 class NeoJunction():
@@ -794,29 +1017,48 @@
         self.event_type = event_type
         return event_type
 
     def retrieve_junction_seq(self):
         if self.event_type != 'invalid':
             ensid = self.uid.split(':')[0]
             subexon1,subexon2 = ':'.join(self.uid.split(':')[1:]).split('-')
-            seq1 = subexon_tran(subexon1,ensid,'site1')
-            seq2 = subexon_tran(subexon2,ensid,'site2')
+            code = is_consecutive(subexon1,subexon2)
+            seq1 = subexon_tran(subexon1,ensid,'site1',code)
+            seq2 = subexon_tran(subexon2,ensid,'site2',code)
             junction = ','.join([seq1,seq2])
             self.junction = junction
         else:
             self.junction = '$' * 10   # indicating invalid uid
 
-    def in_silico_translation(self,ks=[9,10]):
+
+    def in_silico_translation(self,ks=[9,10],strict=False):
         peptides = {k:[] for k in ks}
-        if '$' not in self.junction and '*' not in self.junction and '#' not in self.junction:
+        coord = uid_to_coord(self.uid)  # chr1:555-666(+)
+        if '$' not in self.junction and '*' not in self.junction and '#' not in self.junction and 'unknown' not in coord:
             first,second = self.junction.split(',')
+            # annotate peptide based on starting codon evidence
+            ensg = self.uid.split(':')[0]
+            strand = coord.split('(')[1].rstrip(')')
+            if strand == '+':
+                coord_first_exon_last_base = coord.split(':')[1].split('-')[0]
+            elif strand == '-':
+                coord_first_exon_last_base = coord.split(':')[1].split('(')[0].split('-')[1]
+            possible_start_codon_coord = dict_start_codon.get(ensg,[])   # [333,444] or []
+            support_phases_dict = {}   # {0:[(333,enst,+)]} or {}
+            for pssc in possible_start_codon_coord:
+                supports = get_support_phase(ensg,coord_first_exon_last_base,pssc,strand,len(first))
+                for (phase_, pssc_, enst_, strand_) in supports:
+                    support_phases_dict.setdefault(phase_,[]).append((pssc_,enst_,strand_))
             for phase in [0,1,2]:  # tranlation starts with index "phase"
+                evidences = tuple(support_phases_dict.get(phase,[]))
+                if strict and len(evidences)==0:  # in strict mode, without start_codon evidence, let's skip this phase
+                    continue
                 de_facto_first = first[phase:]
-                pep_dict = get_peptides(de_facto_first,second,ks)
-                for k in ks:
+                pep_dict = get_peptides(de_facto_first,second,ks,phase,evidences)   # (pep,extra,n_from_first,phase,evidences)
+                for k in ks:  
                     peptides[k].extend(pep_dict[k])
                     peptides[k] = list(set(peptides[k]))
         self.peptides = peptides
         return peptides
 
     def binding_prediction(self,hlas,binding_method=None):
         hlas = list(set(hlas))
@@ -876,15 +1118,15 @@
             self.candidates = new
 
 
 
 
 
     def visualize(self,outdir,name,criterion=[('netMHCpan_el',0,'<=',2),('deepimmuno_immunogenicity',1,'==','True'),]):
-        reduced = self.enhanced_peptides.filter_based_on_criterion(criterion,False)
+        reduced = self.enhanced_peptides.filter_based_on_criterion(criterion,False) # now each element should add phase and evidences as well
         '''
         {9: [('LPSPPAQEL', 2, 0, 'HLA-B*08:01'), ('LPSPPAQEL', 2, 0, 'HLA-B*08:02'), 
              ('SLYLLLQHR', 1, 2, 'HLA-A*68:01')], 
         10: [('TSLYLLLQHR', 1, 3, 'HLA-A*68:01'), 
              ('TLPSPPAQEL', 2, 1, 'HLA-A*02:01'), ('TLPSPPAQEL', 2, 1, 'HLA-A*24:02'), ('TLPSPPAQEL', 2, 1, 'HLA-B*08:01'), 
              ('TLPSPPAQEL', 2, 1, 'HLA-B*08:02')]}
         '''
@@ -904,22 +1146,22 @@
             for j in range(0,gs.ncols):
                 ax = fig.add_subplot(gs[i,j])
                 axes_list.append(ax)
         ax_genome = draw_genome(ax_genome,self.uid,dict_exonCoords)
         for i,ax in enumerate(axes_list):
             if i < n_axes:
                 # info
-                aa, extra, n_from_first, hla = to_draw[i]
+                aa, extra, n_from_first, hla, phase, evidences = to_draw[i]
                 first,second = self.junction.split(',')
                 dna_first = extra + n_from_first * 3
                 dna_second = -extra + (len(aa)-n_from_first) * 3
                 binding_score = self.enhanced_peptides[len(aa)][aa][hla]['netMHCpan_el'][0]
                 immunogenicity_score = self.enhanced_peptides[len(aa)][aa][hla]['deepimmuno_immunogenicity'][0]   
                 # draw     
-                ax = show_candicates(ax,aa,extra,n_from_first,hla,first,second,dna_first,dna_second,binding_score,immunogenicity_score) 
+                ax = show_candicates(ax,aa,extra,n_from_first,hla,phase,evidences,first,second,dna_first,dna_second,binding_score,immunogenicity_score) 
             else:
                 ax.axis('off') 
         fig.subplots_adjust(top=0.9)             
         fig.suptitle('{} Count:{}'.format(self.uid,self.count))
         plt.savefig(os.path.join(outdir,name),bbox_inches='tight')
         plt.close()
 
@@ -937,15 +1179,15 @@
         post = [hla[:8] + ':' + hla[-2:] for hla in pre]
     return post
 
 
 
 
 
-def get_peptides(de_facto_first,second,ks):
+def get_peptides(de_facto_first,second,ks,phase,evidences):
     peptides = {k:[] for k in ks}
     extra = len(de_facto_first) % 3  # how many base left in first assuming no stop condon in front of it.
     num = len(de_facto_first) // 3   # how many set of codons in the first.
     aa_first = str(Seq(de_facto_first).translate(to_stop=True))  # if not the multiple of 3, only translate the part that are divisible by 3, it will be a warning for BioPython
     if len(aa_first) == num:  # successfully read through
         if extra == 0:
             continue_second = second
@@ -974,15 +1216,15 @@
                         '''
                         continue
                     if n_from_first <= first_most:
                         if n_from_first > 0:
                             pep = aa_first[-n_from_first:] + aa_second[:n_from_second]
                         elif n_from_first == 0:
                             pep = aa_second[:n_from_second]
-                        peptides[k].append((pep,extra,n_from_first))
+                        peptides[k].append((pep,extra,n_from_first,phase,evidences))
     return peptides
                         
 
 
 def query_from_dict_fa(abs_start,abs_end,EnsID,strand):
     '''
     abs_start and abs_end always means the xth base in forward strand
@@ -1044,27 +1286,56 @@
         my_dict = xmltodict.parse(response.content)
     except:
         exon_seq = '#' * 10  # indicating the UCSC doesn't work
         return exon_seq
     exon_seq = my_dict['DASDNA']['SEQUENCE']['DNA']['#text'].replace('\n','').upper()
     return exon_seq
 
-def subexon_tran(subexon,EnsID,flag):  # flag either site1 or site2
+def is_consecutive(subexon1,subexon2):
+    # I only care of E3.3-E3.4, other form will automatically being labelled as not consecutive
+    # the return code: 0 -> not consecutive, 1 -> consecutive
+    code = 0
+    pattern1 = re.compile(r'^E(\d{1,3})\.(\d{1,3})$')
+    match1 = re.search(pattern1,subexon1)
+    if match1:
+        captured_group1 = match1.group(1)
+        captured_group2 = match1.group(2)
+        pattern2 = re.compile(rf'^E{captured_group1}\.{int(captured_group2)+1}$')
+        match2 = re.search(pattern2,subexon2)
+        if match2:
+            code = 1
+    return code
+
+def subexon_tran(subexon,EnsID,flag,code):  # flag either site1 or site2
     '''
     1. subexon can take multiple forms depending on the event type
     E1.2 or I3.4
     E6.2_67996641 or I40.1_13076665, also depending on whether they are subexon1 or subexon2
     ENSG00000213934:E3.1 or ENSG00000213934:E2.1_473843893894
     U0.1_49689185
     2. everything with trailing suffix will depend on the subexon1 or subexon2, but sometimes, it is fixed (trans-splicing can only be in subexon2)
     3. to be clear, the exon_seq returned is always 5'-3' sequence, not forward anymore.
+
+    if code is 1, meaning its consecutive, E3.3-E3.4, if the flag is site2, then offset the start position of it by 1, the start position is the conceptual
+    start position, if it is in negative string, it will be operated by the stop position.
     '''
+    # let's remove those in the first place
+    # if EnsID not in set(dict_exonCoords.keys()):
+    #     exon_seq = '*' * 10  # indicator for error on MultiPath-PSI itself
+    #     return exon_seq
+        
     try:   # E1.2 or I3.4
         attrs = dict_exonCoords[EnsID][subexon]  # [chr,strand,start,end,suffer] 
-        exon_seq = query_from_dict_fa(attrs[2],attrs[3],EnsID,attrs[1])  
+        if code == 1 and flag == 'site2':
+            if attrs[1] == '+':
+                exon_seq = query_from_dict_fa(int(attrs[2])+1,attrs[3],EnsID,attrs[1])   
+            else:
+                exon_seq = query_from_dict_fa(attrs[2],int(attrs[3])-1,EnsID,attrs[1])
+        else:
+            exon_seq = query_from_dict_fa(attrs[2],attrs[3],EnsID,attrs[1])
     except KeyError:
         if ':' in subexon: # ENSG00000213934:E3.1
             fusionGeneEnsID = subexon.split(':')[0] 
             fusionGeneExon = subexon.split(':')[1]        
             if  '_' in fusionGeneExon:   # ENSG:E2.1_473843893894
                 suffix = fusionGeneExon.split('_')[1]
                 subexon = fusionGeneExon.split('_')[0]
```

### Comparing `SNAF-0.6.0/snaf/data_io.py` & `SNAF-0.7.0/snaf/surface/data_io.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-#!/data/salomonis2/LabFiles/Frank-Li/refactor/neo_env/bin/python3.7
-
-import numpy as np
 import pandas as pd
-import os
-import sys
-import pickle
-import h5py
-import matplotlib.pyplot as plt
-
-# for biopython, pip install biopython
+import numpy as np
+import os,sys
+import subprocess
+import multiprocessing
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from Bio.Seq import Seq
 
-'''
-the pipeline allows seamless integration with all mainstream splicing detection algorithms
-'''
+
+
+def read_uniprot_seq(path):
+    dict_fa = {}
+    with open(path,'r') as in_handle:
+        for title,seq in SimpleFastaParser(in_handle):
+            ensgid = title.split('|')[3]
+            accid = title.split('|')[1]
+            try:
+                dict_fa[ensgid][accid] = seq
+            except KeyError:
+                dict_fa[ensgid] = {}
+                dict_fa[ensgid][accid] = seq
+    return dict_fa   
 
 def fasta_to_dict(path):
     '''
     Let's talk about the fasta file
     >ENSG|chro|start|end
     seq
-
     the start and end always correspond to xth base in forward strand,
     however, if the ENSG falls into backward strand, the seq it stored is actually the 
     backward strand from its own 5' - 3'.
     '''
     dict_fa = {}  # {ENSID, [chro,start,end,seq]}
     with open(path,'r') as in_handle:
         for title,seq in SimpleFastaParser(in_handle):
@@ -34,15 +38,14 @@
             chro = title.split('|')[1]
             start = title.split('|')[2]
             end = title.split('|')[3]
             temp_list=[chro,start,end,seq]
             dict_fa[EnsID] = temp_list
     return dict_fa
 
-
 def exonCoords_to_dict(path):
     '''
     1. the start and end always forward strand
     2. to clarify the overhang issue, the issue is every middle subexon, its end coord need to be backtracted by 1.
     However, this is different operationally in + and - strand. positive strand is to substract the end by 1 (for middle subexon).
     the negative strand is to add the start by 1 (for middle subexon.)
     '''
@@ -56,15 +59,26 @@
             if items[0] in dict_exonCoords:
                 dict_exonCoords[items[0]][items[1]] = coords
             else:
                 dict_exonCoords[items[0]] = {}
                 dict_exonCoords[items[0]][items[1]] = coords
     return dict_exonCoords
 
-
-
+def biotype(df):
+    # make biotype df to a dictionary
+    dic = {} # {EnsGID:{EnsPID:Anno,EnsPID:Anno}}
+    for i in range(df.shape[0]):
+        EnsGID = df.iat[i,0]
+        EnsPID = df.iat[i,1]
+        Anno = df.iat[i,2]
+        try:
+            dic[EnsGID][EnsPID] = Anno
+        except KeyError:
+            dic[EnsGID] = {EnsPID:Anno}
+    return dic
+
```

### Comparing `SNAF-0.6.0/snaf/surface/alignment.py` & `SNAF-0.7.0/snaf/surface/alignment.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/surface/data_io.py` & `SNAF-0.7.0/snaf/data_io.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-import pandas as pd
+#!/data/salomonis2/LabFiles/Frank-Li/refactor/neo_env/bin/python3.7
+
 import numpy as np
-import os,sys
-import subprocess
-import multiprocessing
+import pandas as pd
+import os
+import sys
+import pickle
+import h5py
+import matplotlib.pyplot as plt
+
+# for biopython, pip install biopython
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from Bio.Seq import Seq
 
-
-
-def read_uniprot_seq(path):
-    dict_fa = {}
-    with open(path,'r') as in_handle:
-        for title,seq in SimpleFastaParser(in_handle):
-            ensgid = title.split('|')[3]
-            accid = title.split('|')[1]
-            try:
-                dict_fa[ensgid][accid] = seq
-            except KeyError:
-                dict_fa[ensgid] = {}
-                dict_fa[ensgid][accid] = seq
-    return dict_fa   
+'''
+the pipeline allows seamless integration with all mainstream splicing detection algorithms
+'''
 
 def fasta_to_dict(path):
     '''
     Let's talk about the fasta file
     >ENSG|chro|start|end
     seq
+
     the start and end always correspond to xth base in forward strand,
     however, if the ENSG falls into backward strand, the seq it stored is actually the 
     backward strand from its own 5' - 3'.
     '''
     dict_fa = {}  # {ENSID, [chro,start,end,seq]}
     with open(path,'r') as in_handle:
         for title,seq in SimpleFastaParser(in_handle):
@@ -38,14 +34,15 @@
             chro = title.split('|')[1]
             start = title.split('|')[2]
             end = title.split('|')[3]
             temp_list=[chro,start,end,seq]
             dict_fa[EnsID] = temp_list
     return dict_fa
 
+
 def exonCoords_to_dict(path):
     '''
     1. the start and end always forward strand
     2. to clarify the overhang issue, the issue is every middle subexon, its end coord need to be backtracted by 1.
     However, this is different operationally in + and - strand. positive strand is to substract the end by 1 (for middle subexon).
     the negative strand is to add the start by 1 (for middle subexon.)
     '''
@@ -59,26 +56,22 @@
             if items[0] in dict_exonCoords:
                 dict_exonCoords[items[0]][items[1]] = coords
             else:
                 dict_exonCoords[items[0]] = {}
                 dict_exonCoords[items[0]][items[1]] = coords
     return dict_exonCoords
 
-def biotype(df):
-    # make biotype df to a dictionary
-    dic = {} # {EnsGID:{EnsPID:Anno,EnsPID:Anno}}
-    for i in range(df.shape[0]):
-        EnsGID = df.iat[i,0]
-        EnsPID = df.iat[i,1]
-        Anno = df.iat[i,2]
-        try:
-            dic[EnsGID][EnsPID] = Anno
-        except KeyError:
-            dic[EnsGID] = {EnsPID:Anno}
+
+def construct_dict_exonlist(transcript_db):
+    # this will take the mRNA-exonid file, construct to a lookup table
+    # ENSG: [E1.1|E3.4|E4.5,E1.1|E3.4|E4.6]
+    df_exonlist = pd.read_csv(transcript_db,sep='\t',header=None,names=['EnsGID','EnsTID','EnsPID','Exons'])  # index is number
+    dic = df_exonlist.groupby(by='EnsGID')['Exons'].apply(lambda x:x.tolist()).to_dict()
     return dic
-    
+
+
```

### Comparing `SNAF-0.6.0/snaf/surface/emboss.py` & `SNAF-0.7.0/snaf/surface/emboss.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/surface/api.py` & `SNAF-0.7.0/snaf/surface/api.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/surface/orf_finder.py` & `SNAF-0.7.0/snaf/surface/orf_finder.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/surface/main.py` & `SNAF-0.7.0/snaf/surface/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,51 +6,122 @@
 import re
 import pickle
 from datetime import datetime,date
 from ast import literal_eval
 import requests
 import xmltodict
 from tqdm import tqdm
+from bisect import bisect
 from .data_io import *
 from .orf_finder import *
 from .orf_check import *
 from .alignment import *
 from .api import *
 
 
 import matplotlib as mpl
 mpl.rcParams['pdf.fonttype'] = 42
 mpl.rcParams['ps.fonttype'] = 42
 mpl.rcParams['font.family'] = 'Arial'
 
 
 def initialize(db_dir):
+    '''
+    setting up additional global variables for running B antigen program
+
+    :param db_dir: string, the path to the database folder
+
+    Examples::
+
+        from snaf import surface
+        surface.initialize(db_dir=db_dir)
+
+    '''
     global df_exonlist
     global dict_exonCoords
     global dict_fa
     global dict_biotype
     global df_membrane_proteins
     global dict_uni_fa
+    global df_topology
     print('{} {} starting surface antigen initialization'.format(date.today(),datetime.now().strftime('%H:%M:%S')))
-    transcript_db = os.path.join(db_dir,'mRNA-ExonIDs.txt')
-    exon_table = os.path.join(db_dir,'Hs_Ensembl_exon_add_col.txt')
-    fasta = os.path.join(db_dir,'Hs_gene-seq-2000_flank.fa')
-    biotype_db = os.path.join(db_dir,'Hs_Ensembl_transcript-biotypes.txt')
-    membrane_db = os.path.join(db_dir,'human_membrane_proteins.txt')
-    membrane_fasta_db = os.path.join(db_dir,'uniprot_isoform_enhance.fasta')
+    transcript_db = os.path.join(db_dir,'Alt91_db','mRNA-ExonIDs.txt')
+    exon_table = os.path.join(db_dir,'Alt91_db','Hs_Ensembl_exon_add_col.txt')
+    fasta = os.path.join(db_dir,'Alt91_db','Hs_gene-seq-2000_flank.fa')
+    biotype_db = os.path.join(db_dir,'Alt91_db','Hs_Ensembl_transcript-biotypes.txt')
+    membrane_db = os.path.join(db_dir,'Alt91_db','human_membrane_proteins_acc2ens.txt')
+    membrane_fasta_db = os.path.join(db_dir,'Alt91_db','uniprot_isoform_enhance.fasta')
     df_exonlist = pd.read_csv(transcript_db,sep='\t',header=None,names=['EnsGID','EnsTID','EnsPID','Exons'])  # index is number
     dict_exonCoords = exonCoords_to_dict(exon_table) 
     dict_fa = fasta_to_dict(fasta)
     dict_biotype = biotype(pd.read_csv(biotype_db,sep='\t'))  # index is number
     df_membrane_proteins = pd.read_csv(membrane_db,sep='\t',index_col=0)
     dict_uni_fa = read_uniprot_seq(membrane_fasta_db)
+    df_topology = pd.read_csv(os.path.join(db_dir,'Alt91_db','ENSP_topology.txt'),sep='\t')
     print('{} {} finished surface antigen initialization'.format(date.today(),datetime.now().strftime('%H:%M:%S')))
 
+def generate_full_results(outdir,freq_path,mode,validation_gtf):
+    '''
+    preferred api for wraping both generate_results and report_candiates, good for general usage
+
+    :param outdir: string, the output folder
+    :param freq_path: string, the path to the frequency_stage0_verbosity1_uid_gene_symbol_coord_mean_mle.txt file from T antigen pipeline
+    :param mode: string, either long_read or short_read
+    :param validation_gtf: string, the path to the validation long_read gtf when mode=short_read
 
+    Examples::
 
+        # long read mode
+        surface.generate_full_results(outdir='result/surface',freq_path='result/frequency_stage0_verbosity1_uid_gene_symbol_coord_mean_mle.txt',mode='long_read')
+        # short read mode
+        surface.generate_full_results(outdir='result/surface',freq_path='result/frequency_stage0_verbosity1_uid_gene_symbol_coord_mean_mle.txt',mode='short_read',validation_gtf='/data/salomonis2/LabFiles/Frank-Li/neoantigen/TCGA/SKCM/snaf_analysis/SQANTI-all/collapse_isoforms_classification.filtered_lite.gtf')
+
+    '''
+    if mode == 'long_read':
+        for style in [None,'deletion','insertion']:
+            for overlap_extracellular in [True,False]:
+                cc,cf = generate_results(pickle_path=os.path.join(outdir,'surface_antigen_lr.p'),strigency=3,outdir=outdir,long_read=True,style=style,overlap_extracellular=overlap_extracellular)
+                if cc > 0:
+                    report_candidates(pickle_path=os.path.join(outdir,'surface_antigen_lr.p'),
+                                            candidates_path=os.path.join(outdir,'candidates_3_lr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            validation_path=os.path.join(outdir,'validation_3_lr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            freq_df_path=freq_path,
+                                            mode='long_read',outdir=os.path.join(outdir,'B_candidates'),name='lr_str3_report_{}_{}.txt'.format(style,overlap_extracellular))
+    elif mode == 'short_read':
+        # first strigency 5
+        for style in [None,'deletion','insertion']:
+            for overlap_extracellular in [True,False]:
+                cc,cf = generate_results(pickle_path=os.path.join(outdir,'surface_antigen_sr.p'),strigency=5,outdir=outdir,long_read=False,style=style,overlap_extracellular=overlap_extracellular,gtf=validation_gtf)
+                if cc > 0:
+                    report_candidates(pickle_path=os.path.join(outdir,'surface_antigen_sr.p'),
+                                            candidates_path=os.path.join(outdir,'candidates_5_sr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            validation_path=os.path.join(outdir,'validation_5_sr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            freq_df_path=freq_path,
+                                            mode='short_read',outdir=os.path.join(outdir,'B_candidates'),name='sr_str5_report_{}_{}.txt'.format(style,overlap_extracellular)) 
+        # next strigency 4
+        for style in [None,'deletion','insertion']:
+            for overlap_extracellular in [True,False]:
+                cc, cf = generate_results(pickle_path=os.path.join(outdir,'surface_antigen_sr.p'),strigency=4,outdir=outdir,long_read=False,style=style,overlap_extracellular=overlap_extracellular,gtf=validation_gtf)
+                if cc > 0:
+                    report_candidates(pickle_path=os.path.join(outdir,'surface_antigen_sr.p'),
+                                            candidates_path=os.path.join(outdir,'candidates_4_sr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            validation_path=os.path.join(outdir,'validation_4_sr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            freq_df_path=freq_path,
+                                            mode='short_read',outdir=os.path.join(outdir,'B_candidates'),name='sr_str4_report_{}_{}.txt'.format(style,overlap_extracellular)) 
+
+         # then strigency 3
+        for style in [None,'deletion','insertion']:
+            for overlap_extracellular in [True,False]:
+                cc, cf = generate_results(pickle_path=os.path.join(outdir,'surface_antigen_sr.p'),strigency=3,outdir=outdir,long_read=False,style=style,overlap_extracellular=overlap_extracellular,gtf=None)
+                if cc > 0:
+                    report_candidates(pickle_path=os.path.join(outdir,'surface_antigen_sr.p'),
+                                            candidates_path=os.path.join(outdir,'candidates_3_sr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            validation_path=os.path.join(outdir,'validation_3_sr_{}_{}.txt'.format(style,overlap_extracellular)),
+                                            freq_df_path=freq_path,
+                                            mode='short_read',outdir=os.path.join(outdir,'B_candidates'),name='sr_str3_report_{}_{}.txt'.format(style,overlap_extracellular)) 
 
 def _run_dash_prioritizer_return_events(candidates):
     # candidates is a list of each lines, containing the newline symbol
     collect = []
     for i,line in enumerate(candidates):
         if i % 14 == 0:
             collect.append(line.rstrip('\n')[4:])
@@ -186,22 +257,23 @@
 
 
 def run_dash_B_antigen(pkl,prediction_mode,candidates,python_executable,host=None,port='8050'):
     '''
     run the dash B antigen viewer
 
     :param pkl: string, the path to the surface B pipeline pickle file
+    :param prediction_mode: string, either short_read or long_read
     :param candidates: string ,the path to the candidates.txt file
     :param python_executable: string ,the path to the python executable you are using
     :param host: None or string, string or None, if None, program will run hostname to automatically detect
     :param port: string, default is 8050
 
     Example::
 
-        surface.run_dash_B_antigen(pkl='result/surface_antigen.p',candidates='result/candidates_5.txt',
+        surface.run_dash_B_antigen(pkl='result/surface_antigen.p',candidates='result/candidates_5.txt',prediction_mode='long_read',
                            python_executable='/data/salomonis2/LabFiles/Frank-Li/refactor/neo_env/bin/python3.7')
 
 
 
     '''
     if prediction_mode == 'long_read':
         _run_dash_long_read_mode(pkl,candidates,python_executable,host=host,port=port)
@@ -316,15 +388,15 @@
                 enst = df_certain.loc[df_certain['index']==value_index,:]['EnsTID'].values[0]
                 ensembl_sequence = run_ensembl(ens=enst)
                 emboss_alignment = 'only support peptide now'
             elif value_display == 'orfp':
                 sequence =  sa.orfp[value_index]
                 ensp = df_certain.loc[df_certain['index']==value_index,:]['EnsPID'].values[0]
                 ensembl_sequence = run_ensembl(ens=ensp)
-                emboss_alignment = run_emboss(asequence=ensembl_sequence,bsequence=sequence,python_executable=python_executable)
+                emboss_alignment = run_emboss(asequence=sequence,bsequence=ensembl_sequence,python_executable=python_executable)
                 emboss_alignment = emboss_alignment.replace('\n','<br/>')
             elif value_display == 'junction':
                 sequence = sa.junction
                 enst = df_certain.loc[df_certain['index']==value_index,:]['EnsTID'].values[0]
                 ensembl_sequence = run_ensembl(ens=enst)
                 emboss_alignment = 'only support peptide now'
             elif value_display == 'score':
@@ -493,15 +565,17 @@
 
 def run(uids,outdir,prediction_mode='short_read',n_stride=2,gtf=None,tmhmm=False,software_path=None,serialize=True):
     '''
     main function for run B antigen pipeline
 
     :param uids: list, the membrane tuples
     :param outdir: string, the path where all the output will go into
+    :param prediction_mode: string, either 'short_read' or 'long_read'
     :param n_stride: int, how many exons define a early stop codon, for NMD check
+    :param gtf: None or string, if prediction mode is long_read, supply the path to the gtf file
     :param tmhmm: bool, use tmhmm or not
     :param software_path: None or string, if tmhmm=True, specify the tmhmm software path
     :param serialize: bool, serialize to the pickle file for the result
 
     Examples::
 
         # if using TMHMM
@@ -509,36 +583,38 @@
         # if not using TMHMM
         surface.run(membrane_tuples,outdir='result',tmhmm=False,software_path=None)
     '''
     if not os.path.exists(outdir):
         os.mkdir(outdir)
     results = []
     if prediction_mode == 'short_read':
+        file_name = 'surface_antigen_sr.p'
         for uid,score,df,ed,freq in tqdm(uids,total=len(uids)):
             sa = SurfaceAntigen(uid,score,df,ed,freq,False)
             sa.detect_type()
             sa.retrieve_junction_seq()
             sa.recovery_full_length_protein()
             sa.find_orf()
             sa.orf_check(n_stride=n_stride)
             sa.align_uniprot(tmhmm=tmhmm,software_path=software_path)
             results.append(sa)
     elif prediction_mode == 'long_read':
+        file_name = 'surface_antigen_lr.p'
         gtf_dict = process_est_or_long_read_with_id(gtf)
         for uid,score,df,ed,freq in tqdm(uids,total=len(uids)):
             sa = SurfaceAntigen(uid,score,df,ed,freq,False)
             sa.detect_type()
             sa.retrieve_junction_seq()
             sa.recovery_full_length_protein_long_read(gtf_dict)  # change
             sa.find_orf()
             sa.pseudo_orf_check()  # change
             sa.align_uniprot(tmhmm=tmhmm,software_path=software_path)
             results.append(sa)
     if serialize:
-        with open(os.path.join(outdir,'surface_antigen.p'),'wb') as f:
+        with open(os.path.join(outdir,file_name),'wb') as f:
             pickle.dump(results,f)     
 
     # remove scratch
     name = os.getpid()
     int_file_path = os.path.join(os.path.dirname(os.path.dirname(__file__)),'scratch','{}.fasta'.format(name))  
     os.remove(int_file_path) 
     
@@ -677,15 +753,15 @@
         else:
             if ei == si + 1:
                 return_value = True
                 return_cand = attrs
                 break
     return return_value, return_cand
     
-def report_candidates(pickle_path,candidates_path,validation_path,freq_df_path,mode='short_read',outdir='.',name=None):
+def report_candidates(pickle_path,candidates_path,validation_path,freq_df_path,mode,outdir='.',name=None):
     '''
     report SNAF-B antigen candidates, a more organized and tidy file format for all the candidate.
 
     :param pickle_path: string ,the path to the saved pickle object from `run` command.
     :param candidates_path: string, the path to the saved candidates.txt file which we'd like to reformat
     :param validation_path: string, the path to the saved validation.txt file which accoompanying the candidates.txt file
     :param freq_df_path: string, the path to the frequency table from SNAF-T pipeline, this will provide the frequency of each neojunction in whole cohort.
@@ -696,14 +772,16 @@
     Example::
 
         surface.report_candidates('result/surface_antigen.p','result/candidates_3.txt','result/validation_3.txt',
                                   'result/frequency_stage0_verbosity1_uid_gene_symbol_coord_mean_mle.txt','short_read',
                                   'result','sr_str3_report.txt')
 
     '''
+    if not os.path.exists(outdir):
+        os.mkdir(outdir)
     with open(pickle_path,'rb') as f1:
         results = pickle.load(f1)   # a list of sa object
     with open(candidates_path,'r') as f2:
         candidates = f2.readlines()
     freq_df = pd.read_csv(freq_df_path,sep='\t',index_col=0)
     freq_df['uid'] = [item.split(',')[1] for item in freq_df.index]
     uid_2_ts_mean = pd.Series(index=freq_df['uid'].values,data=freq_df['tumor_specificity_mean'].values).to_dict()
@@ -747,105 +825,183 @@
                     orfp_sequence = sa.orfp[value_index]
                     evidence = sa.full_length_attrs[value_index]
                     candidate_count += 1
                     stream = 'candidate{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\n'.format(candidate_count,uid,mode,evidence,orft_sequence,orfp_sequence,gene,sa.freq,ts_mean,ts_mle,line.rstrip('\n'))
                     f3.write(stream)        
 
 
+def overlap_with_extracellular(sa):
+    uid = sa.uid
+    ensg = uid.split(':')[0]
+    event_type = sa.event_type
+    is_overlap = False
+    if event_type != 'intron_retention':
+        junction_span = uid_to_coord(uid)
+    else:
+        junction_span = uid_to_coord_regular_intron_retention(uid)
+    if 'unknown' in junction_span:  # give it a chance for manual inspection, since not too many unknown
+        return True
+    else:
+        junction_span = junction_span.split('(')[0].split(':')[1].split('-')
+        ensps = ensg2ensps[ensg]
+        for ensp in ensps:
+            try:
+                regions = ensp2regions[ensp]
+            except KeyError:
+                continue
+            coords = []
+            for item in regions:
+                coords.extend(list(item))
+            coords.sort()  # ascending, forward string 
+            left_insert_index = bisect(coords,int(junction_span[0]))
+            right_insert_index = bisect(coords,int(junction_span[1]))
+            if left_insert_index % 2 == 0:  # even number, not in extracellular
+                if right_insert_index > left_insert_index:
+                    is_overlap = True
+            else:
+                is_overlap = True
+        return is_overlap
+
 
 
-    
 
+    
+def send_or_not(op,ref_seq,style,overlap_extracellular,sa):
+    # compare length
+    if len(op) > len(ref_seq):
+        result = 'insertion'
+    else:
+        result = 'deletion'
+    # whether overlap
+    if overlap_extracellular:
+        is_overlap = overlap_with_extracellular(sa)
+    # default send 
+    send = False
+    if style is None:
+        if overlap_extracellular:
+            if is_overlap:
+                send = True
+        else:
+            send = True
+    elif style == result:
+        if overlap_extracellular:
+            if is_overlap:
+                send = True
+        else:
+            send = True
+    return send
 
 
-def generate_results(pickle_path,strigency=3,outdir='.',gtf=None,long_read=False):
+def generate_results(pickle_path,strigency=3,outdir='.',gtf=None,long_read=False,style=None,overlap_extracellular=False):
     '''
     Generate candidates for B antigen
 
     :param pickle_path: string, the path to the pickle result file
     :param strigency: int, from 1-5, how strigent you want to program to be for calling B antigen
 
         * strigency1: novel isoform needs to be absent in uniprot database
         * strigency2: novel isoform also needs to be a documented protein-coding gene
         * strigency3: novel isoform also needs to not be subjected to Nonsense Mediated Decay (NMD)
         * strigency4: novel isoform also needs to have long-read or EST support (as long as the novel junction present in full-length)
         * strigency5: novel isoform also needs to have long-read or EST support (whole ORF needs to be the same as full-length)
     :param outdir: string, path to the output folder
     :param gtf: string, if strigency>3, you need to specify the path to the long-read or EST gtf file
     :param long_read: boolean, whether the last run was using prediction_mode as long_read or not, default to False
+    :param style: None or string, can either be 'deletion' or 'insertion' meaning only generate result with deleted or inserted region
+    :param overlap_extracellular: boolean, default is True, only generate result whose junction overlap with extracellular domain
 
     Example::
 
         # if having gtf file for long-read data
         surface.generate_results(pickle_path='./result/surface_antigen.p',outdir='result',strigency=5,gtf='./SQANTI-all/collapse_isoforms_classification.filtered_lite.gtf')
         # if not having
         surface.generate_results(pickle_path='./result/surface_antigen.p',outdir='result',strigency=3,gtf=None)
 
     '''
     if not os.path.exists(outdir):
         os.mkdir(outdir)
     if gtf is not None:
         global gtf_dict
         gtf_dict = process_est_or_long_read_with_id(gtf)
+    if overlap_extracellular:   # have to load some database
+        global ensg2ensps
+        global ensp2regions
+        ensg2ensps = pd.Series(index=df_exonlist['EnsGID'].values,data=df_exonlist['EnsPID'].values).groupby(level=0).apply(lambda x:x.tolist()).to_dict()
+        df_topology['region'] = [(int(start),int(end)) for start,end in zip(df_topology['genomic_start'],df_topology['genomic_stop'])]
+        ensp2regions = df_topology.groupby(by='ensembl_prot')['region'].apply(lambda x:x.tolist()).to_dict()
     with open(pickle_path,'rb') as f:
         results = pickle.load(f)
     count_candidates = 0
     count_further = 0
     candidates = []
     with open(os.path.join(outdir,'further.txt'),'w') as f2:
         for sa in results:
+            uid = sa.uid
+            ensg = sa.uid.split(':')[0]
+            ref_seq = list(dict_uni_fa[ensg].items())[0][1]
             valid_indices = []
             if len(sa.comments) > 0:
                 print(sa,file=f2)
                 count_further += 1
             else:
-                send = False
+                sends = []
                 for i,(op,n,t,a) in enumerate(zip(sa.orfp,sa.nmd,sa.translatability,sa.alignment)):
                     if strigency == 5:
                         if n == '#' and t == '#' and a==True:
                             value,cand_attrs = is_support_by_est_or_long_read(sa,op,strict=True)
                             if value:
-                                send = True
-                                valid_indices.append(i)
+                                send = send_or_not(op,ref_seq,style,overlap_extracellular,sa)
+                                sends.append(send)
+                                if send:
+                                    valid_indices.append(i)
                     elif strigency == 4:
                         if n == '#' and t == '#' and a==True:
                             value,cand_attrs = is_support_by_est_or_long_read(sa,op,strict=False)
                             if value:
-                                send = True
-                                valid_indices.append(i)
+                                send = send_or_not(op,ref_seq,style,overlap_extracellular,sa)
+                                sends.append(send)
+                                if send:
+                                    valid_indices.append(i)
                     elif strigency == 3:
                         if n == '#' and t == '#' and a==True:
-                            send = True
-                            valid_indices.append(i)
-                            cand_attrs = None
-                    elif strigency == 2:
+                            send = send_or_not(op,ref_seq,style,overlap_extracellular,sa)
+                            sends.append(send)
+                            if send:
+                                valid_indices.append(i)
+                                cand_attrs = None
+                    elif strigency == 2:    # out of development
                         if t == '#' and a==True:
-                            send = True
-                            valid_indices.append(i)
-                            cand_attrs = None
-                    elif strigency == 1:
+                            send = compare_length(op,ref_seq,style)
+                            if send:
+                                valid_indices.append(i)
+                                cand_attrs = None
+                    elif strigency == 1:   # out of development
                         if a==True:
-                            send = not send
-                            valid_indices.append(i)
-                            cand_attrs = None
-                if send:
+                            send = compare_length(op,ref_seq,style)
+                            if send:
+                                valid_indices.append(i)
+                                cand_attrs = None
+                if any(sends):
                     candidates.append((sa,sa.score,sa.freq,len(valid_indices),sa.uid,valid_indices,cand_attrs))
                     count_candidates += 1
-    sorted_candidates = sorted(candidates,key=lambda x:(x[1],-x[2],-x[3]),reverse=False)
-    uid_list = list(list(zip(*sorted_candidates))[4])
-    ensg_list = [uid.split(':')[0] for uid in uid_list]
-    gene_symbols = ensemblgene_to_symbol(ensg_list,'human')
-    if long_read:
-        file_name_lr = '_lr'
+    if count_candidates > 0:
+        sorted_candidates = sorted(candidates,key=lambda x:(x[1],-x[2],-x[3]),reverse=False)
+        uid_list = list(list(zip(*sorted_candidates))[4])
+        ensg_list = [uid.split(':')[0] for uid in uid_list]
+        gene_symbols = ensemblgene_to_symbol(ensg_list,'human')
+        if long_read:
+            file_name_lr = '_lr'
+        else:
+            file_name_lr = '_sr'
+        with open(os.path.join(outdir,'candidates_{}{}_{}_{}.txt'.format(strigency,file_name_lr,style,overlap_extracellular)),'w') as f1, open(os.path.join(outdir,'validation_{}{}_{}_{}.txt'.format(strigency,file_name_lr,style,overlap_extracellular)),'w') as f3:
+            for (sa,score,freq,hit,uid,vi,ca),gene in zip(sorted_candidates,gene_symbols):
+                print(sa,'valid_indices:{}\n'.format(vi),'gene_symbol:{}\n'.format(gene),file=f1,sep='',end='\n')
+                print(ca,file=f3,sep='\n',end='\n')
     else:
-        file_name_lr = ''
-    with open(os.path.join(outdir,'candidates_{}{}.txt'.format(strigency,file_name_lr)),'w') as f1, open(os.path.join(outdir,'validation_{}{}.txt'.format(strigency,file_name_lr)),'w') as f3:
-        for (sa,score,freq,hit,uid,vi,ca),gene in zip(sorted_candidates,gene_symbols):
-            print(sa,'valid_indices:{}\n'.format(vi),'gene_symbol:{}\n'.format(gene),file=f1,sep='',end='\n')
-            print(ca,file=f3,sep='\n',end='\n')
+        print('no candidates for strigency {} style {} overlap_extracellular {}'.format(strigency, style, overlap_extracellular))
     return count_candidates,count_further
 
 
 def ensemblgene_to_symbol(query,species):
     '''
     Examples::
         from sctriangulate.preprocessing import GeneConvert
```

### Comparing `SNAF-0.6.0/snaf/surface/orf_check.py` & `SNAF-0.7.0/snaf/surface/orf_check.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/visualize.py` & `SNAF-0.7.0/snaf/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 '''
 
 import matplotlib as mpl
 mpl.rcParams['pdf.fonttype'] = 42
 mpl.rcParams['ps.fonttype'] = 42
 mpl.rcParams['font.family'] = 'Arial'
 
-def show_candicates(ax,aa,extra,n_from_first,hla,first,second,dna_first,dna_second,binding_score,immunogenicity_score):
+def show_candicates(ax,aa,extra,n_from_first,hla,phase,evidences,first,second,dna_first,dna_second,binding_score,immunogenicity_score):
     # set lim
     ax.set_xlim(0,100)
     ax.set_ylim(0,100)
     # draw exons
     rect_first = Rectangle((30,10),20,5,linewidth=1,edgecolor='k',facecolor='blue')
     rect_second = Rectangle((50,10),20,5,linewidth=1,edgecolor='k',facecolor='orange')
     ax.add_patch(rect_first)
@@ -46,15 +46,15 @@
     # draw barplot for scores
     barcontainer = ax.bar(x=[25,75],height=[np.interp(binding_score,xp=(0,2),fp=(0,50)),np.interp(immunogenicity_score,xp=(0,1),fp=(0,50))],bottom=50,width=20,color=['#158BFB','#F2075D'])
     ax.text(x=barcontainer[0].get_x() + barcontainer[0].get_width()/2,y=50,s='binding',fontsize=3,va='top',ha='center')
     ax.text(x=barcontainer[1].get_x() + barcontainer[1].get_width()/2,y=50,s='immunogenicity',fontsize=3,va='top',ha='center')
     ax.text(x=barcontainer[0].get_x() + barcontainer[0].get_width()/2,y=barcontainer[0].get_y() + barcontainer[0].get_height(),s='{}'.format(round(binding_score,3)),fontsize=3,va='top',ha='center')
     ax.text(x=barcontainer[1].get_x() + barcontainer[1].get_width()/2,y=barcontainer[1].get_y() + barcontainer[1].get_height(),s='{}'.format(round(immunogenicity_score,3)),fontsize=3,va='top',ha='center')
     # annotate HLA and score
-    ax.set_title('{}'.format(hla),fontsize=3)
+    ax.set_title('{}\n{}\n{}'.format(hla,phase,evidences),fontsize=3)
     # remove tick and labels
     ax.set_xticks([])
     ax.set_yticks([])
     return ax
 
 def get_base_subexon_and_trail(subexon):
     if 'U' in subexon:
```

### Comparing `SNAF-0.6.0/snaf/dash_app/pweblogo.py` & `SNAF-0.7.0/snaf/dash_app/pweblogo.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/dash_app/app.py` & `SNAF-0.7.0/snaf/dash_app/app.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/dash_app/schema.py` & `SNAF-0.7.0/snaf/dash_app/schema.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/deepimmuno/deepimmuno.py` & `SNAF-0.7.0/snaf/deepimmuno/deepimmuno.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/deepimmuno/models/cnn_model_331_3_7/.index` & `SNAF-0.7.0/snaf/deepimmuno/models/cnn_model_331_3_7/.index`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/deepimmuno/models/cnn_model_331_3_7/.data-00000-of-00001` & `SNAF-0.7.0/snaf/deepimmuno/models/cnn_model_331_3_7/.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/deepimmuno/data/hla2paratopeTable_aligned.txt` & `SNAF-0.7.0/snaf/deepimmuno/data/hla2paratopeTable_aligned.txt`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/deepimmuno/data/after_pca.txt` & `SNAF-0.7.0/snaf/deepimmuno/data/after_pca.txt`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/snaf/binding.py` & `SNAF-0.7.0/snaf/binding.py`

 * *Files identical despite different names*

### Comparing `SNAF-0.6.0/README.md` & `SNAF-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 ![workflow](./images/fig1.png)
 
 
 # Tutorial and documentation
 
 [Full Documentation](https://snaf.readthedocs.io)
 
-# Input and Output
-
-Simply put, user needs to supply ``a folder with bam files``, and the ``HLA type`` assciated with each patient (using your favorite HLA typing tool). And it will generate predicted immunogenic MHC-bound peptides and altered surface protein. Moreover, there's a myriad of convenient function that enables users to conduct survival analysis, association analysis and publication-quality visualiztion. Check our tutorials for more detail.
-
-# Interactive Viewers
+# Interactive Viewers (below, take a few seconds to load)
 
 <p float="left">
   <img src="images/T_viewer.gif" width="45%" />
   <img src="images/B_viewer.gif" width="45%" /> 
 </p>
 
+# Input and Output 
+
+Simply put, user needs to supply ``a folder with bam files``, and the ``HLA type`` assciated with each patient (using your favorite HLA typing tool). And it will generate predicted immunogenic MHC-bound peptides and altered surface protein. Moreover, there's a myriad of convenient function that enables users to conduct survival analysis, association analysis and publication-quality visualiztion. Check our tutorials for more detail.
+
+
 # Citation
 
 [Guangyuan Li, Nathan Salomonis. SNAF: Accurate and compatible computational framework for identifying splicing derived neoantigens [abstract]. Cancer Res 2022;82(12_Suppl)](https://aacrjournals.org/cancerres/article/82/12_Supplement/1898/701846/Abstract-1898-SNAF-Accurate-and-compatible)
 
 A preprint will be released soon.
 
 # Contact
```

### Comparing `SNAF-0.6.0/setup.py` & `SNAF-0.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,29 +29,29 @@
     'dash==2.0.0',
     'dash-dangerously-set-inner-html==0.0.2',
     'mygene==3.2.2'
 ]
 
 setup(
     name = 'SNAF',
-    version = '0.6.0',
+    version = '0.7.0',
     description = 'A Python package to predict, prioritize and visualize splicing derived neoantigens, including MHC-bound peptides (T cell antigen) and altered surface protein (B cell antigen)',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author = 'Guangyuan(Frank) Li',
     author_email='li2g2@mail.uc.edu',
     maintainer='Guangyuan(Frank) Li',
     maintainer_email = 'li2g2@mail.uc.edu',
     url='https://github.com/frankligy/SNAF',
     project_urls={
         'Documentation':'https://snaf.readthedocs.io',
     },
     packages=['snaf','snaf/deepimmuno','snaf/dash_app','snaf/surface'],
     package_data = {'snaf/deepimmuno':['data/*','models/cnn_model_331_3_7/.data-00000-of-00001','models/cnn_model_331_3_7/.index','models/cnn_model_331_3_7/checkpoint'],
-                    'snaf':['mqpar.xml']},
+                    'snaf':['mqpar.xml','HLA_Allele_frequency_21_populations.csv']},
     install_requires=requires,
     python_requires='>=3.7',
     classifers=[
           'Development Status :: 3 - Alpha',
           'Programming Language :: Python :: 3',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
```

