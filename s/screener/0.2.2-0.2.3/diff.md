# Comparing `tmp/screener-0.2.2.tar.gz` & `tmp/screener-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screener-0.2.2.tar", max compression
+gzip compressed data, was "screener-0.2.3.tar", max compression
```

## Comparing `screener-0.2.2.tar` & `screener-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2564 2023-05-21 20:33:51.440358 screener-0.2.2/README.md
--rw-r--r--   0        0        0     2308 2023-05-23 18:37:42.326224 screener-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.2.2/screener/__init__.py
--rw-r--r--   0        0        0     1839 2023-05-21 15:27:52.900285 screener-0.2.2/screener/__main__.py
--rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.2.2/screener/parser/__init__.py
--rw-r--r--   0        0        0      727 2023-05-21 20:35:22.715235 screener-0.2.2/screener/parser/epub.py
--rw-r--r--   0        0        0      809 2023-05-22 09:42:14.086332 screener-0.2.2/screener/parser/kindle.py
--rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.2.2/screener/reader/__init__.py
--rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.2.2/screener/reader/abstract.py
--rw-r--r--   0        0        0      877 2023-05-22 10:19:24.692693 screener-0.2.2/screener/reader/epub.py
--rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.2.2/screener/reader/kindle.py
--rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.2.2/screener/utils.py
--rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 screener-0.2.2/setup.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 screener-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1866 2023-05-23 18:42:05.097804 screener-0.2.3/README.md
+-rw-r--r--   0        0        0     2451 2023-05-23 18:56:40.870037 screener-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.2.3/screener/__init__.py
+-rw-r--r--   0        0        0     1839 2023-05-23 18:56:40.885037 screener-0.2.3/screener/__main__.py
+-rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.2.3/screener/parser/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-21 20:35:22.715235 screener-0.2.3/screener/parser/epub.py
+-rw-r--r--   0        0        0      809 2023-05-22 09:42:14.086332 screener-0.2.3/screener/parser/kindle.py
+-rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.2.3/screener/reader/__init__.py
+-rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.2.3/screener/reader/abstract.py
+-rw-r--r--   0        0        0      877 2023-05-22 10:19:24.692693 screener-0.2.3/screener/reader/epub.py
+-rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.2.3/screener/reader/kindle.py
+-rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.2.3/screener/utils.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 screener-0.2.3/setup.py
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 screener-0.2.3/PKG-INFO
```

### Comparing `screener-0.2.2/README.md` & `screener-0.2.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-# Screener
-
-Check e-book files for security and privacy issues.
-
-_Screener is currently in early development. Please consider contributing if you have the time and know-how!_
-
-## Motivation
-
-E-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.
-
-Screener aims to check e-book files for these issues so that you can read with peace of mind!
-
-## Features
-
-- Check e-book files for JavaScript tags.
-- Check e-book files for images with external sources to prevent tracking.
-- Supports `.epub`, `.mobi`, and `.azw3` files.
-
-## Get started
-
-These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
-
-### Prerequisites
-
-Screener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 is recommended), [pip](https://pip.pypa.io/en/stable/getting-started/), and [Poetry](https://python-poetry.org/docs/#installation) to be installed.
-
-### Installing
-
-Copy the files in this repository and navigate to the repository directory. You can run the project with `poetry run`.
-
-```commandline
-poetry run python -m screener
-```
-
-You can also run tests.
-
-```commandline
-poetry run pytest
-```
-
-With coverage metrics:
-
-```commandline
-poetry run coverage run -m pytest
-```
-
-Type-checking:
-
-```commandline
-poetry run mypy screener/
-```
-
-This is the recommended way to install Screener for development and testing.
-
-#### Alternative installation
-
-If you would rather not use `poetry run`, you can use `poetry export` to create a `requirements.txt` file and install the packages directly using `pip`.
-
-```commandline
-poetry export -f requirements.txt --output requirements.txt
-pip install -r requirements.txt
-```
-
-You can then use Python as normal.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-At present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.
-
-Please make sure to update tests as appropriate.
-
-## Versioning
-
-This project uses [SemVer](http://semver.org/) for versioning.
-
-## Authors
-
-Screener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).
-
-## Licence
-
-Screener is released under the [LGPL version 3](LICENCE).
+Metadata-Version: 2.1
+Name: screener
+Version: 0.2.3
+Summary: Check e-book files for security and privacy issues.
+Home-page: https://github.com/tjkuson/screener/
+License: GPL-3.0-only
+Keywords: ebook,security,privacy,epub,mobi,kindle
+Author: Tom Kuson
+Author-email: mail@tjkuson.me
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
+Requires-Dist: EbookLib (>=0.18,<0.19)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: mobi (>=0.3.3,<0.4.0)
+Project-URL: Repository, https://github.com/tjkuson/screener/
+Description-Content-Type: text/markdown
+
+# Screener
+
+Check e-book files for security and privacy issues.
+
+_Screener is currently in early development. Please consider contributing if you have the time and know-how!_
+
+## Motivation
+
+E-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.
+
+Screener aims to check e-book files for these issues so that you can read with peace of mind!
+
+## Features
+
+- Check e-book files for JavaScript tags.
+- Check e-book files for images with external sources to prevent tracking.
+- Supports `.epub`, `.mobi`, and `.azw3` files.
+
+## Get started
+
+These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
+
+### Prerequisites
+
+Screener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).
+
+### Installing
+
+Screen is available on [PyPI](https://pypi.org/project/screener/). To install, run:
+
+```bash
+pip install screener
+```
+
+#### Development installation
+
+To install Screener for development, clone the repository and run:
+
+```bash
+poetry install
+```
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+At present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.
+
+Please make sure to update tests as appropriate.
+
+## Versioning
+
+This project uses [SemVer](http://semver.org/) for versioning.
+
+## Authors
+
+Screener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).
+
+## Licence
+
+Screener is released under the [LGPL version 3](LICENCE).
+
```

### Comparing `screener-0.2.2/pyproject.toml` & `screener-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 [tool.poetry]
 name = "Screener"
-version = "0.2.2"
+version = "0.2.3"
 description = "Check e-book files for security and privacy issues."
-license = "LGPL-3.0-only"
 authors = ["Tom Kuson <mail@tjkuson.me>"]
-repository = "https://github.com/tjkuson/screener/"
+license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "screener", from = "." },
 ]
+repository = "https://github.com/tjkuson/screener/"
+keywords = ["ebook", "security", "privacy", "epub", "mobi", "kindle"]
+classifiers = [
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 EbookLib = "^0.18"
 beautifulsoup4 = "^4.12.2"
 mobi = "^0.3.3"
```

### Comparing `screener-0.2.2/screener/__main__.py` & `screener-0.2.3/screener/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         usage="%(prog)s [OPTION] [FILE]...",
         description="Check e-book files for security and privacy issues.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
-        version=f"{parser.prog} version 0.2.1",
+        version=f"{parser.prog} version 0.2.3",
     )
     parser.add_argument("files", nargs="*")
     return parser
 
 
 def main() -> None:
     """Read system args and check e-book files."""
```

### Comparing `screener-0.2.2/screener/parser/epub.py` & `screener-0.2.3/screener/parser/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.2/screener/parser/kindle.py` & `screener-0.2.3/screener/parser/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.2/screener/reader/abstract.py` & `screener-0.2.3/screener/reader/abstract.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.2/screener/reader/epub.py` & `screener-0.2.3/screener/reader/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.2/screener/reader/kindle.py` & `screener-0.2.3/screener/reader/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.2/screener/utils.py` & `screener-0.2.3/screener/utils.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.2/setup.py` & `screener-0.2.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['EbookLib>=0.18,<0.19', 'beautifulsoup4>=4.12.2,<5.0.0', 'mobi>=0.3.3,<0.4.0']
 
 setup_kwargs = {
     'name': 'screener',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Check e-book files for security and privacy issues.',
-    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n_Screener is currently in early development. Please consider contributing if you have the time and know-how!_\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 is recommended), [pip](https://pip.pypa.io/en/stable/getting-started/), and [Poetry](https://python-poetry.org/docs/#installation) to be installed.\n\n### Installing\n\nCopy the files in this repository and navigate to the repository directory. You can run the project with `poetry run`.\n\n```commandline\npoetry run python -m screener\n```\n\nYou can also run tests.\n\n```commandline\npoetry run pytest\n```\n\nWith coverage metrics:\n\n```commandline\npoetry run coverage run -m pytest\n```\n\nType-checking:\n\n```commandline\npoetry run mypy screener/\n```\n\nThis is the recommended way to install Screener for development and testing.\n\n#### Alternative installation\n\nIf you would rather not use `poetry run`, you can use `poetry export` to create a `requirements.txt` file and install the packages directly using `pip`.\n\n```commandline\npoetry export -f requirements.txt --output requirements.txt\npip install -r requirements.txt\n```\n\nYou can then use Python as normal.\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
+    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n_Screener is currently in early development. Please consider contributing if you have the time and know-how!_\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreen is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
     'author': 'Tom Kuson',
     'author_email': 'mail@tjkuson.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tjkuson/screener/',
     'package_dir': package_dir,
     'packages': packages,
```

