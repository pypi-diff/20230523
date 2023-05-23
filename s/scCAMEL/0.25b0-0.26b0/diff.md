# Comparing `tmp/scCAMEL-0.25b0.tar.gz` & `tmp/scCAMEL-0.26b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCAMEL-0.25b0.tar", last modified: Tue May 23 10:18:32 2023, max compression
+gzip compressed data, was "scCAMEL-0.26b0.tar", last modified: Tue May 23 10:53:45 2023, max compression
```

## Comparing `scCAMEL-0.25b0.tar` & `scCAMEL-0.26b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:32.596347 scCAMEL-0.25b0/
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    34870 2023-05-23 10:09:37.000000 scCAMEL-0.25b0/LICENSE.txt
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:18:32.588348 scCAMEL-0.25b0/PKG-INFO
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      298 2022-11-01 09:55:19.000000 scCAMEL-0.25b0/README.md
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       86 2022-07-05 13:12:44.000000 scCAMEL-0.25b0/pyproject.toml
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       38 2023-05-23 10:18:32.598347 scCAMEL-0.25b0/setup.cfg
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      961 2023-05-23 10:10:33.000000 scCAMEL-0.25b0/setup.py
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:31.786799 scCAMEL-0.25b0/src/
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:32.256342 scCAMEL-0.25b0/src/scCAMEL/
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    62722 2023-04-18 10:06:59.000000 scCAMEL-0.25b0/src/scCAMEL/CamelEvo.py
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    56615 2023-04-18 09:44:23.000000 scCAMEL-0.25b0/src/scCAMEL/CamelPrefiltering.py
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)   121627 2023-04-18 09:29:24.000000 scCAMEL-0.25b0/src/scCAMEL/CamelSwapline.py
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      125 2022-10-31 11:06:46.000000 scCAMEL-0.25b0/src/scCAMEL/__init__.py
-drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:32.520344 scCAMEL-0.25b0/src/scCAMEL.egg-info/
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/PKG-INFO
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      295 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/SOURCES.txt
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        1 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/dependency_links.txt
--rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        8 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/top_level.txt
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:45.178655 scCAMEL-0.26b0/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    34870 2023-05-23 10:09:37.000000 scCAMEL-0.26b0/LICENSE.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:53:45.170656 scCAMEL-0.26b0/PKG-INFO
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      298 2022-11-01 09:55:19.000000 scCAMEL-0.26b0/README.md
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       86 2022-07-05 13:12:44.000000 scCAMEL-0.26b0/pyproject.toml
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       38 2023-05-23 10:53:45.181654 scCAMEL-0.26b0/setup.cfg
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      952 2023-05-23 10:53:19.000000 scCAMEL-0.26b0/setup.py
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:44.369352 scCAMEL-0.26b0/src/
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:44.830355 scCAMEL-0.26b0/src/scCAMEL/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    62722 2023-04-18 10:06:59.000000 scCAMEL-0.26b0/src/scCAMEL/CamelEvo.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    56615 2023-04-18 09:44:23.000000 scCAMEL-0.26b0/src/scCAMEL/CamelPrefiltering.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)   121678 2023-05-23 10:32:37.000000 scCAMEL-0.26b0/src/scCAMEL/CamelSwapline.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      125 2022-10-31 11:06:46.000000 scCAMEL-0.26b0/src/scCAMEL/__init__.py
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:53:45.098357 scCAMEL-0.26b0/src/scCAMEL.egg-info/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:53:43.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/PKG-INFO
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      295 2023-05-23 10:53:44.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        1 2023-05-23 10:53:43.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        8 2023-05-23 10:53:43.000000 scCAMEL-0.26b0/src/scCAMEL.egg-info/top_level.txt
```

### Comparing `scCAMEL-0.25b0/LICENSE.txt` & `scCAMEL-0.26b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scCAMEL-0.25b0/PKG-INFO` & `scCAMEL-0.26b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCAMEL
-Version: 0.25b0
+Version: 0.26b0
 Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
 Home-page: https://sccamel.readthedocs.io/
 Author: Yizhou Hu
 Author-email: yizhou.hu@ki.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scCAMEL-0.25b0/setup.py` & `scCAMEL-0.26b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scCAMEL",
-    version="0.25b",
+    version="0.26b",
     author="Yizhou Hu",
     author_email="yizhou.hu@ki.se",
     description="scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sccamel.readthedocs.io/",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: Microsoft :: Windows",
+'Operating System :: Microsoft :: Windows'
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `scCAMEL-0.25b0/src/scCAMEL/CamelEvo.py` & `scCAMEL-0.26b0/src/scCAMEL/CamelEvo.py`

 * *Files identical despite different names*

### Comparing `scCAMEL-0.25b0/src/scCAMEL/CamelPrefiltering.py` & `scCAMEL-0.26b0/src/scCAMEL/CamelPrefiltering.py`

 * *Files identical despite different names*

### Comparing `scCAMEL-0.25b0/src/scCAMEL/CamelSwapline.py` & `scCAMEL-0.26b0/src/scCAMEL/CamelSwapline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1700,31 +1700,31 @@
     ax = plt.gca()
     for art in ax.get_children():
         if isinstance(art, PolyCollection):
             art.set_edgecolor((0.6, 0.6, 0.6))
 
 def ProbMultiPlot( datax, mcolor_dict,fs=15):
 
-    """
-    Input:
+     """
+        Input:
 
-    datax: AnnData object
-    mcolor_dict: dictionary containing color values for each cell type
-    fs: font size for plot labels
-    Output:
+        datax: AnnData object
+        mcolor_dict: dictionary containing color values for each cell type
+        fs: font size for plot labels
+        Output:
 
-    fig: matplotlib figure object
-    Functionality:
-    This function generates a violin plot of the probability of cell type similarity for each cell in the dataset,
-     along with a scatter plot of the same data points. The violin plot shows the distribution of the probability of similarity for each cell type, while the scatter plot shows the actual values for each cell.
-     The color of each data point in the scatter plot corresponds to the cell type of the cell. The function also adds a legend to the plot showing the color-coding for each cell type.
-    The function returns the generated matplotlib figure object.
-    """
+        fig: matplotlib figure object
+        Functionality:
+        This function generates a violin plot of the probability of cell type similarity for each cell in the dataset,
+         along with a scatter plot of the same data points. The violin plot shows the distribution of the probability of similarity for each cell type, while the scatter plot shows the actual values for each cell.
+         The color of each data point in the scatter plot corresponds to the cell type of the cell. The function also adds a legend to the plot showing the color-coding for each cell type.
+        The function returns the generated matplotlib figure object.
+     """
      #dfprobRef, dfpfcclus, mwanted_order, mcolor_dict
-#dfprobRef=dfprobRef, dfpfcclus=dfpfcclus, mwanted_order=mwanted_order,
+     #dfprobRef=dfprobRef, dfpfcclus=dfpfcclus, mwanted_order=mwanted_order,
                   # mcolor_dict=refcolor_dict
      mcolor_dict=pd.Series(mcolor_dict)
      mcolor_dict = mcolor_dict.map(lambda x: list(map(lambda y: y / 255., x)))
      dfprobRef = pd.DataFrame(datax.obsm["Celltype_Score"], index=datax.obs.index,
                               columns=datax.uns["Celltype_Score_RefCellType"])
      dfpfcclus = datax.obs[["mtrain_index", "Cluster"]].T
      mwanted_order = datax.uns["mwanted_order"]
```

### Comparing `scCAMEL-0.25b0/src/scCAMEL.egg-info/PKG-INFO` & `scCAMEL-0.26b0/src/scCAMEL.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCAMEL
-Version: 0.25b0
+Version: 0.26b0
 Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
 Home-page: https://sccamel.readthedocs.io/
 Author: Yizhou Hu
 Author-email: yizhou.hu@ki.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
```

