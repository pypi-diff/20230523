# Comparing `tmp/bioplotz-0.1.0.dev6.tar.gz` & `tmp/bioplotz-0.1.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioplotz-0.1.0.dev6.tar", last modified: Tue May  9 09:43:05 2023, max compression
+gzip compressed data, was "bioplotz-0.1.0.dev7.tar", last modified: Tue May 23 03:57:09 2023, max compression
```

## Comparing `bioplotz-0.1.0.dev6.tar` & `bioplotz-0.1.0.dev7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/
--rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/LICENSE
--rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/MANIFEST.in
--rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)    13548 2023-05-05 02:18:26.000000 bioplotz-0.1.0.dev6/README.md
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-09 09:43:05.276982 bioplotz-0.1.0.dev6/bioplotz/
--rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-09 09:42:11.000000 bioplotz-0.1.0.dev6/bioplotz/__init__.py
--rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/bioplotz/chromosome.py
--rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/bioplotz/genecluster.py
--rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev6/bioplotz/manhattan.py
--rw-r--r--   0 zsc       (1000) users      (100)     4706 2023-05-08 07:20:31.000000 bioplotz-0.1.0.dev6/bioplotz/multialign.py
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/bioplotz.egg-info/
--rw-r--r--   0 zsc       (1000) users      (100)    13845 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/SOURCES.txt
--rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/dependency_links.txt
--rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/requires.txt
--rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-09 09:43:05.000000 bioplotz-0.1.0.dev6/bioplotz.egg-info/top_level.txt
--rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-09 09:43:05.280982 bioplotz-0.1.0.dev6/setup.cfg
--rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-09 09:42:35.000000 bioplotz-0.1.0.dev6/setup.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-23 03:57:09.708321 bioplotz-0.1.0.dev7/
+-rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-12 09:00:44.000000 bioplotz-0.1.0.dev7/LICENSE
+-rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-12 09:00:44.000000 bioplotz-0.1.0.dev7/MANIFEST.in
+-rw-r--r--   0 zsc       (1000) users      (100)    14492 2023-05-23 03:57:09.708321 bioplotz-0.1.0.dev7/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)    14195 2023-05-23 03:54:40.000000 bioplotz-0.1.0.dev7/README.md
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-23 03:57:09.708321 bioplotz-0.1.0.dev7/bioplotz/
+-rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-23 03:50:37.000000 bioplotz-0.1.0.dev7/bioplotz/__init__.py
+-rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-12 09:00:44.000000 bioplotz-0.1.0.dev7/bioplotz/chromosome.py
+-rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-12 09:00:44.000000 bioplotz-0.1.0.dev7/bioplotz/genecluster.py
+-rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-12 09:00:44.000000 bioplotz-0.1.0.dev7/bioplotz/manhattan.py
+-rw-r--r--   0 zsc       (1000) users      (100)     6194 2023-05-23 03:49:51.000000 bioplotz-0.1.0.dev7/bioplotz/multialign.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-23 03:57:09.708321 bioplotz-0.1.0.dev7/bioplotz.egg-info/
+-rw-r--r--   0 zsc       (1000) users      (100)    14492 2023-05-23 03:57:09.000000 bioplotz-0.1.0.dev7/bioplotz.egg-info/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-23 03:57:09.000000 bioplotz-0.1.0.dev7/bioplotz.egg-info/SOURCES.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-23 03:57:09.000000 bioplotz-0.1.0.dev7/bioplotz.egg-info/dependency_links.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-23 03:57:09.000000 bioplotz-0.1.0.dev7/bioplotz.egg-info/requires.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-23 03:57:09.000000 bioplotz-0.1.0.dev7/bioplotz.egg-info/top_level.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-23 03:57:09.708321 bioplotz-0.1.0.dev7/setup.cfg
+-rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-23 03:50:31.000000 bioplotz-0.1.0.dev7/setup.py
```

### Comparing `bioplotz-0.1.0.dev6/LICENSE` & `bioplotz-0.1.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev6/PKG-INFO` & `bioplotz-0.1.0.dev7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1
-Name: bioplotz
-Version: 0.1.0.dev6
-Summary: A python package for drawing some bioinformatic pictures.
-Home-page: https://github.com/sc-zhang/bioplotz
-Author: Shengcheng Zhang
-Author-email: zsc-zhang@foxmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Introduction
 
 This is a package for plotting some images for bioinformatics.
 
 ## Dependencies
 Python modules:  
 &ensp;&ensp;&ensp;&ensp;numpy  
 &ensp;&ensp;&ensp;&ensp;matplotlib  
 &ensp;&ensp;&ensp;&ensp;pandas  
 
 ## Installation
+### Install via pip
+```bash
+pip install bioplotz
+```
+
+### Install from source code
 ```bash
 pip install git+https://github.com/sc-zhang/bioplotz.git --user
 ```
 
 ## Usage
 
 ### Manhattan Plot
@@ -104,23 +100,26 @@
 ### Multi Alignment Plot
 
 ```python
 import bioplotz as bp
 
 fig, ax = bp.multialign(data)
 ```
-| parameter               | value type | Optional | Default | explain                                                 |
-|-------------------------|------------|----------|---------|---------------------------------------------------------|
-| **data**                | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence     |
-| **match_color**         | str        | Yes      | blue    | color for displaying matched bases                      |
-| **mismatch_color**      | str        | Yes      | red     | color for highlighting mismatched bases                 |
-| **base_per_line**       | int        | Yes      | 80      | base count to display for each line                     |
-| **highlight_positions** | list       | Yes      | None    | positions for highlighting, 0-base                      |
-| **highlight_color**     | str        | Yes      | green   | color for highlighting positions in highlight_positions |
-| ****kwargs**            | any        | Yes      | -       | same with which use in ax.text                          |
+| parameter                      | value type | Optional | Default | explain                                                           |
+|--------------------------------|------------|----------|---------|-------------------------------------------------------------------|
+| **data**                       | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence               |
+| **match_color**                | str        | Yes      | blue    | color of matched bases                                            |
+| **match_background_color**     | str        | Yes      | None    | background color of matched bases                                 |
+| **mismatch_color**             | str        | Yes      | red     | color of mismatched bases                                         |
+| **mismatch_background_color**  | str        | Yes      | None    | background color of mismatched bases                              |
+| **base_per_line**              | int        | Yes      | 80      | base count to display for each line                               |
+| **highlight_positions**        | list       | Yes      | None    | positions for highlighting, 0-base                                |
+| **highlight_color**            | str        | Yes      | green   | color of highlighting positions in highlight_positions            |
+| **highlight_background_color** | str        | Yes      | None    | background color of highlighting positions in highlight_positions |
+| ****kwargs**                   | any        | Yes      | -       | same with which use in ax.text                                    |
 
 **Notice**, the figsize should be (8, x) where x=align_length/80*gene_count/5, and the font must be  monospaced, 
 like "Courier New", that sometimes user need add codes as following.
 ```python
 import matplotlib as mpl
 import bioplotz as bp
 
@@ -131,8 +130,8 @@
 ```python
 plt.rcParams['font.sans-serif'] = 'Courier New'
 ```
 <table align="center">
 <tr>
 <td><img width=600 src="examples/multialign.png"></td>
 </tr>
-</table>
+</table>
```

### Comparing `bioplotz-0.1.0.dev6/README.md` & `bioplotz-0.1.0.dev7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,34 @@
+Metadata-Version: 2.1
+Name: bioplotz
+Version: 0.1.0.dev7
+Summary: A python package for drawing some bioinformatic pictures.
+Home-page: https://github.com/sc-zhang/bioplotz
+Author: Shengcheng Zhang
+Author-email: zsc-zhang@foxmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Introduction
 
 This is a package for plotting some images for bioinformatics.
 
 ## Dependencies
 Python modules:  
 &ensp;&ensp;&ensp;&ensp;numpy  
 &ensp;&ensp;&ensp;&ensp;matplotlib  
 &ensp;&ensp;&ensp;&ensp;pandas  
 
 ## Installation
+### Install via pip
+```bash
+pip install bioplotz
+```
+
+### Install from source code
 ```bash
 pip install git+https://github.com/sc-zhang/bioplotz.git --user
 ```
 
 ## Usage
 
 ### Manhattan Plot
@@ -94,23 +110,26 @@
 ### Multi Alignment Plot
 
 ```python
 import bioplotz as bp
 
 fig, ax = bp.multialign(data)
 ```
-| parameter               | value type | Optional | Default | explain                                                 |
-|-------------------------|------------|----------|---------|---------------------------------------------------------|
-| **data**                | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence     |
-| **match_color**         | str        | Yes      | blue    | color for displaying matched bases                      |
-| **mismatch_color**      | str        | Yes      | red     | color for highlighting mismatched bases                 |
-| **base_per_line**       | int        | Yes      | 80      | base count to display for each line                     |
-| **highlight_positions** | list       | Yes      | None    | positions for highlighting, 0-base                      |
-| **highlight_color**     | str        | Yes      | green   | color for highlighting positions in highlight_positions |
-| ****kwargs**            | any        | Yes      | -       | same with which use in ax.text                          |
+| parameter                      | value type | Optional | Default | explain                                                           |
+|--------------------------------|------------|----------|---------|-------------------------------------------------------------------|
+| **data**                       | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence               |
+| **match_color**                | str        | Yes      | blue    | color of matched bases                                            |
+| **match_background_color**     | str        | Yes      | None    | background color of matched bases                                 |
+| **mismatch_color**             | str        | Yes      | red     | color of mismatched bases                                         |
+| **mismatch_background_color**  | str        | Yes      | None    | background color of mismatched bases                              |
+| **base_per_line**              | int        | Yes      | 80      | base count to display for each line                               |
+| **highlight_positions**        | list       | Yes      | None    | positions for highlighting, 0-base                                |
+| **highlight_color**            | str        | Yes      | green   | color of highlighting positions in highlight_positions            |
+| **highlight_background_color** | str        | Yes      | None    | background color of highlighting positions in highlight_positions |
+| ****kwargs**                   | any        | Yes      | -       | same with which use in ax.text                                    |
 
 **Notice**, the figsize should be (8, x) where x=align_length/80*gene_count/5, and the font must be  monospaced, 
 like "Courier New", that sometimes user need add codes as following.
 ```python
 import matplotlib as mpl
 import bioplotz as bp
 
@@ -121,8 +140,8 @@
 ```python
 plt.rcParams['font.sans-serif'] = 'Courier New'
 ```
 <table align="center">
 <tr>
 <td><img width=600 src="examples/multialign.png"></td>
 </tr>
-</table>
+</table>
```

### Comparing `bioplotz-0.1.0.dev6/bioplotz/chromosome.py` & `bioplotz-0.1.0.dev7/bioplotz/chromosome.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev6/bioplotz/genecluster.py` & `bioplotz-0.1.0.dev7/bioplotz/genecluster.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev6/bioplotz/manhattan.py` & `bioplotz-0.1.0.dev7/bioplotz/manhattan.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev6/bioplotz.egg-info/PKG-INFO` & `bioplotz-0.1.0.dev7/bioplotz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -15,14 +15,20 @@
 ## Dependencies
 Python modules:  
 &ensp;&ensp;&ensp;&ensp;numpy  
 &ensp;&ensp;&ensp;&ensp;matplotlib  
 &ensp;&ensp;&ensp;&ensp;pandas  
 
 ## Installation
+### Install via pip
+```bash
+pip install bioplotz
+```
+
+### Install from source code
 ```bash
 pip install git+https://github.com/sc-zhang/bioplotz.git --user
 ```
 
 ## Usage
 
 ### Manhattan Plot
@@ -104,23 +110,26 @@
 ### Multi Alignment Plot
 
 ```python
 import bioplotz as bp
 
 fig, ax = bp.multialign(data)
 ```
-| parameter               | value type | Optional | Default | explain                                                 |
-|-------------------------|------------|----------|---------|---------------------------------------------------------|
-| **data**                | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence     |
-| **match_color**         | str        | Yes      | blue    | color for displaying matched bases                      |
-| **mismatch_color**      | str        | Yes      | red     | color for highlighting mismatched bases                 |
-| **base_per_line**       | int        | Yes      | 80      | base count to display for each line                     |
-| **highlight_positions** | list       | Yes      | None    | positions for highlighting, 0-base                      |
-| **highlight_color**     | str        | Yes      | green   | color for highlighting positions in highlight_positions |
-| ****kwargs**            | any        | Yes      | -       | same with which use in ax.text                          |
+| parameter                      | value type | Optional | Default | explain                                                           |
+|--------------------------------|------------|----------|---------|-------------------------------------------------------------------|
+| **data**                       | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence               |
+| **match_color**                | str        | Yes      | blue    | color of matched bases                                            |
+| **match_background_color**     | str        | Yes      | None    | background color of matched bases                                 |
+| **mismatch_color**             | str        | Yes      | red     | color of mismatched bases                                         |
+| **mismatch_background_color**  | str        | Yes      | None    | background color of mismatched bases                              |
+| **base_per_line**              | int        | Yes      | 80      | base count to display for each line                               |
+| **highlight_positions**        | list       | Yes      | None    | positions for highlighting, 0-base                                |
+| **highlight_color**            | str        | Yes      | green   | color of highlighting positions in highlight_positions            |
+| **highlight_background_color** | str        | Yes      | None    | background color of highlighting positions in highlight_positions |
+| ****kwargs**                   | any        | Yes      | -       | same with which use in ax.text                                    |
 
 **Notice**, the figsize should be (8, x) where x=align_length/80*gene_count/5, and the font must be  monospaced, 
 like "Courier New", that sometimes user need add codes as following.
 ```python
 import matplotlib as mpl
 import bioplotz as bp
```

### Comparing `bioplotz-0.1.0.dev6/setup.py` & `bioplotz-0.1.0.dev7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='bioplotz',
-    version='0.1.0.dev6',
+    version='0.1.0.dev7',
     packages=['bioplotz'],
     url='https://github.com/sc-zhang/bioplotz',
     license='',
     author='Shengcheng Zhang',
     author_email='zsc-zhang@foxmail.com',
     description='A python package for drawing some bioinformatic pictures.',
     long_description=long_description,
```

