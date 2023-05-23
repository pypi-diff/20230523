# Comparing `tmp/succulent-0.1.1.tar.gz` & `tmp/succulent-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "succulent-0.1.1.tar", max compression
+gzip compressed data, was "succulent-0.1.2.tar", max compression
```

## Comparing `succulent-0.1.1.tar` & `succulent-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-05-21 15:50:22.668905 succulent-0.1.1/LICENSE
--rw-r--r--   0        0        0     2399 2023-05-21 15:50:22.668905 succulent-0.1.1/README.md
--rw-r--r--   0        0        0      669 2023-05-21 15:50:22.668905 succulent-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      107 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/__init__.py
--rw-r--r--   0        0        0     1367 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/api.py
--rw-r--r--   0        0        0      335 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/configuration.py
--rw-r--r--   0        0        0      102 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/configuration.yml
--rw-r--r--   0        0        0     1998 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/processing.py
--rw-r--r--   0        0        0     3108 2023-05-21 15:50:29.580088 succulent-0.1.1/setup.py
--rw-r--r--   0        0        0     3118 2023-05-21 15:50:29.580277 succulent-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-04-18 11:02:21.268343 succulent-0.1.2/LICENSE
+-rw-r--r--   0        0        0      708 2023-05-22 11:47:40.523766 succulent-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2629 2023-05-21 17:13:44.496804 succulent-0.1.2/README.md
+-rw-r--r--   0        0        0      113 2023-05-22 11:47:49.704491 succulent-0.1.2/succulent/__init__.py
+-rw-r--r--   0        0        0     1763 2023-05-22 07:54:07.348467 succulent-0.1.2/succulent/api.py
+-rw-r--r--   0        0        0      348 2023-05-21 12:41:59.963130 succulent-0.1.2/succulent/configuration.py
+-rw-r--r--   0        0        0      107 2023-05-21 12:48:12.736290 succulent-0.1.2/succulent/configuration.yml
+-rw-r--r--   0        0        0      140 2023-05-22 07:35:30.619588 succulent-0.1.2/succulent/main.py
+-rw-r--r--   0        0        0     2706 2023-05-22 07:54:17.873198 succulent-0.1.2/succulent/processing.py
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 succulent-0.1.2/PKG-INFO
```

### Comparing `succulent-0.1.1/LICENSE` & `succulent-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Iztok Fister Jr.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Iztok Fister Jr.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `succulent-0.1.1/README.md` & `succulent-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,22 @@
 
 ```python
 from succulent.api import SucculentAPI
 api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
 api.start()
 ```
 
+### Parameters
+| Parameter | Description | Options |
+| --- | --- | --- |
+| `host` | Host address | |
+| `port` | Port number | |
+| `config` | Path to configuration file | |
+| `format` | Output format | csv, json, sqlite |
+
 ## Configuration
 In the root directory, create a file named `configuration.yml` and define the following:
 ```yml
 data:
   - name: # Measure name
 ```
```

### Comparing `succulent-0.1.1/succulent/processing.py` & `succulent-0.1.2/succulent/processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,75 @@
-import os
-import pandas as pd
-
-class Processing:
-    def __init__(self, config, format):
-        self.format = format
-        self.columns = [configuration['name'] for configuration in config['data']]
-    
-    def parameters(self):
-        parameters = [f'{column}=' for column in self.columns]
-        parameters = '&'.join(parameters)
-        return parameters
-        
-    def process(self, req):
-        # Define paths
-        path = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), 'data', f'data.{self.format}'
-        )
-        output_path = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), 'data', f'data.{self.format}'
-        )
-
-        # Load existing data
-        if os.path.exists(path):
-            if self.format == 'csv':
-                df = pd.read_csv(path, sep=',')
-            elif self.format == 'json':
-                df = pd.read_json(path, orient='records')
-            else:
-                raise ValueError(f'Invalid file type: {self.format}')
-        # Initialise new data
-        else:
-            df = pd.DataFrame(columns=self.columns)
-
-        # Parse data from request
-        data = {}
-        if req.is_json:
-            for column in self.columns:
-                try:
-                    data[column] = req.json[column]
-                except:
-                    data[column] = None
-        else:
-            for column in self.columns:
-                try: 
-                    data[column] = req.args.get(column)
-                except:
-                    data[column] = None
-        data = pd.Series(data, index=self.columns)
-
-        # Merge data
-        df = pd.concat([df, data.to_frame().T], ignore_index=True)
-
-        # Store data to device
-        if self.format == 'csv':
-            df.to_csv(output_path, sep=',', index=False)
-        elif self.format == 'json':
-            df.to_json(output_path, orient='records', indent=4)
-        else:
+import os
+import sqlite3
+import pandas as pd
+
+class Processing:
+    def __init__(self, config, format):
+        self.format = format
+        self.columns = [configuration['name'] for configuration in config]
+        self.df = None  # Initialize df attribute
+    
+    def parameters(self):
+        parameters = [f'{column}=' for column in self.columns]
+        parameters = '&'.join(parameters)
+        return parameters
+        
+    def process(self, req):
+        # Directory preparation
+        directory = os.path.join(os.path.abspath(os.getcwd()), 'data')
+        if not os.path.exists(directory):
+            os.makedirs(directory)
+
+        # Define paths
+        path = os.path.join(
+            os.path.abspath(os.getcwd()), 'data', f'data.{self.format}'
+        )
+        output_path = os.path.join(
+            os.path.abspath(os.getcwd()), 'data', f'data.{self.format}'
+        )
+
+        # Load existing data
+        if os.path.exists(path):
+            if self.format == 'csv':
+                self.df = pd.read_csv(path, sep=',')
+            elif self.format == 'json':
+                self.df = pd.read_json(path, orient='records')
+            elif self.format == 'sqlite':
+                conn = sqlite3.connect(path)
+                self.df = pd.read_sql_query("SELECT * FROM data", conn)
+                conn.close()
+            else:
+                raise ValueError(f'Invalid file type: {self.format}')
+        # Initialise new data
+        else:
+            self.df = pd.DataFrame(columns=self.columns)
+
+        # Parse data from request
+        data = {}
+        if req.is_json:
+            for column in self.columns:
+                try:
+                    data[column] = req.json[column]
+                except:
+                    data[column] = None
+        else:
+            for column in self.columns:
+                try: 
+                    data[column] = str(req.args.get(column, default=''))
+                except:
+                    data[column] = ''
+        data = pd.Series(data, index=self.columns)
+
+        # Merge data
+        self.df = pd.concat([self.df, data.to_frame().T], ignore_index=True)
+
+        # Store data to device
+        if self.format == 'csv':
+            self.df.to_csv(output_path, sep=',', index=False)
+        elif self.format == 'json':
+            self.df.to_json(output_path, orient='records', indent=4)
+        elif self.format == 'sqlite':
+            conn = sqlite3.connect(output_path)
+            self.df.to_sql('data', conn, if_exists='replace', index=False)
+            conn.close()
+        else:
             raise ValueError(f'Invalid format: {self.format}')
```

### Comparing `succulent-0.1.1/setup.py` & `succulent-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,89 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: succulent
+Version: 0.1.2
+Summary: Collect POST requests easily
+Home-page: https://github.com/firefly-cpp/succulent
+License: MIT
+Keywords: data collection,data science,sensor measurements
+Author: Iztok Fister Jr.
+Author-email: iztok@iztok-jr-fister.eu
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/firefly-cpp/succulent
+Description-Content-Type: text/markdown
+
+---
+
+# succulent - Collect POST requests easily
+
+---
+![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
+[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)
+![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)
+[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)
+[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")
+
+## About
+
+succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in smart agriculture. The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations.
+
+## Detailed insights
+The current version includes (but is not limited to) the following functions:
+
+- Request URL generation for data collection
+- Data collection from POST requests
+
+## Installation
+
+### pip
+
+Install succulent with pip:
+
+```sh
+pip install succulent
+```
+
+## Usage
+
+### Example
+
+```python
+from succulent.api import SucculentAPI
+api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
+api.start()
+```
+
+### Parameters
+| Parameter | Description | Options |
+| --- | --- | --- |
+| `host` | Host address | |
+| `port` | Port number | |
+| `config` | Path to configuration file | |
+| `format` | Output format | csv, json, sqlite |
+
+## Configuration
+In the root directory, create a file named `configuration.yml` and define the following:
+```yml
+data:
+  - name: # Measure name
+```
 
-packages = \
-['succulent']
+## License
 
-package_data = \
-{'': ['*']}
+This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
 
-install_requires = \
-['flask>=2.3.2,<3.0.0', 'pandas>=2.0.1,<3.0.0', 'pyyaml>=6.0,<7.0']
-
-setup_kwargs = {
-    'name': 'succulent',
-    'version': '0.1.1',
-    'description': 'Collect POST requests easily',
-    'long_description': '---\n\n# succulent - Collect POST requests easily\n\n---\n![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)\n[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)\n![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)\n[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")\n[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")\n\n## About\n\nsucculent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in smart agriculture. The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations.\n\n## Detailed insights\nThe current version includes (but is not limited to) the following functions:\n\n- Request URL generation for data collection\n- Data collection from POST requests\n\n## Installation\n\n### pip\n\nInstall succulent with pip:\n\n```sh\npip install succulent\n```\n\n## Usage\n\n### Example\n\n```python\nfrom succulent.api import SucculentAPI\napi = SucculentAPI(host=\'0.0.0.0\', port=8080, config=\'configuration.yml\', format=\'csv\')\napi.start()\n```\n\n## Configuration\nIn the root directory, create a file named `configuration.yml` and define the following:\n```yml\ndata:\n  - name: # Measure name\n```\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
-    'author': 'Iztok Fister Jr.',
-    'author_email': 'iztok@iztok-jr-fister.eu',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/firefly-cpp/succulent',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## Disclaimer
 
+This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
 
-setup(**setup_kwargs)
```

