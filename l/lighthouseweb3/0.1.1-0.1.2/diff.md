# Comparing `tmp/lighthouseweb3-0.1.1.tar.gz` & `tmp/lighthouseweb3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lighthouseweb3-0.1.1.tar", last modified: Wed May  3 07:55:34 2023, max compression
+gzip compressed data, was "lighthouseweb3-0.1.2.tar", last modified: Mon May 22 17:20:47 2023, max compression
```

## Comparing `lighthouseweb3-0.1.1.tar` & `lighthouseweb3-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:55:34.261839 lighthouseweb3-0.1.1/
--rw-rw-rw-   0        0        0    35562 2023-05-02 13:14:59.000000 lighthouseweb3-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     2569 2023-05-03 07:55:34.261839 lighthouseweb3-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2023-05-02 13:15:23.000000 lighthouseweb3-0.1.1/README.md
--rw-rw-rw-   0        0        0      113 2023-05-03 07:55:34.263279 lighthouseweb3-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1274 2023-05-03 07:55:12.000000 lighthouseweb3-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:55:34.233955 lighthouseweb3-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 07:55:34.238812 lighthouseweb3-0.1.1/src/lighthouseweb3/
--rw-rw-rw-   0        0        0     2192 2023-05-02 20:06:36.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:55:34.260533 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:14:59.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-02 13:15:23.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/axios.py
--rw-rw-rw-   0        0        0      351 2023-05-02 20:06:36.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/config.py
--rw-rw-rw-   0        0        0      435 2023-05-02 20:06:36.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/deal_status.py
--rw-rw-rw-   0        0        0      712 2023-05-02 20:06:36.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/get_uploads.py
--rw-rw-rw-   0        0        0     1020 2023-05-02 13:15:23.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/types.py
--rw-rw-rw-   0        0        0     2427 2023-05-02 13:15:23.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/upload.py
--rw-rw-rw-   0        0        0     2183 2023-05-02 13:15:23.000000 lighthouseweb3-0.1.1/src/lighthouseweb3/functions/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:55:34.251226 lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/
--rw-rw-rw-   0        0        0     2569 2023-05-03 07:55:34.000000 lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-05-03 07:55:34.000000 lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:55:34.000000 lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 07:55:34.000000 lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 07:55:34.000000 lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 17:20:47.512242 lighthouseweb3-0.1.2/
+-rw-rw-rw-   0        0        0    35562 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     2619 2023-05-22 17:20:47.512242 lighthouseweb3-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/README.md
+-rw-rw-rw-   0        0        0      113 2023-05-22 17:20:47.513474 lighthouseweb3-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-05-22 17:17:41.000000 lighthouseweb3-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:20:47.488055 lighthouseweb3-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 17:20:47.494849 lighthouseweb3-0.1.2/src/lighthouseweb3/
+-rw-rw-rw-   0        0        0     4600 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:20:47.510795 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/
+-rw-rw-rw-   0        0        0        0 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/axios.py
+-rw-rw-rw-   0        0        0      419 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/config.py
+-rw-rw-rw-   0        0        0      435 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/deal_status.py
+-rw-rw-rw-   0        0        0      712 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/get_uploads.py
+-rw-rw-rw-   0        0        0     1020 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/types.py
+-rw-rw-rw-   0        0        0     3073 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/upload.py
+-rw-rw-rw-   0        0        0     2183 2023-05-22 16:48:41.000000 lighthouseweb3-0.1.2/src/lighthouseweb3/functions/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:20:47.502469 lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/
+-rw-rw-rw-   0        0        0     2619 2023-05-22 17:20:47.000000 lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-05-22 17:20:47.000000 lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:20:47.000000 lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 17:20:47.000000 lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 17:20:47.000000 lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/top_level.txt
```

### Comparing `lighthouseweb3-0.1.1/LICENSE.md` & `lighthouseweb3-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.1/PKG-INFO` & `lighthouseweb3-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: lighthouseweb3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lighthouse Python SDK
 Home-page: https://github.com/lighthouse-web3/lighthouse-python-sdk
-Author: Ayobami Oki| Ravish Sharma | Perfection Loveday
-Author-email: ravish@lighthouse.storage
+Author: Ravish Sharma | Ayobami Oki | Nandit Mehra
+Author-email: nandit123@lighthouse.storage
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: lighthouse storage sdk python filecoin ipfs web3 perpetual
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Lighthouse Python SDK
 
 Lighthouse is a permanent decentralized file storage protocol that allows the ability to pay once and store forever. While traditionally, users need to repeatedly keep track and pay for their storage after every fixed amount of time, Lighthouse manages this for them and makes sure that user files are stored forever. The aim is to move users from a rent-based cost model where they are renting their own files on cloud storage to a permanent ownership model. It is built on top of IPFS, Filecoin, and Polygon. It uses the existing miner network and storage capacity of the filecoin network.
```

### Comparing `lighthouseweb3-0.1.1/README.md` & `lighthouseweb3-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.1/setup.py` & `lighthouseweb3-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 import pathlib
 from setuptools import setup, find_packages
 
 setup(
     name="lighthouseweb3",
-    version="0.1.1",
+    version="0.1.2",
     license="GNU GENERAL PUBLIC LICENSE",
     description="Lighthouse Python SDK",
-    author="Ayobami Oki| Ravish Sharma | Perfection Loveday",
-    author_email="ravish@lighthouse.storage",
+    author="Ravish Sharma | Ayobami Oki | Nandit Mehra",
+    author_email="nandit123@lighthouse.storage",
     url="https://github.com/lighthouse-web3/lighthouse-python-sdk",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=["requests"],
     python_requires=">=3.6",
     classifiers=[
         "License :: OSI Approved :: MIT License",
@@ -20,14 +20,15 @@
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="lighthouse storage sdk python filecoin ipfs web3 perpetual",
     long_description=(
         (pathlib.Path(__file__).parent.resolve()) / "README.md"
     ).read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
 )
```

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3/functions/axios.py` & `lighthouseweb3-0.1.2/src/lighthouseweb3/functions/axios.py`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3/functions/get_uploads.py` & `lighthouseweb3-0.1.2/src/lighthouseweb3/functions/get_uploads.py`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3/functions/types.py` & `lighthouseweb3-0.1.2/src/lighthouseweb3/functions/types.py`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3/functions/upload.py` & `lighthouseweb3-0.1.2/src/lighthouseweb3/functions/upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, List, Tuple
 from .axios import Axios
 from .utils import is_dir, walk_dir_tree, extract_file_name, NamedBufferedReader
 from .config import Config
 from . import types as t
 
 
-def upload(source: str | BufferedReader | NamedBufferedReader, token: str) -> t.Upload:
+def upload(source: str | BufferedReader | NamedBufferedReader, token: str, tag: str = "") -> t.Upload:
     """
     Deploy a file or directory to the lighthouse network
     @params {source}: str, path to file or directory
     @params {token}: str, lighthouse api token
     """
     # create headers
     headers = {
@@ -36,23 +36,32 @@
                 file_dict["is_dir"] = True
                 file_dict["path"] = root
             else:
                 # add file to list
                 file_dict["files"] = [source]
                 file_dict["is_dir"] = False
                 file_dict["path"] = source
-            return {"data": axios.post_files(file_dict, headers)}
+            hashData = axios.post_files(file_dict, headers)
         else:
-            return {"data": axios.post_blob(source, source.name, headers)}
+            hashData = axios.post_blob(source, source.name, headers)
+
+        if len(tag):
+            _axios = Axios(Config.lighthouse_api + "/api/user/create_tag")
+            data = _axios.post({
+                "tag": tag,
+                "cid": hashData.get("Hash")
+            }, {
+                "Authorization": f"Bearer {token}", })
+        return {"data": hashData}
     except Exception as e:
         print(e)
         raise e
 
 
-def uploadBlob(source:  BufferedReader, filename: str, token: str) -> t.Upload:
+def uploadBlob(source:  BufferedReader, filename: str, token: str, tag: str = "") -> t.Upload:
     """
     Upload a Buffer or readable Object
     @params {source}: str, path to file or directory
     @params {token}: str, lighthouse api token
     """
     # create headers
     headers = {
@@ -61,11 +70,20 @@
         "Encryption": "false",
         "Mime-Type": "application/octet-stream",
     }
     try:
         # create http object
         axios = Axios(Config.lighthouse_node + "/api/v0/add")
         # create list of files to upload
-        return {"data": axios.post_blob(source, filename, headers)}
+
+        hashData = axios.post_blob(source, filename, headers)
+        if len(tag):
+            _axios = Axios(Config.lighthouse_api + "/api/user/create_tag")
+            data = _axios.post({
+                "tag": tag,
+                "cid": hashData.get("Hash")
+            }, {
+                "Authorization": f"Bearer {token}", })
+        return {"data": hashData}
     except Exception as e:
         print(e)
         raise e
```

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3/functions/utils.py` & `lighthouseweb3-0.1.2/src/lighthouseweb3/functions/utils.py`

 * *Files identical despite different names*

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/PKG-INFO` & `lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: lighthouseweb3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lighthouse Python SDK
 Home-page: https://github.com/lighthouse-web3/lighthouse-python-sdk
-Author: Ayobami Oki| Ravish Sharma | Perfection Loveday
-Author-email: ravish@lighthouse.storage
+Author: Ravish Sharma | Ayobami Oki | Nandit Mehra
+Author-email: nandit123@lighthouse.storage
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: lighthouse storage sdk python filecoin ipfs web3 perpetual
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Lighthouse Python SDK
 
 Lighthouse is a permanent decentralized file storage protocol that allows the ability to pay once and store forever. While traditionally, users need to repeatedly keep track and pay for their storage after every fixed amount of time, Lighthouse manages this for them and makes sure that user files are stored forever. The aim is to move users from a rent-based cost model where they are renting their own files on cloud storage to a permanent ownership model. It is built on top of IPFS, Filecoin, and Polygon. It uses the existing miner network and storage capacity of the filecoin network.
```

### Comparing `lighthouseweb3-0.1.1/src/lighthouseweb3.egg-info/SOURCES.txt` & `lighthouseweb3-0.1.2/src/lighthouseweb3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

