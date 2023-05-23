# Comparing `tmp/otools-rpc-0.2.5.tar.gz` & `tmp/otools-rpc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.2.5.tar", last modified: Mon May 22 13:48:11 2023, max compression
+gzip compressed data, was "otools-rpc-0.2.6.tar", last modified: Tue May 23 14:39:33 2023, max compression
```

## Comparing `otools-rpc-0.2.5.tar` & `otools-rpc-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/LICENSE.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2841 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2348 2023-05-22 13:47:55.000000 otools-rpc-0.2.5/README.md
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/otools_rpc/
--rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/__init__.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/otools_rpc/external_api/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/external_api/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)      959 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/external_api/common.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     4812 2023-05-22 13:47:55.000000 otools-rpc-0.2.5/otools_rpc/external_api/environment.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     6037 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/external_api/recordset.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/otools_rpc.egg-info/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     2841 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/PKG-INFO
--rw-r--r--   0 opennet   (1000) opennet   (1000)      368 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       46 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/requires.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/top_level.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/setup.cfg
--rw-r--r--   0 opennet   (1000) opennet   (1000)      828 2023-05-22 13:47:55.000000 otools-rpc-0.2.5/setup.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 13:36:09.000000 otools-rpc-0.2.6/LICENSE.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     3458 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     2837 2023-05-23 14:35:04.000000 otools-rpc-0.2.6/README.md
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/otools_rpc/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.2.6/otools_rpc/__init__.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/otools_rpc/db_manager/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-23 14:35:04.000000 otools-rpc-0.2.6/otools_rpc/db_manager/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1115 2023-05-23 14:35:04.000000 otools-rpc-0.2.6/otools_rpc/db_manager/database_utils.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/otools_rpc/external_api/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 13:36:09.000000 otools-rpc-0.2.6/otools_rpc/external_api/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      959 2023-05-22 13:36:09.000000 otools-rpc-0.2.6/otools_rpc/external_api/common.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     4812 2023-05-22 13:47:55.000000 otools-rpc-0.2.6/otools_rpc/external_api/environment.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     6037 2023-05-22 13:36:09.000000 otools-rpc-0.2.6/otools_rpc/external_api/recordset.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/otools_rpc.egg-info/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     3458 2023-05-23 14:39:33.000000 otools-rpc-0.2.6/otools_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      442 2023-05-23 14:39:33.000000 otools-rpc-0.2.6/otools_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-05-23 14:39:33.000000 otools-rpc-0.2.6/otools_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-05-23 14:39:33.000000 otools-rpc-0.2.6/otools_rpc.egg-info/requires.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-05-23 14:39:33.000000 otools-rpc-0.2.6/otools_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-23 14:39:33.936354 otools-rpc-0.2.6/setup.cfg
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1045 2023-05-23 14:35:04.000000 otools-rpc-0.2.6/setup.py
```

### Comparing `otools-rpc-0.2.5/LICENSE.txt` & `otools-rpc-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.5/PKG-INFO` & `otools-rpc-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.2.5
+Version: 0.2.6
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.5-blue.svg)](https://pypi.org/project/otools-rpc/)
-[![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/pypi/v/otools-rpc?color=blue&label=version)](https://pypi.org/project/otools-rpc/)
+[![Status](https://img.shields.io/pypi/status/otools-rpc?color=orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
 
@@ -39,22 +42,26 @@
 ```console
 $ pip install otools-rpc
 ```
 
 See on pypi: https://pypi.org/project/otools-rpc/
 
 ## Usage
+
+### Environment
 Here are some examples of how to use otools-rpc to interact with the Odoo ERP system via the external API:
 
 ```python
 from otools_rpc.external_api import Environment
 
+
 url = "http://localhost:8069/"
 username = "admin"
 password = "admin"
+master_password = "adminadmin"
 
 # Create an instance of the environment
 env = Environment(url, username, password, db='my_odoo')
 env = env.with_context(lang='en_US')
 print(env)
 
 # Example: Create an invoice for a specific partner
@@ -77,10 +84,30 @@
     ],
 }
 invoice_id = env['account.move'].create(invoice_vals)
 print("Created invoice:", invoice_id)
 
 # Posting the invoice
 invoice_id.action_post()
+
+```
+
+### DBManager
+```python
+from otools_rpc.db_manager import DBManager
+
+url = "http://localhost:8069/"
+master_password = "adminadmin"
+
+dbmanager = DBManager(url, master_password)
+
+#Return list of all the available DB in your Odoo ENV
+dbmanager.dbobject.list()
+
+#Duplicating my_odoo to my_new_odoo
+db.manager.duplicate(db='my_odoo', new_name="my_new_odoo")
+
+#Deleting my_new_odoo
+db.manager.drop(db='my_new_odoo')
 ```
 
 More details are coming soon...
```

### Comparing `otools-rpc-0.2.5/README.md` & `otools-rpc-0.2.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.5-blue.svg)](https://pypi.org/project/otools-rpc/)
-[![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/pypi/v/otools-rpc?color=blue&label=version)](https://pypi.org/project/otools-rpc/)
+[![Status](https://img.shields.io/pypi/status/otools-rpc?color=orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
 
@@ -23,22 +23,26 @@
 ```console
 $ pip install otools-rpc
 ```
 
 See on pypi: https://pypi.org/project/otools-rpc/
 
 ## Usage
+
+### Environment
 Here are some examples of how to use otools-rpc to interact with the Odoo ERP system via the external API:
 
 ```python
 from otools_rpc.external_api import Environment
 
+
 url = "http://localhost:8069/"
 username = "admin"
 password = "admin"
+master_password = "adminadmin"
 
 # Create an instance of the environment
 env = Environment(url, username, password, db='my_odoo')
 env = env.with_context(lang='en_US')
 print(env)
 
 # Example: Create an invoice for a specific partner
@@ -61,10 +65,30 @@
     ],
 }
 invoice_id = env['account.move'].create(invoice_vals)
 print("Created invoice:", invoice_id)
 
 # Posting the invoice
 invoice_id.action_post()
+
+```
+
+### DBManager
+```python
+from otools_rpc.db_manager import DBManager
+
+url = "http://localhost:8069/"
+master_password = "adminadmin"
+
+dbmanager = DBManager(url, master_password)
+
+#Return list of all the available DB in your Odoo ENV
+dbmanager.dbobject.list()
+
+#Duplicating my_odoo to my_new_odoo
+db.manager.duplicate(db='my_odoo', new_name="my_new_odoo")
+
+#Deleting my_new_odoo
+db.manager.drop(db='my_new_odoo')
 ```
 
 More details are coming soon...
```

### Comparing `otools-rpc-0.2.5/otools_rpc/external_api/common.py` & `otools-rpc-0.2.6/otools_rpc/external_api/common.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.5/otools_rpc/external_api/environment.py` & `otools-rpc-0.2.6/otools_rpc/external_api/environment.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.5/otools_rpc/external_api/recordset.py` & `otools-rpc-0.2.6/otools_rpc/external_api/recordset.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.5/otools_rpc.egg-info/PKG-INFO` & `otools-rpc-0.2.6/otools_rpc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.2.5
+Version: 0.2.6
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.5-blue.svg)](https://pypi.org/project/otools-rpc/)
-[![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/pypi/v/otools-rpc?color=blue&label=version)](https://pypi.org/project/otools-rpc/)
+[![Status](https://img.shields.io/pypi/status/otools-rpc?color=orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
 
@@ -39,22 +42,26 @@
 ```console
 $ pip install otools-rpc
 ```
 
 See on pypi: https://pypi.org/project/otools-rpc/
 
 ## Usage
+
+### Environment
 Here are some examples of how to use otools-rpc to interact with the Odoo ERP system via the external API:
 
 ```python
 from otools_rpc.external_api import Environment
 
+
 url = "http://localhost:8069/"
 username = "admin"
 password = "admin"
+master_password = "adminadmin"
 
 # Create an instance of the environment
 env = Environment(url, username, password, db='my_odoo')
 env = env.with_context(lang='en_US')
 print(env)
 
 # Example: Create an invoice for a specific partner
@@ -77,10 +84,30 @@
     ],
 }
 invoice_id = env['account.move'].create(invoice_vals)
 print("Created invoice:", invoice_id)
 
 # Posting the invoice
 invoice_id.action_post()
+
+```
+
+### DBManager
+```python
+from otools_rpc.db_manager import DBManager
+
+url = "http://localhost:8069/"
+master_password = "adminadmin"
+
+dbmanager = DBManager(url, master_password)
+
+#Return list of all the available DB in your Odoo ENV
+dbmanager.dbobject.list()
+
+#Duplicating my_odoo to my_new_odoo
+db.manager.duplicate(db='my_odoo', new_name="my_new_odoo")
+
+#Deleting my_new_odoo
+db.manager.drop(db='my_new_odoo')
 ```
 
 More details are coming soon...
```

### Comparing `otools-rpc-0.2.5/setup.py` & `otools-rpc-0.2.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="otools-rpc",
-    version="0.2.5",
+    version="0.2.6",
     description="A tool to interact with Odoo's external API.",
     packages=find_packages(exclude=["tests"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrFaBemol/otools-rpc",
     author="Gautier Casabona",
     author_email="gcasabona.pro@gmail.com",
     license="MIT",
     classifiers=[
+        "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
+        "Intended Audience :: Developers",
+        "Natural Language :: English"
+    ],
+    install_requires=[
+        "loguru >= 0.7.0",
+        "requests == 2.29.0" #Higher version can break your docker python lib
     ],
-    install_requires=["loguru >= 0.7.0"],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.8",
 )
```

