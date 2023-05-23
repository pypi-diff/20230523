# Comparing `tmp/pylookyloo-1.8.1.tar.gz` & `tmp/pylookyloo-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookyloo-1.8.1.tar", max compression
+gzip compressed data, was "pylookyloo-1.9.0.tar", max compression
```

## Comparing `pylookyloo-1.8.1.tar` & `pylookyloo-1.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2020-09-08 11:35:20.750489 pylookyloo-1.8.1/LICENSE
--rw-r--r--   0        0        0      959 2021-03-23 13:46:11.991472 pylookyloo-1.8.1/README.md
--rw-r--r--   0        0        0     1749 2021-09-11 14:45:53.271216 pylookyloo-1.8.1/pylookyloo/__init__.py
--rw-r--r--   0        0        0     9549 2021-09-11 14:44:41.710338 pylookyloo-1.8.1/pylookyloo/api.py
--rw-r--r--   0        0        0        0 2020-03-16 16:12:28.873646 pylookyloo-1.8.1/pylookyloo/py.typed
--rw-r--r--   0        0        0     1254 2021-09-11 14:46:57.628004 pylookyloo-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1858 2021-09-11 14:50:20.701645 pylookyloo-1.8.1/setup.py
--rw-r--r--   0        0        0     2129 2021-09-11 14:50:20.701948 pylookyloo-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1516 2020-09-08 11:35:20.750489 pylookyloo-1.9.0/LICENSE
+-rw-r--r--   0        0        0      959 2021-03-23 13:46:11.991472 pylookyloo-1.9.0/README.md
+-rw-r--r--   0        0        0     1749 2021-09-11 14:45:53.271216 pylookyloo-1.9.0/pylookyloo/__init__.py
+-rw-r--r--   0        0        0     9558 2021-09-11 14:51:32.555354 pylookyloo-1.9.0/pylookyloo/api.py
+-rw-r--r--   0        0        0        0 2020-03-16 16:12:28.873646 pylookyloo-1.9.0/pylookyloo/py.typed
+-rw-r--r--   0        0        0     1254 2021-09-28 15:43:53.965556 pylookyloo-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1858 2021-09-28 15:44:46.381154 pylookyloo-1.9.0/setup.py
+-rw-r--r--   0        0        0     2129 2021-09-28 15:44:46.381512 pylookyloo-1.9.0/PKG-INFO
```

### Comparing `pylookyloo-1.8.1/LICENSE` & `pylookyloo-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookyloo-1.8.1/README.md` & `pylookyloo-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pylookyloo-1.8.1/pylookyloo/__init__.py` & `pylookyloo-1.9.0/pylookyloo/__init__.py`

 * *Files identical despite different names*

### Comparing `pylookyloo-1.8.1/pylookyloo/api.py` & `pylookyloo-1.9.0/pylookyloo/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,18 +70,19 @@
             raise PyLookylooError(f'url entry required: {kwargs}')
 
         if url:
             to_send = {'url': url, **kwargs}
         else:
             to_send = kwargs
         response = self.session.post(urljoin(self.root_url, 'submit'), json=to_send)
+        uuid = response.json()
         if quiet:
-            return response.json()
+            return uuid
         else:
-            return urljoin(self.root_url, f'tree/{response.json()}')
+            return urljoin(self.root_url, f'tree/{uuid}')
 
     def get_apikey(self, username: str, password: str) -> Dict[str, str]:
         '''Get the API key for the given user.'''
         to_post = {'username': username, 'password': password}
         r = self.session.post(urljoin(self.root_url, str(Path('json', 'get_token'))), json=to_post)
         return r.json()
```

### Comparing `pylookyloo-1.8.1/pyproject.toml` & `pylookyloo-1.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylookyloo"
-version = "1.8.1"
+version = "1.9.0"
 description = "Python CLI and module for Lookyloo"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/lookyloo/PyLookyloo"
 documentation = "https://pylookyloo.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,19 +28,19 @@
 
 [tool.poetry.scripts]
 lookyloo = 'pylookyloo:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
-Sphinx = { version = "^4.0.2", optional = true }
+Sphinx = { version = "^4.2.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.910"
-types-requests = "^2.25.0"
+types-requests = "^2.25.9"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry_core>=1.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylookyloo-1.8.1/setup.py` & `pylookyloo-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.26.0,<3.0.0']
 
 extras_require = \
-{'docs': ['Sphinx>=4.0.2,<5.0.0']}
+{'docs': ['Sphinx>=4.2.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['lookyloo = pylookyloo:main']}
 
 setup_kwargs = {
     'name': 'pylookyloo',
-    'version': '1.8.1',
+    'version': '1.9.0',
     'description': 'Python CLI and module for Lookyloo',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/pylookyloo/badge/?version=latest)](https://pylookyloo.readthedocs.io/en/latest/?badge=latest)\n\n# PyLookyloo\n\nThis is the client API for [Lookyloo](https://www.lookyloo.eu).\n\n## Installation\n\n```bash\npip install pylookyloo\n```\n\n## Usage\n\n### Command line\n\nYou can use the `lookyloo` command to enqueue a URL.\n\n```bash\nusage: lookyloo [-h] [--url URL] --query QUERY\n\nEnqueue a URL on Lookyloo.\n\noptional arguments:\n  -h, --help     show this help message and exit\n  --url URL      URL of the instance (defaults to https://lookyloo.circl.lu/,\n                 the public instance).\n  --query QUERY  URL to enqueue.\n  --listing      Should the report be publicly listed.\n  --redirects    Get redirects for a given capture.\n\nThe response is the permanent URL where you can see the result of the capture.\n```\n\n### Library\n\nSee [API Reference](https://pylookyloo.readthedocs.io/en/latest/api_reference.html)\n',
     'author': 'Raphaël Vinot',
     'author_email': 'raphael.vinot@circl.lu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/lookyloo/PyLookyloo',
```

### Comparing `pylookyloo-1.8.1/PKG-INFO` & `pylookyloo-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookyloo
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python CLI and module for Lookyloo
 Home-page: https://github.com/lookyloo/PyLookyloo
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.0.2,<5.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=4.2.0,<5.0.0); extra == "docs"
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Documentation, https://pylookyloo.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/lookyloo/PyLookyloo
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pylookyloo/badge/?version=latest)](https://pylookyloo.readthedocs.io/en/latest/?badge=latest)
```

