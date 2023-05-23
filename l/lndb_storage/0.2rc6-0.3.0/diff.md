# Comparing `tmp/lndb_storage-0.2rc6.tar.gz` & `tmp/lndb_storage-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.2rc6.tar", last modified: Mon Apr 24 16:54:33 2023, max compression
+gzip compressed data, was "lndb_storage-0.3.0.tar", last modified: Tue May 23 16:02:13 2023, max compression
```

## Comparing `lndb_storage-0.2rc6.tar` & `lndb_storage-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.2rc6/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc6/.gitignore
--rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.2rc6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc6/LICENSE
--rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc6/README.md
--rw-r--r--   0        0        0     2770 2023-04-24 16:54:08.774433 lndb_storage-0.2rc6/docs/changelog.md
--rw-r--r--   0        0        0     9684 2023-04-23 22:03:51.292643 lndb_storage-0.2rc6/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc6/docs/guide/index.md
--rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc6/docs/guide/iris.csv
--rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc6/docs/guide/iris.data
--rw-r--r--   0        0        0     4349 2023-04-23 22:03:51.292792 lndb_storage-0.2rc6/docs/guide/new_iris.csv
--rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.2rc6/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     4069 2023-04-24 16:53:24.501276 lndb_storage-0.2rc6/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.2rc6/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.2rc6/docs/index.md
--rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc6/docs/reference.md
--rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc6/lamin-project.yaml
--rw-r--r--   0        0        0      580 2023-04-24 16:53:45.180185 lndb_storage-0.2rc6/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.2rc6/lndb_storage/_file.py
--rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.2rc6/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc6/lndb_storage/_images.py
--rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc6/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc6/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc6/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.2rc6/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc6/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc6/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc6/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     4937 2023-04-24 16:53:24.501473 lndb_storage-0.2rc6/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      919 2023-04-24 16:53:24.501654 lndb_storage-0.2rc6/noxfile.py
--rw-r--r--   0        0        0     1086 2023-04-24 02:04:57.542525 lndb_storage-0.2rc6/pyproject.toml
--rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc6/tests/test_notebooks.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 lndb_storage-0.2rc6/PKG-INFO
+-rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.3.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.3.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.3.0/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.3.0/README.md
+-rw-r--r--   0        0        0     3250 2023-05-23 16:01:47.084797 lndb_storage-0.3.0/docs/changelog.md
+-rw-r--r--   0        0        0     9684 2023-04-23 22:03:51.292643 lndb_storage-0.3.0/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.3.0/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.3.0/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.3.0/docs/guide/iris.data
+-rw-r--r--   0        0        0     4349 2023-04-23 22:03:51.292792 lndb_storage-0.3.0/docs/guide/new_iris.csv
+-rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.3.0/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     4069 2023-04-24 16:53:24.501276 lndb_storage-0.3.0/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.3.0/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.3.0/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.3.0/lamin-project.yaml
+-rw-r--r--   0        0        0      579 2023-05-23 16:01:34.728417 lndb_storage-0.3.0/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.3.0/lndb_storage/_file.py
+-rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.3.0/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.3.0/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.3.0/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.3.0/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.3.0/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.3.0/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.3.0/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.3.0/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.3.0/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     4853 2023-05-23 14:42:49.806479 lndb_storage-0.3.0/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      919 2023-04-24 16:53:24.501654 lndb_storage-0.3.0/noxfile.py
+-rw-r--r--   0        0        0     1108 2023-05-23 14:40:16.493381 lndb_storage-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      484 2023-05-23 14:40:16.493813 lndb_storage-0.3.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 lndb_storage-0.3.0/PKG-INFO
```

### Comparing `lndb_storage-0.2rc6/.github/workflows/build.yml` & `lndb_storage-0.3.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/.github/workflows/latest-changes.yml` & `lndb_storage-0.3.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/.gitignore` & `lndb_storage-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/.pre-commit-config.yaml` & `lndb_storage-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/LICENSE` & `lndb_storage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/changelog.md` & `lndb_storage-0.3.0/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✅ Use nbproject-test directly in test_notebooks.py | [31](https://github.com/laminlabs/lndb-storage/pull/31) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 | 0.3.0
+♻️ Refactor CloudAnnData | [29](https://github.com/laminlabs/lndb-storage/pull/29) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
+🦺 Check that obs and var are dataframes in subset | [28](https://github.com/laminlabs/lndb-storage/pull/28) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 ✨ Add `CloudAnnData` | [26](https://github.com/laminlabs/lndb-storage/pull/26) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.2rc6
 📝 Drastically simplify streaming guide | [25](https://github.com/laminlabs/lndb-storage/pull/25) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 |
 ✅ Add additional tests for replace | [24](https://github.com/laminlabs/lndb-storage/pull/24) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 |
 ✅ Check add with key | [20](https://github.com/laminlabs/lndb-storage/pull/20) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 | 0.2rc5
 ♻️ Refactoring | [19](https://github.com/laminlabs/lndb-storage/pull/19) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 |
 ♻️ Remove call to nbproject in progress bar | [18](https://github.com/laminlabs/lndb-storage/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-04-14 | 0.2rc4
 ✅ Introduce separate upload guide | [14](https://github.com/laminlabs/lndb-storage/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 | 0.2rc3
```

### Comparing `lndb_storage-0.2rc6/docs/guide/add-replace-stage.ipynb` & `lndb_storage-0.3.0/docs/guide/add-replace-stage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/guide/iris.csv` & `lndb_storage-0.3.0/docs/guide/iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/guide/iris.data` & `lndb_storage-0.3.0/docs/guide/iris.data`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/guide/new_iris.csv` & `lndb_storage-0.3.0/docs/guide/new_iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/guide/serialize-cache.ipynb` & `lndb_storage-0.3.0/docs/guide/serialize-cache.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/guide/stream.ipynb` & `lndb_storage-0.3.0/docs/guide/stream.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/docs/guide/upload.ipynb` & `lndb_storage-0.3.0/docs/guide/upload.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/__init__.py` & `lndb_storage-0.3.0/lndb_storage/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :toctree: .
 
    store_object
    store_png
    delete_storage
 """
 
-__version__ = "0.2rc6"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.3.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 from lndb.dev.upath import UPath
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 
 from ._file import delete_storage, load_to_memory, store_object
 from ._h5ad import h5ad_to_anndata
 from ._images import store_png
```

### Comparing `lndb_storage-0.2rc6/lndb_storage/_file.py` & `lndb_storage-0.3.0/lndb_storage/_file.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/_subset.py` & `lndb_storage-0.3.0/lndb_storage/_subset.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/_zarr.py` & `lndb_storage-0.3.0/lndb_storage/_zarr.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/object/_anndata.py` & `lndb_storage-0.3.0/lndb_storage/object/_anndata.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/object/_anndata_sizes.py` & `lndb_storage-0.3.0/lndb_storage/object/_anndata_sizes.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/object/_core.py` & `lndb_storage-0.3.0/lndb_storage/object/_core.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/object/_lazy_field.py` & `lndb_storage-0.3.0/lndb_storage/object/_lazy_field.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.3.0/lndb_storage/object/_subset_anndata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 from functools import cached_property
-from typing import Literal, Optional, Union
+from typing import Optional, Union
 
 import h5py
 import pandas as pd
 import zarr
 from anndata import AnnData
 from anndata._io.specs.methods import _read_partial
 from anndata._io.specs.registry import read_elem, read_elem_partial
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 from lnschema_core import File
-from lnschema_core.dev._storage import filepath_from_file
+from lnschema_core._core import filepath_from_file_or_folder
 
 from ._lazy_field import LazySelector
 
 
 def _indices(base_indices, select_indices):
     if len(base_indices) == len(select_indices):
         return slice(None)
     else:
         return list(base_indices.get_indexer(select_indices))
 
 
+def _to_df(val):
+    if isinstance(val, pd.DataFrame):
+        return val
+    # is array
+    elif "index" in val.dtype.fields:
+        return pd.DataFrame.from_records(val, index="index")
+    else:
+        return pd.DataFrame.from_records(val)
+
+
 def _subset_adata_storage(
     storage: Union[zarr.Group, h5py.File],
     query_obs: Optional[Union[str, LazySelector]] = None,
     query_var: Optional[Union[str, LazySelector]] = None,
 ) -> Union[AnnData, None]:
     with storage as access:
-        obs = read_elem(access["obs"])
-        var = read_elem(access["var"])
+        obs = _to_df(read_elem(access["obs"]))
+        var = _to_df(read_elem(access["var"]))
 
         if query_obs is not None:
             if hasattr(query_obs, "evaluate"):
                 obs_result = obs[query_obs.evaluate(obj=obs)]  # type: ignore
             else:
                 obs_result = obs.query(query_obs)
         else:
@@ -79,15 +89,15 @@
 
 
 def _subset_anndata_file(
     file: File,
     query_obs: Optional[Union[str, LazySelector]] = None,
     query_var: Optional[Union[str, LazySelector]] = None,
 ) -> Union[AnnData, None]:
-    file_path = filepath_from_file(file)
+    file_path = filepath_from_file_or_folder(file)
     fs, file_path_str = _infer_filesystem(file_path)
 
     adata: Union[AnnData, None] = None
 
     if file.suffix == ".h5ad":
         with fs.open(file_path_str, mode="rb") as file:
             storage = h5py.File(file, mode="r")
@@ -96,45 +106,35 @@
         mapper = fs.get_mapper(file_path_str, check=True)
         storage = zarr.open(mapper, mode="r")
         adata = _subset_adata_storage(storage, query_obs, query_var)
 
     return adata
 
 
-def get_obs_var_storage(
-    storage: Union[zarr.Group, h5py.File], which=Literal["obs", "var"]
-) -> pd.DataFrame:
-    with storage as access:
-        result = read_elem(access[which])
-    if isinstance(result, pd.DataFrame):
-        return result
-    # is array
-    elif "index" in result.dtype.fields:
-        return pd.DataFrame.from_records(result, index="index")
-    else:
-        return pd.DataFrame.from_records(result)
-
-
 class CloudAnnData:
     def __init__(self, file: File):
-        self._file = file
-
-    def _get_obs_var(self, which=Literal["obs", "var"]) -> pd.DataFrame:
-        file_path = filepath_from_file(self._file)
-        fs, file_path_str = _infer_filesystem(file_path)
-        if self._file.suffix == ".h5ad":
-            with fs.open(file_path_str, mode="rb") as f:
-                storage = h5py.File(f, mode="r")
-                df = get_obs_var_storage(storage, which)
-        elif self._file.suffix == ".zarr" or self._file.suffix == ".zrad":
+        fs, file_path_str = _infer_filesystem(filepath_from_file_or_folder(file))
+        if file.suffix == ".h5ad":
+            self._conn = fs.open(file_path_str, mode="rb")
+            self.storage = h5py.File(self._conn, mode="r")
+        elif file.suffix in (".zarr", ".zrad"):
+            self._conn = None
             mapper = fs.get_mapper(file_path_str, check=True)
-            storage = zarr.open(mapper, mode="r")
-            df = get_obs_var_storage(storage, which)
-        return df
+            self.storage = zarr.open(mapper, mode="r")
+        else:
+            raise ValueError(
+                f"file should have .h5ad, .zarr or .zrad suffix, not {file.suffix}."
+            )
+
+    def __del__(self):
+        """Closes the connection."""
+        if self._conn is not None:
+            self.storage.close()
+            self._conn.close()
 
     @cached_property
     def obs(self) -> pd.DataFrame:
-        return self._get_obs_var(which="obs")
+        return _to_df(read_elem(self.storage["obs"]))
 
     @cached_property
     def var(self) -> pd.DataFrame:
-        return self._get_obs_var(which="var")
+        return _to_df(read_elem(self.storage["var"]))
```

### Comparing `lndb_storage-0.2rc6/noxfile.py` & `lndb_storage-0.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc6/pyproject.toml` & `lndb_storage-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ]
 test = [
     "pytest>=6.0",
     "pytest-cov",
     "scanpy",
     "pyarrow",
     "lndb>=0.41rc1",
+    "nbproject-test",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
```

### Comparing `lndb_storage-0.2rc6/PKG-INFO` & `lndb_storage-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.2rc6
+Version: 0.3.0
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
 Requires-Dist: lndb>=0.41.0
 Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
@@ -24,14 +24,15 @@
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: scanpy ; extra == "test"
 Requires-Dist: pyarrow ; extra == "test"
 Requires-Dist: lndb>=0.41rc1 ; extra == "test"
+Requires-Dist: nbproject-test ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb-storage
 Provides-Extra: dev
 Provides-Extra: test
 
 # lndb-storage: LaminDB storage
 
 Latest developer docs: [netlify](https://lndb-storage-soie.netlify.app/docs/lndb-storage/)
```

