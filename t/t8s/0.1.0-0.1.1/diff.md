# Comparing `tmp/t8s-0.1.0.tar.gz` & `tmp/t8s-0.1.1.tar.gz`

## Comparing `t8s-0.1.0.tar` & `t8s-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 t8s-0.1.0/main.py
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.0/test-all.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 t8s-0.1.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.0/src/t8s/__about__.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 t8s-0.1.0/src/t8s/__init__.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 t8s-0.1.0/src/t8s/ts.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 t8s-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 t8s-0.1.0/tests/test_build_from_file.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 t8s-0.1.0/tests/test_to_parquet.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 t8s-0.1.0/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 t8s-0.1.0/README.md
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 t8s-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 t8s-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 t8s-0.1.1/main.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.1/publish-to-pypi.md
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.1/test-all.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 t8s-0.1.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 t8s-0.1.1/docs/dp-strategy.md
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.1/docs/img/strategy-pattern.png
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.1/src/t8s/__about__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 t8s-0.1.1/src/t8s/__init__.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 t8s-0.1.1/src/t8s/log_config.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 t8s-0.1.1/src/t8s/ts.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 t8s-0.1.1/src/t8s/ts_builder.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 t8s-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 t8s-0.1.1/tests/test_build_from_file.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 t8s-0.1.1/tests/test_to_parquet.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 t8s-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 t8s-0.1.1/README.md
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 t8s-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 t8s-0.1.1/PKG-INFO
```

### Comparing `t8s-0.1.0/src/t8s/ts.py` & `t8s-0.1.1/src/t8s/ts.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.0/tests/test_to_parquet.py` & `t8s-0.1.1/tests/test_to_parquet.py`

 * *Files identical despite different names*

### Comparing `t8s-0.1.0/LICENSE.txt` & `t8s-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t8s-0.1.0/README.md` & `t8s-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.0/pyproject.toml` & `t8s-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `t8s-0.1.0/PKG-INFO` & `t8s-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t8s
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Documentation, https://github.com/unknown/t8s#readme
 Project-URL: Issues, https://github.com/unknown/t8s/issues
 Project-URL: Source, https://github.com/unknown/t8s
 Author-email: João Antonio Ferreira <joao.parana@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

