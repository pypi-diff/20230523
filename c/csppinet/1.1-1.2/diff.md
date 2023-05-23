# Comparing `tmp/csppinet-1.1.tar.gz` & `tmp/csppinet-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csppinet-1.1.tar", last modified: Tue May 23 20:29:05 2023, max compression
+gzip compressed data, was "csppinet-1.2.tar", last modified: Tue May 23 21:33:39 2023, max compression
```

## Comparing `csppinet-1.1.tar` & `csppinet-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lucasmiguel  (2303) lucasmiguel  (2304)        0 2023-05-23 20:29:05.060857 csppinet-1.1/
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     7324 2023-05-23 20:29:05.060857 csppinet-1.1/PKG-INFO
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     5535 2023-05-23 02:48:33.000000 csppinet-1.1/README.md
-drwxrwxr-x   0 lucasmiguel  (2303) lucasmiguel  (2304)        0 2023-05-23 20:29:05.060857 csppinet-1.1/csppinet/
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)      461 2023-05-20 07:36:21.000000 csppinet-1.1/csppinet/__init__.py
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     6445 2023-05-23 16:14:19.000000 csppinet-1.1/csppinet/construction.py
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     2621 2023-05-23 20:25:35.000000 csppinet-1.1/csppinet/csppinet.py
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     2681 2023-05-23 16:05:04.000000 csppinet-1.1/csppinet/functions.py
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     3536 2023-05-23 16:18:50.000000 csppinet-1.1/csppinet/network_metrics.py
-drwxrwxr-x   0 lucasmiguel  (2303) lucasmiguel  (2304)        0 2023-05-23 20:29:05.060857 csppinet-1.1/csppinet.egg-info/
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     7324 2023-05-23 20:29:04.000000 csppinet-1.1/csppinet.egg-info/PKG-INFO
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)      329 2023-05-23 20:29:05.000000 csppinet-1.1/csppinet.egg-info/SOURCES.txt
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)        1 2023-05-23 20:29:04.000000 csppinet-1.1/csppinet.egg-info/dependency_links.txt
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)       53 2023-05-23 20:29:04.000000 csppinet-1.1/csppinet.egg-info/entry_points.txt
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)       27 2023-05-23 20:29:04.000000 csppinet-1.1/csppinet.egg-info/requires.txt
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)        9 2023-05-23 20:29:04.000000 csppinet-1.1/csppinet.egg-info/top_level.txt
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)       38 2023-05-23 20:29:05.060857 csppinet-1.1/setup.cfg
--rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     2085 2023-05-23 20:28:39.000000 csppinet-1.1/setup.py
+drwxrwxr-x   0 lucasmiguel  (2303) lucasmiguel  (2304)        0 2023-05-23 21:33:39.072472 csppinet-1.2/
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     6405 2023-05-23 21:33:39.072472 csppinet-1.2/PKG-INFO
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     5535 2023-05-23 02:48:33.000000 csppinet-1.2/README.md
+drwxrwxr-x   0 lucasmiguel  (2303) lucasmiguel  (2304)        0 2023-05-23 21:33:39.072472 csppinet-1.2/csppinet/
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)      461 2023-05-20 07:36:21.000000 csppinet-1.2/csppinet/__init__.py
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     6459 2023-05-23 21:25:30.000000 csppinet-1.2/csppinet/construction.py
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     2621 2023-05-23 21:26:03.000000 csppinet-1.2/csppinet/csppinet.py
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     2681 2023-05-23 16:05:04.000000 csppinet-1.2/csppinet/functions.py
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     3536 2023-05-23 16:18:50.000000 csppinet-1.2/csppinet/network_metrics.py
+drwxrwxr-x   0 lucasmiguel  (2303) lucasmiguel  (2304)        0 2023-05-23 21:33:39.072472 csppinet-1.2/csppinet.egg-info/
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     6405 2023-05-23 21:33:38.000000 csppinet-1.2/csppinet.egg-info/PKG-INFO
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)      329 2023-05-23 21:33:38.000000 csppinet-1.2/csppinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)        1 2023-05-23 21:33:38.000000 csppinet-1.2/csppinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)       52 2023-05-23 21:33:38.000000 csppinet-1.2/csppinet.egg-info/entry_points.txt
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)       27 2023-05-23 21:33:38.000000 csppinet-1.2/csppinet.egg-info/requires.txt
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)        9 2023-05-23 21:33:38.000000 csppinet-1.2/csppinet.egg-info/top_level.txt
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)       38 2023-05-23 21:33:39.072472 csppinet-1.2/setup.cfg
+-rw-rw-r--   0 lucasmiguel  (2303) lucasmiguel  (2304)     2085 2023-05-23 21:33:34.000000 csppinet-1.2/setup.py
```

### Comparing `csppinet-1.1/PKG-INFO` & `csppinet-1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,131 +1,130 @@
 Metadata-Version: 2.1
 Name: csppinet
-Version: 1.1
+Version: 1.2
 Summary: A Python package for context-specific protein-protein interaction network construction and analysis based on omics data.
 Home-page: https://github.com/lmigueel/csppinet/
 Author: Luca Miguel de Carvalho
 Author-email: lucasmigueel@gmail.com
 License: GNU General Public License v3.0
-Description: # csppinet
-        csppinet: A Python package for context-specific biological network construction and analysis based on omics data
-        
-        ```shell
-         ██████ ███████ ██████  ██████  ██ ███    ██ ███████ ████████ 
-        ██      ██      ██   ██ ██   ██ ██ ████   ██ ██         ██    
-        ██      ███████ ██████  ██████  ██ ██ ██  ██ █████      ██    
-        ██           ██ ██      ██      ██ ██  ██ ██ ██         ██    
-         ██████ ███████ ██      ██      ██ ██   ████ ███████    ██ 
-         ```
-                version 1.0
-        
-        
-        - [Installation](#installing)
-        - [Overview](#overview)
-        - [Workflow](#workflow)
-        - [Command-line interface](#command-line-interface)
-        - [Python library usage](#python-library-usage)
-        - [Examples](#examples)
-        - [Article](#article)
-        
-        # Installing
-        
-        To build and install from source, run
-        
-        ```shell
-        python setup.py install
-        ```
-        You can also install from pip with
-        
-        ```shell
-        pip install csppinet
-        ``` 
-        
-        # Overview
-        
-        csppinet construct a context-specific biological network based on omics data. From omics data, such as temporal transcriptome data, csppinet generates a context-specific network for each biological condition. It provides both an easy-to-use object-oriented Python API and a command-line interface (CLI) for context-specific network construction and post-analysis. 
-        
-        In order to fully leverage the capabilities of our package and obtain comprehensive insights, it is crucial to have a diverse and substantial number of biological conditions available for analysis, because the main function to determine a protein activity is based on [three-sigma method](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/10.1002/pmic.201200277).
-        
-        # Workflow
-        
-        csppinet contains a flowchart designed to provide a structured context-specific (cs) network based on omics data, as well metrics and comparative reports.
-        
-        csppinet features include:
-        
-                1. The construction of a context-specific network based on omics data. We account for gene activity across biological conditions, and then take this activity for each network interaction, where it remains if both genes are active;
-                2. The calculation of network metrics for the genes for each context-specific network;
-                3. The calculation of network metrics for each context-specific network.
-        
-        # Command-line interface
-        
-        csppinet can be executed from the command line using the csppinet command. It takes the network and the gene expression file, as well the number of threads (essential for large networks). 
-        
-        ```
-        usage: csppinet [-h] --network_file network.csv --expression_file gene_expression.csv --method METHOD --value VALUE --threads THREADS
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --network_file        A csv file containing the network
-          --expression_file     A csv file containing the expression of the genes per condition
-          --method              A method to determine protein expression. Choose between "3-sigma", "percentile" or "pre-threshold". 
-          --value               A threshold value for "pre-threshold" or "percentile" method.  In the 'pre-threshold' method, the threshold value represents an absolute threshold for gene expression. On the other hand, in the 'percentile' method, the threshold value corresponds to the percentile cutoff. For example, a value of 5 represents the 5th percentile, while a value of 25 represents the 25th percentile or the first quartile. 
-          --threads     Number of threads for multiprocessing. Considere it for large networks
-        
-        example:  python3 csppinet.py --network_file network.csv --expression_file gene_expession.csv --method pre-threshold --value 2 --threads 2
-        ```
-        In your current working folder, csppinet generates the following outputs:
-        
-                1. A csv file containing the context-specific network for each biological condition ("csppinet_csnetwork" prefix);
-                2. A csv file containing the network metrics for the genes of each context-specific network ("csppinet_GenesMetrics" prefix);
-                3. A txt file containing the network metrics report file for each cs network ("csppinet_Reports" prefix).
-                4. A csv file for the metrics Betweenness Centrality (BC), Closeness Centrality (CC) and Degree for all biological conditions in expression file.
-         
-        # Python library usage
-        
-        csppinet generates the files in the  current working directory. 
-        
-        To use as a Python library
-        
-        ```python
-        
-        import csppinet
-        
-        # csppinet arguments. Input files should be in .csv extension 
-        network = '/opt/data/network.csv'
-        exp = '/opt/data/expression_file.csv'
-        threads = 10
-        method = "percentile"
-        value = 25 
-        
-        #construction
-        csppinet.construction(network,exp,threads,method,value)
-        
-        #network metrics
-        csppinet.network_metrics(exp)
-        
-        ```
-        
-        # Examples
-        
-        In these examples we will use as input the network of **Saccharomyces cerevisiae** from STRINGdb with "combined_score" > 900 together with gene expression data from the article by de Carvalho, et al. 2021 (https://doi.org/10.1093/femsyr/foab030). You could find the script in the Article section (next one).
-        
-        ```shell
-        csppinet --network_file STRING_yeast.csv --expression_file expression_deCarvalho2021.csv --threads 10 --method pre-threshold --value 5
-        ```
-        
-        # Article
-        
-        For application examples, scripts and datasets access the package article on BioRxiv.
-        
-        
 Keywords: bioinformatics,context-specific network,PPI network,interactome,network analysis,omics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# csppinet
+csppinet: A Python package for context-specific biological network construction and analysis based on omics data
+
+```shell
+ ██████ ███████ ██████  ██████  ██ ███    ██ ███████ ████████ 
+██      ██      ██   ██ ██   ██ ██ ████   ██ ██         ██    
+██      ███████ ██████  ██████  ██ ██ ██  ██ █████      ██    
+██           ██ ██      ██      ██ ██  ██ ██ ██         ██    
+ ██████ ███████ ██      ██      ██ ██   ████ ███████    ██ 
+ ```
+        version 1.0
+
+
+- [Installation](#installing)
+- [Overview](#overview)
+- [Workflow](#workflow)
+- [Command-line interface](#command-line-interface)
+- [Python library usage](#python-library-usage)
+- [Examples](#examples)
+- [Article](#article)
+
+# Installing
+
+To build and install from source, run
+
+```shell
+python setup.py install
+```
+You can also install from pip with
+
+```shell
+pip install csppinet
+``` 
+
+# Overview
+
+csppinet construct a context-specific biological network based on omics data. From omics data, such as temporal transcriptome data, csppinet generates a context-specific network for each biological condition. It provides both an easy-to-use object-oriented Python API and a command-line interface (CLI) for context-specific network construction and post-analysis. 
+
+In order to fully leverage the capabilities of our package and obtain comprehensive insights, it is crucial to have a diverse and substantial number of biological conditions available for analysis, because the main function to determine a protein activity is based on [three-sigma method](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/10.1002/pmic.201200277).
+
+# Workflow
+
+csppinet contains a flowchart designed to provide a structured context-specific (cs) network based on omics data, as well metrics and comparative reports.
+
+csppinet features include:
+
+        1. The construction of a context-specific network based on omics data. We account for gene activity across biological conditions, and then take this activity for each network interaction, where it remains if both genes are active;
+        2. The calculation of network metrics for the genes for each context-specific network;
+        3. The calculation of network metrics for each context-specific network.
+
+# Command-line interface
+
+csppinet can be executed from the command line using the csppinet command. It takes the network and the gene expression file, as well the number of threads (essential for large networks). 
+
+```
+usage: csppinet [-h] --network_file network.csv --expression_file gene_expression.csv --method METHOD --value VALUE --threads THREADS
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --network_file        A csv file containing the network
+  --expression_file     A csv file containing the expression of the genes per condition
+  --method              A method to determine protein expression. Choose between "3-sigma", "percentile" or "pre-threshold". 
+  --value               A threshold value for "pre-threshold" or "percentile" method.  In the 'pre-threshold' method, the threshold value represents an absolute threshold for gene expression. On the other hand, in the 'percentile' method, the threshold value corresponds to the percentile cutoff. For example, a value of 5 represents the 5th percentile, while a value of 25 represents the 25th percentile or the first quartile. 
+  --threads     Number of threads for multiprocessing. Considere it for large networks
+
+example:  python3 csppinet.py --network_file network.csv --expression_file gene_expession.csv --method pre-threshold --value 2 --threads 2
+```
+In your current working folder, csppinet generates the following outputs:
+
+        1. A csv file containing the context-specific network for each biological condition ("csppinet_csnetwork" prefix);
+        2. A csv file containing the network metrics for the genes of each context-specific network ("csppinet_GenesMetrics" prefix);
+        3. A txt file containing the network metrics report file for each cs network ("csppinet_Reports" prefix).
+        4. A csv file for the metrics Betweenness Centrality (BC), Closeness Centrality (CC) and Degree for all biological conditions in expression file.
+ 
+# Python library usage
+
+csppinet generates the files in the  current working directory. 
+
+To use as a Python library
+
+```python
+
+import csppinet
+
+# csppinet arguments. Input files should be in .csv extension 
+network = '/opt/data/network.csv'
+exp = '/opt/data/expression_file.csv'
+threads = 10
+method = "percentile"
+value = 25 
+
+#construction
+csppinet.construction(network,exp,threads,method,value)
+
+#network metrics
+csppinet.network_metrics(exp)
+
+```
+
+# Examples
+
+In these examples we will use as input the network of **Saccharomyces cerevisiae** from STRINGdb with "combined_score" > 900 together with gene expression data from the article by de Carvalho, et al. 2021 (https://doi.org/10.1093/femsyr/foab030). You could find the script in the Article section (next one).
+
+```shell
+csppinet --network_file STRING_yeast.csv --expression_file expression_deCarvalho2021.csv --threads 10 --method pre-threshold --value 5
+```
+
+# Article
+
+For application examples, scripts and datasets access the package article on BioRxiv.
+
```

### Comparing `csppinet-1.1/README.md` & `csppinet-1.2/README.md`

 * *Files identical despite different names*

### Comparing `csppinet-1.1/csppinet/construction.py` & `csppinet-1.2/csppinet/construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     allowed_values = ["3-sigma", "pre-threshold","percentile"]
 
     if method in allowed_values:
         # Proceed with the desired functionality
         print("Step 2: Processing with method", method)
     else:
         # Stop and produce an error message
-        print("Invalid argument! Please enter either '3-sigma' or 'pre-threshold'.")
+        print("Invalid argument! Please enter either '3-sigma', 'percentile' or 'pre-threshold'.")
         sys.exit(1)
 
 
     # Create an empty dictionary to store the interactomes
     interactomes = {}
 
     # Iterate over each biological condition
```

### Comparing `csppinet-1.1/csppinet/csppinet.py` & `csppinet-1.2/csppinet/csppinet.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import sys
 import csppinet
 
 
 def csppinet_cli(network_file, expression_file,threads, method,value):
 	""" Biological network generation and analysis."""
 
-	csppinet.construction(network_file,expression_file,method,value,threads)
+	csppinet.construction(network_file,expression_file,threads,method,value)
 	csppinet.network_metrics(expression_file)
 	
 def main():
 
 
     usage_text = '''example:
```

### Comparing `csppinet-1.1/csppinet/functions.py` & `csppinet-1.2/csppinet/functions.py`

 * *Files identical despite different names*

### Comparing `csppinet-1.1/csppinet/network_metrics.py` & `csppinet-1.2/csppinet/network_metrics.py`

 * *Files identical despite different names*

### Comparing `csppinet-1.1/csppinet.egg-info/PKG-INFO` & `csppinet-1.2/csppinet.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,131 +1,130 @@
 Metadata-Version: 2.1
 Name: csppinet
-Version: 1.1
+Version: 1.2
 Summary: A Python package for context-specific protein-protein interaction network construction and analysis based on omics data.
 Home-page: https://github.com/lmigueel/csppinet/
 Author: Luca Miguel de Carvalho
 Author-email: lucasmigueel@gmail.com
 License: GNU General Public License v3.0
-Description: # csppinet
-        csppinet: A Python package for context-specific biological network construction and analysis based on omics data
-        
-        ```shell
-         ██████ ███████ ██████  ██████  ██ ███    ██ ███████ ████████ 
-        ██      ██      ██   ██ ██   ██ ██ ████   ██ ██         ██    
-        ██      ███████ ██████  ██████  ██ ██ ██  ██ █████      ██    
-        ██           ██ ██      ██      ██ ██  ██ ██ ██         ██    
-         ██████ ███████ ██      ██      ██ ██   ████ ███████    ██ 
-         ```
-                version 1.0
-        
-        
-        - [Installation](#installing)
-        - [Overview](#overview)
-        - [Workflow](#workflow)
-        - [Command-line interface](#command-line-interface)
-        - [Python library usage](#python-library-usage)
-        - [Examples](#examples)
-        - [Article](#article)
-        
-        # Installing
-        
-        To build and install from source, run
-        
-        ```shell
-        python setup.py install
-        ```
-        You can also install from pip with
-        
-        ```shell
-        pip install csppinet
-        ``` 
-        
-        # Overview
-        
-        csppinet construct a context-specific biological network based on omics data. From omics data, such as temporal transcriptome data, csppinet generates a context-specific network for each biological condition. It provides both an easy-to-use object-oriented Python API and a command-line interface (CLI) for context-specific network construction and post-analysis. 
-        
-        In order to fully leverage the capabilities of our package and obtain comprehensive insights, it is crucial to have a diverse and substantial number of biological conditions available for analysis, because the main function to determine a protein activity is based on [three-sigma method](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/10.1002/pmic.201200277).
-        
-        # Workflow
-        
-        csppinet contains a flowchart designed to provide a structured context-specific (cs) network based on omics data, as well metrics and comparative reports.
-        
-        csppinet features include:
-        
-                1. The construction of a context-specific network based on omics data. We account for gene activity across biological conditions, and then take this activity for each network interaction, where it remains if both genes are active;
-                2. The calculation of network metrics for the genes for each context-specific network;
-                3. The calculation of network metrics for each context-specific network.
-        
-        # Command-line interface
-        
-        csppinet can be executed from the command line using the csppinet command. It takes the network and the gene expression file, as well the number of threads (essential for large networks). 
-        
-        ```
-        usage: csppinet [-h] --network_file network.csv --expression_file gene_expression.csv --method METHOD --value VALUE --threads THREADS
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --network_file        A csv file containing the network
-          --expression_file     A csv file containing the expression of the genes per condition
-          --method              A method to determine protein expression. Choose between "3-sigma", "percentile" or "pre-threshold". 
-          --value               A threshold value for "pre-threshold" or "percentile" method.  In the 'pre-threshold' method, the threshold value represents an absolute threshold for gene expression. On the other hand, in the 'percentile' method, the threshold value corresponds to the percentile cutoff. For example, a value of 5 represents the 5th percentile, while a value of 25 represents the 25th percentile or the first quartile. 
-          --threads     Number of threads for multiprocessing. Considere it for large networks
-        
-        example:  python3 csppinet.py --network_file network.csv --expression_file gene_expession.csv --method pre-threshold --value 2 --threads 2
-        ```
-        In your current working folder, csppinet generates the following outputs:
-        
-                1. A csv file containing the context-specific network for each biological condition ("csppinet_csnetwork" prefix);
-                2. A csv file containing the network metrics for the genes of each context-specific network ("csppinet_GenesMetrics" prefix);
-                3. A txt file containing the network metrics report file for each cs network ("csppinet_Reports" prefix).
-                4. A csv file for the metrics Betweenness Centrality (BC), Closeness Centrality (CC) and Degree for all biological conditions in expression file.
-         
-        # Python library usage
-        
-        csppinet generates the files in the  current working directory. 
-        
-        To use as a Python library
-        
-        ```python
-        
-        import csppinet
-        
-        # csppinet arguments. Input files should be in .csv extension 
-        network = '/opt/data/network.csv'
-        exp = '/opt/data/expression_file.csv'
-        threads = 10
-        method = "percentile"
-        value = 25 
-        
-        #construction
-        csppinet.construction(network,exp,threads,method,value)
-        
-        #network metrics
-        csppinet.network_metrics(exp)
-        
-        ```
-        
-        # Examples
-        
-        In these examples we will use as input the network of **Saccharomyces cerevisiae** from STRINGdb with "combined_score" > 900 together with gene expression data from the article by de Carvalho, et al. 2021 (https://doi.org/10.1093/femsyr/foab030). You could find the script in the Article section (next one).
-        
-        ```shell
-        csppinet --network_file STRING_yeast.csv --expression_file expression_deCarvalho2021.csv --threads 10 --method pre-threshold --value 5
-        ```
-        
-        # Article
-        
-        For application examples, scripts and datasets access the package article on BioRxiv.
-        
-        
 Keywords: bioinformatics,context-specific network,PPI network,interactome,network analysis,omics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# csppinet
+csppinet: A Python package for context-specific biological network construction and analysis based on omics data
+
+```shell
+ ██████ ███████ ██████  ██████  ██ ███    ██ ███████ ████████ 
+██      ██      ██   ██ ██   ██ ██ ████   ██ ██         ██    
+██      ███████ ██████  ██████  ██ ██ ██  ██ █████      ██    
+██           ██ ██      ██      ██ ██  ██ ██ ██         ██    
+ ██████ ███████ ██      ██      ██ ██   ████ ███████    ██ 
+ ```
+        version 1.0
+
+
+- [Installation](#installing)
+- [Overview](#overview)
+- [Workflow](#workflow)
+- [Command-line interface](#command-line-interface)
+- [Python library usage](#python-library-usage)
+- [Examples](#examples)
+- [Article](#article)
+
+# Installing
+
+To build and install from source, run
+
+```shell
+python setup.py install
+```
+You can also install from pip with
+
+```shell
+pip install csppinet
+``` 
+
+# Overview
+
+csppinet construct a context-specific biological network based on omics data. From omics data, such as temporal transcriptome data, csppinet generates a context-specific network for each biological condition. It provides both an easy-to-use object-oriented Python API and a command-line interface (CLI) for context-specific network construction and post-analysis. 
+
+In order to fully leverage the capabilities of our package and obtain comprehensive insights, it is crucial to have a diverse and substantial number of biological conditions available for analysis, because the main function to determine a protein activity is based on [three-sigma method](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/10.1002/pmic.201200277).
+
+# Workflow
+
+csppinet contains a flowchart designed to provide a structured context-specific (cs) network based on omics data, as well metrics and comparative reports.
+
+csppinet features include:
+
+        1. The construction of a context-specific network based on omics data. We account for gene activity across biological conditions, and then take this activity for each network interaction, where it remains if both genes are active;
+        2. The calculation of network metrics for the genes for each context-specific network;
+        3. The calculation of network metrics for each context-specific network.
+
+# Command-line interface
+
+csppinet can be executed from the command line using the csppinet command. It takes the network and the gene expression file, as well the number of threads (essential for large networks). 
+
+```
+usage: csppinet [-h] --network_file network.csv --expression_file gene_expression.csv --method METHOD --value VALUE --threads THREADS
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --network_file        A csv file containing the network
+  --expression_file     A csv file containing the expression of the genes per condition
+  --method              A method to determine protein expression. Choose between "3-sigma", "percentile" or "pre-threshold". 
+  --value               A threshold value for "pre-threshold" or "percentile" method.  In the 'pre-threshold' method, the threshold value represents an absolute threshold for gene expression. On the other hand, in the 'percentile' method, the threshold value corresponds to the percentile cutoff. For example, a value of 5 represents the 5th percentile, while a value of 25 represents the 25th percentile or the first quartile. 
+  --threads     Number of threads for multiprocessing. Considere it for large networks
+
+example:  python3 csppinet.py --network_file network.csv --expression_file gene_expession.csv --method pre-threshold --value 2 --threads 2
+```
+In your current working folder, csppinet generates the following outputs:
+
+        1. A csv file containing the context-specific network for each biological condition ("csppinet_csnetwork" prefix);
+        2. A csv file containing the network metrics for the genes of each context-specific network ("csppinet_GenesMetrics" prefix);
+        3. A txt file containing the network metrics report file for each cs network ("csppinet_Reports" prefix).
+        4. A csv file for the metrics Betweenness Centrality (BC), Closeness Centrality (CC) and Degree for all biological conditions in expression file.
+ 
+# Python library usage
+
+csppinet generates the files in the  current working directory. 
+
+To use as a Python library
+
+```python
+
+import csppinet
+
+# csppinet arguments. Input files should be in .csv extension 
+network = '/opt/data/network.csv'
+exp = '/opt/data/expression_file.csv'
+threads = 10
+method = "percentile"
+value = 25 
+
+#construction
+csppinet.construction(network,exp,threads,method,value)
+
+#network metrics
+csppinet.network_metrics(exp)
+
+```
+
+# Examples
+
+In these examples we will use as input the network of **Saccharomyces cerevisiae** from STRINGdb with "combined_score" > 900 together with gene expression data from the article by de Carvalho, et al. 2021 (https://doi.org/10.1093/femsyr/foab030). You could find the script in the Article section (next one).
+
+```shell
+csppinet --network_file STRING_yeast.csv --expression_file expression_deCarvalho2021.csv --threads 10 --method pre-threshold --value 5
+```
+
+# Article
+
+For application examples, scripts and datasets access the package article on BioRxiv.
+
```

### Comparing `csppinet-1.1/setup.py` & `csppinet-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 setup(
     name='csppinet',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
     license='GNU General Public License v3.0',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     description='A Python package for context-specific protein-protein interaction network construction and analysis based on omics data.',
     install_requires=[ 'numpy', 'pandas', 'networkx >= 2.5'],
     python_requires='>=3',
```

