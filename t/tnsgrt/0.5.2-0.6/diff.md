# Comparing `tmp/tnsgrt-0.5.2.tar.gz` & `tmp/tnsgrt-0.6.tar.gz`

## Comparing `tnsgrt-0.5.2.tar` & `tnsgrt-0.6.tar`

### file list

```diff
@@ -1,65 +1,73 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/.readthedocs.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/requirements.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/Makefile
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/conf.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/make.bat
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/requirements.txt
--rw-r--r--   0        0        0    57596 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/bicycle1.png
--rw-r--r--   0        0        0    14219 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/bicycle2.png
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/loaded.png
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/planar1.png
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/planar2.png
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/planar3.png
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/planar4.png
--rw-r--r--   0        0        0    80392 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/prisms.png
--rw-r--r--   0        0        0    41183 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson.png
--rw-r--r--   0        0        0    40684 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson1.png
--rw-r--r--   0        0        0    40836 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson2.png
--rw-r--r--   0        0        0    52327 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson3.png
--rw-r--r--   0        0        0    52431 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson4.png
--rw-r--r--   0        0        0    56067 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson5.png
--rw-r--r--   0        0        0    55206 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson6.png
--rw-r--r--   0        0        0    64370 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/snelson7.png
--rw-r--r--   0        0        0    19296 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/images/stiffness1.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/tables/tab1.csv
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/tables/tab2.csv
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/tables/tab3.csv
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/tables/tab4.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/tables/tab5.csv
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/tables/tab6.csv
--rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/usage/examples.rst
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/usage/modules.rst
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/usage/properties.rst
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/usage/quickstart.rst
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/usage/structure.rst
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/doc/usage/transformations.rst
--rw-r--r--   0        0        0   543051 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/examples/examples.ipynb
--rw-r--r--   0        0        0    41611 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/examples/properties.ipynb
--rw-r--r--   0        0        0   174568 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/examples/quick_start.ipynb
--rw-r--r--   0        0        0    91403 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/examples/structures.ipynb
--rw-r--r--   0        0        0    65635 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/examples/transformations.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/michell.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/optim.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/prism.py
--rw-r--r--   0        0        0    20635 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/stiffness.py
--rw-r--r--   0        0        0    58984 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/structure.py
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/plotter/__init__.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/plotter/matplotlib.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/plotter/plotter.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/src/tnsgrt/plotter/vispy.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/tests/test_equilibrium.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/tests/test_michell.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/tests/test_prism.py
--rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/tests/test_stiffness.py
--rw-r--r--   0        0        0    43013 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/tests/test_structure.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/tests/test_utils.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/LICENSE
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/README.md
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 tnsgrt-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 tnsgrt-0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tnsgrt-0.6/requirements.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tnsgrt-0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 tnsgrt-0.6/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/Makefile
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/conf.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/make.bat
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/requirements.txt
+-rw-r--r--   0        0        0    57596 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/bicycle1.png
+-rw-r--r--   0        0        0    14219 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/bicycle2.png
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/constraint1.png
+-rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/constraint2.png
+-rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/constraint3.png
+-rw-r--r--   0        0        0    22335 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/constraint4.png
+-rw-r--r--   0        0        0    33689 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/constraint5.png
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/constraint6.png
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/loaded.png
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/planar1.png
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/planar2.png
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/planar3.png
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/planar4.png
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/planar5.png
+-rw-r--r--   0        0        0    80392 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/prisms.png
+-rw-r--r--   0        0        0    41183 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson.png
+-rw-r--r--   0        0        0    40684 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson1.png
+-rw-r--r--   0        0        0    40836 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson2.png
+-rw-r--r--   0        0        0    52327 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson3.png
+-rw-r--r--   0        0        0    52431 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson4.png
+-rw-r--r--   0        0        0    56067 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson5.png
+-rw-r--r--   0        0        0    55206 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson6.png
+-rw-r--r--   0        0        0    64370 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/snelson7.png
+-rw-r--r--   0        0        0    33161 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/soft.png
+-rw-r--r--   0        0        0    19296 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/images/stiffness1.png
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/tables/tab1.csv
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/tables/tab2.csv
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/tables/tab3.csv
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/tables/tab4.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/tables/tab5.csv
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/tables/tab6.csv
+-rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/usage/examples.rst
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/usage/modules.rst
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/usage/properties.rst
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/usage/quickstart.rst
+-rw-r--r--   0        0        0    18319 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/usage/structure.rst
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 tnsgrt-0.6/doc/usage/transformations.rst
+-rw-r--r--   0        0        0   543051 2020-02-02 00:00:00.000000 tnsgrt-0.6/examples/examples.ipynb
+-rw-r--r--   0        0        0    61400 2020-02-02 00:00:00.000000 tnsgrt-0.6/examples/properties.ipynb
+-rw-r--r--   0        0        0   174568 2020-02-02 00:00:00.000000 tnsgrt-0.6/examples/quick_start.ipynb
+-rw-r--r--   0        0        0   299753 2020-02-02 00:00:00.000000 tnsgrt-0.6/examples/structures.ipynb
+-rw-r--r--   0        0        0    65635 2020-02-02 00:00:00.000000 tnsgrt-0.6/examples/transformations.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/michell.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/optim.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/prism.py
+-rw-r--r--   0        0        0    22028 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/stiffness.py
+-rw-r--r--   0        0        0    61948 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/structure.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/plotter/__init__.py
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/plotter/matplotlib.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/plotter/plotter.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 tnsgrt-0.6/src/tnsgrt/plotter/vispy.py
+-rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 tnsgrt-0.6/tests/test_equilibrium.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tnsgrt-0.6/tests/test_michell.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 tnsgrt-0.6/tests/test_prism.py
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 tnsgrt-0.6/tests/test_stiffness.py
+-rw-r--r--   0        0        0    43013 2020-02-02 00:00:00.000000 tnsgrt-0.6/tests/test_structure.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 tnsgrt-0.6/tests/test_utils.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tnsgrt-0.6/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 tnsgrt-0.6/LICENSE
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 tnsgrt-0.6/README.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tnsgrt-0.6/pyproject.toml
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 tnsgrt-0.6/PKG-INFO
```

### Comparing `tnsgrt-0.5.2/.readthedocs.yaml` & `tnsgrt-0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/.github/workflows/python-publish.yml` & `tnsgrt-0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/.github/workflows/python-test.yml` & `tnsgrt-0.6/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/Makefile` & `tnsgrt-0.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/conf.py` & `tnsgrt-0.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/index.rst` & `tnsgrt-0.6/doc/index.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 `vispy <https://vispy.org>`_.
 
 .. toctree::
    :maxdepth: 3
    :caption: User guide
 
    usage/quickstart
-   usage/structure
    usage/properties
    usage/transformations
+   usage/structure
    usage/examples
 
 .. toctree::
    :maxdepth: 2
    :caption: Reference
 
    usage/modules
```

### Comparing `tnsgrt-0.5.2/doc/make.bat` & `tnsgrt-0.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/bicycle1.png` & `tnsgrt-0.6/doc/images/bicycle1.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/bicycle2.png` & `tnsgrt-0.6/doc/images/bicycle2.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/loaded.png` & `tnsgrt-0.6/doc/images/loaded.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/planar1.png` & `tnsgrt-0.6/doc/images/planar1.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/planar2.png` & `tnsgrt-0.6/doc/images/planar2.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/planar3.png` & `tnsgrt-0.6/doc/images/planar3.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/planar4.png` & `tnsgrt-0.6/doc/images/planar4.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/prisms.png` & `tnsgrt-0.6/doc/images/prisms.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson.png` & `tnsgrt-0.6/doc/images/snelson.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson1.png` & `tnsgrt-0.6/doc/images/snelson1.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson2.png` & `tnsgrt-0.6/doc/images/snelson2.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson3.png` & `tnsgrt-0.6/doc/images/snelson3.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson4.png` & `tnsgrt-0.6/doc/images/snelson4.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson5.png` & `tnsgrt-0.6/doc/images/snelson5.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson6.png` & `tnsgrt-0.6/doc/images/snelson6.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/snelson7.png` & `tnsgrt-0.6/doc/images/snelson7.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/images/stiffness1.png` & `tnsgrt-0.6/doc/images/stiffness1.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/usage/examples.rst` & `tnsgrt-0.6/doc/usage/examples.rst`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/usage/modules.rst` & `tnsgrt-0.6/doc/usage/modules.rst`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/usage/properties.rst` & `tnsgrt-0.6/doc/usage/properties.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,66 @@
+.. _properties:
+
 The structure of Structures
 ===========================
 
-Start by building the following simple planar structure
+The prisms seen in the quick start are members of :class:`tnsgrt.structure.Structure`. In fact,
+:class:`tnsgrt.prism.Prism` overloads only the constructor of :class:`tnsgrt.structure.Structure`, which provides most
+of the functionality.
+
+Construction
+------------
+
+Object of class :class:`tnsgrt.structure.Structure` are composed of *nodes* and *members*.
+Nodes are `3 x n` numpy arrays:
 
 .. code-block:: python
 
     import numpy as np
-    from tnsgrt.structure import Structure
+    nodes = np.array([[0,0,0],[0,1,0],[1,0,0],[1,1,0]]).transpose()
 
-    nodes = np.array([[0,0,0], [0,1,0], [2,1,0], [2,0,0]]).transpose()
-    members = np.array([[0,1], [1,2], [2,3], [3,0], [0,2], [1,3]]).transpose()
-    s = Structure(nodes, members, number_of_strings=4)
+Members are *bars* or *strings*, which are specified by a `2 x m` array with the indices of the nodes that define the
+members, as in:
 
-which is visualized as
+.. code-block:: python
 
-.. image:: /images/planar1.png
-  :scale: 50%
+    members = np.array([[0,1],[1,2],[2,3],[3,0],[0,2],[1,3]]).transpose()
 
-by the following code:
+Nodes and members are then combined to build a :class:`tnsgrt.structure.Structure`:
 
 .. code-block:: python
 
-    from matplotlib import pyplot as plt
-    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
-    %matplotlib widget
+    from tnsgrt import Structure
+    s = Structure(nodes, members, number_of_strings=4)
+
+The parameter ``number_of_strings = 4`` means that the first four members are to be considered strings.
+
+As before, the resulting structure can be plotted using :class:`tnsgrt.plotter.MatplotlibPlotter`:
 
+.. code-block:: python
+
+    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
     plotter = MatplotlibPlotter()
     plotter.plot(s)
     fig, ax = plotter.get_handles()
     ax.view_init(90,-90)
     ax.axis('equal')
     ax.axis('off')
     plt.show()
 
-Accessing data
---------------
+to visualize the resulting planar tensegrity structure below:
+
+.. image:: /images/planar1.png
+  :scale: 50%
 
 Quite often, it is useful to view and modify the data stored in a
 Structure. The following examples show several ways of doing that.
 
 Nodes and members
-^^^^^^^^^^^^^^^^^
+-----------------
 
 A string representation of a Structure displays its number of nodes,
 number of bars, and number of strings. Typing
 
 .. code-block:: python
 
     print(s)
@@ -58,34 +74,72 @@
 
 .. code-block:: python
 
     s.nodes
 
 which is a 3 x n numpy array ::
 
-     array([[0., 0., 2., 2.],
+     array([[0., 0., 1., 1.],
             [0., 1., 1., 0.],
             [0., 0., 0., 0.]])
 
 storing the Structure's nodes in its columns, and ``members``
 
 .. code-block:: python
 
     s.members
 
 which is a 2 x m numpy array::
 
      array([[0, 1, 2, 3, 0, 1],
             [1, 2, 3, 0, 2, 3]], dtype=int64)
 
-storing the Structure's members. Each column of ``member`` stores the indices of the nodes to which the
-ends of a bar or of a string is connected to.
+storing the Structure's members. Each column of ``member`` stores the indices of the
+nodes to which the ends of a bar or of a string is connected to.
+
+The values of nodes can be accessed or modified using the convenience methods
+:meth:`tnsgrt.structure.Structure.get_node_values` and
+:meth:`tnsgrt.structure.Structure.set_node_values`. For example:
+
+.. code-block:: python
+
+    s.set_node_values([2, 3], np.array([[2, 1, 0], [2, 0, 0]]).transpose())
+
+modify the location of nodes 2 and 3, and
+
+.. code-block:: python
+
+    s.get_node_values([2, 3])
+
+retrieves the updated values::
+
+     array([[2., 2.],
+            [1., 0.],
+            [0., 0.]])
+
+The change is reflected in the structure geometry, which now looks as in the new figure
+
+.. image:: /images/planar5.png
+  :scale: 50%
+
+generated by the code
+
+.. code-block:: python
+
+    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
+    plotter = MatplotlibPlotter()
+    plotter.plot(s)
+    fig, ax = plotter.get_handles()
+    ax.view_init(90,-90)
+    ax.axis('equal')
+    ax.axis('off')
+    plt.show()
 
 Properties
-^^^^^^^^^^
+----------
 
 Node and member properties are stored as pandas' Dataframes. In this
 example
 
 .. code-block:: python
 
     s.node_properties
@@ -126,15 +180,15 @@
      0  (0.85, 0.325, 0.098)          2         -
      1  (0.85, 0.325, 0.098)          2         -
      2  (0.85, 0.325, 0.098)          2         -
      3  (0.85, 0.325, 0.098)          2         -
      4     (0, 0.447, 0.741)          2         -
      5     (0, 0.447, 0.741)          2         -
 
-The DataFrames can be manipulated directly or one can use some
+The DataFrames can be manipulated directly or one can use
 convenience methods that will be discussed later.
 
 Properties are populated with default values taken from
 ``Structure.NodeProperty``, ``Structure.MemberProperty``, and the
 values in the dictionary
 
 .. code-block:: python
@@ -147,15 +201,15 @@
       'string': {'facecolor': (0.85, 0.325, 0.098),
        'edgecolor': (0.85, 0.325, 0.098),
        'radius': 0.005}}
 
 The keys in this dictionary are *tags*, which we discuss next.
 
 Tags
-^^^^
+----
 
 Nodes and members can be assigned and manipulated via *tags*. Nodes
 do not have any default tag, as
 
 .. code-block:: python
 
     s.node_tags
@@ -215,19 +269,19 @@
 
 which returns::
 
      ['string', 'vertical']
 
 Similar methods exist to manipulate node tags.
 
-Retrieving and setting properties
----------------------------------
+Member and node properties
+--------------------------
 
 Even though it is possible to manipulate the property
-``DataFrame``\ s directly, it is sometimes easier to use some
+``DataFrame``\ s directly, it is often easier to use the provided
 convenience methods.
 
 For example
 
 .. code-block:: python
 
     s.get_member_properties(s.get_members_by_tag('vertical'), 'radius', 'facecolor', 'edgecolor')
```

### Comparing `tnsgrt-0.5.2/doc/usage/quickstart.rst` & `tnsgrt-0.6/doc/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/doc/usage/transformations.rst` & `tnsgrt-0.6/doc/usage/transformations.rst`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/examples/examples.ipynb` & `tnsgrt-0.6/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/examples/properties.ipynb` & `tnsgrt-0.6/examples/properties.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9613042773199023%*

 * *Differences: {"'cells'": "{3: {'source': ['## Construction\\n', '\\n', 'Objects of class "*

 * *            '`tnsgrt.structure.Structure` are composed of *nodes* and *members*. Nodes are `3 x n` '*

 * *            "numpy arrays']}, 4: {'source': {insert: [(1, 'nodes = "*

 * *            "np.array([[0,0,0],[0,1,0],[1,1,0],[1,0,0]]).transpose()')], delete: [5, 4, 3, 2, "*

 * *            "1]}}, 10: {'execution_count': 5, 'outputs': {0: {'data': {'text/plain': "*

 * *            '["Canvas(toolbar=Toolbar(toolitems=[(\'Home\', \'Reset original view […]*

```diff
@@ -18,82 +18,143 @@
                 "sys.path.append('../src')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Start by building the following simple planar structure"
+                "The prisms seen in the quick start are members of `tnsgrt.structure.Structure`. In fact,\n",
+                "`tnsgrt.prism.Prism` overloads only the constructor of `tnsgrt.structure.Structure`, which provides most\n",
+                "of the functionality."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Construction\n",
+                "\n",
+                "Objects of class `tnsgrt.structure.Structure` are composed of *nodes* and *members*. Nodes are `3 x n` numpy arrays"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
+                "nodes = np.array([[0,0,0],[0,1,0],[1,1,0],[1,0,0]]).transpose()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Members are *bars* or *strings*, which are specified by a `2 x m` array with the indices of the nodes that define the\n",
+                "members, as in:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "members = np.array([[0,1],[1,2],[2,3],[3,0],[0,2],[1,3]]).transpose()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Nodes and members are then combined to build a `tnsgrt.structure.Structure`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "from tnsgrt.structure import Structure\n",
-                "\n",
-                "nodes = np.array([[0,0,0], [0,1,0], [2,1,0], [2,0,0]]).transpose()\n",
-                "members = np.array([[0,1], [1,2], [2,3], [3,0], [0,2], [1,3]]).transpose()\n",
                 "s = Structure(nodes, members, number_of_strings=4)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The parameter `number_of_strings = 4` means that the first four members are to be considered *strings*.\n",
+                "\n",
+                "As before, the resulting structure can be plotted using `tnsgrt.plotter.MatplotlibPlotter`"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "3bc730fc6ee749128931889087fac023",
+                            "model_id": "782ede6f1aa649f5986d77ad61334481",
                             "version_major": 2,
                             "version_minor": 0
                         },
-                        "image/png": "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",
-                        "text/html": "\n            <div style=\"display: inline-block;\">\n                <div class=\"jupyter-widgets widget-label\" style=\"text-align: center;\">\n                    Figure\n                </div>\n                <img src='data:image/png;base64,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' width=640.0/>\n            </div>\n        ",
-                        "text/plain": "Canvas(toolbar=Toolbar(toolitems=[('Home', 'Reset original view', 'home', 'home'), ('Back', 'Back to previous \u2026"
+                        "image/png": "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",
+                        "text/html": [
+                            "\n",
+                            "            <div style=\"display: inline-block;\">\n",
+                            "                <div class=\"jupyter-widgets widget-label\" style=\"text-align: center;\">\n",
+                            "                    Figure\n",
+                            "                </div>\n",
+                            "                <img src='data:image/png;base64,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' width=640.0/>\n",
+                            "            </div>\n",
+                            "        "
+                        ],
+                        "text/plain": [
+                            "Canvas(toolbar=Toolbar(toolitems=[('Home', 'Reset original view', 'home', 'home'), ('Back', 'Back to previous \u2026"
+                        ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "from matplotlib import pyplot as plt\n",
                 "from tnsgrt.plotter.matplotlib import MatplotlibPlotter\n",
                 "%matplotlib widget\n",
                 "\n",
                 "plotter = MatplotlibPlotter()\n",
                 "plotter.plot(s)\n",
-                "fig, ax = plotter.get_handles()\n",
+                "_, ax = plotter.get_handles()\n",
                 "ax.view_init(90,-90)\n",
-                "ax.axis('equal')\n",
                 "ax.axis('off')\n",
+                "ax.axis('equal')\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Accessing Structure data\n",
+                "to visualize the resulting planar tensegrity structure built above.\n",
                 "\n",
                 "Quite often, it is useful to view and modify the data stored in a Structure. The following\n",
                 "examples show several ways of doing that.\n",
                 "\n",
                 "### Nodes and members\n",
                 "\n",
                 "A string representation of a Structure displays its number of nodes, number of bars, and number of strings."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Structure with 4 nodes, 2 bars and 4 strings\n"
@@ -109,22 +170,26 @@
             "metadata": {},
             "source": [
                 "A Structure has as attributes `nodes`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([[0., 0., 2., 2.],\n       [0., 1., 1., 0.],\n       [0., 0., 0., 0.]])"
+                        "text/plain": [
+                            "array([[0., 0., 1., 1.],\n",
+                            "       [0., 1., 1., 0.],\n",
+                            "       [0., 0., 0., 0.]])"
+                        ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.nodes"
             ]
@@ -134,52 +199,220 @@
             "metadata": {},
             "source": [
                 "which is a 3 x n numpy array storing the Structure's nodes in its columns and `members`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([[0, 1, 2, 3, 0, 1],\n       [1, 2, 3, 0, 2, 3]], dtype=int64)"
+                        "text/plain": [
+                            "array([[0, 1, 2, 3, 0, 1],\n",
+                            "       [1, 2, 3, 0, 2, 3]], dtype=int64)"
+                        ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.members"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "which is a 2 x m numpy array storing the Structure's members. Each column of `member` stores the indices of the nodes to which the ends of a bar or of a string is connected to.\n",
                 "\n",
-                "### Properties\n",
+                "The values of nodes can be accessed or modified using the convenience methods\n",
+                ":meth:`tnsgrt.structure.Structure.get_node_values` and\n",
+                ":meth:`tnsgrt.structure.Structure.set_node_values`. For example:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "s.set_node_values([2, 3], np.array([[2, 1, 0], [2, 0, 0]]).transpose())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "modify the location of nodes 2 and 3, and"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[2., 2.],\n",
+                            "       [1., 0.],\n",
+                            "       [0., 0.]])"
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "s.get_node_values([2, 3])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "retrieves the updated values\n",
+                "\n",
+                "The change is reflected in the structure geometry, which now looks as in the new figure generated by the code"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "4426baac5a704b6d95d571ae0197fdb0",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "image/png": "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",
+                        "text/html": [
+                            "\n",
+                            "            <div style=\"display: inline-block;\">\n",
+                            "                <div class=\"jupyter-widgets widget-label\" style=\"text-align: center;\">\n",
+                            "                    Figure\n",
+                            "                </div>\n",
+                            "                <img src='data:image/png;base64,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' width=640.0/>\n",
+                            "            </div>\n",
+                            "        "
+                        ],
+                        "text/plain": [
+                            "Canvas(toolbar=Toolbar(toolitems=[('Home', 'Reset original view', 'home', 'home'), ('Back', 'Back to previous \u2026"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "plotter = MatplotlibPlotter()\n",
+                "plotter.plot(s)\n",
+                "_, ax = plotter.get_handles()\n",
+                "ax.view_init(90,-90)\n",
+                "ax.axis('off')\n",
+                "ax.axis('equal')\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Properties\n",
                 "\n",
                 "Node and member properties are stored as pandas' Dataframes. In this example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>radius</th>\n      <th>visible</th>\n      <th>constraint</th>\n      <th>facecolor</th>\n      <th>edgecolor</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>0.002</td>\n      <td>True</td>\n      <td>None</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>(0, 0.447, 0.741)</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>0.002</td>\n      <td>True</td>\n      <td>None</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>(0, 0.447, 0.741)</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>0.002</td>\n      <td>True</td>\n      <td>None</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>(0, 0.447, 0.741)</td>\n    </tr>\n    <tr>\n      <th>3</th>\n      <td>0.002</td>\n      <td>True</td>\n      <td>None</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>(0, 0.447, 0.741)</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "   radius  visible constraint          facecolor          edgecolor\n0   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)\n1   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)\n2   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)\n3   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)"
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>radius</th>\n",
+                            "      <th>visible</th>\n",
+                            "      <th>constraint</th>\n",
+                            "      <th>facecolor</th>\n",
+                            "      <th>edgecolor</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>0.002</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>None</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>0.002</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>None</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>0.002</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>None</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>0.002</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>None</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   radius  visible constraint          facecolor          edgecolor\n",
+                            "0   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)\n",
+                            "1   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)\n",
+                            "2   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)\n",
+                            "3   0.002     True       None  (0, 0.447, 0.741)  (0, 0.447, 0.741)"
+                        ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.node_properties"
             ]
@@ -189,23 +422,202 @@
             "metadata": {},
             "source": [
                 "and"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>lambda_</th>\n      <th>force</th>\n      <th>stiffness</th>\n      <th>volume</th>\n      <th>radius</th>\n      <th>inner_radius</th>\n      <th>mass</th>\n      <th>rest_length</th>\n      <th>yld</th>\n      <th>density</th>\n      <th>modulus</th>\n      <th>visible</th>\n      <th>facecolor</th>\n      <th>edgecolor</th>\n      <th>linewidth</th>\n      <th>linestyle</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.005</td>\n      <td>0.0</td>\n      <td>1.0</td>\n      <td>0.0</td>\n      <td>250000000.0</td>\n      <td>7850.0</td>\n      <td>2.000000e+11</td>\n      <td>True</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>2</td>\n      <td>-</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.005</td>\n      <td>0.0</td>\n      <td>1.0</td>\n      <td>0.0</td>\n      <td>250000000.0</td>\n      <td>7850.0</td>\n      <td>2.000000e+11</td>\n      <td>True</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>2</td>\n      <td>-</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.005</td>\n      <td>0.0</td>\n      <td>1.0</td>\n      <td>0.0</td>\n      <td>250000000.0</td>\n      <td>7850.0</td>\n      <td>2.000000e+11</td>\n      <td>True</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>2</td>\n      <td>-</td>\n    </tr>\n    <tr>\n      <th>3</th>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.005</td>\n      <td>0.0</td>\n      <td>1.0</td>\n      <td>0.0</td>\n      <td>250000000.0</td>\n      <td>7850.0</td>\n      <td>2.000000e+11</td>\n      <td>True</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>2</td>\n      <td>-</td>\n    </tr>\n    <tr>\n      <th>4</th>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.010</td>\n      <td>0.0</td>\n      <td>1.0</td>\n      <td>0.0</td>\n      <td>250000000.0</td>\n      <td>7850.0</td>\n      <td>2.000000e+11</td>\n      <td>True</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>2</td>\n      <td>-</td>\n    </tr>\n    <tr>\n      <th>5</th>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.0</td>\n      <td>0.010</td>\n      <td>0.0</td>\n      <td>1.0</td>\n      <td>0.0</td>\n      <td>250000000.0</td>\n      <td>7850.0</td>\n      <td>2.000000e+11</td>\n      <td>True</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>(0, 0.447, 0.741)</td>\n      <td>2</td>\n      <td>-</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "   lambda_  force  stiffness  volume  radius  inner_radius  mass  rest_length   \n0      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0  \\\n1      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0   \n2      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0   \n3      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0   \n4      0.0    0.0        0.0     0.0   0.010           0.0   1.0          0.0   \n5      0.0    0.0        0.0     0.0   0.010           0.0   1.0          0.0   \n\n           yld  density       modulus  visible             facecolor   \n0  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)  \\\n1  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)   \n2  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)   \n3  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)   \n4  250000000.0   7850.0  2.000000e+11     True     (0, 0.447, 0.741)   \n5  250000000.0   7850.0  2.000000e+11     True     (0, 0.447, 0.741)   \n\n              edgecolor  linewidth linestyle  \n0  (0.85, 0.325, 0.098)          2         -  \n1  (0.85, 0.325, 0.098)          2         -  \n2  (0.85, 0.325, 0.098)          2         -  \n3  (0.85, 0.325, 0.098)          2         -  \n4     (0, 0.447, 0.741)          2         -  \n5     (0, 0.447, 0.741)          2         -  "
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>lambda_</th>\n",
+                            "      <th>force</th>\n",
+                            "      <th>stiffness</th>\n",
+                            "      <th>volume</th>\n",
+                            "      <th>radius</th>\n",
+                            "      <th>inner_radius</th>\n",
+                            "      <th>mass</th>\n",
+                            "      <th>rest_length</th>\n",
+                            "      <th>yld</th>\n",
+                            "      <th>density</th>\n",
+                            "      <th>modulus</th>\n",
+                            "      <th>visible</th>\n",
+                            "      <th>facecolor</th>\n",
+                            "      <th>edgecolor</th>\n",
+                            "      <th>linewidth</th>\n",
+                            "      <th>linestyle</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.005</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>250000000.0</td>\n",
+                            "      <td>7850.0</td>\n",
+                            "      <td>2.000000e+11</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>-</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.005</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>250000000.0</td>\n",
+                            "      <td>7850.0</td>\n",
+                            "      <td>2.000000e+11</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>-</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.005</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>250000000.0</td>\n",
+                            "      <td>7850.0</td>\n",
+                            "      <td>2.000000e+11</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>-</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.005</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>250000000.0</td>\n",
+                            "      <td>7850.0</td>\n",
+                            "      <td>2.000000e+11</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>-</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.010</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>250000000.0</td>\n",
+                            "      <td>7850.0</td>\n",
+                            "      <td>2.000000e+11</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>-</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.010</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>250000000.0</td>\n",
+                            "      <td>7850.0</td>\n",
+                            "      <td>2.000000e+11</td>\n",
+                            "      <td>True</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>(0, 0.447, 0.741)</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>-</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   lambda_  force  stiffness  volume  radius  inner_radius  mass  rest_length   \n",
+                            "0      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0  \\\n",
+                            "1      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0   \n",
+                            "2      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0   \n",
+                            "3      0.0    0.0        0.0     0.0   0.005           0.0   1.0          0.0   \n",
+                            "4      0.0    0.0        0.0     0.0   0.010           0.0   1.0          0.0   \n",
+                            "5      0.0    0.0        0.0     0.0   0.010           0.0   1.0          0.0   \n",
+                            "\n",
+                            "           yld  density       modulus  visible             facecolor   \n",
+                            "0  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)  \\\n",
+                            "1  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)   \n",
+                            "2  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)   \n",
+                            "3  250000000.0   7850.0  2.000000e+11     True  (0.85, 0.325, 0.098)   \n",
+                            "4  250000000.0   7850.0  2.000000e+11     True     (0, 0.447, 0.741)   \n",
+                            "5  250000000.0   7850.0  2.000000e+11     True     (0, 0.447, 0.741)   \n",
+                            "\n",
+                            "              edgecolor  linewidth linestyle  \n",
+                            "0  (0.85, 0.325, 0.098)          2         -  \n",
+                            "1  (0.85, 0.325, 0.098)          2         -  \n",
+                            "2  (0.85, 0.325, 0.098)          2         -  \n",
+                            "3  (0.85, 0.325, 0.098)          2         -  \n",
+                            "4     (0, 0.447, 0.741)          2         -  \n",
+                            "5     (0, 0.447, 0.741)          2         -  "
+                        ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.member_properties"
             ]
@@ -217,51 +629,58 @@
                 "The DataFrames can be manipulated directly or one can use some convenience methods that will be discussed later.\n",
                 "\n",
                 "Properties are populated with default values taken from `Structure.NodeProperty`, `Structure.MemberProperty`, and the values in the dictionary"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "{'bar': {'facecolor': (0, 0.447, 0.741), 'edgecolor': (0, 0.447, 0.741)},\n 'string': {'facecolor': (0.85, 0.325, 0.098),\n  'edgecolor': (0.85, 0.325, 0.098),\n  'radius': 0.005}}"
+                        "text/plain": [
+                            "{'bar': {'facecolor': (0, 0.447, 0.741), 'edgecolor': (0, 0.447, 0.741)},\n",
+                            " 'string': {'facecolor': (0.85, 0.325, 0.098),\n",
+                            "  'edgecolor': (0.85, 0.325, 0.098),\n",
+                            "  'radius': 0.005}}"
+                        ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "Structure.member_defaults"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The keys in this dictionary are *tags*, which we discuss next.\n",
                 "\n",
-                "### Tags\n",
+                "## Tags\n",
                 "\n",
                 "Nodes and members can be assigned and manipulated via *tags*. Nodes do not have any default tag,"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "{}"
+                        "text/plain": [
+                            "{}"
+                        ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.node_tags"
             ]
@@ -271,22 +690,24 @@
             "metadata": {},
             "source": [
                 "but members are automatically assigned either `bar` or `string` as a tag."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "{'bar': array([4, 5], dtype=int64), 'string': array([0, 1, 2, 3], dtype=int64)}"
+                        "text/plain": [
+                            "{'bar': array([4, 5], dtype=int64), 'string': array([0, 1, 2, 3], dtype=int64)}"
+                        ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.member_tags"
             ]
@@ -300,15 +721,15 @@
                 "It is always recommended to manipulate tags using the convenience methods of `tnsgrt.structure.Structure`, which take care of keeping the member and node indices unique and sorted.\n",
                 "\n",
                 "Additional member tags can be assigned using `tnsgrt.structure.Structure.add_member_tag`. For example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s.add_member_tag('vertical', [0, 2])"
             ]
         },
         {
@@ -316,22 +737,24 @@
             "metadata": {},
             "source": [
                 "creates a new tag `vertical` and associated the two members with indices `0` and `2` to it. Conversely, `tnsgrt.structure.Structure.get_members_by_tag` retrieves the member indices associated with a given tag, as in"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([0, 2])"
+                        "text/plain": [
+                            "array([0, 2])"
+                        ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.get_members_by_tag('vertical')"
             ]
@@ -341,54 +764,100 @@
             "metadata": {},
             "source": [
                 "while `tnsgrt.structure.Structure.get_member_tags` retrieve all tags associated with a given member index:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "['string', 'vertical']"
+                        "text/plain": [
+                            "['string', 'vertical']"
+                        ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.get_member_tags(2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Similar methods exist to manipulate node tags.\n",
                 "\n",
-                "### Retrieving and setting properties\n",
+                "## Member and node properties\n",
                 "\n",
-                "Even though it is possible to manipulate the property `DataFrame`s directly, it is sometimes easier to use some convenience methods.\n",
+                "Even though it is possible to manipulate the property `DataFrame`s directly, it is often easier to use the provided convenience methods.\n",
                 "\n",
                 "For example"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>radius</th>\n      <th>facecolor</th>\n      <th>edgecolor</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>0.005</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>(0.85, 0.325, 0.098)</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>0.005</td>\n      <td>(0.85, 0.325, 0.098)</td>\n      <td>(0.85, 0.325, 0.098)</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "   radius             facecolor             edgecolor\n0   0.005  (0.85, 0.325, 0.098)  (0.85, 0.325, 0.098)\n2   0.005  (0.85, 0.325, 0.098)  (0.85, 0.325, 0.098)"
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>radius</th>\n",
+                            "      <th>facecolor</th>\n",
+                            "      <th>edgecolor</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>0.005</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>0.005</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "      <td>(0.85, 0.325, 0.098)</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   radius             facecolor             edgecolor\n",
+                            "0   0.005  (0.85, 0.325, 0.098)  (0.85, 0.325, 0.098)\n",
+                            "2   0.005  (0.85, 0.325, 0.098)  (0.85, 0.325, 0.098)"
+                        ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.get_member_properties(s.get_members_by_tag('vertical'), 'radius', 'facecolor', 'edgecolor')"
             ]
@@ -400,15 +869,15 @@
                 "retrieves a view of the member's properties that have `vertical` as a tag.\n",
                 "\n",
                 "Conversely"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s.set_member_properties(s.get_members_by_tag('vertical'), 'radius', 0.04)"
             ]
         },
         {
@@ -418,15 +887,15 @@
                 "sets the `radius` property of the members that have `vertical`\n",
                 "\n",
                 "`tnsgrt.structure.Structure.set_member_properties` can also be used to set multiple values at the same time, as in"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from tnsgrt.utils import Colors\n",
                 "\n",
                 "s.set_member_properties(s.get_members_by_tag('vertical'),\n",
                 "                        'facecolor', Colors.GREEN.value,\n",
@@ -439,23 +908,70 @@
             "metadata": {},
             "source": [
                 "Retrieving the properties confirm the changes:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>radius</th>\n      <th>mass</th>\n      <th>facecolor</th>\n      <th>edgecolor</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>0.04</td>\n      <td>2.0</td>\n      <td>(0.466, 0.674, 0.188)</td>\n      <td>(0.466, 0.674, 0.188)</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>0.04</td>\n      <td>2.0</td>\n      <td>(0.466, 0.674, 0.188)</td>\n      <td>(0.466, 0.674, 0.188)</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
-                        "text/plain": "   radius  mass              facecolor              edgecolor\n0    0.04   2.0  (0.466, 0.674, 0.188)  (0.466, 0.674, 0.188)\n2    0.04   2.0  (0.466, 0.674, 0.188)  (0.466, 0.674, 0.188)"
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>radius</th>\n",
+                            "      <th>mass</th>\n",
+                            "      <th>facecolor</th>\n",
+                            "      <th>edgecolor</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>0.04</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>(0.466, 0.674, 0.188)</td>\n",
+                            "      <td>(0.466, 0.674, 0.188)</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>0.04</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>(0.466, 0.674, 0.188)</td>\n",
+                            "      <td>(0.466, 0.674, 0.188)</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   radius  mass              facecolor              edgecolor\n",
+                            "0    0.04   2.0  (0.466, 0.674, 0.188)  (0.466, 0.674, 0.188)\n",
+                            "2    0.04   2.0  (0.466, 0.674, 0.188)  (0.466, 0.674, 0.188)"
+                        ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "s.get_member_properties(s.get_members_by_tag('vertical'), 'radius', 'mass', 'facecolor', 'edgecolor')"
             ]
@@ -465,41 +981,59 @@
             "metadata": {},
             "source": [
                 "These changes are also reflected on the structure's plot generated by the following code."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "91700bbb8b58457da51318228b4a10e9",
+                            "model_id": "bd68bd60bd5e4fbdb924eb9634ae4791",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "image/png": "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",
-                        "text/html": "\n            <div style=\"display: inline-block;\">\n                <div class=\"jupyter-widgets widget-label\" style=\"text-align: center;\">\n                    Figure\n                </div>\n                <img src='data:image/png;base64,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' width=640.0/>\n            </div>\n        ",
-                        "text/plain": "Canvas(toolbar=Toolbar(toolitems=[('Home', 'Reset original view', 'home', 'home'), ('Back', 'Back to previous \u2026"
+                        "text/html": [
+                            "\n",
+                            "            <div style=\"display: inline-block;\">\n",
+                            "                <div class=\"jupyter-widgets widget-label\" style=\"text-align: center;\">\n",
+                            "                    Figure\n",
+                            "                </div>\n",
+                            "                <img src='data:image/png;base64,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' width=640.0/>\n",
+                            "            </div>\n",
+                            "        "
+                        ],
+                        "text/plain": [
+                            "Canvas(toolbar=Toolbar(toolitems=[('Home', 'Reset original view', 'home', 'home'), ('Back', 'Back to previous \u2026"
+                        ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plotter = MatplotlibPlotter()\n",
                 "plotter.plot(s)\n",
                 "fig, ax = plotter.get_handles()\n",
                 "ax.view_init(90,-90)\n",
                 "ax.axis('equal')\n",
                 "ax.axis('off')\n",
                 "plt.show()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `tnsgrt-0.5.2/examples/quick_start.ipynb` & `tnsgrt-0.6/examples/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/examples/transformations.ipynb` & `tnsgrt-0.6/examples/transformations.ipynb`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/src/tnsgrt/michell.py` & `tnsgrt-0.6/src/tnsgrt/michell.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/src/tnsgrt/prism.py` & `tnsgrt-0.6/src/tnsgrt/prism.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/src/tnsgrt/stiffness.py` & `tnsgrt-0.6/src/tnsgrt/stiffness.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,35 +25,57 @@
            A x = 0
 
        then the equivalent constraint and its null space
 
        .. math::
            R \\, x = 0, \\quad x = T \\, y, \\quad R R^T = I, \\quad T^T T = I
 
-       is constructed using :func:`tnsgrt.utils.orthogonalize`
+       are constructed using :func:`tnsgrt.utils.orthogonalize`
     """
 
-    def __init__(self, constraint: Optional[npt.NDArray] = None, epsilon: float = 1e-8):
-        if constraint is None:
+    def __init__(self,
+                 constraint: Optional[npt.NDArray] = None,
+                 displacement: Optional[npt.NDArray] = None,
+                 epsilon: float = 1e-8):
+        assert constraint is None or displacement is None, \
+            'constraint and displacement cannot be both given'
+        if constraint is None and displacement is None:
+            # fixed constraint
             self.dof = 0
             self.basis = None
             self.normal = np.eye(3)
-        else:
+        elif constraint is not None:
+            # constraint is given
             assert constraint.ndim == 2 and constraint.shape[1] == 3 and \
-                   constraint.shape[0] < 3, 'normal must be a m x 3, m < 3, array'
+                   constraint.shape[0] < 3, 'constraint must be a m x 3, m < 3, array'
             # first orthogonalize
             rank, r, t = orthogonalize(constraint.transpose(),
                                        mode='complete', epsilon=epsilon)
             self.dof = 3 - rank
             if self.dof == 0:
                 self.basis = None
                 self.normal = np.eye(3)
             else:
                 self.normal = r.transpose()
                 self.basis = t
+        else:  # displacement is not None
+            # displacement is given
+            assert displacement.ndim == 2 and displacement.shape[0] == 3 and \
+                   displacement.shape[1] < 3, \
+                   'displacement must be a 3 x m, m < 3, array'
+            # first orthogonalize
+            rank, t, r = orthogonalize(displacement,
+                                       mode='complete', epsilon=epsilon)
+            self.dof = rank
+            if self.dof == 0:
+                self.basis = None
+                self.normal = np.eye(3)
+            else:
+                self.normal = r.transpose()
+                self.basis = t
 
     @staticmethod
     def node_constraint(nodes: npt.NDArray, constraints: Sequence['NodeConstraint'],
                         storage: Literal['sparse', 'dense'] = 'sparse') \
             -> Union[Tuple[npt.NDArray, npt.NDArray],
                      Tuple[scipy.sparse.csr_array, scipy.sparse.csr_array]]:
         """
@@ -70,71 +92,72 @@
         assert nodes.shape[0] == 3, 'nodes must be a 3 x m array'
         assert nodes.shape[1] == len(constraints), \
             'number of columns of nodes must be equal to to the number of constraints'
 
         # calculate degrees of freedom
         m = nodes.shape[1]
         noc = sum(3 - c.dof for c in constraints if c is not None)
-        dof = 3*m - noc
+        dof = 3 * m - noc
 
         if storage == 'sparse':
-            row_col_r = np.zeros((2, 3*noc))
-            data_r = np.zeros((3*noc))
-            row_col_t = np.zeros((2, 3*dof))
-            data_t = np.zeros((3*dof))
+            row_col_r = np.zeros((2, 3 * noc))
+            data_r = np.zeros((3 * noc))
+            row_col_t = np.zeros((2, 3 * dof))
+            data_t = np.zeros((3 * dof))
             jj = kk = 0
             for i, c in enumerate(constraints):
                 if c is None:
                     # add identity to basis
                     dofj = 3
-                    row_col_t[0, 3*kk:3*kk+3*dofj] = \
-                        np.kron(np.arange(3*i, 3*(i+1)), np.ones((3,)))
-                    row_col_t[1, 3*kk:3*kk+3*dofj] = \
-                        np.kron(np.arange(kk, kk+dofj), np.ones((3,)))
-                    data_t[3*kk:3*kk+3*dofj] = np.eye(dofj).flatten(order='C')
+                    row_col_t[0, 3 * kk:3 * kk + 3 * dofj] = \
+                        np.kron(np.arange(3 * i, 3 * (i + 1)), np.ones((3,)))
+                    row_col_t[1, 3 * kk:3 * kk + 3 * dofj] = \
+                        np.kron(np.arange(kk, kk + dofj), np.ones((3,)))
+                    data_t[3 * kk:3 * kk + 3 * dofj] = np.eye(dofj).flatten(order='C')
                     kk += dofj
                 else:
                     # add to normal
-                    nocj = 3-c.dof
-                    row_col_r[0, 3*jj:3*jj+3*nocj] = \
-                        np.kron(np.arange(jj, jj+nocj), np.ones((3,)))      # row
-                    row_col_r[1, 3*jj:3*jj+3*nocj] = \
-                        np.kron(np.ones((nocj,)), np.arange(3*i, 3*(i+1)))  # col
-                    data_r[3*jj:3*jj+3*nocj] = c.normal.flatten(order='C')
+                    nocj = 3 - c.dof
+                    row_col_r[0, 3 * jj:3 * jj + 3 * nocj] = \
+                        np.kron(np.arange(jj, jj + nocj), np.ones((3,)))  # row
+                    row_col_r[1, 3 * jj:3 * jj + 3 * nocj] = \
+                        np.kron(np.ones((nocj,)), np.arange(3 * i, 3 * (i + 1)))  # col
+                    data_r[3 * jj:3 * jj + 3 * nocj] = c.normal.flatten(order='C')
                     jj += nocj
                     if c.dof:
                         # add to basis
                         dofj = c.dof
-                        row_col_t[0, 3*kk:3*kk+3*dofj] = \
-                            np.kron(np.arange(3*i, 3*(i+1)), np.ones((dofj,)))  # row
-                        row_col_t[1, 3*kk:3*kk+3*dofj] = \
-                            np.kron(np.ones((3,)), np.arange(kk, kk+dofj))      # col
-                        data_t[3*kk:3*kk+3*dofj] = c.basis.flatten(order='C')
+                        row_col_t[0, 3 * kk:3 * kk + 3 * dofj] = \
+                            np.kron(np.arange(3 * i, 3 * (i + 1)),
+                                    np.ones((dofj,)))  # row
+                        row_col_t[1, 3 * kk:3 * kk + 3 * dofj] = \
+                            np.kron(np.ones((3,)), np.arange(kk, kk + dofj))  # col
+                        data_t[3 * kk:3 * kk + 3 * dofj] = c.basis.flatten(order='C')
                         kk += dofj
             R = scipy.sparse.coo_matrix((data_r, row_col_r),
-                                        shape=(noc, 3*m)).tocsr()
+                                        shape=(noc, 3 * m)).tocsr()
             T = scipy.sparse.coo_matrix((data_t, row_col_t),
-                                        shape=(3*m, dof)).tocsr()
+                                        shape=(3 * m, dof)).tocsr()
         else:
-            R = np.zeros((noc, 3*m))
-            T = np.zeros((3*m, dof))
+            R = np.zeros((noc, 3 * m))
+            T = np.zeros((3 * m, dof))
             jj = kk = 0
             for i, c in enumerate(constraints):
                 if c is None:
                     # add identity to basis
-                    T[3*i:3*(i+1), kk:kk+3] = np.eye(3)
+                    T[3 * i:3 * (i + 1), kk:kk + 3] = np.eye(3)
                     kk += 3
                 else:
                     # add to constraint
-                    nocj = 3-c.dof
-                    R[jj:jj+nocj, 3*i:3*(i+1)] = c.normal
+                    nocj = 3 - c.dof
+                    R[jj:jj + nocj, 3 * i:3 * (i + 1)] = c.normal
                     jj += nocj
                     if c.dof:
                         # add to basis
-                        T[3*i:3*(i+1), kk:kk+c.dof] = c.basis
+                        T[3 * i:3 * (i + 1), kk:kk + c.dof] = c.basis
                         kk += c.dof
 
         return R, T
 
     @staticmethod
     def rigid_body_three_point_constraint(nodes: npt.NDArray, epsilon: float = 1e-8) \
             -> Tuple['NodeConstraint', 'NodeConstraint', 'NodeConstraint']:
@@ -223,14 +246,15 @@
         vector
 
         The resulting tuple is compatible with
         :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
 
         :param nodes: 3 x n array of nodes
         :param normal: list with n constraints
+        :param epsilon: accuracy
         :param storage: if ``sparse``, returns sparse arrays
         :return: tuple with the constraint matrix, and its null space
         """
         assert nodes.shape[0] == 3, 'nodes must be a 3 x m array'
         if normal is None:
             normal = np.array([[0], [0], [1]])
         elif normal.ndim == 1 and normal.shape[0] == 3:
@@ -242,57 +266,57 @@
 
         # calculate normal and basis
         _, normal, basis = orthogonalize(normal, mode='complete', epsilon=epsilon)
 
         # calculate degrees of freedom
         n = nodes.shape[1]
         noc = n
-        dof = 2*n
+        dof = 2 * n
 
         if storage == 'sparse':
-            row_col_r = np.zeros((2, 3*noc))
-            data_r = np.zeros((3*noc))
-            row_col_t = np.zeros((2, 3*dof))
-            data_t = np.zeros((3*dof))
+            row_col_r = np.zeros((2, 3 * noc))
+            data_r = np.zeros((3 * noc))
+            row_col_t = np.zeros((2, 3 * dof))
+            data_t = np.zeros((3 * dof))
             jj = kk = 0
             # flatten normal and basis
             normal = normal.flatten(order='C')
             basis = basis.flatten(order='C')
             nocj, dofj = 1, 2
             for i in range(n):
                 # add to constraint
-                row_col_r[0, 3*jj:3*jj+3*nocj] = \
-                    np.kron(np.arange(jj, jj+nocj), np.ones((3,)))      # row
-                row_col_r[1, 3*jj:3*jj+3*nocj] = \
-                    np.kron(np.ones((nocj,)), np.arange(3*i, 3*(i+1)))  # col
-                data_r[3*jj:3*jj+3*nocj] = normal
+                row_col_r[0, 3 * jj:3 * jj + 3 * nocj] = \
+                    np.kron(np.arange(jj, jj + nocj), np.ones((3,)))  # row
+                row_col_r[1, 3 * jj:3 * jj + 3 * nocj] = \
+                    np.kron(np.ones((nocj,)), np.arange(3 * i, 3 * (i + 1)))  # col
+                data_r[3 * jj:3 * jj + 3 * nocj] = normal
                 jj += nocj
                 # add to basis
-                row_col_t[0, 3*kk:3*kk+3*dofj] = \
-                    np.kron(np.arange(3*i, 3*(i+1)), np.ones((dofj,)))  # row
-                row_col_t[1, 3*kk:3*kk+3*dofj] = \
-                    np.kron(np.ones((3,)), np.arange(kk, kk+dofj))      # col
-                data_t[3*kk:3*kk+3*dofj] = basis
+                row_col_t[0, 3 * kk:3 * kk + 3 * dofj] = \
+                    np.kron(np.arange(3 * i, 3 * (i + 1)), np.ones((dofj,)))  # row
+                row_col_t[1, 3 * kk:3 * kk + 3 * dofj] = \
+                    np.kron(np.ones((3,)), np.arange(kk, kk + dofj))  # col
+                data_t[3 * kk:3 * kk + 3 * dofj] = basis
                 kk += dofj
             R = scipy.sparse.coo_matrix((data_r, row_col_r),
-                                        shape=(noc, 3*n)).tocsr()
+                                        shape=(noc, 3 * n)).tocsr()
             T = scipy.sparse.coo_matrix((data_t, row_col_t),
-                                        shape=(3*n, dof)).tocsr()
+                                        shape=(3 * n, dof)).tocsr()
         else:
-            R = np.zeros((noc, 3*n))
-            T = np.zeros((3*n, dof))
+            R = np.zeros((noc, 3 * n))
+            T = np.zeros((3 * n, dof))
             jj = kk = 0
             nocj, dofj = 1, 2
             normal = normal.flatten()
             for i in range(n):
                 # add to constraint
-                R[jj:jj+nocj, 3*i:3*(i+1)] = normal
+                R[jj:jj + nocj, 3 * i:3 * (i + 1)] = normal
                 jj += nocj
                 # add to basis
-                T[3*i:3*(i+1), kk:kk+dofj] = basis
+                T[3 * i:3 * (i + 1), kk:kk + dofj] = basis
                 kk += dofj
 
         return R, T
 
 
 class Stiffness:
     """
@@ -353,27 +377,29 @@
             assert M.ndim == 2 and M.shape[0] == M.shape[1] \
                    and M.shape[0] == K.shape[0], \
                 'M must be a square matrix of same size as K'
 
     def apply_constraint(self,
                          R: Union[npt.NDArray, scipy.sparse.csr_matrix],
                          T: Optional[Union[npt.NDArray, \
-                                           scipy.sparse.csr_matrix]] = None,
-                         local: bool = True, epsilon: float = 1e-8):
+                                     scipy.sparse.csr_matrix]] = None,
+                         local: bool = True, verbose: bool = True,
+                         epsilon: float = 1e-8):
         """
         Apply the constraint
 
         .. math::
             R \\, y = 0, \\qquad y = T z
 
         to the current or the global ``Stiffness`` object coordinate
 
         :param R: the constraint coefficient matrix
         :param T: the allowed node displacements; if ``None`` constraint is normalized
         :param local: if ``True`` the constraint is applied
+        :param verbose: if ``True`` print warnings
         :param epsilon: precision used to assess numerical rank
         :return:
 
         **Notes:**
 
         1. If ``local = True`` and the current constraints are
 
@@ -465,15 +491,15 @@
             if self.T is None:
                 self.T = t
             else:
                 self.T = self.T @ t
 
         else:
             # not local and self.T is not None
-            if T is not None:
+            if T is not None and verbose:
                 warnings.warn("allowed displacements parameter 'T' ignored when "
                               "'local=False'")
             self.apply_constraint(R @ self.T, epsilon=epsilon)
 
     def displacements(self, f: npt.NDArray):
         """
         Calculate displacements due to the application of a global force
@@ -485,20 +511,20 @@
 
         1. The displacements are calculated in global coordinates
 
            .. math::
                x = T K^{-1} T^T f
         """
         m = self.K.shape[0] if self.T is None else self.T.shape[0]
-        assert f.shape[0] == 3 and f.shape[1] == m/3, 'f must be a 3 x m array'
+        assert f.shape[0] == 3 and f.shape[1] == m / 3, 'f must be a 3 x m array'
         x = self.T @ np.linalg.solve(self.K,
                                      self.T.transpose() @ f.flatten(order='F')) \
             if self.T is not None else \
             np.linalg.solve(self.K, f.flatten(order='F'))
-        return x.reshape((3, int(m/3)), order='F')
+        return x.reshape((3, int(m / 3)), order='F')
 
     def eigs(self, k: int = 12,
              which: Literal['LM', 'SM', 'LR', 'SR', 'LI', 'SI'] = 'SM'):
         """
         Compute the eigenvalues and eigenvectors of the stiffness matrix
 
         If the stiffness matrix is stored as a sparse array, return only the first k
@@ -562,18 +588,17 @@
         else:
             # calculate dense eigenvalues
             d, v = scipy.linalg.eigh(self.K, self.M)
 
         # calculate frequencies
         d = np.sqrt(np.abs(d))
         if units == 'Hz':
-            d /= 2*np.pi
+            d /= 2 * np.pi
 
         # sort
         ind = np.argsort(d)
 
         # project eigenvectors
         if self.T is not None:
             v = self.T @ v
 
         return d[ind], v[:, ind]
-
```

### Comparing `tnsgrt-0.5.2/src/tnsgrt/structure.py` & `tnsgrt-0.6/src/tnsgrt/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from functools import reduce
 from typing import Optional, Dict, get_type_hints, Union, List, Sequence, \
     Type, Iterable, Tuple, Set, Any
 from collections import ChainMap, defaultdict
 
 import numpy as np
 import numpy.typing as npt
+import pandas
 import pandas as pd
 import scipy
 
 from . import utils
 from . import optim
 from .stiffness import Stiffness, NodeConstraint
 from .utils import is_colinear
@@ -162,14 +163,35 @@
         # test dimensions
         assert np.all(nodes.shape == self.nodes.shape), \
             'nodes shape must match current shape'
 
         # set nodes
         self.nodes: npt.NDArray[np.float_] = nodes
 
+    def get_node_values(self, index: Union[int, Sequence[int], slice]) -> npt.NDArray:
+        """
+        Get node values
+
+        :param index: the index of the nodes to get;
+                      can be a slice, integer, or sequence
+        :return: the node values
+        """
+        return self.nodes[:, index]
+
+    def set_node_values(self, index: Union[int, Sequence[int], slice],
+                        nodes: npt.NDArray) -> None:
+        """
+        Set node values
+
+        :param index: the index of the nodes to set;
+                      can be a slice, integer, or sequence
+        :param nodes: the values to set
+        """
+        self.nodes[:, index] = nodes
+
     def add_nodes(self, nodes: npt.ArrayLike,
                   node_tags: Optional[Dict[str, npt.NDArray[np.int64]]] = None) -> None:
         """
         Add nodes to the ``Structure``
 
         :param nodes: the nodes to add
         :param node_tags: the node tags to add
@@ -1160,15 +1182,15 @@
         self.member_properties = \
             pd.concat((self.member_properties, s.member_properties), ignore_index=True)
 
     def equilibrium(self,
                     force: Optional[npt.ArrayLike] = None,
                     lambda_bar: Optional[float] = None,
                     equalities: Optional[List[npt.ArrayLike]] = None,
-                    epsilon: float = 1e-7) -> None:
+                    epsilon: float = 1e-7) -> npt.NDArray:
         """
         Solves for the set of internal forces that ensures the equilibrium of the
         current ``Structure`` in response to the vector of external forces ``forces``
 
         Solve the force equilibrium equation
 
         .. math::
@@ -1226,26 +1248,28 @@
 
             **WARNING:** This problem may not be feasible for all
             :math:`\\bar{\\lambda} > 0`!
 
         """
 
         number_of_nodes = self.get_number_of_nodes()
-        number_of_strings = len(self.member_tags.get('string', []))
-        number_of_bars = len(self.member_tags.get('bar', []))
+
+        strings = self.member_tags.get('string', [])
+        bars = self.member_tags.get('bar', [])
+        number_of_strings = len(strings)
+        number_of_bars = len(bars)
         number_of_members = number_of_strings + number_of_bars
 
         assert number_of_members == number_of_bars + number_of_strings, \
             'number of members is not equal to the sum of number of bars and strings'
 
         assert lambda_bar is None or lambda_bar >= 0, 'lambda_bar cannot be negative'
 
         # member vectors
         member_vectors = self.get_member_vectors()
-        strings = self.member_tags['string']
 
         # coefficient matrix
         Aeq = np.zeros((3 * number_of_nodes, number_of_members))
 
         # string coefficient
         if number_of_strings:
             for i in self.member_tags['string']:
@@ -1262,25 +1286,45 @@
 
                 ii = 3 * int(self.members[0, i])
                 Aeq[ii:ii+3, i] = member_vectors[:, i]
 
                 jj = 3 * int(self.members[1, i])
                 Aeq[jj:jj+3, i] = -member_vectors[:, i]
 
-        A = Aeq
-        m = 3 * number_of_nodes
+        # node constraints
+        constraints = self.node_properties['constraint']
+        has_constraints = constraints.isna().sum() < self.get_number_of_nodes()
+        if has_constraints:
+            number_of_reactions = sum(3 - c.dof for c in constraints if c is not None)
+            Ac = np.zeros((3*number_of_nodes, number_of_reactions))
+            jj = 0
+            for i, c in enumerate(constraints):
+                if c is not None:
+                    nocj = 3 - c.dof
+                    Ac[3*i:3*(i+1), jj:jj+nocj] = -c.normal.transpose()
+                    jj += nocj
+
+            A = np.hstack((Aeq, Ac))
+            # m = 3 * number_of_nodes + number_of_reactions
 
-        # sum of the bars
-        ee = np.ones((1, number_of_members)) / self.get_number_of_members_by_tag('bar')
-        ee[:, strings] = 0
-        # TODO: do we need to worry if no bars?
+        else:
+            number_of_reactions = 0
+            A = Aeq
+            # m = 3 * number_of_nodes
+
+        # average of the bars
+        ee = np.zeros((1, number_of_members + number_of_reactions))
+        if number_of_bars:
+            ee[:, bars] = 1 / number_of_bars
+        else:
+            ee[:, strings] = 1 / number_of_strings
+            warnings.warn('structure has no bars, prestressing strings')
 
         if force is None:
             # no external forces
-            # A = np.vstack((A, np.ones((1, number_of_members))))
             A = np.vstack((A, ee))
             blo = bup = np.hstack((np.zeros((3 * number_of_nodes,)), 1))
             if lambda_bar is None:
                 lambda_bar = 1
         else:
             # external forces
             beq = np.array(force)
@@ -1295,15 +1339,16 @@
 
         # For equilibrium: Aeq x = beq
 
         # impose equalities
         # indices in each row are set to be equal
         if equalities is not None:
             number_of_constraints = sum(map(len, equalities)) - len(equalities)
-            Aeq = np.zeros((number_of_constraints, number_of_members))
+            Aeq = np.zeros((number_of_constraints,
+                            number_of_members + number_of_reactions))
             beq = np.zeros((number_of_constraints, ))
             ii = 0
             for eqs in equalities:
                 nn = len(eqs)
                 for jj in range(1, nn):
                     Aeq[ii+jj-1, eqs[0]] = 1
                     Aeq[ii+jj-1, eqs[jj]] = -1
@@ -1312,45 +1357,66 @@
             blo = bup = np.hstack((blo, beq))
 
         # enforce strings have positive force coefficients
         # when there are no external forces set to one to avoid nontrivial solution
         xup = None
         xlo = None
         if number_of_strings:
-            xlo = np.full((number_of_members, ), -np.inf)
-            xlo[self.member_tags['string']] = 0
+            xlo = np.full((number_of_members + number_of_reactions, ), -np.inf)
+            xlo[strings] = 0
 
         # cost function
-        n = number_of_members
-        c = np.ones((n,))
+        # n = number_of_members + number_of_reactions
+        c = np.hstack((np.ones((number_of_members,)), np.zeros((number_of_reactions,))))
 
         # solve lp
-        cost, gamma, status = optim.lp(n, m, c, A, blo, bup, xlo, xup)
+        cost, gamma, status = optim.lp(c, A, blo, bup, xlo, xup)
 
         # if infeasible, throw error
         if status == 'infeasible':
+            # TODO: Should we run a feasibility test if numerical issues arise
+            # optim.feasibility(A, blo, bup, xlo, xup)
             raise Exception('could not find equilibrium')
 
+        # sum reactions at nodes
+        reactions = np.zeros((3, number_of_nodes))
+        if number_of_reactions:
+            fr = gamma[number_of_members:]
+            gamma = gamma[:number_of_members]
+            # set reactions per node
+            jj = 0
+            for i, c in enumerate(constraints):
+                if c is not None:
+                    nocj = 3 - c.dof
+                    reactions[:, i] = np.sum(fr[jj:jj+nocj] * c.normal.transpose(),
+                                             axis=1)
+                    jj += nocj
+
         # flip sign for bars
         lambda_ = gamma
         if number_of_bars:
-            lambda_[self.member_tags['bar']] *= -1
+            lambda_[bars] *= -1
 
             if force is None:
                 # scale solution for bars
-                scale = -np.sum(lambda_[self.member_tags['bar']]) / number_of_bars
+                scale = -np.sum(lambda_[bars]) / number_of_bars
                 lambda_ *= np.abs(lambda_bar) / scale
 
         # assign lambda
         self.member_properties['lambda_'] = lambda_
 
         # update force
         self.update_member_properties('force')
 
-    def stiffness(self, epsilon: float = 1e-6, storage: str = 'sparse',
+        # return reactions
+        return reactions
+
+    def stiffness(self,
+                  force: Optional[npt.ArrayLike] = None,
+                  epsilon: float = 1e-6, storage: str = 'sparse',
                   apply_rigid_body_constraint: bool = False,
                   apply_planar_constraint: bool = False):
         """
         Computes
 
         - `normal`: potential energy (1 x 1)
         - `F`: force vectors (3 x n)
@@ -1384,14 +1450,19 @@
         member_vectors = self.get_member_vectors()
         member_length = self.get_member_length()
 
         k = self.member_properties['stiffness'].values
         lambda_ = self.member_properties['lambda_'].values
         mass = self.member_properties['mass'].values
 
+        # raise error if k is not positive
+        if np.any(k < epsilon):
+            raise Exception('stiffness is not positive; did you call '
+                            'Structure.update_members()?')
+
         # compute potential
         v = np.sum(((lambda_ * member_length) ** 2) / k / 2)
 
         # Compute force and stiffness
 
         # preallocate F
         F = np.zeros((3, number_of_nodes))
@@ -1443,38 +1514,48 @@
         if storage == 'sparse':
             # sparse storage
             M = scipy.sparse.diags(diag, format='csr')
         else:
             # dense storage
             M = np.diag(np.kron(M, np.ones((3,))))
 
-        # Check forces
-        sum_of_forces = np.linalg.norm(F, ord='fro')
-        if sum_of_forces > epsilon:
-            warnings.warn(f'Structure::stiffness: force balance not satisfied, '
-                          f'sum of forces = {sum_of_forces}')
-
         # Build stiffness object
         stiffness = Stiffness(K, M)
 
         # node constraints
         constraints = self.node_properties['constraint']
         has_constraints = constraints.isna().sum() < self.get_number_of_nodes()
         if has_constraints:
             # apply node constraints
             stiffness.apply_constraint(
                 *NodeConstraint.node_constraint(self.nodes, constraints))
         if apply_rigid_body_constraint:
             # apply rigid body constraints
             stiffness.apply_constraint(
-                *NodeConstraint.rigid_body_constraint(self.nodes), local=False)
+                *NodeConstraint.rigid_body_constraint(self.nodes),
+                local=False, verbose=False)
         if apply_planar_constraint:
             # apply planar constraints
             stiffness.apply_constraint(
-                *NodeConstraint.planar_constraint(self.nodes), local=False)
+                *NodeConstraint.planar_constraint(self.nodes),
+                local=False, verbose=False)
+
+        # Check forces
+        if force is not None:
+            f = F + force
+        else:
+            f = F
+        if stiffness.T is not None:
+            # project forces on allowed displacements
+            sum_of_forces = np.linalg.norm(stiffness.T.transpose() @ f.ravel(order='F'))
+        else:
+            sum_of_forces = np.linalg.norm(f, ord='fro')
+        if sum_of_forces > epsilon:
+            warnings.warn(f'Structure::stiffness: force balance not satisfied, '
+                          f'sum of forces = {sum_of_forces}')
 
         return stiffness, F, v
 
 
 # module methods
 def rotate(s: Structure, v: npt.NDArray) -> Structure:
     """
```

### Comparing `tnsgrt-0.5.2/src/tnsgrt/utils.py` & `tnsgrt-0.6/src/tnsgrt/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,17 +27,18 @@
     **Notes:**
 
     1. See :meth:`scipy.spatial.transform.Rotation.from_rotvec` for details
     """
     return scipy.spatial.transform.Rotation.from_rotvec(v).as_matrix()
 
 
-def orthogonalize(a: npt.NDArray, epsilon: float = 1e-8,
+def orthogonalize(a: Union[npt.NDArray, scipy.sparse.csr_matrix],
+                  epsilon: float = 1e-8,
                   mode: Literal['reduced', 'complete'] = 'reduced')\
-        -> Union[Tuple[int, npt.NDArray, npt.NDArray],Tuple[int, npt.NDArray]]:
+        -> Union[Tuple[int, npt.NDArray, npt.NDArray], Tuple[int, npt.NDArray]]:
     """
     Ortoghonalize the constraint
 
     .. math::
         A^T \\, x = 0
 
     :param a: the coefficient array :math:`A`
@@ -45,64 +46,67 @@
     :param mode: 'complete' or 'reduced'
     :return: tuple with rank, the orthogonalized coefficient array, and its null space
              if mode is 'complete'
 
     **Notes:**
 
         1. If ``mode = 'reduced'`` the constraint coefficient is normalized at the
-           constructor by calculating the *reduced* QR decomposition
+           constructor by calculating the *reduced* SVD decomposition
 
            .. math::
-               A = Q R, \\quad Q^T Q = I, \\quad R \\text{ is upper triangular}
+               A = V S U^T, \\quad V^T V = I, \\quad U^T U = I, \\quad
+               S \\text{ is diagonal}
 
            Assuming that :math:`A` is full rank, the equivalent orthogonal constraint
 
            .. math::
-               A^T x = R^T V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0
+               A^T x = U S V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0
 
-           is obtained in which the coefficient is the orthogonal matrix :math:`V = Q`
+           is obtained in which the coefficient is the orthogonal matrix :math:`V`
 
         2. If ``mode = 'complete'`` the constraint coefficient is normalized at the
-           constructor by calculating the *complete* QR decomposition
+           constructor by calculating the *complete* SVD decomposition
 
            .. math::
-               A = Q R, \\quad Q^T Q = Q Q^T = I, \\quad R \\text{ is upper triangular}
+               A = \\tilde{V} \\tilde{S} \\tilde{U}^T, \\quad
+               \\tilde{V}^T \\tilde{V} = \\tilde{V} \\tilde{V}^T = I, \\quad
+               \\tilde{U}^T \\tilde{U} = \\tilde{U} \\tilde{U}^T = I, \\quad
+               \\tilde{S} \\text{ is diagonal}
 
            Assuming that :math:`A` is full rank, partition
 
            .. math::
-               \\begin{bmatrix} V & T \\end{bmatrix} = Q =
-               \\begin{bmatrix} Q_1 & Q_2 \\end{bmatrix}, \\qquad R =
-               \\begin{bmatrix} R_1 \\\\ 0 \\end{bmatrix}, \\quad
-               R_1 \\text{ is upper triangular}
+               \\begin{bmatrix} V & T \\end{bmatrix} = \\tilde{V}, \\qquad
+               \\begin{bmatrix} U & Q \\end{bmatrix} = \\tilde{U}, \\qquad
+               \\tilde{S} = \\begin{bmatrix} S \\\\ 0 \\end{bmatrix}, \\quad
+               S \\text{ is diagonal}
 
            to obtain the equivalent orthogonal constraint and its solution
 
            .. math::
-               A^T x = R_1^T V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0,
-               \\qquad x = T y
+               A^T x = U S V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0,
+               \\qquad x = T \\, y
 
            The matrix :math:`T` is an orthogonal basis for the constraint null space
 
         3. The above factorizations are modified to take into account the numerical
            rank of :math:`A` when it is rank-deficient
     """
     assert a.shape[1] < a.shape[0], 'a must be tall'
-    # QR decomposition
-    if mode == 'complete':
-        q, r = np.linalg.qr(a, mode='complete')
-    else:
-        q, r = np.linalg.qr(a)
-    # check for rank
-    rank = np.count_nonzero(np.abs(np.diag(r)) > epsilon)
+
+    # SVD decomposition
+    u, s, vh = np.linalg.svd(a.toarray() if scipy.sparse.issparse(a) else a,
+                             full_matrices=(mode == 'complete'))
+
+    rank = np.count_nonzero(s > epsilon)
     # return tuple
     if mode == 'complete':
-        return rank, q[:, :rank], q[:, rank:]
+        return rank, u[:, :rank], u[:, rank:]
     else:
-        return rank, q[:, :rank]
+        return rank, u[:, :rank]
 
 
 def is_colinear(a: npt.NDArray, b: npt.NDArray, epsilon: float = 1e-8) -> bool:
     """
     Two vectors are colinear if their orthogonal projection is small
 
     :param a: first vector
```

### Comparing `tnsgrt-0.5.2/src/tnsgrt/plotter/vispy.py` & `tnsgrt-0.6/src/tnsgrt/plotter/vispy.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/tests/test_equilibrium.py` & `tnsgrt-0.6/tests/test_equilibrium.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 
 import numpy as np
+
+from tnsgrt.stiffness import NodeConstraint
 from tnsgrt.structure import Structure
 
 
 class TestStructure(unittest.TestCase):
 
     def test_equilibrium(self):
 
@@ -108,7 +110,61 @@
 
         # no external force, normalize not one
         lmbda = np.array([0., 1., -1/2.]) - 3/2*np.array([-2., -2., 1.])
         np.testing.assert_allclose(s.member_properties['lambda_'], lmbda, atol=1e-6)
         self.assertTrue(np.abs(np.mean(
             s.get_member_properties(
                 s.get_members_by_tag('bar'), 'lambda_')) + 2) < 1e-6)
+
+    def test_constraints(self):
+
+        # planar pole
+        nodes = np.array([[-1, 0, 0], [0, 0, 0], [0, 1, 0], [1, 0, 0]]).transpose()
+        members = np.array([[0, 2], [2, 3], [1, 2]]).transpose()
+        s = Structure(nodes, members, number_of_strings=2)
+
+        # no equilibrium possible
+        self.assertRaises(Exception, s.equilibrium)
+
+        # add constraints
+        s.set_node_properties([0, 1, 3], 'constraint', NodeConstraint())
+
+        # equilibrium with constraints
+        fr = s.equilibrium()
+        lambda_ = np.array([1/2, 1/2, -1])
+        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_)
+        fr_ = np.array([[-1/2, -1/2, 0], [0, 1, 0],
+                        [0, 0, 0], [1/2, -1/2, 0]]).transpose()
+        np.testing.assert_allclose(fr, fr_)
+
+        # planar inverted V
+        nodes = np.array([[-1, 0, 0], [0, 1, 0], [1, 0, 0]]).transpose()
+        members = np.array([[0, 2], [0, 1], [1, 2]]).transpose()
+        s = Structure(nodes, members, number_of_strings=1)
+
+        # no equilibrium possible
+        self.assertRaises(Exception, s.equilibrium)
+
+        # add constraints
+        s.set_node_properties([0, 2], 'constraint', NodeConstraint())
+
+        # equilibrium with constraints
+        fe = np.array([[0, 0, 0], [0, -1, 0], [0, 0, 0]]).transpose()
+        fr = s.equilibrium(fe)
+        lambda_ = np.array([0, -1/2, -1/2])
+        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_, atol=1e-6)
+        fr_ = np.array([[1/2, 1/2, 0], [0, 0, 0], [-1/2, 1/2, 0]]).transpose()
+        np.testing.assert_allclose(fr, fr_)
+
+        # add constraints
+        s.set_node_properties([0], 'constraint', NodeConstraint())
+        s.set_node_properties([2], 'constraint',
+                              NodeConstraint(constraint=np.array([[0, 1, 0],
+                                                                  [0, 0, 1]])))
+
+        # equilibrium with constraints
+        fr = s.equilibrium(fe)
+        lambda_ = np.array([1/4, -1/2, -1/2])
+        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_)
+        fr_ = np.array([[0, 1/2, 0], [0, 0, 0], [0, 1/2, 0]]).transpose()
+        np.testing.assert_allclose(fr, fr_, atol=1e-6)
+
```

### Comparing `tnsgrt-0.5.2/tests/test_michell.py` & `tnsgrt-0.6/tests/test_michell.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/tests/test_prism.py` & `tnsgrt-0.6/tests/test_prism.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/tests/test_structure.py` & `tnsgrt-0.6/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/LICENSE` & `tnsgrt-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/README.md` & `tnsgrt-0.6/README.md`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.5.2/pyproject.toml` & `tnsgrt-0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tnsgrt"
-version = "0.5.2"
+version = "0.6"
 authors = [
     { name = "Mauricio C. de Oliveira", email = "mcdeoliveira@duck.com" }
 ]
 description = "Python library with support for analysis and design of Tensegrity structures"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["Tensegrity", "structures", "trusses"]
```

### Comparing `tnsgrt-0.5.2/PKG-INFO` & `tnsgrt-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnsgrt
-Version: 0.5.2
+Version: 0.6
 Summary: Python library with support for analysis and design of Tensegrity structures
 Project-URL: Homepage, https://github.com/mcdeoliveira/tensegrity
 Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Mauricio de Oliveira
```

