# Comparing `tmp/hyper_requests-0.0.7.tar.gz` & `tmp/hyper_requests-0.0.8.tar.gz`

## Comparing `hyper_requests-0.0.7.tar` & `hyper_requests-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/MANIFEST.in
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/setup.cfg
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/hyper_requests/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/hyper_requests/request_builder.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/hyper_requests/threader.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/performance/test_performance.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/unit/test_check_request_params.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/unit/test_threader.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/unit/test_threader_setup.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/LICENSE
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/MANIFEST.in
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/setup.cfg
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/hyper_requests/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/hyper_requests/request_builder.py
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/hyper_requests/threader.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/test/performance/test_performance.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/test/unit/test_check_request_params.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/test/unit/test_threader.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/test/unit/test_threader_setup.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 hyper_requests-0.0.8/PKG-INFO
```

### Comparing `hyper_requests-0.0.7/.pre-commit-config.yaml` & `hyper_requests-0.0.8/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
   rev: v2.31.1
   hooks:
     - id: pyupgrade
       args: [--py37-plus]
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
-    - id: flake8
+    - id: flake8
```

### Comparing `hyper_requests-0.0.7/.github/workflows/python-package-conda.yml` & `hyper_requests-0.0.8/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/hyper_requests/request_builder.py` & `hyper_requests-0.0.8/hyper_requests/request_builder.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/hyper_requests/threader.py` & `hyper_requests-0.0.8/hyper_requests/threader.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import requests
 
 from hyper_requests.request_builder import check_request_params
 
 nest_asyncio.apply()
 
 
-def get(request_params: list[dict[str, Any]], workers: int = 10) -> list[dict[str, Any]]:
+def get(
+    request_params: list[dict[str, Any]], workers: int = 10
+) -> list[dict[str, Any]]:
     """
     Fetches data from multiple URLs asynchronously using multithreading.
 
     :param request_params: List of dictionaries containing URL and parameter information.
     :param workers: Number of concurrent workers to use for multithreading. Default is 10.
     :return: List of JSON data returned by the APIs.
     """
@@ -52,14 +54,28 @@
 
         :param request_params: List of dictionaries containing URL and parameter information.
         :param workers: Number of concurrent workers to use for multithreading. Default is 10.
         """
         self.request_params = check_request_params(request_params)
         self.workers = workers
 
+    def __enter__(self):
+        """Enter the context."""
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        """
+        Exit the context.
+
+        :param exc_type: Exception type (if an exception occurred) or None (if no exception occurred).
+        :param exc_val: Exception value (instance of the exception that was raised) or None.
+        :param exc_tb: Exception traceback object (contains information about the stack frames) or None.
+        """
+        pass
+
     @staticmethod
     def _fetch(session, dict_in: dict[str, str]) -> dict[str, Any]:
         """
         Private method that runs the request to the API and returns the JSON data.
 
         :param session: The requests session object.
         :param dict_in: Dictionary containing the request parameters (URL, headers, etc.).
```

### Comparing `hyper_requests-0.0.7/test/performance/test_performance.py` & `hyper_requests-0.0.8/test/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/test/unit/test_check_request_params.py` & `hyper_requests-0.0.8/test/unit/test_check_request_params.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/test/unit/test_threader.py` & `hyper_requests-0.0.8/test/unit/test_threader.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/test/unit/test_threader_setup.py` & `hyper_requests-0.0.8/test/unit/test_threader_setup.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/.gitignore` & `hyper_requests-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/LICENSE` & `hyper_requests-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.7/README.md` & `hyper_requests-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 for response in returned_data:
     print(response)
 ```
 This example demonstrates the usage of hyper-requests to perform asynchronous HTTP requests.
 
 First, make sure you have installed hyper-requests by running the command pip install hyper-requests.
 
-Next, import the AsyncRequests class from the hyper_requests.threader module.
+Next, import hyper_requests nad utilise the .get() function.
 
 Create a list of request parameters using dictionaries, where each dictionary represents a set of parameters for an individual request. In this example, each request MUST have a URL specified with the 'url' key, all other paramters must match the classic request template.
 
 Create an instance of AsyncRequests with the request_params argument set to your list of request parameters. Specify the number of concurrent worker threads to use with the workers argument (in this case, workers=10).
 
 Execute the requests using the run_threads() method, which returns the data obtained from the requests.
```

### Comparing `hyper_requests-0.0.7/PKG-INFO` & `hyper_requests-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-requests
-Version: 0.0.7
+Version: 0.0.8
 Summary: Concurrent request HTTP execution library
 Project-URL: Homepage, https://github.com/edjones84/hyper-requests
 Project-URL: Bug Tracker, https://github.com/edjones84/hyper-requests/issues
 Author-email: Ed Jones <ejones84@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 for response in returned_data:
     print(response)
 ```
 This example demonstrates the usage of hyper-requests to perform asynchronous HTTP requests.
 
 First, make sure you have installed hyper-requests by running the command pip install hyper-requests.
 
-Next, import the AsyncRequests class from the hyper_requests.threader module.
+Next, import hyper_requests nad utilise the .get() function.
 
 Create a list of request parameters using dictionaries, where each dictionary represents a set of parameters for an individual request. In this example, each request MUST have a URL specified with the 'url' key, all other paramters must match the classic request template.
 
 Create an instance of AsyncRequests with the request_params argument set to your list of request parameters. Specify the number of concurrent worker threads to use with the workers argument (in this case, workers=10).
 
 Execute the requests using the run_threads() method, which returns the data obtained from the requests.
```

