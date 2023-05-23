# Comparing `tmp/mlbi_at_dku_lib-0.1.1.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.1.tar", last modified: Tue May 23 01:54:36 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.2.tar", last modified: Tue May 23 02:14:41 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.1.tar` & `mlbi_at_dku_lib-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.1/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.1/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.1/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    32541 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      422 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2725 2023-05-23 01:49:57.000000 mlbi_at_dku_lib-0.1.1/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.1/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 02:14:41.114926 mlbi_at_dku_lib-0.1.2/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.2/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.2/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 02:14:41.114926 mlbi_at_dku_lib-0.1.2/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.2/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 02:14:41.114926 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    32652 2023-05-23 02:13:51.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 02:14:41.114926 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 02:14:40.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      422 2023-05-23 02:14:41.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 02:14:40.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-05-23 02:14:40.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-05-23 02:14:40.000000 mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-05-23 02:14:41.114926 mlbi_at_dku_lib-0.1.2/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2725 2023-05-23 02:13:39.000000 mlbi_at_dku_lib-0.1.2/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 02:14:41.114926 mlbi_at_dku_lib-0.1.2/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.2/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.1/LICENSE` & `mlbi_at_dku_lib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.1/PKG-INFO` & `mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mlbi_at_dku_lib
-Version: 0.1.1
+Name: mlbi-at-dku-lib
+Version: 0.1.2
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.2/mlbi_at_dku_lib/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     fig.show()   
     return
 
 
 ### Example 
 # df_cnt, df_pct= get_population( adata_s.obs['sid'], 
 #                                 adata_s.obs['minor'], sort_by = [] )
-# plot_population(df_pct, figsize=(6, 4), dpi = 80)
+# plot_population(df_pct, figsize=(6, 4), dpi = 80, return_fig = False)
 # df_cnt
     
 def get_population( pids, cts, sort_by = [] ):
     
     pid_lst = list(set(list(pids)))
     pid_lst.sort()
     celltype_lst = list(set(list(cts)))
@@ -180,19 +180,24 @@
     
     if len(sort_by) > 0:
         df_celltype_pct.sort_values(by = sort_by, inplace = True)
 
     return df_celltype_cnt, df_celltype_pct
 
 
-def plot_population(df_celltype_pct, figsize=(5, 3), dpi = 80):    
-    sc.settings.set_figure_params(figsize=figsize, dpi=dpi, facecolor='white')
+def plot_population(df_celltype_pct, figsize=(5, 3), dpi = 80, return_fig = False):    
+
+    # sc.settings.set_figure_params(figsize=figsize, dpi=dpi, facecolor='white')
     ax = df_celltype_pct.plot.bar(stacked = True, rot = 90)
     ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=(1, 1) )
-    plt.show()
+    if return_fig:
+        return ax
+    else:
+        plt.show()
+        return
     return
 
 def plot_composition_bar( adata_t,  pid_field = 'pid', cell_type_field = 'cell_type_major_pred',
                           sort_by = [] ):
     
     pid_lst = list(adata_t.obs[pid_field].unique())
 
@@ -211,15 +216,15 @@
             df_celltype_cnt.loc[pid, ct] = np.sum(bx)
 
     df_celltype_pct = df_celltype_cnt.div(df_celltype_cnt.sum(axis = 1), axis = 0)*100
     
     if len(sort_by) > 0:
         df_celltype_pct.sort_values(by = sort_by, inplace = True)
 
-    sc.settings.set_figure_params(figsize=(5, 3), dpi=80, facecolor='white')
+    # sc.settings.set_figure_params(figsize=(5, 3), dpi=80, facecolor='white')
     ax = df_celltype_pct.plot.bar(stacked = True, rot = 90)
     ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=(1, 1) )
     
     return df_celltype_cnt
 
 
 ### DigitalCellSorter
```

### Comparing `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mlbi-at-dku-lib
-Version: 0.1.1
+Name: mlbi_at_dku_lib
+Version: 0.1.2
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.1/setup.py` & `mlbi_at_dku_lib-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.1',
+    version             = '0.1.2',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

