# Comparing `tmp/dare_datasets-0.1.0.tar.gz` & `tmp/dare_datasets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dare_datasets-0.1.0.tar", max compression
+gzip compressed data, was "dare_datasets-0.1.2.tar", max compression
```

## Comparing `dare_datasets-0.1.0.tar` & `dare_datasets-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,8 @@
--rw-r--r--   0        0        0       18 2023-05-23 16:07:53.827473 dare_datasets-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:43:53.291198 dare_datasets-0.1.0/dare_datasets/__init__.py
--rw-r--r--   0        0        0     1956 2023-05-23 16:06:06.798116 dare_datasets-0.1.0/dare_datasets/dataset_abc.py
--rw-r--r--   0        0        0     1427 2023-05-23 16:09:11.956481 dare_datasets-0.1.0/dare_datasets/qr2t_benchmark.py
--rw-r--r--   0        0        0        0 2023-05-23 16:00:22.538021 dare_datasets-0.1.0/dare_datasets/utils/__init__.py
--rw-r--r--   0        0        0      695 2023-05-23 15:58:58.181106 dare_datasets-0.1.0/dare_datasets/utils/downloader.py
--rw-r--r--   0        0        0   145893 2023-05-23 15:44:28.381255 dare_datasets-0.1.0/dare_datasets/~/.cache/dare-datasets/QR2T_Benchmark/dev.json
--rw-r--r--   0        0        0   185820 2023-05-23 15:44:29.769275 dare_datasets-0.1.0/dare_datasets/~/.cache/dare-datasets/QR2T_Benchmark/eval.json
--rw-r--r--   0        0        0   586497 2023-05-23 15:44:31.705303 dare_datasets-0.1.0/dare_datasets/~/.cache/dare-datasets/QR2T_Benchmark/train.json
--rw-r--r--   0        0        0      349 2023-05-23 14:18:46.555219 dare_datasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 dare_datasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/__init__.py
+-rw-r--r--   0        0        0     1953 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/dataset_abc.py
+-rw-r--r--   0        0        0     1427 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/qr2t_benchmark.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      696 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/utils/downloader.py
+-rw-r--r--   0        0        0      406 2023-05-23 16:47:14.766549 dare_datasets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 dare_datasets-0.1.2/PKG-INFO
```

### Comparing `dare_datasets-0.1.0/dare_datasets/dataset_abc.py` & `dare_datasets-0.1.2/dare_datasets/dataset_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC, abstractmethod
 
-
 # Url of the FOLDER of the dataset in Google Drive. The folder must be publicly available.
 GDRIVE_URL = ""
 
 
 class Dataset(ABC):
     """
     Set of methods that every dataset should implement. Apart from these methods the class can
@@ -57,9 +56,7 @@
             {
                  "train":[],
                  "dev":[],
                  "test":[]
             }
         """
         pass
-
-
```

### Comparing `dare_datasets-0.1.0/dare_datasets/qr2t_benchmark.py` & `dare_datasets-0.1.2/dare_datasets/qr2t_benchmark.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 import json
 import os
 import typing
-
 from pathlib import Path
+
 from dare_datasets.dataset_abc import Dataset
 from dare_datasets.utils.downloader import get_file_from_gdrive
 
 GDRIVE_URL = "https://drive.google.com/drive/folders/1LCD4gObeX-PBxkNYNuZxSmrTBvzEK095?usp=sharing"
 DATASET_NAME = "QR2T_Benchmark"
```

### Comparing `dare_datasets-0.1.0/dare_datasets/utils/downloader.py` & `dare_datasets-0.1.2/dare_datasets/utils/downloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import gdown
 import glob
 import logging
 import os
-
 from pathlib import Path
+
+import gdown
+
 print()
 
 
 def get_file_from_gdrive(url: str, folder_name: str, cache_dir: str) -> None:
     cached_datasets = list(map(os.path.basename, glob.glob(f"{cache_dir}*")))
 
     if folder_name not in cached_datasets:  # Check if file is already downloaded in cache
```

