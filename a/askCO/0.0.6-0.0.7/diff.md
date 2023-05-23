# Comparing `tmp/askCO-0.0.6.tar.gz` & `tmp/askCO-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.6.tar", last modified: Tue May 23 04:35:07 2023, max compression
+gzip compressed data, was "askCO-0.0.7.tar", last modified: Tue May 23 04:41:32 2023, max compression
```

## Comparing `askCO-0.0.6.tar` & `askCO-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.189811 askCO-0.0.6/
--rw-rw-rw-   0        0        0     3994 2023-05-23 04:35:07.189811 askCO-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.6/README.md
--rw-rw-rw-   0        0        0      676 2023-05-23 04:34:15.000000 askCO-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 04:35:07.189811 askCO-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.158586 askCO-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.158586 askCO-0.0.6/src/askCO/
--rw-rw-rw-   0        0        0     9765 2023-05-23 03:56:27.000000 askCO-0.0.6/src/askCO/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-05-18 02:08:58.000000 askCO-0.0.6/src/askCO/tryCO.py
-drwxrwxrwx   0        0        0        0 2023-05-23 04:35:07.189811 askCO-0.0.6/src/askCO.egg-info/
--rw-rw-rw-   0        0        0     3994 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-23 04:35:07.000000 askCO-0.0.6/src/askCO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.099534 askCO-0.0.7/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 04:41:32.099534 askCO-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.7/README.md
+-rw-rw-rw-   0        0        0      676 2023-05-23 04:40:23.000000 askCO-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 04:41:32.099534 askCO-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.068288 askCO-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.068288 askCO-0.0.7/src/askCO/
+-rw-rw-rw-   0        0        0     9732 2023-05-23 04:37:53.000000 askCO-0.0.7/src/askCO/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-05-18 02:08:58.000000 askCO-0.0.7/src/askCO/tryCO.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:41:32.099534 askCO-0.0.7/src/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 04:41:32.000000 askCO-0.0.7/src/askCO.egg-info/top_level.txt
```

### Comparing `askCO-0.0.6/PKG-INFO` & `askCO-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.6/README.md` & `askCO-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.0.6/pyproject.toml` & `askCO-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "askCO"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
 	{name = "Lucy Schrader", email = "lucy@schrader.nz"},
 ]
 description = "Python interface for Te Papa's collections API"
 readme = "README.md"
 keywords = ["python", "museum", "api"]
 requires-python = ">=3.7"
```

### Comparing `askCO-0.0.6/src/askCO/__init__.py` & `askCO-0.0.7/src/askCO/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -293,17 +293,17 @@
 	def build_query(self):
 		self.request_url = "{b}/{e}/{i}".format(b=self.base_url, e=self.endpoint, i=self.irn)
 
 		# Build a search for related
 		if self.related == True:
 			self.request_url += "/related"
 			if self.size or self.types:
-        		self.request_url += "?"
-    		if self.size:
-		        self.request_url += "size={}".format(size)
-		    if self.size and self.types:
-		        self.request_url += "&"
-		    if self.types:
-		        self.request_url += "types={}".format(types)
+				self.request_url += "?"
+			if self.size:
+				self.request_url += "size={}".format(size)
+			if self.size and self.types:
+				self.request_url += "&"
+			if self.types:
+				self.request_url += "types={}".format(types)
 
 	def save_record(self):
 		self.response_text = json.loads(self.response.text)
```

### Comparing `askCO-0.0.6/src/askCO/tryCO.py` & `askCO-0.0.7/src/askCO/tryCO.py`

 * *Files identical despite different names*

### Comparing `askCO-0.0.6/src/askCO.egg-info/PKG-INFO` & `askCO-0.0.7/src/askCO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

