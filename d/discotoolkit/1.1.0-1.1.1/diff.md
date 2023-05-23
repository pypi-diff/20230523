# Comparing `tmp/discotoolkit-1.1.0.tar.gz` & `tmp/discotoolkit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.1.0.tar", last modified: Fri May 19 09:04:08 2023, max compression
+gzip compressed data, was "discotoolkit-1.1.1.tar", last modified: Tue May 23 02:20:18 2023, max compression
```

## Comparing `discotoolkit-1.1.0.tar` & `discotoolkit-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-19 09:03:56.958628 discotoolkit-1.1.0/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.1.0/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-19 09:03:56.958628 discotoolkit-1.1.0/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     2618 2023-05-19 08:34:31.000000 discotoolkit-1.1.0/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-19 09:03:56.922628 discotoolkit-1.1.0/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    17688 2023-05-16 05:02:50.000000 discotoolkit-1.1.0/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.1.0/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.1.0/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     7361 2023-05-18 08:03:41.000000 discotoolkit-1.1.0/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     4372 2023-05-19 08:58:58.000000 discotoolkit-1.1.0/discotoolkit/GeneSearch.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.1.0/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.1.0/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      156 2023-05-19 08:34:53.000000 discotoolkit-1.1.0/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-19 09:03:56.950628 discotoolkit-1.1.0/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-19 09:03:56.000000 discotoolkit-1.1.0/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      431 2023-05-19 09:03:56.000000 discotoolkit-1.1.0/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-19 09:03:56.000000 discotoolkit-1.1.0/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      122 2023-05-19 09:03:56.000000 discotoolkit-1.1.0/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-19 09:03:56.000000 discotoolkit-1.1.0/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-19 09:03:56.962628 discotoolkit-1.1.0/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-05-19 08:34:14.000000 discotoolkit-1.1.0/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-23 02:20:06.683257 discotoolkit-1.1.1/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.1.1/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-23 02:20:06.679257 discotoolkit-1.1.1/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2618 2023-05-23 02:19:32.000000 discotoolkit-1.1.1/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-23 02:20:06.647257 discotoolkit-1.1.1/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    17809 2023-05-23 02:18:50.000000 discotoolkit-1.1.1/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.1.1/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.1.1/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     7361 2023-05-18 08:03:41.000000 discotoolkit-1.1.1/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     4372 2023-05-22 02:26:21.000000 discotoolkit-1.1.1/discotoolkit/GeneSearch.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.1.1/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.1.1/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      156 2023-05-23 02:19:38.000000 discotoolkit-1.1.1/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-23 02:20:06.675257 discotoolkit-1.1.1/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-23 02:20:06.000000 discotoolkit-1.1.1/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      431 2023-05-23 02:20:06.000000 discotoolkit-1.1.1/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-23 02:20:06.000000 discotoolkit-1.1.1/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      122 2023-05-23 02:20:06.000000 discotoolkit-1.1.1/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-23 02:20:06.000000 discotoolkit-1.1.1/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-23 02:20:06.683257 discotoolkit-1.1.1/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-05-23 02:19:26.000000 discotoolkit-1.1.1/setup.py
```

### Comparing `discotoolkit-1.1.0/PKG-INFO` & `discotoolkit-1.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.         It provides the following functions
```

### Comparing `discotoolkit-1.1.0/README.md` & `discotoolkit-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
 [![Documentation Status](https://readthedocs.org/projects/discotoolkit-py/badge/?version=latest)](https://discotoolkit-py.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/discotoolkit?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/discotoolkit) [![PyPI version](https://img.shields.io/pypi/v/discotoolkit)](https://pypi.org/project/discotoolkit)
 
-# DISCOtoolkit 1.1.0
+# DISCOtoolkit 1.1.1
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://discotoolkit-py.readthedocs.io/en/latest/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
```

### Comparing `discotoolkit-1.1.0/discotoolkit/CELLiD.py` & `discotoolkit-1.1.1/discotoolkit/CELLiD.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
             os.mkdir(ref_path)
         
         # check if the file does not exist
         if not (os.path.exists(ref_path + "/ref_geneset.pkl")):
             # downloading the geneset data from disco database
             response = requests.get(url=prefix_disco_url +"/getGeneSetPkl", timeout=timeout)
             open(ref_path + "/ref_geneset.pkl", "wb").write(response.content)
+            reference = pd.read_pickle(ref_path + "/ref_geneset.pkl", compression = {'method':'gzip','compresslevel':6})
 
         else:
             # read the data into pandas dataframe for subsequent analysis
             reference = pd.read_pickle(ref_path + "/ref_geneset.pkl", compression = {'method':'gzip','compresslevel':6})
 
     # rename the name data to include the reference atlas
     reference["name"] = reference["name"] + " in " + reference["atlas"]
```

### Comparing `discotoolkit-1.1.0/discotoolkit/DiscoClass.py` & `discotoolkit-1.1.1/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.0/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.1.1/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.0/discotoolkit/GeneSearch.py` & `discotoolkit-1.1.1/discotoolkit/GeneSearch.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.0/discotoolkit/GetMetadata.py` & `discotoolkit-1.1.1/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.0/discotoolkit/GlobalVariable.py` & `discotoolkit-1.1.1/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.1.0/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.1.1/discotoolkit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.         It provides the following functions
```

### Comparing `discotoolkit-1.1.0/setup.py` & `discotoolkit-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='discotoolkit',
-    version="1.1.0",
+    version="1.1.1",
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.16',
```

