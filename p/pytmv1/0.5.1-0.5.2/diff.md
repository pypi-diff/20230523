# Comparing `tmp/pytmv1-0.5.1.tar.gz` & `tmp/pytmv1-0.5.2.tar.gz`

## Comparing `pytmv1-0.5.1.tar` & `pytmv1-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.1/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.1/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10964 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.1/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.1/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.1/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.2/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.2/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10964 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3203 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.2/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.2/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.2/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.2/PKG-INFO
```

### Comparing `pytmv1-0.5.1/src/pytmv1/__init__.py` & `pytmv1-0.5.2/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/caller.py` & `pytmv1-0.5.2/src/pytmv1/caller.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/core.py` & `pytmv1-0.5.2/src/pytmv1/core.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/exceptions.py` & `pytmv1-0.5.2/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/mapper.py` & `pytmv1-0.5.2/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/results.py` & `pytmv1-0.5.2/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/utils.py` & `pytmv1-0.5.2/src/pytmv1/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 
 
 def endpoint_query(op: QueryOp, *values: str) -> Dict[str, str]:
     return {
         "TMV1-Query": op.join(
             "("
             + QueryOp.OR.join(
-                f"{qt.value}:'{value}'" for qt in endpoint_query_field(value)
+                f"{qt.value} eq '{value}'"
+                for qt in endpoint_query_field(value)
             )
             + ")"
             for value in values
         )
     }
```

### Comparing `pytmv1-0.5.1/src/pytmv1/model/commons.py` & `pytmv1-0.5.2/src/pytmv1/model/commons.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/model/enums.py` & `pytmv1-0.5.2/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/model/requests.py` & `pytmv1-0.5.2/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/src/pytmv1/model/responses.py` & `pytmv1-0.5.2/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/LICENSE.txt` & `pytmv1-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/README.md` & `pytmv1-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/pyproject.toml` & `pytmv1-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.1/PKG-INFO` & `pytmv1-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

