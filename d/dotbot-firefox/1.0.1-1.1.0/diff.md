# Comparing `tmp/dotbot-firefox-1.0.1.tar.gz` & `tmp/dotbot_firefox-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotbot-firefox-1.0.1.tar", max compression
+gzip compressed data, was "dotbot_firefox-1.1.0.tar", max compression
```

## Comparing `dotbot-firefox-1.0.1.tar` & `dotbot_firefox-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     3017 2022-10-09 01:15:46.028647 dotbot-firefox-1.0.1/dotbot_firefox.py
--rw-r--r--   0        0        0     1089 2022-09-26 13:38:12.956138 dotbot-firefox-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1073 2022-10-09 01:15:46.029645 dotbot-firefox-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5726 2022-10-08 21:38:12.100184 dotbot-firefox-1.0.1/README.rst
--rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 dotbot-firefox-1.0.1/setup.py
--rw-r--r--   0        0        0     6439 1970-01-01 00:00:00.000000 dotbot-firefox-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3721 2023-05-23 13:34:38.829122 dotbot_firefox-1.1.0/dotbot_firefox.py
+-rw-r--r--   0        0        0     1094 2023-05-23 13:33:04.675300 dotbot_firefox-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1233 2023-05-23 13:34:38.829122 dotbot_firefox-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5827 2023-05-23 13:33:04.675300 dotbot_firefox-1.1.0/README.rst
+-rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 dotbot_firefox-1.1.0/PKG-INFO
```

### Comparing `dotbot-firefox-1.0.1/dotbot_firefox.py` & `dotbot_firefox-1.1.0/dotbot_firefox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # dotbot-firefox -- Configure your Firefox profile(s) using dotbot.
-# Copyright 2022 Kurt McKee <contactme@kurtmckee.org>
+# Copyright 2022-2023 Kurt McKee <contactme@kurtmckee.org>
 # SPDX-License-Identifier: MIT
 
 
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
 import sys
 import typing
 
 import dotbot.plugin
 import dotbot.plugins.link
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 VALID_DIRECTIVES: set[str] = {"firefox"}
 
 log = logging.getLogger(__name__)
 
 
 def _get_profile_directories() -> typing.Iterable[pathlib.Path]:
@@ -42,25 +42,42 @@
         #     snap run --shell firefox -c 'echo $SNAP_USER_COMMON'
         #
         # ...but that seems unnecessary, and may be fragile and insecure.
         #
         snap_user_common = "~/snap/firefox/common"
         defaults.append(f"{snap_user_common}/.mozilla/firefox")
 
+        # When Firefox is installed and run as a flatpak,
+        # it stores its profile info under this directory:
+        #
+        #     $HOME/.var/app/org.mozilla.firefox
+        #
+        # $HOME can be customized inside the flatpak sandbox environment,
+        # but it seems unlikely that this level of customization will be needed.
+        #
+        flatpak_home = "~/.var/app/org.mozilla.firefox"
+        defaults.append(f"{flatpak_home}/.mozilla/firefox")
+
     for default in defaults:
         path = pathlib.Path(os.path.expandvars(os.path.expanduser(default)))
         if not path.is_dir():
             continue
 
         for profile in path.glob("*"):
             if profile.is_dir() and (profile / "prefs.js").is_file():
                 yield profile
 
 
-class Firefox(dotbot.plugin.Plugin):
+# mypy 1.3.0 reports the following error for the Firefox class:
+#
+#   Class cannot subclass "Plugin" (has type "Any")  [misc]
+#
+# The "type: ignore[misc]" comment below suppresses this specific error.
+#
+class Firefox(dotbot.plugin.Plugin):  # type: ignore[misc]
     def can_handle(self, directive: str) -> bool:
         """
         Flag whether this plugin supports the given *directive*.
         """
 
         return directive in VALID_DIRECTIVES
 
@@ -91,8 +108,8 @@
             str(profile / "user.js"): value for profile in _get_profile_directories()
         }
 
         if not links:
             log.warning("No Firefox profiles found")
             return True
 
-        return link_plugin.handle("link", links)
+        return bool(link_plugin.handle("link", links))
```

### Comparing `dotbot-firefox-1.0.1/LICENSE.txt` & `dotbot_firefox-1.1.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright 2022 Kurt McKee <contactme@kurtmckee.org>
+Copyright 2022-2023 Kurt McKee <contactme@kurtmckee.org>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dotbot-firefox-1.0.1/pyproject.toml` & `dotbot_firefox-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 [tool.poetry]
 name = "dotbot-firefox"
-version = "1.0.1"
+version = "1.1.0"
 description = "Configure your Firefox profile(s) using dotbot"
 authors = ["Kurt McKee <contactme@kurtmckee.org>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/kurtmckee/dotbot-firefox"
 keywords = ["dotbot", "dotbot-plugin", "firefox", "dotfiles"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-dotbot = "^1.19.0"
+python = ">=3.8"
+dotbot = ">=1.19.0"
 
 [tool.poetry.group.dev.dependencies]
-tox = "^3.26.0"
-pytest = "^7.1.3"
-pre-commit = "^2.20.0"
-scriv = {extras = ["toml"], version = "^0.17.0"}
+scriv = {extras = ["toml"], version = ">=1.2.0"}
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 branch = true
 parallel = true
+data_file = ".tox/.coverage-data-files/.coverage"
 source = [
     "dotbot_firefox",
     "tests",
 ]
 
 [tool.coverage.paths]
 source = [
     "src",
     "*/site-packages",
 ]
 
 [tool.coverage.report]
 fail_under = 100
 
+[tool.mypy]
+packages = "dotbot_firefox"
+strict = true
+sqlite_cache = true
+
 [[tool.mypy.overrides]]
 module = [
     "dotbot.*",
     "pytest",
 ]
 ignore_missing_imports = true
 
 [tool.scriv]
 version = "literal: pyproject.toml: tool.poetry.version"
 categories = [
+    "Python support",
     "Added",
     "Removed",
     "Changed",
     "Fixed",
 ]
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+]
```

### Comparing `dotbot-firefox-1.0.1/README.rst` & `dotbot_firefox-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..  dotbot-firefox -- Configure your Firefox profile(s) using dotbot.
-..  Copyright 2022 Kurt McKee <contactme@kurtmckee.org>
+..  Copyright 2022-2023 Kurt McKee <contactme@kurtmckee.org>
 ..  SPDX-License-Identifier: MIT
 
 
 dotbot-firefox
 ##############
 
 Configure your Firefox profile(s) using `dotbot`_.
@@ -161,14 +161,15 @@
 
 The dotbot-firefox plugin is aware of the following default directories:
 
 *   ``%APPDATA%\Mozilla\Firefox\Profiles`` (Windows)
 *   ``~/Library/Application Support/Firefox/Profiles`` (Mac OS)
 *   ``~/.mozilla/firefox`` (Linux)
 *   ``~/snap/firefox/common/.mozilla/firefox`` (Firefox Snap for Linux)
+*   ``~/.var/app/org.mozilla.firefox/.mozilla/firefox`` (Firefox Flatpak for Linux)
 
 Only profile subdirectories that contain a ``prefs.js`` file
 will be considered valid by the plugin.
 
 
 Development
 ===========
@@ -186,16 +187,16 @@
 
     # Activate the virtual environment (Windows)
     $ & .venv/Scripts/Activate.ps1
 
     # Update pip and setuptools, and install wheel
     (.venv) $ pip install -U pip setuptools wheel
 
-    # Install poetry
-    (.venv) $ pip install poetry
+    # Install poetry and tox
+    (.venv) $ pip install poetry tox
 
     # Install all dependencies
     (.venv) $ poetry install
 
     # Run the unit tests locally
     (.venv) $ tox
```

### Comparing `dotbot-firefox-1.0.1/PKG-INFO` & `dotbot_firefox-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: dotbot-firefox
-Version: 1.0.1
+Version: 1.1.0
 Summary: Configure your Firefox profile(s) using dotbot
 Home-page: https://github.com/kurtmckee/dotbot-firefox
 License: MIT
 Keywords: dotbot,dotbot-plugin,firefox,dotfiles
 Author: Kurt McKee
 Author-email: contactme@kurtmckee.org
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: dotbot (>=1.19.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dotbot (>=1.19.0)
 Project-URL: Repository, https://github.com/kurtmckee/dotbot-firefox
 Description-Content-Type: text/x-rst
 
 ..  dotbot-firefox -- Configure your Firefox profile(s) using dotbot.
-..  Copyright 2022 Kurt McKee <contactme@kurtmckee.org>
+..  Copyright 2022-2023 Kurt McKee <contactme@kurtmckee.org>
 ..  SPDX-License-Identifier: MIT
 
 
 dotbot-firefox
 ##############
 
 Configure your Firefox profile(s) using `dotbot`_.
@@ -180,14 +181,15 @@
 
 The dotbot-firefox plugin is aware of the following default directories:
 
 *   ``%APPDATA%\Mozilla\Firefox\Profiles`` (Windows)
 *   ``~/Library/Application Support/Firefox/Profiles`` (Mac OS)
 *   ``~/.mozilla/firefox`` (Linux)
 *   ``~/snap/firefox/common/.mozilla/firefox`` (Firefox Snap for Linux)
+*   ``~/.var/app/org.mozilla.firefox/.mozilla/firefox`` (Firefox Flatpak for Linux)
 
 Only profile subdirectories that contain a ``prefs.js`` file
 will be considered valid by the plugin.
 
 
 Development
 ===========
@@ -205,16 +207,16 @@
 
     # Activate the virtual environment (Windows)
     $ & .venv/Scripts/Activate.ps1
 
     # Update pip and setuptools, and install wheel
     (.venv) $ pip install -U pip setuptools wheel
 
-    # Install poetry
-    (.venv) $ pip install poetry
+    # Install poetry and tox
+    (.venv) $ pip install poetry tox
 
     # Install all dependencies
     (.venv) $ poetry install
 
     # Run the unit tests locally
     (.venv) $ tox
```

