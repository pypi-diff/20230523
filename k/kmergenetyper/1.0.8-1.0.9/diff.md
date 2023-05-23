# Comparing `tmp/kmergenetyper-1.0.8.tar.gz` & `tmp/kmergenetyper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmergenetyper-1.0.8.tar", last modified: Thu Apr 13 12:05:07 2023, max compression
+gzip compressed data, was "kmergenetyper-1.0.9.tar", last modified: Mon May  1 12:23:23 2023, max compression
```

## Comparing `kmergenetyper-1.0.8.tar` & `kmergenetyper-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.641918 kmergenetyper-1.0.8/
--rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.8/LICENSE
--rw-r--r--   0 malhal     (502) staff       (20)      645 2023-04-13 12:05:07.641797 kmergenetyper-1.0.8/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      361 2023-04-13 12:04:26.000000 kmergenetyper-1.0.8/README.md
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.639987 kmergenetyper-1.0.8/bin/
--rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.8/bin/kmergenetyper
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.641168 kmergenetyper-1.0.8/kmergenetyper/
--rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.8/kmergenetyper/__init__.py
--rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.8/kmergenetyper/kma.py
--rw-r--r--   0 malhal     (502) staff       (20)     4010 2023-04-11 12:06:05.000000 kmergenetyper-1.0.8/kmergenetyper/realignConsensus.py
--rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.8/kmergenetyper/typeGenes.py
--rw-r--r--   0 malhal     (502) staff       (20)       21 2023-04-13 12:04:58.000000 kmergenetyper-1.0.8/kmergenetyper/version.py
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.641610 kmergenetyper-1.0.8/kmergenetyper.egg-info/
--rw-r--r--   0 malhal     (502) staff       (20)      645 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/SOURCES.txt
--rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/dependency_links.txt
--rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/top_level.txt
--rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-13 12:05:07.641963 kmergenetyper-1.0.8/setup.cfg
--rw-r--r--   0 malhal     (502) staff       (20)      659 2023-04-13 12:05:04.000000 kmergenetyper-1.0.8/setup.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.551486 kmergenetyper-1.0.9/
+-rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.9/LICENSE
+-rw-r--r--   0 malhal     (502) staff       (20)      645 2023-05-01 12:23:23.551356 kmergenetyper-1.0.9/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      361 2023-04-13 12:04:26.000000 kmergenetyper-1.0.9/README.md
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.549758 kmergenetyper-1.0.9/bin/
+-rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.9/bin/kmergenetyper
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.550786 kmergenetyper-1.0.9/kmergenetyper/
+-rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.9/kmergenetyper/__init__.py
+-rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.9/kmergenetyper/kma.py
+-rw-r--r--   0 malhal     (502) staff       (20)     4303 2023-05-01 12:22:54.000000 kmergenetyper-1.0.9/kmergenetyper/realignConsensus.py
+-rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.9/kmergenetyper/typeGenes.py
+-rw-r--r--   0 malhal     (502) staff       (20)       21 2023-05-01 12:23:10.000000 kmergenetyper-1.0.9/kmergenetyper/version.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.551204 kmergenetyper-1.0.9/kmergenetyper.egg-info/
+-rw-r--r--   0 malhal     (502) staff       (20)      645 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      325 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/SOURCES.txt
+-rw-r--r--   0 malhal     (502) staff       (20)        1 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/dependency_links.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       14 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/top_level.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       38 2023-05-01 12:23:23.551529 kmergenetyper-1.0.9/setup.cfg
+-rw-r--r--   0 malhal     (502) staff       (20)      710 2023-04-21 07:49:49.000000 kmergenetyper-1.0.9/setup.py
```

### Comparing `kmergenetyper-1.0.8/LICENSE` & `kmergenetyper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.8/PKG-INFO` & `kmergenetyper-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmergenetyper
-Version: 1.0.8
+Version: 1.0.9
 Summary: kmergenetyper - K-mer Gene Typer
 Home-page: https://https://github.com/MBHallgren/kmergenetyper
 Author: Malte B. Hallgren
 Author-email: malhal@food.dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kmergenetyper-1.0.8/bin/kmergenetyper` & `kmergenetyper-1.0.9/bin/kmergenetyper`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.8/kmergenetyper/kma.py` & `kmergenetyper-1.0.9/kmergenetyper/kma.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.8/kmergenetyper/realignConsensus.py` & `kmergenetyper-1.0.9/kmergenetyper/realignConsensus.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open('{}/{}.res'.format(output, prefix), 'r') as f:
         for line in f:
             line = line.strip()
             if not line.startswith('#'):
                 line = line.split('\t')
                 for item in line:
                     item = item.strip()
-                if float(line[4]) < 100.00:
+                if float(line[4]) != 100.00 or float(line[5]) != 100.00 or float(line[6]) != 100.00: #Non perfect alignment for Template_Identity	Template_Coverage	Query_Identity
                     non_perfect_hits.append('>' + line[0].strip())
                 alignment_dict[line[0]] = line[1:]
             else:
                 headers = line
 
     alignment_dict = reformat_dict(alignment_dict)
 
@@ -51,15 +51,15 @@
         for value in input_dict[item]:
             output_dict[item.strip()].append(value.strip())
     return output_dict
 def eval_realignments(output, prefix, headers, alignment_dict, non_perfect_hits):
     realignment_dict = {}
 
     for item in alignment_dict:
-        if float(alignment_dict[item][3]) == 100.00:
+        if float(alignment_dict[item][3]) == 100.00 and float(alignment_dict[item][4]) == 100.00 and float(alignment_dict[item][5]) == 100.00: #Perfect alignment for Template_Identity	Template_Coverage	Query_Identity
             realignment_dict[item] = alignment_dict[item]
 
     for item in non_perfect_hits:
         with open('{}/{}.res'.format(output, item[1:]), 'r') as f:
             original_gene = item[1:]
             for line in f:
                 line = line.rstrip()
@@ -68,22 +68,22 @@
                     if gene not in realignment_dict:
                         realignment_dict[gene] = alignment_dict[original_gene]
                         t_id_1 = realignment_dict[gene][3]
                         t_id_2 = line.split('\t')[4]
                         if float(t_id_1) < float(t_id_2):
                             realignment_dict[gene][3] = t_id_2 # Replace template identity
                             realignment_dict[gene][4] = line.split('\t')[5]  # Replace template coverage
-                            realignment_dict[gene][5] = line.split('\t')[6]  # Replace template coverage
+                            realignment_dict[gene][5] = line.split('\t')[6]  # Replace query identity
                     else:
                         t_id_1 = realignment_dict[gene][3]
                         t_id_2 = line.split('\t')[4]
                         if float(t_id_1) < float(t_id_2):
                             realignment_dict[gene][3] = t_id_2 #Replace template identity
                             realignment_dict[gene][4] = line.split('\t')[5] #Replace template coverage
-                            realignment_dict[gene][5] = line.split('\t')[6]  # Replace template coverage
+                            realignment_dict[gene][5] = line.split('\t')[6]  # Replace query identity
     realignment_dict = reformat_dict(realignment_dict)
 
     keys = list(realignment_dict.keys())
     keys.sort()
 
     with open('{}/final_{}.res'.format(output, prefix), 'w') as f:
         print (headers, file=f)
```

### Comparing `kmergenetyper-1.0.8/kmergenetyper/typeGenes.py` & `kmergenetyper-1.0.9/kmergenetyper/typeGenes.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.8/kmergenetyper.egg-info/PKG-INFO` & `kmergenetyper-1.0.9/kmergenetyper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmergenetyper
-Version: 1.0.8
+Version: 1.0.9
 Summary: kmergenetyper - K-mer Gene Typer
 Home-page: https://https://github.com/MBHallgren/kmergenetyper
 Author: Malte B. Hallgren
 Author-email: malhal@food.dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kmergenetyper-1.0.8/setup.py` & `kmergenetyper-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+from kmergenetyper.version import __version__
+
 setup(
     name='kmergenetyper',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.8',
+    version=__version__,
     packages=find_packages(),
     data_files=[],
     include_package_data=True,
     url='https://https://github.com/MBHallgren/kmergenetyper',
     license='',
     install_requires=(),
     author='Malte B. Hallgren',
```

