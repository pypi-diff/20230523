# Comparing `tmp/pytmv1-0.5.2.tar.gz` & `tmp/pytmv1-0.5.3.tar.gz`

## Comparing `pytmv1-0.5.2.tar` & `pytmv1-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.2/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.2/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10964 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3203 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.2/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.2/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.2/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.2/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.2/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.3/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.3/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10938 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3203 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.3/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.3/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.3/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.3/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.3/PKG-INFO
```

### Comparing `pytmv1-0.5.2/src/pytmv1/__init__.py` & `pytmv1-0.5.3/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/caller.py` & `pytmv1-0.5.3/src/pytmv1/caller.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/core.py` & `pytmv1-0.5.3/src/pytmv1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,15 @@
             total_count += 1
         if response.next_link:
             sr: SplitResult = urlsplit(response.next_link)
             log.info("Found nextLink")
             return self._consume_linkable(
                 lambda: self._process(
                     type(response),
-                    sr.path[5:],
-                    params={"skipToken": sr.query.split("=")[-1]},
+                    sr.path[5:] + f"?skipToken={sr.query.split('=')[-1]}",
                 ),
                 consumer,
                 total_count,
             )
         log.info(
             "Records consumed: [Total=%s, Type=%s]",
             total_count,
```

### Comparing `pytmv1-0.5.2/src/pytmv1/exceptions.py` & `pytmv1-0.5.3/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/mapper.py` & `pytmv1-0.5.3/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/results.py` & `pytmv1-0.5.3/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/utils.py` & `pytmv1-0.5.3/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/model/commons.py` & `pytmv1-0.5.3/src/pytmv1/model/commons.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/model/enums.py` & `pytmv1-0.5.3/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/model/requests.py` & `pytmv1-0.5.3/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/src/pytmv1/model/responses.py` & `pytmv1-0.5.3/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/LICENSE.txt` & `pytmv1-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/README.md` & `pytmv1-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/pyproject.toml` & `pytmv1-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.2/PKG-INFO` & `pytmv1-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

