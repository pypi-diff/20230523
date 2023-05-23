# Comparing `tmp/scCAMEL-0.24b0.tar.gz` & `tmp/scCAMEL-0.25b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCAMEL-0.24b0.tar", last modified: Tue Feb  7 14:42:09 2023, max compression
+gzip compressed data, was "scCAMEL-0.25b0.tar", last modified: Tue May 23 10:18:32 2023, max compression
```

## Comparing `scCAMEL-0.24b0.tar` & `scCAMEL-0.25b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 14:42:09.736970 scCAMEL-0.24b0/
--rw-rw-rw-   0        0        0    34870 2022-10-31 11:12:14.000000 scCAMEL-0.24b0/LICENSE.txt
--rw-rw-rw-   0        0        0      983 2023-02-07 14:42:09.736970 scCAMEL-0.24b0/PKG-INFO
--rw-rw-rw-   0        0        0      298 2022-11-01 09:55:19.000000 scCAMEL-0.24b0/README.md
--rw-rw-rw-   0        0        0       86 2022-07-05 13:12:44.000000 scCAMEL-0.24b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-07 14:42:09.736970 scCAMEL-0.24b0/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-02-07 14:41:11.000000 scCAMEL-0.24b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-07 14:42:09.687016 scCAMEL-0.24b0/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 14:42:09.727024 scCAMEL-0.24b0/src/scCAMEL/
--rw-rw-rw-   0        0        0    52333 2023-02-06 14:25:53.000000 scCAMEL-0.24b0/src/scCAMEL/CamelEvo.py
--rw-rw-rw-   0        0        0    39037 2023-02-07 14:37:20.000000 scCAMEL-0.24b0/src/scCAMEL/CamelPrefiltering.py
--rw-rw-rw-   0        0        0    89606 2023-01-11 15:43:39.000000 scCAMEL-0.24b0/src/scCAMEL/CamelSwapline.py
--rw-rw-rw-   0        0        0      125 2022-10-31 11:06:46.000000 scCAMEL-0.24b0/src/scCAMEL/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-07 14:42:09.736970 scCAMEL-0.24b0/src/scCAMEL.egg-info/
--rw-rw-rw-   0        0        0      983 2023-02-07 14:42:09.000000 scCAMEL-0.24b0/src/scCAMEL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-02-07 14:42:09.000000 scCAMEL-0.24b0/src/scCAMEL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 14:42:09.000000 scCAMEL-0.24b0/src/scCAMEL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-07 14:42:09.000000 scCAMEL-0.24b0/src/scCAMEL.egg-info/top_level.txt
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:32.596347 scCAMEL-0.25b0/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    34870 2023-05-23 10:09:37.000000 scCAMEL-0.25b0/LICENSE.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:18:32.588348 scCAMEL-0.25b0/PKG-INFO
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      298 2022-11-01 09:55:19.000000 scCAMEL-0.25b0/README.md
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       86 2022-07-05 13:12:44.000000 scCAMEL-0.25b0/pyproject.toml
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)       38 2023-05-23 10:18:32.598347 scCAMEL-0.25b0/setup.cfg
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      961 2023-05-23 10:10:33.000000 scCAMEL-0.25b0/setup.py
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:31.786799 scCAMEL-0.25b0/src/
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:32.256342 scCAMEL-0.25b0/src/scCAMEL/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    62722 2023-04-18 10:06:59.000000 scCAMEL-0.25b0/src/scCAMEL/CamelEvo.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)    56615 2023-04-18 09:44:23.000000 scCAMEL-0.25b0/src/scCAMEL/CamelPrefiltering.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)   121627 2023-04-18 09:29:24.000000 scCAMEL-0.25b0/src/scCAMEL/CamelSwapline.py
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      125 2022-10-31 11:06:46.000000 scCAMEL-0.25b0/src/scCAMEL/__init__.py
+drwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        0 2023-05-23 10:18:32.520344 scCAMEL-0.25b0/src/scCAMEL.egg-info/
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      960 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/PKG-INFO
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)      295 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        1 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 huyiz     (1000) huyiz     (1000)        8 2023-05-23 10:18:31.000000 scCAMEL-0.25b0/src/scCAMEL.egg-info/top_level.txt
```

### Comparing `scCAMEL-0.24b0/LICENSE.txt` & `scCAMEL-0.25b0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 GPLv3 License
 
-Copyright (c) [2022] [YIZHOU HU]
+Copyright (c) [2023] [YIZHOU HU]
 
 GNU GENERAL PUBLIC LICENSE
 Version 3, 29 June 2007
 
 Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
 
 Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
```

### Comparing `scCAMEL-0.24b0/PKG-INFO` & `scCAMEL-0.25b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: scCAMEL
-Version: 0.24b0
-Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
-Home-page: https://sccamel.readthedocs.io/
-Author: Yizhou Hu
-Author-email: yizhou.hu@ki.se
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory
-
-License: GPL version 3
-https://pypi.org/project/scCAMEL/
-
-Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet
-
-Tutorials and other informations in :
-https://sccamel.readthedocs.io/
+Metadata-Version: 2.1
+Name: scCAMEL
+Version: 0.25b0
+Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
+Home-page: https://sccamel.readthedocs.io/
+Author: Yizhou Hu
+Author-email: yizhou.hu@ki.se
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory
+
+License: GPL version 3
+https://pypi.org/project/scCAMEL/
+
+Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet
+
+Tutorials and other informations in :
+https://sccamel.readthedocs.io/
```

### Comparing `scCAMEL-0.24b0/setup.py` & `scCAMEL-0.25b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scCAMEL",
-    version="0.24b",
+    version="0.25b",
     author="Yizhou Hu",
     author_email="yizhou.hu@ki.se",
     description="scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sccamel.readthedocs.io/",
     classifiers=[
```

### Comparing `scCAMEL-0.24b0/src/scCAMEL/CamelEvo.py` & `scCAMEL-0.25b0/src/scCAMEL/CamelEvo.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,19 +20,17 @@
 import torch.nn.functional as F
 import math
 #import gpytorch
 import logging
 import datetime
 from scipy import sparse
 import numpy as np
-import pandas as pd
 import seaborn as sns
 from sklearn.decomposition import PCA
 from sklearn.cross_decomposition import CCA
-import pandas as pd
 import os.path
 from arboreto.utils import load_tf_names
 from arboreto.algo import grnboost2
 from distributed import LocalCluster, Client
 from kneed import KneeLocator
 import scanpy as sc
 import matplotlib.patches as patches
@@ -50,16 +48,14 @@
 
 import scipy.cluster.hierarchy as sch
 import matplotlib.pyplot as plt
 import numpy as np
 import matplotlib.cm as cm
 import matplotlib
 from matplotlib.lines import Line2D
-import numpy as np
-import pandas as pd
 import seaborn as sns
 from scipy.spatial import distance
 from scipy.cluster import hierarchy
 import matplotlib.patches as patches
 from matplotlib import pyplot as plt
 from matplotlib.path import Path
 
@@ -351,14 +347,27 @@
     if figsavename != None:
         plt.savefig(figsavename, bbox_inches='tight')
     else:
         plt.show()
     # fig, ax
 
 def PCAesti(adatax,ReadyModel=None):
+    """
+    Input:
+    adatax: AnnData object containing raw expression data and PCA coordinates.
+    ReadyModel: PCA model object (optional)
+    Output:
+    adatax: AnnData object with updated PCA coordinates and explained variance ratio.
+    PCAmodel: PCA model object (optional)
+    Function description:
+    This function performs principal component analysis (PCA) on the input AnnData object containing raw expression data and PCA coordinates.
+    If a pre-existing PCA model is provided, the function applies the model to the input data instead of creating a new model.
+     The function returns the updated AnnData object with the new PCA coordinates and explained variance ratio.
+    Additionally, if a new PCA model is created, the function also returns the PCA model object.
+    """
     X =adatax.obsm["PCAraw0"]
     if ReadyModel==None:
         pca_ = PCA(n_components=adatax.obsm["PCAraw0"].shape[1]-1, svd_solver='arpack', random_state=0)
         PCAmodel= pca_.fit(X)
         #X_cca,Y_cca=cca_.fit_transform(X,Y)
         X_pcavalue=PCAmodel.transform(X)
         adatax.obsm['Celltype_ScoreAll']=X_pcavalue
@@ -384,14 +393,38 @@
 
 from scipy import sparse
 import scipy
 
 
 def FindGenePatterns(adata, celltypelabel="Cluster", corrThre=0.3, ThreNumber=2,
                       TopWeightedFilter=False, DatasetName=None, filelist=None, plotfig=False):
+
+    """
+    Inputs:
+
+    adata: AnnData object containing gene expression data
+    celltypelabel: string, the column name for cell type annotation
+    corrThre: float, correlation threshold for selecting associated genes
+    ThreNumber: int, the minimum number of associated genes for each gene pattern
+    TopWeightedFilter: boolean, whether to filter associated gene patterns based on the top-weighted genes in other datasets
+    DatasetName: list of dataset names used for the TopWeightedFilter
+    filelist: list of file paths containing gene expression data for the TopWeightedFilter
+    plotfig: boolean, whether to plot the dendrogram for hierarchical clustering
+    Outputs:
+
+    adataGP: AnnData object containing gene expression data of the selected associated gene patterns
+    Functionality:
+
+    Selects the signature genes from each cell type using Wilcoxon rank-sum test
+    Calculates associated genes based on Spearman correlation coefficient
+    Hierarchical clustering to group associated genes into gene patterns
+    Filters gene patterns based on the number of associated genes and top-weighted genes in other datasets if TopWeightedFilter is True
+    Returns a new AnnData object containing gene expression data of the selected associated gene patterns.
+    The var attribute of the new AnnData object contains additional information about gene clusters and whether a gene pattern has been filtered.
+    """
     if type(adata.X) == sparse.csr.csr_matrix:
         adata.X = adata.X.toarray()
     adata1 = adata[:, adata.X.T.sum(1) > 0]
     df_dev = pd.DataFrame(adata1.X.T, index=adata1.var.index, columns=adata1.obs.index)
     dfpfcclus = pd.DataFrame(adata1.obs[celltypelabel].values, index=adata1.obs.index, columns=[celltypelabel]).T
     logging.info('Camel_Evo...Running: select the signature genes from each cell types....')
     sc.tl.rank_genes_groups(adata1, celltypelabel, method='wilcoxon')
@@ -483,14 +516,28 @@
     return adataGP
 
 
 import os.path
 
 
 def GRN_TFscore(df_dev, GRNgenes):
+    """
+    Input:
+    df_dev: Pandas DataFrame object containing expression values for genes in the dataset. Rows correspond to genes and columns correspond to cells.
+    GRNgenes: list of gene names to be used as input for calculating the GRN score.
+    Output:
+
+    TFscore: numpy array of length equal to the number of cells in the dataset, containing the GRN score for the input gene list.
+    Functionality:
+
+    This function calculates the GRN score for a list of genes,
+    which represents the expression level of these genes normalized by the average expression level of a set of control genes.
+    The function first divides the cells into bins based on their average expression level and then randomly selects control genes from each bin.
+    The GRN score is calculated as the mean expression level of the input genes minus the mean expression level of the control genes.
+    """
     var_names = df_dev.index
     gene_list = GRNgenes
 
     obs_avg = df_dev.mean(1)
     obs_avg = obs_avg[np.isfinite(obs_avg)]
     n_items = int(np.round(len(obs_avg) / 50))
     obs_cut = obs_avg.rank(method='min') // n_items
@@ -510,14 +557,37 @@
 
 def FindTFassociatedGP(adata, tf_filepath=None,
                        N_CPU=2, N_memory=16e9, N_threads=1,
                        filepath=None,
                        TFtoGeneFile=None,
                        TFassociatedGeneFile="TF-Top100Targets.csv",
                        plotfig=True):
+
+    """
+    Inputs:
+    adata: AnnData object
+    tf_filepath: path to the file containing list of transcription factors
+    N_CPU: integer, number of CPUs to use for GRN inference
+    N_memory: integer, amount of memory to allocate for GRN inference
+    N_threads: integer, number of threads to use for GRN inference
+    filepath: path to the directory to save the results
+    TFtoGeneFile: name of the file to save TF-associated gene network
+    TFassociatedGeneFile: name of the file to save TF-associated gene patterns
+    plotfig: boolean, whether to plot a figure
+    Outputs:
+    adataTF: AnnData object, containing TF-associated gene patterns
+    Functionality:
+
+    Reads the adata object and assigns X to a dataframe
+    Reads the file containing list of transcription factors or performs GRN inference to obtain the network
+    Filters the network to only include important transcription factors
+    Calculates the score of TF-associated gene patterns for each transcription factor
+    Saves the TF-associated gene patterns to a file
+    Returns the AnnData object containing TF-associated gene patterns
+    """
     df_dev = pd.DataFrame(adata.X.T, index=adata.var.index, columns=adata.obs.index)
     TFtoGeneFilePath = filepath + TFtoGeneFile
     if os.path.isfile(TFtoGeneFilePath):
         print('CamelEvo...Running: TFtoGene File is ready, reading.....')
         network = pd.read_table(TFtoGeneFilePath, index_col=0, header=0, sep=",")
     else:
         logging.info('CamelEvo...Running: TF associated genes, will take hours.....')
@@ -602,14 +672,28 @@
     return adataTF
 
 
 
 def SpeciesTFgenePatternsRaw(adata, fontsizeWeight=0.65, clusterlist=None,
                            filepath="/Yizhou_KI_OneCloud/OneDrive - Karolinska Institutet/Datasets_Template/scCamel_result_files/",
                           savefig="SpeciesTFgenePatterns.png"):
+    """
+    Inputs:
+    adata: AnnData object containing gene expression data and cluster annotations.
+    fontsizeWeight: float, optional. Font size for the plot.
+    clusterlist: list or array-like object, optional. List of cluster names to include in the plot.
+    filepath: str, optional. Path to save the figure.
+    savefig: str or None, optional. If not None, saves the figure with the given file name.
+    The function generates a heatmap plot of gene expression patterns for each cluster, either for all clusters or for a subset of clusters based on the clusterlist argument.
+    Functionality:
+    This function takes an AnnData object with gene expression data and cluster annotations and generates a heatmap plot of gene expression patterns for each cluster.
+    The plot shows the average gene expression levels across all cells in each cluster.
+    The user can choose to include all clusters or a subset of clusters using the clusterlist argument.
+    The plot is saved to file if a file name is provided in the savefig argument.
+    """
     dfregscore=pd.DataFrame(adata.X)
     dfregscore.index=adata.obs.index
     dfregscore.columns=adata.var.index
     dfregscore=dfregscore.join(adata.obs["Cluster"],how="inner")
     dfscore=dfregscore.groupby(["Cluster"]).mean()
     if clusterlist==None:
         plt.figure(figsize=(int(dfscore.shape[1]/4.5),int(dfscore.shape[0]/4.5)))
@@ -645,14 +729,29 @@
             savefile=filepath+savefig
             plt.savefig(savefile)
 
 
 def SpeciesTFgenePatterns(adata, fontsizeWeight=0.65, clusterlist=None, tfindex=None,
                            filepath="/Yizhou_KI_OneCloud/OneDrive - Karolinska Institutet/Datasets_Template/scCamel_result_files/",
                            savefig="SpeciesTFgenePatterns.png"):
+    """
+    Input:
+    adata: AnnData object containing gene expression data.
+    fontsizeWeight: float indicating the font size of the plot.
+    clusterlist: list of strings containing cluster IDs for subsetting the data. Default is None.
+    tfindex: list of strings containing gene names to be included in the plot. Default is None.
+    filepath: string indicating the path where the plot will be saved. Default is "/Yizhou_KI_OneCloud/OneDrive - Karolinska Institutet/Datasets_Template/scCamel_result_files/".
+    savefig: string indicating the name of the file where the plot will be saved. Default is "SpeciesTFgenePatterns.png".
+    Functionality:
+    This function creates a heatmap of gene expression patterns for species-specific transcription factors (TFs).
+     The gene expression data is extracted from the adata object and processed to generate a dataframe containing mean gene expression values for each TF across all clusters.
+     The resulting dataframe is clustered using hierarchical clustering based on correlation distance. The resulting heatmap includes rows for each TF and columns for each cluster.
+     The rows and columns are colored by species of origin and the color scheme is defined by the lut dictionary.
+    The heatmap can be subsetted using the clusterlist and tfindex parameters, and the resulting plot can be saved to a file using the filepath and savefig parameters.
+    """
     dfregscore = pd.DataFrame(adata.X)
     dfregscore.index = adata.obs.index
     dfregscore.columns = adata.var.index
 
     dfregscore = dfregscore.join(adata.obs["Cluster"], how="inner")
     dfscore = dfregscore.groupby(["Cluster"]).mean()
     clist = []
@@ -772,14 +871,32 @@
                     ncol=6, prop={'size': int(dfscore.shape[0] / 4.5)})
             if savefig != None:
                 savefile = filepath + savefig
                 plt.savefig(savefile, bbox_inches='tight')
 
 
 def MergeObjectValue(DatasetName, filelist,filepath):
+
+    """
+
+    Inputs:
+    DatasetName: a list of unique dataset names.
+    filelist: a list of filenames, where each filename contains the dataset name as its prefix.
+    filepath: the directory path where the data files are located.
+    Outputs:
+
+    adatax: a merged AnnData object that combines the data from all input files.
+    Functionality:
+    This function merges multiple AnnData objects by dataset name.
+    It iterates over each unique dataset name in the input list, and reads in all files that have that dataset name as its prefix.
+    It then concatenates these files together and generates a new AnnData object. For each dataset,
+    it also calculates a gene expression matrix by summing the expression counts across cells and normalizing by the total number of cells in which each gene is expressed.
+    It also adds a new column to the obs dataframe, called "Dataset",
+     which indicates which dataset each cell belongs to. Finally, it returns the merged AnnData object.
+    """
     for jname in set(DatasetName):
         xcount=0
         for item in filelist:
             if item.split("_")[0]==jname:
                 if xcount==0:
                     tempname="sc%s"%(jname)
                     vars()[tempname] = anndata.read(filepath+item)
@@ -828,14 +945,29 @@
 
 
 def pandas_plot(df):
     pass
 
 
 def ConservedCellTypePlot(dataref, dataz, datas, threshold, FigName=None):
+    """
+    Inputs:
+    dataref: an AnnData object containing the reference dataset.
+    dataz: an AnnData object containing the dataset to be compared to the reference.
+    datas: an AnnData object containing the second dataset to be compared to the reference.
+    threshold: a float specifying the minimum weight required to show a connection in the plot.
+    FigName: a string specifying the name of the file to save the figure (optional).
+    Output: None
+
+    Functionality:
+    This function creates a Sankey diagram comparing the cell types between dataref, dataz, and datas.
+    The weight of each connection represents the fraction of cells assigned to a particular cell type in dataz and datas that are assigned to a particular cell type in dataref.
+    The resulting plot shows the connections between cell types across the three datasets. The threshold parameter controls the minimum weight required for a connection to be shown in the plot.
+    If specified, the plot can be saved to a file with the name specified by FigName.
+    """
     dfc = dataref.obs.groupby(["Cluster", "Assigned_Celltype"]).count()
     dfmean = dfc / dataref.obs.groupby(["Cluster"]).count()
     dfnew = dfmean
     dfz = dfnew.loc[set(dataz.obs["Cluster"])]
     dfz["OriCluster"] = dfz.index.get_level_values(0)
     dfz["AssignedCluster"] = dfz.index.get_level_values(1)
     dfz1 = pd.pivot_table(dfz, values='color', index=['AssignedCluster'], columns='OriCluster').reindex(
@@ -896,14 +1028,28 @@
 
 # Location of bounds (if a phase is drawn from 0 to 1).
 LEFT = .1
 RIGHT = .9
 
 
 def MergeObject(DatasetName, filelist,filepath):
+    """
+    Inputs:
+    DatasetName: a list of strings representing unique names for each dataset.
+    filelist: a list of strings representing filenames of datasets to be merged.
+    filepath: a string representing the file path of the datasets.
+    Outputs:
+    adatax: an AnnData object that is the merged dataset.
+    Functionality:
+
+    The function merges multiple datasets into one by concatenating them along the samples axis.
+    It first reads in each dataset using the read() function of the AnnData object.
+    It then concatenates the datasets using the concat() function of the AnnData object.
+    It adds a new "Dataset" column to the .obs attribute of the merged dataset to indicate which dataset each sample belongs to.
+    """
     for jname in set(DatasetName):
         xcount=0
         for item in filelist:
             if item.split("_")[0]==jname:
                 if xcount==0:
                     tempname="sc%s"%(jname)
                     vars()[tempname] = anndata.read(filepath+item)
@@ -924,14 +1070,28 @@
 
 
 
 def DrawFlow(start, end, width, left, right, color):
     """
     Draw a single flow, from "left" to "right", with y going from "start" to
     "end", width "width" and color "color".
+    Input:
+
+    start: float
+    end: float
+    width: float
+    left: float
+    right: float
+    color: str
+    Output: None
+
+    Functionality:
+
+    Draws a single flow with specified start and end points, width, and color using a Path object and adds it to the current axis.
+     The flow is curved at the top and bottom, with the width increasing from the start to the middle, and decreasing from the middle to the end.
     """
     space = right - left
 
     verts = np.zeros(shape=(9, 2), dtype='float')
     verts[:, 1] = start
     verts[2:6, 1] = end
     verts[4:, 1] += width
@@ -967,14 +1127,36 @@
     return node_sizes.format(label=start, size=size)
 
 
 def EvoTreePlot(adatax, ConnFeature="connectivities", color_thresholdValue=5, methodvalue="average",
                 metricvalue='correlation',
                 fontsize=20, figsize=[10, 10], pallete="gist_rainbow", addlabels=True, figname="202210Treeplot.svg",
                 sample_classes=None, colorlabels=None, colorlabels_legend=None):
+    """
+    Inputs:
+    adatax: AnnData object containing the gene expression data and clustering information.
+    ConnFeature: Connectivity feature used to calculate the distance matrix (default: "connectivities").
+    color_thresholdValue: Threshold for coloring clusters in the dendrogram (default: 5).
+    methodvalue: Method used for hierarchical clustering (default: "average").
+    metricvalue: Distance metric used for hierarchical clustering (default: "correlation").
+    fontsize: Font size for the plot (default: 20).
+    figsize: Figure size for the plot (default: [10, 10]).
+    pallete: Color palette used for coloring the clusters (default: "gist_rainbow").
+    addlabels: Whether to add labels to the dendrogram (default: True).
+    figname: File name for saving the figure (default: "202210Treeplot.svg").
+    sample_classes: List of sample classes used for coloring the data points (default: None).
+    colorlabels: List of labels for coloring the data points (default: None).
+    colorlabels_legend: Title for the legend of the color labels (default: None).
+
+    Functionality:
+    This function takes an AnnData object containing gene expression data and clustering information and
+    creates a dendrogram plot of the hierarchical clustering. It uses a connectivity feature to calculate the distance matrix
+     and applies hierarchical clustering using the specified method and metric. The resulting dendrogram is colored based on the specified threshold and a color palette,
+    and the data points can be colored based on sample classes and color labels. The plot can be saved with the specified file name.
+    """
     dfdist = pd.DataFrame(adatax.obsp[ConnFeature].toarray())
     dfdist.index = adatax.obs.index
     dfdist.columns = adatax.obs.index
     dfdist["Cluster"] = adatax.obs["Cluster"]
     dfdist2 = dfdist.groupby(["Cluster"]).mean().T
     dfdist2["Cluster"] = adatax.obs["Cluster"]
     dfdist2 = dfdist2.groupby(["Cluster"]).mean()
@@ -998,49 +1180,26 @@
 
 def CAMELsanky(data,  # cmap=plt.get_cmap('jet_r'),
                colors=None,
                flows_color=None,
                labels_color='black', titles_color='black', labels_size=20,
                titles_size=20, node_sizes=False, sort_flows_by_nodes=False):
     """
-    Draw a sankey diagram.
-    Parameters
-    ----------
-    data : pandas DataFrame, numpy 2-D array, or list of equal length lists
-        The data to be represented. Each row describes a flow from the
-        beginning to the end. The first column must be numeric and represents
-        the (positive) width of the flow. Each other column describes the label
-        of the flow at a given stage.
-        At least two stages (start, end) are needed to produce a meaningful
-        diagram, hence "data" needs to hold three or more columns.
-    cmap : colormap, default: 'jet_r'
-        Used to assign a color to each block (and to its outgoing flows, unless
-        the "flows_color" argument is used).
-    flows_color : color, default: None
-        Draw all flows of a same color, rather than of the color of each flow's
-        starting block.
-    labels_color : color or None, default: 'black'
-        Color to be used for labels, None to hide them.
-    titles_color : color or None, default: 'black'
-        Color to be used for titles, None to hide them.
-    labels_size : int, default: 20
-        Font size for node labels.
-    titles_size : int, default: 20
-        Font size for titles.
-    node_sizes : Boolean or string, default: False
-        Whether to show node sizes close to node labels.
-        A format string with named placeholders can be passed to control the
-        formatting, as in '{label}\n({size}\%)': if only a non-named
-        placeholder is present, as in '- {}', the label is prepended separated
-        by a space.
-        Passing True is equivalent to passing '{label} ({size})' (or '({})').
-    sort_flows_by_nodes : Boolean, default: False
-        Whether flows from/to a given node should be sorted based on the
-        position of the starting and ending nodes - the default is to sort them
-        based on their position in the passed data.
+    CAMELsanky function for generating a Sankey diagram.
+
+    Args:
+    data (pd.DataFrame): Input data for the diagram.
+    colors (dict, optional): A dictionary mapping labels to colors.
+    flows_color (str, optional): Color for flows between nodes.
+    labels_color (str, optional): Color for node labels.
+    titles_color (str, optional): Color for titles.
+    labels_size (int, optional): Font size for node labels.
+    titles_size (int, optional): Font size for titles.
+    node_sizes (bool, optional): If True, display node sizes in the diagram.
+    sort_flows_by_nodes (bool, optional): If True, sort flows by nodes.
     """
 
     data = pd.DataFrame(data)
 
     # One column is for the weights, the remaining n+1 limits define n phases:
     phases = data.shape[1] - 2
```

### Comparing `scCAMEL-0.24b0/src/scCAMEL/CamelSwapline.py` & `scCAMEL-0.25b0/src/scCAMEL/CamelSwapline.py`

 * *Files 25% similar despite different names*

```diff
@@ -111,15 +111,34 @@
     if mode == "continuous":
         return -np.sum(pS*np.log2(S))
     if mode == "discrete":
         pS = pS[np.nonzero(pS)[0]]
         return -np.sum(pS*np.log2(pS))
 
 
+
+
 def PurityEstimationLearningScore(datax, clusterlist,  elbow=True, figureplot=True):
+
+    """
+    The function first calculates the Shannon entropy for each cluster based on their PCA scores,
+    and then calculates the Shannon entropy for each cluster after shuffling the PCA scores.
+    The ratio of these two values, normalized by the number of PCA dimensions, is used as a measure of purity.
+    The function returns a pandas dataframe sorted by the purity scores, with an optional elbow plot if figureplot is True.
+
+    Input:
+
+    datax: Single-cell RNAseq dataset
+    clusterlist: String indicating the name of the cluster column
+    elbow: Boolean indicating whether to perform elbow analysis to determine the optimal number of clusters
+    figureplot: Boolean indicating whether to plot the result
+    Output:
+
+    dfsort: Pandas dataframe sorted by purity scores, with an optional elbow plot if figureplot is True.
+    """
     cluslist = list(set(datax.obs[clusterlist]))
     entropyValue1=[]
     for item in cluslist:
         scpd1 = datax[datax.obs[clusterlist] == item]
         X_pcavalue=np.array(scpd1.obsm['Celltype_Score'])
         v0 = shannon_entropy(
             (X_pcavalue[:, 0] - X_pcavalue[:, 0].min()) / (X_pcavalue[:, 0].max() - X_pcavalue[:, 0].min()))
@@ -172,14 +191,34 @@
         plt.xlabel("Cell Types", fontsize=20)
         ax.spines.right.set_visible(False)
         ax.spines.top.set_visible(False)
         plt.grid(False)
     return dfsort
 
 def PurityEstimationPCA(datax, clusterlist, PCnum=10, elbow=True, figureplot=True):
+    """
+    Inputs:
+
+    datax: AnnData object, input data to perform PCA on
+    clusterlist: str, name of column in data.obs that contains cluster information
+    PCnum: int, number of principal components to use in entropy calculation, default=10
+    elbow: bool, whether to use elbow method to determine cutoff for low purity clusters, default=True
+    figureplot: bool, whether to generate a scatter plot of purity values, default=True
+    Outputs:
+
+    dfsort: pandas DataFrame with columns "Name", "Values", and "Purity". "Name" contains cluster names, "Values" contains normalized purity values, and "Purity" indicates whether the cluster is considered high (1) or low (0) purity based on cutoff determined by elbow method or not used if elbow=False.
+    Functionality:
+
+    Calculates the normalized entropy values for each cluster based on the specified number of principal components.
+    Calculates the normalized entropy values for each cluster after shuffling the principal component values, which serves as a null model.
+    Calculates the purity value for each cluster by subtracting the normalized entropy value of the null model from the original normalized entropy value, and dividing by the original normalized entropy value.
+    Sorts the clusters by decreasing purity values.
+    Uses the elbow method to determine the cutoff for low purity clusters if elbow=True.
+    Returns a pandas DataFrame with cluster names, normalized purity values, and high/low purity status. Also generates a scatter plot of cluster purity values if figureplot=True.
+    """
     num = PCnum
     cluslist = list(set(datax.obs[clusterlist]))
     X = datax.X
     pca_ = PCA(n_components=min(datax.shape[0], num), svd_solver='auto', random_state=0)
     PCAmodel = pca_.fit(X)
         # X_cca,Y_cca=cca_.fit_transform(X,Y)
     X_pcavalueAll = abs(PCAmodel.transform(X))
@@ -237,14 +276,29 @@
         plt.xlabel("Cell Types", fontsize=20)
         ax.spines.right.set_visible(False)
         ax.spines.top.set_visible(False)
         plt.grid(False)
     return dfsort
 
 def PurityEstimation(datax, clusterlist, PCnum=10, figureplot=True):
+    """
+    Inputs
+    datax: an AnnData object
+    clusterlist: a string representing the column name in the datax.obs dataframe that contains the cell type cluster assignments
+    PCnum: an integer specifying the number of principal components to use for entropy estimation
+    figureplot: a boolean indicating whether to generate a plot or not (default is True)
+    Outputs:
+    dfsort: a pandas dataframe with columns "Name" (cell type names), "Values" (entropy values), and "Purity" (0 for impure and 1 for pure cell types)
+    Functionality:
+
+    For each cell type in clusterlist, it performs PCA on the subset of data in datax that is assigned to that cell type, and estimates entropy based on the first PCnum principal components.
+    It calculates the product of the entropy values and raises it to the power of -1/PCnum to obtain a "purity score" for the cell type.
+    It sorts the cell types by their purity scores and assigns a purity label (0 or 1) based on the "knee point" in the sorted list (determined using the kneed package).
+    It generates a scatter plot of the entropy values for each cell type and marks the knee point with a vertical dashed line.
+    """
     entropyValue = []
     num = PCnum
     cluslist = list(set(datax.obs[clusterlist]))
     for item in cluslist:
         scpd1 = datax[datax.obs[clusterlist] == item]
         X = scpd1.X
         pca_ = PCA(n_components=min(scpd1.shape[0], num), svd_solver='auto', random_state=0)
@@ -297,14 +351,29 @@
     #dfg = pd.DataFrame(X_r)
     #dfg.index = XXdf.index
     #dfg2 = dfg.join(XXdf.iloc[:,-1:], how="inner")
     return datax, umaptrain
 
 
 def EnrichScore_Ranksum(adata, foldchange=1, meanthreshold=0.05, pvalue=0.1):
+    """
+    Input:
+    adata: AnnData object containing the count matrix and cell metadata information
+    foldchange: fold change threshold for differential expression analysis (default = 1)
+    meanthreshold: mean expression threshold for differential expression analysis (default = 0.05)
+    pvalue: p-value threshold for differential expression analysis (default = 0.1)
+    Output:
+
+    dfmk: DataFrame containing the differentially expressed genes for each cluster,
+    along with the cluster name and the number of other clusters in which the gene is differentially expressed
+    Functionality:
+    This function performs differential expression analysis using ranksum test and generates a list of differentially expressed genes for each cluster based on the specified thresholds for fold change, mean expression, and p-value.
+    It returns a DataFrame containing the differentially expressed genes for each cluster,
+     along with the cluster name and the number of other clusters in which the gene is differentially expressed.
+    """
     cluslist = list(set(adata.obs["Cluster"]))
     dfgrp = pd.DataFrame(adata.X.T, index=adata.var.index, columns=adata.obs.index).T
     dfgrp["Cluster"] = adata.obs["Cluster"]
     # dfgrp.shape
     markers = defaultdict(set)
     mkdict = {}
     sys.stdout.write("[%s]" % "Processing")
@@ -359,14 +428,33 @@
     dfmk = pd.DataFrame([genelist, grouplist, numberlist])
     dfmk.columns = dfmk.iloc[0, :]
     dfmk = dfmk.T
     dfmk.columns = ["Gene", "Group", "Num"]
     return dfmk
 
 def ConsistantAssign(datax,dfsig,outputfilepath=None,outputPlot=True ):
+    """
+    Inputs:
+
+    datax: AnnData object containing the scRNA-seq data with cell type scores
+    dfsig: Pandas dataframe containing signature matrix for cell type scores
+    outputfilepath: Path to output file for cells with inconsistent cluster assignment (default=None)
+    outputPlot: Boolean to control whether to plot the consistency score (default=True)
+    Outputs:
+
+    datax: AnnData object with additional columns "PredictCluster" and "ClusterConsistanceScore"
+    If outputfilepath is provided, a tab-separated file with cells with inconsistent cluster assignment will be saved to the specified path
+    If outputPlot is set to True, a bar plot showing the percentage of consistently assigned cells for each cluster will be displayed
+    Functionality:
+
+    Calculates the consistency score for each cell by comparing its true cluster assignment with its predicted cluster assignment based on the highest cell type score
+    Adds the predicted cluster assignment and the consistency score as new columns in the AnnData object
+    Optionally saves a file with cells that have inconsistent cluster assignment
+    Optionally displays a bar plot showing the percentage of consistently assigned cells for each cluster
+    """
     dfprob=pd.DataFrame(datax.obsm['Celltype_Score'], index=datax.obs.index,columns=datax.uns['Celltype_Score_RefCellType'])
     dfprob1=dfprob-dfsig.quantile(0.95)
     dfprob1[dfprob1<0]=0
     dfprob1neg=dfprob1.loc[dfprob1.sum(1)==0]
     dfprob1posi=dfprob1.loc[dfprob1.sum(1)>0]
     cluslist=[]
     colname=dfprob1posi.columns
@@ -427,14 +515,29 @@
 from matplotlib import pyplot
 from matplotlib import gridspec
 
 
 
 def CellTypeSimilarityViolinPlot(datax, dataref,fontsizevalue=15):
     #### need set if, to check the Cluster, celltype_score, etc......
+    """
+    Input:
+    datax: AnnData object containing query cells
+    dataref: AnnData object containing reference cells
+    fontsizevalue: Font size for plot labels
+    Output:
+    dfprob: Pandas dataframe containing the cell type score for each cell in datax
+    Functionality:
+
+    Creates a violin plot showing the similarity of each query cell type to each reference cell type based on the cell type scores
+    The plot has a separate row for each query cell type and a separate column for each reference cell type
+    The plot is divided into violins for each reference cell type, with the density of query cells for each reference cell type displayed within each violin
+    The plot is colored according to the color scheme specified in the reference data
+    The output dataframe contains the cell type score for each cell in the query data
+    """
     genename = np.sort(list(set(datax.obs["Cluster"])))
     name = np.sort(list(set(dataref.obs["Cluster"])))
     dfprob = pd.DataFrame(datax.obsm['Celltype_Score'])
     dfprob.columns = datax.uns['Celltype_Score_RefCellType']
     dfprob.index = datax.obs.index
     dfmk = dfprob.astype(float).join(datax.obs["Cluster"], how="inner").T
     refcolor_dict=pd.Series(dataref.uns["refcolor_dict"])
@@ -528,14 +631,29 @@
         loaded_model = pickle.load((open(filename, 'rb')))
         return loaded_model
 
 def rgb2hex(r,g,b):
     return "#{:02x}{:02x}{:02x}".format(r,g,b)
 
 def addcolor(datax,clustername="Cluster", colorcode="color", predef=pd.Series()):
+    """
+    Input:
+    datax: AnnData object, a data matrix with annotation, where the row index is the cell barcode, and the columns are the gene names and cell annotations
+    clustername: str, the name of the column in the annotation that contains the cell cluster information
+    colorcode: str, the name of the new column to be added to the annotation, which contains the color code for each cell
+    predef: pd.Series, optional argument, a pre-defined dictionary with cluster name as key and color code as value
+    Output:
+    datax: AnnData object, a data matrix with annotation, where the row index is the cell barcode, and the columns are the gene names and cell annotations,
+    with a new column added that contains the color code for each cell
+    Functionality:
+
+    This function adds a new column to the annotation of the data matrix, which contains the color code for each cell based on the cluster information in the specified column.
+    If a pre-defined dictionary is provided, the function uses that to assign color codes to each cluster instead of generating a new color code.
+    The color codes are added as a new column to the data matrix and stored in the uns field with the key "refcolor_dict".
+    """
     if not colorcode in datax.obs.columns:
         if predef.empty:
             color_dict = {}
             wanted_order=list(set(datax.obs[clustername]))
             for item in wanted_order:
                 color_dict[item] = np.array(random.sample(range(0, 255), 3)).tolist()
             colorlist=[]
@@ -568,14 +686,36 @@
             newlist.append(item)
     adatax.obs[ 'Assigned_Celltype']=newlist
     return adatax
 
 def UMAP_plot(datax,clustername="Cluster", colorcode="color",legendOnPlot=False,Ncol=2,
               legendshow=True,figuresize=(10,10),alphavalue=0.8, lwvalue=0.1, markervalue=".",
              dotsize=200,lengendfont=20, legendloc=2,bbox_to_anchorvalues=(1.15, 1.2)):
+    """
+    This function takes a scanpy object and generates a UMAP plot based on the computed UMAP coordinates of the cells in the object. It also allows coloring of the cells based on a specified categorical variable in the object, and adds a legend to the plot.
+
+    Inputs:
+    datax: A scanpy object containing the data to plot
+    clustername: The name of the categorical variable to use for coloring the cells (default: "Cluster")
+    colorcode: The name of the new column to add to the object to store the cell colors (default: "color")
+    legendOnPlot: If True, shows the legend on the plot itself (default: False)
+    Ncol: Number of columns to use for the legend if it is shown on the plot (default: 2)
+    legendshow: If True, shows the legend (default: True)
+    figuresize: A tuple specifying the size of the plot in inches (default: (10,10))
+    alphavalue: Alpha value for the cells (default: 0.8)
+    lwvalue: Line width for the cells (default: 0.1)
+    markervalue: Marker style for the cells (default: ".")
+    dotsize: Size of the cells in the plot (default: 200)
+    lengendfont: Font size for the legend (default: 20)
+    legendloc: Location of the legend on the plot (default: 2)
+    bbox_to_anchorvalues: Tuple specifying the location of the legend box on the plot (default: (1.15, 1.2))
+    Output:
+    datax: The scanpy object with the added color column
+    ax: The plot axis object
+    """
     #groups=list(set(df["Cluster"]))
     #annot=dfref["Cluster"].values
     #fname="uMAP_GBM"
     #title=''
     #prefix='uMAP'
     #colorlist=[]
     #for item in df["Cluster"].values:
@@ -618,14 +758,41 @@
 
 
 def UMAPplotRefPred(DataRef, DataPdt, refClusterName,pdtClusterName, refColorCode, pdtColorCode,figuresize=(10, 10),
                     RefAlphaValue=0.8, RefLwValue=0.1, RefMarkerValue="x", RefDotSize=200,
                     PdtAlphaValue=0.8, PdtLwValue=0.1, PdtMarkerValue=".", PdtDotSize=200,
                     lengendfont=20, RefLegendloc=2, PdtLegendloc=3, Refbbox_to_anchorvalues=(1.15, 1.2),
                     Pdtbbox_to_anchorvalues=(1.15, 0.05)):
+    """
+    Inputs:
+    DataRef: Reference dataset (an AnnData object) to be plotted on UMAP.
+    DataPdt: Predicted dataset (an AnnData object) to be plotted on UMAP.
+    refClusterName: The column name of the cluster labels of the reference dataset.
+    pdtClusterName: The column name of the cluster labels of the predicted dataset.
+    refColorCode: The column name of the colors assigned to each cluster in the reference dataset.
+    pdtColorCode: The column name of the colors assigned to each cluster in the predicted dataset.
+    figuresize: A tuple specifying the figure size (default: (10,10)).
+    RefAlphaValue: The alpha value of the markers for the reference dataset (default: 0.8).
+    RefLwValue: The line width value for the reference dataset (default: 0.1).
+    RefMarkerValue: The marker value for the reference dataset (default: "x").
+    RefDotSize: The dot size value for the reference dataset (default: 200).
+    PdtAlphaValue: The alpha value of the markers for the predicted dataset (default: 0.8).
+    PdtLwValue: The line width value for the predicted dataset (default: 0.1).
+    PdtMarkerValue: The marker value for the predicted dataset (default: ".").
+    PdtDotSize: The dot size value for the predicted dataset (default: 200).
+    lengendfont: The font size of the legend (default: 20).
+    RefLegendloc: The location of the legend for the reference dataset (default: 2).
+    PdtLegendloc: The location of the legend for the predicted dataset (default: 3).
+    Refbbox_to_anchorvalues: The anchor values for the reference legend box (default: (1.15, 1.2)).
+    Pdtbbox_to_anchorvalues: The anchor values for the predicted legend box (default: (1.15, 0.05)).
+    Outputs:
+    DataRef: The reference dataset (an AnnData object).
+    DataPdt: The predicted dataset (an AnnData object).
+    ax: The matplotlib axes object containing the UMAP plot.
+    """
     # groups=list(set(df["Cluster"]))
     # annot=dfref["Cluster"].values
     # fname="uMAP_GBM"
     # title=''
     # prefix='uMAP'
     # colorlist=[]
     # for item in df["Cluster"].values:
@@ -702,14 +869,30 @@
                                 indptr),
                                 shape=(nobs, nobs))
     D.eliminate_zeros()
     return D
 
 def connectivities_to_igraph(adjacency, directed=None):
     """Get igraph graph from adjacency matrix."""
+    """
+    The function connectivities_to_igraph takes an adjacency matrix and returns a graph object from the igraph library.
+
+    Input:
+    adjacency: A square, symmetric matrix representing the pairwise similarities or distances between observations.
+    directed: A boolean indicating whether the graph should be directed or undirected (default is None).
+    Output:
+    gph: An igraph Graph object.
+   
+    np.nonzero(): Returns the indices of the elements that are non-zero.
+    zip(): Returns an iterator of tuples, where the i-th tuple contains the i-th element from each of the argument sequences or iterables.
+    igraph.Graph.add_vertices(): Adds vertices to the graph.
+    igraph.Graph.add_edges(): Adds edges to the graph.
+    igraph.EdgeSeq.es: Property that returns the sequence of edges of a graph.
+    warn() (from the logging module): Logs a warning message.
+    Note: The function tries to set the weights of the edges using the weight attribute of gph.es. If this fails, it silently ignores the error."""
     try:
         import igraph as ig
     except ImportError:
         raise ImportError(
             'Please install igraph!'
         )
     sources, targets = adjacency.nonzero()
@@ -726,14 +909,32 @@
     if gph.vcount() != adjacency.shape[0]:
         logging.warn('The constructed graph has only {} nodes. '
                   'Your adjacency matrix contained redundant nodes.'
                   .format(gph.vcount()))
     return gph
 
 def UMAPindices_distancesTosparseMatrix(knn_indices, knn_dists, n_obs, n_neighbors):
+    """
+    This function takes in the indices and distances of the k-nearest neighbors (knn_indices, knn_dists),
+    the total number of observations (n_obs), and the number of neighbors used to calculate the distances (n_neighbors),
+    and returns a sparse matrix in CSR format representing the pairwise distances between the observations.
+
+    Input:
+    knn_indices: array-like, shape (n_obs, n_neighbors)
+    The indices of the k-nearest neighbors for each observation.
+    knn_dists: array-like, shape (n_obs, n_neighbors)
+    The distances to the k-nearest neighbors for each observation.
+    n_obs: int
+    The total number of observations.
+    n_neighbors: int
+    The number of neighbors used to calculate the distances.
+    Output:
+    result: scipy.sparse.csr_matrix, shape (n_obs, n_obs)
+    A sparse matrix in CSR format representing the pairwise distances between the observations.
+    """
     rows = np.zeros((n_obs * n_neighbors), dtype=np.int64)
     cols = np.zeros((n_obs * n_neighbors), dtype=np.int64)
     vals = np.zeros((n_obs * n_neighbors), dtype=np.float64)
 
     for i in range(knn_indices.shape[0]):
         for j in range(n_neighbors):
             if knn_indices[i, j] == -1:
@@ -793,14 +994,26 @@
     distances = UMAPindices_distancesTosparseMatrix(
         knn_indices, knn_dists, n_obs, n_neighbors
     )
 
     return distances, connectivities.tocsr()
 
 def SWAPLINE_dist(datax, n_neighbors=50, metric = 'euclidean'):
+    """
+    Inputs:
+    datax: an AnnData object containing cell type scores.
+    n_neighbors (optional, default=50): an integer value for the number of nearest neighbors to be used in the pairwise distance calculation.
+    metric (optional, default='euclidean'): a string value for the metric used to calculate pairwise distances.
+    Outputs:
+    datax: an AnnData object with updated connectivities and distances.
+    Function description:
+    This function calculates the pairwise distances between cell type scores in the input data, and then calculates the connectivities and distances using the UMAP algorithm.
+    The resulting connectivities and distances are stored in the output AnnData object.
+    The number of nearest neighbors to be used in the pairwise distance calculation and the metric used to calculate pairwise distances can be customized by the user.
+    """
     #n_pcs = 30, n_neighbors = len(dfnn.index),  metric = 'euclidean'
     ####
     # must be np.float32
     ####
     XX = datax.obsm["Celltype_Score"].astype(np.float32)
 
     #pca_ = PCA(n_components=n_pcs, svd_solver='arpack', random_state=0)
@@ -824,26 +1037,40 @@
     #neighbors_connectivities = _connectivities
     #adjacency = _connectivities
     #neighbors_connectivities = _connectivities
     logging.info('Camel...Running: finish.....')
     return datax
 
 def clusterfinder(datax,Th_value =1, method="Louvain"):
+    """
+    Inputs:
+
+    datax: AnnData object containing the gene expression data and UMAP coordinates
+    Th_value: Resolution parameter value for the clustering algorithm. Default is 1.
+    method: Clustering algorithm to use. Two options are available: "Louvain" (default) or "Leiden".
+    Outputs:
+
+    Returns an AnnData object with a new observation-level column "Assigned_Celltype" containing the cell cluster assignments generated by the chosen clustering algorithm.
+    Functionality:
+    This function performs clustering on the gene expression data and UMAP coordinates contained in an AnnData object. The user can choose between two clustering algorithms:
+    Louvain or Leiden. The resolution parameter for the clustering algorithm can be set by the user (default is 1).
+    The function returns the original AnnData object with a new observation-level column containing the cluster assignments generated by the chosen algorithm.
+
+    """
+
     buildgraph = connectivities_to_igraph(adjacency=datax.obsp["connectivities"], directed=True)
     if method=="Louvain":
 
         from natsort import natsorted
         try:
             import louvain
-            #import leidenalg
         except ImportError:
             raise ImportError(
                 'Please install the louvain!.'
             )
-        #partition_kwargs = dict(partition_kwargs)
 
         logging.info('Camel...Running: Louvain clustering')
 
         parttern = louvain.find_partition(
             buildgraph,
             partition_type=louvain.RBConfigurationVertexPartition,
             resolution_parameter=Th_value,
@@ -864,22 +1091,14 @@
         except ImportError:
             raise ImportError(
                 'Please install leidenalg!'
             )
         #partition_kwargs = dict(partition_kwargs)
 
         print('Camel...Running: Leiden clustering')
-        #partition_type options:
-        #leidenalg.RBConfigurationVertexPartition
-        #leidenalg.CPMVertexPartition
-        #leidenalg.SignificanceVertexPartition
-        #leidenalg.RBERVertexPartition
-        #leidenalg.MutableVertexPartition
-        #leidenalg.ModularityVertexPartition
-        # clustering proper
         parttern = leidenalg.find_partition(
             buildgraph,
             partition_type = leidenalg.RBConfigurationVertexPartition,
             resolution_parameter=Th_value,
             )
         # output clusters
         clustergroups = np.array(parttern.membership)
@@ -887,14 +1106,33 @@
             values=clustergroups.astype('U'),
             categories=natsorted(np.unique(clustergroups).astype('U')),
         )
     datax.obs["Assigned_Celltype"]=cellcluster
     return datax
 
 def transfer_learning(UMAPmodel, datapdt, datax,clustername, colorcode, n_neighbors=50):
+    """
+    Input:
+
+    UMAPmodel: a trained UMAP model
+    datapdt: a scanpy AnnData object containing the predicted cell type scores
+    datax: a scanpy AnnData object containing the original data with known cell type annotations
+    clustername: a string representing the name of the cluster column in both datapdt and datax
+    colorcode: a string representing the name of the column containing cell colors in datax
+    n_neighbors: an integer representing the number of neighbors to use in the K-nearest neighbors classifier
+    Output:
+
+    datapdt: a scanpy AnnData object with predicted cell types and colors
+    Function description: The function uses transfer learning to predict cell types and colors for new data based on a trained model.
+     It first uses a UMAP model to transform the predicted cell type scores in datapdt into two-dimensional UMAP coordinates.
+     It then trains a K-nearest neighbors classifier on the cell type scores and cluster annotations in datax.
+     Finally, it predicts cell types for the cells in datapdt using the trained classifier and assigns colors based on the colorcode column in datax if available. T
+    the function returns the modified datapdt object.
+
+    """
     try:
         from sklearn.neighbors import KNeighborsClassifier
     except ImportError:
         raise ImportError(
             'Please install sklearn!'
         )
     X_rTest = UMAPmodel.transform(datapdt.obsm["Celltype_Score"])
@@ -918,14 +1156,36 @@
 
 def prediction(datax, mcolor_dict,net,learninggroup="train", radarplot=True, fontsizeValue=35,
               datarefplot=None,
                ncolnm=1, bbValue=(1.1, 1.05)):
     #mwanted_order = mwanted_order, mclasses_names = mclasses_names, mprotogruop = dfpfcclus.loc["Cluster"].values,
     #mdf_train_set = mdf_train_set, figsizeV = 18, mtrain_index = mtrain_index, net = net, mreorder_ix = mreorder_ix,
     #mcolor_dict = refcolor_dict, learninggroup = "test"
+    """
+    Inputs:
+
+    datax: an AnnData object containing gene expression data
+    mcolor_dict: a dictionary mapping cell type names to colors
+    net: a trained neural network model
+    learninggroup: a string indicating whether to perform the prediction on the "train" or "test" set
+    radarplot: a boolean indicating whether to generate a radar plot of the results
+    fontsizeValue: an integer specifying the font size of the radar plot labels
+    datarefplot: an AnnData object containing reference gene expression data (only used if learninggroup is "test")
+    ncolnm: an integer specifying the number of columns in the radar plot
+    bbValue: a tuple of two floats specifying the scaling factor for the radar plot axes
+    Outputs:
+
+    datax: an AnnData object containing the predicted cell type scores
+    (if radarplot is True):
+    axm: the Matplotlib axis object for the radar plot
+    dfclRef: a Pandas DataFrame containing the coordinates of the cell type scores in the radar plot
+    Function description: This function predicts cell type scores using a trained neural network model,
+    either on the train or test set of gene expression data stored in an AnnData object.
+    If radarplot is True, it generates a radar plot of the predicted scores.
+    """
 
     mcolor_dict=pd.Series(mcolor_dict)
     if  learninggroup=="train":
         mdf_train_set = pd.DataFrame(datax.obsm["train_set_values"].T, index=datax.uns["train_set_gene"],
                                      columns=datax.obs.index)
         mtrain_index = datax.obs["mtrain_index"].values
         mwanted_order = datax.uns["mwanted_order"]
@@ -1033,30 +1293,29 @@
 
 
 
 
 def RadarPlot(data, scaling=False,start_angle=90, rotate_labels=True, labels=('one','two','three'),fontsizeV=20,
                   sides=3, label_offset=0.10, fig_args = {'figsize':(18,18),'facecolor':'white','edgecolor':'white'}):
     '''
-    This will create a basic polygonal plot
+    Inputs:
+
+    data: array-like object of shape (N, S), where N is the number of data points and S is the number of sides/vertices of the polygon.
+    scaling: boolean, whether to scale the data so that it sums to 1.
+    start_angle: int, the angle in degrees of the first vertex.
+    rotate_labels: boolean, whether to rotate the labels so they are perpendicular to the vertices.
+    labels: array-like object of length S, the labels for the vertices.
+    fontsizeV: int, the font size for the labels.
+    sides: int, the number of sides/vertices of the polygon.
+    label_offset: float, the offset for the label from the vertex (as a percentage of the distance from the origin).
+    fig_args: dict, additional arguments for the plt.figure() function.
+    Outputs:
 
-    # Scale data for plot (i.e. a + b + c = 1)
-    scaling=True,
-    # Direction of first vertex.
-    start_angle=90,
-    # Orient labels perpendicular to vertices.
-    rotate_labels=True,
-    # Labels for vertices.
-    labels=('one','two','three')
-    # Offset for label from vertex (percent of distance from origin).
-    label_offset=0.10,
-    # Any matplotlib keyword args for plots.
-    edge_args={'color':'black','linewidth':2},
-    # Any matplotlib keyword args for figures.
-    fig_args = {'figsize':(8,8),'facecolor':'white','edgecolor':'white'},
+    newdata: array of shape (N, 2), the transformed data used to plot the radar chart.
+    ax: the axis object for the plot.
     '''
     pi=np.pi
     basis = np.array([[np.cos(2*i*pi/sides + start_angle*pi/180),
                     np.sin(2*i*pi/sides + start_angle*pi/180)] for i in range(sides)])
     RadialBasis=np.array([[np.cos(2*i*pi/sides + (start_angle+180/sides)*pi/180),
                     np.sin(2*i*pi/sides + (start_angle+180/sides)*pi/180)] for i in range(sides)])
 
@@ -1166,14 +1425,47 @@
     return newdata,ax
 
 
 def RadarVisualization(refdataLR, dataclpn, mreorder_ix, fontsizeValue,bbValue,
                        mtrain_index, mwanted_order,Ncolm,
                        mprotogruop,mdf_train_set,
                        mclasses_names, mcolor_dict, learninggroup="train"):
+    """
+    Input:
+
+    refdataLR: numpy array
+    dataclpn: numpy array
+    mreorder_ix: numpy array
+    fontsizeValue: int
+    bbValue: tuple
+    mtrain_index: numpy array
+    mwanted_order: numpy array
+    Ncolm: int
+    mprotogruop: numpy array
+    mdf_train_set: pandas dataframe
+    mclasses_names: numpy array
+    mcolor_dict: dictionary
+    learninggroup: string
+    Output:
+
+    axm: matplotlib axis object
+    dfnewcl: pandas dataframe
+    The function takes in input several arguments, including refdataLR and dataclpn which are numpy arrays, mreorder_ix,
+    mtrain_index, mwanted_order, mprotogruop, and mclasses_names which are numpy arrays, mdf_train_set which is a pandas dataframe,
+    mcolor_dict which is a dictionary, and fontsizeValue and Ncolm which are integers.
+    t also takes a string learninggroup which specifies whether the function is being called for the train or test dataset.
+
+    The function returns a matplotlib axis object axm and a pandas dataframe dfnewcl.
+    The function plots a radar chart using the RadarPlot function,
+    and then adds scatter points to the chart based on the values in mtrain_index and mwanted_order.
+    If learninggroup is set to "test", the scatter points are based on dataclpn. The function also adds a legend to the chart using the mwanted_order and mcolor_dict.
+    The dfnewcl dataframe is a dataframe of the x and y coordinates of the scatter points.
+
+    """
+
     #refdataLR = refdataLR, dataclpn = dataclpn, mreorder_ix = mreorder_idx,
     #mtrain_index = mtrain_index, mwanted_order = wanted_orderclpn,
     #mprotogruop = dfpfcclus.loc["Cluster"].values,mdf_train_set=mdf_train_set,
     #mclasses_names = mclasses_names, mcolor_dict = color_dictclpn, learninggroup = "train"
     if learninggroup == "train":
         mnewdata, axm = RadarPlot(refdataLR[:, mreorder_ix], sides=len(mreorder_ix),
                                   fontsizeV=fontsizeValue,labels=mclasses_names[mreorder_ix])
@@ -1218,14 +1510,30 @@
             recs.append(mpatches.Rectangle((0, 0), 1, 1, fc=mcolor_dict[item]))
         axm.legend(recs, mwanted_order, loc=2, bbox_to_anchor=bbValue,ncol=Ncolm, prop={'size': fontsizeValue})
         return axm, dfnewcl
 
 
 
 def permutationTest(datax,net,num, plotshow=True):
+
+    """
+    Input:
+    datax: AnnData object containing the count data, cell type scores, and other relevant information.
+    net: Trained scDeepCluster network
+    num: Number of iterations to run the permutation test
+    plotshow: Boolean value indicating whether to show the violin plot or not
+    Output:
+    dftest0: Pandas DataFrame containing the results of the permutation test, showing the predicted cell type fractions for each iteration.
+    ratiodf: Pandas DataFrame containing the fraction of iterations for which each cell type has a predicted fraction greater than or equal to a given threshold.
+    Function: The permutationTest function runs a permutation test to assess the robustness of the cell type predictions made by a scDeepCluster network.
+    The function generates random permutations of the count data and uses the trained network to predict the cell type fractions for each permutation.
+    The resulting predicted cell type fractions are used to generate a violin plot showing the distribution of predicted fractions for each cell type.
+    The function also generates a DataFrame showing the fraction of iterations for which each cell type has a predicted fraction greater than or equal to a given threshold.
+    The function returns the dftest0 and ratiodf dataframes.
+    """
     dfprobRef = pd.DataFrame(datax.obsm["Celltype_Score"], index=datax.obs.index,
                              columns=datax.uns["Celltype_Score_RefCellType"])
     #dfpfcclus = datax.obs[["mtrain_index", "Cluster"]].T
     #mwanted_order = datax.uns["mwanted_order"]
     mreorder_ix=datax.uns["Celltype_OrderNumber"]
     mdf_train_set = pd.DataFrame(datax.obsm["train_set_values"].T, index=datax.uns["train_set_gene"],
                                  columns=datax.obs.index)
@@ -1284,14 +1592,32 @@
         ax.spines['top'].set_visible(False)
     return dftest0, ratiodf
 
 
 
 
 def ProbSinglePlot (datax, mcolor_dict, fs=25):
+    """
+    Input:
+
+    datax: AnnData object containing the cell type probability scores for each cell
+    mcolor_dict: dictionary mapping each cell type to a RGB color code
+    fs: font size for the plot
+    Output:
+
+    fig: the generated matplotlib figure object
+    Functionality:
+    This function generates a violin plot for each cell type in datax,
+    displaying the distribution of probability scores for each cell in that cell type.
+    The violin plots are arranged in a grid, with one plot for each cell type.
+    The x-axis displays the cell type names, and the y-axis displays the probability score (from 0 to 100%).
+    Additionally, for each cell type, a bar is displayed at the top of the plot to indicate the threshold value for the probability score (set at 80%).
+    The function also uses the mcolor_dict input to color each violin plot based on the corresponding cell type color.
+
+    """
     import seaborn as sns
     #dfprobRef = dfprobRef, dfpfcclus = dfpfcclus, mwanted_order = mwanted_order, mcolor_dict = refcolor_dict
     # mdf_train_set = pd.DataFrame(datax.obsm["train_set_values"].T, index=datax.uns["train_set_gene"],
     #                             columns=datax.obs.index)
     #mtrain_index = datax.obs["mtrain_index"].values
     #mwanted_order = datax.uns["mwanted_order"]
     #mclasses_names = datax.uns["mclasses_names"]
@@ -1373,14 +1699,30 @@
     from matplotlib.collections import PolyCollection
     ax = plt.gca()
     for art in ax.get_children():
         if isinstance(art, PolyCollection):
             art.set_edgecolor((0.6, 0.6, 0.6))
 
 def ProbMultiPlot( datax, mcolor_dict,fs=15):
+
+    """
+    Input:
+
+    datax: AnnData object
+    mcolor_dict: dictionary containing color values for each cell type
+    fs: font size for plot labels
+    Output:
+
+    fig: matplotlib figure object
+    Functionality:
+    This function generates a violin plot of the probability of cell type similarity for each cell in the dataset,
+     along with a scatter plot of the same data points. The violin plot shows the distribution of the probability of similarity for each cell type, while the scatter plot shows the actual values for each cell.
+     The color of each data point in the scatter plot corresponds to the cell type of the cell. The function also adds a legend to the plot showing the color-coding for each cell type.
+    The function returns the generated matplotlib figure object.
+    """
      #dfprobRef, dfpfcclus, mwanted_order, mcolor_dict
 #dfprobRef=dfprobRef, dfpfcclus=dfpfcclus, mwanted_order=mwanted_order,
                   # mcolor_dict=refcolor_dict
      mcolor_dict=pd.Series(mcolor_dict)
      mcolor_dict = mcolor_dict.map(lambda x: list(map(lambda y: y / 255., x)))
      dfprobRef = pd.DataFrame(datax.obsm["Celltype_Score"], index=datax.obs.index,
                               columns=datax.uns["Celltype_Score_RefCellType"])
@@ -1432,19 +1774,32 @@
      ax.legend(recs, mwanted_order, loc=2, bbox_to_anchor=(1.05, 1.05), prop={'size': fs})
      # plt.savefig("GBMDGTFgenes_mDG_vs_PEgbm_wheel%sPlot.png"%cvalue,bbox_inches='tight')
      return fig
 
 
 
 def scaling_data(datax, LogMinMax=False):
+    """
+    Input:
+    datax: AnnData object containing the raw expression data
+    LogMinMax (optional): Boolean, default False. If True, apply log normalization followed by min-max scaling.
+    Output:
+    datax: AnnData object with the scaled expression data in the "Scaled_Matrix" layer.
+    Functionality:
+    The function scales the input expression data by dividing
+    each cell's expression values by the median expression value across all cells,
+    and then scaling to a total count of 100,000. If LogMinMax is True,
+    the function first applies log normalization (log10(x+1)) followed by min-max scaling to values between 0 and 1.
+    The scaled expression matrix is stored in the "Scaled_Matrix" layer of the input AnnData object.
+    """
     XX = datax.X
     countsInEachCell = np.ravel(XX.astype(float).sum(1)).copy()
     # XX = XXV.copy()
     if issubclass(XX.dtype.type, (int, np.integer)):
-        XX = XX.astype(np.float32)  # np.float32 or float (64)
+        XX = XX.astype(np.float32)  # np.float32
     countsInEachCell = np.asarray(countsInEachCell)
     after = np.median(countsInEachCell[countsInEachCell > 0], axis=0)
     countsInEachCell += (countsInEachCell == 0)
     countsInEachCell = countsInEachCell / after
     np.divide(XX, countsInEachCell[:, None], out=XX)
     XX = (XX.T / XX.sum(1)).T * 100000
     if LogMinMax == True:
@@ -1454,14 +1809,23 @@
     XX = np.nan_to_num(XX)
     datax.layers["Scaled_Matrix"] = XX
 
     return datax
 
 
 def MarkerGenePlot(datax, genelist, nrow=2,fc=12,colormapopt="cividis"):
+    """
+    Inputs:
+    datax: AnnData object containing gene expression data and UMAP coordinates.
+    genelist: list of genes to plot.
+    nrow: number of rows in the plot. Default value is 2.
+    fc: font size of the plot titles. Default value is 12.
+    colormapopt: colormap option to use in the plot. Default value is "cividis".
+    Outputs: fig: matplotlib figure object containing the scatterplots of the gene expression levels in the UMAP space for each gene in the genelist.
+    """
     import math
     dfexpr = pd.DataFrame(datax.layers['Scaled_Matrix'].T, index=datax.var.index, columns=datax.obs.index)
     dfexpr = dfexpr.T
     dfexpr["UMAPX"] = datax.obsm["X_umap"][:, 0]
     dfexpr["UMAPY"] = datax.obsm["X_umap"][:, 1]
     fig = plt.figure(figsize=(15, 15), facecolor='w')
     for i in range(1, len(genelist) + 1):
@@ -1473,14 +1837,27 @@
         plt.title(genename, fontsize=fc)
         plt.axis("off")
     return fig
 
 
 
 def ConstrualValue(datax,net,filepath, ConstrualModel="DeepLift", MarkerGeneFinder=True,fcV=3, pValCutOff = 0.1):
+    """
+    Function name: ConstrualValue
+    Input:
+    datax: AnnData object containing gene expression data.
+    net: PyTorch model trained for the task of interest.
+    filepath: Path to save the output files.
+    ConstrualModel (optional, default="DeepLift"): String indicating the attribution algorithm to be used.
+    MarkerGeneFinder (optional, default=True): Boolean indicating whether to perform marker gene analysis.
+    fcV (optional, default=3): Fold change cutoff for differential expression analysis.
+    pValCutOff (optional, default=0.1): p-value cutoff for differential expression analysis.
+    Output: Modified datax AnnData object containing the construal value scores for each sample in the dataset,
+    as well as the top marker genes (if MarkerGeneFinder=True).
+    """
     torch.manual_seed(0);
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     print("CamelRunning with %s"%device)
     if "test_set_values" in datax.obsm:
         mdf_train_set = pd.DataFrame(datax.obsm["test_set_values"].T, index=datax.uns["train_set_gene"],
                                  columns=datax.obs.index)
     elif "train_set_values" in datax.obsm:
@@ -1524,15 +1901,32 @@
             dfmk100.to_csv("%s_Top100Marker.csv"%filepath,sep="\t")
             datax.uns["TopMarkerGene"]=dfmk100.values
             datax.uns["TopMarkerGene_Cluster"]=columnlist
         return datax
     else:
         return datax
 
-def ConstrualValue22(datax,net,filepath, ConstrualModel="DeepLift", targetvalue=0,MarkerGeneFinder=True,fcV=3, pValCutOff = 0.1):
+def ConstrualValue22(datax,net,filepath, ConstrualModel="DeepLift", targetvalue=0,
+                     MarkerGeneFinder=True,fcV=3, pValCutOff = 0.1):
+    """
+    The ConstrualValue22 function takes a scRNA-seq dataset datax,
+    a neural network model net, and several optional parameters to compute the "construal value" of each gene
+    in each cell of the dataset. The construal value represents the importance of each gene
+    to the identity of the cell.
+    The function first preprocesses the input data and normalizes it.
+    Then, it uses the DeepLift algorithm from the captum library to compute the construal value of each gene.
+    If the MarkerGeneFinder parameter is set to True,
+    the function performs a marker gene analysis using the computed construal values.
+    This analysis identifies genes that are differentially expressed between different cell clusters.
+    The results of the analysis are saved to an Excel file, and the top 100 marker genes for each cluster
+    are also saved to a separate CSV file. The function returns the updated datax object
+    with the computed construal values and the marker gene analysis results (if applicable).
+
+    """
+
     torch.manual_seed(0);
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     print("CamelRunning with %s"%device)
     if "test_set_values" in datax.obsm:
         mdf_train_set = pd.DataFrame(datax.obsm["test_set_values"].T, index=datax.uns["train_set_gene"],
                                  columns=datax.obs.index)
     elif "train_set_values" in datax.obsm:
@@ -1579,14 +1973,20 @@
             datax.uns["TopMarkerGene_Cluster"]=columnlist
         return datax
     else:
         return datax
 
 
 def ConstrualValueRef(datax,net, ConstrualModelvalue="DeepLift"):
+    """
+    This function aims to create a reference matrix for construal value prediction using the DeepLift model. The input parameters are:
+    datax: AnnData object, the dataset on which the reference matrix is to be constructed
+    net: Keras model, the neural network model used for prediction
+    ConstrualModelvalue: string, the type of method used for generating construal values, in this case "DeepLift"
+    """
     clist=[]
     for i in datax.uns['Celltype_OrderNumber']:
         datax=ConstrualValue22(datax=datax,net=net, filepath=None,targetvalue=i,
                                ConstrualModel="DeepLift",MarkerGeneFinder=False,
                                fcV=1.5, pValCutOff = 0.1)
         clist.append(datax.obsm['ConstrualValue_DeepLift'].T.sum(1).tolist())
     datax.uns['ConstrualValue_DeepLift_ClusterRef']=np.array(clist)
@@ -1625,14 +2025,22 @@
     dfrefv.index = datapdt.obs.index
     dfrefv = dfrefv / dfrefv.max()
     dfall = (dfrefv * dfref) ** 0.5
     datapdt.obsm["NormalizedMatrix"] = dfall.values
     return datapdt
     
 def MarkerDotPlot(datax,filepath, clustername):
+    """
+    Input Parameters:
+    datax: AnnData object containing the gene expression data
+    filepath: file path to the file containing the marker gene information
+    clustername: the name of the column in the marker gene file that contains the cluster labels
+    Output:
+    A scatter plot visualizing the marker gene expression across the specified clusters
+    """
     from mpl_toolkits.axes_grid1.inset_locator import inset_axes
     df=pd.DataFrame(datax.X.T,index=datax.var.index,columns=datax.obs.index)
     dfmk=pd.read_table(filepath,index_col=0,sep="\t")
     dfgrpref=df.loc[dfmk[clustername].dropna().values].T
     dfgrpref["Cluster"]=datax.obs["Cluster"]
     dfgrpref=dfgrpref[dfgrpref.columns[::-1]]
     dfmean=dfgrpref.groupby(["Cluster"]).mean()
@@ -1659,14 +2067,29 @@
     plt.colorbar(ax, anchor=(0.5,1),fraction=0.05)
     plt.grid("on",alpha=0.5)
     return ax
 
 
 def CellTypeSimilarity(datax, labelnum=False, RowCluster=True, fontsizeWeight=0.65,
                         ColCluster=True, metricvalue='correlation', methodvalue="average"):
+
+    """
+    Inputs:
+
+    datax: AnnData object containing the cell type scores in the obsm attribute and the cell cluster annotations in the obs attribute
+    labelnum: a boolean value indicating whether to show the average cell type scores in the heatmap or not (default=False)
+    RowCluster: a boolean value indicating whether to cluster rows (default=True)
+    fontsizeWeight: the font scale weight for the heatmap labels (default=0.65)
+    ColCluster: a boolean value indicating whether to cluster columns (default=True)
+    metricvalue: the distance metric to use when clustering (default='correlation')
+    methodvalue: the linkage method to use when clustering (default="average")
+    Outputs:
+
+    A heatmap visualizing the similarity of cell type scores across different cell clusters in the input AnnData object.
+    """
     dfprob = pd.DataFrame(datax.obsm['Celltype_Score'], index=datax.obs.index,
                           columns=datax.uns['Celltype_Score_RefCellType'])
     dfprob["Cluster"] = datax.obs["Cluster"]
     dfpb2 = dfprob.groupby(["Cluster"]).mean()
     dfpb2 = (dfpb2 + dfpb2.T) / 2
     correlations_array = np.asarray(np.log2(dfpb2.values + 1))
     if labelnum == False:
@@ -1724,14 +2147,29 @@
                             row_cluster=RowCluster, col_cluster=ColCluster,
                             figsize=(int(dfpb2.shape[1]), int(dfpb2.shape[0])), cmap="cividis")
         plt.setp(cg.ax_heatmap.yaxis.get_majorticklabels(), rotation=0, fontsize=15)
         plt.setp(cg.ax_heatmap.xaxis.get_majorticklabels(), rotation=90, fontsize=15)
 
 def SelfSimilarity(datax, labelnum=False, RowCluster=True,
                    ColCluster=True, metricvalue='correlation',methodvalue="average"):
+    """
+    datax: a Pandas dataframe containing cell type scores for each sample
+    labelnum: a boolean value indicating whether to annotate the heatmap with the values of the cell type scores
+    RowCluster: a boolean value indicating whether to cluster the rows of the heatmap
+    ColCluster: a boolean value indicating whether to cluster the columns of the heatmap
+    metricvalue: a string specifying the distance metric to be used for clustering
+    methodvalue: a string specifying the clustering method to be used
+    The function starts by creating a new dataframe dfprob by extracting cell type scores from the input dataframe datax and grouping them by cluster. It then calculates the average cell type score for each cluster and creates a symmetric dataframe dfpb2 by averaging the values of the cluster-cell type score matrix and its transpose.
+
+    If labelnum is set to False, the function generates a heatmap using Seaborn's clustermap function, with the log2-transformed dfpb2 dataframe as the input. The method and metric parameters specify the clustering method and distance metric to be used, respectively. The z_score parameter normalizes the data by subtracting the mean and dividing by the standard deviation. The heatmap is then displayed with the x and y axis tick labels set to a rotation of 90 and 0 degrees, respectively.
+
+    If labelnum is set to True, the function creates a similar heatmap with the addition of cell type score annotations. The annot parameter is set to labels, which is a rounded version of the dfpb2 dataframe values.
+
+    """
+
     dfprob = pd.DataFrame(datax.obsm['Celltype_Score'], index=datax.obs.index,
                           columns=datax.uns['Celltype_Score_RefCellType'])
     dfprob["Cluster"] = datax.obs["Cluster"]
     dfpb2 = dfprob.groupby(["Cluster"]).mean()
     dfpb2 = (dfpb2 + dfpb2.T) / 2
     if labelnum==False:
         sns.set(font_scale=1)
@@ -1760,18 +2198,41 @@
 def ConvertSparse(adata):
     if type(adata.X)==sparse.csr.csr_matrix:
         adata.X=adata.X.todense()
     return adata
 
 
 def writedata(adatax,filename,filepath=""):
+    """
+    Inputs:
+
+    df_dev: a pandas DataFrame containing gene expression data. Each row represents a gene, and each column represents a sample.
+    FeatureGenes: a list of gene names for which to calculate the feature enrichment score.
+    controlnumber: the number of control genes to use when calculating the score (default is 50).
+    cuts: the number of quantiles to divide the gene expression distribution into (default is 25).
+    Outputs:
+    FeatureScore: a numpy array of feature enrichment scores, with one score for each gene in FeatureGenes.
+    """
     adatax.X= sparse.csr_matrix(adatax.X)
     adatax.write(os.path.join(filepath, filename))
 
 def enrichmentscoreBETA(dfpfcclus, df_dev, fc=3, pvalcutoff=0.1, shortcut=True):
+    """
+    dfpfcclus: a pandas DataFrame containing the cluster labels for each cell in the gene expression data
+    df_dev: a pandas DataFrame containing the gene expression data for each cell
+    fc: a fold change threshold used for the enrichment score calculation
+    pvalcutoff: a p-value cutoff used for the enrichment score calculation
+    shortcut: a boolean value indicating whether to use a shortcut method for the calculation or not
+    The function first joins the two input DataFrames on the common cells and clusters, and then calculates the mean expression for each gene in each cluster. It then calculates the fold change of gene expression between each cluster and a control group (computed as the mean expression of all cells), and multiplies it by the ratio of the number of cells with non-zero expression of the gene in the cluster and control group. The resulting value is the enrichment score for each gene in each cluster.
+
+    If shortcut is set to True, the function uses a simplified method for the calculation, which involves calculating the fold change of gene expression between each cluster and the control group and filtering genes based on fold change and median expression values.
+
+    The function returns a pandas DataFrame containing the enriched genes for each cluster, along with their enrichment scores and gene expression values.
+
+    """
     # dfpfcclus = dfpfcclus, df_dev = df_dev, fc = 1.25, shortcut = True
     dfgrp = df_dev.T.astype(float).join(dfpfcclus.T, how="inner")
     dfmean = dfgrp.groupby(['Cluster']).mean()
     dfmedian = dfgrp.groupby(['Cluster']).median().T
     df_means = df_dev.mean(1)
     if shortcut == False:
         print("Camel...Running: clusteringValue1...")
@@ -1910,7 +2371,41 @@
             # setup toolbar
 
             sys.stdout.write("-%s%%-" % int(itemindex * 100 / perc))
             sys.stdout.flush()
         print("Camel...Running: output genelist...")
         return genelist
 
+
+
+
+def FeatureEnrichScore(df_dev, FeatureGenes, controlnumber=50, cuts=25):
+    """
+    Inputs:
+    df_dev: a pandas DataFrame containing gene expression data. Each row represents a gene, and each column represents a sample.
+    FeatureGenes: a list of gene names for which to calculate the feature enrichment score.
+    controlnumber: the number of control genes to use when calculating the score (default is 50).
+    cuts: the number of quantiles to divide the gene expression distribution into (default is 25).
+    Outputs:
+    FeatureScore: a numpy array of feature enrichment scores, with one score for each gene in FeatureGenes.
+    """
+
+    var_names = df_dev.index
+    gene_list = FeatureGenes
+
+    obs_avg = df_dev.mean(1)
+    obs_avg = obs_avg[np.isfinite(obs_avg)]
+    n_items = int(np.round(len(obs_avg) / cuts))
+    obs_cut = obs_avg.rank(method='min') // n_items
+
+    ctrl_size = controlnumber
+    control_genes = set()
+    for cut in np.unique(obs_cut.loc[gene_list]):
+        r_genes = np.array(obs_cut[obs_cut == cut].index)
+        np.random.shuffle(r_genes)
+        control_genes.update(set(r_genes[:ctrl_size]))
+    control_genes = list(control_genes - set(gene_list))
+    gene_list = list(gene_list)
+    X_list = df_dev.loc[gene_list].T.values
+    X_control = df_dev.loc[control_genes].mean().values
+    FeatureScore = np.nanmean(X_list, axis=1) - X_control
+    return FeatureScore
```

### Comparing `scCAMEL-0.24b0/src/scCAMEL.egg-info/PKG-INFO` & `scCAMEL-0.25b0/src/scCAMEL.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: scCAMEL
-Version: 0.24b0
-Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
-Home-page: https://sccamel.readthedocs.io/
-Author: Yizhou Hu
-Author-email: yizhou.hu@ki.se
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory
-
-License: GPL version 3
-https://pypi.org/project/scCAMEL/
-
-Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet
-
-Tutorials and other informations in :
-https://sccamel.readthedocs.io/
+Metadata-Version: 2.1
+Name: scCAMEL
+Version: 0.25b0
+Summary: scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory;License: GPL version 3;Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet;Tutorials and other informations in :https://sccamel.readthedocs.io/
+Home-page: https://sccamel.readthedocs.io/
+Author: Yizhou Hu
+Author-email: yizhou.hu@ki.se
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+scCAMEL: single cell Cross- Annotation and Multimodal Estimation on Lineage trajectory
+
+License: GPL version 3
+https://pypi.org/project/scCAMEL/
+
+Developed by: Yizhou Hu, Patrik Ernfors lab, MBB, Karolinska Institutet
+
+Tutorials and other informations in :
+https://sccamel.readthedocs.io/
```

