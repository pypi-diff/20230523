# Comparing `tmp/PyBerries-0.2.8.post1.tar.gz` & `tmp/PyBerries-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.8.post1.tar", last modified: Wed May 10 14:53:54 2023, max compression
+gzip compressed data, was "PyBerries-0.2.9.tar", last modified: Wed May 17 10:08:05 2023, max compression
```

## Comparing `PyBerries-0.2.8.post1.tar` & `PyBerries-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.235192 PyBerries-0.2.8.post1/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.8.post1/LICENSE
--rw-rw-rw-   0        0        0     2202 2023-05-10 14:53:54.235192 PyBerries-0.2.8.post1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.211193 PyBerries-0.2.8.post1/PyBerries.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-05-10 14:53:54.000000 PyBerries-0.2.8.post1/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-05-10 14:53:54.000000 PyBerries-0.2.8.post1/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:53:54.000000 PyBerries-0.2.8.post1/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-05-10 14:53:54.000000 PyBerries-0.2.8.post1/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 14:53:54.000000 PyBerries-0.2.8.post1/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1890 2023-05-10 14:47:29.000000 PyBerries-0.2.8.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.211193 PyBerries-0.2.8.post1/pyberries/
--rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.8.post1/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.219193 PyBerries-0.2.8.post1/pyberries/data/
--rw-rw-rw-   0        0        0    15750 2023-05-10 13:22:01.000000 PyBerries-0.2.8.post1/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     3083 2023-05-08 13:08:41.000000 PyBerries-0.2.8.post1/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.8.post1/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.8.post1/pyberries/data/util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.227193 PyBerries-0.2.8.post1/pyberries/file_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.8.post1/pyberries/file_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.8.post1/pyberries/file_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.8.post1/pyberries/file_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.8.post1/pyberries/file_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.227193 PyBerries-0.2.8.post1/pyberries/metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.8.post1/pyberries/metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.8.post1/pyberries/metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.8.post1/pyberries/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:53:54.235192 PyBerries-0.2.8.post1/pyberries/plots/
--rw-rw-rw-   0        0        0     5459 2023-05-10 09:21:07.000000 PyBerries-0.2.8.post1/pyberries/plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.8.post1/pyberries/plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1463 2023-05-10 08:28:13.000000 PyBerries-0.2.8.post1/pyberries/plots/Plots.py
--rw-rw-rw-   0        0        0       96 2023-05-08 14:30:38.000000 PyBerries-0.2.8.post1/pyberries/plots/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-10 14:53:54.235192 PyBerries-0.2.8.post1/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-05-10 14:52:51.000000 PyBerries-0.2.8.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.580360 PyBerries-0.2.9/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     2909 2023-05-17 10:08:05.580360 PyBerries-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.567359 PyBerries-0.2.9/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0     2909 2023-05-17 10:08:05.000000 PyBerries-0.2.9/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-05-17 10:08:05.000000 PyBerries-0.2.9/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:08:05.000000 PyBerries-0.2.9/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-05-17 10:08:05.000000 PyBerries-0.2.9/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 10:08:05.000000 PyBerries-0.2.9/PyBerries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2603 2023-05-11 12:43:56.000000 PyBerries-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.568360 PyBerries-0.2.9/pyberries/
+-rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.9/pyberries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.572359 PyBerries-0.2.9/pyberries/data/
+-rw-rw-rw-   0        0        0    16806 2023-05-16 12:53:07.000000 PyBerries-0.2.9/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     3083 2023-05-08 13:08:41.000000 PyBerries-0.2.9/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.9/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.9/pyberries/data/util.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.575359 PyBerries-0.2.9/pyberries/file_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.9/pyberries/file_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.9/pyberries/file_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.9/pyberries/file_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.9/pyberries/file_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.577359 PyBerries-0.2.9/pyberries/metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.9/pyberries/metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.9/pyberries/metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.9/pyberries/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:08:05.579360 PyBerries-0.2.9/pyberries/plots/
+-rw-rw-rw-   0        0        0     5445 2023-05-16 15:33:21.000000 PyBerries-0.2.9/pyberries/plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.9/pyberries/plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1556 2023-05-17 08:22:16.000000 PyBerries-0.2.9/pyberries/plots/Plots.py
+-rw-rw-rw-   0        0        0       96 2023-05-08 14:30:38.000000 PyBerries-0.2.9/pyberries/plots/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:08:05.580360 PyBerries-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-05-15 15:11:46.000000 PyBerries-0.2.9/setup.py
```

### Comparing `PyBerries-0.2.8.post1/LICENSE` & `PyBerries-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/PKG-INFO` & `PyBerries-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.8.post1
+Version: 0.2.9
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyBerries
 
 PyBerries is a Python package that can be used to import, manipulate and plot data from Bacmman measurement tables.
 
 It relies mainly on Pandas for data handling and Seaborn/Matplotlib for plotting.
 
-[[_TOC_]]
-
-----
 
 ## Installation
 
-### Anaconda (recommended)
+### Optional: install Jupyter-lab (to run Jupyter Notebooks)
+
+#### Anaconda (recommended)
 
   Anaconda will install both Python and Jupyter-lab (used to run Python notebooks) easily. Note however that it requires ~5 Gb free disk space.
   For a lighter installation procedure, see the next section "Command line install".
 
   - Download Anaconda from the [official website](https://www.anaconda.com/)
   - Run the installer (leave all options as default)
   - Start "Anaconda Navigator"
-  - In Anaconda, launch the "Jupyter Lab" module
+  - In Anaconda, launch the "Jupyter Lab" module (you might need to click on "Install" first)
 
-### Command line install (advanced users)
+#### Command line install
 
   - Open a terminal (macOS/Linux) or Powershell (Windows)
   - Install Python
       - Enter the command `python --version`
       - If an error or a version < 3.9 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
-  - After installing, restart your terminal/powershell; both of the above commands should display a version number
+  - After installing, restart your terminal/powershell; the `python --version` command should display a version number > 3.9
   - Install Jupyter Lab
       - In a terminal/powershell, run the command `python -m pip install jupyterlab`
       - After the installation completes, Jupyter Lab can be started using the command `jupyter-lab`
 
+### Installing the package
+
+To install the package, use the following command in a terminal:
+
+`python -m pip install PyBerries`
+
+You can also install a specific version number (useful e.g. to make sure you code won't be broken by a future update):
+
+`python -m pip install PyBerries==0.2.8`
+
+In a jupyter notebook, use the command:
+
+`%pip install PyBerries`, or `%pip install PyBerries==0.2.8` for a specific version.
+
 
 ## Getting started
 
-Try downloading and running the [tutorial notebook](./Tutorial/Tutorial.ipynb) to get acquainted with data import and plotting in PyBerries.
+Try downloading and running the [tutorial notebook](https://gitlab.com/MEKlab/pyberries/-/raw/main/Tutorial/Tutorial.ipynb?inline=false) to get acquainted with data import and plotting in PyBerries.
 
-For further details, see the [main functionalities](./doc/PyBerries_main_functionalities.md) documentation, as well as the [DatasetPool](./doc/DatasetPool.md) documentation.
+For further details, see the [main functionalities](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/PyBerries_main_functionalities.md) documentation, as well as the [DatasetPool](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/DatasetPool.md) documentation.
 
-For info and examples on plots, see the [preset plots gallery](./doc/Plot_preset_gallery.md) and the [Seaborn documentation](https://seaborn.pydata.org/index.html)
+For info and examples on plots, see the [preset plots gallery](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/Plot_preset_gallery.md) and the [Seaborn documentation](https://seaborn.pydata.org/index.html)
```

### Comparing `PyBerries-0.2.8.post1/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.9/PyBerries.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.8.post1
+Version: 0.2.9
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyBerries
 
 PyBerries is a Python package that can be used to import, manipulate and plot data from Bacmman measurement tables.
 
 It relies mainly on Pandas for data handling and Seaborn/Matplotlib for plotting.
 
-[[_TOC_]]
-
-----
 
 ## Installation
 
-### Anaconda (recommended)
+### Optional: install Jupyter-lab (to run Jupyter Notebooks)
+
+#### Anaconda (recommended)
 
   Anaconda will install both Python and Jupyter-lab (used to run Python notebooks) easily. Note however that it requires ~5 Gb free disk space.
   For a lighter installation procedure, see the next section "Command line install".
 
   - Download Anaconda from the [official website](https://www.anaconda.com/)
   - Run the installer (leave all options as default)
   - Start "Anaconda Navigator"
-  - In Anaconda, launch the "Jupyter Lab" module
+  - In Anaconda, launch the "Jupyter Lab" module (you might need to click on "Install" first)
 
-### Command line install (advanced users)
+#### Command line install
 
   - Open a terminal (macOS/Linux) or Powershell (Windows)
   - Install Python
       - Enter the command `python --version`
       - If an error or a version < 3.9 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
-  - After installing, restart your terminal/powershell; both of the above commands should display a version number
+  - After installing, restart your terminal/powershell; the `python --version` command should display a version number > 3.9
   - Install Jupyter Lab
       - In a terminal/powershell, run the command `python -m pip install jupyterlab`
       - After the installation completes, Jupyter Lab can be started using the command `jupyter-lab`
 
+### Installing the package
+
+To install the package, use the following command in a terminal:
+
+`python -m pip install PyBerries`
+
+You can also install a specific version number (useful e.g. to make sure you code won't be broken by a future update):
+
+`python -m pip install PyBerries==0.2.8`
+
+In a jupyter notebook, use the command:
+
+`%pip install PyBerries`, or `%pip install PyBerries==0.2.8` for a specific version.
+
 
 ## Getting started
 
-Try downloading and running the [tutorial notebook](./Tutorial/Tutorial.ipynb) to get acquainted with data import and plotting in PyBerries.
+Try downloading and running the [tutorial notebook](https://gitlab.com/MEKlab/pyberries/-/raw/main/Tutorial/Tutorial.ipynb?inline=false) to get acquainted with data import and plotting in PyBerries.
 
-For further details, see the [main functionalities](./doc/PyBerries_main_functionalities.md) documentation, as well as the [DatasetPool](./doc/DatasetPool.md) documentation.
+For further details, see the [main functionalities](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/PyBerries_main_functionalities.md) documentation, as well as the [DatasetPool](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/DatasetPool.md) documentation.
 
-For info and examples on plots, see the [preset plots gallery](./doc/Plot_preset_gallery.md) and the [Seaborn documentation](https://seaborn.pydata.org/index.html)
+For info and examples on plots, see the [preset plots gallery](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/Plot_preset_gallery.md) and the [Seaborn documentation](https://seaborn.pydata.org/index.html)
```

### Comparing `PyBerries-0.2.8.post1/PyBerries.egg-info/SOURCES.txt` & `PyBerries-0.2.9/PyBerries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/README.md` & `PyBerries-0.2.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 # PyBerries
 
 PyBerries is a Python package that can be used to import, manipulate and plot data from Bacmman measurement tables.
 
 It relies mainly on Pandas for data handling and Seaborn/Matplotlib for plotting.
 
-[[_TOC_]]
-
-----
 
 ## Installation
 
-### Anaconda (recommended)
+### Optional: install Jupyter-lab (to run Jupyter Notebooks)
+
+#### Anaconda (recommended)
 
   Anaconda will install both Python and Jupyter-lab (used to run Python notebooks) easily. Note however that it requires ~5 Gb free disk space.
   For a lighter installation procedure, see the next section "Command line install".
 
   - Download Anaconda from the [official website](https://www.anaconda.com/)
   - Run the installer (leave all options as default)
   - Start "Anaconda Navigator"
-  - In Anaconda, launch the "Jupyter Lab" module
+  - In Anaconda, launch the "Jupyter Lab" module (you might need to click on "Install" first)
 
-### Command line install (advanced users)
+#### Command line install
 
   - Open a terminal (macOS/Linux) or Powershell (Windows)
   - Install Python
       - Enter the command `python --version`
       - If an error or a version < 3.9 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
-  - After installing, restart your terminal/powershell; both of the above commands should display a version number
+  - After installing, restart your terminal/powershell; the `python --version` command should display a version number > 3.9
   - Install Jupyter Lab
       - In a terminal/powershell, run the command `python -m pip install jupyterlab`
       - After the installation completes, Jupyter Lab can be started using the command `jupyter-lab`
 
+### Installing the package
+
+To install the package, use the following command in a terminal:
+
+`python -m pip install PyBerries`
+
+You can also install a specific version number (useful e.g. to make sure you code won't be broken by a future update):
+
+`python -m pip install PyBerries==0.2.8`
+
+In a jupyter notebook, use the command:
+
+`%pip install PyBerries`, or `%pip install PyBerries==0.2.8` for a specific version.
+
 
 ## Getting started
 
-Try downloading and running the [tutorial notebook](./Tutorial/Tutorial.ipynb) to get acquainted with data import and plotting in PyBerries.
+Try downloading and running the [tutorial notebook](https://gitlab.com/MEKlab/pyberries/-/raw/main/Tutorial/Tutorial.ipynb?inline=false) to get acquainted with data import and plotting in PyBerries.
 
-For further details, see the [main functionalities](./doc/PyBerries_main_functionalities.md) documentation, as well as the [DatasetPool](./doc/DatasetPool.md) documentation.
+For further details, see the [main functionalities](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/PyBerries_main_functionalities.md) documentation, as well as the [DatasetPool](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/DatasetPool.md) documentation.
 
-For info and examples on plots, see the [preset plots gallery](./doc/Plot_preset_gallery.md) and the [Seaborn documentation](https://seaborn.pydata.org/index.html)
+For info and examples on plots, see the [preset plots gallery](https://gitlab.com/MEKlab/pyberries/-/blob/main/doc/Plot_preset_gallery.md) and the [Seaborn documentation](https://seaborn.pydata.org/index.html)
```

### Comparing `PyBerries-0.2.8.post1/pyberries/data/DatasetPool.py` & `PyBerries-0.2.9/pyberries/data/DatasetPool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from os import listdir
 from os.path import join, exists
 import json
-import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from IPython.display import display
 from warnings import warn
 from .util import dict_val_to_list, arg_to_list, set_to_several_objects
 import pyberries as pyb
 
@@ -22,42 +21,35 @@
                  preprocessing={}
                  ):
         
         path = arg_to_list(path)
         dsList = arg_to_list(dsList)
         preprocessing = dict_val_to_list(preprocessing)
 
-        # One item per dataset
         self.path = path
         self.dsList = dsList
-
-        # One item per Bacmman object
-        self.table = dict()
-        self.parent = dict()
-        self.channel = dict()
+        self._parents = dict()
 
         for i, ds in enumerate(dsList):
             ds_path = path[0] if len(path) == 1 else path[i]
             assert exists(ds_path), f'Bacmman folder not found: {ds_path}'
             assert exists(join(ds_path, ds)), f'Dataset {ds} not found.\nMaybe looking for {" or ".join([x for x in listdir(ds_path) if x.startswith(ds[0:6])])}?'
             assert (len(groups) >= len(dsList)) or not groups, 'If groups are provided, one group should be defined per dataset'
 
             # Load configuration
             cf = join(ds_path, ds, f"{ds}_config.json")
             with open(cf, errors='ignore') as f:
                 conf = json.load(f)
                 object_class_names = [c["name"] for c in conf["structures"]["list"]]
                 object_parents = [c["segmentationParent"] for c in conf["structures"]["list"]]
-                channel_images = [c["channelImage"] for c in conf["structures"]["list"]]
 
             # Add Viewfield object if measurement table is available
             if exists(join(ds_path, ds, f"{ds}_{-1}.csv")):
                 object_class_names.insert(0, 'Viewfield')
                 object_parents.insert(0, [])
-                channel_images.insert(0, [-1])
                 start_table = -1
             else:
                 start_table = 0
 
             # Load data tables
             k = 0
             for j, obj in enumerate(object_class_names, start_table):
@@ -68,29 +60,36 @@
                 if obj in preprocessing.keys():
                     if len(preprocessing[obj]) == 1:
                         df_in = df_in.transform(preprocessing[obj][0])
                     elif len(preprocessing[obj]) > 1:
                         assert len(preprocessing[obj]) == len(self.dsList), 'If multiple pre-processings are provided, there should be one per dataset'
                         if preprocessing[obj][i]:
                             df_in = df_in.transform(preprocessing[obj][i])
-                self.table[obj] = df_in if obj not in self.table.keys() else pd.concat([self.table[obj], df_in], axis=0)
-                self.parent[obj] = object_class_names[object_parents[k][0]-start_table] if object_parents[k] else 'Viewfield'
-                self.channel[obj] = channel_images[k][0]
+                df = df_in if obj not in self.__dict__.keys() else pd.concat([self[obj], df_in], axis=0)
+                setattr(self, obj, df)
+                self._parents[obj] = object_class_names[object_parents[k][0]-start_table] if object_parents[k] else 'Viewfield'
                 k+=1
             print(f'Dataset {ds}: loaded objects {object_class_names}')
-        self.objects = self.table.keys()
-        for data in self.table.values():
-            data.reset_index(drop=True, inplace=True)
+        self.objects = list(self._parents.keys())
+        for obj in self.objects:
+            self[obj].reset_index(drop=True, inplace=True)
 
         self.add_metadata(metadata)
         self.apply_filters(filters)
 
+
+    def __getitem__(self, name):
+        return getattr(self, name)
+    def __setitem__(self, name, value):
+        return setattr(self, name, value)
+
     def describe(self, agg, include='all'):
         include = arg_to_list(include)
-        for obj, df in self.table.items():
+        for obj in self.objects:
+            df = self[obj]
             if include != ['all']:
                 df = df.filter(items=include + ['Dataset', 'Group'])
                 if not [item for item in list(df.columns) + ['All'] if item in include]:
                     df = pd.DataFrame()
             print(f'{obj}')
             if df.empty:
                 print('No data')
@@ -105,29 +104,61 @@
                     .agg(agg, numeric_only=True)
                     )
                 if isinstance(agg, list):
                     df2.columns = df2.columns.map(' ('.join) + ')'
                 df3 = df[['Group', 'Dataset']].drop_duplicates().set_index('Dataset')
                 df_out = df3.join([df1, df2])
                 display(df_out)
+
+    def has_na(self, object_name=None):
+        if object_name:
+            objects = arg_to_list(object_name)
+        else:
+            objects = self.objects
+        for obj in objects:
+            df = self[obj].loc[:, ~self[obj].columns.isin(['Position','PositionIdx','Indices','Frame','Idx','Time','Group','Dataset'])]
+            if not df.empty:
+                print(f'{obj}')
+                display(df.isna().sum())
+
+    def dropna(self, object_name=None, **kwargs):
+        if object_name:
+            objects = arg_to_list(object_name)
+        else:
+            objects = self.objects
+        for obj in objects:
+            if not self[obj].empty:
+                self[obj] = self[obj].dropna(**kwargs)
+
+    def fillna(self, object_name=None, col=None, **kwargs):
+        if object_name:
+            objects = arg_to_list(object_name)
+        else:
+            objects = self.objects
+        for obj in objects:
+            if not self[obj].empty:
+                if col:
+                    self[obj][col] = self[obj][col].fillna(**kwargs)
+                else:
+                    self[obj] = self[obj].fillna(**kwargs)
     
     def head(self, nlines:int=5):
-        for obj, df in self.table.items():
+        for obj in self.objects:
             print(f'{obj}')
-            if df.empty:
+            if self[obj].empty:
                 print('No data')
             else:
-                display(df.head(nlines))
+                display(self[obj].head(nlines))
     
     def add_metadata(self, metadata):
         metadata = set_to_several_objects(metadata, self.objects)
         metadata = dict_val_to_list(metadata)
         for obj in metadata.keys():
-            if not self.table[obj].empty:
-                df = self.table[obj]
+            if not self[obj].empty:
+                df = self[obj]
                 for var in metadata[obj]:
                     df[var.replace(' ', '_')] = 0
                     if var == 'DateTime':
                         df['TimeDelta'] = 0
                         df['Time_min'] = 0
                     for i, ds in enumerate(self.dsList):
                         ds_path = self.path[0] if len(self.path) == 1 else self.path[i]
@@ -140,114 +171,117 @@
                         if 'DateTime' in df.columns:
                             df.loc[df['Dataset'] == ds] = (df.loc[df['Dataset'] == ds]
                                                             .assign(DateTime = lambda df: pd.to_datetime(df.DateTime, format='%Y%m%d %H:%M:%S.%f'),
                                                                     TimeDelta = lambda df: df.DateTime - df.DateTime.iloc[0],
                                                                     Time_min = lambda df: df.TimeDelta.dt.total_seconds().div(60)
                                                                     )
                                                             )
-                self.table[obj] = df
+                self[obj] = df
     
     def apply_filters(self, filters):
         filters = set_to_several_objects(filters, self.objects)
         filters = dict_val_to_list(filters)
         for obj, filter in filters.items():
             if len(filter) == 1:
-                self.table[obj] = self.table[obj].query(filter[0])
+                setattr(self, obj, self[obj].query(filter[0]))
             elif len(filter) > 1:
                 assert len(filter) == len(self.dsList), 'If multiple filters are provided, there should be one per dataset'
                 df = pd.DataFrame()
                 i=0
-                for _, data in self.table[obj].groupby('Dataset', sort=False):
+                for _, data in self[obj].groupby('Dataset', sort=False):
                     if filter[i]:
                         df = pd.concat([df, data.query(filter[i])], axis=0)
                     else:
                         df = pd.concat([df, data], axis=0)
                     i+=1
-                self.table[obj] = df
             # Propagate filters to children (if any)
-            for child, parent in self.parent.items():
+            for child, parent in self._parents.items():
                 if parent == obj:
                     self.propagate_filters(parent, child)
 
+    def propagate_filters(self, parent:str, child:str):
+        self.get_parent_indices(obj=child)
+        self[child] = (self[child]
+                            .merge(self[parent][['Dataset', 'PositionIdx', 'Indices']], suffixes=(None, '_tmp'), left_on = ['Dataset', 'PositionIdx', 'ParentIndices'], right_on=['Dataset', 'PositionIdx', 'Indices'])
+                            .transform(lambda df: df.loc[:, ~df.columns.str.contains('_tmp')])
+                            )
+
     def rename_object(self, rename:dict):
         for old_name, new_name in rename.items():
             if new_name in self.objects:
-                self.table[new_name] = pd.concat([self.table[new_name], self.table[old_name]], axis=0).reset_index(drop=True, inplace=True)
+                self[new_name] = pd.concat([self[new_name], self[old_name]], axis=0).reset_index(drop=True, inplace=True)
             else:
-                self.table[new_name] = self.table[old_name]
-                self.channel[new_name] = self.channel[old_name]
-                self.parent[new_name] = self.parent[old_name]
-            del self.table[old_name]
-            del self.channel[old_name]
-            del self.parent[old_name]
-            self.objects = self.table.keys()
+                self[new_name] = self[old_name]
+                self._parents[new_name] = self._parents[old_name]
+            for child, parent in self._parents.items():
+                if parent == old_name:
+                    self._parents[child] = new_name
+            delattr(self, old_name)
+            del self._parents[old_name]
+            self.objects = list(self._parents.keys())
 
     def get_parent_indices(self, obj:str, indices:str='Indices', newcol:str='ParentIndices'):
-        self.table[obj][newcol] = (self.table[obj]
-                                            [indices]
-                                            .str.split('-', expand=True)
-                                            .iloc[:,:-1]
-                                            .agg('-'.join, axis=1)
-                                            )
+        self[obj][newcol] = (self[obj]
+                                    [indices]
+                                    .str.split('-', expand=True)
+                                    .iloc[:,:-1]
+                                    .agg('-'.join, axis=1)
+                                    )
     
     def get_idx(self, obj:str, idx:int=0, indices:str='Indices', newcol:str='ParentIdx'):
-        self.table[obj][newcol] = (self.table[obj]
-                                            [indices]
-                                            .str.split('-', expand=True)
-                                            .iloc[:,idx]
-                                            .astype('int64')
-                                            )
+        self[obj][newcol] = (self[obj]
+                                    [indices]
+                                    .str.split('-', expand=True)
+                                    .iloc[:,idx]
+                                    .astype('int64')
+                                    )
         
     def fuse_columns(self, obj:str, cols:list=[], new:str='new_col'):
-        self.table[obj][new] = self.table[obj][cols].astype('str').agg('-'.join, axis=1)
+        self[obj][new] = self[obj][cols].astype('str').agg('-'.join, axis=1)
 
     def normalise(self, object_name:str, col:str='', normalise_by:str='', new_col:str=''):
-        if new_col in self.table[object_name].columns:
-            self.table[object_name].drop(columns=new_col, inplace=True)
-        self.table[object_name] = (self.table[object_name]
-                                        .assign(new_tmp = lambda df: df[col] / df[normalise_by])
-                                        .rename(columns={'new_tmp':new_col})
-                                        )
-    
-    def propagate_filters(self, parent:str, child:str):
-        self.get_parent_indices(obj=child)
-        self.table[child] = (self.table[child]
-                            .merge(self.table[parent][['Dataset', 'PositionIdx', 'Indices']], suffixes=(None, '_tmp'), left_on = ['Dataset', 'PositionIdx', 'ParentIndices'], right_on=['Dataset', 'PositionIdx', 'Indices'])
-                            .transform(lambda df: df.loc[:, ~df.columns.str.contains('_tmp')])
-                            )
+        if new_col in self[object_name].columns:
+            self[object_name].drop(columns=new_col, inplace=True)
+        if new_col:
+            self[object_name] = (self[object_name]
+                                            .assign(new_tmp = lambda df: df[col] / df[normalise_by])
+                                            .rename(columns={'new_tmp':new_col})
+                                            )
+        else:
+            self[object_name] = (self[object_name]
+                                            .assign(new_tmp = lambda df: df[col] / df[normalise_by])
+                                            .drop(columns=col)
+                                            .rename(columns={'new_tmp':col})
+                                            )
 
     def add_from_parent(self, object_name:str, col:list=[]):
-        parent = self.parent[object_name]
+        parent = self._parents[object_name]
         self.get_parent_indices(obj=object_name)
-        df = self.table[object_name]
         for c in col:
-            df = (df
-                .merge(self.table[parent][['PositionIdx', 'Indices', c]], suffixes=(None, '_tmp'), left_on = ['PositionIdx', 'ParentIndices'], right_on=['PositionIdx', 'Indices'])
-                .transform(lambda df: df.loc[:, ~df.columns.str.contains('_tmp')])
-                )
-        self.table[object_name] = df
+            self[object_name] = (self[object_name]
+                                        .merge(self[parent][['PositionIdx', 'Indices', c]], suffixes=(None, '_tmp'), left_on = ['PositionIdx', 'ParentIndices'], right_on=['PositionIdx', 'Indices'])
+                                        .transform(lambda df: df.loc[:, ~df.columns.str.contains('_tmp')])
+                                        )
 
     def add_columns(self, object_name:str, metrics, **kwargs):
-        df = self.table[object_name]
+        df = self[object_name]
         for m in metrics:
             if m == 'Heatmap':
                 df = pyb.metrics.heatmap_metrics(df, **kwargs)
             elif m == 'is_col_larger':
                 df = pyb.metrics.is_col_larger(df, **kwargs)
             elif m == 'bin_column':
                 df = pyb.metrics.bin_column(df, **kwargs)
             elif m == 'Dapp':
                 df = pyb.metrics.tracking_Dapp(df, **kwargs)
             else:
                 ValueError(f'Metric "{m}" not found')
-        self.table[object_name] = df
 
     def get_timeseries(self, object_name:str, metric, **kwargs):
-        df_in = self.table[object_name]
-        self.timeseries = dict()
+        df_in = self[object_name]
         if metric == 'SpineLength':
             df_out = pyb.metrics.Cell_length(df_in, **kwargs)
         elif metric == 'ObjectCount':
             df_out = pyb.metrics.Object_count(df_in, **kwargs)
         elif metric == 'ObjectClass':
             df_out = pyb.metrics.Object_classifier(df_in, **kwargs)
         elif metric == 'Intensity':
@@ -256,23 +290,23 @@
             df_out = pyb.metrics.Column_quantile(df_in, **kwargs)
         elif metric == 'Aggregation':
             df_out = pyb.metrics.Column_aggregation(df_in, **kwargs)
         elif metric == 'Fluo_intensity':
             df_out = pyb.metrics.Fluo_intensity(df_in, **kwargs)
         else:
             ValueError(f'Metric "{metric}" not found')
-        self.timeseries[object_name] = df_out
+        self[f'{object_name}_timeseries'] = df_out
 
-    def plot_preset(self, preset:str, object_name:str='', timeseries:bool=False, drop_duplicates_by=[], return_axes:bool=False, **kwargs):
+    def plot_preset(self, preset:str, object_name:str='', drop_duplicates_by=[], return_axes:bool=False, **kwargs):
         hue = kwargs.get('hue','')
         if isinstance(hue, list):
             self.fuse_columns(obj=object_name, cols=hue, new='_'.join(hue))
             kwargs['hue'] = '_'.join(hue)
         if object_name:
-            df_in = self.timeseries[object_name] if timeseries else self.table[object_name]
+            df_in = self[object_name].copy()
             if drop_duplicates_by:
                 df_in = df_in.drop_duplicates(subset = drop_duplicates_by)
         _,ax = plt.subplots(dpi=130)
         if preset == 'histogram':
             ax = pyb.plots.plot_histogram(df_in, ax=ax, **kwargs)
         elif preset == 'histogram_fit':
             ax = pyb.plots.plot_histogram_fit(df_in, ax=ax, **kwargs)
@@ -294,18 +328,16 @@
             ax = pyb.plots.boxplot(df_in, ax=ax, **kwargs)
         elif preset == 'boxenplot':
             ax = pyb.plots.plot_boxenplot(df_in, ax=ax, **kwargs)
         elif preset == 'spot_tracks':
             lineage = kwargs.pop('lineage','')
             self.fuse_columns(obj=object_name, cols=['Idx','BacteriaLineage'], new='Track')
             if lineage:
-                df = df_in.copy().query('BacteriaLineage == @lineage')
-            else:
-                df = df_in.copy()
-            ax=pyb.plots.lineplot(df, hue='Track', sort=False, ax=ax, **kwargs)
+                df_in = df_in.copy().query('BacteriaLineage == @lineage')
+            ax=pyb.plots.lineplot(df_in, hue='Track', sort=False, ax=ax, **kwargs)
         elif preset == 'rates_summary':
             ax = pyb.plots.plot_rates_summary(ax=ax, **kwargs)
         elif preset == 'grey_lines_and_highlight':
             ax = pyb.plots.plot_grey_lines_and_highlight(df_in, ax=ax, **kwargs)
         else:
             warn('Plot preset not found!')
         if return_axes: return ax
```

### Comparing `PyBerries-0.2.8.post1/pyberries/data/Fitting.py` & `PyBerries-0.2.9/pyberries/data/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/data/util.py` & `PyBerries-0.2.9/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/file_utilities/Filename_utils.py` & `PyBerries-0.2.9/pyberries/file_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/file_utilities/Stack_tiffs.py` & `PyBerries-0.2.9/pyberries/file_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/file_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.9/pyberries/file_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/metrics/Metrics.py` & `PyBerries-0.2.9/pyberries/metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/metrics/Time_metrics.py` & `PyBerries-0.2.9/pyberries/metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.8.post1/pyberries/plots/Plot_presets.py` & `PyBerries-0.2.9/pyberries/plots/Plot_presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             x_model = np.linspace(data[x].iloc[0], data[x].iloc[-1], 300)
             df = pd.DataFrame({'x':x_model, 'Fit':model(x_model, *fit_results[grp]), groupby:grp})
             fit_df = pd.concat([fit_df, df], axis=0)
     ax = pyb.plots.lineplot(df_in, ax=ax, **kwargs)
     ax = sns.lineplot(data=fit_df, x='x', y='Fit', hue=groupby, hue_order=fit_df[groupby].unique(), legend=False, ax=ax, linestyle='dashed')
 
 def plot_rates_summary(rates, ax, **kwargs):
-    ax = pyb.plots.stripplot(rates, ax=ax, jitter=False, **kwargs)
+    ax = pyb.plots.pointplot(rates, ax=ax, **kwargs)
     sns.move_legend(ax, "upper left", bbox_to_anchor=(1, 1), labelspacing=1)
 
 def plot_grey_lines_and_highlight(df_in, ax, color='gray', estimator=None, alpha=0.4, highlight=None, **kwargs):
     highlight_by_index = kwargs.pop('highlight_by_index', False)
     units = kwargs.get('units')
     ax = pyb.plots.lineplot(df_in, color=color, estimator=estimator, alpha=alpha, legend=False, ax=ax, **kwargs)
     df = df_in.copy()
```

### Comparing `PyBerries-0.2.8.post1/pyberries/plots/Plots.py` & `PyBerries-0.2.9/pyberries/plots/Plots.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,7 +48,11 @@
     return g
 
 @plot
 def boxplot(df, **kwargs):
     g = sns.boxplot(data=df, **kwargs)
     return g
 
+@plot
+def pointplot(df, **kwargs):
+    g = sns.pointplot(data=df, **kwargs)
+    return g
```

### Comparing `PyBerries-0.2.8.post1/setup.py` & `PyBerries-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.8.post1",
+    version="0.2.9",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
     packages=setuptools.find_packages(),
```

