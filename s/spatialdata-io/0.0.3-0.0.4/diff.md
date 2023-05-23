# Comparing `tmp/spatialdata_io-0.0.3.tar.gz` & `tmp/spatialdata_io-0.0.4.tar.gz`

## Comparing `spatialdata_io-0.0.3.tar` & `spatialdata_io-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.codecov.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.mypy.ini
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/_version.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/Makefile
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/changelog.md
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/conf.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/contributing.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/references.md
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/template_usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/extensions/.gitkeep
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_constants/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_constants/_constants.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_constants/_enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/__init__.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/cosmx.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/mcmicro.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/metaspace.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/resolve.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/steinbock.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/visium.py
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/xenium.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/__init__.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_read_10x_h5.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/tests/test_basic.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/LICENSE
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.codecov.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.mypy.ini
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/_version.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/changelog.md
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/references.md
+-rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/template_usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/extensions/.gitkeep
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_constants/__init__.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_constants/_constants.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_constants/_enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/__init__.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/cosmx.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/curio.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/mcmicro.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/metaspace.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/resolve.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/steinbock.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/visium.py
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/xenium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/__init__.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_read_10x_h5.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/tests/test_basic.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/PKG-INFO
```

### Comparing `spatialdata_io-0.0.3/.flake8` & `spatialdata_io-0.0.4/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/.mypy.ini` & `spatialdata_io-0.0.4/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/.pre-commit-config.yaml` & `spatialdata_io-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/.github/workflows/build.yaml` & `spatialdata_io-0.0.4/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/.github/workflows/test_and_deploy.yaml` & `spatialdata_io-0.0.4/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/Makefile` & `spatialdata_io-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/conf.py` & `spatialdata_io-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/contributing.md` & `spatialdata_io-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/make.bat` & `spatialdata_io-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/references.bib` & `spatialdata_io-0.0.4/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/template_usage.md` & `spatialdata_io-0.0.4/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/_templates/autosummary/class.rst` & `spatialdata_io-0.0.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/docs/extensions/typed_returns.py` & `spatialdata_io-0.0.4/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/_docs.py` & `spatialdata_io-0.0.4/src/spatialdata_io/_docs.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/_constants/_constants.py` & `spatialdata_io-0.0.4/src/spatialdata_io/_constants/_constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 from enum import unique
 
 from spatialdata_io._constants._enum import ModeEnum
 
 
 @unique
+class CurioKeys(ModeEnum):
+    """Keys for *Curio* formatted dataset."""
+
+    # files and directories
+    ANNDATA_FILE = ".h5ad"
+    CLUSTER_ASSIGNMENT = "cluster_assignment.txt"
+    METRICS_FILE = "Metrics.csv"
+    VAR_FEATURES_CLUSTERS = "variable_features_clusters.txt"
+    VAR_FEATURES_MORANSI = "variable_features_moransi.txt"
+    # metadata
+    CATEGORY = "Category"
+    TOP_CLUSTER_DEFINING_FEATURES = "Top_cluster_defining_features"
+
+
+@unique
 class CosmxKeys(ModeEnum):
     """Keys for *Nanostring Cosmx* formatted dataset."""
 
     # files and directories
     COUNTS_SUFFIX = "exprMat_file.csv"
     TRANSCRIPTS_SUFFIX = "tx_file.csv"
     METADATA_SUFFIX = "metadata_file.csv"
```

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/_constants/_enum.py` & `spatialdata_io-0.0.4/src/spatialdata_io/_constants/_enum.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/cosmx.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/cosmx.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/mcmicro.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/mcmicro.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/steinbock.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/steinbock.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/visium.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/visium.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/xenium.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/xenium.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_read_10x_h5.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_read_10x_h5.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_utils.py` & `spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/LICENSE` & `spatialdata_io-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/README.md` & `spatialdata_io-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/pyproject.toml` & `spatialdata_io-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.3/PKG-INFO` & `spatialdata_io-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata-io
-Version: 0.0.3
+Version: 0.0.4
 Summary: SpatialData IO for common techs
 Project-URL: Documentation, https://spatialdata-io.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-io
 Project-URL: Home-page, https://github.com/scverse/spatialdata-io
 Author: scverse
 Maintainer-email: scverse <scverse@scverse.scverse>
 License: BSD 3-Clause License
```

