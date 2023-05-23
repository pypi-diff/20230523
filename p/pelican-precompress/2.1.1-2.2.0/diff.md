# Comparing `tmp/pelican_precompress-2.1.1.tar.gz` & `tmp/pelican_precompress-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_precompress-2.1.1.tar", max compression
+gzip compressed data, was "pelican_precompress-2.2.0.tar", max compression
```

## Comparing `pelican_precompress-2.1.1.tar` & `pelican_precompress-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1098 2022-03-29 13:26:52.335321 pelican_precompress-2.1.1/LICENSE.txt
--rw-r--r--   0        0        0      924 2022-03-29 13:26:52.335321 pelican_precompress-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     7139 2022-03-29 13:26:52.335321 pelican_precompress-2.1.1/README.rst
--rw-r--r--   0        0        0     8447 2022-03-29 13:26:52.335321 pelican_precompress-2.1.1/src/pelican/plugins/precompress/__init__.py
--rw-r--r--   0        0        0     8162 2022-03-29 13:27:26.455483 pelican_precompress-2.1.1/setup.py
--rw-r--r--   0        0        0     8050 2022-03-29 13:27:26.455483 pelican_precompress-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-23 01:32:07.104662 pelican_precompress-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1064 2023-05-23 01:32:07.107747 pelican_precompress-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7300 2023-05-23 01:32:07.105659 pelican_precompress-2.2.0/README.rst
+-rw-r--r--   0        0        0     8447 2023-05-23 01:32:07.109910 pelican_precompress-2.2.0/src/pelican/plugins/precompress/__init__.py
+-rw-r--r--   0        0        0     8205 1970-01-01 00:00:00.000000 pelican_precompress-2.2.0/PKG-INFO
```

### Comparing `pelican_precompress-2.1.1/LICENSE.txt` & `pelican_precompress-2.2.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2022 Kurt McKee <contactme@kurtmckee.org>
+Copyright (c) 2019-2023 Kurt McKee <contactme@kurtmckee.org>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pelican_precompress-2.1.1/pyproject.toml` & `pelican_precompress-2.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican_precompress"
-version = "2.1.1"
+version = "2.2.0"
 description = "Pre-compress your Pelican site using gzip, zopfli, and brotli!"
 authors = ["Kurt McKee <contactme@kurtmckee.org>"]
 license = "MIT"
 packages = [
     { include = "pelican", from = "src" }
 ]
 readme = "README.rst"
@@ -12,33 +12,44 @@
 keywords = ["pelican", "plugin", "gzip", "brotli", "zopfli"]
 classifiers = [
     "Framework :: Pelican :: Plugins",
     "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.8"
 pelican-granular-signals = "^1.0.0"
 
-[tool.poetry.dev-dependencies]
-tox = "^3.23.0"
-isort = "^5.10.1"
-black = "^22.3.0"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.coverage.run]
 branch = true
+parallel = true
+data_file = ".tox/.coverage-data-files/.coverage"
+source = [
+    "pelican.plugins.precompress",
+    "tests",
+]
 
 
 [tool.coverage.paths]
 source = [
     "src",
     "*/site-packages",
 ]
 
 
+[tool.coverage.report]
+fail_under = 100
+
+
 [tool.isort]
 profile = "black"
+
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+]
```

### Comparing `pelican_precompress-2.1.1/README.rst` & `pelican_precompress-2.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..  This file is part of the pelican_precompress plugin.
-..  Copyright 2019-2022 Kurt McKee <contactme@kurtmckee.org>
+..  Copyright 2019-2023 Kurt McKee <contactme@kurtmckee.org>
 ..  Released under the MIT license.
 
 pelican_precompress
 *******************
 
 *Pre-compress your Pelican site using gzip, zopfli, and brotli!*
 
@@ -167,19 +167,28 @@
 If you'd like to develop and/or test the code yourself,
 clone the git repository and run these commands to set
 up a Python virtual environment, install dependencies,
 and run the test suite:
 
 ..  code-block:: shell
 
-    $ python -m venv venv
-    $ source venv/bin/activate
-    (venv) $ python -m pip install poetry
-    (venv) $ poetry update
-    (venv) $ tox
+    python -m venv .venv
+
+    # Activate the virtual environment (Linux)
+    source .venv/bin/activate
+
+    # Activate the virtual environment (Windows)
+    & .venv/Scripts/Activate.ps1
+
+    python -m pip install poetry pre-commit tox
+    pre-commit install
+    poetry install
+
+    # Run the test suite
+    tox
 
 The test suite uses tox to setup multiple environments with varying
 dependencies using multiple Python interpreters; pytest allows the
 test suite to have parametrized tests; pyfakefs creates a fake
 filesystem that the tests safely create and erase files in;
 and coverage keeps track of which lines of code have been run.
 
@@ -196,12 +205,12 @@
 ..  _Pelican plugins: https://docs.getpelican.com/en/latest/plugins.html
 ..  _zopfli: https://pypi.org/project/zopfli/
 ..  _brotli: https://pypi.org/project/Brotli/
 ..  _gzip_static: https://nginx.org/en/docs/http/ngx_http_gzip_static_module.html#gzip_static
 ..  _gzip_vary: https://nginx.org/en/docs/http/ngx_http_gzip_module.html#gzip_vary
 ..  _nginx brotli module: https://github.com/google/ngx_brotli
 ..  _poetry: https://python-poetry.org/
-..  _tox: https://tox.readthedocs.io/en/latest/
+..  _tox: https://tox.wiki/en/latest/
 ..  _pytest: https://docs.pytest.org/en/latest/
-..  _pyfakefs: https://jmcgeheeiv.github.io/pyfakefs/release/
+..  _pyfakefs: https://pytest-pyfakefs.readthedocs.io/en/latest/
 ..  _venv: https://docs.python.org/3/library/venv.html
 ..  _coverage: https://coverage.readthedocs.io/en/latest/
```

### Comparing `pelican_precompress-2.1.1/src/pelican/plugins/precompress/__init__.py` & `pelican_precompress-2.2.0/src/pelican/plugins/precompress/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is part of the pelican-precompress plugin.
-# Copyright 2019-2022 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2019-2023 Kurt McKee <contactme@kurtmckee.org>
 # Released under the MIT license.
 
 import functools
 import gzip
 import logging
 import multiprocessing
 import pathlib
```

### Comparing `pelican_precompress-2.1.1/setup.py` & `pelican_precompress-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,239 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-precompress
+Version: 2.2.0
+Summary: Pre-compress your Pelican site using gzip, zopfli, and brotli!
+Home-page: https://github.com/kurtmckee/pelican_precompress/
+License: MIT
+Keywords: pelican,plugin,gzip,brotli,zopfli
+Author: Kurt McKee
+Author-email: contactme@kurtmckee.org
+Requires-Python: >=3.8
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pelican :: Plugins
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pelican-granular-signals (>=1.0.0,<2.0.0)
+Project-URL: Repository, https://github.com/kurtmckee/pelican_precompress/
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+..  This file is part of the pelican_precompress plugin.
+..  Copyright 2019-2023 Kurt McKee <contactme@kurtmckee.org>
+..  Released under the MIT license.
 
-packages = \
-['pelican', 'pelican.plugins.precompress']
+pelican_precompress
+*******************
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pelican-granular-signals>=1.0.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pelican-precompress',
-    'version': '2.1.1',
-    'description': 'Pre-compress your Pelican site using gzip, zopfli, and brotli!',
-    'long_description': "..  This file is part of the pelican_precompress plugin.\n..  Copyright 2019-2022 Kurt McKee <contactme@kurtmckee.org>\n..  Released under the MIT license.\n\npelican_precompress\n*******************\n\n*Pre-compress your Pelican site using gzip, zopfli, and brotli!*\n\n----\n\nAre you using `Pelican`_, the static site generator? If so, great!\nAre you pre-compressing your static files to have the fastest site possible?\nIf not, install **pelican_precompress** today!\nIt's the plugin that makes your visitors happy and saves you money!\n\n\nInstallation\n============\n\nThere are three steps required to start using static compression:\n\n#.  Install the plugin and any supporting Python packages you want.\n#.  Configure Pelican to use the pelican_precompress plugin.\n#.  Configure your web server to use static, pre-compressed files.\n\n\n1. Install the Python modules\n-----------------------------\n\nAt minimum, you'll need to install the pelican_precompress plugin.\nIt will automatically generate gzip files because gzip is built into the\nPython standard library.\n\nHowever, if you want highly-optimized gzip files you'll need the zopfli module.\nAnd if you want to have the very best compression currently available, you'll\nneed to install the brotli module (which will require extra work in step 3).\n\n..  code-block:: shell-session\n\n    $ pip install pelican_precompress\n    $ pip install zopfli  # This produces smaller gzip'd files. Use it!\n    $ pip install brotli  # This requires extra work in step 3.\n\nFurther reading: `zopfli`_, `brotli`_\n\n\n2. Configure Pelican\n--------------------\n\nIf you're using Pelican 4.5 or higher then you might not need to configure anything.\npelican_precompress supports Pelican's namespace plugin architecture\nand will be automatically detected and loaded when Pelican runs.\n\nHowever, if you're maintaining a list of plugins for Pelican to use (even in Pelican 4.5)\nthen you'll need to add it to the list of active plugins.\n\nFeel free to copy and paste the code below into your Pelican configuration file.\nJust uncomment and edit the configuration lines to your liking...or leave\nthem alone because the defaults are awesome!\n\n..  code-block:: python3\n\n    # Pelican 4.5 introduced automatic plugin discovery and loading.\n    # You only need to add pelican_precompress to your PLUGINS list\n    # if your configuration file already has a PLUGINS list!\n    #\n    # PLUGINS = ['pelican.plugins.precompress']\n\n    # These options can be customized as desired.\n    #\n    # PRECOMPRESS_GZIP = True or False\n    # PRECOMPRESS_ZOPFLI = True or False\n    # PRECOMPRESS_BROTLI = True or False\n    # PRECOMPRESS_OVERWRITE = False\n    # PRECOMPRESS_MIN_SIZE = 20\n    # PRECOMPRESS_TEXT_EXTENSIONS = {\n    #     '.atom',\n    #     '.css',\n    #     '.html',\n    #     '.but-the-default-extensions-are-pretty-comprehensive',\n    # }\n\nFurther reading: `Pelican plugins`_\n\n\n3. Configure nginx\n------------------\n\nnginx supports gzip compression right out of the box.\nTo enable it, add something like this to your nginx configuration file:\n\n..  code-block:: nginx\n\n    http {\n        gzip_static on;\n        gzip_vary on;\n    }\n\nAt the time of writing, nginx doesn't natively support brotli compression.\nTo get it, you'll need to compile the static brotli module as an nginx\ndynamic module, or recompile nginx from scratch. When it's done you'll\nadd something like this to your nginx configuration file:\n\n..  code-block:: nginx\n\n    load_module /usr/lib/nginx/modules/ngx_http_brotli_static_module.so;\n\n    http {\n        brotli_static on;\n    }\n\nFurther reading: `gzip_static`_, `gzip_vary`_, `nginx brotli module`_\n\n\nConfiguration\n=============\n\nThere are a small number of configuration options available.\nYou set them in your Pelican configuration file.\n\n*   ``PRECOMPRESS_GZIP`` (bool, default is True)\n\n    This is always ``True`` unless you set this to ``False``.\n    For example, you might turn this off during development.\n\n*   ``PRECOMPRESS_ZOPFLI`` (bool, default is True if zopfli is installed)\n\n    If the zopfli module is installed this will default to ``True``.\n    You might set this to ``False`` during development.\n    Note that if you try to enable zopfli compression but the module\n    isn't installed then nothing will happen.\n\n*   ``PRECOMPRESS_BROTLI`` (bool, default is True if brotli is installed)\n\n    If the brotli module is installed this will default to ``True``.\n    You might set this to ``False`` during development.\n    Like ``PRECOMPRESS_ZOPFLI``, if you set this to ``True`` when the\n    brotli module isn't installed then nothing will happen.\n\n*   ``PRECOMPRESS_OVERWRITE`` (bool, default is False)\n\n    When pelican_precompress encounters an existing compressed file\n    it will refuse to overwrite it. If you want the plugin to overwrite\n    files you can set this to ``True``.\n\n*   ``PRECOMPRESS_TEXT_EXTENSIONS`` (Set[str])\n\n    This setting controls which file extensions will be pre-compressed.\n\n    If you modify this setting in the Pelican configuration file it will\n    completely replace the default extensions!\n\n*   ``PRECOMPRESS_MIN_SIZE`` (int, default is 20)\n\n    Small files tend to result in a larger file size when compressed, and any\n    improvement is likely to be marginal. The default setting is chosen to\n    avoid speculatively compressing files that are likely to result in a\n    larger file size after compression.\n\n    To try compressing every file regardless of size, set this to ``0``.\n\n\nDevelopment\n===========\n\nIf you'd like to develop and/or test the code yourself,\nclone the git repository and run these commands to set\nup a Python virtual environment, install dependencies,\nand run the test suite:\n\n..  code-block:: shell\n\n    $ python -m venv venv\n    $ source venv/bin/activate\n    (venv) $ python -m pip install poetry\n    (venv) $ poetry update\n    (venv) $ tox\n\nThe test suite uses tox to setup multiple environments with varying\ndependencies using multiple Python interpreters; pytest allows the\ntest suite to have parametrized tests; pyfakefs creates a fake\nfilesystem that the tests safely create and erase files in;\nand coverage keeps track of which lines of code have been run.\n\n**pelican_precompress** has 100% test coverage, but there may still be bugs.\nPlease report any issues that you encounter.\n\nFurther reading: `poetry`_, `tox`_, `venv`_, `pytest`_, `pyfakefs`_, `coverage`_\n\n\n..  Links\n..  =====\n\n..  _Pelican: https://getpelican.com/\n..  _Pelican plugins: https://docs.getpelican.com/en/latest/plugins.html\n..  _zopfli: https://pypi.org/project/zopfli/\n..  _brotli: https://pypi.org/project/Brotli/\n..  _gzip_static: https://nginx.org/en/docs/http/ngx_http_gzip_static_module.html#gzip_static\n..  _gzip_vary: https://nginx.org/en/docs/http/ngx_http_gzip_module.html#gzip_vary\n..  _nginx brotli module: https://github.com/google/ngx_brotli\n..  _poetry: https://python-poetry.org/\n..  _tox: https://tox.readthedocs.io/en/latest/\n..  _pytest: https://docs.pytest.org/en/latest/\n..  _pyfakefs: https://jmcgeheeiv.github.io/pyfakefs/release/\n..  _venv: https://docs.python.org/3/library/venv.html\n..  _coverage: https://coverage.readthedocs.io/en/latest/\n",
-    'author': 'Kurt McKee',
-    'author_email': 'contactme@kurtmckee.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/kurtmckee/pelican_precompress/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0',
-}
+*Pre-compress your Pelican site using gzip, zopfli, and brotli!*
 
+----
+
+Are you using `Pelican`_, the static site generator? If so, great!
+Are you pre-compressing your static files to have the fastest site possible?
+If not, install **pelican_precompress** today!
+It's the plugin that makes your visitors happy and saves you money!
+
+
+Installation
+============
+
+There are three steps required to start using static compression:
+
+#.  Install the plugin and any supporting Python packages you want.
+#.  Configure Pelican to use the pelican_precompress plugin.
+#.  Configure your web server to use static, pre-compressed files.
+
+
+1. Install the Python modules
+-----------------------------
+
+At minimum, you'll need to install the pelican_precompress plugin.
+It will automatically generate gzip files because gzip is built into the
+Python standard library.
+
+However, if you want highly-optimized gzip files you'll need the zopfli module.
+And if you want to have the very best compression currently available, you'll
+need to install the brotli module (which will require extra work in step 3).
+
+..  code-block:: shell-session
+
+    $ pip install pelican_precompress
+    $ pip install zopfli  # This produces smaller gzip'd files. Use it!
+    $ pip install brotli  # This requires extra work in step 3.
+
+Further reading: `zopfli`_, `brotli`_
+
+
+2. Configure Pelican
+--------------------
+
+If you're using Pelican 4.5 or higher then you might not need to configure anything.
+pelican_precompress supports Pelican's namespace plugin architecture
+and will be automatically detected and loaded when Pelican runs.
+
+However, if you're maintaining a list of plugins for Pelican to use (even in Pelican 4.5)
+then you'll need to add it to the list of active plugins.
+
+Feel free to copy and paste the code below into your Pelican configuration file.
+Just uncomment and edit the configuration lines to your liking...or leave
+them alone because the defaults are awesome!
+
+..  code-block:: python3
+
+    # Pelican 4.5 introduced automatic plugin discovery and loading.
+    # You only need to add pelican_precompress to your PLUGINS list
+    # if your configuration file already has a PLUGINS list!
+    #
+    # PLUGINS = ['pelican.plugins.precompress']
+
+    # These options can be customized as desired.
+    #
+    # PRECOMPRESS_GZIP = True or False
+    # PRECOMPRESS_ZOPFLI = True or False
+    # PRECOMPRESS_BROTLI = True or False
+    # PRECOMPRESS_OVERWRITE = False
+    # PRECOMPRESS_MIN_SIZE = 20
+    # PRECOMPRESS_TEXT_EXTENSIONS = {
+    #     '.atom',
+    #     '.css',
+    #     '.html',
+    #     '.but-the-default-extensions-are-pretty-comprehensive',
+    # }
+
+Further reading: `Pelican plugins`_
+
+
+3. Configure nginx
+------------------
+
+nginx supports gzip compression right out of the box.
+To enable it, add something like this to your nginx configuration file:
+
+..  code-block:: nginx
+
+    http {
+        gzip_static on;
+        gzip_vary on;
+    }
+
+At the time of writing, nginx doesn't natively support brotli compression.
+To get it, you'll need to compile the static brotli module as an nginx
+dynamic module, or recompile nginx from scratch. When it's done you'll
+add something like this to your nginx configuration file:
+
+..  code-block:: nginx
+
+    load_module /usr/lib/nginx/modules/ngx_http_brotli_static_module.so;
+
+    http {
+        brotli_static on;
+    }
+
+Further reading: `gzip_static`_, `gzip_vary`_, `nginx brotli module`_
+
+
+Configuration
+=============
+
+There are a small number of configuration options available.
+You set them in your Pelican configuration file.
+
+*   ``PRECOMPRESS_GZIP`` (bool, default is True)
+
+    This is always ``True`` unless you set this to ``False``.
+    For example, you might turn this off during development.
+
+*   ``PRECOMPRESS_ZOPFLI`` (bool, default is True if zopfli is installed)
+
+    If the zopfli module is installed this will default to ``True``.
+    You might set this to ``False`` during development.
+    Note that if you try to enable zopfli compression but the module
+    isn't installed then nothing will happen.
+
+*   ``PRECOMPRESS_BROTLI`` (bool, default is True if brotli is installed)
+
+    If the brotli module is installed this will default to ``True``.
+    You might set this to ``False`` during development.
+    Like ``PRECOMPRESS_ZOPFLI``, if you set this to ``True`` when the
+    brotli module isn't installed then nothing will happen.
+
+*   ``PRECOMPRESS_OVERWRITE`` (bool, default is False)
+
+    When pelican_precompress encounters an existing compressed file
+    it will refuse to overwrite it. If you want the plugin to overwrite
+    files you can set this to ``True``.
+
+*   ``PRECOMPRESS_TEXT_EXTENSIONS`` (Set[str])
+
+    This setting controls which file extensions will be pre-compressed.
+
+    If you modify this setting in the Pelican configuration file it will
+    completely replace the default extensions!
+
+*   ``PRECOMPRESS_MIN_SIZE`` (int, default is 20)
+
+    Small files tend to result in a larger file size when compressed, and any
+    improvement is likely to be marginal. The default setting is chosen to
+    avoid speculatively compressing files that are likely to result in a
+    larger file size after compression.
+
+    To try compressing every file regardless of size, set this to ``0``.
+
+
+Development
+===========
+
+If you'd like to develop and/or test the code yourself,
+clone the git repository and run these commands to set
+up a Python virtual environment, install dependencies,
+and run the test suite:
+
+..  code-block:: shell
+
+    python -m venv .venv
+
+    # Activate the virtual environment (Linux)
+    source .venv/bin/activate
+
+    # Activate the virtual environment (Windows)
+    & .venv/Scripts/Activate.ps1
+
+    python -m pip install poetry pre-commit tox
+    pre-commit install
+    poetry install
+
+    # Run the test suite
+    tox
+
+The test suite uses tox to setup multiple environments with varying
+dependencies using multiple Python interpreters; pytest allows the
+test suite to have parametrized tests; pyfakefs creates a fake
+filesystem that the tests safely create and erase files in;
+and coverage keeps track of which lines of code have been run.
+
+**pelican_precompress** has 100% test coverage, but there may still be bugs.
+Please report any issues that you encounter.
+
+Further reading: `poetry`_, `tox`_, `venv`_, `pytest`_, `pyfakefs`_, `coverage`_
+
+
+..  Links
+..  =====
+
+..  _Pelican: https://getpelican.com/
+..  _Pelican plugins: https://docs.getpelican.com/en/latest/plugins.html
+..  _zopfli: https://pypi.org/project/zopfli/
+..  _brotli: https://pypi.org/project/Brotli/
+..  _gzip_static: https://nginx.org/en/docs/http/ngx_http_gzip_static_module.html#gzip_static
+..  _gzip_vary: https://nginx.org/en/docs/http/ngx_http_gzip_module.html#gzip_vary
+..  _nginx brotli module: https://github.com/google/ngx_brotli
+..  _poetry: https://python-poetry.org/
+..  _tox: https://tox.wiki/en/latest/
+..  _pytest: https://docs.pytest.org/en/latest/
+..  _pyfakefs: https://pytest-pyfakefs.readthedocs.io/en/latest/
+..  _venv: https://docs.python.org/3/library/venv.html
+..  _coverage: https://coverage.readthedocs.io/en/latest/
 
-setup(**setup_kwargs)
```

