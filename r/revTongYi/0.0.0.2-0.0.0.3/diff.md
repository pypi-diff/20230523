# Comparing `tmp/revtongyi-0.0.0.2.tar.gz` & `tmp/revtongyi-0.0.0.3.tar.gz`

## Comparing `revtongyi-0.0.0.2.tar` & `revtongyi-0.0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/test.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/revTongYi/__init__.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/LICENSE
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 revtongyi-0.0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/test.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/revTongYi/__init__.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/LICENSE
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 revtongyi-0.0.0.3/PKG-INFO
```

### Comparing `revtongyi-0.0.0.2/test.py` & `revtongyi-0.0.0.3/test.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.2/revTongYi/__init__.py` & `revtongyi-0.0.0.3/revTongYi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             "sec-ch-ua": '"Microsoft Edge";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": '"Windows"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.50",
-            "x-xsrf-token": "50f6b58b-4251-42e9-906d-97dc5d1eee61",
+            "x-xsrf-token": self.cookies['XSRF-TOKEN'],
             "cookie": self.cookies_str
         }
 
         data = {
             "firstQuery": firstQuery
         }
```

### Comparing `revtongyi-0.0.0.2/.gitignore` & `revtongyi-0.0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.2/LICENSE` & `revtongyi-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.2/README.md` & `revtongyi-0.0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `revtongyi-0.0.0.2/pyproject.toml` & `revtongyi-0.0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revTongYi"
-version = "0.0.0.2"
+version = "0.0.0.3"
 authors = [
   { name="xw5xr6", email="xw5xr6@hotmail.com" },
 ]
 description = "阿里通义千问逆向工程API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `revtongyi-0.0.0.2/PKG-INFO` & `revtongyi-0.0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revTongYi
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: 阿里通义千问逆向工程API
 Project-URL: Homepage, https://github.com/xw5xr6/revTongYi
 Project-URL: Bug Tracker, https://github.com/xw5xr6/revTongYi/issues
 Author-email: xw5xr6 <xw5xr6@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

