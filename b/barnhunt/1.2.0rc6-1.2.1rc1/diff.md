# Comparing `tmp/barnhunt-1.2.0rc6.tar.gz` & `tmp/barnhunt-1.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barnhunt-1.2.0rc6.tar", last modified: Thu Apr 27 17:34:20 2023, max compression
+gzip compressed data, was "barnhunt-1.2.1rc1.tar", last modified: Tue May 23 03:12:11 2023, max compression
```

## Comparing `barnhunt-1.2.0rc6.tar` & `barnhunt-1.2.1rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    14281 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/CHANGES.md
--rw-r--r--   0        0        0    32528 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/LICENSE
--rw-r--r--   0        0        0     3179 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/README.md
--rw-r--r--   0        0        0       61 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/__init__.py
--rw-r--r--   0        0        0       61 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/__main__.py
--rw-r--r--   0        0        0      360 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/_compat.py
--rw-r--r--   0        0        0       22 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/_version.py
--rw-r--r--   0        0        0    15274 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/cli.py
--rw-r--r--   0        0        0     8946 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/coursemaps.py
--rw-r--r--   0        0        0        0 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/__init__.py
--rw-r--r--   0        0        0     3022 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/css.py
--rw-r--r--   0        0        0    11435 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/runner.py
--rw-r--r--   0        0        0    11100 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/svg.py
--rw-r--r--   0        0        0     2565 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/utils.py
--rw-r--r--   0        0        0     8378 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/installer/__init__.py
--rw-r--r--   0        0        0     2101 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/installer/github.py
--rw-r--r--   0        0        0     4612 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/installer/metadata.py
--rw-r--r--   0        0        0     4717 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/layerinfo.py
--rw-r--r--   0        0        0     4252 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/pager.py
--rw-r--r--   0        0        0     3843 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/pdfutil.py
--rw-r--r--   0        0        0     7769 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/templating.py
--rw-r--r--   0        0        0     3882 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/pdm_build.py
--rw-r--r--   0        0        0    10037 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/pyoxidizer/pyoxidizer.bzl
--rw-r--r--   0        0        0    21401 2023-04-27 17:34:20.579693 barnhunt-1.2.0rc6/pyproject.toml
--rw-r--r--   0        0        0       35 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/__init__.pyi
--rw-r--r--   0        0        0      205 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/exceptions.pyi
--rw-r--r--   0        0        0     1774 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/popen_spawn.pyi
--rw-r--r--   0        0        0     5501 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/spawnbase.pyi
--rw-r--r--   0        0        0     1033 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/conftest.py
--rw-r--r--   0        0        0     4089 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/drawing.svg
--rw-r--r--   0        0        0      558 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/dummy_inkscape.py
--rw-r--r--   0        0        0     2221 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_css.py
--rw-r--r--   0        0        0     7259 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_runner.py
--rw-r--r--   0        0        0     1899 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_shell_mode_integration.py
--rw-r--r--   0        0        0    10830 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_svg.py
--rw-r--r--   0        0        0     4259 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_utils.py
--rw-r--r--   0        0        0      887 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/ratelimit.py
--rw-r--r--   0        0        0      627 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/test_github.py
--rw-r--r--   0        0        0    11880 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/test_installer.py
--rw-r--r--   0        0        0     3457 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/test_metadata.py
--rw-r--r--   0        0        0     4052 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test1.pdf
--rw-r--r--   0        0        0     4098 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test2.pdf
--rw-r--r--   0        0        0     6922 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_cli.py
--rw-r--r--   0        0        0     8719 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_coursemaps.py
--rw-r--r--   0        0        0     3366 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_functional.py
--rw-r--r--   0        0        0     5833 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_layerinfo.py
--rw-r--r--   0        0        0      350 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_main.py
--rw-r--r--   0        0        0     3616 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_pager.py
--rw-r--r--   0        0        0     3998 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_pdfutil.py
--rw-r--r--   0        0        0     9120 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_templating.py
--rw-r--r--   0        0        0     2780 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/testlib.py
--rw-r--r--   0        0        0     1544 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tox.ini
--rw-r--r--   0        0        0    18572 1970-01-01 00:00:00.000000 barnhunt-1.2.0rc6/PKG-INFO
+-rw-r--r--   0        0        0    15578 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/CHANGES.md
+-rw-r--r--   0        0        0    32528 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/LICENSE
+-rw-r--r--   0        0        0     4615 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/README.md
+-rw-r--r--   0        0        0       61 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/__init__.py
+-rw-r--r--   0        0        0      269 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/__main__.py
+-rw-r--r--   0        0        0      585 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/_compat.py
+-rw-r--r--   0        0        0       22 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/_version.py
+-rw-r--r--   0        0        0    18454 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/cli.py
+-rw-r--r--   0        0        0     8946 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/coursemaps.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/__init__.py
+-rw-r--r--   0        0        0     3022 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/css.py
+-rw-r--r--   0        0        0    12227 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/runner.py
+-rw-r--r--   0        0        0    11100 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/svg.py
+-rw-r--r--   0        0        0     3699 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/inkscape/utils.py
+-rw-r--r--   0        0        0     8378 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/installer/__init__.py
+-rw-r--r--   0        0        0     2101 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/installer/github.py
+-rw-r--r--   0        0        0     4612 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/installer/metadata.py
+-rw-r--r--   0        0        0     4717 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/layerinfo.py
+-rw-r--r--   0        0        0     4252 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/pager.py
+-rw-r--r--   0        0        0     3843 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/pdfutil.py
+-rw-r--r--   0        0        0     7769 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/barnhunt/templating.py
+-rw-r--r--   0        0        0     3882 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/pdm_build.py
+-rw-r--r--   0        0        0     9885 2023-05-23 03:12:01.235781 barnhunt-1.2.1rc1/pyoxidizer/pyoxidizer.bzl
+-rw-r--r--   0        0        0    24251 2023-05-23 03:12:11.768145 barnhunt-1.2.1rc1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/__init__.pyi
+-rw-r--r--   0        0        0      205 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/exceptions.pyi
+-rw-r--r--   0        0        0     1774 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/popen_spawn.pyi
+-rw-r--r--   0        0        0     5501 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/stubs/pexpect/spawnbase.pyi
+-rw-r--r--   0        0        0     1053 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0     4089 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/drawing.svg
+-rw-r--r--   0        0        0      558 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/dummy_inkscape.py
+-rw-r--r--   0        0        0     2221 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_css.py
+-rw-r--r--   0        0        0     8129 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_runner.py
+-rw-r--r--   0        0        0     1899 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_shell_mode_integration.py
+-rw-r--r--   0        0        0    10830 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_svg.py
+-rw-r--r--   0        0        0     5702 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/inkscape/test_utils.py
+-rw-r--r--   0        0        0      887 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/ratelimit.py
+-rw-r--r--   0        0        0      627 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/test_github.py
+-rw-r--r--   0        0        0    11880 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/test_installer.py
+-rw-r--r--   0        0        0     3457 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/installer/test_metadata.py
+-rw-r--r--   0        0        0     4052 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test1.pdf
+-rw-r--r--   0        0        0     4098 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test2.pdf
+-rw-r--r--   0        0        0     6695 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_cli.py
+-rw-r--r--   0        0        0     8719 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_coursemaps.py
+-rw-r--r--   0        0        0     3366 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_functional.py
+-rw-r--r--   0        0        0     5833 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_layerinfo.py
+-rw-r--r--   0        0        0      350 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_main.py
+-rw-r--r--   0        0        0     3616 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_pager.py
+-rw-r--r--   0        0        0     3998 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_pdfutil.py
+-rw-r--r--   0        0        0     9120 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/test_templating.py
+-rw-r--r--   0        0        0     2780 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tests/testlib.py
+-rw-r--r--   0        0        0     1544 2023-05-23 03:12:01.239781 barnhunt-1.2.1rc1/tox.ini
+-rw-r--r--   0        0        0    21367 1970-01-01 00:00:00.000000 barnhunt-1.2.1rc1/PKG-INFO
```

### Comparing `barnhunt-1.2.0rc6/CHANGES.md` & `barnhunt-1.2.1rc1/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,40 @@
 ## Changes
 
+### Release 1.2.1rc1 (2023-05-22)
+
+(There was no final release of 1.2.0. It is a long story. I mistakenly
+committed a couple of files to LFS. To clear out LFS storage for a
+GitHub repo, one has to [delete the whole repo](😬). As a result, the
+workflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump
+is required to keep those PyOxidizer windows build version numbers —
+`<major>.<minor>.<micro>.<run-number>` — monotonic.)
+
+[delete the whole repo]: https://docs.github.com/en/repositories/working-with-files/managing-large-files/removing-files-from-git-large-file-storage#git-lfs-objects-in-your-repository
+
+#### CLI Changes
+
+- The `--inkscape-command`, `--processes` and `--shell-mode-inkscape`
+  options have been moved from the `barnhunt pdfs` subcommand to the
+  man `barnhunt` command group.
+
+- And new `debug-info` subcommand has been added to display various
+  information about the installed version of the `barnhunt` command
+  and its execution environment.
+
+- The `--dump-loaded-modules` option has been removed.  The
+  functionality is still available by setting the
+  `$BARNHUNT_DUMP_LOADED_MODULES` environment variable to a non-empty
+  value.
+
+#### Bugs Fixed
+
+- Fixed exception in `barnhunt.cli.default_2up_output_file` during
+  shell-completion for `barnhunt 2up`.
+
 ### Release 1.2.0rc6 (2023-04-27)
 
 - Build an Windows executable and installer using [PyOxidizer].  The
   .msi installer should be downloadable from the
   [Releases](https://github.com/barnhunt/barnhunt/releases) page.
 
 - Added a `--dump-loaded-modules` option which causes `barnhunt` to
```

### Comparing `barnhunt-1.2.0rc6/LICENSE` & `barnhunt-1.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/README.md` & `barnhunt-1.2.1rc1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Barn Hunt Map Helper
 
-[![Tests](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml/badge.svg)](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml)
-[![PyPI Version](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)
-[![Inkscape Versions](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2-blue.svg?logo=inkscape)](https://inkscape.org/)
-[![PyPI Status](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Test status badge](https://img.shields.io/github/actions/workflow/status/barnhunt/barnhunt/ci.yml?label=tests)](https://github.com/barnhunt/barnhunt/actions/workflows/ci.yml)
+[![Latest version badge](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Supported Python versions badge](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Supported Inkscape versions badge](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2.2-blue.svg?logo=inkscape)](https://inkscape.org/)
+[![Development status badge](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Trackgit-views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhapwefdbvler7yp5dsl)](https://trackgit.com)
 
 This is a helper script Jeff uses for drafting [Barn Hunt][] course
 maps.
 
 It does a bunch of stuff, but the important bit is that it exports PDF
 versions of maps from [Inkscape][] SVG files.
 
@@ -31,16 +32,45 @@
 (Due to a dependency on the [pikepdf][] package, it should work on
 x86_64-based Macs, but may not work on Macs that use Apple silicon. If
 pikepdf compatibility is an issue for you, let me know — it’s probably
 fixable.)
 
 ## Installation
 
+### Windows
+
+We now publish a compiled version of the program for Windows (which may
+even work.) Using this version has the advantage that Python is not required
+to be installed. (And even if Python is installed, this version may work-around
+some bugs having to do with the various different ways that Python can be
+installed on on Windows computer.)
+
+1. Browse to our [releases](https://github.com/barnhunt/barnhunt/releases/)
+   page. Select a release, and look down in the *Assets* section of the
+   release page. (You may have to click the triangle to expand the
+   *Assets* section.)
+
+2. Download the MSI installer (the filename should end with `.msi` —
+   e.g. `Barnhunt-1.2.0.49-x86_64-pc-windows-msvc.msi`). The file
+   is not signed, so you may have to click through some nasty warnings
+   about "unrecognized, potentially dangerous" files.
+
+3. Once downloaded, open (double-click) the file you just
+   downloaded. Hopefully and installer dialog should open.  Accept the
+   default choices.
+
+4. Now open a terminal command-line window. Type `barnhunt
+   --version`. If all is good, barnhunt should report its version. Run
+   `barnhunt --help` for the help screen.
+
+
+### Linux (or Windows with Python installed)
+
 As this package is published to
-[PyPI](https://pypi.org/project/barnhunt/) in may be installed into a
+[PyPI](https://pypi.org/project/barnhunt/) it may be installed into a
 [_virtualenv_][venv] using [`pip`][pip]. It is suggested that you use
 [`pipx`][pipx] to combine those two steps.
 
 A basic outline of how to proceed:
 
 1. Install [python][] if it is not already installed.  (Version 3.7 or
    greater is required.)
```

### Comparing `barnhunt-1.2.0rc6/barnhunt/cli.py` & `barnhunt-1.2.1rc1/barnhunt/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from __future__ import annotations
 
-import atexit
 import datetime
 import logging
 import os
 import random
+import re
 import sys
 from collections import defaultdict
 from contextlib import ExitStack
-from functools import partial
 from itertools import count
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Any
 from typing import BinaryIO
 from typing import Callable
 from typing import Iterable
+from typing import NoReturn
 from typing import Sequence
 from typing import TypeVar
 
 import click
 from atomicwrites import atomic_write
 
 import barnhunt
+from ._compat import Final
+from ._compat import importlib_metadata as metadata
 from .coursemaps import Coursemap
 from .coursemaps import iter_coursemaps
+from .inkscape.runner import DEFAULT_INKSCAPE_COMMAND
+from .inkscape.runner import DEFAULT_SHELL_MODE
 from .inkscape.runner import inkscape_runner
+from .inkscape.utils import get_inkscape_debug_info
 from .inkscape.utils import get_user_data_directory
 from .installer import DEFAULT_REQUIREMENTS
 from .installer import InkexRequirement
 from .installer import Installer
 from .pager import get_pager
 from .pdfutil import concat_pdfs
 from .pdfutil import two_up
@@ -39,49 +43,85 @@
 _U = TypeVar("_U")
 
 log = logging.getLogger("")
 
 POSITIVE_INT = click.IntRange(1, None)
 
 
-def _dump_loaded_modules() -> None:
-    utcnow = datetime.datetime.utcnow()
-    dump_file = f"barnhunt-modules.{os.getpid()}"
-    with open(dump_file, "w") as fp:
-        print(f"# Modules loaded by barnhunt {barnhunt.__version__}", file=fp)
-        print(f"# {utcnow.isoformat(timespec='seconds')}Z", file=fp)
-        print(f"# Command: {' '.join(sys.argv[1:])}", file=fp)
-        for name in sorted(sys.modules):
-            print(name, file=fp)
-    log.warning("Dumped loaded modules to %r", dump_file)
+DEFAULT_PROCESSES: Final = os.cpu_count() or 1
+
+
+class ContextObj:
+    inkscape_command: str = DEFAULT_INKSCAPE_COMMAND
+    shell_mode: bool = DEFAULT_SHELL_MODE
+    processes: int = DEFAULT_PROCESSES
 
 
-@click.group()
+@click.group("barnhunt")
 @click.option("-v", "--verbose", count=True)
+@click.version_option(version=barnhunt.__version__)
 @click.option(
-    "--dump-loaded-modules/--no-dump-loaded-modules",
-    envvar="BARNHUNT_DUMP_LOADED_MODULES",
-    default=False,
-    help=(
-        "Write a list of loaded modules to barnhunt-modes.<pid> after "
-        "command completion. (This can also be controlled by setting "
-        "the $BARNHUNT_DUMP_LOADED_MODULES environment variable.)"
-    ),
+    "--inkscape-command",
+    "--inkscape",
+    metavar="COMMAND",
+    envvar="INKSCAPE_COMMAND",  # NB: this is what inkex uses
+    default=DEFAULT_INKSCAPE_COMMAND,
+    help=f"""
+    Name of (or path to) inkscape executable to use for exporting PDFs and for
+    determining the location of the user profile directory.
+    (Equivalently, you may set the $INKSCAPE_COMMAND environment variable.)
+    The default is {DEFAULT_INKSCAPE_COMMAND!r}.
+    """,
 )
-@click.version_option(version=barnhunt.__version__)
-def barnhunt_cli(verbose: int, dump_loaded_modules: bool) -> None:
+@click.option(
+    "--processes",
+    "-p",
+    metavar="N",
+    type=POSITIVE_INT,
+    default=DEFAULT_PROCESSES,
+    envvar="BARNHUNT_PROCESSES",
+    help=f"""
+    Number of inkscape processes to run in parallel.
+    Set to one to disable parallel processing.
+    The default is {DEFAULT_PROCESSES} (the number of CPUs detected on this platform).
+    (This option may be set via the $BARNHUNT_PROCESSES environment variable.)
+    """,
+)
+@click.option(
+    "--shell-mode-inkscape/--no-shell-mode-inkscape",
+    "shell_mode",
+    default=DEFAULT_SHELL_MODE,
+    envvar="BARNHUNT_SHELL_MODE_INKSCAPE",
+    help=f"""
+    Enable/disable running inkscape in shell-mode for efficiency.
+    The default is to {"use" if DEFAULT_SHELL_MODE else "disable"}
+    shell-mode.
+    (This option may be set via the $BARNHUNT_SHELL_MODE_INKSCAPE environment variable.)
+    """,
+)
+@click.pass_context
+def barnhunt_cli(
+    ctx: click.Context,
+    verbose: int,
+    inkscape_command: str | None,
+    shell_mode: bool | None,
+    processes: int | None,
+) -> None:
     """Utilities for creating Barn Hunt course maps."""
+    ctx.ensure_object(ContextObj)
+    ctx.obj.inkscape_command = inkscape_command
+    ctx.obj.shell_mode = shell_mode
+    ctx.obj.processes = processes
+
     log_level = logging.WARNING
     if verbose:  # pragma: NO COVER
         log_level = logging.DEBUG if verbose > 1 else logging.INFO
     logging.basicConfig(
         level=log_level, format="(%(levelname)1.1s) [%(threadName)s] %(message)s"
     )
-    if dump_loaded_modules:
-        atexit.register(_dump_loaded_modules)  # pragma: no cover
 
 
 @barnhunt_cli.command()
 @click.argument(
     "svgfiles",
     type=click.Path(exists=True, dir_okay=False, writable=True),
     nargs=-1,
@@ -117,92 +157,37 @@
         random_seed = random.randrange(2**128)
         log.debug("%s: setting random seed to %d", svgpath, random_seed)
         svg.set_random_seed(tree, random_seed)
         with atomic_write(svgpath, mode="wb", overwrite=True) as f:
             tree.write(f)
 
 
-def default_inkscape_command() -> str:
-    # This is what inkex.command does to find Inkscape (after first
-    # checking $INKSCAPE_COMMAND).
-    #
-    # https://gitlab.com/inkscape/extensions/-/blob/cb74374e46894030775cf947e97ca341b6ed85d8/inkex/command.py#L45
-    if sys.platform == "win32":
-        # prefer inkscape.exe over inkscape.com which spawns a command window
-        return "inkscape.exe"
-    return "inkscape"
-
-
-def inkscape_command_option(**kwargs: Any) -> Callable[..., Any]:
-    return click.option(
-        "--inkscape-command",
-        "--inkscape",
-        metavar="COMMAND",
-        envvar="INKSCAPE_COMMAND",  # NB: this is what inkex uses
-        default=default_inkscape_command,
-        help=f"""
-        Name of (or path to) inkscape executable to use for exporting PDFs and for
-        determining the location of the user profile directory.
-        (Equivalently, you may set the $INKSCAPE_COMMAND environment variable.)
-        The default is {default_inkscape_command()!r}.
-        """,
-        **kwargs,
-    )
-
-
-def default_shell_mode() -> bool:
-    """Whether to use Inkscape's shell-mode by default."""
-    if sys.platform == "darwin":
-        return False  # ShellModeRunner current borked
-    return True
-
-
 @barnhunt_cli.command()
 @click.argument("svgfiles", type=click.File("rb"), nargs=-1, required=True)
 @click.option(
     "--output-directory",
     "-o",
     type=click.Path(file_okay=False),
     default="pdfs",
     help="""
     Directory into which to write output PDF files.
     The default is './pdfs'.
     """,
 )
-@click.option(
-    "--processes",
-    "-p",
-    metavar="N",
-    type=POSITIVE_INT,
-    default=os.cpu_count,
-    help="""
-    Number of inkscape processes to run in parallel.
-    Set to one to disable parallel processing.
-    The default is {os.cpu_count()} (the number of CPUs detected on this platform).
-    """,
-)
-@inkscape_command_option()
-@click.option(
-    "--shell-mode-inkscape/--no-shell-mode-inkscape",
-    "shell_mode",
-    default=default_shell_mode,
-    help="""
-    Enable/disable running inkscape in shell-mode for efficiency.
-    The default is enabled (except on macOS, where shell-mode currently
-    seems to be broken).
-    """,
-)
+@click.pass_context
 def pdfs(
+    ctx: click.Context,
     svgfiles: Iterable[BinaryIO],
     output_directory: str,
-    shell_mode: bool,
-    inkscape_command: str,
-    processes: int,
 ) -> None:
     """Export PDFs from inkscape SVG coursemaps."""
+    inkscape_command = ctx.obj.inkscape_command
+    shell_mode = ctx.obj.shell_mode
+    processes = ctx.obj.processes
+
     counter = count(1)
 
     with ExitStack() as stack:
         tmpdir = stack.enter_context(TemporaryDirectory())
         inkscape = stack.enter_context(
             inkscape_runner(shell_mode=shell_mode, executable=inkscape_command)
         )
@@ -317,25 +302,28 @@
         [
             "{0[0]:3d},{0[1]:3d}".format(coord(pt))
             for pt in random.sample(range(n_pts), number_of_rows)
         ]
     )
 
 
-def default_2up_output_file() -> Path:
+def default_2up_output_file() -> Path | None:
     """Compute default output filename."""
     ctx = click.get_current_context()
-    input_paths = {Path(infp.name) for infp in ctx.params.get("pdffiles", ())}
-    if len(input_paths) != 1:
+    pdffiles = ctx.params.get("pdffiles")
+    if ctx.resilient_parsing:
+        return None
+    assert isinstance(pdffiles, Sequence)
+    if len(pdffiles) != 1:
         raise click.UsageError(
             "Can not deduce default output filename when multiple input "
             "files are specified.",
             ctx=ctx,
         )
-    input_path = input_paths.pop()
+    input_path = Path(pdffiles[0].name)
     output_path = input_path.with_name(input_path.stem + "-2up" + input_path.suffix)
     click.echo(f"Writing output to {output_path!s}")
     return output_path
 
 
 @barnhunt_cli.command(name="2up")
 @click.argument("pdffiles", type=click.File("rb"), nargs=-1, required=True)
@@ -380,52 +368,44 @@
             if value.specifier:
                 self.fail("specifiers not allowed in requirement")
             if value.url:
                 self.fail("direct reference (URL) not allowed in requirement")
         return value
 
 
+def get_default_target() -> Path:
+    ctx = click.get_current_context()
+    return get_user_data_directory(ctx.obj.inkscape_command)
+
+
 target_option = click.option(
     "--target",
     type=click.Path(exists=True, file_okay=False, writable=True, path_type=Path),
     envvar="INKSCAPE_PROFILE_DIR",
     help="""
     Where to install distributions.
     Defaults to inkscape’s user data directory, e.g. $XDG_CONFIG_HOME/inkscape, or
     %APPDATA%\\inkscape on Windows.  This may also be set by setting the
     $INKSCAPE_PROFILE_DIR environment variable.""",
+    default=get_default_target,
 )
 
 
-def set_default_target(
-    ctx: click.Context, param: click.Parameter, inkscape_command: str
-) -> str:
-    if ctx.default_map is None:
-        ctx.default_map = {}
-    ctx.default_map["target"] = partial(get_user_data_directory, inkscape_command)
-    return inkscape_command
-
-
 @barnhunt_cli.command()
 @click.argument(
     "requirements",
     type=InkexRequirementType(),
     nargs=-1,
 )
 @click.option(
     "--upgrade/--no-upgrade", "-U", help="Upgrade to the newest available versions."
 )
 @click.option("--pre/--no-pre", help="Include pre-release and development versions.")
 @click.option("-n", "--dry-run/--no-dry-run", help="Just show what would be done.")
 @target_option
-@inkscape_command_option(
-    is_eager=True,
-    expose_value=False,
-    callback=set_default_target,
-)
 @click.option(
     "--github-token",
     envvar="GITHUB_TOKEN",
     help=""" Token to use for authentication to GitHub’s REST API.
     This is not typically necessary, but if you are seeing rate-limit errors, using a
     GitHub “Personal Access Token” here (it does not need to be granted access to any
     scopes) greatly increases the rate-limit thresholds.  The token may also be passed
@@ -450,28 +430,144 @@
 @click.argument(
     "requirements",
     type=InkexRequirementType(allow_specifiers=False),
     nargs=-1,
 )
 @click.option("-n", "--dry-run/--no-dry-run", help="Just show what would be done.")
 @target_option
-@inkscape_command_option(
-    is_eager=True,
-    expose_value=False,
-    callback=set_default_target,
-)
 def uninstall(
     target: Path,
     dry_run: bool,
     requirements: Sequence[InkexRequirement],
 ) -> None:
     """Uninstall extensions and/or symbol sets."""
     installer = Installer(target, dry_run=dry_run)
     for requirement in requirements or DEFAULT_REQUIREMENTS:
         installer.uninstall(requirement)
 
 
-def main(args: Sequence[str] | None = None) -> None:
-    prog_name = None  # by default let click figure out program name
-    if sys.argv[0] == "-c":
-        prog_name = "barnhunt"  # pragma: no cover
-    barnhunt_cli(args, prog_name=prog_name)
+@click.option("--command-info", is_flag=True, help="Show information about the command")
+@click.option("--inkscape-info", is_flag=True, help="Show information about Inkscape")
+@click.option("--system-info", is_flag=True, help="Show information about Python")
+@click.option("--package-info", is_flag=True, help="Show installed python packages")
+@barnhunt_cli.command()
+@click.pass_context
+def debug_info(
+    ctx: click.Context,
+    command_info: bool,
+    inkscape_info: bool,
+    system_info: bool,
+    package_info: bool,
+) -> None:
+    """Show debugging information.
+
+    This command display a compendium of information about the program and
+    the environment it is running in. The output of this command may help
+    in diagnosing the causes of failures or other problems.
+
+
+    Note: Setting the $BARNHUNT_DUMP_LOADED_MODULES environment variable to a non-empty
+    value will cause the program to write a list of loaded modules to a file in the
+    current working directory named "barnhunt-modes.<pid>".
+
+    """
+    inkscape_command = ctx.obj.inkscape_command
+    formatter = ctx.make_formatter()
+
+    if not (command_info or inkscape_info or system_info or package_info):
+        command_info = inkscape_info = system_info = package_info = True
+
+    def nl2br(info: Sequence[tuple[str, str]]) -> list[tuple[str, str]]:
+        return [(term, defn.replace("\n", "\n\n@")) for term, defn in info]
+
+    if command_info:
+        with formatter.section("Barnhunt"):
+            formatter.write_dl(
+                [
+                    ("version", barnhunt.__version__),
+                    ("inkscape-shell-mode", repr(ctx.obj.shell_mode)),
+                    ("processors", str(ctx.obj.processes)),
+                ]
+            )
+
+    if inkscape_info:
+        with formatter.section("Inkscape"):
+            formatter.write_dl(nl2br(get_inkscape_debug_info(inkscape_command)), 0)
+
+    if system_info:
+        with formatter.section("Python Information"):
+            formatter.write_dl(nl2br(_get_system_debug_info()), 0)
+
+    if package_info:
+        with formatter.section("Installed Python Distributions"):
+            formatter.write_dl(_get_package_debug_info(), 22)
+
+    print(re.sub(r"\n\s*(\n\s*)@", r"\1", formatter.getvalue().strip()))
+
+
+def _get_package_debug_info() -> list[tuple[str, str]]:
+    return [
+        (dist.name, dist.version)
+        for dist in sorted(metadata.distributions(), key=lambda d: d.name.lower())
+    ]
+
+
+def _get_system_debug_info() -> list[tuple[str, str]]:
+    debug_items = [
+        "sys.executable",
+        "sys.version",
+        "sys.version_info",
+        "sys.platform",
+        "os.name",
+        "os.uname()",
+        "sys.implementation.name",
+        "sys.implementation.cache_tag",
+        "sys.implementation._multiarch",
+        "sys.api_version",
+        "sys.getdefaultencoding()",
+        "sys.getfilesystemencoding()",
+        "sys.windowsversion",
+        "sys.winver",
+        "sys.argv",
+        "sys.path",
+        "os.get_exec_path()",
+    ]
+
+    def get_value(item: str) -> str:
+        try:
+            value = eval(item, globals(), {})
+        except Exception:
+            return ""
+        if isinstance(value, list):
+            # sys.path
+            return "\n".join(map(repr, value))
+        if isinstance(value, tuple):
+            value = tuple(value)  # get rid of namedtuple names
+        return repr(value)
+
+    return [(item, get_value(item)) for item in debug_items]
+
+
+def main(args: Sequence[str] | None = None, prog_name: str | None = None) -> NoReturn:
+    try:
+        barnhunt_cli.main(args=args, prog_name=prog_name)
+    finally:
+        if os.environ.get("BARNHUNT_DUMP_LOADED_MODULES"):
+            _dump_loaded_modules()
+
+
+def _dump_loaded_modules() -> None:
+    utcnow = datetime.datetime.utcnow()
+    dump_file = f"barnhunt-modules.{os.getpid()}"
+    with open(dump_file, "w") as fp:
+        print(f"# Modules loaded by barnhunt {barnhunt.__version__}", file=fp)
+        print(f"# {utcnow.isoformat(timespec='seconds')}Z", file=fp)
+        print(f"# Command: {' '.join(sys.argv[1:])}", file=fp)
+        for name in sorted(sys.modules):
+            print(name, file=fp)
+
+    formatter = click.HelpFormatter()
+    formatter.write_text(
+        f"Dumped loaded modules to {dump_file!r} "
+        "(Unset $BARNHUNT_DUMP_LOADED_MODULES to prevent this.)"
+    )
+    print("\n" + formatter.getvalue().rstrip(), file=sys.stderr)
```

### Comparing `barnhunt-1.2.0rc6/barnhunt/coursemaps.py` & `barnhunt-1.2.1rc1/barnhunt/coursemaps.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/inkscape/css.py` & `barnhunt-1.2.1rc1/barnhunt/inkscape/css.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/inkscape/runner.py` & `barnhunt-1.2.1rc1/barnhunt/inkscape/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import io
 import locale
 import logging
 import os
 import re
 import shlex
+import sys
 import threading
 import weakref
 from dataclasses import dataclass
 from subprocess import PIPE
 from subprocess import Popen
 from subprocess import run
 from subprocess import STDOUT
@@ -17,19 +18,42 @@
 from typing import Callable
 from typing import Iterable
 from typing import Sequence
 from typing import TypeVar
 
 from pexpect.popen_spawn import PopenSpawn
 
+from .._compat import Final
 from .._compat import Protocol
 
 log = logging.getLogger()
 
 
+def get_default_inkscape_command() -> str:
+    # This is what inkex.command does to find Inkscape (after first
+    # checking $INKSCAPE_COMMAND).
+    #
+    # https://gitlab.com/inkscape/extensions/-/blob/cb74374e46894030775cf947e97ca341b6ed85d8/inkex/command.py#L45
+    if sys.platform == "win32":
+        # prefer inkscape.exe over inkscape.com which spawns a command window
+        return "inkscape.exe"
+    return "inkscape"
+
+
+def get_default_shell_mode() -> bool:
+    """Whether to use Inkscape's shell-mode by default."""
+    if sys.platform == "darwin":
+        return False  # ShellModeRunner current borked
+    return True
+
+
+DEFAULT_INKSCAPE_COMMAND: Final = get_default_inkscape_command()
+DEFAULT_SHELL_MODE: Final = get_default_shell_mode()
+
+
 class InkscapeCommand(Protocol):
     @property
     def cli_args(self) -> Iterable[str]:
         """Commmand line args for Inkscape."""
         raise NotImplementedError()
 
     @property
```

### Comparing `barnhunt-1.2.0rc6/barnhunt/inkscape/svg.py` & `barnhunt-1.2.1rc1/barnhunt/inkscape/svg.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/inkscape/utils.py` & `barnhunt-1.2.1rc1/barnhunt/inkscape/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import os
 import shutil
 import sys
 from pathlib import Path
 from subprocess import run
 
@@ -68,7 +70,38 @@
         HWND(), c_int(CSIDL_APPDATA), HANDLE(), DWORD(), path_buf
     )
     if result != 0:
         raise RuntimeError(  # pragma: NO COVER
             f"ctypes call to SHGetFolderPathW failed ({result})"
         )
     return path_buf.value
+
+
+def get_inkscape_debug_info(inkscape_command: str) -> list[tuple[str, str]]:
+    """Get information about the installed version of Inkscape.
+
+    This information is displayed by the ``barnhunt debug-info`` command.
+
+    """
+    info = [("inkscape_command", inkscape_command)]
+    inkscape = shutil.which(inkscape_command)
+    if not inkscape:
+        info.append(("which", "<not found>"))
+        return info
+    info.append(("which", inkscape))
+
+    try:
+        resolved = Path(inkscape).resolve(strict=True)
+    except Exception as exc:  # pragma: no cover
+        info.append(("resolved", repr(exc)))
+    else:
+        info.append(("resolved", repr(str(resolved))))
+
+    proc = run((inkscape, "--debug-info"), capture_output=True, text=True)
+    if proc.returncode == 0:
+        info.append(("debug-info", proc.stdout.rstrip()))
+    else:
+        proc = run((inkscape, "--version"), capture_output=True, text=True)
+        info.append(("version", proc.stdout.rstrip().rpartition("\n")[2]))
+    if proc.stderr.strip():
+        info.append(("stderr⇒", proc.stderr.rstrip()))
+    return info
```

### Comparing `barnhunt-1.2.0rc6/barnhunt/installer/__init__.py` & `barnhunt-1.2.1rc1/barnhunt/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/installer/github.py` & `barnhunt-1.2.1rc1/barnhunt/installer/github.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/installer/metadata.py` & `barnhunt-1.2.1rc1/barnhunt/installer/metadata.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/layerinfo.py` & `barnhunt-1.2.1rc1/barnhunt/layerinfo.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/pager.py` & `barnhunt-1.2.1rc1/barnhunt/pager.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/pdfutil.py` & `barnhunt-1.2.1rc1/barnhunt/pdfutil.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/barnhunt/templating.py` & `barnhunt-1.2.1rc1/barnhunt/templating.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/pdm_build.py` & `barnhunt-1.2.1rc1/pdm_build.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/pyoxidizer/pyoxidizer.bzl` & `barnhunt-1.2.1rc1/pyoxidizer/pyoxidizer.bzl`

 * *Files 2% similar despite different names*

```diff
@@ -216,35 +216,29 @@
     # This variable defines the configuration of the embedded Python
     python_config = dist.make_python_interpreter_config()
 
     # Set initial value for `sys.path`. If the string `$ORIGIN` exists in
     # a value, it will be expanded to the directory of the built executable.
 
     # FIXME: needed? (neither seem to be?)
-    python_config.module_search_paths = ["$ORIGIN/lib"]
+    # python_config.module_search_paths = ["$ORIGIN/lib"]
     # python_config.filesystem_importer = True
 
     # Write files containing loaded modules to the directory specified
     # by the given environment variable.
     # python_config.write_modules_directory_env = "/tmp/oxidized/loaded_modules"
 
     # Run a Python module as __main__ when the interpreter starts.
-    #
-    # This doesn't work. sys.argv[0] ends up being None
-    #
+    # NB: sys.argv[0] ends up being None, so make sure to ancipate that
     # See https://github.com/indygreg/PyOxidizer/issues/307
-    #
-    # python_config.run_module = "barnhunt.__main__"
+    python_config.run_module = "barnhunt"
 
     # Make the embedded interpreter behave like a `python` process.
     # python_config.config_profile = "python"
 
-    # Evaluate a string as Python code when the interpreter starts.
-    python_config.run_command = "from barnhunt.cli import main; main()"
-
     exe = dist.to_python_executable(
         name="barnhunt",
         packaging_policy=policy,
         config=python_config,
     )
 
     for resource in exe.pip_install(["--only-binary", ":all:", project_root]):
```

### Comparing `barnhunt-1.2.0rc6/pyproject.toml` & `barnhunt-1.2.1rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,38 +27,39 @@
     "Topic :: Printing",
     "Topic :: Utilities",
 ]
 requires-python = ">= 3.7"
 dependencies = [
     "atomicwrites~=1.4",
     "click~=8.1",
+    "importlib-metadata==4; python_version < '3.10'",
     "jinja2~=3.1",
     "lxml~=4.9",
     "marshmallow~=3.19",
     "marshmallow-dataclass~=8.5.13",
     "packaging~=23.1",
     "pexpect~=4.8",
     "pikepdf~=6.2",
     "requests~=2.29",
     "tinycss2~=1.2",
     "typing-extensions~=4.5; python_version < \"3.10\"",
 ]
-version = "1.2.0rc6"
+version = "1.2.1rc1"
 
 [project.license]
 text = "GPL-3.0-only"
 
 [project.urls]
 Homepage = "https://github.com/barnhunt/barnhunt"
 
 [project.entry-points.console_scripts]
 barnhunt = "barnhunt.cli:main"
 
 [project.readme]
-text = "# Barn Hunt Map Helper\n\n[![Tests](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml/badge.svg)](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml)\n[![PyPI Version](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Python Versions](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Inkscape Versions](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2-blue.svg?logo=inkscape)](https://inkscape.org/)\n[![PyPI Status](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n\nThis is a helper script Jeff uses for drafting [Barn Hunt][] course\nmaps.\n\nIt does a bunch of stuff, but the important bit is that it exports PDF\nversions of maps from [Inkscape][] SVG files.\n\nI draw all the maps for a given ring (for a day or weekend) in a\nsingle Inkscape drawing.  Various maps (for different trials/classes,\nbuild map, rat-maps, base maps, etc.) are generated by hiding and\nunhiding appropriate layers in the drawing and exporting to PDF.\n\nThis program automates that process.\n\n## Requirements\n\nThis program requires Python, version 3.7 or higher to run.\n\nIt \"should\" work with all versions of Inkscape, 0.9x through 1.2.1.\n\nI use this program on Linux, however the package now includes a GitHub\nCI workflow that performs rudimentary testing on Windows and macOS, so\nthere’s a moderate chance it might \"just work\" on those platforms.\n(Due to a dependency on the [pikepdf][] package, it should work on\nx86_64-based Macs, but may not work on Macs that use Apple silicon. If\npikepdf compatibility is an issue for you, let me know — it’s probably\nfixable.)\n\n## Installation\n\nAs this package is published to\n[PyPI](https://pypi.org/project/barnhunt/) in may be installed into a\n[_virtualenv_][venv] using [`pip`][pip]. It is suggested that you use\n[`pipx`][pipx] to combine those two steps.\n\nA basic outline of how to proceed:\n\n1. Install [python][] if it is not already installed.  (Version 3.7 or\n   greater is required.)\n\n2. Install [pipx][].  This might look like:\n\n   ```sh\n   python3 -m pip install --user pipx\n   python3 -m pipx ensurepath\n   ```\n\n3. Install `barnhunt`.\n\n   ```sh\n   pipx install barnhunt\n   ```\n\n## How to Use\n\nSadly, this program is currently quite under-documented.\n\nThe functions of the basic sub-commands and command-line options are\ntersely documented via the `--help` option.  Try:\n\n```sh\nbarnhunt --help\n```\n\nand\n\n```sh\nbarnhunt pdfs --help\n```\n\nfor starters.\n\nIf you get stuck, kick me!\n\n## Author\n\nThis package was written by Jeff Dairiki, BHAJ-221A, <dairiki@dairiki.org>.\n\n----\n\n[Inkscape]: https://inkscape.org/ (The Inkscape home page)\n[Barn Hunt]: https://www.barnhunt.com/ (Barn Hunt — a fabulous sport for dogs)\n[python]: https://www.python.org/ (The Python home page)\n[venv]: https://docs.python.org/3/library/venv.html\n(Python venv module documentation)\n[pipx]: https://pypa.github.io/pipx/ (The pipx home page)\n[pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)\n[pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html\n(The Installation section of the pikepdf documentation)\n\n## Changes\n\n### Release 1.2.0rc6 (2023-04-27)\n\n- Build an Windows executable and installer using [PyOxidizer].  The\n  .msi installer should be downloadable from the\n  [Releases](https://github.com/barnhunt/barnhunt/releases) page.\n\n- Added a `--dump-loaded-modules` option which causes `barnhunt` to\n  write a list of all loaded modules the current working directory.\n  (This is a development tool, not generally useful to most users.)\n\n- Hardwire the distribution version into `barnhunt.__version__` rather\n  than deducing it via `importlib.metadata`.  This allows us to monkey\n  with the version we report from the PyOxidizer-built Windows\n  executable so that it indicates the MSI build version as well as\n  the distribution version.\n\n- Convert package from setuptools to PDM.\n\n[PyOxidizer]: https://pyoxidizer.readthedocs.io/en/stable/pyoxidizer.html\n\n### Release 1.2.0rc5 (2023-03-05)\n\n#### Bugs Fixed\n\n- When there was a visible “clone” (`<svg:use>` element) that\n  referenced a source on a hidden layer were being pruned from the SVG\n  before conversion to PDF.  (When exporting an SVG, hidden layers are\n  omitted from the SVG — this speeds Inkscape up considerably when\n  there is a large amount of hidden content.) Now we detect hidden\n  layers that contain source material for clones, and retain them in\n  the SVG file.\n\n- Add a cruft pattern to ignore “`Gtk-WARNING\"`” messages that have\n  started appearing since I installed Inkscape from [Inkscape’s ppa][ppa].\n\n- Fix tests to workaround segfault from pikepdf 7.0.0, 7.1.0, and 7.1.1.\n  (See [pikepdf/pikepdf#452].)\n\n[ppa]: https://inkscape.org/release/inkscape-1.2.2/gnulinux/ubuntu/ppa/dl/\n[pikepdf/pikepdf#452]: https://github.com/pikepdf/pikepdf/issues/452).\n\n### Release 1.2.0rc4 (2023-01-09)\n\nSupport python 3.11.\n\n#### Bugs\n\n- Shell-mode runner: fix readline/pexpect disagreement with respect to\n  horizontal scrolling of long lines.  In some cases, when Inkscape is\n  compiled to use GNU readline, long input lines will be scrolled\n  horizontally (even when stdin is not a tty). This messes with\n  pexpect's head. We've now added some basic tests for this, and set\n  some environment variables to try to convince readline not to do the\n  scrolling.\n\n#### Testing\n\n- Test under python 3.11\n- Fix tests for Windows environments where $APPDATA is not set\n- Fix tests for error message changes in packaging>=22\n\n### Release 1.2.0rc3 (2022-10-19)\n\n#### Extension/Symbols Installer\n\n- Make code for deducing Inkscape profile directory more robust.\n  (There's now a beter chance this will actually work on Windows.)\n- Support setting Inkscape profile directory via `$INKSCAPE_PROFILE_DIR`.\n\n### Release 1.2.0rc2 (2022-10-17)\n\n### Extension and Symbol Set Installation\n\n- This release add a `barnhunt install` (and `uninstall`) sub-command\n  to simplify installation of the\n  [inkex-bh](https://github.com/barnhunt/inkex-bh) Inkscape extensions\n  and [bh-symbols](https://github.com/barnhunt/bh-symbols) symbol\n  sets.\n\n#### Testing\n\n- Update to `mypy==0.982` for testing. Fix spurious mypy errors.\n\n### Release 1.2.0rc1 (2022-08-31)\n\nFirst public release to PyPI. Moved project to\n[GitHub](https://github.com/barnhunt/barnhunt).\n\n- Dropped support for python 3.6\n- Changed license to GPL version 3\n- We now do rudimentary testing under Windows and macOS.\n\n#### Dependencies\n\n- Use [pikepdf](https://pypi.org/project/pikepdf/) instead of\n  [pdfrw](https://pypi.org/project/pdfrw/) to manipulate PDFs.  (Pdfrw\n  seems not to be very actively maintained.) The only possible\n  downside of this is that `pikepdf` is not pure-python. It claims to\n  be easily installable on Windows and _x86_64_ Macs, but is not\n  (easily) installable on Macs with Apple silicon.\n\n- Generated PDFs are now [linearized][qpdf-linearize] and\n  [compressed][qpdf-object-streams].\n\n- Add test dependency on\n  [pdfminer.six](https://pypi.org/project/pdfminer.six/) (but drop\n  dependency on [PyPDF2](https://pypi.org/project/PyPDF2/)).\n\n\n#### Compatibility\n\n- Refactor `barnhunt.inkscape.runner` to support running\n  Inkscape >= 1.0 (as well as continuing to support Inkscape 0.9x).\n\n- Add `--inkscape-command` parameter to the `barnhunt pdfs` command\n  to specify the name/path of the Inkscape binary to run to export PDFs.\n  This also supports setting the Inkscape executable via the `$INKSCAPE_COMMAND`\n  environment variable.  Default executable is not `inkscape.exe` on Windows\n  (and `inkscape` everywhere else).\n\n- Use `pexpect.popen_spawn.PopenSpawn` instead of `pexpect.spawn` to\n  run Inkscape in shell-mode. Due to `pexpect.spawn`'s use of ptys, it\n  [will not work][pexpect-windows] on Windows.\n\n- **MacOS**: our code for running Inkscape in shell-mode appears to be broken.\n  For now, on _macOS_ we default to not using shell-mode.\n\n#### Packaging\n\n- Added a stub `barnhunt.__main__` module to allow running via `python\n  -m barnhunt`.\n\n#### Testing\n\n- Add type annotations.\n\n#### Bit Rot\n\n- Fix up tests to address deprecations in PyPDF2.\n\n[qpdf-linearize]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=linearize#option-linearize\n[qpdf-object-streams]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=object-streams#option-object-streams\n[pexpect-windows]: https://pexpect.readthedocs.io/en/stable/overview.html#windows\n\n### Release 1.1.0a1 (2022-03-08)\n\n#### \"Base Map\" support\n\nAdd ability to mark layers for exclusion from particular output files.\n\nThis adds the ability to list multiple comma-separated output base\nfilenames for a given overlay.\nE.g. A layer with label `\"[o|build_notes,base] Build Notes\"`\nwill define an overlay which will generate maps in two separate\noutput files.\n\nTagging a layer with `[!`_output-basename_`]` will exclude that\nlayer from any maps which are directed to the specified output\nfilename.\n\nTagging a layer with `[=`_output-basename_`]` will include that layer\nfrom any maps which are directed to the specified output filename, while\nexcluding all other sibling layers not explicitly tagged to be included\nin that output file.\n\n\n### Release 1.0.1 (2021-11-10)\n\n#### Diagnostics\n\n`Barnhunt pdfs` now issues a warning when generating PDFs from an SVG\nfile which does not have an explicit random-seed set.\n\n#### Bugs Fixed\n\nOpen SVG files in binary mode in order to let the XML parser figure\nout the encoding from the XML declaration.\n\n### Release 1.0 (2021-11-10)\n\nSupport python 3.10.\n\n#### Random Seed\n\nThe way the random seed (used for generating random rat numbers) for\neach SVG layer is computed has been changed in a\n**backward-incompatible** way.  This was done so that rat numbers can\nbe kept from changing when an SVG source file is copied or edited in\nsuch a way that the device and/or inode of the file changes.\n\nNow, the file-level random seed (an integer) is read from the\n`bh:random-seed` attribute of the root `svg` element of the SVG\nfile. If no `bh:random-seed` attribute is set, the file-level seed is\ncomputed by hashing the device and inode numbers of the SVG file.\n\nThe layer-level seed is formed by hashing the file-level random seed\nwith the XML *id* of the layer.\n\n(Formerly, the layer-level seed was form by hashing a triple of the\nfile-level seed (which was always zero), the hash of the SVG files\ndevice and inode, and the id of the layer.)\n\nA new `barnhunt random-seed` sub-command has been implemented to help\nwith setting the random seed for SVG source files.\n\n#### Bit-rot\n\nAddress `DeprecationWarning: 'contextfunction' is renamed to\n'pass_context'` from Jinja2. Require `Jinja2>3`.\n\n#### OCDisms\n\nRun `pyupgrade --py36-plus` on source.\n\n\n### Release 0.5 (2021-05-04)\n\nMake `-o` option to `2up` sub-command optional.\n\nRemove support for python < 3.6.\n\n### Release 0.4 (2019-02-25)\n\n#### New Sub-Command: 2up\n\nNew `2up` sub-command to format PDFs for 2-up printing.  Pages are\npre-shuffled so that the 2-up pages do not need to be shuffled after\ncutting.\n\n\n### Release 0.3 (2019-02-20)\n\n#### `barnhunt pdfs`\n\n- Multi-page output support.\n\n  There is a new syntax to specify the output file basename for an overlay.\n  Multiple overlays which specify the same output file will all be saved to\n  the same file.\n\n- It is now possible to render course maps from multiple SVG files in a\n  single invocation.  (Just list all the files to be rendered on the\n  command line.)\n\n#### Tests\n\n- `test_layerinfo.test_layerflags_str`: Fix test to deal with\n  arbitrary ordering of `enum.Flag` flags.\n\n### Release 0.2 (2018-11-07)\n\n#### Templating\n\n- Do not expand text within hidden layers.  This avoids generating\n  error messages (e.g. \"'overlay' is undefined\") due to template\n  expansion of unused text.\n\n- Add optional `skip` argument to the `random_rats` function.\n  This allows the generation of more than one set of stable random rat\n  numbers per layer.  E.g. `random_rats(skip=5)` will generate a set\n  of random number totally uncorrelated to that generated by\n  `random_rats()`.  Using `skip` has the advantage over using\n  `seed=None` that the results are stable and do not vary from\n  render to render.\n\n### Release 0.1 (2018-11-07)\n\n- Python 3.7 is now supported.\n\n- The template for the output filename has been generalized to work\n  sensibly in the case where overlays are nested more than two deep.\n\n#### Templating\n\n- Added new attributes to layers:\n\n  `layer.is_overlay`\n      Boolean.  True if layer is an overlay.\n\n  `layer.lineage`\n      Sequence starting with layer and including each parent layer in\n      turn.\n\n  `layer.overlay`\n      Returns the nearest overlay layer.  If the layer is an overlay,\n      `layer.overlay` returns `layer`, otherwise it returns the\n      nearest parent layer which is an overlay.  If the layer is not\n      contained within an overlay, returns `None`.\n\n- Added new values to context when expanding text in SVG:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the text\n      element, in order from outermost to innermost.\n\n  `course`\n      The outermost overlay layer.  (Equivalent to `overlays[0]`.)\n      This value already existed in the context used for filename expansion.\n\n  `overlay`\n      If the element is at least two overlays deep, this is the\n      innermost overlay.  Otherwise it is unset.  This value already\n      existed in the context used for filename expansion.\n\n- Added new values to context when expanding output filenames:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the overlay\n      being expanded.\n\n#### Bugs\n\n- Templating: the `safepath` filter would fail with a `TypeError`\n  if applied to anything but a string.  Now it coerces its argument to\n  text.\n\n- Templating: (New style) layer flags in parent layers were not being\n  removed from the layer labels.  (E.g. `\"{{ layer.parent.label }}\"`\n  was expanding to `\"[o] Some Overlay\"`, when it should expand to\n  `\"Some Overlay\"`.)\n\n- Pexpect==4.4.0 appears to have a subtle brokenness when\n  `searchwindowsize` is set to something other than `None`.  The\n  problem seems to be in [pexpect.expect.py][], and is triggered when\n  multiple chunks of output are read before a match is found.\n\n[pexpect.expect.py]: <https://github.com/pexpect/pexpect/blob/606f368b4a0dc442e2523d439d722a389b6e54c6/pexpect/expect.py#L22>\n\n#### Bit-Rot\n\n- Use `log.warning`, rather than the deprecated `log.warn`.\n\n### Release 0.1a12 (2017-02-09)\n\n- Remove tags from layer.label when expanding templated text in SVG file.\n\n### Release 0.1a11 (2017-02-01)\n\n- Add `--version` command line option\n\n#### Pager for `coords`\n\n- A fancy pager (poor man's `less`) has been added for viewing the\n  output of the `barnhunt coords` sub-command.  If any of `sys.stdin`\n  or `sys.stdout` is not a tty, then the pager will be disabled.\n\n- Since there is now a fancy pager, the default for `--number-of-rows`\n  has been increased to 1000.\n\n### Release 0.1a10 (2017-01-30)\n\n#### Things still to be fixed\n\nThings still to be fixed: I'm pretty sure things are direly broken if\na drawing contains no overlays, and somewhat broken if a drawing\ncontains more than two layers of overlays.  The problems have to do\nwith how the output PDF filenames are determined...\n\n#### New layer flag scheme\n\nNew scheme for marking overlay and hidden layers.  One can now set\nbit-flags on layers by including the flags in square brackets at the\nbeginning of the layer label.  I.e. a label like `\"[o] Master Trial\n1\"` marks the layer as an overlay layer, while `\"[h] Prototypes\"`\nmarks a hidden layer.\n\nIf no layers have any flags, `barnhunt pdfs` will fall back to the\nold name-based heuristics for determining hidden and overlay layers.\n\n\n### Release 0.1a9 (2017-01-03)\n\n* When exporting PDFs, run `inkscape` with `--export-area-page`.\n\n#### Packaging\n\n* Fix MANIFEST.in. Tests were not being included in sdist.\n\n* Add `url` to package metadata.\n\n### Release 0.1a8 (2018-01-03)\n\n* Ignore *ring* layers when identifying *course* layers.  (Now a layer\n  labeled “C8 Ring” will not be treated as a course layer.)\n\n* `pdfs`: default `--output-directory` to `.` (avoiding exception when no\n  explicit output directory is specified.)\n\n### Release 0.1a7 (2017-11-18)\n\n* Change `barnhunt coords` so that it omits duplicate coordinates in its output.\n  Also increase the default for `--number-of-rows` to 50 and\n  add the `--group-size` parameter to separate output into groups.\n\n### Release 0.1a6 (2017-11-15)\n\n* Templating: `LabelAdapter` now stringifies to the layer label, and\n  `FileAdapter` now stringifies to the file name.\n* More refactoring, more tests\n* Run several inkscapes in parallel.  This results in a major speedup.\n\n### Release 0.1a5 (2017-11-13)\n\n* Expand text in SVG file.\n* Add tests.\n* Major code refactor.\n\n### Release 0.1a4 (2017-11-10)\n\n#### PDFS\n\n* Log unexpected output from inkscape.\n\n* Add `--no-shell-mode-inkscape` option to control whether shell-mode inkscape\n  optimization is used.\n\n### Release 0.1a3.post1 (2017-11-10)\n\n#### PDFS\n\n* Reverse order that layers are considered.  (Layers are listed from\n  bottom to top in the SVG file.)\n\n### Release 0.1a3 (2017-11-10)\n\n#### PDFS\n\nReplace spaces and other shell-unfriendly characters with underscores\nin output file names.\n\n### Release 0.1a2 (2017-11-09)\n\nAdd sub-commands for generating random numbers.\n\n### Release 0.1a1 (2017-11-07)\n\nInitial release.\n"
+text = "# Barn Hunt Map Helper\n\n[![Test status badge](https://img.shields.io/github/actions/workflow/status/barnhunt/barnhunt/ci.yml?label=tests)](https://github.com/barnhunt/barnhunt/actions/workflows/ci.yml)\n[![Latest version badge](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Supported Python versions badge](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Supported Inkscape versions badge](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2.2-blue.svg?logo=inkscape)](https://inkscape.org/)\n[![Development status badge](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)\n[![Trackgit-views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhapwefdbvler7yp5dsl)](https://trackgit.com)\n\nThis is a helper script Jeff uses for drafting [Barn Hunt][] course\nmaps.\n\nIt does a bunch of stuff, but the important bit is that it exports PDF\nversions of maps from [Inkscape][] SVG files.\n\nI draw all the maps for a given ring (for a day or weekend) in a\nsingle Inkscape drawing.  Various maps (for different trials/classes,\nbuild map, rat-maps, base maps, etc.) are generated by hiding and\nunhiding appropriate layers in the drawing and exporting to PDF.\n\nThis program automates that process.\n\n## Requirements\n\nThis program requires Python, version 3.7 or higher to run.\n\nIt \"should\" work with all versions of Inkscape, 0.9x through 1.2.1.\n\nI use this program on Linux, however the package now includes a GitHub\nCI workflow that performs rudimentary testing on Windows and macOS, so\nthere’s a moderate chance it might \"just work\" on those platforms.\n(Due to a dependency on the [pikepdf][] package, it should work on\nx86_64-based Macs, but may not work on Macs that use Apple silicon. If\npikepdf compatibility is an issue for you, let me know — it’s probably\nfixable.)\n\n## Installation\n\n### Windows\n\nWe now publish a compiled version of the program for Windows (which may\neven work.) Using this version has the advantage that Python is not required\nto be installed. (And even if Python is installed, this version may work-around\nsome bugs having to do with the various different ways that Python can be\ninstalled on on Windows computer.)\n\n1. Browse to our [releases](https://github.com/barnhunt/barnhunt/releases/)\n   page. Select a release, and look down in the *Assets* section of the\n   release page. (You may have to click the triangle to expand the\n   *Assets* section.)\n\n2. Download the MSI installer (the filename should end with `.msi` —\n   e.g. `Barnhunt-1.2.0.49-x86_64-pc-windows-msvc.msi`). The file\n   is not signed, so you may have to click through some nasty warnings\n   about \"unrecognized, potentially dangerous\" files.\n\n3. Once downloaded, open (double-click) the file you just\n   downloaded. Hopefully and installer dialog should open.  Accept the\n   default choices.\n\n4. Now open a terminal command-line window. Type `barnhunt\n   --version`. If all is good, barnhunt should report its version. Run\n   `barnhunt --help` for the help screen.\n\n\n### Linux (or Windows with Python installed)\n\nAs this package is published to\n[PyPI](https://pypi.org/project/barnhunt/) it may be installed into a\n[_virtualenv_][venv] using [`pip`][pip]. It is suggested that you use\n[`pipx`][pipx] to combine those two steps.\n\nA basic outline of how to proceed:\n\n1. Install [python][] if it is not already installed.  (Version 3.7 or\n   greater is required.)\n\n2. Install [pipx][].  This might look like:\n\n   ```sh\n   python3 -m pip install --user pipx\n   python3 -m pipx ensurepath\n   ```\n\n3. Install `barnhunt`.\n\n   ```sh\n   pipx install barnhunt\n   ```\n\n## How to Use\n\nSadly, this program is currently quite under-documented.\n\nThe functions of the basic sub-commands and command-line options are\ntersely documented via the `--help` option.  Try:\n\n```sh\nbarnhunt --help\n```\n\nand\n\n```sh\nbarnhunt pdfs --help\n```\n\nfor starters.\n\nIf you get stuck, kick me!\n\n## Author\n\nThis package was written by Jeff Dairiki, BHAJ-221A, <dairiki@dairiki.org>.\n\n----\n\n[Inkscape]: https://inkscape.org/ (The Inkscape home page)\n[Barn Hunt]: https://www.barnhunt.com/ (Barn Hunt — a fabulous sport for dogs)\n[python]: https://www.python.org/ (The Python home page)\n[venv]: https://docs.python.org/3/library/venv.html\n(Python venv module documentation)\n[pipx]: https://pypa.github.io/pipx/ (The pipx home page)\n[pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)\n[pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html\n(The Installation section of the pikepdf documentation)\n\n## Changes\n\n### Release 1.2.1rc1 (2023-05-22)\n\n(There was no final release of 1.2.0. It is a long story. I mistakenly\ncommitted a couple of files to LFS. To clear out LFS storage for a\nGitHub repo, one has to [delete the whole repo](😬). As a result, the\nworkflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump\nis required to keep those PyOxidizer windows build version numbers —\n`<major>.<minor>.<micro>.<run-number>` — monotonic.)\n\n[delete the whole repo]: https://docs.github.com/en/repositories/working-with-files/managing-large-files/removing-files-from-git-large-file-storage#git-lfs-objects-in-your-repository\n\n#### CLI Changes\n\n- The `--inkscape-command`, `--processes` and `--shell-mode-inkscape`\n  options have been moved from the `barnhunt pdfs` subcommand to the\n  man `barnhunt` command group.\n\n- And new `debug-info` subcommand has been added to display various\n  information about the installed version of the `barnhunt` command\n  and its execution environment.\n\n- The `--dump-loaded-modules` option has been removed.  The\n  functionality is still available by setting the\n  `$BARNHUNT_DUMP_LOADED_MODULES` environment variable to a non-empty\n  value.\n\n#### Bugs Fixed\n\n- Fixed exception in `barnhunt.cli.default_2up_output_file` during\n  shell-completion for `barnhunt 2up`.\n\n### Release 1.2.0rc6 (2023-04-27)\n\n- Build an Windows executable and installer using [PyOxidizer].  The\n  .msi installer should be downloadable from the\n  [Releases](https://github.com/barnhunt/barnhunt/releases) page.\n\n- Added a `--dump-loaded-modules` option which causes `barnhunt` to\n  write a list of all loaded modules the current working directory.\n  (This is a development tool, not generally useful to most users.)\n\n- Hardwire the distribution version into `barnhunt.__version__` rather\n  than deducing it via `importlib.metadata`.  This allows us to monkey\n  with the version we report from the PyOxidizer-built Windows\n  executable so that it indicates the MSI build version as well as\n  the distribution version.\n\n- Convert package from setuptools to PDM.\n\n[PyOxidizer]: https://pyoxidizer.readthedocs.io/en/stable/pyoxidizer.html\n\n### Release 1.2.0rc5 (2023-03-05)\n\n#### Bugs Fixed\n\n- When there was a visible “clone” (`<svg:use>` element) that\n  referenced a source on a hidden layer were being pruned from the SVG\n  before conversion to PDF.  (When exporting an SVG, hidden layers are\n  omitted from the SVG — this speeds Inkscape up considerably when\n  there is a large amount of hidden content.) Now we detect hidden\n  layers that contain source material for clones, and retain them in\n  the SVG file.\n\n- Add a cruft pattern to ignore “`Gtk-WARNING\"`” messages that have\n  started appearing since I installed Inkscape from [Inkscape’s ppa][ppa].\n\n- Fix tests to workaround segfault from pikepdf 7.0.0, 7.1.0, and 7.1.1.\n  (See [pikepdf/pikepdf#452].)\n\n[ppa]: https://inkscape.org/release/inkscape-1.2.2/gnulinux/ubuntu/ppa/dl/\n[pikepdf/pikepdf#452]: https://github.com/pikepdf/pikepdf/issues/452).\n\n### Release 1.2.0rc4 (2023-01-09)\n\nSupport python 3.11.\n\n#### Bugs\n\n- Shell-mode runner: fix readline/pexpect disagreement with respect to\n  horizontal scrolling of long lines.  In some cases, when Inkscape is\n  compiled to use GNU readline, long input lines will be scrolled\n  horizontally (even when stdin is not a tty). This messes with\n  pexpect's head. We've now added some basic tests for this, and set\n  some environment variables to try to convince readline not to do the\n  scrolling.\n\n#### Testing\n\n- Test under python 3.11\n- Fix tests for Windows environments where $APPDATA is not set\n- Fix tests for error message changes in packaging>=22\n\n### Release 1.2.0rc3 (2022-10-19)\n\n#### Extension/Symbols Installer\n\n- Make code for deducing Inkscape profile directory more robust.\n  (There's now a beter chance this will actually work on Windows.)\n- Support setting Inkscape profile directory via `$INKSCAPE_PROFILE_DIR`.\n\n### Release 1.2.0rc2 (2022-10-17)\n\n### Extension and Symbol Set Installation\n\n- This release add a `barnhunt install` (and `uninstall`) sub-command\n  to simplify installation of the\n  [inkex-bh](https://github.com/barnhunt/inkex-bh) Inkscape extensions\n  and [bh-symbols](https://github.com/barnhunt/bh-symbols) symbol\n  sets.\n\n#### Testing\n\n- Update to `mypy==0.982` for testing. Fix spurious mypy errors.\n\n### Release 1.2.0rc1 (2022-08-31)\n\nFirst public release to PyPI. Moved project to\n[GitHub](https://github.com/barnhunt/barnhunt).\n\n- Dropped support for python 3.6\n- Changed license to GPL version 3\n- We now do rudimentary testing under Windows and macOS.\n\n#### Dependencies\n\n- Use [pikepdf](https://pypi.org/project/pikepdf/) instead of\n  [pdfrw](https://pypi.org/project/pdfrw/) to manipulate PDFs.  (Pdfrw\n  seems not to be very actively maintained.) The only possible\n  downside of this is that `pikepdf` is not pure-python. It claims to\n  be easily installable on Windows and _x86_64_ Macs, but is not\n  (easily) installable on Macs with Apple silicon.\n\n- Generated PDFs are now [linearized][qpdf-linearize] and\n  [compressed][qpdf-object-streams].\n\n- Add test dependency on\n  [pdfminer.six](https://pypi.org/project/pdfminer.six/) (but drop\n  dependency on [PyPDF2](https://pypi.org/project/PyPDF2/)).\n\n\n#### Compatibility\n\n- Refactor `barnhunt.inkscape.runner` to support running\n  Inkscape >= 1.0 (as well as continuing to support Inkscape 0.9x).\n\n- Add `--inkscape-command` parameter to the `barnhunt pdfs` command\n  to specify the name/path of the Inkscape binary to run to export PDFs.\n  This also supports setting the Inkscape executable via the `$INKSCAPE_COMMAND`\n  environment variable.  Default executable is not `inkscape.exe` on Windows\n  (and `inkscape` everywhere else).\n\n- Use `pexpect.popen_spawn.PopenSpawn` instead of `pexpect.spawn` to\n  run Inkscape in shell-mode. Due to `pexpect.spawn`'s use of ptys, it\n  [will not work][pexpect-windows] on Windows.\n\n- **MacOS**: our code for running Inkscape in shell-mode appears to be broken.\n  For now, on _macOS_ we default to not using shell-mode.\n\n#### Packaging\n\n- Added a stub `barnhunt.__main__` module to allow running via `python\n  -m barnhunt`.\n\n#### Testing\n\n- Add type annotations.\n\n#### Bit Rot\n\n- Fix up tests to address deprecations in PyPDF2.\n\n[qpdf-linearize]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=linearize#option-linearize\n[qpdf-object-streams]: https://qpdf.readthedocs.io/en/latest/cli.html?highlight=object-streams#option-object-streams\n[pexpect-windows]: https://pexpect.readthedocs.io/en/stable/overview.html#windows\n\n### Release 1.1.0a1 (2022-03-08)\n\n#### \"Base Map\" support\n\nAdd ability to mark layers for exclusion from particular output files.\n\nThis adds the ability to list multiple comma-separated output base\nfilenames for a given overlay.\nE.g. A layer with label `\"[o|build_notes,base] Build Notes\"`\nwill define an overlay which will generate maps in two separate\noutput files.\n\nTagging a layer with `[!`_output-basename_`]` will exclude that\nlayer from any maps which are directed to the specified output\nfilename.\n\nTagging a layer with `[=`_output-basename_`]` will include that layer\nfrom any maps which are directed to the specified output filename, while\nexcluding all other sibling layers not explicitly tagged to be included\nin that output file.\n\n\n### Release 1.0.1 (2021-11-10)\n\n#### Diagnostics\n\n`Barnhunt pdfs` now issues a warning when generating PDFs from an SVG\nfile which does not have an explicit random-seed set.\n\n#### Bugs Fixed\n\nOpen SVG files in binary mode in order to let the XML parser figure\nout the encoding from the XML declaration.\n\n### Release 1.0 (2021-11-10)\n\nSupport python 3.10.\n\n#### Random Seed\n\nThe way the random seed (used for generating random rat numbers) for\neach SVG layer is computed has been changed in a\n**backward-incompatible** way.  This was done so that rat numbers can\nbe kept from changing when an SVG source file is copied or edited in\nsuch a way that the device and/or inode of the file changes.\n\nNow, the file-level random seed (an integer) is read from the\n`bh:random-seed` attribute of the root `svg` element of the SVG\nfile. If no `bh:random-seed` attribute is set, the file-level seed is\ncomputed by hashing the device and inode numbers of the SVG file.\n\nThe layer-level seed is formed by hashing the file-level random seed\nwith the XML *id* of the layer.\n\n(Formerly, the layer-level seed was form by hashing a triple of the\nfile-level seed (which was always zero), the hash of the SVG files\ndevice and inode, and the id of the layer.)\n\nA new `barnhunt random-seed` sub-command has been implemented to help\nwith setting the random seed for SVG source files.\n\n#### Bit-rot\n\nAddress `DeprecationWarning: 'contextfunction' is renamed to\n'pass_context'` from Jinja2. Require `Jinja2>3`.\n\n#### OCDisms\n\nRun `pyupgrade --py36-plus` on source.\n\n\n### Release 0.5 (2021-05-04)\n\nMake `-o` option to `2up` sub-command optional.\n\nRemove support for python < 3.6.\n\n### Release 0.4 (2019-02-25)\n\n#### New Sub-Command: 2up\n\nNew `2up` sub-command to format PDFs for 2-up printing.  Pages are\npre-shuffled so that the 2-up pages do not need to be shuffled after\ncutting.\n\n\n### Release 0.3 (2019-02-20)\n\n#### `barnhunt pdfs`\n\n- Multi-page output support.\n\n  There is a new syntax to specify the output file basename for an overlay.\n  Multiple overlays which specify the same output file will all be saved to\n  the same file.\n\n- It is now possible to render course maps from multiple SVG files in a\n  single invocation.  (Just list all the files to be rendered on the\n  command line.)\n\n#### Tests\n\n- `test_layerinfo.test_layerflags_str`: Fix test to deal with\n  arbitrary ordering of `enum.Flag` flags.\n\n### Release 0.2 (2018-11-07)\n\n#### Templating\n\n- Do not expand text within hidden layers.  This avoids generating\n  error messages (e.g. \"'overlay' is undefined\") due to template\n  expansion of unused text.\n\n- Add optional `skip` argument to the `random_rats` function.\n  This allows the generation of more than one set of stable random rat\n  numbers per layer.  E.g. `random_rats(skip=5)` will generate a set\n  of random number totally uncorrelated to that generated by\n  `random_rats()`.  Using `skip` has the advantage over using\n  `seed=None` that the results are stable and do not vary from\n  render to render.\n\n### Release 0.1 (2018-11-07)\n\n- Python 3.7 is now supported.\n\n- The template for the output filename has been generalized to work\n  sensibly in the case where overlays are nested more than two deep.\n\n#### Templating\n\n- Added new attributes to layers:\n\n  `layer.is_overlay`\n      Boolean.  True if layer is an overlay.\n\n  `layer.lineage`\n      Sequence starting with layer and including each parent layer in\n      turn.\n\n  `layer.overlay`\n      Returns the nearest overlay layer.  If the layer is an overlay,\n      `layer.overlay` returns `layer`, otherwise it returns the\n      nearest parent layer which is an overlay.  If the layer is not\n      contained within an overlay, returns `None`.\n\n- Added new values to context when expanding text in SVG:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the text\n      element, in order from outermost to innermost.\n\n  `course`\n      The outermost overlay layer.  (Equivalent to `overlays[0]`.)\n      This value already existed in the context used for filename expansion.\n\n  `overlay`\n      If the element is at least two overlays deep, this is the\n      innermost overlay.  Otherwise it is unset.  This value already\n      existed in the context used for filename expansion.\n\n- Added new values to context when expanding output filenames:\n\n  `overlays`\n      A list of all overlay layers in the lineage of the overlay\n      being expanded.\n\n#### Bugs\n\n- Templating: the `safepath` filter would fail with a `TypeError`\n  if applied to anything but a string.  Now it coerces its argument to\n  text.\n\n- Templating: (New style) layer flags in parent layers were not being\n  removed from the layer labels.  (E.g. `\"{{ layer.parent.label }}\"`\n  was expanding to `\"[o] Some Overlay\"`, when it should expand to\n  `\"Some Overlay\"`.)\n\n- Pexpect==4.4.0 appears to have a subtle brokenness when\n  `searchwindowsize` is set to something other than `None`.  The\n  problem seems to be in [pexpect.expect.py][], and is triggered when\n  multiple chunks of output are read before a match is found.\n\n[pexpect.expect.py]: <https://github.com/pexpect/pexpect/blob/606f368b4a0dc442e2523d439d722a389b6e54c6/pexpect/expect.py#L22>\n\n#### Bit-Rot\n\n- Use `log.warning`, rather than the deprecated `log.warn`.\n\n### Release 0.1a12 (2017-02-09)\n\n- Remove tags from layer.label when expanding templated text in SVG file.\n\n### Release 0.1a11 (2017-02-01)\n\n- Add `--version` command line option\n\n#### Pager for `coords`\n\n- A fancy pager (poor man's `less`) has been added for viewing the\n  output of the `barnhunt coords` sub-command.  If any of `sys.stdin`\n  or `sys.stdout` is not a tty, then the pager will be disabled.\n\n- Since there is now a fancy pager, the default for `--number-of-rows`\n  has been increased to 1000.\n\n### Release 0.1a10 (2017-01-30)\n\n#### Things still to be fixed\n\nThings still to be fixed: I'm pretty sure things are direly broken if\na drawing contains no overlays, and somewhat broken if a drawing\ncontains more than two layers of overlays.  The problems have to do\nwith how the output PDF filenames are determined...\n\n#### New layer flag scheme\n\nNew scheme for marking overlay and hidden layers.  One can now set\nbit-flags on layers by including the flags in square brackets at the\nbeginning of the layer label.  I.e. a label like `\"[o] Master Trial\n1\"` marks the layer as an overlay layer, while `\"[h] Prototypes\"`\nmarks a hidden layer.\n\nIf no layers have any flags, `barnhunt pdfs` will fall back to the\nold name-based heuristics for determining hidden and overlay layers.\n\n\n### Release 0.1a9 (2017-01-03)\n\n* When exporting PDFs, run `inkscape` with `--export-area-page`.\n\n#### Packaging\n\n* Fix MANIFEST.in. Tests were not being included in sdist.\n\n* Add `url` to package metadata.\n\n### Release 0.1a8 (2018-01-03)\n\n* Ignore *ring* layers when identifying *course* layers.  (Now a layer\n  labeled “C8 Ring” will not be treated as a course layer.)\n\n* `pdfs`: default `--output-directory` to `.` (avoiding exception when no\n  explicit output directory is specified.)\n\n### Release 0.1a7 (2017-11-18)\n\n* Change `barnhunt coords` so that it omits duplicate coordinates in its output.\n  Also increase the default for `--number-of-rows` to 50 and\n  add the `--group-size` parameter to separate output into groups.\n\n### Release 0.1a6 (2017-11-15)\n\n* Templating: `LabelAdapter` now stringifies to the layer label, and\n  `FileAdapter` now stringifies to the file name.\n* More refactoring, more tests\n* Run several inkscapes in parallel.  This results in a major speedup.\n\n### Release 0.1a5 (2017-11-13)\n\n* Expand text in SVG file.\n* Add tests.\n* Major code refactor.\n\n### Release 0.1a4 (2017-11-10)\n\n#### PDFS\n\n* Log unexpected output from inkscape.\n\n* Add `--no-shell-mode-inkscape` option to control whether shell-mode inkscape\n  optimization is used.\n\n### Release 0.1a3.post1 (2017-11-10)\n\n#### PDFS\n\n* Reverse order that layers are considered.  (Layers are listed from\n  bottom to top in the SVG file.)\n\n### Release 0.1a3 (2017-11-10)\n\n#### PDFS\n\nReplace spaces and other shell-unfriendly characters with underscores\nin output file names.\n\n### Release 0.1a2 (2017-11-09)\n\nAdd sub-commands for generating random numbers.\n\n### Release 0.1a1 (2017-11-07)\n\nInitial release.\n"
 content-type = "text/markdown"
 
 [tool.pdm.version]
 source = "scm"
 write_to = "barnhunt/_version.py"
 write_template = "__version__ = \"{}\""
```

### Comparing `barnhunt-1.2.0rc6/stubs/pexpect/popen_spawn.pyi` & `barnhunt-1.2.1rc1/stubs/pexpect/popen_spawn.pyi`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/stubs/pexpect/spawnbase.pyi` & `barnhunt-1.2.1rc1/stubs/pexpect/spawnbase.pyi`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/conftest.py` & `barnhunt-1.2.1rc1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import shutil
 from pathlib import Path
 
 import pytest
 
-from barnhunt.cli import default_inkscape_command
+from barnhunt.inkscape.runner import get_default_inkscape_command
 
 
 @pytest.fixture
 def tests_dir() -> Path:
     return Path(__file__).parent
 
 
@@ -33,15 +33,15 @@
 def tmp_drawing_svg(tmp_path: Path, drawing_svg: Path) -> Path:
     tmp_drawing_svg = tmp_path / drawing_svg.name
     shutil.copyfile(drawing_svg, tmp_drawing_svg)
     return tmp_drawing_svg
 
 
 _inkscape_executable = shutil.which(
-    os.environ.get("INKSCAPE_COMMAND", default_inkscape_command())
+    os.environ.get("INKSCAPE_COMMAND", get_default_inkscape_command())
 )
 
 
 @pytest.fixture
 def inkscape_executable() -> str:
     """Path to inkscape executable."""
     if _inkscape_executable is None:
```

### Comparing `barnhunt-1.2.0rc6/tests/drawing.svg` & `barnhunt-1.2.1rc1/tests/drawing.svg`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/inkscape/dummy_inkscape.py` & `barnhunt-1.2.1rc1/tests/inkscape/dummy_inkscape.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/inkscape/test_css.py` & `barnhunt-1.2.1rc1/tests/inkscape/test_css.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/inkscape/test_runner.py` & `barnhunt-1.2.1rc1/tests/inkscape/test_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,52 @@
 import pytest
 
 from barnhunt.inkscape.runner import CliRunner
 from barnhunt.inkscape.runner import dwim_old_inkscape
 from barnhunt.inkscape.runner import ExportPdfCommand
 from barnhunt.inkscape.runner import ExportPdfCommand_0_9x
 from barnhunt.inkscape.runner import ExportPdfCommand_1_0
+from barnhunt.inkscape.runner import get_default_inkscape_command
+from barnhunt.inkscape.runner import get_default_shell_mode
 from barnhunt.inkscape.runner import inkscape_runner
 from barnhunt.inkscape.runner import InkscapeApi
 from barnhunt.inkscape.runner import log_output
 from barnhunt.inkscape.runner import Runner
 from barnhunt.inkscape.runner import ShellModeRunner
 
 
+@pytest.mark.parametrize(
+    "platform, expect",
+    [
+        ("linux", "inkscape"),
+        ("win32", "inkscape.exe"),
+    ],
+)
+def test_get_default_inkscape_command(
+    platform: str, expect: str, monkeypatch: pytest.MonkeyPatch
+) -> None:
+    monkeypatch.delitem(os.environ, "INKSCAPE_COMMAND", raising=False)
+    monkeypatch.setattr("sys.platform", platform)
+    assert get_default_inkscape_command() == expect
+
+
+@pytest.mark.parametrize(
+    "platform, expect",
+    [
+        ("linux", True),
+        ("darwin", False),
+    ],
+)
+def test_get_default_shell_mode(
+    platform: str, expect: bool, monkeypatch: pytest.MonkeyPatch
+) -> None:
+    monkeypatch.setattr("sys.platform", platform)
+    assert get_default_shell_mode() is expect
+
+
 class TestExportPdfCommand:
     @pytest.fixture(params=[ExportPdfCommand_0_9x, ExportPdfCommand_1_0])
     def command_class(self, request: pytest.FixtureRequest) -> ExportPdfCommand:
         return request.param  # type: ignore[no-any-return]
 
     def test_no_pdf_version(self, command_class: Type[ExportPdfCommand]) -> None:
         command = command_class("in.svg", "out.pdf")
```

### Comparing `barnhunt-1.2.0rc6/tests/inkscape/test_shell_mode_integration.py` & `barnhunt-1.2.1rc1/tests/inkscape/test_shell_mode_integration.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/inkscape/test_svg.py` & `barnhunt-1.2.1rc1/tests/inkscape/test_svg.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/inkscape/test_utils.py` & `barnhunt-1.2.1rc1/tests/inkscape/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import ctypes
+import inspect
 import os
 import re
 import sys
 from pathlib import Path
 from subprocess import CompletedProcess
 from types import ModuleType
 from types import SimpleNamespace
 
 import pytest
 from pytest_mock import MockerFixture
 
 from barnhunt.inkscape.utils import _get_appdata
 from barnhunt.inkscape.utils import get_default_user_data_directory
+from barnhunt.inkscape.utils import get_inkscape_debug_info
 from barnhunt.inkscape.utils import get_user_data_directory
 
 if sys.version_info >= (3, 8):
     from ctypes import wintypes
 else:
     wintypes = ModuleType("ctypes.wintypes")
     wintypes.HWND = ctypes.c_void_p
@@ -114,7 +116,53 @@
     assert default_user_data_directory.name == "inkscape"
 
 
 @pytest.mark.skipif(sys.platform != "win32", reason="not Windows system")
 def test_get_appdata(monkeypatch: pytest.MonkeyPatch) -> None:
     appdata = _get_appdata()
     assert Path(appdata).is_absolute()
+
+
+def test_get_inkscape_debug_info_no_inkscape() -> None:
+    info = dict(get_inkscape_debug_info("inkscape-is-not-installed"))
+    assert "not found" in info["which"]
+
+
+@pytest.fixture
+def dummy_script(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> None:
+    """Create a dummy script named "inkscape" in the PATH
+
+    The script will echo its arguments, and then exit with a non-zero exit code.
+
+    """
+    if sys.platform == "win32":
+        script_path = tmp_path / "inkscape.bat"
+        script_path.write_text(
+            inspect.cleandoc(
+                """@echo off
+                if "%~1" NEQ "" echo %*
+                echo "diagnostics" 1>&2
+                exit 1
+                """
+            )
+        )
+    else:
+        script_path = tmp_path / "inkscape"
+        script_path.write_text(
+            inspect.cleandoc(
+                """#!/bin/sh
+                echo "$*"
+                echo "diagnostics" 1>&2
+                exit 1
+                """
+            )
+        )
+        script_path.chmod(0o500)
+    monkeypatch.setenv("PATH", os.fspath(tmp_path))
+
+
+@pytest.mark.usefixtures("dummy_script")
+def test_get_inkscape_debug_info_old_inkscape() -> None:
+    info = dict(get_inkscape_debug_info("inkscape"))
+    assert "debug-info" not in info
+    assert "--version" in info["version"]
+    assert "diagnostics" in info["stderr⇒"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `barnhunt-1.2.0rc6/tests/installer/ratelimit.py` & `barnhunt-1.2.1rc1/tests/installer/ratelimit.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/installer/test_github.py` & `barnhunt-1.2.1rc1/tests/installer/test_github.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/installer/test_installer.py` & `barnhunt-1.2.1rc1/tests/installer/test_installer.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/installer/test_metadata.py` & `barnhunt-1.2.1rc1/tests/installer/test_metadata.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test1.pdf` & `barnhunt-1.2.1rc1/tests/test1.pdf`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test2.pdf` & `barnhunt-1.2.1rc1/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test_cli.py` & `barnhunt-1.2.1rc1/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,36 @@
 import os
-import subprocess
-import sys
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Iterator
 
 import click
 import pytest
 from click.testing import CliRunner
 from pytest_mock import MockerFixture
 
 from barnhunt.cli import _dump_loaded_modules
 from barnhunt.cli import barnhunt_cli
 from barnhunt.cli import default_2up_output_file
-from barnhunt.cli import default_inkscape_command
-from barnhunt.cli import default_shell_mode
 from barnhunt.cli import InkexRequirementType
 from barnhunt.cli import main
 from barnhunt.cli import pdf_2up
 from barnhunt.installer import DEFAULT_REQUIREMENTS
 from barnhunt.installer import InkexRequirement
 
 
-@pytest.mark.parametrize(
-    "platform, expect",
-    [
-        ("linux", "inkscape"),
-        ("win32", "inkscape.exe"),
-    ],
-)
-def test_default_inkscape_command(
-    platform: str, expect: str, monkeypatch: pytest.MonkeyPatch
-) -> None:
-    monkeypatch.delitem(os.environ, "INKSCAPE_COMMAND", raising=False)
-    monkeypatch.setattr("sys.platform", platform)
-    assert default_inkscape_command() == expect
-
-
-@pytest.mark.parametrize(
-    "platform, expect",
-    [
-        ("linux", True),
-        ("darwin", False),
-    ],
-)
-def test_default_shell_mode(
-    platform: str, expect: bool, monkeypatch: pytest.MonkeyPatch
-) -> None:
-    monkeypatch.setattr("sys.platform", platform)
-    assert default_shell_mode() is expect
-
-
 class Test_default_2up_output_file:
     @pytest.fixture
-    def ctx(self) -> Iterator[click.Context]:
-        with click.Context(pdf_2up) as ctx:
+    def resilient_parsing(self) -> bool:
+        return False
+
+    @pytest.fixture
+    def ctx(self, resilient_parsing: bool) -> Iterator[click.Context]:
+        with click.Context(pdf_2up, resilient_parsing=resilient_parsing) as ctx:
             yield ctx
 
     @pytest.fixture
     def add_input_file(
         self, ctx: click.Context, tmp_path: Path
     ) -> Callable[[str], Path]:
         def add_input_file(filename: str) -> Path:
@@ -88,33 +59,39 @@
         self, ctx: click.Context, add_input_file: Callable[[str], Path]
     ) -> None:
         add_input_file("input1.pdf")
         add_input_file("input2.pdf")
         with pytest.raises(click.UsageError, match="multiple input files"):
             default_2up_output_file()
 
+    @pytest.mark.parametrize("resilient_parsing", [True])
+    def test_resilient(self, ctx: click.Context) -> None:
+        assert default_2up_output_file() is None
+
+    def test_shell_completion(self) -> None:
+        runner = CliRunner()
+        result = runner.invoke(
+            barnhunt_cli,
+            args="2up",
+            env={
+                "_BARNHUNT_COMPLETE": "bash_complete",
+                "COMP_WORDS": "barnhunt 2up",
+                "COMP_CWORD": "2",
+            },
+        )
+        assert result.stdout.strip() == "file,"
+
 
 def test_main(capsys: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(SystemExit):
         main(["--help"])
     std = capsys.readouterr()
     assert "export pdfs from inkscape" in std.out.lower()
 
 
-def test_execute_python_c() -> None:
-    proc = subprocess.run(
-        [sys.executable, "-c", "from barnhunt.cli import main; main()", "--help"],
-        stdout=subprocess.PIPE,
-        text=True,
-        check=True,
-    )
-    assert "usage: barnhunt" in proc.stdout.lower()
-    assert proc.returncode == 0
-
-
 class Test_InkexRequirementType:
     CF = Callable[[Any], InkexRequirement]
 
     @pytest.fixture
     def allow_specifiers(self) -> bool:
         return True
 
@@ -160,15 +137,15 @@
     mocker.patch.dict("os.environ", GITHUB_TOKEN="token")
     target = tmp_path
     get_user_data_directory = mocker.patch(
         "barnhunt.cli.get_user_data_directory", return_value=target
     )
     Installer = mocker.patch("barnhunt.cli.Installer")
     runner = CliRunner()
-    result = runner.invoke(barnhunt_cli, ("install", "--inkscape", "myinkscape"))
+    result = runner.invoke(barnhunt_cli, ("--inkscape", "myinkscape", "install"))
     assert result.exit_code == 0
     get_user_data_directory.assert_called_once_with("myinkscape")
     Installer.assert_called_once_with(target, dry_run=False, github_token="token")
 
 
 def test_uninstall(mocker: MockerFixture, tmp_path: Path) -> None:
     Installer = mocker.patch("barnhunt.cli.Installer")
@@ -177,33 +154,38 @@
     assert result.exit_code == 0
     assert Installer.mock_calls == [
         mocker.call(tmp_path, dry_run=False),
         *(mocker.call().uninstall(req) for req in DEFAULT_REQUIREMENTS),
     ]
 
 
-def test_dump_loaded_modules_option(
-    tmp_path: Path, monkeypatch: pytest.MonkeyPatch
+def test_debug_info() -> None:
+    runner = CliRunner()
+    result = runner.invoke(barnhunt_cli, ("debug-info",))
+    assert result.exit_code == 0
+
+
+def test_main_dumps_loaded_modules(
+    tmp_path: Path, monkeypatch: pytest.MonkeyPatch, capsys: pytest.CaptureFixture[str]
 ) -> None:
     monkeypatch.chdir(tmp_path)
-    proc = subprocess.run(
-        [sys.executable, "-m", "barnhunt", "--dump-loaded-modules", "rats"],
-        capture_output=True,
-        text=True,
-        check=True,
-    )
-    assert "Dumped loaded modules" in proc.stderr
+    monkeypatch.setenv("BARNHUNT_DUMP_LOADED_MODULES", "true")
+    monkeypatch.setattr("sys.argv", ["-c", "--version"])
+    with pytest.raises(SystemExit) as exc_info:
+        main()
+    assert exc_info.value.code == 0
+    assert "Dumped loaded modules" in capsys.readouterr().err
     dumpfiles = [p for p in tmp_path.iterdir() if p.name.startswith("barnhunt-modules")]
     assert len(dumpfiles) == 1
     modules = set(dumpfiles[0].read_text("utf-8").splitlines())
     assert "pikepdf" in modules
 
 
 def test_dump_loaded_modules(
-    tmp_path: Path, monkeypatch: pytest.MonkeyPatch, caplog: pytest.LogCaptureFixture
+    tmp_path: Path, monkeypatch: pytest.MonkeyPatch, capsys: pytest.CaptureFixture[str]
 ) -> None:
     monkeypatch.chdir(tmp_path)
     _dump_loaded_modules()
-    assert len(caplog.records) == 1
-    assert "Dumped loaded modules" in caplog.text
+    captured = capsys.readouterr()
+    assert "Dumped loaded modules" in captured.err
     dumpfiles = [p for p in tmp_path.iterdir() if p.name.startswith("barnhunt-modules")]
     assert len(dumpfiles) == 1
```

### Comparing `barnhunt-1.2.0rc6/tests/test_coursemaps.py` & `barnhunt-1.2.1rc1/tests/test_coursemaps.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test_functional.py` & `barnhunt-1.2.1rc1/tests/test_functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     tmp_path: Path, caplog: pytest.LogCaptureFixture, processes: str | None
 ) -> None:
     caplog.set_level(logging.INFO)
     here = os.path.dirname(__file__)
     drawing_svg = os.path.join(here, "drawing.svg")
     cmd = ["pdfs", "-o", os.fspath(tmp_path), drawing_svg]
     if processes is not None:
-        cmd[1:1] = ["-p", processes]
+        cmd[0:0] = ["-p", processes]
     runner = CliRunner()
     result = runner.invoke(barnhunt_cli, cmd)
     assert result.exit_code == 0
     expected_pdfs = {
         "novice.pdf",
         "Master_1/Blind_1.pdf",
     }
```

### Comparing `barnhunt-1.2.0rc6/tests/test_layerinfo.py` & `barnhunt-1.2.1rc1/tests/test_layerinfo.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test_pager.py` & `barnhunt-1.2.1rc1/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test_pdfutil.py` & `barnhunt-1.2.1rc1/tests/test_pdfutil.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/test_templating.py` & `barnhunt-1.2.1rc1/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tests/testlib.py` & `barnhunt-1.2.1rc1/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/tox.ini` & `barnhunt-1.2.1rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc6/PKG-INFO` & `barnhunt-1.2.1rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barnhunt
-Version: 1.2.0rc6
+Version: 1.2.1rc1
 Summary: Helpers for drawing Barn Hunt course maps using Inkscape
 Keywords: barn hunt inkscape course maps
 Author-Email: Jeff Dairiki <dairiki@dairiki.org>
 License: GPL-3.0-only
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -13,33 +13,35 @@
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
 Project-URL: Homepage, https://github.com/barnhunt/barnhunt
 Requires-Python: >=3.7
 Requires-Dist: atomicwrites~=1.4
 Requires-Dist: click~=8.1
+Requires-Dist: importlib-metadata==4; python_version < "3.10"
 Requires-Dist: jinja2~=3.1
 Requires-Dist: lxml~=4.9
 Requires-Dist: marshmallow~=3.19
 Requires-Dist: marshmallow-dataclass~=8.5.13
 Requires-Dist: packaging~=23.1
 Requires-Dist: pexpect~=4.8
 Requires-Dist: pikepdf~=6.2
 Requires-Dist: requests~=2.29
 Requires-Dist: tinycss2~=1.2
 Requires-Dist: typing-extensions~=4.5; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # Barn Hunt Map Helper
 
-[![Tests](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml/badge.svg)](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml)
-[![PyPI Version](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)
-[![Inkscape Versions](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2-blue.svg?logo=inkscape)](https://inkscape.org/)
-[![PyPI Status](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Test status badge](https://img.shields.io/github/actions/workflow/status/barnhunt/barnhunt/ci.yml?label=tests)](https://github.com/barnhunt/barnhunt/actions/workflows/ci.yml)
+[![Latest version badge](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Supported Python versions badge](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Supported Inkscape versions badge](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2.2-blue.svg?logo=inkscape)](https://inkscape.org/)
+[![Development status badge](https://img.shields.io/pypi/status/barnhunt.svg)](https://pypi.org/project/barnhunt/)
+[![Trackgit-views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhapwefdbvler7yp5dsl)](https://trackgit.com)
 
 This is a helper script Jeff uses for drafting [Barn Hunt][] course
 maps.
 
 It does a bunch of stuff, but the important bit is that it exports PDF
 versions of maps from [Inkscape][] SVG files.
 
@@ -62,16 +64,45 @@
 (Due to a dependency on the [pikepdf][] package, it should work on
 x86_64-based Macs, but may not work on Macs that use Apple silicon. If
 pikepdf compatibility is an issue for you, let me know — it’s probably
 fixable.)
 
 ## Installation
 
+### Windows
+
+We now publish a compiled version of the program for Windows (which may
+even work.) Using this version has the advantage that Python is not required
+to be installed. (And even if Python is installed, this version may work-around
+some bugs having to do with the various different ways that Python can be
+installed on on Windows computer.)
+
+1. Browse to our [releases](https://github.com/barnhunt/barnhunt/releases/)
+   page. Select a release, and look down in the *Assets* section of the
+   release page. (You may have to click the triangle to expand the
+   *Assets* section.)
+
+2. Download the MSI installer (the filename should end with `.msi` —
+   e.g. `Barnhunt-1.2.0.49-x86_64-pc-windows-msvc.msi`). The file
+   is not signed, so you may have to click through some nasty warnings
+   about "unrecognized, potentially dangerous" files.
+
+3. Once downloaded, open (double-click) the file you just
+   downloaded. Hopefully and installer dialog should open.  Accept the
+   default choices.
+
+4. Now open a terminal command-line window. Type `barnhunt
+   --version`. If all is good, barnhunt should report its version. Run
+   `barnhunt --help` for the help screen.
+
+
+### Linux (or Windows with Python installed)
+
 As this package is published to
-[PyPI](https://pypi.org/project/barnhunt/) in may be installed into a
+[PyPI](https://pypi.org/project/barnhunt/) it may be installed into a
 [_virtualenv_][venv] using [`pip`][pip]. It is suggested that you use
 [`pipx`][pipx] to combine those two steps.
 
 A basic outline of how to proceed:
 
 1. Install [python][] if it is not already installed.  (Version 3.7 or
    greater is required.)
@@ -124,14 +155,45 @@
 [pipx]: https://pypa.github.io/pipx/ (The pipx home page)
 [pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)
 [pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html
 (The Installation section of the pikepdf documentation)
 
 ## Changes
 
+### Release 1.2.1rc1 (2023-05-22)
+
+(There was no final release of 1.2.0. It is a long story. I mistakenly
+committed a couple of files to LFS. To clear out LFS storage for a
+GitHub repo, one has to [delete the whole repo](😬). As a result, the
+workflow `$GITHUB_RUN_NUMBER` has reset. Thus a micro-version bump
+is required to keep those PyOxidizer windows build version numbers —
+`<major>.<minor>.<micro>.<run-number>` — monotonic.)
+
+[delete the whole repo]: https://docs.github.com/en/repositories/working-with-files/managing-large-files/removing-files-from-git-large-file-storage#git-lfs-objects-in-your-repository
+
+#### CLI Changes
+
+- The `--inkscape-command`, `--processes` and `--shell-mode-inkscape`
+  options have been moved from the `barnhunt pdfs` subcommand to the
+  man `barnhunt` command group.
+
+- And new `debug-info` subcommand has been added to display various
+  information about the installed version of the `barnhunt` command
+  and its execution environment.
+
+- The `--dump-loaded-modules` option has been removed.  The
+  functionality is still available by setting the
+  `$BARNHUNT_DUMP_LOADED_MODULES` environment variable to a non-empty
+  value.
+
+#### Bugs Fixed
+
+- Fixed exception in `barnhunt.cli.default_2up_output_file` during
+  shell-completion for `barnhunt 2up`.
+
 ### Release 1.2.0rc6 (2023-04-27)
 
 - Build an Windows executable and installer using [PyOxidizer].  The
   .msi installer should be downloadable from the
   [Releases](https://github.com/barnhunt/barnhunt/releases) page.
 
 - Added a `--dump-loaded-modules` option which causes `barnhunt` to
```

