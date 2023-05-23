# Comparing `tmp/range_compression-0.1.1.tar.gz` & `tmp/range_compression-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "range_compression-0.1.1.tar", max compression
+gzip compressed data, was "range_compression-0.2.0.tar", max compression
```

## Comparing `range_compression-0.1.1.tar` & `range_compression-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.1.1/README.md
--rw-r--r--   0        0        0      516 2023-05-19 02:30:47.432855 range_compression-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-05-19 02:26:56.109857 range_compression-0.1.1/range_compression/__init__.py
--rw-r--r--   0        0        0     6565 2023-05-19 02:07:33.880367 range_compression-0.1.1/range_compression/range_compression.py
--rw-r--r--   0        0        0     1150 1970-01-01 00:00:00.000000 range_compression-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.0/README.md
+-rw-r--r--   0        0        0      622 2023-05-23 09:46:46.677631 range_compression-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-05-19 02:26:56.109857 range_compression-0.2.0/range_compression/__init__.py
+-rw-r--r--   0        0        0     6868 2023-05-23 09:05:15.106083 range_compression-0.2.0/range_compression/range_compression.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.0/PKG-INFO
```

### Comparing `range_compression-0.1.1/pyproject.toml` & `range_compression-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "range-compression"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["myuan <zhengmy@ion.ac.cn>"]
 license = "LGPL"
 readme = "README.md"
 packages = [{include = "range_compression"}]
 repository = "https://github.com/myuanz/matrix-range-compression"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<=3.11"
+python = ">=3.8,<3.12"
 numba = "^0.57.0"
-numpy = "^1.24.3"
-polars = "^0.17.14"
+numpy = "^1.24"
+polars = "^0.17"
+importlib-metadata = { version = "^6.6.0", python = "^3.8" }
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
+opencv-python-headless = "^4.7.0.72"
+tox = "^4.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `range_compression-0.1.1/range_compression/range_compression.py` & `range_compression-0.2.0/range_compression/range_compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 from dataclasses import dataclass
 from datetime import datetime
+from os import PathLike
 from pathlib import Path
+from typing import Union, Optional
 
 import numba as nb
 import numpy as np
 import polars as pl
 
 
 @dataclass
@@ -16,37 +18,41 @@
     encodings: np.ndarray
     '表达区间用，shape: (n, 4)，[(start_x, end_x, value, row_index), ...]'
 
     row_indexes: np.ndarray
     '快速从 y 查找编码行，shape: (n, 2)，[(start_y, encoding_count), ...]'
 
 
-    def save(self, base_dir: Path):
+    def save(self, base_dir: Union[str, PathLike], compression='gzip'):
+        base_dir = Path(base_dir)
+
         base_dir.mkdir(exist_ok=True)
         dfe = pl.from_numpy(self.encodings, schema=['start', 'end', 'v', 'row_index'])
-        dfe.write_parquet(base_dir / f'encodings.parquet')
+        dfe.write_parquet(base_dir / f'encodings.parquet', compression=compression)
 
         dfer = pl.from_numpy(self.row_indexes, schema=['row_start_index', 'row_count'])
-        dfer.write_parquet(base_dir / f'row_indexes.parquet')
+        dfer.write_parquet(base_dir / f'row_indexes.parquet', compression=compression)
 
         (base_dir / 'meta.json').write_text(json.dumps({
             'w': self.w,
             'h': self.h,
             'datetime': datetime.now(),
-        }))
+        }, default=str))
 
     @staticmethod
-    def load(base_dir: Path, chip: str | None = None, no_row_index=True):
+    def load(base_dir: Union[str, PathLike], chip: Optional[str] = None, no_row_index=True):
         '''从文件夹中导入
 
         base_dir: 文件夹路径
         chip: 如果有 chip，那么会在 base_dir/chip 中寻找文件
         no_row_index: 原始 encodings 是四列的，最后一列是 row_index，
                       如果不需要 row_index，可以设置为 True，可以把更多数据放到缓存里
         '''
+        base_dir = Path(base_dir)
+
         if chip is not None:
             base_dir = base_dir / chip
 
         dfe = pl.read_parquet(base_dir / f'encodings.parquet')
         encodings = dfe.to_numpy()[:, :3]
         if no_row_index:
             encodings = np.ascontiguousarray(encodings[:, :3])
@@ -58,22 +64,23 @@
             w=meta['w'],
             h=meta['h'],
             encodings=encodings,
             row_indexes=row_indexes,
         )
 
     @staticmethod
-    def targets(base_dir: Path | None = None, chip: str | None = None):
+    def targets(base_dir: Union[str, PathLike, None] = None, chip: Optional[str] = None):
         base = [
             'encodings.parquet',
             'row_indexes.parquet',
             'meta.json',
         ]
 
         if base_dir is not None:
+            base_dir = Path(base_dir)
             if chip is not None:
                 base_dir = base_dir / chip
             base = [base_dir / x for x in base]
 
         return base
 
     def find_index(
```

### Comparing `range_compression-0.1.1/PKG-INFO` & `range_compression-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: range-compression
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/myuanz/matrix-range-compression
 License: LGPL
 Author: myuan
 Author-email: zhengmy@ion.ac.cn
-Requires-Python: >=3.10,<=3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: numba (>=0.57.0,<0.58.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: polars (>=0.17.14,<0.18.0)
+Requires-Dist: numpy (>=1.24,<2.0)
+Requires-Dist: polars (>=0.17,<0.18)
 Project-URL: Repository, https://github.com/myuanz/matrix-range-compression
 Description-Content-Type: text/markdown
 
 # 矩阵区间压缩
 
 ## Quick start
```

