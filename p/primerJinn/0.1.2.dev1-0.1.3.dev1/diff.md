# Comparing `tmp/primerJinn-0.1.2.dev1.tar.gz` & `tmp/primerJinn-0.1.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerJinn-0.1.2.dev1.tar", last modified: Wed May 10 16:27:16 2023, max compression
+gzip compressed data, was "primerJinn-0.1.3.dev1.tar", last modified: Tue May 23 20:34:54 2023, max compression
```

## Comparing `primerJinn-0.1.2.dev1.tar` & `primerJinn-0.1.3.dev1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-10 16:27:16.908419 primerJinn-0.1.2.dev1/
--rw-r--r--   0 semiquant   (502) staff       (20)    10175 2023-05-10 16:27:16.908159 primerJinn-0.1.2.dev1/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     9746 2023-05-10 01:04:40.000000 primerJinn-0.1.2.dev1/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-10 16:27:16.907977 primerJinn-0.1.2.dev1/primerJinn.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)    10175 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-10 16:27:16.908463 primerJinn-0.1.2.dev1/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-10 16:27:07.000000 primerJinn-0.1.2.dev1/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-23 20:34:54.437572 primerJinn-0.1.3.dev1/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10988 2023-05-23 20:34:54.437273 primerJinn-0.1.3.dev1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)    10559 2023-05-23 20:30:00.000000 primerJinn-0.1.3.dev1/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-23 20:34:54.437083 primerJinn-0.1.3.dev1/primerJinn.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10988 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-23 20:34:54.437621 primerJinn-0.1.3.dev1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-23 20:34:36.000000 primerJinn-0.1.3.dev1/setup.py
```

### Comparing `primerJinn-0.1.2.dev1/PKG-INFO` & `primerJinn-0.1.3.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.2.dev1
+Version: 0.1.3.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,17 @@
 | **Both**          | N            | output             | The name of the output file.                                                                                                                                              | 'MultiPlexPrimerSet' or 'in_silico_PCR' |
 | **primer design** | N            | primer_len         | The desired length of the primers.                                                                                                                                        | 20                                      |
 | **primer design** | N            | product_size_min   | The desired min size for the PCR product.                                                                                                                                 | 400                                     |
 | **primer design** | N            | product_size_max   | The desired max size for the PCR product.                                                                                                                                 | 800                                     |
 | **primer design** | N            | ret                | The maximum number of primer pairs to return                                                                                                                              | 100                                     |
 | **primer design** | N            | Q5                 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3                                                                                       | TRUE                                    |
 | **primer design** | N            | background         | The path to the mispriming library FASTA file                                                                                                                             |                                         |
+| **primer design** | N            | ill_adapt         | Add Illumina partial adapters                                                                                                                              | FALSE                                         |
+| **primer design** | N            | clamp         | Require GC clamp                                                                                                                               | 0                                         |
+| **primer design** | N            | clamp         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
 | **in silico PCR** | N            | product_size_max   | Maximum length of PCR products in nucleotides.                                                                                                                            | 2000                                    |
 | **in silico PCR** | N            | req_five           | Require the 5' end of the primer to bind?                                                                                                                                 | TRUE                                    |
 
 
 ### Dependencies
 
 -   Python 3
```

### Comparing `primerJinn-0.1.2.dev1/README.md` & `primerJinn-0.1.3.dev1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 | **Both**          | N            | output             | The name of the output file.                                                                                                                                              | 'MultiPlexPrimerSet' or 'in_silico_PCR' |
 | **primer design** | N            | primer_len         | The desired length of the primers.                                                                                                                                        | 20                                      |
 | **primer design** | N            | product_size_min   | The desired min size for the PCR product.                                                                                                                                 | 400                                     |
 | **primer design** | N            | product_size_max   | The desired max size for the PCR product.                                                                                                                                 | 800                                     |
 | **primer design** | N            | ret                | The maximum number of primer pairs to return                                                                                                                              | 100                                     |
 | **primer design** | N            | Q5                 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3                                                                                       | TRUE                                    |
 | **primer design** | N            | background         | The path to the mispriming library FASTA file                                                                                                                             |                                         |
+| **primer design** | N            | ill_adapt         | Add Illumina partial adapters                                                                                                                              | FALSE                                         |
+| **primer design** | N            | clamp         | Require GC clamp                                                                                                                               | 0                                         |
+| **primer design** | N            | clamp         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
 | **in silico PCR** | N            | product_size_max   | Maximum length of PCR products in nucleotides.                                                                                                                            | 2000                                    |
 | **in silico PCR** | N            | req_five           | Require the 5' end of the primer to bind?                                                                                                                                 | TRUE                                    |
 
 
 ### Dependencies
 
 -   Python 3
```

### Comparing `primerJinn-0.1.2.dev1/primerJinn.egg-info/PKG-INFO` & `primerJinn-0.1.3.dev1/primerJinn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.2.dev1
+Version: 0.1.3.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,17 @@
 | **Both**          | N            | output             | The name of the output file.                                                                                                                                              | 'MultiPlexPrimerSet' or 'in_silico_PCR' |
 | **primer design** | N            | primer_len         | The desired length of the primers.                                                                                                                                        | 20                                      |
 | **primer design** | N            | product_size_min   | The desired min size for the PCR product.                                                                                                                                 | 400                                     |
 | **primer design** | N            | product_size_max   | The desired max size for the PCR product.                                                                                                                                 | 800                                     |
 | **primer design** | N            | ret                | The maximum number of primer pairs to return                                                                                                                              | 100                                     |
 | **primer design** | N            | Q5                 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3                                                                                       | TRUE                                    |
 | **primer design** | N            | background         | The path to the mispriming library FASTA file                                                                                                                             |                                         |
+| **primer design** | N            | ill_adapt         | Add Illumina partial adapters                                                                                                                              | FALSE                                         |
+| **primer design** | N            | clamp         | Require GC clamp                                                                                                                               | 0                                         |
+| **primer design** | N            | clamp         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
 | **in silico PCR** | N            | product_size_max   | Maximum length of PCR products in nucleotides.                                                                                                                            | 2000                                    |
 | **in silico PCR** | N            | req_five           | Require the 5' end of the primer to bind?                                                                                                                                 | TRUE                                    |
 
 
 ### Dependencies
 
 -   Python 3
```

### Comparing `primerJinn-0.1.2.dev1/setup.py` & `primerJinn-0.1.3.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.14.0+/bin"))
 
 
 setup(
     name='primerJinn',
-    version='0.1.2.dev1',
+    version='0.1.3.dev1',
     url='https://github.com/SemiQuant/primerJinn',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
```

