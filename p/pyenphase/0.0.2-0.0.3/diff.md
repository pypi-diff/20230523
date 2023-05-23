# Comparing `tmp/pyenphase-0.0.2.tar.gz` & `tmp/pyenphase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.0.2.tar", max compression
+gzip compressed data, was "pyenphase-0.0.3.tar", max compression
```

## Comparing `pyenphase-0.0.2.tar` & `pyenphase-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-05-23 14:45:58.481011 pyenphase-0.0.2/LICENSE
--rw-r--r--   0        0        0     3476 2023-05-23 14:45:58.475854 pyenphase-0.0.2/README.md
--rw-r--r--   0        0        0     2226 2023-05-23 15:13:56.980875 pyenphase-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-23 14:46:16.272879 pyenphase-0.0.2/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-23 14:59:20.964327 pyenphase-0.0.2/src/pyenphase/auth.py
--rw-r--r--   0        0        0     2404 2023-05-23 15:04:01.936595 pyenphase-0.0.2/src/pyenphase/envoy.py
--rw-r--r--   0        0        0      446 2023-05-23 14:53:58.015119 pyenphase-0.0.2/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1321 2023-05-23 15:05:28.214252 pyenphase-0.0.2/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-05-23 14:45:58.501807 pyenphase-0.0.2/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-05-23 14:45:58.501248 pyenphase-0.0.2/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-05-23 15:05:18.328813 pyenphase-0.0.2/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 pyenphase-0.0.2/setup.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 pyenphase-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 15:34:59.410828 pyenphase-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3476 2023-05-23 15:34:59.410828 pyenphase-0.0.3/README.md
+-rw-r--r--   0        0        0     2226 2023-05-23 15:35:00.174826 pyenphase-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-23 15:35:00.138826 pyenphase-0.0.3/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/auth.py
+-rw-r--r--   0        0        0     2404 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0      446 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1321 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-05-23 15:34:59.414828 pyenphase-0.0.3/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 pyenphase-0.0.3/PKG-INFO
```

### Comparing `pyenphase-0.0.2/LICENSE` & `pyenphase-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.2/README.md` & `pyenphase-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.2/pyproject.toml` & `pyenphase-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.0.2"
+version = "0.0.3"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.0.2/src/pyenphase/auth.py` & `pyenphase-0.0.3/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.2/src/pyenphase/envoy.py` & `pyenphase-0.0.3/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.2/src/pyenphase/firmware.py` & `pyenphase-0.0.3/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.2/src/pyenphase/ssl.py` & `pyenphase-0.0.3/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.2/setup.py` & `pyenphase-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyenphase
+Version: 0.0.3
+Summary: Library to control enphase envoy
+Home-page: https://github.com/pyenphase/pyenphase
+License: MIT
+Author: pyenphase
+Author-email: cgarwood@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: awesomeversion (>=22.9.0)
+Requires-Dist: httpx (>=0.24.0)
+Requires-Dist: lxml (>=4.9.2)
+Requires-Dist: pyjwt (>=2.7.0)
+Project-URL: Bug Tracker, https://github.com/pyenphase/pyenphase/issues
+Project-URL: Changelog, https://github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://pyenphase.readthedocs.io
+Project-URL: Repository, https://github.com/pyenphase/pyenphase
+Description-Content-Type: text/markdown
+
+# pyenphase
+
+<p align="center">
+  <a href="https://github.com/pyenphase/pyenphase/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/pyenphase/pyenphase/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://pyenphase.readthedocs.io">
+    <img src="https://img.shields.io/readthedocs/pyenphase.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/pyenphase/pyenphase">
+    <img src="https://img.shields.io/codecov/c/github/pyenphase/pyenphase.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/pyenphase/">
+    <img src="https://img.shields.io/pypi/v/pyenphase.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/pyenphase.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/pyenphase.svg?style=flat-square" alt="License">
+</p>
+
+Library to control enphase envoy
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install pyenphase`
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-enable -->
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pyenphase']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['awesomeversion>=22.9.0', 'httpx>=0.24.0', 'lxml>=4.9.2', 'pyjwt>=2.7.0']
-
-setup_kwargs = {
-    'name': 'pyenphase',
-    'version': '0.0.2',
-    'description': 'Library to control enphase envoy',
-    'long_description': '# pyenphase\n\n<p align="center">\n  <a href="https://github.com/pyenphase/pyenphase/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/pyenphase/pyenphase/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://pyenphase.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/pyenphase.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/pyenphase/pyenphase">\n    <img src="https://img.shields.io/codecov/c/github/pyenphase/pyenphase.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/pyenphase/">\n    <img src="https://img.shields.io/pypi/v/pyenphase.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/pyenphase.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/pyenphase.svg?style=flat-square" alt="License">\n</p>\n\nLibrary to control enphase envoy\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install pyenphase`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
-    'author': 'pyenphase',
-    'author_email': 'cgarwood@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pyenphase/pyenphase',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['pyenphase'] package_data = \ {'': ['*']} install_requires
-= \ ['awesomeversion>=22.9.0', 'httpx>=0.24.0', 'lxml>=4.9.2', 'pyjwt>=2.7.0']
-setup_kwargs = { 'name': 'pyenphase', 'version': '0.0.2', 'description':
-'Library to control enphase envoy', 'long_description': '# pyenphase\n\n
-     \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
-                                percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nLibrary to control enphase envoy\n\n## Installation\n\nInstall this via pip
-(or your favourite package manager):\n\n`pip install pyenphase`\n\n##
-Contributors â¨\n\nThanks goes to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n\n\n\n\nThis project follows
-the [all-contributors](https://github.com/all-contributors/all-contributors)
-specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package
-was created with\n[Copier](https://copier.readthedocs.io/) and the\n
-[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
-template)\nproject template.\n', 'author': 'pyenphase', 'author_email':
-'cgarwood@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/pyenphase/pyenphase', 'package_dir': package_dir,
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: pyenphase Version: 0.0.3 Summary: Library to
+control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
+License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
+Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: awesomeversion (>=22.9.0) Requires-Dist: httpx (>=0.24.0) Requires-Dist:
+lxml (>=4.9.2) Requires-Dist: pyjwt (>=2.7.0) Project-URL: Bug Tracker, https:/
+/github.com/pyenphase/pyenphase/issues Project-URL: Changelog, https://
+github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md Project-URL:
+Documentation, https://pyenphase.readthedocs.io Project-URL: Repository, https:
+//github.com/pyenphase/pyenphase Description-Content-Type: text/markdown #
+pyenphase
+         [CI_Status] [Documentation_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+Library to control enphase envoy ## Installation Install this via pip (or your
+favourite package manager): `pip install pyenphase` ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)):       This project follows the [all-contributors](https://
+github.com/all-contributors/all-contributors) specification. Contributions of
+any kind welcome! ## Credits This package was created with [Copier](https://
+copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
+github.com/browniebroke/pypackage-template) project template.
```

