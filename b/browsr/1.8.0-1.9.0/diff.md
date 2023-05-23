# Comparing `tmp/browsr-1.8.0.tar.gz` & `tmp/browsr-1.9.0.tar.gz`

## Comparing `browsr-1.8.0.tar` & `browsr-1.9.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 browsr-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.8.0/.releaserc.js
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.8.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/__main__.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_base.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_cli.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_config.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_tools.py
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_version.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/browsr.css
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/browsr.py
--rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/universal_directory_tree.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/contributing.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/index.md
--rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/browsr.png
--rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/browsr_no_label.png
--rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_datatable.png
--rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_markdown.png
--rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_mona_lisa.png
--rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_utils.png
--rw-r--r--   0        0        0   124812 2020-02-02 00:00:00.000000 browsr-1.8.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.8.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/helpers.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/test_config.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/test_screenshots.py
--rw-r--r--   0        0        0    12523 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/cassettes/test_github_screenshot.yaml
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/cassettes/test_github_screenshot_license.yaml
--rw-r--r--   0        0        0    35329 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/cassettes/test_textual_app_context_path_github.yaml
--rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/screenshots/test_github_screenshot.svg
--rw-r--r--   0        0        0    47130 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/screenshots/test_github_screenshot_license.svg
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.8.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.8.0/LICENSE
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 browsr-1.8.0/README.md
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 browsr-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 browsr-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 browsr-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.9.0/.releaserc.js
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.9.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.9.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/__main__.py
+-rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/_base.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/_config.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/_tools.py
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/browsr.css
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/browsr.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 browsr-1.9.0/browsr/universal_directory_tree.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.9.0/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   124812 2020-02-02 00:00:00.000000 browsr-1.9.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.9.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/helpers.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/test_config.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/test_screenshots.py
+-rw-r--r--   0        0        0    12523 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/cassettes/test_github_screenshot.yaml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/cassettes/test_github_screenshot_license.yaml
+-rw-r--r--   0        0        0    35329 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/cassettes/test_textual_app_context_path_github.yaml
+-rw-r--r--   0        0        0    62632 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/screenshots/test_github_screenshot.svg
+-rw-r--r--   0        0        0    47225 2020-02-02 00:00:00.000000 browsr-1.9.0/tests/screenshots/test_github_screenshot_license.svg
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 browsr-1.9.0/README.md
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 browsr-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 browsr-1.9.0/PKG-INFO
```

### Comparing `browsr-1.8.0/.pre-commit-config.yaml` & `browsr-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.releaserc.js` & `browsr-1.9.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/mkdocs.yaml` & `browsr-1.9.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.github/semantic_release/package-lock.json` & `browsr-1.9.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.github/semantic_release/release_notes.hbs` & `browsr-1.9.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.github/workflows/lint.yaml` & `browsr-1.9.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.github/workflows/publish.yaml` & `browsr-1.9.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.github/workflows/release.yaml` & `browsr-1.9.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/.github/workflows/tests.yaml` & `browsr-1.9.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/browsr/_base.py` & `browsr-1.9.0/browsr/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import numpy as np
 import upath
 from pandas import DataFrame
 from rich import traceback
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.text import Text
+from textual import on
 from textual.app import App, ComposeResult
 from textual.containers import Container
 from textual.reactive import reactive, var
 from textual.widget import Widget
 from textual.widgets import Button, DataTable, Static
 
 from browsr._config import favorite_themes
@@ -209,15 +210,16 @@
         Compose the Confirmation Pop Up
         """
         self.download_message = Static(Markdown(""))
         yield self.download_message
         yield Button("Yes", variant="success")
         yield Button("No", variant="error")
 
-    def on_button_pressed(self, event: Button.Pressed) -> None:
+    @on(Button.Pressed)
+    def handle_download_selection(self, message: Button.Pressed) -> None:
         """
         Handle Button Presses
         """
         self.app.confirmation_window.display = False  # type: ignore[attr-defined]
-        if event.button.variant == "success":
+        if message.button.variant == "success":
             self.app.download_selected_file()  # type: ignore[attr-defined]
         self.app.table_view.display = self.app.hidden_table_view  # type: ignore[attr-defined]
```

### Comparing `browsr-1.8.0/browsr/_cli.py` & `browsr-1.9.0/browsr/_cli.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/browsr/_config.py` & `browsr-1.9.0/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/browsr/_tools.py` & `browsr-1.9.0/browsr/_tools.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/browsr/_utils.py` & `browsr-1.9.0/browsr/_utils.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/browsr/browsr.css` & `browsr-1.9.0/browsr/browsr.css`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/browsr/browsr.py` & `browsr-1.9.0/browsr/browsr.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 import pandas as pd
 import upath
 from art import text2art  # type: ignore[import]
 from rich.markdown import Markdown
 from rich.syntax import Syntax
 from rich.traceback import Traceback
 from rich_pixels import Pixels
+from textual import on
 from textual.binding import Binding
 from textual.containers import Container, Horizontal, VerticalScroll
+from textual.events import Mount
 from textual.reactive import var
 from textual.widget import Widget
 from textual.widgets import DataTable, Footer, Header, Static
 from upath.implementations.cloud import CloudPath
 
 from browsr._base import (
     BrowsrTextualApp,
@@ -249,36 +251,38 @@
                 self.table_view.display = False
                 self.code_view.display = True
                 code_view.update(element)
             if scroll_home is True:
                 self.query_one("#code-view").scroll_home(animate=False)
             self.sub_title = f"{file_path} [{self.rich_themes[self.theme_index]}]"
 
-    def on_mount(self) -> None:
+    @on(Mount)
+    def start_up_app(self) -> None:
         """
         On Application Mount - See If a File Should be Displayed
         """
         if self.selected_file_path is not None:
             self.show_tree = self.force_show_tree
             self.render_code_page(file_path=self.selected_file_path)
         else:
             self.show_tree = True
             self.render_code_page(
                 file_path=pathlib.Path.cwd(), content=__application__.upper()
             )
 
-    def on_universal_directory_tree_file_selected(
-        self, event: UniversalDirectoryTree.FileSelected
+    @on(UniversalDirectoryTree.FileSelected)
+    def handle_file_selected(
+        self, message: UniversalDirectoryTree.FileSelected
     ) -> None:
         """
         Called when the user click a file in the directory tree.
         """
-        self.selected_file_path = upath.UPath(event.path)
+        self.selected_file_path = upath.UPath(message.path)
         file_info = get_file_info(file_path=self.selected_file_path)
-        self.render_code_page(file_path=upath.UPath(event.path))
+        self.render_code_page(file_path=upath.UPath(message.path))
         self.file_information.file_info = file_info
 
     def action_toggle_files(self) -> None:
         """
         Called in response to key binding.
         """
         self.show_tree = not self.show_tree
```

### Comparing `browsr-1.8.0/docs/contributing.md` & `browsr-1.9.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/gen_ref_pages.py` & `browsr-1.9.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/index.md` & `browsr-1.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/_static/browsr.png` & `browsr-1.9.0/docs/_static/browsr.png`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/_static/browsr_no_label.png` & `browsr-1.9.0/docs/_static/browsr_no_label.png`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/_static/screenshot_datatable.png` & `browsr-1.9.0/docs/_static/screenshot_datatable.png`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/_static/screenshot_markdown.png` & `browsr-1.9.0/docs/_static/screenshot_markdown.png`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/_static/screenshot_mona_lisa.png` & `browsr-1.9.0/docs/_static/screenshot_mona_lisa.png`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/docs/_static/screenshot_utils.png` & `browsr-1.9.0/docs/_static/screenshot_utils.png`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/requirements/requirements-dev.txt` & `browsr-1.9.0/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1518,17 +1518,17 @@
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
     #   vcrpy
-textual[dev]==0.24.1 \
-    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
-    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
+textual[dev]==0.25.0 \
+    --hash=sha256:5e2d6320026dd8ff86e0d023fc4988071e80ec2e34de913bd63263a8301d664b \
+    --hash=sha256:8258499a09793696e13a1d1e1391810916828015a91770abd7ce3d9ab64cfd9e
     # via -r requirements.in
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   black
     #   build
```

### Comparing `browsr-1.8.0/requirements/requirements-prod.txt` & `browsr-1.9.0/requirements/requirements-prod.txt`

 * *Files 0% similar despite different names*

```diff
@@ -961,17 +961,17 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual==0.24.1 \
-    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
-    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
+textual==0.25.0 \
+    --hash=sha256:5e2d6320026dd8ff86e0d023fc4988071e80ec2e34de913bd63263a8301d664b \
+    --hash=sha256:8258499a09793696e13a1d1e1391810916828015a91770abd7ce3d9ab64cfd9e
     # via -r requirements.in
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via
     #   azure-core
     #   azure-storage-blob
```

### Comparing `browsr-1.8.0/tests/conftest.py` & `browsr-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/tests/helpers.py` & `browsr-1.9.0/tests/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Helpers for the tests
 """
 
 import pathlib
-from os import environ
+from os import environ, getenv
 from typing import List, Optional, Tuple
 
 from browsr import Browsr
 from browsr._base import TextualAppContext
 from browsr._tools import take_screenshot
 
 
@@ -30,14 +30,16 @@
         self, press: Optional[List[str]] = None
     ) -> Tuple[str, pathlib.Path]:
         """
         Take a Screenshot
         """
         screenshot = take_screenshot(app=self.app, press=press)
         screenshot_path = self._get_screenshot_path()
+        if getenv("BROWSR_REGENERATE_SCREENSHOTS", "0") != "0":
+            screenshot_path.write_text(screenshot)
         return screenshot, screenshot_path
 
     @classmethod
     def _get_screenshot_path(cls) -> pathlib.Path:
         """
         Get the Screenshot Path
         """
```

### Comparing `browsr-1.8.0/tests/test_config.py` & `browsr-1.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/tests/test_screenshots.py` & `browsr-1.9.0/tests/test_screenshots.py`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/tests/cassettes/test_github_screenshot.yaml` & `browsr-1.9.0/tests/cassettes/test_github_screenshot.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/tests/cassettes/test_github_screenshot_license.yaml` & `browsr-1.9.0/tests/cassettes/test_github_screenshot_license.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/tests/cassettes/test_textual_app_context_path_github.yaml` & `browsr-1.9.0/tests/cassettes/test_textual_app_context_path_github.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/tests/screenshots/test_github_screenshot.svg` & `browsr-1.9.0/tests/screenshots/test_github_screenshot.svg`

 * *Files 12% similar despite different names*

```diff
@@ -54,3837 +54,3862 @@
 00000350: 302f 776f 6666 2f46 6972 6143 6f64 652d  0/woff/FiraCode-
 00000360: 426f 6c64 2e77 6f66 6622 2920 666f 726d  Bold.woff") form
 00000370: 6174 2822 776f 6666 2229 3b0a 2020 2020  at("woff");.    
 00000380: 2020 2020 666f 6e74 2d73 7479 6c65 3a20      font-style: 
 00000390: 626f 6c64 3b0a 2020 2020 2020 2020 666f  bold;.        fo
 000003a0: 6e74 2d77 6569 6768 743a 2037 3030 3b0a  nt-weight: 700;.
 000003b0: 2020 2020 7d0a 0a20 2020 202e 7465 726d      }..    .term
-000003c0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
+000003c0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
 000003d0: 6d61 7472 6978 207b 0a20 2020 2020 2020  matrix {.       
 000003e0: 2066 6f6e 742d 6661 6d69 6c79 3a20 4669   font-family: Fi
 000003f0: 7261 2043 6f64 652c 206d 6f6e 6f73 7061  ra Code, monospa
 00000400: 6365 3b0a 2020 2020 2020 2020 666f 6e74  ce;.        font
 00000410: 2d73 697a 653a 2032 3070 783b 0a20 2020  -size: 20px;.   
 00000420: 2020 2020 206c 696e 652d 6865 6967 6874       line-height
 00000430: 3a20 3234 2e34 7078 3b0a 2020 2020 2020  : 24.4px;.      
 00000440: 2020 666f 6e74 2d76 6172 6961 6e74 2d65    font-variant-e
 00000450: 6173 742d 6173 6961 6e3a 2066 756c 6c2d  ast-asian: full-
 00000460: 7769 6474 683b 0a20 2020 207d 0a0a 2020  width;.    }..  
-00000470: 2020 2e74 6572 6d69 6e61 6c2d 3137 3234    .terminal-1724
-00000480: 3735 3934 3635 2d74 6974 6c65 207b 0a20  759465-title {. 
+00000470: 2020 2e74 6572 6d69 6e61 6c2d 3231 3637    .terminal-2167
+00000480: 3038 3133 3630 2d74 6974 6c65 207b 0a20  081360-title {. 
 00000490: 2020 2020 2020 2066 6f6e 742d 7369 7a65         font-size
 000004a0: 3a20 3138 7078 3b0a 2020 2020 2020 2020  : 18px;.        
 000004b0: 666f 6e74 2d77 6569 6768 743a 2062 6f6c  font-weight: bol
 000004c0: 643b 0a20 2020 2020 2020 2066 6f6e 742d  d;.        font-
 000004d0: 6661 6d69 6c79 3a20 6172 6961 6c3b 0a20  family: arial;. 
 000004e0: 2020 207d 0a0a 2020 2020 2e74 6572 6d69     }..    .termi
-000004f0: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
+000004f0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
 00000500: 3120 7b20 6669 6c6c 3a20 2363 3563 3863  1 { fill: #c5c8c
-00000510: 3620 7d0a 2e74 6572 6d69 6e61 6c2d 3137  6 }..terminal-17
-00000520: 3234 3735 3934 3635 2d72 3220 7b20 6669  24759465-r2 { fi
+00000510: 3620 7d0a 2e74 6572 6d69 6e61 6c2d 3231  6 }..terminal-21
+00000520: 3637 3038 3133 3630 2d72 3220 7b20 6669  67081360-r2 { fi
 00000530: 6c6c 3a20 2365 3065 3065 3020 7d0a 2e74  ll: #e0e0e0 }..t
-00000540: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-00000550: 3635 2d72 3320 7b20 6669 6c6c 3a20 2339  65-r3 { fill: #9
+00000540: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00000550: 3630 2d72 3320 7b20 6669 6c6c 3a20 2339  60-r3 { fill: #9
 00000560: 3039 3039 3020 7d0a 2e74 6572 6d69 6e61  09090 }..termina
-00000570: 6c2d 3137 3234 3735 3934 3635 2d72 3420  l-1724759465-r4 
+00000570: 6c2d 3231 3637 3038 3133 3630 2d72 3420  l-2167081360-r4 
 00000580: 7b20 6669 6c6c 3a20 2365 3265 3365 3320  { fill: #e2e3e3 
-00000590: 7d0a 2e74 6572 6d69 6e61 6c2d 3137 3234  }..terminal-1724
-000005a0: 3735 3934 3635 2d72 3520 7b20 6669 6c6c  759465-r5 { fill
-000005b0: 3a20 2331 6131 3030 303b 666f 6e74 2d77  : #1a1000;font-w
+00000590: 7d0a 2e74 6572 6d69 6e61 6c2d 3231 3637  }..terminal-2167
+000005a0: 3038 3133 3630 2d72 3520 7b20 6669 6c6c  081360-r5 { fill
+000005b0: 3a20 2332 3131 3530 353b 666f 6e74 2d77  : #211505;font-w
 000005c0: 6569 6768 743a 2062 6f6c 6420 7d0a 2e74  eight: bold }..t
-000005d0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-000005e0: 3635 2d72 3620 7b20 6669 6c6c 3a20 2364  65-r6 { fill: #d
+000005d0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+000005e0: 3630 2d72 3620 7b20 6669 6c6c 3a20 2364  60-r6 { fill: #d
 000005f0: 6664 6664 6620 7d0a 2e74 6572 6d69 6e61  fdfdf }..termina
-00000600: 6c2d 3137 3234 3735 3934 3635 2d72 3720  l-1724759465-r7 
-00000610: 7b20 6669 6c6c 3a20 2330 3038 3133 3920  { fill: #008139 
-00000620: 7d0a 2e74 6572 6d69 6e61 6c2d 3137 3234  }..terminal-1724
-00000630: 3735 3934 3635 2d72 3820 7b20 6669 6c6c  759465-r8 { fill
-00000640: 3a20 2339 3139 3439 373b 666f 6e74 2d77  : #919497;font-w
-00000650: 6569 6768 743a 2062 6f6c 6420 7d0a 2e74  eight: bold }..t
-00000660: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-00000670: 3635 2d72 3920 7b20 6669 6c6c 3a20 2364  65-r9 { fill: #d
-00000680: 6664 6664 663b 666f 6e74 2d77 6569 6768  fdfdf;font-weigh
-00000690: 743a 2062 6f6c 6420 7d0a 2e74 6572 6d69  t: bold }..termi
-000006a0: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-000006b0: 3130 207b 2066 696c 6c3a 2023 6532 6533  10 { fill: #e2e3
-000006c0: 6533 3b66 6f6e 742d 7765 6967 6874 3a20  e3;font-weight: 
-000006d0: 626f 6c64 207d 0a2e 7465 726d 696e 616c  bold }..terminal
-000006e0: 2d31 3732 3437 3539 3436 352d 7231 3120  -1724759465-r11 
-000006f0: 7b20 6669 6c6c 3a20 2336 3038 6162 313b  { fill: #608ab1;
-00000700: 7465 7874 2d64 6563 6f72 6174 696f 6e3a  text-decoration:
-00000710: 2075 6e64 6572 6c69 6e65 3b20 7d0a 2e74   underline; }..t
-00000720: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-00000730: 3635 2d72 3132 207b 2066 696c 6c3a 2023  65-r12 { fill: #
-00000740: 3931 3934 3937 3b66 6f6e 742d 7374 796c  919497;font-styl
-00000750: 653a 2069 7461 6c69 633b 207d 0a2e 7465  e: italic; }..te
-00000760: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00000770: 352d 7231 3320 7b20 6669 6c6c 3a20 2336  5-r13 { fill: #6
-00000780: 3861 3062 333b 666f 6e74 2d77 6569 6768  8a0b3;font-weigh
-00000790: 743a 2062 6f6c 6420 7d0a 2e74 6572 6d69  t: bold }..termi
-000007a0: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-000007b0: 3134 207b 2066 696c 6c3a 2023 6532 6533  14 { fill: #e2e3
-000007c0: 6533 3b66 6f6e 742d 7374 796c 653a 2069  e3;font-style: i
-000007d0: 7461 6c69 633b 207d 0a2e 7465 726d 696e  talic; }..termin
-000007e0: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-000007f0: 3520 7b20 6669 6c6c 3a20 2364 6664 6664  5 { fill: #dfdfd
-00000800: 663b 666f 6e74 2d77 6569 6768 743a 2062  f;font-weight: b
-00000810: 6f6c 643b 7465 7874 2d64 6563 6f72 6174  old;text-decorat
-00000820: 696f 6e3a 2075 6e64 6572 6c69 6e65 3b20  ion: underline; 
-00000830: 7d0a 2e74 6572 6d69 6e61 6c2d 3137 3234  }..terminal-1724
-00000840: 3735 3934 3635 2d72 3136 207b 2066 696c  759465-r16 { fil
-00000850: 6c3a 2023 6638 6638 6632 207d 0a2e 7465  l: #f8f8f2 }..te
-00000860: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00000870: 352d 7231 3720 7b20 6669 6c6c 3a20 2365  5-r17 { fill: #e
-00000880: 3664 6237 3420 7d0a 2e74 6572 6d69 6e61  6db74 }..termina
-00000890: 6c2d 3137 3234 3735 3934 3635 2d72 3138  l-1724759465-r18
-000008a0: 207b 2066 696c 6c3a 2023 3134 3139 3166   { fill: #14191f
-000008b0: 207d 0a2e 7465 726d 696e 616c 2d31 3732   }..terminal-172
-000008c0: 3437 3539 3436 352d 7231 3920 7b20 6669  4759465-r19 { fi
-000008d0: 6c6c 3a20 2338 3461 3463 6320 7d0a 2e74  ll: #84a4cc }..t
-000008e0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-000008f0: 3635 2d72 3230 207b 2066 696c 6c3a 2023  65-r20 { fill: #
-00000900: 6464 6538 6633 3b66 6f6e 742d 7765 6967  dde8f3;font-weig
-00000910: 6874 3a20 626f 6c64 207d 0a2e 7465 726d  ht: bold }..term
-00000920: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-00000930: 7232 3120 7b20 6669 6c6c 3a20 2364 6465  r21 { fill: #dde
-00000940: 6466 3920 7d0a 2020 2020 3c2f 7374 796c  df9 }.    </styl
-00000950: 653e 0a0a 2020 2020 3c64 6566 733e 0a20  e>..    <defs>. 
-00000960: 2020 203c 636c 6970 5061 7468 2069 643d     <clipPath id=
-00000970: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00000980: 3934 3635 2d63 6c69 702d 7465 726d 696e  9465-clip-termin
-00000990: 616c 223e 0a20 2020 2020 203c 7265 6374  al">.      <rect
-000009a0: 2078 3d22 3022 2079 3d22 3022 2077 6964   x="0" y="0" wid
-000009b0: 7468 3d22 3139 3531 2e30 2220 6865 6967  th="1951.0" heig
-000009c0: 6874 3d22 3131 3730 2e31 3939 3939 3939  ht="1170.1999999
-000009d0: 3939 3939 3938 2220 2f3e 0a20 2020 203c  999998" />.    <
-000009e0: 2f63 6c69 7050 6174 683e 0a20 2020 203c  /clipPath>.    <
-000009f0: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00000a00: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00000a10: 2d6c 696e 652d 3022 3e0a 2020 2020 3c72  -line-0">.    <r
-00000a20: 6563 7420 783d 2230 2220 793d 2231 2e35  ect x="0" y="1.5
-00000a30: 2220 7769 6474 683d 2231 3935 3222 2068  " width="1952" h
-00000a40: 6569 6768 743d 2232 342e 3635 222f 3e0a  eight="24.65"/>.
-00000a50: 2020 2020 2020 2020 2020 2020 3c2f 636c              </cl
-00000a60: 6970 5061 7468 3e0a 3c63 6c69 7050 6174  ipPath>.<clipPat
-00000a70: 6820 6964 3d22 7465 726d 696e 616c 2d31  h id="terminal-1
-00000a80: 3732 3437 3539 3436 352d 6c69 6e65 2d31  724759465-line-1
-00000a90: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-00000aa0: 3022 2079 3d22 3235 2e39 2220 7769 6474  0" y="25.9" widt
-00000ab0: 683d 2231 3935 3222 2068 6569 6768 743d  h="1952" height=
-00000ac0: 2232 342e 3635 222f 3e0a 2020 2020 2020  "24.65"/>.      
-00000ad0: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
-00000ae0: 3e0a 3c63 6c69 7050 6174 6820 6964 3d22  >.<clipPath id="
-00000af0: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-00000b00: 3436 352d 6c69 6e65 2d32 223e 0a20 2020  465-line-2">.   
-00000b10: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
-00000b20: 3530 2e33 2220 7769 6474 683d 2231 3935  50.3" width="195
-00000b30: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00000b40: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00000b50: 3c2f 636c 6970 5061 7468 3e0a 3c63 6c69  </clipPath>.<cli
-00000b60: 7050 6174 6820 6964 3d22 7465 726d 696e  pPath id="termin
-00000b70: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-00000b80: 6e65 2d33 223e 0a20 2020 203c 7265 6374  ne-3">.    <rect
-00000b90: 2078 3d22 3022 2079 3d22 3734 2e37 2220   x="0" y="74.7" 
-00000ba0: 7769 6474 683d 2231 3935 3222 2068 6569  width="1952" hei
-00000bb0: 6768 743d 2232 342e 3635 222f 3e0a 2020  ght="24.65"/>.  
-00000bc0: 2020 2020 2020 2020 2020 3c2f 636c 6970            </clip
-00000bd0: 5061 7468 3e0a 3c63 6c69 7050 6174 6820  Path>.<clipPath 
-00000be0: 6964 3d22 7465 726d 696e 616c 2d31 3732  id="terminal-172
-00000bf0: 3437 3539 3436 352d 6c69 6e65 2d34 223e  4759465-line-4">
-00000c00: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
-00000c10: 2079 3d22 3939 2e31 2220 7769 6474 683d   y="99.1" width=
-00000c20: 2231 3935 3222 2068 6569 6768 743d 2232  "1952" height="2
-00000c30: 342e 3635 222f 3e0a 2020 2020 2020 2020  4.65"/>.        
-00000c40: 2020 2020 3c2f 636c 6970 5061 7468 3e0a      </clipPath>.
-00000c50: 3c63 6c69 7050 6174 6820 6964 3d22 7465  <clipPath id="te
-00000c60: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00000c70: 352d 6c69 6e65 2d35 223e 0a20 2020 203c  5-line-5">.    <
-00000c80: 7265 6374 2078 3d22 3022 2079 3d22 3132  rect x="0" y="12
-00000c90: 332e 3522 2077 6964 7468 3d22 3139 3532  3.5" width="1952
-00000ca0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00000cb0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00000cc0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00000cd0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00000ce0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00000cf0: 652d 3622 3e0a 2020 2020 3c72 6563 7420  e-6">.    <rect 
-00000d00: 783d 2230 2220 793d 2231 3437 2e39 2220  x="0" y="147.9" 
-00000d10: 7769 6474 683d 2231 3935 3222 2068 6569  width="1952" hei
-00000d20: 6768 743d 2232 342e 3635 222f 3e0a 2020  ght="24.65"/>.  
-00000d30: 2020 2020 2020 2020 2020 3c2f 636c 6970            </clip
-00000d40: 5061 7468 3e0a 3c63 6c69 7050 6174 6820  Path>.<clipPath 
-00000d50: 6964 3d22 7465 726d 696e 616c 2d31 3732  id="terminal-172
-00000d60: 3437 3539 3436 352d 6c69 6e65 2d37 223e  4759465-line-7">
-00000d70: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
-00000d80: 2079 3d22 3137 322e 3322 2077 6964 7468   y="172.3" width
-00000d90: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
-00000da0: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
-00000db0: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
-00000dc0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
-00000dd0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-00000de0: 3635 2d6c 696e 652d 3822 3e0a 2020 2020  65-line-8">.    
-00000df0: 3c72 6563 7420 783d 2230 2220 793d 2231  <rect x="0" y="1
-00000e00: 3936 2e37 2220 7769 6474 683d 2231 3935  96.7" width="195
-00000e10: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00000e20: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00000e30: 3c2f 636c 6970 5061 7468 3e0a 3c63 6c69  </clipPath>.<cli
-00000e40: 7050 6174 6820 6964 3d22 7465 726d 696e  pPath id="termin
-00000e50: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-00000e60: 6e65 2d39 223e 0a20 2020 203c 7265 6374  ne-9">.    <rect
-00000e70: 2078 3d22 3022 2079 3d22 3232 312e 3122   x="0" y="221.1"
-00000e80: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00000e90: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00000ea0: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00000eb0: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-00000ec0: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-00000ed0: 3234 3735 3934 3635 2d6c 696e 652d 3130  24759465-line-10
-00000ee0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-00000ef0: 3022 2079 3d22 3234 352e 3522 2077 6964  0" y="245.5" wid
-00000f00: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-00000f10: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-00000f20: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00000f30: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00000f40: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00000f50: 3934 3635 2d6c 696e 652d 3131 223e 0a20  9465-line-11">. 
-00000f60: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00000f70: 3d22 3236 392e 3922 2077 6964 7468 3d22  ="269.9" width="
-00000f80: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00000f90: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00000fa0: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00000fb0: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00000fc0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00000fd0: 2d6c 696e 652d 3132 223e 0a20 2020 203c  -line-12">.    <
-00000fe0: 7265 6374 2078 3d22 3022 2079 3d22 3239  rect x="0" y="29
-00000ff0: 342e 3322 2077 6964 7468 3d22 3139 3532  4.3" width="1952
-00001000: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00001010: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001020: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00001030: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001040: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001050: 652d 3133 223e 0a20 2020 203c 7265 6374  e-13">.    <rect
-00001060: 2078 3d22 3022 2079 3d22 3331 382e 3722   x="0" y="318.7"
-00001070: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001080: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001090: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-000010a0: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-000010b0: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-000010c0: 3234 3735 3934 3635 2d6c 696e 652d 3134  24759465-line-14
-000010d0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-000010e0: 3022 2079 3d22 3334 332e 3122 2077 6964  0" y="343.1" wid
-000010f0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-00001100: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-00001110: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00001120: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00001130: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001140: 3934 3635 2d6c 696e 652d 3135 223e 0a20  9465-line-15">. 
-00001150: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001160: 3d22 3336 372e 3522 2077 6964 7468 3d22  ="367.5" width="
-00001170: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001180: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001190: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-000011a0: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-000011b0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-000011c0: 2d6c 696e 652d 3136 223e 0a20 2020 203c  -line-16">.    <
-000011d0: 7265 6374 2078 3d22 3022 2079 3d22 3339  rect x="0" y="39
-000011e0: 312e 3922 2077 6964 7468 3d22 3139 3532  1.9" width="1952
-000011f0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00001200: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001210: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00001220: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001230: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001240: 652d 3137 223e 0a20 2020 203c 7265 6374  e-17">.    <rect
-00001250: 2078 3d22 3022 2079 3d22 3431 362e 3322   x="0" y="416.3"
-00001260: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001270: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001280: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00001290: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-000012a0: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-000012b0: 3234 3735 3934 3635 2d6c 696e 652d 3138  24759465-line-18
-000012c0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-000012d0: 3022 2079 3d22 3434 302e 3722 2077 6964  0" y="440.7" wid
-000012e0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-000012f0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-00001300: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00001310: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00001320: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001330: 3934 3635 2d6c 696e 652d 3139 223e 0a20  9465-line-19">. 
-00001340: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001350: 3d22 3436 352e 3122 2077 6964 7468 3d22  ="465.1" width="
-00001360: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001370: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001380: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001390: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-000013a0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-000013b0: 2d6c 696e 652d 3230 223e 0a20 2020 203c  -line-20">.    <
-000013c0: 7265 6374 2078 3d22 3022 2079 3d22 3438  rect x="0" y="48
-000013d0: 392e 3522 2077 6964 7468 3d22 3139 3532  9.5" width="1952
-000013e0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000013f0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001400: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00001410: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001420: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001430: 652d 3231 223e 0a20 2020 203c 7265 6374  e-21">.    <rect
-00001440: 2078 3d22 3022 2079 3d22 3531 332e 3922   x="0" y="513.9"
-00001450: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001460: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001470: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00001480: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-00001490: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-000014a0: 3234 3735 3934 3635 2d6c 696e 652d 3232  24759465-line-22
-000014b0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-000014c0: 3022 2079 3d22 3533 382e 3322 2077 6964  0" y="538.3" wid
-000014d0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-000014e0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-000014f0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00001500: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00001510: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001520: 3934 3635 2d6c 696e 652d 3233 223e 0a20  9465-line-23">. 
-00001530: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001540: 3d22 3536 322e 3722 2077 6964 7468 3d22  ="562.7" width="
-00001550: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001560: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001570: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001580: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00001590: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-000015a0: 2d6c 696e 652d 3234 223e 0a20 2020 203c  -line-24">.    <
-000015b0: 7265 6374 2078 3d22 3022 2079 3d22 3538  rect x="0" y="58
-000015c0: 372e 3122 2077 6964 7468 3d22 3139 3532  7.1" width="1952
-000015d0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000015e0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000015f0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00001600: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001610: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001620: 652d 3235 223e 0a20 2020 203c 7265 6374  e-25">.    <rect
-00001630: 2078 3d22 3022 2079 3d22 3631 312e 3522   x="0" y="611.5"
-00001640: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001650: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001660: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00001670: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-00001680: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-00001690: 3234 3735 3934 3635 2d6c 696e 652d 3236  24759465-line-26
-000016a0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-000016b0: 3022 2079 3d22 3633 352e 3922 2077 6964  0" y="635.9" wid
-000016c0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-000016d0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-000016e0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-000016f0: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00001700: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001710: 3934 3635 2d6c 696e 652d 3237 223e 0a20  9465-line-27">. 
-00001720: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001730: 3d22 3636 302e 3322 2077 6964 7468 3d22  ="660.3" width="
-00001740: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001750: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001760: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001770: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00001780: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00001790: 2d6c 696e 652d 3238 223e 0a20 2020 203c  -line-28">.    <
-000017a0: 7265 6374 2078 3d22 3022 2079 3d22 3638  rect x="0" y="68
-000017b0: 342e 3722 2077 6964 7468 3d22 3139 3532  4.7" width="1952
-000017c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000017d0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000017e0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-000017f0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001800: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001810: 652d 3239 223e 0a20 2020 203c 7265 6374  e-29">.    <rect
-00001820: 2078 3d22 3022 2079 3d22 3730 392e 3122   x="0" y="709.1"
-00001830: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001840: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001850: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00001860: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-00001870: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-00001880: 3234 3735 3934 3635 2d6c 696e 652d 3330  24759465-line-30
-00001890: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-000018a0: 3022 2079 3d22 3733 332e 3522 2077 6964  0" y="733.5" wid
-000018b0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-000018c0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-000018d0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-000018e0: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-000018f0: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001900: 3934 3635 2d6c 696e 652d 3331 223e 0a20  9465-line-31">. 
-00001910: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001920: 3d22 3735 372e 3922 2077 6964 7468 3d22  ="757.9" width="
-00001930: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001940: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001950: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001960: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00001970: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00001980: 2d6c 696e 652d 3332 223e 0a20 2020 203c  -line-32">.    <
-00001990: 7265 6374 2078 3d22 3022 2079 3d22 3738  rect x="0" y="78
-000019a0: 322e 3322 2077 6964 7468 3d22 3139 3532  2.3" width="1952
-000019b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000019c0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000019d0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-000019e0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-000019f0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001a00: 652d 3333 223e 0a20 2020 203c 7265 6374  e-33">.    <rect
-00001a10: 2078 3d22 3022 2079 3d22 3830 362e 3722   x="0" y="806.7"
-00001a20: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001a30: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001a40: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00001a50: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-00001a60: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-00001a70: 3234 3735 3934 3635 2d6c 696e 652d 3334  24759465-line-34
-00001a80: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-00001a90: 3022 2079 3d22 3833 312e 3122 2077 6964  0" y="831.1" wid
-00001aa0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-00001ab0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-00001ac0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00001ad0: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00001ae0: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001af0: 3934 3635 2d6c 696e 652d 3335 223e 0a20  9465-line-35">. 
-00001b00: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001b10: 3d22 3835 352e 3522 2077 6964 7468 3d22  ="855.5" width="
-00001b20: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001b30: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001b40: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001b50: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00001b60: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00001b70: 2d6c 696e 652d 3336 223e 0a20 2020 203c  -line-36">.    <
-00001b80: 7265 6374 2078 3d22 3022 2079 3d22 3837  rect x="0" y="87
-00001b90: 392e 3922 2077 6964 7468 3d22 3139 3532  9.9" width="1952
-00001ba0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00001bb0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001bc0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00001bd0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001be0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001bf0: 652d 3337 223e 0a20 2020 203c 7265 6374  e-37">.    <rect
-00001c00: 2078 3d22 3022 2079 3d22 3930 342e 3322   x="0" y="904.3"
-00001c10: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
-00001c20: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
-00001c30: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
-00001c40: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-00001c50: 2069 643d 2274 6572 6d69 6e61 6c2d 3137   id="terminal-17
-00001c60: 3234 3735 3934 3635 2d6c 696e 652d 3338  24759465-line-38
-00001c70: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
-00001c80: 3022 2079 3d22 3932 382e 3722 2077 6964  0" y="928.7" wid
-00001c90: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
-00001ca0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
-00001cb0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00001cc0: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00001cd0: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-00001ce0: 3934 3635 2d6c 696e 652d 3339 223e 0a20  9465-line-39">. 
-00001cf0: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
-00001d00: 3d22 3935 332e 3122 2077 6964 7468 3d22  ="953.1" width="
-00001d10: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001d20: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001d30: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001d40: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00001d50: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00001d60: 2d6c 696e 652d 3430 223e 0a20 2020 203c  -line-40">.    <
-00001d70: 7265 6374 2078 3d22 3022 2079 3d22 3937  rect x="0" y="97
-00001d80: 372e 3522 2077 6964 7468 3d22 3139 3532  7.5" width="1952
-00001d90: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00001da0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001db0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
-00001dc0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001dd0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00001de0: 652d 3431 223e 0a20 2020 203c 7265 6374  e-41">.    <rect
-00001df0: 2078 3d22 3022 2079 3d22 3130 3031 2e39   x="0" y="1001.9
-00001e00: 2220 7769 6474 683d 2231 3935 3222 2068  " width="1952" h
-00001e10: 6569 6768 743d 2232 342e 3635 222f 3e0a  eight="24.65"/>.
-00001e20: 2020 2020 2020 2020 2020 2020 3c2f 636c              </cl
-00001e30: 6970 5061 7468 3e0a 3c63 6c69 7050 6174  ipPath>.<clipPat
-00001e40: 6820 6964 3d22 7465 726d 696e 616c 2d31  h id="terminal-1
-00001e50: 3732 3437 3539 3436 352d 6c69 6e65 2d34  724759465-line-4
-00001e60: 3222 3e0a 2020 2020 3c72 6563 7420 783d  2">.    <rect x=
-00001e70: 2230 2220 793d 2231 3032 362e 3322 2077  "0" y="1026.3" w
-00001e80: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
-00001e90: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
-00001ea0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
-00001eb0: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
-00001ec0: 643d 2274 6572 6d69 6e61 6c2d 3137 3234  d="terminal-1724
-00001ed0: 3735 3934 3635 2d6c 696e 652d 3433 223e  759465-line-43">
-00001ee0: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
-00001ef0: 2079 3d22 3130 3530 2e37 2220 7769 6474   y="1050.7" widt
-00001f00: 683d 2231 3935 3222 2068 6569 6768 743d  h="1952" height=
-00001f10: 2232 342e 3635 222f 3e0a 2020 2020 2020  "24.65"/>.      
-00001f20: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
-00001f30: 3e0a 3c63 6c69 7050 6174 6820 6964 3d22  >.<clipPath id="
-00001f40: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-00001f50: 3436 352d 6c69 6e65 2d34 3422 3e0a 2020  465-line-44">.  
-00001f60: 2020 3c72 6563 7420 783d 2230 2220 793d    <rect x="0" y=
-00001f70: 2231 3037 352e 3122 2077 6964 7468 3d22  "1075.1" width="
-00001f80: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
-00001f90: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
-00001fa0: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
-00001fb0: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00001fc0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00001fd0: 2d6c 696e 652d 3435 223e 0a20 2020 203c  -line-45">.    <
-00001fe0: 7265 6374 2078 3d22 3022 2079 3d22 3130  rect x="0" y="10
-00001ff0: 3939 2e35 2220 7769 6474 683d 2231 3935  99.5" width="195
-00002000: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00002010: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002020: 3c2f 636c 6970 5061 7468 3e0a 3c63 6c69  </clipPath>.<cli
-00002030: 7050 6174 6820 6964 3d22 7465 726d 696e  pPath id="termin
-00002040: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-00002050: 6e65 2d34 3622 3e0a 2020 2020 3c72 6563  ne-46">.    <rec
-00002060: 7420 783d 2230 2220 793d 2231 3132 332e  t x="0" y="1123.
-00002070: 3922 2077 6964 7468 3d22 3139 3532 2220  9" width="1952" 
-00002080: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
-00002090: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
-000020a0: 6c69 7050 6174 683e 0a20 2020 203c 2f64  lipPath>.    </d
-000020b0: 6566 733e 0a0a 2020 2020 3c72 6563 7420  efs>..    <rect 
-000020c0: 6669 6c6c 3d22 2332 3932 3932 3922 2073  fill="#292929" s
-000020d0: 7472 6f6b 653d 2272 6762 6128 3235 352c  troke="rgba(255,
-000020e0: 3235 352c 3235 352c 302e 3335 2922 2073  255,255,0.35)" s
-000020f0: 7472 6f6b 652d 7769 6474 683d 2231 2220  troke-width="1" 
-00002100: 783d 2231 2220 793d 2231 2220 7769 6474  x="1" y="1" widt
-00002110: 683d 2231 3936 3822 2068 6569 6768 743d  h="1968" height=
-00002120: 2231 3231 392e 3222 2072 783d 2238 222f  "1219.2" rx="8"/
-00002130: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-00002140: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00002150: 352d 7469 746c 6522 2066 696c 6c3d 2223  5-title" fill="#
-00002160: 6335 6338 6336 2220 7465 7874 2d61 6e63  c5c8c6" text-anc
-00002170: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
-00002180: 3938 3422 2079 3d22 3237 223e 6272 6f77  984" y="27">brow
-00002190: 7372 3c2f 7465 7874 3e0a 2020 2020 2020  sr</text>.      
-000021a0: 2020 2020 2020 3c67 2074 7261 6e73 666f        <g transfo
-000021b0: 726d 3d22 7472 616e 736c 6174 6528 3236  rm="translate(26
-000021c0: 2c32 3229 223e 0a20 2020 2020 2020 2020  ,22)">.         
-000021d0: 2020 203c 6369 7263 6c65 2063 783d 2230     <circle cx="0
-000021e0: 2220 6379 3d22 3022 2072 3d22 3722 2066  " cy="0" r="7" f
-000021f0: 696c 6c3d 2223 6666 3566 3537 222f 3e0a  ill="#ff5f57"/>.
-00002200: 2020 2020 2020 2020 2020 2020 3c63 6972              <cir
-00002210: 636c 6520 6378 3d22 3232 2220 6379 3d22  cle cx="22" cy="
-00002220: 3022 2072 3d22 3722 2066 696c 6c3d 2223  0" r="7" fill="#
-00002230: 6665 6263 3265 222f 3e0a 2020 2020 2020  febc2e"/>.      
-00002240: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00002250: 3d22 3434 2220 6379 3d22 3022 2072 3d22  ="44" cy="0" r="
-00002260: 3722 2066 696c 6c3d 2223 3238 6338 3430  7" fill="#28c840
-00002270: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002280: 3c2f 673e 0a20 2020 2020 2020 200a 2020  </g>.        .  
-00002290: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-000022a0: 7472 616e 736c 6174 6528 392c 2034 3129  translate(9, 41)
-000022b0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-000022c0: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-000022d0: 3539 3436 352d 636c 6970 2d74 6572 6d69  59465-clip-termi
-000022e0: 6e61 6c29 223e 0a20 2020 203c 7265 6374  nal)">.    <rect
-000022f0: 2066 696c 6c3d 2223 3138 3138 3138 2220   fill="#181818" 
-00002300: 783d 2230 2220 793d 2231 2e35 2220 7769  x="0" y="1.5" wi
-00002310: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00002320: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00002330: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00002340: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00002350: 6c6c 3d22 2331 3831 3831 3822 2078 3d22  ll="#181818" x="
-00002360: 3132 2e32 2220 793d 2231 2e35 2220 7769  12.2" y="1.5" wi
-00002370: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00002380: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00002390: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000023a0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000023b0: 6c6c 3d22 2331 3831 3831 3822 2078 3d22  ll="#181818" x="
-000023c0: 3234 2e34 2220 793d 2231 2e35 2220 7769  24.4" y="1.5" wi
-000023d0: 6474 683d 2236 3122 2068 6569 6768 743d  dth="61" height=
-000023e0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000023f0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00002400: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00002410: 3d22 2331 3831 3831 3822 2078 3d22 3835  ="#181818" x="85
-00002420: 2e34 2220 793d 2231 2e35 2220 7769 6474  .4" y="1.5" widt
-00002430: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00002440: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00002450: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00002460: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00002470: 3d22 2331 3831 3831 3822 2078 3d22 3937  ="#181818" x="97
-00002480: 2e36 2220 793d 2231 2e35 2220 7769 6474  .6" y="1.5" widt
-00002490: 683d 2235 3132 2e34 2220 6865 6967 6874  h="512.4" height
-000024a0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000024b0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000024c0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000024d0: 6c3d 2223 3138 3138 3138 2220 783d 2236  l="#181818" x="6
-000024e0: 3130 2220 793d 2231 2e35 2220 7769 6474  10" y="1.5" widt
-000024f0: 683d 2231 3039 2e38 2220 6865 6967 6874  h="109.8" height
-00002500: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00002510: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00002520: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00002530: 6c3d 2223 3138 3138 3138 2220 783d 2237  l="#181818" x="7
-00002540: 3139 2e38 2220 793d 2231 2e35 2220 7769  19.8" y="1.5" wi
-00002550: 6474 683d 2235 3937 2e38 2220 6865 6967  dth="597.8" heig
-00002560: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00002570: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00002580: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00002590: 696c 6c3d 2223 3138 3138 3138 2220 783d  ill="#181818" x=
-000025a0: 2231 3331 372e 3622 2079 3d22 312e 3522  "1317.6" y="1.5"
-000025b0: 2077 6964 7468 3d22 3531 322e 3422 2068   width="512.4" h
-000025c0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000025d0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000025e0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000025f0: 7420 6669 6c6c 3d22 2331 3831 3831 3822  t fill="#181818"
-00002600: 2078 3d22 3138 3330 2220 793d 2231 2e35   x="1830" y="1.5
-00002610: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00002620: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00002630: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00002640: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00002650: 7420 6669 6c6c 3d22 2331 3831 3831 3822  t fill="#181818"
-00002660: 2078 3d22 3138 3432 2e32 2220 793d 2231   x="1842.2" y="1
-00002670: 2e35 2220 7769 6474 683d 2239 372e 3622  .5" width="97.6"
-00002680: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00002690: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000026a0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000026b0: 6563 7420 6669 6c6c 3d22 2331 3831 3831  ect fill="#18181
-000026c0: 3822 2078 3d22 3139 3339 2e38 2220 793d  8" x="1939.8" y=
-000026d0: 2231 2e35 2220 7769 6474 683d 2231 322e  "1.5" width="12.
-000026e0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-000026f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00002700: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00002710: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
-00002720: 3932 6622 2078 3d22 3022 2079 3d22 3235  92f" x="0" y="25
-00002730: 2e39 2220 7769 6474 683d 2233 362e 3622  .9" width="36.6"
-00002740: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00002750: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00002760: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00002770: 6563 7420 6669 6c6c 3d22 2363 6637 6530  ect fill="#cf7e0
-00002780: 3022 2078 3d22 3336 2e36 2220 793d 2232  0" x="36.6" y="2
-00002790: 352e 3922 2077 6964 7468 3d22 3336 3622  5.9" width="366"
-000027a0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000027b0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000027c0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000027d0: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
-000027e0: 6622 2078 3d22 3430 322e 3622 2079 3d22  f" x="402.6" y="
-000027f0: 3235 2e39 2220 7769 6474 683d 2234 382e  25.9" width="48.
-00002800: 3822 2068 6569 6768 743d 2232 342e 3635  8" height="24.65
-00002810: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00002820: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00002830: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00002840: 6430 6422 2078 3d22 3435 312e 3422 2079  d0d" x="451.4" y
-00002850: 3d22 3235 2e39 2220 7769 6474 683d 2231  ="25.9" width="1
-00002860: 3437 362e 3222 2068 6569 6768 743d 2232  476.2" height="2
-00002870: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00002880: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00002890: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000028a0: 2332 3335 3638 6222 2078 3d22 3139 3237  #23568b" x="1927
-000028b0: 2e36 2220 793d 2232 352e 3922 2077 6964  .6" y="25.9" wid
-000028c0: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
-000028d0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000028e0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000028f0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00002900: 6c3d 2223 3234 3239 3266 2220 783d 2230  l="#24292f" x="0
-00002910: 2220 793d 2235 302e 3322 2077 6964 7468  " y="50.3" width
-00002920: 3d22 3438 2e38 2220 6865 6967 6874 3d22  ="48.8" height="
-00002930: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00002940: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00002950: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00002960: 2223 3234 3239 3266 2220 783d 2234 382e  "#24292f" x="48.
-00002970: 3822 2079 3d22 3530 2e33 2220 7769 6474  8" y="50.3" widt
-00002980: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
-00002990: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000029a0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000029b0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000029c0: 3d22 2332 3432 3932 6622 2078 3d22 3835  ="#24292f" x="85
-000029d0: 2e34 2220 793d 2235 302e 3322 2077 6964  .4" y="50.3" wid
-000029e0: 7468 3d22 3835 2e34 2220 6865 6967 6874  th="85.4" height
-000029f0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00002a00: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00002a10: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00002a20: 6c3d 2223 3234 3239 3266 2220 783d 2231  l="#24292f" x="1
-00002a30: 3730 2e38 2220 793d 2235 302e 3322 2077  70.8" y="50.3" w
-00002a40: 6964 7468 3d22 3238 302e 3622 2068 6569  idth="280.6" hei
-00002a50: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00002a60: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00002a70: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00002a80: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00002a90: 3d22 3435 312e 3422 2079 3d22 3530 2e33  ="451.4" y="50.3
-00002aa0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00002ab0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00002ac0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00002ad0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00002ae0: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00002af0: 2078 3d22 3436 332e 3622 2079 3d22 3530   x="463.6" y="50
-00002b00: 2e33 2220 7769 6474 683d 2231 322e 3222  .3" width="12.2"
-00002b10: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00002b20: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00002b30: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00002b40: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00002b50: 6422 2078 3d22 3437 352e 3822 2079 3d22  d" x="475.8" y="
-00002b60: 3530 2e33 2220 7769 6474 683d 2236 3731  50.3" width="671
-00002b70: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00002b80: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00002b90: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00002ba0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00002bb0: 3064 2220 783d 2231 3134 362e 3822 2079  0d" x="1146.8" y
-00002bc0: 3d22 3530 2e33 2220 7769 6474 683d 2237  ="50.3" width="7
-00002bd0: 332e 3222 2068 6569 6768 743d 2232 342e  3.2" height="24.
-00002be0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00002bf0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00002c00: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00002c10: 6430 6430 6422 2078 3d22 3132 3230 2220  d0d0d" x="1220" 
-00002c20: 793d 2235 302e 3322 2077 6964 7468 3d22  y="50.3" width="
-00002c30: 3638 332e 3222 2068 6569 6768 743d 2232  683.2" height="2
-00002c40: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00002c50: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00002c60: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00002c70: 2330 6430 6430 6422 2078 3d22 3139 3033  #0d0d0d" x="1903
-00002c80: 2e32 2220 793d 2235 302e 3322 2077 6964  .2" y="50.3" wid
-00002c90: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00002ca0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00002cb0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00002cc0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00002cd0: 6c3d 2223 3064 3064 3064 2220 783d 2231  l="#0d0d0d" x="1
-00002ce0: 3931 352e 3422 2079 3d22 3530 2e33 2220  915.4" y="50.3" 
-00002cf0: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00002d00: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00002d10: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00002d20: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00002d30: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00002d40: 3d22 3139 3237 2e36 2220 793d 2235 302e  ="1927.6" y="50.
-00002d50: 3322 2077 6964 7468 3d22 3234 2e34 2220  3" width="24.4" 
-00002d60: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00002d70: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00002d80: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00002d90: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
-00002da0: 2220 783d 2230 2220 793d 2237 342e 3722  " x="0" y="74.7"
-00002db0: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
-00002dc0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00002dd0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00002de0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00002df0: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00002e00: 783d 2234 382e 3822 2079 3d22 3734 2e37  x="48.8" y="74.7
-00002e10: 2220 7769 6474 683d 2233 362e 3622 2068  " width="36.6" h
-00002e20: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00002e30: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00002e40: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00002e50: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00002e60: 2078 3d22 3835 2e34 2220 793d 2237 342e   x="85.4" y="74.
-00002e70: 3722 2077 6964 7468 3d22 3733 2e32 2220  7" width="73.2" 
-00002e80: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00002e90: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00002ea0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00002eb0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
-00002ec0: 2220 783d 2231 3538 2e36 2220 793d 2237  " x="158.6" y="7
-00002ed0: 342e 3722 2077 6964 7468 3d22 3239 322e  4.7" width="292.
-00002ee0: 3822 2068 6569 6768 743d 2232 342e 3635  8" height="24.65
-00002ef0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00002f00: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00002f10: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00002f20: 6430 6422 2078 3d22 3435 312e 3422 2079  d0d" x="451.4" y
-00002f30: 3d22 3734 2e37 2220 7769 6474 683d 2231  ="74.7" width="1
-00002f40: 3437 362e 3222 2068 6569 6768 743d 2232  476.2" height="2
-00002f50: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00002f60: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00002f70: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00002f80: 2332 3335 3638 6222 2078 3d22 3139 3237  #23568b" x="1927
-00002f90: 2e36 2220 793d 2237 342e 3722 2077 6964  .6" y="74.7" wid
-00002fa0: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
-00002fb0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00002fc0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00002fd0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00002fe0: 6c3d 2223 3234 3239 3266 2220 783d 2230  l="#24292f" x="0
-00002ff0: 2220 793d 2239 392e 3122 2077 6964 7468  " y="99.1" width
-00003000: 3d22 3438 2e38 2220 6865 6967 6874 3d22  ="48.8" height="
-00003010: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00003020: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00003030: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00003040: 2223 3234 3239 3266 2220 783d 2234 382e  "#24292f" x="48.
-00003050: 3822 2079 3d22 3939 2e31 2220 7769 6474  8" y="99.1" widt
-00003060: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
-00003070: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00003080: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00003090: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000030a0: 3d22 2332 3432 3932 6622 2078 3d22 3835  ="#24292f" x="85
-000030b0: 2e34 2220 793d 2239 392e 3122 2077 6964  .4" y="99.1" wid
-000030c0: 7468 3d22 3438 2e38 2220 6865 6967 6874  th="48.8" height
-000030d0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000030e0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000030f0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00003100: 6c3d 2223 3234 3239 3266 2220 783d 2231  l="#24292f" x="1
-00003110: 3334 2e32 2220 793d 2239 392e 3122 2077  34.2" y="99.1" w
-00003120: 6964 7468 3d22 3331 372e 3222 2068 6569  idth="317.2" hei
-00003130: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00003140: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00003150: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00003160: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00003170: 3d22 3435 312e 3422 2079 3d22 3939 2e31  ="451.4" y="99.1
-00003180: 2220 7769 6474 683d 2231 3437 362e 3222  " width="1476.2"
-00003190: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000031a0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000031b0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000031c0: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-000031d0: 6222 2078 3d22 3139 3237 2e36 2220 793d  b" x="1927.6" y=
-000031e0: 2239 392e 3122 2077 6964 7468 3d22 3234  "99.1" width="24
-000031f0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00003200: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00003210: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00003220: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-00003230: 3239 3266 2220 783d 2230 2220 793d 2231  292f" x="0" y="1
-00003240: 3233 2e35 2220 7769 6474 683d 2234 382e  23.5" width="48.
-00003250: 3822 2068 6569 6768 743d 2232 342e 3635  8" height="24.65
-00003260: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00003270: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00003280: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
-00003290: 3932 6622 2078 3d22 3438 2e38 2220 793d  92f" x="48.8" y=
-000032a0: 2231 3233 2e35 2220 7769 6474 683d 2233  "123.5" width="3
-000032b0: 362e 3622 2068 6569 6768 743d 2232 342e  6.6" height="24.
-000032c0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000032d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000032e0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-000032f0: 3432 3932 6622 2078 3d22 3835 2e34 2220  4292f" x="85.4" 
-00003300: 793d 2231 3233 2e35 2220 7769 6474 683d  y="123.5" width=
-00003310: 2231 3436 2e34 2220 6865 6967 6874 3d22  "146.4" height="
-00003320: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00003330: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00003340: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00003350: 2223 3234 3239 3266 2220 783d 2232 3331  "#24292f" x="231
-00003360: 2e38 2220 793d 2231 3233 2e35 2220 7769  .8" y="123.5" wi
-00003370: 6474 683d 2232 3139 2e36 2220 6865 6967  dth="219.6" heig
-00003380: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00003390: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-000033a0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-000033b0: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
-000033c0: 2234 3531 2e34 2220 793d 2231 3233 2e35  "451.4" y="123.5
-000033d0: 2220 7769 6474 683d 2231 3437 362e 3222  " width="1476.2"
-000033e0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000033f0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00003400: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00003410: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-00003420: 6222 2078 3d22 3139 3237 2e36 2220 793d  b" x="1927.6" y=
-00003430: 2231 3233 2e35 2220 7769 6474 683d 2232  "123.5" width="2
-00003440: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
-00003450: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00003460: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00003470: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00003480: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
-00003490: 3134 372e 3922 2077 6964 7468 3d22 3438  147.9" width="48
-000034a0: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
-000034b0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000034c0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000034d0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-000034e0: 3239 3266 2220 783d 2234 382e 3822 2079  292f" x="48.8" y
-000034f0: 3d22 3134 372e 3922 2077 6964 7468 3d22  ="147.9" width="
-00003500: 3336 2e36 2220 6865 6967 6874 3d22 3234  36.6" height="24
-00003510: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00003520: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00003530: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00003540: 3234 3239 3266 2220 783d 2238 352e 3422  24292f" x="85.4"
-00003550: 2079 3d22 3134 372e 3922 2077 6964 7468   y="147.9" width
-00003560: 3d22 3631 2220 6865 6967 6874 3d22 3234  ="61" height="24
-00003570: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00003580: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00003590: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-000035a0: 3234 3239 3266 2220 783d 2231 3436 2e34  24292f" x="146.4
-000035b0: 2220 793d 2231 3437 2e39 2220 7769 6474  " y="147.9" widt
-000035c0: 683d 2233 3035 2220 6865 6967 6874 3d22  h="305" height="
-000035d0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000035e0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000035f0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00003600: 2223 3064 3064 3064 2220 783d 2234 3531  "#0d0d0d" x="451
-00003610: 2e34 2220 793d 2231 3437 2e39 2220 7769  .4" y="147.9" wi
-00003620: 6474 683d 2233 362e 3622 2068 6569 6768  dth="36.6" heigh
-00003630: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00003640: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00003650: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00003660: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-00003670: 3438 3822 2079 3d22 3134 372e 3922 2077  488" y="147.9" w
-00003680: 6964 7468 3d22 3137 302e 3822 2068 6569  idth="170.8" hei
-00003690: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000036a0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000036b0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000036c0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-000036d0: 3d22 3635 382e 3822 2079 3d22 3134 372e  ="658.8" y="147.
-000036e0: 3922 2077 6964 7468 3d22 3132 2e32 2220  9" width="12.2" 
-000036f0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00003700: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00003710: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00003720: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
-00003730: 2220 783d 2236 3731 2220 793d 2231 3437  " x="671" y="147
-00003740: 2e39 2220 7769 6474 683d 2233 362e 3622  .9" width="36.6"
-00003750: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00003760: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00003770: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00003780: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00003790: 6422 2078 3d22 3730 372e 3622 2079 3d22  d" x="707.6" y="
-000037a0: 3134 372e 3922 2077 6964 7468 3d22 3438  147.9" width="48
-000037b0: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
-000037c0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000037d0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000037e0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-000037f0: 3064 3064 2220 783d 2237 3536 2e34 2220  0d0d" x="756.4" 
-00003800: 793d 2231 3437 2e39 2220 7769 6474 683d  y="147.9" width=
-00003810: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00003820: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00003830: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00003840: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00003850: 2330 6430 6430 6422 2078 3d22 3736 382e  #0d0d0d" x="768.
-00003860: 3622 2079 3d22 3134 372e 3922 2077 6964  6" y="147.9" wid
-00003870: 7468 3d22 3336 2e36 2220 6865 6967 6874  th="36.6" height
-00003880: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00003890: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000038a0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000038b0: 6c3d 2223 3064 3064 3064 2220 783d 2238  l="#0d0d0d" x="8
-000038c0: 3035 2e32 2220 793d 2231 3437 2e39 2220  05.2" y="147.9" 
-000038d0: 7769 6474 683d 2231 3730 2e38 2220 6865  width="170.8" he
-000038e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-000038f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00003900: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00003910: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
-00003920: 783d 2239 3736 2220 793d 2231 3437 2e39  x="976" y="147.9
-00003930: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00003940: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003950: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00003960: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00003970: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00003980: 2078 3d22 3938 382e 3222 2079 3d22 3134   x="988.2" y="14
-00003990: 372e 3922 2077 6964 7468 3d22 3336 2e36  7.9" width="36.6
-000039a0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000039b0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000039c0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000039d0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-000039e0: 3064 2220 783d 2231 3032 342e 3822 2079  0d" x="1024.8" y
-000039f0: 3d22 3134 372e 3922 2077 6964 7468 3d22  ="147.9" width="
-00003a00: 3137 302e 3822 2068 6569 6768 743d 2232  170.8" height="2
-00003a10: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00003a20: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00003a30: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00003a40: 2330 6430 6430 6422 2078 3d22 3131 3935  #0d0d0d" x="1195
-00003a50: 2e36 2220 793d 2231 3437 2e39 2220 7769  .6" y="147.9" wi
-00003a60: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00003a70: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00003a80: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00003a90: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00003aa0: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-00003ab0: 3132 3037 2e38 2220 793d 2231 3437 2e39  1207.8" y="147.9
-00003ac0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00003ad0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003ae0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00003af0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00003b00: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00003b10: 2078 3d22 3132 3230 2220 793d 2231 3437   x="1220" y="147
-00003b20: 2e39 2220 7769 6474 683d 2231 322e 3222  .9" width="12.2"
-00003b30: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00003b40: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00003b50: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00003b60: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00003b70: 6422 2078 3d22 3132 3332 2e32 2220 793d  d" x="1232.2" y=
-00003b80: 2231 3437 2e39 2220 7769 6474 683d 2231  "147.9" width="1
-00003b90: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00003ba0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00003bb0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00003bc0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00003bd0: 6430 6430 6422 2078 3d22 3132 3434 2e34  d0d0d" x="1244.4
-00003be0: 2220 793d 2231 3437 2e39 2220 7769 6474  " y="147.9" widt
-00003bf0: 683d 2236 3833 2e32 2220 6865 6967 6874  h="683.2" height
-00003c00: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00003c10: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00003c20: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00003c30: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
-00003c40: 3932 372e 3622 2079 3d22 3134 372e 3922  927.6" y="147.9"
-00003c50: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-00003c60: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00003c70: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00003c80: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00003c90: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00003ca0: 783d 2230 2220 793d 2231 3732 2e33 2220  x="0" y="172.3" 
-00003cb0: 7769 6474 683d 2234 382e 3822 2068 6569  width="48.8" hei
-00003cc0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00003cd0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00003ce0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00003cf0: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-00003d00: 3d22 3438 2e38 2220 793d 2231 3732 2e33  ="48.8" y="172.3
-00003d10: 2220 7769 6474 683d 2233 362e 3622 2068  " width="36.6" h
-00003d20: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003d30: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00003d40: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00003d50: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00003d60: 2078 3d22 3835 2e34 2220 793d 2231 3732   x="85.4" y="172
-00003d70: 2e33 2220 7769 6474 683d 2231 3232 2220  .3" width="122" 
-00003d80: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00003d90: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00003da0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00003db0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
-00003dc0: 2220 783d 2232 3037 2e34 2220 793d 2231  " x="207.4" y="1
-00003dd0: 3732 2e33 2220 7769 6474 683d 2232 3434  72.3" width="244
-00003de0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00003df0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00003e00: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00003e10: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00003e20: 3064 2220 783d 2234 3531 2e34 2220 793d  0d" x="451.4" y=
-00003e30: 2231 3732 2e33 2220 7769 6474 683d 2231  "172.3" width="1
-00003e40: 3437 362e 3222 2068 6569 6768 743d 2232  476.2" height="2
-00003e50: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00003e60: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00003e70: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00003e80: 2332 3335 3638 6222 2078 3d22 3139 3237  #23568b" x="1927
-00003e90: 2e36 2220 793d 2231 3732 2e33 2220 7769  .6" y="172.3" wi
-00003ea0: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
-00003eb0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00003ec0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00003ed0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00003ee0: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
-00003ef0: 3022 2079 3d22 3139 362e 3722 2077 6964  0" y="196.7" wid
-00003f00: 7468 3d22 3438 2e38 2220 6865 6967 6874  th="48.8" height
-00003f10: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00003f20: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00003f30: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00003f40: 6c3d 2223 3234 3239 3266 2220 783d 2234  l="#24292f" x="4
-00003f50: 382e 3822 2079 3d22 3139 362e 3722 2077  8.8" y="196.7" w
-00003f60: 6964 7468 3d22 3336 2e36 2220 6865 6967  idth="36.6" heig
-00003f70: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00003f80: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00003f90: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00003fa0: 696c 6c3d 2223 3234 3239 3266 2220 783d  ill="#24292f" x=
-00003fb0: 2238 352e 3422 2079 3d22 3139 362e 3722  "85.4" y="196.7"
-00003fc0: 2077 6964 7468 3d22 3238 302e 3622 2068   width="280.6" h
-00003fd0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003fe0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00003ff0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00004000: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00004010: 2078 3d22 3336 3622 2079 3d22 3139 362e   x="366" y="196.
-00004020: 3722 2077 6964 7468 3d22 3835 2e34 2220  7" width="85.4" 
-00004030: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00004040: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00004050: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00004060: 6374 2066 696c 6c3d 2223 3462 3465 3535  ct fill="#4b4e55
-00004070: 2220 783d 2234 3531 2e34 2220 793d 2231  " x="451.4" y="1
-00004080: 3936 2e37 2220 7769 6474 683d 2237 332e  96.7" width="73.
-00004090: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-000040a0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000040b0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000040c0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-000040d0: 6430 6422 2078 3d22 3532 342e 3622 2079  d0d" x="524.6" y
-000040e0: 3d22 3139 362e 3722 2077 6964 7468 3d22  ="196.7" width="
-000040f0: 3834 312e 3822 2068 6569 6768 743d 2232  841.8" height="2
-00004100: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00004110: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00004120: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00004130: 2330 6430 6430 6422 2078 3d22 3133 3636  #0d0d0d" x="1366
-00004140: 2e34 2220 793d 2231 3936 2e37 2220 7769  .4" y="196.7" wi
-00004150: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00004160: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00004170: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00004180: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00004190: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-000041a0: 3133 3738 2e36 2220 793d 2231 3936 2e37  1378.6" y="196.7
-000041b0: 2220 7769 6474 683d 2235 3234 2e36 2220  " width="524.6" 
-000041c0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-000041d0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-000041e0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-000041f0: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
-00004200: 2220 783d 2231 3930 332e 3222 2079 3d22  " x="1903.2" y="
-00004210: 3139 362e 3722 2077 6964 7468 3d22 3234  196.7" width="24
-00004220: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00004230: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00004240: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00004250: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
-00004260: 3536 3862 2220 783d 2231 3932 372e 3622  568b" x="1927.6"
-00004270: 2079 3d22 3139 362e 3722 2077 6964 7468   y="196.7" width
-00004280: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
-00004290: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000042a0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000042b0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-000042c0: 2223 3234 3239 3266 2220 783d 2230 2220  "#24292f" x="0" 
-000042d0: 793d 2232 3231 2e31 2220 7769 6474 683d  y="221.1" width=
-000042e0: 2234 382e 3822 2068 6569 6768 743d 2232  "48.8" height="2
-000042f0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00004300: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00004310: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00004320: 2332 3432 3932 6622 2078 3d22 3438 2e38  #24292f" x="48.8
-00004330: 2220 793d 2232 3231 2e31 2220 7769 6474  " y="221.1" widt
-00004340: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
-00004350: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004360: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004370: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004380: 3d22 2332 3432 3932 6622 2078 3d22 3835  ="#24292f" x="85
-00004390: 2e34 2220 793d 2232 3231 2e31 2220 7769  .4" y="221.1" wi
-000043a0: 6474 683d 2231 3538 2e36 2220 6865 6967  dth="158.6" heig
-000043b0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-000043c0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-000043d0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-000043e0: 696c 6c3d 2223 3234 3239 3266 2220 783d  ill="#24292f" x=
-000043f0: 2232 3434 2220 793d 2232 3231 2e31 2220  "244" y="221.1" 
-00004400: 7769 6474 683d 2232 3037 2e34 2220 6865  width="207.4" he
-00004410: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00004420: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00004430: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00004440: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
-00004450: 783d 2234 3531 2e34 2220 793d 2232 3231  x="451.4" y="221
-00004460: 2e31 2220 7769 6474 683d 2234 3633 2e36  .1" width="463.6
-00004470: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00004480: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00004490: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000044a0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-000044b0: 3064 2220 783d 2239 3135 2220 793d 2232  0d" x="915" y="2
-000044c0: 3231 2e31 2220 7769 6474 683d 2231 322e  21.1" width="12.
-000044d0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-000044e0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000044f0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00004500: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00004510: 6430 6422 2078 3d22 3932 372e 3222 2079  d0d" x="927.2" y
-00004520: 3d22 3232 312e 3122 2077 6964 7468 3d22  ="221.1" width="
-00004530: 3437 352e 3822 2068 6569 6768 743d 2232  475.8" height="2
-00004540: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00004550: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00004560: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00004570: 2330 6430 6430 6422 2078 3d22 3134 3033  #0d0d0d" x="1403
-00004580: 2220 793d 2232 3231 2e31 2220 7769 6474  " y="221.1" widt
-00004590: 683d 2235 3234 2e36 2220 6865 6967 6874  h="524.6" height
-000045a0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000045b0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000045c0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000045d0: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
-000045e0: 3932 372e 3622 2079 3d22 3232 312e 3122  927.6" y="221.1"
-000045f0: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-00004600: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00004610: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00004620: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00004630: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00004640: 783d 2230 2220 793d 2232 3435 2e35 2220  x="0" y="245.5" 
-00004650: 7769 6474 683d 2234 382e 3822 2068 6569  width="48.8" hei
-00004660: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00004670: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00004680: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00004690: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-000046a0: 3d22 3438 2e38 2220 793d 2232 3435 2e35  ="48.8" y="245.5
-000046b0: 2220 7769 6474 683d 2233 362e 3622 2068  " width="36.6" h
-000046c0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000046d0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000046e0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000046f0: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00004700: 2078 3d22 3835 2e34 2220 793d 2232 3435   x="85.4" y="245
-00004710: 2e35 2220 7769 6474 683d 2238 352e 3422  .5" width="85.4"
-00004720: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00004730: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00004740: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00004750: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
-00004760: 6622 2078 3d22 3137 302e 3822 2079 3d22  f" x="170.8" y="
-00004770: 3234 352e 3522 2077 6964 7468 3d22 3238  245.5" width="28
-00004780: 302e 3622 2068 6569 6768 743d 2232 342e  0.6" height="24.
-00004790: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000047a0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000047b0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-000047c0: 6430 6430 6422 2078 3d22 3435 312e 3422  d0d0d" x="451.4"
-000047d0: 2079 3d22 3234 352e 3522 2077 6964 7468   y="245.5" width
-000047e0: 3d22 3134 3736 2e32 2220 6865 6967 6874  ="1476.2" height
-000047f0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00004800: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00004810: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00004820: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
-00004830: 3932 372e 3622 2079 3d22 3234 352e 3522  927.6" y="245.5"
-00004840: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-00004850: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00004860: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00004870: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00004880: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00004890: 783d 2230 2220 793d 2232 3639 2e39 2220  x="0" y="269.9" 
-000048a0: 7769 6474 683d 2234 382e 3822 2068 6569  width="48.8" hei
-000048b0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000048c0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000048d0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000048e0: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-000048f0: 3d22 3438 2e38 2220 793d 2232 3639 2e39  ="48.8" y="269.9
-00004900: 2220 7769 6474 683d 2233 362e 3622 2068  " width="36.6" h
-00004910: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00004920: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00004930: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00004940: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00004950: 2078 3d22 3835 2e34 2220 793d 2232 3639   x="85.4" y="269
-00004960: 2e39 2220 7769 6474 683d 2237 332e 3222  .9" width="73.2"
-00004970: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00004980: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00004990: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000049a0: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
-000049b0: 6622 2078 3d22 3135 382e 3622 2079 3d22  f" x="158.6" y="
-000049c0: 3236 392e 3922 2077 6964 7468 3d22 3631  269.9" width="61
-000049d0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000049e0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000049f0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00004a00: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
-00004a10: 3266 2220 783d 2232 3139 2e36 2220 793d  2f" x="219.6" y=
-00004a20: 2232 3639 2e39 2220 7769 6474 683d 2232  "269.9" width="2
-00004a30: 3331 2e38 2220 6865 6967 6874 3d22 3234  31.8" height="24
-00004a40: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00004a50: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00004a60: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00004a70: 3064 3064 3064 2220 783d 2234 3531 2e34  0d0d0d" x="451.4
-00004a80: 2220 793d 2232 3639 2e39 2220 7769 6474  " y="269.9" widt
-00004a90: 683d 2231 3437 362e 3222 2068 6569 6768  h="1476.2" heigh
-00004aa0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00004ab0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00004ac0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00004ad0: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-00004ae0: 3139 3237 2e36 2220 793d 2232 3639 2e39  1927.6" y="269.9
-00004af0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
-00004b00: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00004b10: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00004b20: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00004b30: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00004b40: 2078 3d22 3022 2079 3d22 3239 342e 3322   x="0" y="294.3"
-00004b50: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
-00004b60: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00004b70: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00004b80: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00004b90: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00004ba0: 783d 2234 382e 3822 2079 3d22 3239 342e  x="48.8" y="294.
-00004bb0: 3322 2077 6964 7468 3d22 3336 2e36 2220  3" width="36.6" 
-00004bc0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00004bd0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00004be0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00004bf0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
-00004c00: 2220 783d 2238 352e 3422 2079 3d22 3239  " x="85.4" y="29
-00004c10: 342e 3322 2077 6964 7468 3d22 3130 392e  4.3" width="109.
-00004c20: 3822 2068 6569 6768 743d 2232 342e 3635  8" height="24.65
-00004c30: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00004c40: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00004c50: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
-00004c60: 3932 6622 2078 3d22 3139 352e 3222 2079  92f" x="195.2" y
-00004c70: 3d22 3239 342e 3322 2077 6964 7468 3d22  ="294.3" width="
-00004c80: 3631 2220 6865 6967 6874 3d22 3234 2e36  61" height="24.6
-00004c90: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00004ca0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00004cb0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-00004cc0: 3239 3266 2220 783d 2232 3536 2e32 2220  292f" x="256.2" 
-00004cd0: 793d 2232 3934 2e33 2220 7769 6474 683d  y="294.3" width=
-00004ce0: 2231 3935 2e32 2220 6865 6967 6874 3d22  "195.2" height="
-00004cf0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00004d00: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00004d10: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00004d20: 2223 3064 3064 3064 2220 783d 2234 3531  "#0d0d0d" x="451
-00004d30: 2e34 2220 793d 2232 3934 2e33 2220 7769  .4" y="294.3" wi
-00004d40: 6474 683d 2231 3437 362e 3222 2068 6569  dth="1476.2" hei
-00004d50: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00004d60: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00004d70: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00004d80: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00004d90: 3d22 3139 3237 2e36 2220 793d 2232 3934  ="1927.6" y="294
-00004da0: 2e33 2220 7769 6474 683d 2232 342e 3422  .3" width="24.4"
-00004db0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00004dc0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00004dd0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00004de0: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
-00004df0: 6622 2078 3d22 3022 2079 3d22 3331 382e  f" x="0" y="318.
-00004e00: 3722 2077 6964 7468 3d22 3438 2e38 2220  7" width="48.8" 
-00004e10: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00004e20: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00004e30: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00004e40: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
-00004e50: 2220 783d 2234 382e 3822 2079 3d22 3331  " x="48.8" y="31
-00004e60: 382e 3722 2077 6964 7468 3d22 3336 2e36  8.7" width="36.6
-00004e70: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00004e80: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00004e90: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00004ea0: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
-00004eb0: 3266 2220 783d 2238 352e 3422 2079 3d22  2f" x="85.4" y="
-00004ec0: 3331 382e 3722 2077 6964 7468 3d22 3733  318.7" width="73
-00004ed0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-00004ee0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00004ef0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00004f00: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-00004f10: 3239 3266 2220 783d 2231 3538 2e36 2220  292f" x="158.6" 
-00004f20: 793d 2233 3138 2e37 2220 7769 6474 683d  y="318.7" width=
-00004f30: 2233 362e 3622 2068 6569 6768 743d 2232  "36.6" height="2
-00004f40: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00004f50: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00004f60: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00004f70: 2332 3432 3932 6622 2078 3d22 3139 352e  #24292f" x="195.
-00004f80: 3222 2079 3d22 3331 382e 3722 2077 6964  2" y="318.7" wid
-00004f90: 7468 3d22 3235 362e 3222 2068 6569 6768  th="256.2" heigh
-00004fa0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00004fb0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00004fc0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00004fd0: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-00004fe0: 3435 312e 3422 2079 3d22 3331 382e 3722  451.4" y="318.7"
-00004ff0: 2077 6964 7468 3d22 3134 3736 2e32 2220   width="1476.2" 
-00005000: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00005010: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00005020: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00005030: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
-00005040: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00005050: 3331 382e 3722 2077 6964 7468 3d22 3234  318.7" width="24
-00005060: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00005070: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00005080: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00005090: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-000050a0: 3239 3266 2220 783d 2230 2220 793d 2233  292f" x="0" y="3
-000050b0: 3433 2e31 2220 7769 6474 683d 2234 3531  43.1" width="451
-000050c0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-000050d0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000050e0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000050f0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00005100: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
-00005110: 793d 2233 3433 2e31 2220 7769 6474 683d  y="343.1" width=
-00005120: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
-00005130: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005140: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005150: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005160: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
-00005170: 3237 2e36 2220 793d 2233 3433 2e31 2220  27.6" y="343.1" 
-00005180: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-00005190: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000051a0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000051b0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000051c0: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-000051d0: 3d22 3022 2079 3d22 3336 372e 3522 2077  ="0" y="367.5" w
-000051e0: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
-000051f0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005200: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005210: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005220: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00005230: 3d22 3435 312e 3422 2079 3d22 3336 372e  ="451.4" y="367.
-00005240: 3522 2077 6964 7468 3d22 3635 382e 3822  5" width="658.8"
-00005250: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00005260: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00005270: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00005280: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00005290: 6422 2078 3d22 3131 3130 2e32 2220 793d  d" x="1110.2" y=
-000052a0: 2233 3637 2e35 2220 7769 6474 683d 2231  "367.5" width="1
-000052b0: 3436 2e34 2220 6865 6967 6874 3d22 3234  46.4" height="24
-000052c0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-000052d0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-000052e0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-000052f0: 3064 3064 3064 2220 783d 2231 3235 362e  0d0d0d" x="1256.
-00005300: 3622 2079 3d22 3336 372e 3522 2077 6964  6" y="367.5" wid
-00005310: 7468 3d22 3637 3122 2068 6569 6768 743d  th="671" height=
-00005320: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005330: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005340: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005350: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
-00005360: 3237 2e36 2220 793d 2233 3637 2e35 2220  27.6" y="367.5" 
-00005370: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-00005380: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005390: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000053a0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000053b0: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-000053c0: 3d22 3022 2079 3d22 3339 312e 3922 2077  ="0" y="391.9" w
-000053d0: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
-000053e0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000053f0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005400: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005410: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00005420: 3d22 3435 312e 3422 2079 3d22 3339 312e  ="451.4" y="391.
-00005430: 3922 2077 6964 7468 3d22 3134 3736 2e32  9" width="1476.2
-00005440: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00005450: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00005460: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00005470: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
-00005480: 3862 2220 783d 2231 3932 372e 3622 2079  8b" x="1927.6" y
-00005490: 3d22 3339 312e 3922 2077 6964 7468 3d22  ="391.9" width="
-000054a0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-000054b0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-000054c0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-000054d0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-000054e0: 3234 3239 3266 2220 783d 2230 2220 793d  24292f" x="0" y=
-000054f0: 2234 3136 2e33 2220 7769 6474 683d 2234  "416.3" width="4
-00005500: 3531 2e34 2220 6865 6967 6874 3d22 3234  51.4" height="24
-00005510: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00005520: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00005530: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00005540: 3064 3064 3064 2220 783d 2234 3531 2e34  0d0d0d" x="451.4
-00005550: 2220 793d 2234 3136 2e33 2220 7769 6474  " y="416.3" widt
-00005560: 683d 2233 3533 2e38 2220 6865 6967 6874  h="353.8" height
-00005570: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00005580: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00005590: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000055a0: 6c3d 2223 3064 3064 3064 2220 783d 2238  l="#0d0d0d" x="8
-000055b0: 3035 2e32 2220 793d 2234 3136 2e33 2220  05.2" y="416.3" 
-000055c0: 7769 6474 683d 2234 382e 3822 2068 6569  width="48.8" hei
-000055d0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000055e0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000055f0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005600: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00005610: 3d22 3835 3422 2079 3d22 3431 362e 3322  ="854" y="416.3"
-00005620: 2077 6964 7468 3d22 3230 372e 3422 2068   width="207.4" h
-00005630: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00005640: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00005650: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00005660: 7420 6669 6c6c 3d22 2334 6234 6535 3522  t fill="#4b4e55"
-00005670: 2078 3d22 3130 3631 2e34 2220 793d 2234   x="1061.4" y="4
-00005680: 3136 2e33 2220 7769 6474 683d 2234 382e  16.3" width="48.
-00005690: 3822 2068 6569 6768 743d 2232 342e 3635  8" height="24.65
-000056a0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000056b0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000056c0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-000056d0: 6430 6422 2078 3d22 3131 3130 2e32 2220  d0d" x="1110.2" 
-000056e0: 793d 2234 3136 2e33 2220 7769 6474 683d  y="416.3" width=
-000056f0: 2232 3932 2e38 2220 6865 6967 6874 3d22  "292.8" height="
-00005700: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00005710: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00005720: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00005730: 2223 3064 3064 3064 2220 783d 2231 3430  "#0d0d0d" x="140
-00005740: 3322 2079 3d22 3431 362e 3322 2077 6964  3" y="416.3" wid
-00005750: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00005760: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00005770: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00005780: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00005790: 6c3d 2223 3064 3064 3064 2220 783d 2231  l="#0d0d0d" x="1
-000057a0: 3431 352e 3222 2079 3d22 3431 362e 3322  415.2" y="416.3"
-000057b0: 2077 6964 7468 3d22 3531 322e 3422 2068   width="512.4" h
-000057c0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000057d0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000057e0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000057f0: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-00005800: 2078 3d22 3139 3237 2e36 2220 793d 2234   x="1927.6" y="4
-00005810: 3136 2e33 2220 7769 6474 683d 2232 342e  16.3" width="24.
-00005820: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00005830: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00005840: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00005850: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
-00005860: 3932 6622 2078 3d22 3022 2079 3d22 3434  92f" x="0" y="44
-00005870: 302e 3722 2077 6964 7468 3d22 3435 312e  0.7" width="451.
-00005880: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00005890: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000058a0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000058b0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-000058c0: 6430 6422 2078 3d22 3435 312e 3422 2079  d0d" x="451.4" y
-000058d0: 3d22 3434 302e 3722 2077 6964 7468 3d22  ="440.7" width="
-000058e0: 3432 3722 2068 6569 6768 743d 2232 342e  427" height="24.
-000058f0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00005900: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00005910: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2334  /><rect fill="#4
-00005920: 6234 6535 3522 2078 3d22 3837 382e 3422  b4e55" x="878.4"
-00005930: 2079 3d22 3434 302e 3722 2077 6964 7468   y="440.7" width
-00005940: 3d22 3336 2e36 2220 6865 6967 6874 3d22  ="36.6" height="
-00005950: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00005960: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00005970: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00005980: 2223 3064 3064 3064 2220 783d 2239 3135  "#0d0d0d" x="915
-00005990: 2220 793d 2234 3430 2e37 2220 7769 6474  " y="440.7" widt
-000059a0: 683d 2232 3830 2e36 2220 6865 6967 6874  h="280.6" height
-000059b0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000059c0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000059d0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000059e0: 6c3d 2223 3462 3465 3535 2220 783d 2231  l="#4b4e55" x="1
-000059f0: 3139 352e 3622 2079 3d22 3434 302e 3722  195.6" y="440.7"
-00005a00: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
-00005a10: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00005a20: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00005a30: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00005a40: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
-00005a50: 783d 2231 3234 342e 3422 2079 3d22 3434  x="1244.4" y="44
-00005a60: 302e 3722 2077 6964 7468 3d22 3132 2e32  0.7" width="12.2
-00005a70: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00005a80: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00005a90: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00005aa0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00005ab0: 3064 2220 783d 2231 3235 362e 3622 2079  0d" x="1256.6" y
-00005ac0: 3d22 3434 302e 3722 2077 6964 7468 3d22  ="440.7" width="
-00005ad0: 3631 2220 6865 6967 6874 3d22 3234 2e36  61" height="24.6
-00005ae0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00005af0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00005b00: 3e3c 7265 6374 2066 696c 6c3d 2223 3462  ><rect fill="#4b
-00005b10: 3465 3535 2220 783d 2231 3331 372e 3622  4e55" x="1317.6"
-00005b20: 2079 3d22 3434 302e 3722 2077 6964 7468   y="440.7" width
-00005b30: 3d22 3336 2e36 2220 6865 6967 6874 3d22  ="36.6" height="
-00005b40: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00005b50: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00005b60: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00005b70: 2223 3064 3064 3064 2220 783d 2231 3335  "#0d0d0d" x="135
-00005b80: 342e 3222 2079 3d22 3434 302e 3722 2077  4.2" y="440.7" w
-00005b90: 6964 7468 3d22 3236 382e 3422 2068 6569  idth="268.4" hei
-00005ba0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005bb0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005bc0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005bd0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00005be0: 3d22 3136 3232 2e36 2220 793d 2234 3430  ="1622.6" y="440
-00005bf0: 2e37 2220 7769 6474 683d 2233 3035 2220  .7" width="305" 
-00005c00: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00005c10: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00005c20: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00005c30: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
-00005c40: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00005c50: 3434 302e 3722 2077 6964 7468 3d22 3234  440.7" width="24
-00005c60: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00005c70: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00005c80: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00005c90: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-00005ca0: 3239 3266 2220 783d 2230 2220 793d 2234  292f" x="0" y="4
-00005cb0: 3635 2e31 2220 7769 6474 683d 2234 3531  65.1" width="451
-00005cc0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00005cd0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00005ce0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00005cf0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00005d00: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
-00005d10: 793d 2234 3635 2e31 2220 7769 6474 683d  y="465.1" width=
-00005d20: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
-00005d30: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005d40: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005d50: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005d60: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
-00005d70: 3237 2e36 2220 793d 2234 3635 2e31 2220  27.6" y="465.1" 
-00005d80: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-00005d90: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005da0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005db0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005dc0: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-00005dd0: 3d22 3022 2079 3d22 3438 392e 3522 2077  ="0" y="489.5" w
-00005de0: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
-00005df0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005e00: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005e10: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005e20: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
-00005e30: 3d22 3435 312e 3422 2079 3d22 3438 392e  ="451.4" y="489.
-00005e40: 3522 2077 6964 7468 3d22 3134 3736 2e32  5" width="1476.2
-00005e50: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00005e60: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00005e70: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00005e80: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
-00005e90: 3862 2220 783d 2231 3932 372e 3622 2079  8b" x="1927.6" y
-00005ea0: 3d22 3438 392e 3522 2077 6964 7468 3d22  ="489.5" width="
-00005eb0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-00005ec0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00005ed0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00005ee0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00005ef0: 3234 3239 3266 2220 783d 2230 2220 793d  24292f" x="0" y=
-00005f00: 2235 3133 2e39 2220 7769 6474 683d 2234  "513.9" width="4
-00005f10: 3531 2e34 2220 6865 6967 6874 3d22 3234  51.4" height="24
-00005f20: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00005f30: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00005f40: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00005f50: 3237 3238 3232 2220 783d 2234 3531 2e34  272822" x="451.4
-00005f60: 2220 793d 2235 3133 2e39 2220 7769 6474  " y="513.9" widt
-00005f70: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00005f80: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005f90: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005fa0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005fb0: 3d22 2332 3732 3832 3222 2078 3d22 3436  ="#272822" x="46
-00005fc0: 332e 3622 2079 3d22 3531 332e 3922 2077  3.6" y="513.9" w
-00005fd0: 6964 7468 3d22 3438 2e38 2220 6865 6967  idth="48.8" heig
-00005fe0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00005ff0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00006000: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00006010: 696c 6c3d 2223 3237 3238 3232 2220 783d  ill="#272822" x=
-00006020: 2235 3132 2e34 2220 793d 2235 3133 2e39  "512.4" y="513.9
-00006030: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00006040: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006050: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00006060: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00006070: 7420 6669 6c6c 3d22 2332 3732 3832 3222  t fill="#272822"
-00006080: 2078 3d22 3532 342e 3622 2079 3d22 3531   x="524.6" y="51
-00006090: 332e 3922 2077 6964 7468 3d22 3835 2e34  3.9" width="85.4
-000060a0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000060b0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000060c0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000060d0: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
-000060e0: 3232 2220 783d 2236 3130 2220 793d 2235  22" x="610" y="5
-000060f0: 3133 2e39 2220 7769 6474 683d 2231 322e  13.9" width="12.
-00006100: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00006110: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006120: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006130: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
-00006140: 3832 3222 2078 3d22 3632 322e 3222 2079  822" x="622.2" y
-00006150: 3d22 3531 332e 3922 2077 6964 7468 3d22  ="513.9" width="
-00006160: 3733 2e32 2220 6865 6967 6874 3d22 3234  73.2" height="24
-00006170: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00006180: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00006190: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-000061a0: 3237 3238 3232 2220 783d 2236 3935 2e34  272822" x="695.4
-000061b0: 2220 793d 2235 3133 2e39 2220 7769 6474  " y="513.9" widt
-000061c0: 683d 2231 3232 3022 2068 6569 6768 743d  h="1220" height=
-000061d0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000061e0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000061f0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00006200: 3d22 2332 3732 3832 3222 2078 3d22 3139  ="#272822" x="19
-00006210: 3135 2e34 2220 793d 2235 3133 2e39 2220  15.4" y="513.9" 
-00006220: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00006230: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00006240: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00006250: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00006260: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00006270: 3d22 3139 3237 2e36 2220 793d 2235 3133  ="1927.6" y="513
-00006280: 2e39 2220 7769 6474 683d 2232 342e 3422  .9" width="24.4"
-00006290: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000062a0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000062b0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000062c0: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
-000062d0: 6622 2078 3d22 3022 2079 3d22 3533 382e  f" x="0" y="538.
-000062e0: 3322 2077 6964 7468 3d22 3435 312e 3422  3" width="451.4"
-000062f0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00006300: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00006310: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00006320: 6563 7420 6669 6c6c 3d22 2332 3732 3832  ect fill="#27282
-00006330: 3222 2078 3d22 3435 312e 3422 2079 3d22  2" x="451.4" y="
-00006340: 3533 382e 3322 2077 6964 7468 3d22 3134  538.3" width="14
-00006350: 3736 2e32 2220 6865 6967 6874 3d22 3234  76.2" height="24
-00006360: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00006370: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00006380: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00006390: 3233 3536 3862 2220 783d 2231 3932 372e  23568b" x="1927.
-000063a0: 3622 2079 3d22 3533 382e 3322 2077 6964  6" y="538.3" wid
-000063b0: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
-000063c0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000063d0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000063e0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000063f0: 6c3d 2223 3234 3239 3266 2220 783d 2230  l="#24292f" x="0
-00006400: 2220 793d 2235 3632 2e37 2220 7769 6474  " y="562.7" widt
-00006410: 683d 2234 3531 2e34 2220 6865 6967 6874  h="451.4" height
-00006420: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00006430: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00006440: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00006450: 6c3d 2223 3064 3064 3064 2220 783d 2234  l="#0d0d0d" x="4
-00006460: 3531 2e34 2220 793d 2235 3632 2e37 2220  51.4" y="562.7" 
-00006470: 7769 6474 683d 2231 3437 362e 3222 2068  width="1476.2" h
-00006480: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006490: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000064a0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000064b0: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-000064c0: 2078 3d22 3139 3237 2e36 2220 793d 2235   x="1927.6" y="5
-000064d0: 3632 2e37 2220 7769 6474 683d 2232 342e  62.7" width="24.
-000064e0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-000064f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006500: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006510: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
-00006520: 3932 6622 2078 3d22 3022 2079 3d22 3538  92f" x="0" y="58
-00006530: 372e 3122 2077 6964 7468 3d22 3435 312e  7.1" width="451.
-00006540: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00006550: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006560: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006570: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00006580: 6430 6422 2078 3d22 3435 312e 3422 2079  d0d" x="451.4" y
-00006590: 3d22 3538 372e 3122 2077 6964 7468 3d22  ="587.1" width="
-000065a0: 3134 3736 2e32 2220 6865 6967 6874 3d22  1476.2" height="
-000065b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000065c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000065d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-000065e0: 2223 3233 3536 3862 2220 783d 2231 3932  "#23568b" x="192
-000065f0: 372e 3622 2079 3d22 3538 372e 3122 2077  7.6" y="587.1" w
-00006600: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
-00006610: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00006620: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00006630: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00006640: 696c 6c3d 2223 3234 3239 3266 2220 783d  ill="#24292f" x=
-00006650: 2230 2220 793d 2236 3131 2e35 2220 7769  "0" y="611.5" wi
-00006660: 6474 683d 2234 3531 2e34 2220 6865 6967  dth="451.4" heig
-00006670: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00006680: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00006690: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-000066a0: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
-000066b0: 2234 3531 2e34 2220 793d 2236 3131 2e35  "451.4" y="611.5
-000066c0: 2220 7769 6474 683d 2236 3232 2e32 2220  " width="622.2" 
-000066d0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-000066e0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-000066f0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00006700: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
-00006710: 2220 783d 2231 3037 332e 3622 2079 3d22  " x="1073.6" y="
-00006720: 3631 312e 3522 2077 6964 7468 3d22 3231  611.5" width="21
-00006730: 392e 3622 2068 6569 6768 743d 2232 342e  9.6" height="24.
-00006740: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00006750: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00006760: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00006770: 6430 6430 6422 2078 3d22 3132 3933 2e32  d0d0d" x="1293.2
-00006780: 2220 793d 2236 3131 2e35 2220 7769 6474  " y="611.5" widt
-00006790: 683d 2236 3334 2e34 2220 6865 6967 6874  h="634.4" height
-000067a0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000067b0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000067c0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000067d0: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
-000067e0: 3932 372e 3622 2079 3d22 3631 312e 3522  927.6" y="611.5"
-000067f0: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-00006800: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00006810: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00006820: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00006830: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00006840: 783d 2230 2220 793d 2236 3335 2e39 2220  x="0" y="635.9" 
-00006850: 7769 6474 683d 2234 3531 2e34 2220 6865  width="451.4" he
-00006860: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00006870: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00006880: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00006890: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
-000068a0: 783d 2234 3531 2e34 2220 793d 2236 3335  x="451.4" y="635
-000068b0: 2e39 2220 7769 6474 683d 2231 3437 362e  .9" width="1476.
-000068c0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-000068d0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000068e0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000068f0: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-00006900: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
-00006910: 793d 2236 3335 2e39 2220 7769 6474 683d  y="635.9" width=
-00006920: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
-00006930: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00006940: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00006950: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00006960: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
-00006970: 3d22 3636 302e 3322 2077 6964 7468 3d22  ="660.3" width="
-00006980: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
-00006990: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000069a0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000069b0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000069c0: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
-000069d0: 3422 2079 3d22 3636 302e 3322 2077 6964  4" y="660.3" wid
-000069e0: 7468 3d22 3330 3522 2068 6569 6768 743d  th="305" height=
-000069f0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00006a00: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00006a10: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00006a20: 3d22 2334 6234 6535 3522 2078 3d22 3735  ="#4b4e55" x="75
-00006a30: 362e 3422 2079 3d22 3636 302e 3322 2077  6.4" y="660.3" w
-00006a40: 6964 7468 3d22 3733 2e32 2220 6865 6967  idth="73.2" heig
-00006a50: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00006a60: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00006a70: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00006a80: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
-00006a90: 2238 3239 2e36 2220 793d 2236 3630 2e33  "829.6" y="660.3
-00006aa0: 2220 7769 6474 683d 2237 3933 2220 6865  " width="793" he
-00006ab0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00006ac0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00006ad0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00006ae0: 2066 696c 6c3d 2223 3462 3465 3535 2220   fill="#4b4e55" 
-00006af0: 783d 2231 3632 322e 3622 2079 3d22 3636  x="1622.6" y="66
-00006b00: 302e 3322 2077 6964 7468 3d22 3733 2e32  0.3" width="73.2
-00006b10: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00006b20: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00006b30: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00006b40: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00006b50: 3064 2220 783d 2231 3639 352e 3822 2079  0d" x="1695.8" y
-00006b60: 3d22 3636 302e 3322 2077 6964 7468 3d22  ="660.3" width="
-00006b70: 3835 2e34 2220 6865 6967 6874 3d22 3234  85.4" height="24
-00006b80: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00006b90: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00006ba0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00006bb0: 3064 3064 3064 2220 783d 2231 3738 312e  0d0d0d" x="1781.
-00006bc0: 3222 2079 3d22 3636 302e 3322 2077 6964  2" y="660.3" wid
-00006bd0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00006be0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00006bf0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00006c00: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00006c10: 6c3d 2223 3064 3064 3064 2220 783d 2231  l="#0d0d0d" x="1
-00006c20: 3739 332e 3422 2079 3d22 3636 302e 3322  793.4" y="660.3"
-00006c30: 2077 6964 7468 3d22 3130 392e 3822 2068   width="109.8" h
-00006c40: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006c50: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00006c60: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00006c70: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00006c80: 2078 3d22 3139 3033 2e32 2220 793d 2236   x="1903.2" y="6
-00006c90: 3630 2e33 2220 7769 6474 683d 2232 342e  60.3" width="24.
-00006ca0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00006cb0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006cc0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006cd0: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-00006ce0: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
-00006cf0: 793d 2236 3630 2e33 2220 7769 6474 683d  y="660.3" width=
-00006d00: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
-00006d10: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00006d20: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00006d30: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00006d40: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
-00006d50: 3d22 3638 342e 3722 2077 6964 7468 3d22  ="684.7" width="
-00006d60: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
-00006d70: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00006d80: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00006d90: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00006da0: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
-00006db0: 3422 2079 3d22 3638 342e 3722 2077 6964  4" y="684.7" wid
-00006dc0: 7468 3d22 3639 352e 3422 2068 6569 6768  th="695.4" heigh
-00006dd0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00006de0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00006df0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00006e00: 6c6c 3d22 2334 6234 6535 3522 2078 3d22  ll="#4b4e55" x="
-00006e10: 3131 3436 2e38 2220 793d 2236 3834 2e37  1146.8" y="684.7
-00006e20: 2220 7769 6474 683d 2238 352e 3422 2068  " width="85.4" h
-00006e30: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006e40: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00006e50: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00006e60: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00006e70: 2078 3d22 3132 3332 2e32 2220 793d 2236   x="1232.2" y="6
-00006e80: 3834 2e37 2220 7769 6474 683d 2233 3035  84.7" width="305
-00006e90: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00006ea0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00006eb0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00006ec0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00006ed0: 3064 2220 783d 2231 3533 372e 3222 2079  0d" x="1537.2" y
-00006ee0: 3d22 3638 342e 3722 2077 6964 7468 3d22  ="684.7" width="
-00006ef0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-00006f00: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00006f10: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00006f20: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00006f30: 3064 3064 3064 2220 783d 2231 3534 392e  0d0d0d" x="1549.
-00006f40: 3422 2079 3d22 3638 342e 3722 2077 6964  4" y="684.7" wid
-00006f50: 7468 3d22 3234 3422 2068 6569 6768 743d  th="244" height=
-00006f60: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00006f70: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00006f80: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00006f90: 3d22 2334 6234 6535 3522 2078 3d22 3137  ="#4b4e55" x="17
-00006fa0: 3933 2e34 2220 793d 2236 3834 2e37 2220  93.4" y="684.7" 
-00006fb0: 7769 6474 683d 2233 362e 3622 2068 6569  width="36.6" hei
-00006fc0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00006fd0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00006fe0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00006ff0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00007000: 3d22 3138 3330 2220 793d 2236 3834 2e37  ="1830" y="684.7
-00007010: 2220 7769 6474 683d 2238 352e 3422 2068  " width="85.4" h
-00007020: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00007030: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00007040: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00007050: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00007060: 2078 3d22 3139 3135 2e34 2220 793d 2236   x="1915.4" y="6
-00007070: 3834 2e37 2220 7769 6474 683d 2231 322e  84.7" width="12.
-00007080: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00007090: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000070a0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000070b0: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-000070c0: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
-000070d0: 793d 2236 3834 2e37 2220 7769 6474 683d  y="684.7" width=
-000070e0: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
-000070f0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00007100: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00007110: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00007120: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
-00007130: 3d22 3730 392e 3122 2077 6964 7468 3d22  ="709.1" width="
-00007140: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
-00007150: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00007160: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00007170: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00007180: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
-00007190: 3422 2079 3d22 3730 392e 3122 2077 6964  4" y="709.1" wid
-000071a0: 7468 3d22 3236 382e 3422 2068 6569 6768  th="268.4" heigh
-000071b0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-000071c0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000071d0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000071e0: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-000071f0: 3731 392e 3822 2079 3d22 3730 392e 3122  719.8" y="709.1"
-00007200: 2077 6964 7468 3d22 3132 3037 2e38 2220   width="1207.8" 
-00007210: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00007220: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00007230: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00007240: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
-00007250: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00007260: 3730 392e 3122 2077 6964 7468 3d22 3234  709.1" width="24
-00007270: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00007280: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00007290: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000072a0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-000072b0: 3239 3266 2220 783d 2230 2220 793d 2237  292f" x="0" y="7
-000072c0: 3333 2e35 2220 7769 6474 683d 2234 3531  33.5" width="451
-000072d0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-000072e0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000072f0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00007300: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00007310: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
-00007320: 793d 2237 3333 2e35 2220 7769 6474 683d  y="733.5" width=
-00007330: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
-00007340: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00007350: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00007360: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00007370: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
-00007380: 3237 2e36 2220 793d 2237 3333 2e35 2220  27.6" y="733.5" 
-00007390: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-000073a0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000073b0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000073c0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000073d0: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-000073e0: 3d22 3022 2079 3d22 3735 372e 3922 2077  ="0" y="757.9" w
-000073f0: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
-00007400: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00007410: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00007420: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00007430: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
-00007440: 3d22 3435 312e 3422 2079 3d22 3735 372e  ="451.4" y="757.
-00007450: 3922 2077 6964 7468 3d22 3134 3736 2e32  9" width="1476.2
-00007460: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00007470: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00007480: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00007490: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
-000074a0: 3862 2220 783d 2231 3932 372e 3622 2079  8b" x="1927.6" y
-000074b0: 3d22 3735 372e 3922 2077 6964 7468 3d22  ="757.9" width="
-000074c0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-000074d0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-000074e0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-000074f0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00007500: 3234 3239 3266 2220 783d 2230 2220 793d  24292f" x="0" y=
-00007510: 2237 3832 2e33 2220 7769 6474 683d 2234  "782.3" width="4
-00007520: 3531 2e34 2220 6865 6967 6874 3d22 3234  51.4" height="24
-00007530: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00007540: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00007550: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00007560: 3237 3238 3232 2220 783d 2234 3531 2e34  272822" x="451.4
-00007570: 2220 793d 2237 3832 2e33 2220 7769 6474  " y="782.3" widt
-00007580: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00007590: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000075a0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000075b0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000075c0: 3d22 2332 3732 3832 3222 2078 3d22 3436  ="#272822" x="46
-000075d0: 332e 3622 2079 3d22 3738 322e 3322 2077  3.6" y="782.3" w
-000075e0: 6964 7468 3d22 3438 2e38 2220 6865 6967  idth="48.8" heig
-000075f0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00007600: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00007610: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00007620: 696c 6c3d 2223 3237 3238 3232 2220 783d  ill="#272822" x=
-00007630: 2235 3132 2e34 2220 793d 2237 3832 2e33  "512.4" y="782.3
-00007640: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00007650: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00007660: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00007670: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00007680: 7420 6669 6c6c 3d22 2332 3732 3832 3222  t fill="#272822"
-00007690: 2078 3d22 3532 342e 3622 2079 3d22 3738   x="524.6" y="78
-000076a0: 322e 3322 2077 6964 7468 3d22 3835 2e34  2.3" width="85.4
-000076b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000076c0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000076d0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000076e0: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
-000076f0: 3232 2220 783d 2236 3130 2220 793d 2237  22" x="610" y="7
-00007700: 3832 2e33 2220 7769 6474 683d 2231 322e  82.3" width="12.
-00007710: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00007720: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007730: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007740: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
-00007750: 3832 3222 2078 3d22 3632 322e 3222 2079  822" x="622.2" y
-00007760: 3d22 3738 322e 3322 2077 6964 7468 3d22  ="782.3" width="
-00007770: 3135 382e 3622 2068 6569 6768 743d 2232  158.6" height="2
-00007780: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00007790: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000077a0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000077b0: 2332 3732 3832 3222 2078 3d22 3738 302e  #272822" x="780.
-000077c0: 3822 2079 3d22 3738 322e 3322 2077 6964  8" y="782.3" wid
-000077d0: 7468 3d22 3131 3334 2e36 2220 6865 6967  th="1134.6" heig
-000077e0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-000077f0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00007800: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00007810: 696c 6c3d 2223 3237 3238 3232 2220 783d  ill="#272822" x=
-00007820: 2231 3931 352e 3422 2079 3d22 3738 322e  "1915.4" y="782.
-00007830: 3322 2077 6964 7468 3d22 3132 2e32 2220  3" width="12.2" 
-00007840: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00007850: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00007860: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00007870: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
-00007880: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00007890: 3738 322e 3322 2077 6964 7468 3d22 3234  782.3" width="24
-000078a0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-000078b0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000078c0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000078d0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-000078e0: 3239 3266 2220 783d 2230 2220 793d 2238  292f" x="0" y="8
-000078f0: 3036 2e37 2220 7769 6474 683d 2234 3531  06.7" width="451
-00007900: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00007910: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00007920: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00007930: 3e3c 7265 6374 2066 696c 6c3d 2223 3237  ><rect fill="#27
-00007940: 3238 3232 2220 783d 2234 3531 2e34 2220  2822" x="451.4" 
-00007950: 793d 2238 3036 2e37 2220 7769 6474 683d  y="806.7" width=
-00007960: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
-00007970: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00007980: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00007990: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000079a0: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
-000079b0: 3237 2e36 2220 793d 2238 3036 2e37 2220  27.6" y="806.7" 
-000079c0: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-000079d0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000079e0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000079f0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00007a00: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
-00007a10: 3d22 3022 2079 3d22 3833 312e 3122 2077  ="0" y="831.1" w
-00007a20: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
-00007a30: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00007a40: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00007a50: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00007a60: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00007a70: 3d22 3435 312e 3422 2079 3d22 3833 312e  ="451.4" y="831.
-00007a80: 3122 2077 6964 7468 3d22 3134 3736 2e32  1" width="1476.2
-00007a90: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00007aa0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00007ab0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00007ac0: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
-00007ad0: 3862 2220 783d 2231 3932 372e 3622 2079  8b" x="1927.6" y
-00007ae0: 3d22 3833 312e 3122 2077 6964 7468 3d22  ="831.1" width="
-00007af0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-00007b00: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00007b10: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00007b20: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00007b30: 3234 3239 3266 2220 783d 2230 2220 793d  24292f" x="0" y=
-00007b40: 2238 3535 2e35 2220 7769 6474 683d 2234  "855.5" width="4
-00007b50: 3531 2e34 2220 6865 6967 6874 3d22 3234  51.4" height="24
-00007b60: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00007b70: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00007b80: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00007b90: 3064 3064 3064 2220 783d 2234 3531 2e34  0d0d0d" x="451.4
-00007ba0: 2220 793d 2238 3535 2e35 2220 7769 6474  " y="855.5" widt
-00007bb0: 683d 2231 3437 362e 3222 2068 6569 6768  h="1476.2" heigh
-00007bc0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00007bd0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00007be0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00007bf0: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-00007c00: 3139 3237 2e36 2220 793d 2238 3535 2e35  1927.6" y="855.5
-00007c10: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
-00007c20: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00007c30: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00007c40: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00007c50: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
-00007c60: 2078 3d22 3022 2079 3d22 3837 392e 3922   x="0" y="879.9"
-00007c70: 2077 6964 7468 3d22 3435 312e 3422 2068   width="451.4" h
-00007c80: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00007c90: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00007ca0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00007cb0: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00007cc0: 2078 3d22 3435 312e 3422 2079 3d22 3837   x="451.4" y="87
-00007cd0: 392e 3922 2077 6964 7468 3d22 3730 372e  9.9" width="707.
-00007ce0: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
-00007cf0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007d00: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007d10: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00007d20: 6430 6422 2078 3d22 3131 3539 2220 793d  d0d" x="1159" y=
-00007d30: 2238 3739 2e39 2220 7769 6474 683d 2236  "879.9" width="6
-00007d40: 3122 2068 6569 6768 743d 2232 342e 3635  1" height="24.65
-00007d50: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007d60: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007d70: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00007d80: 6430 6422 2078 3d22 3132 3230 2220 793d  d0d" x="1220" y=
-00007d90: 2238 3739 2e39 2220 7769 6474 683d 2237  "879.9" width="7
-00007da0: 3037 2e36 2220 6865 6967 6874 3d22 3234  07.6" height="24
-00007db0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00007dc0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00007dd0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00007de0: 3233 3536 3862 2220 783d 2231 3932 372e  23568b" x="1927.
-00007df0: 3622 2079 3d22 3837 392e 3922 2077 6964  6" y="879.9" wid
-00007e00: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
-00007e10: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00007e20: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00007e30: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00007e40: 6c3d 2223 3234 3239 3266 2220 783d 2230  l="#24292f" x="0
-00007e50: 2220 793d 2239 3034 2e33 2220 7769 6474  " y="904.3" widt
-00007e60: 683d 2234 3531 2e34 2220 6865 6967 6874  h="451.4" height
-00007e70: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00007e80: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00007e90: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00007ea0: 6c3d 2223 3064 3064 3064 2220 783d 2234  l="#0d0d0d" x="4
-00007eb0: 3531 2e34 2220 793d 2239 3034 2e33 2220  51.4" y="904.3" 
-00007ec0: 7769 6474 683d 2231 3437 362e 3222 2068  width="1476.2" h
-00007ed0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00007ee0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00007ef0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00007f00: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-00007f10: 2078 3d22 3139 3237 2e36 2220 793d 2239   x="1927.6" y="9
-00007f20: 3034 2e33 2220 7769 6474 683d 2232 342e  04.3" width="24.
-00007f30: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00007f40: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007f50: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007f60: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
-00007f70: 3932 6622 2078 3d22 3022 2079 3d22 3932  92f" x="0" y="92
-00007f80: 382e 3722 2077 6964 7468 3d22 3435 312e  8.7" width="451.
-00007f90: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00007fa0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007fb0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007fc0: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
-00007fd0: 3832 3222 2078 3d22 3435 312e 3422 2079  822" x="451.4" y
-00007fe0: 3d22 3932 382e 3722 2077 6964 7468 3d22  ="928.7" width="
-00007ff0: 3134 3736 2e32 2220 6865 6967 6874 3d22  1476.2" height="
-00008000: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00008010: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00008020: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00008030: 2223 3233 3536 3862 2220 783d 2231 3932  "#23568b" x="192
-00008040: 372e 3622 2079 3d22 3932 382e 3722 2077  7.6" y="928.7" w
-00008050: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
-00008060: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00008070: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00008080: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00008090: 696c 6c3d 2223 3234 3239 3266 2220 783d  ill="#24292f" x=
-000080a0: 2230 2220 793d 2239 3533 2e31 2220 7769  "0" y="953.1" wi
-000080b0: 6474 683d 2234 3531 2e34 2220 6865 6967  dth="451.4" heig
-000080c0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-000080d0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-000080e0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-000080f0: 696c 6c3d 2223 3237 3238 3232 2220 783d  ill="#272822" x=
-00008100: 2234 3531 2e34 2220 793d 2239 3533 2e31  "451.4" y="953.1
-00008110: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00008120: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00008130: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00008140: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00008150: 7420 6669 6c6c 3d22 2332 3732 3832 3222  t fill="#272822"
-00008160: 2078 3d22 3436 332e 3622 2079 3d22 3935   x="463.6" y="95
-00008170: 332e 3122 2077 6964 7468 3d22 3733 2e32  3.1" width="73.2
-00008180: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00008190: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000081a0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000081b0: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
-000081c0: 3232 2220 783d 2235 3336 2e38 2220 793d  22" x="536.8" y=
-000081d0: 2239 3533 2e31 2220 7769 6474 683d 2231  "953.1" width="1
-000081e0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-000081f0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00008200: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00008210: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00008220: 3732 3832 3222 2078 3d22 3534 3922 2079  72822" x="549" y
-00008230: 3d22 3935 332e 3122 2077 6964 7468 3d22  ="953.1" width="
-00008240: 3134 362e 3422 2068 6569 6768 743d 2232  146.4" height="2
-00008250: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00008260: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00008270: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00008280: 2332 3732 3832 3222 2078 3d22 3639 352e  #272822" x="695.
-00008290: 3422 2079 3d22 3935 332e 3122 2077 6964  4" y="953.1" wid
-000082a0: 7468 3d22 3132 3230 2220 6865 6967 6874  th="1220" height
-000082b0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000082c0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000082d0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000082e0: 6c3d 2223 3237 3238 3232 2220 783d 2231  l="#272822" x="1
-000082f0: 3931 352e 3422 2079 3d22 3935 332e 3122  915.4" y="953.1"
-00008300: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
-00008310: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00008320: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00008330: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00008340: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-00008350: 783d 2231 3932 372e 3622 2079 3d22 3935  x="1927.6" y="95
-00008360: 332e 3122 2077 6964 7468 3d22 3234 2e34  3.1" width="24.4
-00008370: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00008380: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00008390: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000083a0: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
-000083b0: 3266 2220 783d 2230 2220 793d 2239 3737  2f" x="0" y="977
-000083c0: 2e35 2220 7769 6474 683d 2234 3531 2e34  .5" width="451.4
-000083d0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000083e0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000083f0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00008400: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
-00008410: 3232 2220 783d 2234 3531 2e34 2220 793d  22" x="451.4" y=
-00008420: 2239 3737 2e35 2220 7769 6474 683d 2231  "977.5" width="1
-00008430: 3437 362e 3222 2068 6569 6768 743d 2232  476.2" height="2
-00008440: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00008450: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00008460: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00008470: 2331 3431 3931 6622 2078 3d22 3139 3237  #14191f" x="1927
-00008480: 2e36 2220 793d 2239 3737 2e35 2220 7769  .6" y="977.5" wi
-00008490: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
-000084a0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-000084b0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000084c0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000084d0: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
-000084e0: 3022 2079 3d22 3130 3031 2e39 2220 7769  0" y="1001.9" wi
-000084f0: 6474 683d 2234 3531 2e34 2220 6865 6967  dth="451.4" heig
-00008500: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00008510: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00008520: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00008530: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
-00008540: 2234 3531 2e34 2220 793d 2231 3030 312e  "451.4" y="1001.
-00008550: 3922 2077 6964 7468 3d22 3134 3736 2e32  9" width="1476.2
-00008560: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00008570: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00008580: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00008590: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-000085a0: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
-000085b0: 3d22 3130 3031 2e39 2220 7769 6474 683d  ="1001.9" width=
-000085c0: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
-000085d0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000085e0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000085f0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00008600: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
-00008610: 3d22 3130 3236 2e33 2220 7769 6474 683d  ="1026.3" width=
-00008620: 2234 3531 2e34 2220 6865 6967 6874 3d22  "451.4" height="
-00008630: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00008640: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00008650: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00008660: 2223 3064 3064 3064 2220 783d 2234 3531  "#0d0d0d" x="451
-00008670: 2e34 2220 793d 2231 3032 362e 3322 2077  .4" y="1026.3" w
-00008680: 6964 7468 3d22 3134 362e 3422 2068 6569  idth="146.4" hei
+00000600: 6c2d 3231 3637 3038 3133 3630 2d72 3720  l-2167081360-r7 
+00000610: 7b20 6669 6c6c 3a20 2366 6561 3632 623b  { fill: #fea62b;
+00000620: 666f 6e74 2d77 6569 6768 743a 2062 6f6c  font-weight: bol
+00000630: 6420 7d0a 2e74 6572 6d69 6e61 6c2d 3231  d }..terminal-21
+00000640: 3637 3038 3133 3630 2d72 3820 7b20 6669  67081360-r8 { fi
+00000650: 6c6c 3a20 2339 3139 3439 373b 666f 6e74  ll: #919497;font
+00000660: 2d77 6569 6768 743a 2062 6f6c 6420 7d0a  -weight: bold }.
+00000670: 2e74 6572 6d69 6e61 6c2d 3231 3637 3038  .terminal-216708
+00000680: 3133 3630 2d72 3920 7b20 6669 6c6c 3a20  1360-r9 { fill: 
+00000690: 2364 6664 6664 663b 666f 6e74 2d77 6569  #dfdfdf;font-wei
+000006a0: 6768 743a 2062 6f6c 6420 7d0a 2e74 6572  ght: bold }..ter
+000006b0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+000006c0: 2d72 3130 207b 2066 696c 6c3a 2023 6532  -r10 { fill: #e2
+000006d0: 6533 6533 3b66 6f6e 742d 7765 6967 6874  e3e3;font-weight
+000006e0: 3a20 626f 6c64 207d 0a2e 7465 726d 696e  : bold }..termin
+000006f0: 616c 2d32 3136 3730 3831 3336 302d 7231  al-2167081360-r1
+00000700: 3120 7b20 6669 6c6c 3a20 2336 3038 6162  1 { fill: #608ab
+00000710: 313b 7465 7874 2d64 6563 6f72 6174 696f  1;text-decoratio
+00000720: 6e3a 2075 6e64 6572 6c69 6e65 3b20 7d0a  n: underline; }.
+00000730: 2e74 6572 6d69 6e61 6c2d 3231 3637 3038  .terminal-216708
+00000740: 3133 3630 2d72 3132 207b 2066 696c 6c3a  1360-r12 { fill:
+00000750: 2023 3931 3934 3937 3b66 6f6e 742d 7374   #919497;font-st
+00000760: 796c 653a 2069 7461 6c69 633b 207d 0a2e  yle: italic; }..
+00000770: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+00000780: 3336 302d 7231 3320 7b20 6669 6c6c 3a20  360-r13 { fill: 
+00000790: 2336 3861 3062 333b 666f 6e74 2d77 6569  #68a0b3;font-wei
+000007a0: 6768 743a 2062 6f6c 6420 7d0a 2e74 6572  ght: bold }..ter
+000007b0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+000007c0: 2d72 3134 207b 2066 696c 6c3a 2023 6532  -r14 { fill: #e2
+000007d0: 6533 6533 3b66 6f6e 742d 7374 796c 653a  e3e3;font-style:
+000007e0: 2069 7461 6c69 633b 207d 0a2e 7465 726d   italic; }..term
+000007f0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+00000800: 7231 3520 7b20 6669 6c6c 3a20 2364 6664  r15 { fill: #dfd
+00000810: 6664 663b 666f 6e74 2d77 6569 6768 743a  fdf;font-weight:
+00000820: 2062 6f6c 643b 7465 7874 2d64 6563 6f72   bold;text-decor
+00000830: 6174 696f 6e3a 2075 6e64 6572 6c69 6e65  ation: underline
+00000840: 3b20 7d0a 2e74 6572 6d69 6e61 6c2d 3231  ; }..terminal-21
+00000850: 3637 3038 3133 3630 2d72 3136 207b 2066  67081360-r16 { f
+00000860: 696c 6c3a 2023 6638 6638 6632 207d 0a2e  ill: #f8f8f2 }..
+00000870: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+00000880: 3336 302d 7231 3720 7b20 6669 6c6c 3a20  360-r17 { fill: 
+00000890: 2365 3664 6237 3420 7d0a 2e74 6572 6d69  #e6db74 }..termi
+000008a0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+000008b0: 3138 207b 2066 696c 6c3a 2023 3134 3139  18 { fill: #1419
+000008c0: 3166 207d 0a2e 7465 726d 696e 616c 2d32  1f }..terminal-2
+000008d0: 3136 3730 3831 3336 302d 7231 3920 7b20  167081360-r19 { 
+000008e0: 6669 6c6c 3a20 2338 3461 3463 6320 7d0a  fill: #84a4cc }.
+000008f0: 2e74 6572 6d69 6e61 6c2d 3231 3637 3038  .terminal-216708
+00000900: 3133 3630 2d72 3230 207b 2066 696c 6c3a  1360-r20 { fill:
+00000910: 2023 6464 6538 6633 3b66 6f6e 742d 7765   #dde8f3;font-we
+00000920: 6967 6874 3a20 626f 6c64 207d 0a2e 7465  ight: bold }..te
+00000930: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+00000940: 302d 7232 3120 7b20 6669 6c6c 3a20 2364  0-r21 { fill: #d
+00000950: 6465 6466 3920 7d0a 2020 2020 3c2f 7374  dedf9 }.    </st
+00000960: 796c 653e 0a0a 2020 2020 3c64 6566 733e  yle>..    <defs>
+00000970: 0a20 2020 203c 636c 6970 5061 7468 2069  .    <clipPath i
+00000980: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00000990: 3038 3133 3630 2d63 6c69 702d 7465 726d  081360-clip-term
+000009a0: 696e 616c 223e 0a20 2020 2020 203c 7265  inal">.      <re
+000009b0: 6374 2078 3d22 3022 2079 3d22 3022 2077  ct x="0" y="0" w
+000009c0: 6964 7468 3d22 3139 3531 2e30 2220 6865  idth="1951.0" he
+000009d0: 6967 6874 3d22 3131 3730 2e31 3939 3939  ight="1170.19999
+000009e0: 3939 3939 3939 3938 2220 2f3e 0a20 2020  99999998" />.   
+000009f0: 203c 2f63 6c69 7050 6174 683e 0a20 2020   </clipPath>.   
+00000a00: 203c 636c 6970 5061 7468 2069 643d 2274   <clipPath id="t
+00000a10: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00000a20: 3630 2d6c 696e 652d 3022 3e0a 2020 2020  60-line-0">.    
+00000a30: 3c72 6563 7420 783d 2230 2220 793d 2231  <rect x="0" y="1
+00000a40: 2e35 2220 7769 6474 683d 2231 3935 3222  .5" width="1952"
+00000a50: 2068 6569 6768 743d 2232 342e 3635 222f   height="24.65"/
+00000a60: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00000a70: 636c 6970 5061 7468 3e0a 3c63 6c69 7050  clipPath>.<clipP
+00000a80: 6174 6820 6964 3d22 7465 726d 696e 616c  ath id="terminal
+00000a90: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+00000aa0: 2d31 223e 0a20 2020 203c 7265 6374 2078  -1">.    <rect x
+00000ab0: 3d22 3022 2079 3d22 3235 2e39 2220 7769  ="0" y="25.9" wi
+00000ac0: 6474 683d 2231 3935 3222 2068 6569 6768  dth="1952" heigh
+00000ad0: 743d 2232 342e 3635 222f 3e0a 2020 2020  t="24.65"/>.    
+00000ae0: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
+00000af0: 7468 3e0a 3c63 6c69 7050 6174 6820 6964  th>.<clipPath id
+00000b00: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+00000b10: 3831 3336 302d 6c69 6e65 2d32 223e 0a20  81360-line-2">. 
+00000b20: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
+00000b30: 3d22 3530 2e33 2220 7769 6474 683d 2231  ="50.3" width="1
+00000b40: 3935 3222 2068 6569 6768 743d 2232 342e  952" height="24.
+00000b50: 3635 222f 3e0a 2020 2020 2020 2020 2020  65"/>.          
+00000b60: 2020 3c2f 636c 6970 5061 7468 3e0a 3c63    </clipPath>.<c
+00000b70: 6c69 7050 6174 6820 6964 3d22 7465 726d  lipPath id="term
+00000b80: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+00000b90: 6c69 6e65 2d33 223e 0a20 2020 203c 7265  line-3">.    <re
+00000ba0: 6374 2078 3d22 3022 2079 3d22 3734 2e37  ct x="0" y="74.7
+00000bb0: 2220 7769 6474 683d 2231 3935 3222 2068  " width="1952" h
+00000bc0: 6569 6768 743d 2232 342e 3635 222f 3e0a  eight="24.65"/>.
+00000bd0: 2020 2020 2020 2020 2020 2020 3c2f 636c              </cl
+00000be0: 6970 5061 7468 3e0a 3c63 6c69 7050 6174  ipPath>.<clipPat
+00000bf0: 6820 6964 3d22 7465 726d 696e 616c 2d32  h id="terminal-2
+00000c00: 3136 3730 3831 3336 302d 6c69 6e65 2d34  167081360-line-4
+00000c10: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
+00000c20: 3022 2079 3d22 3939 2e31 2220 7769 6474  0" y="99.1" widt
+00000c30: 683d 2231 3935 3222 2068 6569 6768 743d  h="1952" height=
+00000c40: 2232 342e 3635 222f 3e0a 2020 2020 2020  "24.65"/>.      
+00000c50: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
+00000c60: 3e0a 3c63 6c69 7050 6174 6820 6964 3d22  >.<clipPath id="
+00000c70: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+00000c80: 3336 302d 6c69 6e65 2d35 223e 0a20 2020  360-line-5">.   
+00000c90: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+00000ca0: 3132 332e 3522 2077 6964 7468 3d22 3139  123.5" width="19
+00000cb0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+00000cc0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00000cd0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00000ce0: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00000cf0: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00000d00: 696e 652d 3622 3e0a 2020 2020 3c72 6563  ine-6">.    <rec
+00000d10: 7420 783d 2230 2220 793d 2231 3437 2e39  t x="0" y="147.9
+00000d20: 2220 7769 6474 683d 2231 3935 3222 2068  " width="1952" h
+00000d30: 6569 6768 743d 2232 342e 3635 222f 3e0a  eight="24.65"/>.
+00000d40: 2020 2020 2020 2020 2020 2020 3c2f 636c              </cl
+00000d50: 6970 5061 7468 3e0a 3c63 6c69 7050 6174  ipPath>.<clipPat
+00000d60: 6820 6964 3d22 7465 726d 696e 616c 2d32  h id="terminal-2
+00000d70: 3136 3730 3831 3336 302d 6c69 6e65 2d37  167081360-line-7
+00000d80: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
+00000d90: 3022 2079 3d22 3137 322e 3322 2077 6964  0" y="172.3" wid
+00000da0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
+00000db0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
+00000dc0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
+00000dd0: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
+00000de0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+00000df0: 3133 3630 2d6c 696e 652d 3822 3e0a 2020  1360-line-8">.  
+00000e00: 2020 3c72 6563 7420 783d 2230 2220 793d    <rect x="0" y=
+00000e10: 2231 3936 2e37 2220 7769 6474 683d 2231  "196.7" width="1
+00000e20: 3935 3222 2068 6569 6768 743d 2232 342e  952" height="24.
+00000e30: 3635 222f 3e0a 2020 2020 2020 2020 2020  65"/>.          
+00000e40: 2020 3c2f 636c 6970 5061 7468 3e0a 3c63    </clipPath>.<c
+00000e50: 6c69 7050 6174 6820 6964 3d22 7465 726d  lipPath id="term
+00000e60: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+00000e70: 6c69 6e65 2d39 223e 0a20 2020 203c 7265  line-9">.    <re
+00000e80: 6374 2078 3d22 3022 2079 3d22 3232 312e  ct x="0" y="221.
+00000e90: 3122 2077 6964 7468 3d22 3139 3532 2220  1" width="1952" 
+00000ea0: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00000eb0: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00000ec0: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+00000ed0: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+00000ee0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+00000ef0: 3130 223e 0a20 2020 203c 7265 6374 2078  10">.    <rect x
+00000f00: 3d22 3022 2079 3d22 3234 352e 3522 2077  ="0" y="245.5" w
+00000f10: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+00000f20: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+00000f30: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00000f40: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00000f50: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00000f60: 3038 3133 3630 2d6c 696e 652d 3131 223e  081360-line-11">
+00000f70: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00000f80: 2079 3d22 3236 392e 3922 2077 6964 7468   y="269.9" width
+00000f90: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00000fa0: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00000fb0: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00000fc0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+00000fd0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00000fe0: 3630 2d6c 696e 652d 3132 223e 0a20 2020  60-line-12">.   
+00000ff0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+00001000: 3239 342e 3322 2077 6964 7468 3d22 3139  294.3" width="19
+00001010: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+00001020: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00001030: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001040: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001050: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001060: 696e 652d 3133 223e 0a20 2020 203c 7265  ine-13">.    <re
+00001070: 6374 2078 3d22 3022 2079 3d22 3331 382e  ct x="0" y="318.
+00001080: 3722 2077 6964 7468 3d22 3139 3532 2220  7" width="1952" 
+00001090: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+000010a0: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+000010b0: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+000010c0: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+000010d0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+000010e0: 3134 223e 0a20 2020 203c 7265 6374 2078  14">.    <rect x
+000010f0: 3d22 3022 2079 3d22 3334 332e 3122 2077  ="0" y="343.1" w
+00001100: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+00001110: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+00001120: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00001130: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001140: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001150: 3038 3133 3630 2d6c 696e 652d 3135 223e  081360-line-15">
+00001160: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001170: 2079 3d22 3336 372e 3522 2077 6964 7468   y="367.5" width
+00001180: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001190: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+000011a0: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+000011b0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+000011c0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+000011d0: 3630 2d6c 696e 652d 3136 223e 0a20 2020  60-line-16">.   
+000011e0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+000011f0: 3339 312e 3922 2077 6964 7468 3d22 3139  391.9" width="19
+00001200: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+00001210: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00001220: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001230: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001240: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001250: 696e 652d 3137 223e 0a20 2020 203c 7265  ine-17">.    <re
+00001260: 6374 2078 3d22 3022 2079 3d22 3431 362e  ct x="0" y="416.
+00001270: 3322 2077 6964 7468 3d22 3139 3532 2220  3" width="1952" 
+00001280: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00001290: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+000012a0: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+000012b0: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+000012c0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+000012d0: 3138 223e 0a20 2020 203c 7265 6374 2078  18">.    <rect x
+000012e0: 3d22 3022 2079 3d22 3434 302e 3722 2077  ="0" y="440.7" w
+000012f0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+00001300: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+00001310: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00001320: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001330: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001340: 3038 3133 3630 2d6c 696e 652d 3139 223e  081360-line-19">
+00001350: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001360: 2079 3d22 3436 352e 3122 2077 6964 7468   y="465.1" width
+00001370: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001380: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001390: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+000013a0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+000013b0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+000013c0: 3630 2d6c 696e 652d 3230 223e 0a20 2020  60-line-20">.   
+000013d0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+000013e0: 3438 392e 3522 2077 6964 7468 3d22 3139  489.5" width="19
+000013f0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+00001400: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00001410: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001420: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001430: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001440: 696e 652d 3231 223e 0a20 2020 203c 7265  ine-21">.    <re
+00001450: 6374 2078 3d22 3022 2079 3d22 3531 332e  ct x="0" y="513.
+00001460: 3922 2077 6964 7468 3d22 3139 3532 2220  9" width="1952" 
+00001470: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00001480: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00001490: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+000014a0: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+000014b0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+000014c0: 3232 223e 0a20 2020 203c 7265 6374 2078  22">.    <rect x
+000014d0: 3d22 3022 2079 3d22 3533 382e 3322 2077  ="0" y="538.3" w
+000014e0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+000014f0: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+00001500: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00001510: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001520: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001530: 3038 3133 3630 2d6c 696e 652d 3233 223e  081360-line-23">
+00001540: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001550: 2079 3d22 3536 322e 3722 2077 6964 7468   y="562.7" width
+00001560: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001570: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001580: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00001590: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+000015a0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+000015b0: 3630 2d6c 696e 652d 3234 223e 0a20 2020  60-line-24">.   
+000015c0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+000015d0: 3538 372e 3122 2077 6964 7468 3d22 3139  587.1" width="19
+000015e0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+000015f0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00001600: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001610: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001620: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001630: 696e 652d 3235 223e 0a20 2020 203c 7265  ine-25">.    <re
+00001640: 6374 2078 3d22 3022 2079 3d22 3631 312e  ct x="0" y="611.
+00001650: 3522 2077 6964 7468 3d22 3139 3532 2220  5" width="1952" 
+00001660: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00001670: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00001680: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+00001690: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+000016a0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+000016b0: 3236 223e 0a20 2020 203c 7265 6374 2078  26">.    <rect x
+000016c0: 3d22 3022 2079 3d22 3633 352e 3922 2077  ="0" y="635.9" w
+000016d0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+000016e0: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+000016f0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00001700: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001710: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001720: 3038 3133 3630 2d6c 696e 652d 3237 223e  081360-line-27">
+00001730: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001740: 2079 3d22 3636 302e 3322 2077 6964 7468   y="660.3" width
+00001750: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001760: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001770: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00001780: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+00001790: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+000017a0: 3630 2d6c 696e 652d 3238 223e 0a20 2020  60-line-28">.   
+000017b0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+000017c0: 3638 342e 3722 2077 6964 7468 3d22 3139  684.7" width="19
+000017d0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+000017e0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+000017f0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001800: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001810: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001820: 696e 652d 3239 223e 0a20 2020 203c 7265  ine-29">.    <re
+00001830: 6374 2078 3d22 3022 2079 3d22 3730 392e  ct x="0" y="709.
+00001840: 3122 2077 6964 7468 3d22 3139 3532 2220  1" width="1952" 
+00001850: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00001860: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00001870: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+00001880: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+00001890: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+000018a0: 3330 223e 0a20 2020 203c 7265 6374 2078  30">.    <rect x
+000018b0: 3d22 3022 2079 3d22 3733 332e 3522 2077  ="0" y="733.5" w
+000018c0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+000018d0: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+000018e0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+000018f0: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001900: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001910: 3038 3133 3630 2d6c 696e 652d 3331 223e  081360-line-31">
+00001920: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001930: 2079 3d22 3735 372e 3922 2077 6964 7468   y="757.9" width
+00001940: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001950: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001960: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00001970: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+00001980: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00001990: 3630 2d6c 696e 652d 3332 223e 0a20 2020  60-line-32">.   
+000019a0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+000019b0: 3738 322e 3322 2077 6964 7468 3d22 3139  782.3" width="19
+000019c0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+000019d0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+000019e0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+000019f0: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001a00: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001a10: 696e 652d 3333 223e 0a20 2020 203c 7265  ine-33">.    <re
+00001a20: 6374 2078 3d22 3022 2079 3d22 3830 362e  ct x="0" y="806.
+00001a30: 3722 2077 6964 7468 3d22 3139 3532 2220  7" width="1952" 
+00001a40: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00001a50: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00001a60: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+00001a70: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+00001a80: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+00001a90: 3334 223e 0a20 2020 203c 7265 6374 2078  34">.    <rect x
+00001aa0: 3d22 3022 2079 3d22 3833 312e 3122 2077  ="0" y="831.1" w
+00001ab0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+00001ac0: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+00001ad0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00001ae0: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001af0: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001b00: 3038 3133 3630 2d6c 696e 652d 3335 223e  081360-line-35">
+00001b10: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001b20: 2079 3d22 3835 352e 3522 2077 6964 7468   y="855.5" width
+00001b30: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001b40: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001b50: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00001b60: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+00001b70: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00001b80: 3630 2d6c 696e 652d 3336 223e 0a20 2020  60-line-36">.   
+00001b90: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+00001ba0: 3837 392e 3922 2077 6964 7468 3d22 3139  879.9" width="19
+00001bb0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+00001bc0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00001bd0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001be0: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001bf0: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001c00: 696e 652d 3337 223e 0a20 2020 203c 7265  ine-37">.    <re
+00001c10: 6374 2078 3d22 3022 2079 3d22 3930 342e  ct x="0" y="904.
+00001c20: 3322 2077 6964 7468 3d22 3139 3532 2220  3" width="1952" 
+00001c30: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
+00001c40: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00001c50: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
+00001c60: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
+00001c70: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+00001c80: 3338 223e 0a20 2020 203c 7265 6374 2078  38">.    <rect x
+00001c90: 3d22 3022 2079 3d22 3932 382e 3722 2077  ="0" y="928.7" w
+00001ca0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
+00001cb0: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
+00001cc0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00001cd0: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
+00001ce0: 643d 2274 6572 6d69 6e61 6c2d 3231 3637  d="terminal-2167
+00001cf0: 3038 3133 3630 2d6c 696e 652d 3339 223e  081360-line-39">
+00001d00: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
+00001d10: 2079 3d22 3935 332e 3122 2077 6964 7468   y="953.1" width
+00001d20: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001d30: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001d40: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00001d50: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+00001d60: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00001d70: 3630 2d6c 696e 652d 3430 223e 0a20 2020  60-line-40">.   
+00001d80: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+00001d90: 3937 372e 3522 2077 6964 7468 3d22 3139  977.5" width="19
+00001da0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
+00001db0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
+00001dc0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
+00001dd0: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
+00001de0: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00001df0: 696e 652d 3431 223e 0a20 2020 203c 7265  ine-41">.    <re
+00001e00: 6374 2078 3d22 3022 2079 3d22 3130 3031  ct x="0" y="1001
+00001e10: 2e39 2220 7769 6474 683d 2231 3935 3222  .9" width="1952"
+00001e20: 2068 6569 6768 743d 2232 342e 3635 222f   height="24.65"/
+00001e30: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00001e40: 636c 6970 5061 7468 3e0a 3c63 6c69 7050  clipPath>.<clipP
+00001e50: 6174 6820 6964 3d22 7465 726d 696e 616c  ath id="terminal
+00001e60: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+00001e70: 2d34 3222 3e0a 2020 2020 3c72 6563 7420  -42">.    <rect 
+00001e80: 783d 2230 2220 793d 2231 3032 362e 3322  x="0" y="1026.3"
+00001e90: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
+00001ea0: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
+00001eb0: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
+00001ec0: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
+00001ed0: 2069 643d 2274 6572 6d69 6e61 6c2d 3231   id="terminal-21
+00001ee0: 3637 3038 3133 3630 2d6c 696e 652d 3433  67081360-line-43
+00001ef0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
+00001f00: 3022 2079 3d22 3130 3530 2e37 2220 7769  0" y="1050.7" wi
+00001f10: 6474 683d 2231 3935 3222 2068 6569 6768  dth="1952" heigh
+00001f20: 743d 2232 342e 3635 222f 3e0a 2020 2020  t="24.65"/>.    
+00001f30: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
+00001f40: 7468 3e0a 3c63 6c69 7050 6174 6820 6964  th>.<clipPath id
+00001f50: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+00001f60: 3831 3336 302d 6c69 6e65 2d34 3422 3e0a  81360-line-44">.
+00001f70: 2020 2020 3c72 6563 7420 783d 2230 2220      <rect x="0" 
+00001f80: 793d 2231 3037 352e 3122 2077 6964 7468  y="1075.1" width
+00001f90: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
+00001fa0: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
+00001fb0: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
+00001fc0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
+00001fd0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00001fe0: 3630 2d6c 696e 652d 3435 223e 0a20 2020  60-line-45">.   
+00001ff0: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
+00002000: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00002010: 3935 3222 2068 6569 6768 743d 2232 342e  952" height="24.
+00002020: 3635 222f 3e0a 2020 2020 2020 2020 2020  65"/>.          
+00002030: 2020 3c2f 636c 6970 5061 7468 3e0a 3c63    </clipPath>.<c
+00002040: 6c69 7050 6174 6820 6964 3d22 7465 726d  lipPath id="term
+00002050: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+00002060: 6c69 6e65 2d34 3622 3e0a 2020 2020 3c72  line-46">.    <r
+00002070: 6563 7420 783d 2230 2220 793d 2231 3132  ect x="0" y="112
+00002080: 332e 3922 2077 6964 7468 3d22 3139 3532  3.9" width="1952
+00002090: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000020a0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+000020b0: 2f63 6c69 7050 6174 683e 0a20 2020 203c  /clipPath>.    <
+000020c0: 2f64 6566 733e 0a0a 2020 2020 3c72 6563  /defs>..    <rec
+000020d0: 7420 6669 6c6c 3d22 2332 3932 3932 3922  t fill="#292929"
+000020e0: 2073 7472 6f6b 653d 2272 6762 6128 3235   stroke="rgba(25
+000020f0: 352c 3235 352c 3235 352c 302e 3335 2922  5,255,255,0.35)"
+00002100: 2073 7472 6f6b 652d 7769 6474 683d 2231   stroke-width="1
+00002110: 2220 783d 2231 2220 793d 2231 2220 7769  " x="1" y="1" wi
+00002120: 6474 683d 2231 3936 3822 2068 6569 6768  dth="1968" heigh
+00002130: 743d 2231 3231 392e 3222 2072 783d 2238  t="1219.2" rx="8
+00002140: 222f 3e3c 7465 7874 2063 6c61 7373 3d22  "/><text class="
+00002150: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+00002160: 3336 302d 7469 746c 6522 2066 696c 6c3d  360-title" fill=
+00002170: 2223 6335 6338 6336 2220 7465 7874 2d61  "#c5c8c6" text-a
+00002180: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
+00002190: 3d22 3938 3422 2079 3d22 3237 223e 6272  ="984" y="27">br
+000021a0: 6f77 7372 3c2f 7465 7874 3e0a 2020 2020  owsr</text>.    
+000021b0: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+000021c0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+000021d0: 3236 2c32 3229 223e 0a20 2020 2020 2020  26,22)">.       
+000021e0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+000021f0: 2230 2220 6379 3d22 3022 2072 3d22 3722  "0" cy="0" r="7"
+00002200: 2066 696c 6c3d 2223 6666 3566 3537 222f   fill="#ff5f57"/
+00002210: 3e0a 2020 2020 2020 2020 2020 2020 3c63  >.            <c
+00002220: 6972 636c 6520 6378 3d22 3232 2220 6379  ircle cx="22" cy
+00002230: 3d22 3022 2072 3d22 3722 2066 696c 6c3d  ="0" r="7" fill=
+00002240: 2223 6665 6263 3265 222f 3e0a 2020 2020  "#febc2e"/>.    
+00002250: 2020 2020 2020 2020 3c63 6972 636c 6520          <circle 
+00002260: 6378 3d22 3434 2220 6379 3d22 3022 2072  cx="44" cy="0" r
+00002270: 3d22 3722 2066 696c 6c3d 2223 3238 6338  ="7" fill="#28c8
+00002280: 3430 222f 3e0a 2020 2020 2020 2020 2020  40"/>.          
+00002290: 2020 3c2f 673e 0a20 2020 2020 2020 200a    </g>.        .
+000022a0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+000022b0: 3d22 7472 616e 736c 6174 6528 392c 2034  ="translate(9, 4
+000022c0: 3129 2220 636c 6970 2d70 6174 683d 2275  1)" clip-path="u
+000022d0: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+000022e0: 3730 3831 3336 302d 636c 6970 2d74 6572  7081360-clip-ter
+000022f0: 6d69 6e61 6c29 223e 0a20 2020 203c 7265  minal)">.    <re
+00002300: 6374 2066 696c 6c3d 2223 3138 3138 3138  ct fill="#181818
+00002310: 2220 783d 2230 2220 793d 2231 2e35 2220  " x="0" y="1.5" 
+00002320: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+00002330: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00002340: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00002350: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00002360: 6669 6c6c 3d22 2331 3831 3831 3822 2078  fill="#181818" x
+00002370: 3d22 3132 2e32 2220 793d 2231 2e35 2220  ="12.2" y="1.5" 
+00002380: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+00002390: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+000023a0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+000023b0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+000023c0: 6669 6c6c 3d22 2331 3831 3831 3822 2078  fill="#181818" x
+000023d0: 3d22 3234 2e34 2220 793d 2231 2e35 2220  ="24.4" y="1.5" 
+000023e0: 7769 6474 683d 2236 3122 2068 6569 6768  width="61" heigh
+000023f0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002400: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002410: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002420: 6c6c 3d22 2331 3831 3831 3822 2078 3d22  ll="#181818" x="
+00002430: 3835 2e34 2220 793d 2231 2e35 2220 7769  85.4" y="1.5" wi
+00002440: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00002450: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002460: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002470: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002480: 6c6c 3d22 2331 3831 3831 3822 2078 3d22  ll="#181818" x="
+00002490: 3937 2e36 2220 793d 2231 2e35 2220 7769  97.6" y="1.5" wi
+000024a0: 6474 683d 2235 3132 2e34 2220 6865 6967  dth="512.4" heig
+000024b0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+000024c0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000024d0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000024e0: 696c 6c3d 2223 3138 3138 3138 2220 783d  ill="#181818" x=
+000024f0: 2236 3130 2220 793d 2231 2e35 2220 7769  "610" y="1.5" wi
+00002500: 6474 683d 2231 3039 2e38 2220 6865 6967  dth="109.8" heig
+00002510: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00002520: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00002530: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00002540: 696c 6c3d 2223 3138 3138 3138 2220 783d  ill="#181818" x=
+00002550: 2237 3139 2e38 2220 793d 2231 2e35 2220  "719.8" y="1.5" 
+00002560: 7769 6474 683d 2235 3937 2e38 2220 6865  width="597.8" he
+00002570: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00002580: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00002590: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000025a0: 2066 696c 6c3d 2223 3138 3138 3138 2220   fill="#181818" 
+000025b0: 783d 2231 3331 372e 3622 2079 3d22 312e  x="1317.6" y="1.
+000025c0: 3522 2077 6964 7468 3d22 3531 322e 3422  5" width="512.4"
+000025d0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+000025e0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+000025f0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00002600: 6563 7420 6669 6c6c 3d22 2331 3831 3831  ect fill="#18181
+00002610: 3822 2078 3d22 3138 3330 2220 793d 2231  8" x="1830" y="1
+00002620: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+00002630: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00002640: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00002650: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00002660: 6563 7420 6669 6c6c 3d22 2331 3831 3831  ect fill="#18181
+00002670: 3822 2078 3d22 3138 3432 2e32 2220 793d  8" x="1842.2" y=
+00002680: 2231 2e35 2220 7769 6474 683d 2230 2220  "1.5" width="0" 
+00002690: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000026a0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000026b0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000026c0: 6374 2066 696c 6c3d 2223 3138 3138 3138  ct fill="#181818
+000026d0: 2220 783d 2231 3834 322e 3222 2079 3d22  " x="1842.2" y="
+000026e0: 312e 3522 2077 6964 7468 3d22 3937 2e36  1.5" width="97.6
+000026f0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00002700: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00002710: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00002720: 7265 6374 2066 696c 6c3d 2223 3138 3138  rect fill="#1818
+00002730: 3138 2220 783d 2231 3933 392e 3822 2079  18" x="1939.8" y
+00002740: 3d22 312e 3522 2077 6964 7468 3d22 3132  ="1.5" width="12
+00002750: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00002760: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00002770: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00002780: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
+00002790: 3239 3266 2220 783d 2230 2220 793d 2232  292f" x="0" y="2
+000027a0: 352e 3922 2077 6964 7468 3d22 3336 2e36  5.9" width="36.6
+000027b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000027c0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000027d0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000027e0: 7265 6374 2066 696c 6c3d 2223 6665 6136  rect fill="#fea6
+000027f0: 3262 2220 783d 2233 362e 3622 2079 3d22  2b" x="36.6" y="
+00002800: 3235 2e39 2220 7769 6474 683d 2233 3636  25.9" width="366
+00002810: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00002820: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00002830: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00002840: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
+00002850: 3266 2220 783d 2234 3032 2e36 2220 793d  2f" x="402.6" y=
+00002860: 2232 352e 3922 2077 6964 7468 3d22 3438  "25.9" width="48
+00002870: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
+00002880: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00002890: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000028a0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+000028b0: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
+000028c0: 793d 2232 352e 3922 2077 6964 7468 3d22  y="25.9" width="
+000028d0: 3134 3736 2e32 2220 6865 6967 6874 3d22  1476.2" height="
+000028e0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000028f0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00002900: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00002910: 2223 3233 3536 3862 2220 783d 2231 3932  "#23568b" x="192
+00002920: 372e 3622 2079 3d22 3235 2e39 2220 7769  7.6" y="25.9" wi
+00002930: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+00002940: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002950: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002960: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002970: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+00002980: 3022 2079 3d22 3530 2e33 2220 7769 6474  0" y="50.3" widt
+00002990: 683d 2234 382e 3822 2068 6569 6768 743d  h="48.8" height=
+000029a0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000029b0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000029c0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+000029d0: 3d22 2332 3432 3932 6622 2078 3d22 3438  ="#24292f" x="48
+000029e0: 2e38 2220 793d 2235 302e 3322 2077 6964  .8" y="50.3" wid
+000029f0: 7468 3d22 3336 2e36 2220 6865 6967 6874  th="36.6" height
+00002a00: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00002a10: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00002a20: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00002a30: 6c3d 2223 3234 3239 3266 2220 783d 2238  l="#24292f" x="8
+00002a40: 352e 3422 2079 3d22 3530 2e33 2220 7769  5.4" y="50.3" wi
+00002a50: 6474 683d 2238 352e 3422 2068 6569 6768  dth="85.4" heigh
+00002a60: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002a70: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002a80: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002a90: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+00002aa0: 3137 302e 3822 2079 3d22 3530 2e33 2220  170.8" y="50.3" 
+00002ab0: 7769 6474 683d 2232 3830 2e36 2220 6865  width="280.6" he
+00002ac0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00002ad0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00002ae0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00002af0: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00002b00: 783d 2234 3531 2e34 2220 793d 2235 302e  x="451.4" y="50.
+00002b10: 3322 2077 6964 7468 3d22 3132 2e32 2220  3" width="12.2" 
+00002b20: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00002b30: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00002b40: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00002b50: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00002b60: 2220 783d 2234 3633 2e36 2220 793d 2235  " x="463.6" y="5
+00002b70: 302e 3322 2077 6964 7468 3d22 3132 2e32  0.3" width="12.2
+00002b80: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00002b90: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00002ba0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00002bb0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+00002bc0: 3064 2220 783d 2234 3735 2e38 2220 793d  0d" x="475.8" y=
+00002bd0: 2235 302e 3322 2077 6964 7468 3d22 3637  "50.3" width="67
+00002be0: 3122 2068 6569 6768 743d 2232 342e 3635  1" height="24.65
+00002bf0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00002c00: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00002c10: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00002c20: 6430 6422 2078 3d22 3131 3436 2e38 2220  d0d" x="1146.8" 
+00002c30: 793d 2235 302e 3322 2077 6964 7468 3d22  y="50.3" width="
+00002c40: 3733 2e32 2220 6865 6967 6874 3d22 3234  73.2" height="24
+00002c50: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00002c60: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00002c70: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00002c80: 3064 3064 3064 2220 783d 2231 3232 3022  0d0d0d" x="1220"
+00002c90: 2079 3d22 3530 2e33 2220 7769 6474 683d   y="50.3" width=
+00002ca0: 2236 3833 2e32 2220 6865 6967 6874 3d22  "683.2" height="
+00002cb0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00002cc0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00002cd0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00002ce0: 2223 3064 3064 3064 2220 783d 2231 3930  "#0d0d0d" x="190
+00002cf0: 332e 3222 2079 3d22 3530 2e33 2220 7769  3.2" y="50.3" wi
+00002d00: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00002d10: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002d20: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002d30: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002d40: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00002d50: 3139 3135 2e34 2220 793d 2235 302e 3322  1915.4" y="50.3"
+00002d60: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00002d70: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00002d80: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00002d90: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00002da0: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00002db0: 783d 2231 3932 372e 3622 2079 3d22 3530  x="1927.6" y="50
+00002dc0: 2e33 2220 7769 6474 683d 2232 342e 3422  .3" width="24.4"
+00002dd0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00002de0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00002df0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00002e00: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
+00002e10: 6622 2078 3d22 3022 2079 3d22 3734 2e37  f" x="0" y="74.7
+00002e20: 2220 7769 6474 683d 2234 382e 3822 2068  " width="48.8" h
+00002e30: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00002e40: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00002e50: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00002e60: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+00002e70: 2078 3d22 3438 2e38 2220 793d 2237 342e   x="48.8" y="74.
+00002e80: 3722 2077 6964 7468 3d22 3336 2e36 2220  7" width="36.6" 
+00002e90: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00002ea0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00002eb0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00002ec0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+00002ed0: 2220 783d 2238 352e 3422 2079 3d22 3734  " x="85.4" y="74
+00002ee0: 2e37 2220 7769 6474 683d 2237 332e 3222  .7" width="73.2"
+00002ef0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00002f00: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00002f10: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00002f20: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
+00002f30: 6622 2078 3d22 3135 382e 3622 2079 3d22  f" x="158.6" y="
+00002f40: 3734 2e37 2220 7769 6474 683d 2232 3932  74.7" width="292
+00002f50: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
+00002f60: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00002f70: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00002f80: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00002f90: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
+00002fa0: 793d 2237 342e 3722 2077 6964 7468 3d22  y="74.7" width="
+00002fb0: 3134 3736 2e32 2220 6865 6967 6874 3d22  1476.2" height="
+00002fc0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00002fd0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00002fe0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00002ff0: 2223 3233 3536 3862 2220 783d 2231 3932  "#23568b" x="192
+00003000: 372e 3622 2079 3d22 3734 2e37 2220 7769  7.6" y="74.7" wi
+00003010: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+00003020: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00003030: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00003040: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003050: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+00003060: 3022 2079 3d22 3939 2e31 2220 7769 6474  0" y="99.1" widt
+00003070: 683d 2234 382e 3822 2068 6569 6768 743d  h="48.8" height=
+00003080: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00003090: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000030a0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+000030b0: 3d22 2332 3432 3932 6622 2078 3d22 3438  ="#24292f" x="48
+000030c0: 2e38 2220 793d 2239 392e 3122 2077 6964  .8" y="99.1" wid
+000030d0: 7468 3d22 3336 2e36 2220 6865 6967 6874  th="36.6" height
+000030e0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000030f0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00003100: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00003110: 6c3d 2223 3234 3239 3266 2220 783d 2238  l="#24292f" x="8
+00003120: 352e 3422 2079 3d22 3939 2e31 2220 7769  5.4" y="99.1" wi
+00003130: 6474 683d 2234 382e 3822 2068 6569 6768  dth="48.8" heigh
+00003140: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00003150: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00003160: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003170: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+00003180: 3133 342e 3222 2079 3d22 3939 2e31 2220  134.2" y="99.1" 
+00003190: 7769 6474 683d 2233 3137 2e32 2220 6865  width="317.2" he
+000031a0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000031b0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000031c0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000031d0: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+000031e0: 783d 2234 3531 2e34 2220 793d 2239 392e  x="451.4" y="99.
+000031f0: 3122 2077 6964 7468 3d22 3134 3736 2e32  1" width="1476.2
+00003200: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00003210: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00003220: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00003230: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00003240: 3862 2220 783d 2231 3932 372e 3622 2079  8b" x="1927.6" y
+00003250: 3d22 3939 2e31 2220 7769 6474 683d 2232  ="99.1" width="2
+00003260: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+00003270: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00003280: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00003290: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+000032a0: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
+000032b0: 3132 332e 3522 2077 6964 7468 3d22 3438  123.5" width="48
+000032c0: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
+000032d0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000032e0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000032f0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
+00003300: 3239 3266 2220 783d 2234 382e 3822 2079  292f" x="48.8" y
+00003310: 3d22 3132 332e 3522 2077 6964 7468 3d22  ="123.5" width="
+00003320: 3336 2e36 2220 6865 6967 6874 3d22 3234  36.6" height="24
+00003330: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00003340: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00003350: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00003360: 3234 3239 3266 2220 783d 2238 352e 3422  24292f" x="85.4"
+00003370: 2079 3d22 3132 332e 3522 2077 6964 7468   y="123.5" width
+00003380: 3d22 3134 362e 3422 2068 6569 6768 743d  ="146.4" height=
+00003390: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000033a0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000033b0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+000033c0: 3d22 2332 3432 3932 6622 2078 3d22 3233  ="#24292f" x="23
+000033d0: 312e 3822 2079 3d22 3132 332e 3522 2077  1.8" y="123.5" w
+000033e0: 6964 7468 3d22 3231 392e 3622 2068 6569  idth="219.6" hei
+000033f0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00003400: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00003410: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00003420: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
+00003430: 3d22 3435 312e 3422 2079 3d22 3132 332e  ="451.4" y="123.
+00003440: 3522 2077 6964 7468 3d22 3134 3736 2e32  5" width="1476.2
+00003450: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00003460: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00003470: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00003480: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00003490: 3862 2220 783d 2231 3932 372e 3622 2079  8b" x="1927.6" y
+000034a0: 3d22 3132 332e 3522 2077 6964 7468 3d22  ="123.5" width="
+000034b0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
+000034c0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+000034d0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+000034e0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+000034f0: 3234 3239 3266 2220 783d 2230 2220 793d  24292f" x="0" y=
+00003500: 2231 3437 2e39 2220 7769 6474 683d 2234  "147.9" width="4
+00003510: 382e 3822 2068 6569 6768 743d 2232 342e  8.8" height="24.
+00003520: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00003530: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00003540: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00003550: 3432 3932 6622 2078 3d22 3438 2e38 2220  4292f" x="48.8" 
+00003560: 793d 2231 3437 2e39 2220 7769 6474 683d  y="147.9" width=
+00003570: 2233 362e 3622 2068 6569 6768 743d 2232  "36.6" height="2
+00003580: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00003590: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+000035a0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000035b0: 2332 3432 3932 6622 2078 3d22 3835 2e34  #24292f" x="85.4
+000035c0: 2220 793d 2231 3437 2e39 2220 7769 6474  " y="147.9" widt
+000035d0: 683d 2236 3122 2068 6569 6768 743d 2232  h="61" height="2
+000035e0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+000035f0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00003600: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00003610: 2332 3432 3932 6622 2078 3d22 3134 362e  #24292f" x="146.
+00003620: 3422 2079 3d22 3134 372e 3922 2077 6964  4" y="147.9" wid
+00003630: 7468 3d22 3330 3522 2068 6569 6768 743d  th="305" height=
+00003640: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00003650: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00003660: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00003670: 3d22 2330 6430 6430 6422 2078 3d22 3435  ="#0d0d0d" x="45
+00003680: 312e 3422 2079 3d22 3134 372e 3922 2077  1.4" y="147.9" w
+00003690: 6964 7468 3d22 3336 2e36 2220 6865 6967  idth="36.6" heig
+000036a0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+000036b0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000036c0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000036d0: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+000036e0: 2234 3838 2220 793d 2231 3437 2e39 2220  "488" y="147.9" 
+000036f0: 7769 6474 683d 2231 3730 2e38 2220 6865  width="170.8" he
+00003700: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00003710: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00003720: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00003730: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00003740: 783d 2236 3538 2e38 2220 793d 2231 3437  x="658.8" y="147
+00003750: 2e39 2220 7769 6474 683d 2231 322e 3222  .9" width="12.2"
+00003760: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00003770: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00003780: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00003790: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
+000037a0: 6422 2078 3d22 3637 3122 2079 3d22 3134  d" x="671" y="14
+000037b0: 372e 3922 2077 6964 7468 3d22 3336 2e36  7.9" width="36.6
+000037c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000037d0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000037e0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000037f0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+00003800: 3064 2220 783d 2237 3037 2e36 2220 793d  0d" x="707.6" y=
+00003810: 2231 3437 2e39 2220 7769 6474 683d 2234  "147.9" width="4
+00003820: 382e 3822 2068 6569 6768 743d 2232 342e  8.8" height="24.
+00003830: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00003840: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00003850: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00003860: 6430 6430 6422 2078 3d22 3735 362e 3422  d0d0d" x="756.4"
+00003870: 2079 3d22 3134 372e 3922 2077 6964 7468   y="147.9" width
+00003880: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00003890: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000038a0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000038b0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000038c0: 2223 3064 3064 3064 2220 783d 2237 3638  "#0d0d0d" x="768
+000038d0: 2e36 2220 793d 2231 3437 2e39 2220 7769  .6" y="147.9" wi
+000038e0: 6474 683d 2233 362e 3622 2068 6569 6768  dth="36.6" heigh
+000038f0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00003900: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00003910: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003920: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00003930: 3830 352e 3222 2079 3d22 3134 372e 3922  805.2" y="147.9"
+00003940: 2077 6964 7468 3d22 3137 302e 3822 2068   width="170.8" h
+00003950: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00003960: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00003970: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00003980: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
+00003990: 2078 3d22 3937 3622 2079 3d22 3134 372e   x="976" y="147.
+000039a0: 3922 2077 6964 7468 3d22 3132 2e32 2220  9" width="12.2" 
+000039b0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000039c0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000039d0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000039e0: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+000039f0: 2220 783d 2239 3838 2e32 2220 793d 2231  " x="988.2" y="1
+00003a00: 3437 2e39 2220 7769 6474 683d 2233 362e  47.9" width="36.
+00003a10: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+00003a20: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00003a30: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00003a40: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00003a50: 6430 6422 2078 3d22 3130 3234 2e38 2220  d0d" x="1024.8" 
+00003a60: 793d 2231 3437 2e39 2220 7769 6474 683d  y="147.9" width=
+00003a70: 2231 3730 2e38 2220 6865 6967 6874 3d22  "170.8" height="
+00003a80: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00003a90: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00003aa0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00003ab0: 2223 3064 3064 3064 2220 783d 2231 3139  "#0d0d0d" x="119
+00003ac0: 352e 3622 2079 3d22 3134 372e 3922 2077  5.6" y="147.9" w
+00003ad0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00003ae0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00003af0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00003b00: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00003b10: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+00003b20: 2231 3230 372e 3822 2079 3d22 3134 372e  "1207.8" y="147.
+00003b30: 3922 2077 6964 7468 3d22 3132 2e32 2220  9" width="12.2" 
+00003b40: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00003b50: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00003b60: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00003b70: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00003b80: 2220 783d 2231 3232 3022 2079 3d22 3134  " x="1220" y="14
+00003b90: 372e 3922 2077 6964 7468 3d22 3132 2e32  7.9" width="12.2
+00003ba0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00003bb0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00003bc0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00003bd0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+00003be0: 3064 2220 783d 2231 3233 322e 3222 2079  0d" x="1232.2" y
+00003bf0: 3d22 3134 372e 3922 2077 6964 7468 3d22  ="147.9" width="
+00003c00: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00003c10: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00003c20: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00003c30: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00003c40: 3064 3064 3064 2220 783d 2231 3234 342e  0d0d0d" x="1244.
+00003c50: 3422 2079 3d22 3134 372e 3922 2077 6964  4" y="147.9" wid
+00003c60: 7468 3d22 3638 332e 3222 2068 6569 6768  th="683.2" heigh
+00003c70: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00003c80: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00003c90: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003ca0: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
+00003cb0: 3139 3237 2e36 2220 793d 2231 3437 2e39  1927.6" y="147.9
+00003cc0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+00003cd0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00003ce0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00003cf0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00003d00: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+00003d10: 2078 3d22 3022 2079 3d22 3137 322e 3322   x="0" y="172.3"
+00003d20: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
+00003d30: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00003d40: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00003d50: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00003d60: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00003d70: 783d 2234 382e 3822 2079 3d22 3137 322e  x="48.8" y="172.
+00003d80: 3322 2077 6964 7468 3d22 3336 2e36 2220  3" width="36.6" 
+00003d90: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00003da0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00003db0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00003dc0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+00003dd0: 2220 783d 2238 352e 3422 2079 3d22 3137  " x="85.4" y="17
+00003de0: 322e 3322 2077 6964 7468 3d22 3132 3222  2.3" width="122"
+00003df0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00003e00: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00003e10: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00003e20: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
+00003e30: 6622 2078 3d22 3230 372e 3422 2079 3d22  f" x="207.4" y="
+00003e40: 3137 322e 3322 2077 6964 7468 3d22 3234  172.3" width="24
+00003e50: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+00003e60: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00003e70: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00003e80: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00003e90: 6430 6422 2078 3d22 3435 312e 3422 2079  d0d" x="451.4" y
+00003ea0: 3d22 3137 322e 3322 2077 6964 7468 3d22  ="172.3" width="
+00003eb0: 3134 3736 2e32 2220 6865 6967 6874 3d22  1476.2" height="
+00003ec0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00003ed0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00003ee0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00003ef0: 2223 3233 3536 3862 2220 783d 2231 3932  "#23568b" x="192
+00003f00: 372e 3622 2079 3d22 3137 322e 3322 2077  7.6" y="172.3" w
+00003f10: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
+00003f20: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00003f30: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00003f40: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00003f50: 696c 6c3d 2223 3234 3239 3266 2220 783d  ill="#24292f" x=
+00003f60: 2230 2220 793d 2231 3936 2e37 2220 7769  "0" y="196.7" wi
+00003f70: 6474 683d 2234 382e 3822 2068 6569 6768  dth="48.8" heigh
+00003f80: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00003f90: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00003fa0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003fb0: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+00003fc0: 3438 2e38 2220 793d 2231 3936 2e37 2220  48.8" y="196.7" 
+00003fd0: 7769 6474 683d 2233 362e 3622 2068 6569  width="36.6" hei
+00003fe0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00003ff0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00004000: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00004010: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
+00004020: 3d22 3835 2e34 2220 793d 2231 3936 2e37  ="85.4" y="196.7
+00004030: 2220 7769 6474 683d 2232 3830 2e36 2220  " width="280.6" 
+00004040: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00004050: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00004060: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00004070: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+00004080: 2220 783d 2233 3636 2220 793d 2231 3936  " x="366" y="196
+00004090: 2e37 2220 7769 6474 683d 2238 352e 3422  .7" width="85.4"
+000040a0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+000040b0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+000040c0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+000040d0: 6563 7420 6669 6c6c 3d22 2334 6234 6535  ect fill="#4b4e5
+000040e0: 3522 2078 3d22 3435 312e 3422 2079 3d22  5" x="451.4" y="
+000040f0: 3139 362e 3722 2077 6964 7468 3d22 3733  196.7" width="73
+00004100: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00004110: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00004120: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004130: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00004140: 3064 3064 2220 783d 2235 3234 2e36 2220  0d0d" x="524.6" 
+00004150: 793d 2231 3936 2e37 2220 7769 6474 683d  y="196.7" width=
+00004160: 2238 3431 2e38 2220 6865 6967 6874 3d22  "841.8" height="
+00004170: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004180: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004190: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000041a0: 2223 3064 3064 3064 2220 783d 2231 3336  "#0d0d0d" x="136
+000041b0: 362e 3422 2079 3d22 3139 362e 3722 2077  6.4" y="196.7" w
+000041c0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+000041d0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+000041e0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000041f0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00004200: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+00004210: 2231 3337 382e 3622 2079 3d22 3139 362e  "1378.6" y="196.
+00004220: 3722 2077 6964 7468 3d22 3532 342e 3622  7" width="524.6"
+00004230: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00004240: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00004250: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00004260: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
+00004270: 6422 2078 3d22 3139 3033 2e32 2220 793d  d" x="1903.2" y=
+00004280: 2231 3936 2e37 2220 7769 6474 683d 2232  "196.7" width="2
+00004290: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+000042a0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000042b0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000042c0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+000042d0: 3335 3638 6222 2078 3d22 3139 3237 2e36  3568b" x="1927.6
+000042e0: 2220 793d 2231 3936 2e37 2220 7769 6474  " y="196.7" widt
+000042f0: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
+00004300: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00004310: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00004320: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00004330: 3d22 2332 3432 3932 6622 2078 3d22 3022  ="#24292f" x="0"
+00004340: 2079 3d22 3232 312e 3122 2077 6964 7468   y="221.1" width
+00004350: 3d22 3438 2e38 2220 6865 6967 6874 3d22  ="48.8" height="
+00004360: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004370: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004380: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004390: 2223 3234 3239 3266 2220 783d 2234 382e  "#24292f" x="48.
+000043a0: 3822 2079 3d22 3232 312e 3122 2077 6964  8" y="221.1" wid
+000043b0: 7468 3d22 3336 2e36 2220 6865 6967 6874  th="36.6" height
+000043c0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000043d0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000043e0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000043f0: 6c3d 2223 3234 3239 3266 2220 783d 2238  l="#24292f" x="8
+00004400: 352e 3422 2079 3d22 3232 312e 3122 2077  5.4" y="221.1" w
+00004410: 6964 7468 3d22 3135 382e 3622 2068 6569  idth="158.6" hei
+00004420: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00004430: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00004440: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00004450: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
+00004460: 3d22 3234 3422 2079 3d22 3232 312e 3122  ="244" y="221.1"
+00004470: 2077 6964 7468 3d22 3230 372e 3422 2068   width="207.4" h
+00004480: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00004490: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+000044a0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+000044b0: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
+000044c0: 2078 3d22 3435 312e 3422 2079 3d22 3232   x="451.4" y="22
+000044d0: 312e 3122 2077 6964 7468 3d22 3436 332e  1.1" width="463.
+000044e0: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+000044f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00004500: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00004510: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00004520: 6430 6422 2078 3d22 3931 3522 2079 3d22  d0d" x="915" y="
+00004530: 3232 312e 3122 2077 6964 7468 3d22 3132  221.1" width="12
+00004540: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00004550: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00004560: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004570: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00004580: 3064 3064 2220 783d 2239 3237 2e32 2220  0d0d" x="927.2" 
+00004590: 793d 2232 3231 2e31 2220 7769 6474 683d  y="221.1" width=
+000045a0: 2234 3735 2e38 2220 6865 6967 6874 3d22  "475.8" height="
+000045b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000045c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000045d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000045e0: 2223 3064 3064 3064 2220 783d 2231 3430  "#0d0d0d" x="140
+000045f0: 3322 2079 3d22 3232 312e 3122 2077 6964  3" y="221.1" wid
+00004600: 7468 3d22 3532 342e 3622 2068 6569 6768  th="524.6" heigh
+00004610: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00004620: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00004630: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00004640: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
+00004650: 3139 3237 2e36 2220 793d 2232 3231 2e31  1927.6" y="221.1
+00004660: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+00004670: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00004680: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00004690: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+000046a0: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+000046b0: 2078 3d22 3022 2079 3d22 3234 352e 3522   x="0" y="245.5"
+000046c0: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
+000046d0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000046e0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000046f0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004700: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00004710: 783d 2234 382e 3822 2079 3d22 3234 352e  x="48.8" y="245.
+00004720: 3522 2077 6964 7468 3d22 3336 2e36 2220  5" width="36.6" 
+00004730: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00004740: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00004750: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00004760: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+00004770: 2220 783d 2238 352e 3422 2079 3d22 3234  " x="85.4" y="24
+00004780: 352e 3522 2077 6964 7468 3d22 3835 2e34  5.5" width="85.4
+00004790: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000047a0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000047b0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000047c0: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
+000047d0: 3266 2220 783d 2231 3730 2e38 2220 793d  2f" x="170.8" y=
+000047e0: 2232 3435 2e35 2220 7769 6474 683d 2232  "245.5" width="2
+000047f0: 3830 2e36 2220 6865 6967 6874 3d22 3234  80.6" height="24
+00004800: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00004810: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00004820: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00004830: 3064 3064 3064 2220 783d 2234 3531 2e34  0d0d0d" x="451.4
+00004840: 2220 793d 2232 3435 2e35 2220 7769 6474  " y="245.5" widt
+00004850: 683d 2231 3437 362e 3222 2068 6569 6768  h="1476.2" heigh
+00004860: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00004870: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00004880: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00004890: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
+000048a0: 3139 3237 2e36 2220 793d 2232 3435 2e35  1927.6" y="245.5
+000048b0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+000048c0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+000048d0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+000048e0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+000048f0: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+00004900: 2078 3d22 3022 2079 3d22 3236 392e 3922   x="0" y="269.9"
+00004910: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
+00004920: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00004930: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004940: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004950: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00004960: 783d 2234 382e 3822 2079 3d22 3236 392e  x="48.8" y="269.
+00004970: 3922 2077 6964 7468 3d22 3336 2e36 2220  9" width="36.6" 
+00004980: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00004990: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000049a0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000049b0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+000049c0: 2220 783d 2238 352e 3422 2079 3d22 3236  " x="85.4" y="26
+000049d0: 392e 3922 2077 6964 7468 3d22 3733 2e32  9.9" width="73.2
+000049e0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000049f0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00004a00: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00004a10: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
+00004a20: 3266 2220 783d 2231 3538 2e36 2220 793d  2f" x="158.6" y=
+00004a30: 2232 3639 2e39 2220 7769 6474 683d 2236  "269.9" width="6
+00004a40: 3122 2068 6569 6768 743d 2232 342e 3635  1" height="24.65
+00004a50: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00004a60: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00004a70: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
+00004a80: 3932 6622 2078 3d22 3231 392e 3622 2079  92f" x="219.6" y
+00004a90: 3d22 3236 392e 3922 2077 6964 7468 3d22  ="269.9" width="
+00004aa0: 3233 312e 3822 2068 6569 6768 743d 2232  231.8" height="2
+00004ab0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00004ac0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00004ad0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00004ae0: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
+00004af0: 3422 2079 3d22 3236 392e 3922 2077 6964  4" y="269.9" wid
+00004b00: 7468 3d22 3134 3736 2e32 2220 6865 6967  th="1476.2" heig
+00004b10: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00004b20: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00004b30: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00004b40: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00004b50: 2231 3932 372e 3622 2079 3d22 3236 392e  "1927.6" y="269.
+00004b60: 3922 2077 6964 7468 3d22 3234 2e34 2220  9" width="24.4" 
+00004b70: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00004b80: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00004b90: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00004ba0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+00004bb0: 2220 783d 2230 2220 793d 2232 3934 2e33  " x="0" y="294.3
+00004bc0: 2220 7769 6474 683d 2234 382e 3822 2068  " width="48.8" h
+00004bd0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00004be0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00004bf0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00004c00: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+00004c10: 2078 3d22 3438 2e38 2220 793d 2232 3934   x="48.8" y="294
+00004c20: 2e33 2220 7769 6474 683d 2233 362e 3622  .3" width="36.6"
+00004c30: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00004c40: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00004c50: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00004c60: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
+00004c70: 6622 2078 3d22 3835 2e34 2220 793d 2232  f" x="85.4" y="2
+00004c80: 3934 2e33 2220 7769 6474 683d 2231 3039  94.3" width="109
+00004c90: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
+00004ca0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00004cb0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004cc0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
+00004cd0: 3239 3266 2220 783d 2231 3935 2e32 2220  292f" x="195.2" 
+00004ce0: 793d 2232 3934 2e33 2220 7769 6474 683d  y="294.3" width=
+00004cf0: 2236 3122 2068 6569 6768 743d 2232 342e  "61" height="24.
+00004d00: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00004d10: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00004d20: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00004d30: 3432 3932 6622 2078 3d22 3235 362e 3222  4292f" x="256.2"
+00004d40: 2079 3d22 3239 342e 3322 2077 6964 7468   y="294.3" width
+00004d50: 3d22 3139 352e 3222 2068 6569 6768 743d  ="195.2" height=
+00004d60: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00004d70: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00004d80: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00004d90: 3d22 2330 6430 6430 6422 2078 3d22 3435  ="#0d0d0d" x="45
+00004da0: 312e 3422 2079 3d22 3239 342e 3322 2077  1.4" y="294.3" w
+00004db0: 6964 7468 3d22 3134 3736 2e32 2220 6865  idth="1476.2" he
+00004dc0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00004dd0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004de0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004df0: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00004e00: 783d 2231 3932 372e 3622 2079 3d22 3239  x="1927.6" y="29
+00004e10: 342e 3322 2077 6964 7468 3d22 3234 2e34  4.3" width="24.4
+00004e20: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00004e30: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00004e40: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00004e50: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
+00004e60: 3266 2220 783d 2230 2220 793d 2233 3138  2f" x="0" y="318
+00004e70: 2e37 2220 7769 6474 683d 2234 382e 3822  .7" width="48.8"
+00004e80: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00004e90: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00004ea0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00004eb0: 6563 7420 6669 6c6c 3d22 2332 3432 3932  ect fill="#24292
+00004ec0: 6622 2078 3d22 3438 2e38 2220 793d 2233  f" x="48.8" y="3
+00004ed0: 3138 2e37 2220 7769 6474 683d 2233 362e  18.7" width="36.
+00004ee0: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+00004ef0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00004f00: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00004f10: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
+00004f20: 3932 6622 2078 3d22 3835 2e34 2220 793d  92f" x="85.4" y=
+00004f30: 2233 3138 2e37 2220 7769 6474 683d 2237  "318.7" width="7
+00004f40: 332e 3222 2068 6569 6768 743d 2232 342e  3.2" height="24.
+00004f50: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00004f60: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00004f70: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00004f80: 3432 3932 6622 2078 3d22 3135 382e 3622  4292f" x="158.6"
+00004f90: 2079 3d22 3331 382e 3722 2077 6964 7468   y="318.7" width
+00004fa0: 3d22 3336 2e36 2220 6865 6967 6874 3d22  ="36.6" height="
+00004fb0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004fc0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004fd0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004fe0: 2223 3234 3239 3266 2220 783d 2231 3935  "#24292f" x="195
+00004ff0: 2e32 2220 793d 2233 3138 2e37 2220 7769  .2" y="318.7" wi
+00005000: 6474 683d 2232 3536 2e32 2220 6865 6967  dth="256.2" heig
+00005010: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00005020: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00005030: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00005040: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+00005050: 2234 3531 2e34 2220 793d 2233 3138 2e37  "451.4" y="318.7
+00005060: 2220 7769 6474 683d 2231 3437 362e 3222  " width="1476.2"
+00005070: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00005080: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00005090: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+000050a0: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
+000050b0: 6222 2078 3d22 3139 3237 2e36 2220 793d  b" x="1927.6" y=
+000050c0: 2233 3138 2e37 2220 7769 6474 683d 2232  "318.7" width="2
+000050d0: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+000050e0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000050f0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00005100: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00005110: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
+00005120: 3334 332e 3122 2077 6964 7468 3d22 3435  343.1" width="45
+00005130: 312e 3422 2068 6569 6768 743d 2232 342e  1.4" height="24.
+00005140: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00005150: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00005160: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00005170: 6430 6430 6422 2078 3d22 3435 312e 3422  d0d0d" x="451.4"
+00005180: 2079 3d22 3334 332e 3122 2077 6964 7468   y="343.1" width
+00005190: 3d22 3022 2068 6569 6768 743d 2232 342e  ="0" height="24.
+000051a0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000051b0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000051c0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+000051d0: 6430 6430 6422 2078 3d22 3435 312e 3422  d0d0d" x="451.4"
+000051e0: 2079 3d22 3334 332e 3122 2077 6964 7468   y="343.1" width
+000051f0: 3d22 3134 3736 2e32 2220 6865 6967 6874  ="1476.2" height
+00005200: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005210: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005220: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005230: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
+00005240: 3932 372e 3622 2079 3d22 3334 332e 3122  927.6" y="343.1"
+00005250: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+00005260: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005270: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005280: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005290: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+000052a0: 783d 2230 2220 793d 2233 3637 2e35 2220  x="0" y="367.5" 
+000052b0: 7769 6474 683d 2234 3531 2e34 2220 6865  width="451.4" he
+000052c0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000052d0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000052e0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000052f0: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00005300: 783d 2234 3531 2e34 2220 793d 2233 3637  x="451.4" y="367
+00005310: 2e35 2220 7769 6474 683d 2236 3538 2e38  .5" width="658.8
+00005320: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00005330: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00005340: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00005350: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+00005360: 3064 2220 783d 2231 3131 302e 3222 2079  0d" x="1110.2" y
+00005370: 3d22 3336 372e 3522 2077 6964 7468 3d22  ="367.5" width="
+00005380: 3134 362e 3422 2068 6569 6768 743d 2232  146.4" height="2
+00005390: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+000053a0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+000053b0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000053c0: 2330 6430 6430 6422 2078 3d22 3132 3536  #0d0d0d" x="1256
+000053d0: 2e36 2220 793d 2233 3637 2e35 2220 7769  .6" y="367.5" wi
+000053e0: 6474 683d 2236 3731 2220 6865 6967 6874  dth="671" height
+000053f0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005400: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005410: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005420: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
+00005430: 3932 372e 3622 2079 3d22 3336 372e 3522  927.6" y="367.5"
+00005440: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+00005450: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005460: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005470: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005480: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00005490: 783d 2230 2220 793d 2233 3931 2e39 2220  x="0" y="391.9" 
+000054a0: 7769 6474 683d 2234 3531 2e34 2220 6865  width="451.4" he
+000054b0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000054c0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000054d0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000054e0: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+000054f0: 783d 2234 3531 2e34 2220 793d 2233 3931  x="451.4" y="391
+00005500: 2e39 2220 7769 6474 683d 2231 3437 362e  .9" width="1476.
+00005510: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00005520: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00005530: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00005540: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
+00005550: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
+00005560: 793d 2233 3931 2e39 2220 7769 6474 683d  y="391.9" width=
+00005570: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00005580: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00005590: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+000055a0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000055b0: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
+000055c0: 3d22 3431 362e 3322 2077 6964 7468 3d22  ="416.3" width="
+000055d0: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
+000055e0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+000055f0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00005600: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00005610: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
+00005620: 3422 2079 3d22 3431 362e 3322 2077 6964  4" y="416.3" wid
+00005630: 7468 3d22 3335 332e 3822 2068 6569 6768  th="353.8" heigh
+00005640: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00005650: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00005660: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00005670: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00005680: 3830 352e 3222 2079 3d22 3431 362e 3322  805.2" y="416.3"
+00005690: 2077 6964 7468 3d22 3438 2e38 2220 6865   width="48.8" he
+000056a0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000056b0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000056c0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000056d0: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+000056e0: 783d 2238 3534 2220 793d 2234 3136 2e33  x="854" y="416.3
+000056f0: 2220 7769 6474 683d 2232 3037 2e34 2220  " width="207.4" 
+00005700: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00005710: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00005720: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00005730: 6374 2066 696c 6c3d 2223 3462 3465 3535  ct fill="#4b4e55
+00005740: 2220 783d 2231 3036 312e 3422 2079 3d22  " x="1061.4" y="
+00005750: 3431 362e 3322 2077 6964 7468 3d22 3438  416.3" width="48
+00005760: 2e38 2220 6865 6967 6874 3d22 3234 2e36  .8" height="24.6
+00005770: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00005780: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00005790: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+000057a0: 3064 3064 2220 783d 2231 3131 302e 3222  0d0d" x="1110.2"
+000057b0: 2079 3d22 3431 362e 3322 2077 6964 7468   y="416.3" width
+000057c0: 3d22 3239 322e 3822 2068 6569 6768 743d  ="292.8" height=
+000057d0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000057e0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000057f0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00005800: 3d22 2330 6430 6430 6422 2078 3d22 3134  ="#0d0d0d" x="14
+00005810: 3033 2220 793d 2234 3136 2e33 2220 7769  03" y="416.3" wi
+00005820: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00005830: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00005840: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00005850: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00005860: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00005870: 3134 3135 2e32 2220 793d 2234 3136 2e33  1415.2" y="416.3
+00005880: 2220 7769 6474 683d 2235 3132 2e34 2220  " width="512.4" 
+00005890: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000058a0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000058b0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000058c0: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+000058d0: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+000058e0: 3431 362e 3322 2077 6964 7468 3d22 3234  416.3" width="24
+000058f0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00005900: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00005910: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00005920: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
+00005930: 3239 3266 2220 783d 2230 2220 793d 2234  292f" x="0" y="4
+00005940: 3430 2e37 2220 7769 6474 683d 2234 3531  40.7" width="451
+00005950: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00005960: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00005970: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00005980: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00005990: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
+000059a0: 793d 2234 3430 2e37 2220 7769 6474 683d  y="440.7" width=
+000059b0: 2234 3237 2220 6865 6967 6874 3d22 3234  "427" height="24
+000059c0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+000059d0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+000059e0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+000059f0: 3462 3465 3535 2220 783d 2238 3738 2e34  4b4e55" x="878.4
+00005a00: 2220 793d 2234 3430 2e37 2220 7769 6474  " y="440.7" widt
+00005a10: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
+00005a20: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00005a30: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00005a40: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00005a50: 3d22 2330 6430 6430 6422 2078 3d22 3931  ="#0d0d0d" x="91
+00005a60: 3522 2079 3d22 3434 302e 3722 2077 6964  5" y="440.7" wid
+00005a70: 7468 3d22 3238 302e 3622 2068 6569 6768  th="280.6" heigh
+00005a80: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00005a90: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00005aa0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00005ab0: 6c6c 3d22 2334 6234 6535 3522 2078 3d22  ll="#4b4e55" x="
+00005ac0: 3131 3935 2e36 2220 793d 2234 3430 2e37  1195.6" y="440.7
+00005ad0: 2220 7769 6474 683d 2234 382e 3822 2068  " width="48.8" h
+00005ae0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00005af0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00005b00: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00005b10: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
+00005b20: 2078 3d22 3132 3434 2e34 2220 793d 2234   x="1244.4" y="4
+00005b30: 3430 2e37 2220 7769 6474 683d 2231 322e  40.7" width="12.
+00005b40: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00005b50: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00005b60: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00005b70: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00005b80: 6430 6422 2078 3d22 3132 3536 2e36 2220  d0d" x="1256.6" 
+00005b90: 793d 2234 3430 2e37 2220 7769 6474 683d  y="440.7" width=
+00005ba0: 2236 3122 2068 6569 6768 743d 2232 342e  "61" height="24.
+00005bb0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00005bc0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00005bd0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2334  /><rect fill="#4
+00005be0: 6234 6535 3522 2078 3d22 3133 3137 2e36  b4e55" x="1317.6
+00005bf0: 2220 793d 2234 3430 2e37 2220 7769 6474  " y="440.7" widt
+00005c00: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
+00005c10: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00005c20: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00005c30: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00005c40: 3d22 2330 6430 6430 6422 2078 3d22 3133  ="#0d0d0d" x="13
+00005c50: 3534 2e32 2220 793d 2234 3430 2e37 2220  54.2" y="440.7" 
+00005c60: 7769 6474 683d 2232 3638 2e34 2220 6865  width="268.4" he
+00005c70: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005c80: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005c90: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005ca0: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00005cb0: 783d 2231 3632 322e 3622 2079 3d22 3434  x="1622.6" y="44
+00005cc0: 302e 3722 2077 6964 7468 3d22 3330 3522  0.7" width="305"
+00005cd0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00005ce0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00005cf0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00005d00: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
+00005d10: 6222 2078 3d22 3139 3237 2e36 2220 793d  b" x="1927.6" y=
+00005d20: 2234 3430 2e37 2220 7769 6474 683d 2232  "440.7" width="2
+00005d30: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+00005d40: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00005d50: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00005d60: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00005d70: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
+00005d80: 3436 352e 3122 2077 6964 7468 3d22 3435  465.1" width="45
+00005d90: 312e 3422 2068 6569 6768 743d 2232 342e  1.4" height="24.
+00005da0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00005db0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00005dc0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00005dd0: 6430 6430 6422 2078 3d22 3435 312e 3422  d0d0d" x="451.4"
+00005de0: 2079 3d22 3436 352e 3122 2077 6964 7468   y="465.1" width
+00005df0: 3d22 3134 3736 2e32 2220 6865 6967 6874  ="1476.2" height
+00005e00: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005e10: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005e20: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005e30: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
+00005e40: 3932 372e 3622 2079 3d22 3436 352e 3122  927.6" y="465.1"
+00005e50: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+00005e60: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005e70: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005e80: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005e90: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00005ea0: 783d 2230 2220 793d 2234 3839 2e35 2220  x="0" y="489.5" 
+00005eb0: 7769 6474 683d 2234 3531 2e34 2220 6865  width="451.4" he
+00005ec0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005ed0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005ee0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005ef0: 2066 696c 6c3d 2223 3237 3238 3232 2220   fill="#272822" 
+00005f00: 783d 2234 3531 2e34 2220 793d 2234 3839  x="451.4" y="489
+00005f10: 2e35 2220 7769 6474 683d 2231 3437 362e  .5" width="1476.
+00005f20: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00005f30: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00005f40: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00005f50: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
+00005f60: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
+00005f70: 793d 2234 3839 2e35 2220 7769 6474 683d  y="489.5" width=
+00005f80: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00005f90: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00005fa0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00005fb0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00005fc0: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
+00005fd0: 3d22 3531 332e 3922 2077 6964 7468 3d22  ="513.9" width="
+00005fe0: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
+00005ff0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00006000: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00006010: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00006020: 2332 3732 3832 3222 2078 3d22 3435 312e  #272822" x="451.
+00006030: 3422 2079 3d22 3531 332e 3922 2077 6964  4" y="513.9" wid
+00006040: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00006050: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00006060: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00006070: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00006080: 6c3d 2223 3237 3238 3232 2220 783d 2234  l="#272822" x="4
+00006090: 3633 2e36 2220 793d 2235 3133 2e39 2220  63.6" y="513.9" 
+000060a0: 7769 6474 683d 2234 382e 3822 2068 6569  width="48.8" hei
+000060b0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+000060c0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+000060d0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+000060e0: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
+000060f0: 3d22 3531 322e 3422 2079 3d22 3531 332e  ="512.4" y="513.
+00006100: 3922 2077 6964 7468 3d22 3132 2e32 2220  9" width="12.2" 
+00006110: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006120: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006130: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006140: 6374 2066 696c 6c3d 2223 3237 3238 3232  ct fill="#272822
+00006150: 2220 783d 2235 3234 2e36 2220 793d 2235  " x="524.6" y="5
+00006160: 3133 2e39 2220 7769 6474 683d 2238 352e  13.9" width="85.
+00006170: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+00006180: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00006190: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000061a0: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
+000061b0: 3832 3222 2078 3d22 3631 3022 2079 3d22  822" x="610" y="
+000061c0: 3531 332e 3922 2077 6964 7468 3d22 3132  513.9" width="12
+000061d0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000061e0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000061f0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00006200: 3e3c 7265 6374 2066 696c 6c3d 2223 3237  ><rect fill="#27
+00006210: 3238 3232 2220 783d 2236 3232 2e32 2220  2822" x="622.2" 
+00006220: 793d 2235 3133 2e39 2220 7769 6474 683d  y="513.9" width=
+00006230: 2237 332e 3222 2068 6569 6768 743d 2232  "73.2" height="2
+00006240: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00006250: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00006260: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00006270: 2332 3732 3832 3222 2078 3d22 3639 352e  #272822" x="695.
+00006280: 3422 2079 3d22 3531 332e 3922 2077 6964  4" y="513.9" wid
+00006290: 7468 3d22 3132 3230 2220 6865 6967 6874  th="1220" height
+000062a0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000062b0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000062c0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000062d0: 6c3d 2223 3237 3238 3232 2220 783d 2231  l="#272822" x="1
+000062e0: 3931 352e 3422 2079 3d22 3531 332e 3922  915.4" y="513.9"
+000062f0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00006300: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00006310: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00006320: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00006330: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00006340: 783d 2231 3932 372e 3622 2079 3d22 3531  x="1927.6" y="51
+00006350: 332e 3922 2077 6964 7468 3d22 3234 2e34  3.9" width="24.4
+00006360: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00006370: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00006380: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00006390: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
+000063a0: 3266 2220 783d 2230 2220 793d 2235 3338  2f" x="0" y="538
+000063b0: 2e33 2220 7769 6474 683d 2234 3531 2e34  .3" width="451.4
+000063c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000063d0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000063e0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000063f0: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
+00006400: 3232 2220 783d 2234 3531 2e34 2220 793d  22" x="451.4" y=
+00006410: 2235 3338 2e33 2220 7769 6474 683d 2231  "538.3" width="1
+00006420: 3437 362e 3222 2068 6569 6768 743d 2232  476.2" height="2
+00006430: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00006440: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00006450: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00006460: 2332 3335 3638 6222 2078 3d22 3139 3237  #23568b" x="1927
+00006470: 2e36 2220 793d 2235 3338 2e33 2220 7769  .6" y="538.3" wi
+00006480: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+00006490: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000064a0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000064b0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+000064c0: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+000064d0: 3022 2079 3d22 3536 322e 3722 2077 6964  0" y="562.7" wid
+000064e0: 7468 3d22 3435 312e 3422 2068 6569 6768  th="451.4" heigh
+000064f0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00006500: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00006510: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00006520: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00006530: 3435 312e 3422 2079 3d22 3536 322e 3722  451.4" y="562.7"
+00006540: 2077 6964 7468 3d22 3134 3736 2e32 2220   width="1476.2" 
+00006550: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006560: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006570: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006580: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+00006590: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+000065a0: 3536 322e 3722 2077 6964 7468 3d22 3234  562.7" width="24
+000065b0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+000065c0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000065d0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000065e0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
+000065f0: 3239 3266 2220 783d 2230 2220 793d 2235  292f" x="0" y="5
+00006600: 3837 2e31 2220 7769 6474 683d 2234 3531  87.1" width="451
+00006610: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00006620: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00006630: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00006640: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00006650: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
+00006660: 793d 2235 3837 2e31 2220 7769 6474 683d  y="587.1" width=
+00006670: 2230 2220 6865 6967 6874 3d22 3234 2e36  "0" height="24.6
+00006680: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00006690: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000066a0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+000066b0: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
+000066c0: 793d 2235 3837 2e31 2220 7769 6474 683d  y="587.1" width=
+000066d0: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
+000066e0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000066f0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00006700: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00006710: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
+00006720: 3237 2e36 2220 793d 2235 3837 2e31 2220  27.6" y="587.1" 
+00006730: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
+00006740: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00006750: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00006760: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00006770: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
+00006780: 3d22 3022 2079 3d22 3631 312e 3522 2077  ="0" y="611.5" w
+00006790: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
+000067a0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+000067b0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+000067c0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+000067d0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
+000067e0: 3d22 3435 312e 3422 2079 3d22 3631 312e  ="451.4" y="611.
+000067f0: 3522 2077 6964 7468 3d22 3632 322e 3222  5" width="622.2"
+00006800: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00006810: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00006820: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00006830: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
+00006840: 6422 2078 3d22 3130 3733 2e36 2220 793d  d" x="1073.6" y=
+00006850: 2236 3131 2e35 2220 7769 6474 683d 2232  "611.5" width="2
+00006860: 3139 2e36 2220 6865 6967 6874 3d22 3234  19.6" height="24
+00006870: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00006880: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00006890: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+000068a0: 3064 3064 3064 2220 783d 2231 3239 332e  0d0d0d" x="1293.
+000068b0: 3222 2079 3d22 3631 312e 3522 2077 6964  2" y="611.5" wid
+000068c0: 7468 3d22 3633 342e 3422 2068 6569 6768  th="634.4" heigh
+000068d0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000068e0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000068f0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00006900: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
+00006910: 3139 3237 2e36 2220 793d 2236 3131 2e35  1927.6" y="611.5
+00006920: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+00006930: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00006940: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00006950: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00006960: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+00006970: 2078 3d22 3022 2079 3d22 3633 352e 3922   x="0" y="635.9"
+00006980: 2077 6964 7468 3d22 3435 312e 3422 2068   width="451.4" h
+00006990: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+000069a0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+000069b0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+000069c0: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
+000069d0: 2078 3d22 3435 312e 3422 2079 3d22 3633   x="451.4" y="63
+000069e0: 352e 3922 2077 6964 7468 3d22 3134 3736  5.9" width="1476
+000069f0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00006a00: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00006a10: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00006a20: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00006a30: 3536 3862 2220 783d 2231 3932 372e 3622  568b" x="1927.6"
+00006a40: 2079 3d22 3633 352e 3922 2077 6964 7468   y="635.9" width
+00006a50: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00006a60: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00006a70: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00006a80: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00006a90: 2223 3234 3239 3266 2220 783d 2230 2220  "#24292f" x="0" 
+00006aa0: 793d 2236 3630 2e33 2220 7769 6474 683d  y="660.3" width=
+00006ab0: 2234 3531 2e34 2220 6865 6967 6874 3d22  "451.4" height="
+00006ac0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00006ad0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00006ae0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00006af0: 2223 3064 3064 3064 2220 783d 2234 3531  "#0d0d0d" x="451
+00006b00: 2e34 2220 793d 2236 3630 2e33 2220 7769  .4" y="660.3" wi
+00006b10: 6474 683d 2233 3035 2220 6865 6967 6874  dth="305" height
+00006b20: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00006b30: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00006b40: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00006b50: 6c3d 2223 3462 3465 3535 2220 783d 2237  l="#4b4e55" x="7
+00006b60: 3536 2e34 2220 793d 2236 3630 2e33 2220  56.4" y="660.3" 
+00006b70: 7769 6474 683d 2237 332e 3222 2068 6569  width="73.2" hei
+00006b80: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00006b90: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00006ba0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00006bb0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
+00006bc0: 3d22 3832 392e 3622 2079 3d22 3636 302e  ="829.6" y="660.
+00006bd0: 3322 2077 6964 7468 3d22 3739 3322 2068  3" width="793" h
+00006be0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00006bf0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00006c00: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00006c10: 7420 6669 6c6c 3d22 2334 6234 6535 3522  t fill="#4b4e55"
+00006c20: 2078 3d22 3136 3232 2e36 2220 793d 2236   x="1622.6" y="6
+00006c30: 3630 2e33 2220 7769 6474 683d 2237 332e  60.3" width="73.
+00006c40: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00006c50: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00006c60: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00006c70: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00006c80: 6430 6422 2078 3d22 3136 3935 2e38 2220  d0d" x="1695.8" 
+00006c90: 793d 2236 3630 2e33 2220 7769 6474 683d  y="660.3" width=
+00006ca0: 2238 352e 3422 2068 6569 6768 743d 2232  "85.4" height="2
+00006cb0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00006cc0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00006cd0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00006ce0: 2330 6430 6430 6422 2078 3d22 3137 3831  #0d0d0d" x="1781
+00006cf0: 2e32 2220 793d 2236 3630 2e33 2220 7769  .2" y="660.3" wi
+00006d00: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00006d10: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00006d20: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00006d30: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00006d40: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00006d50: 3137 3933 2e34 2220 793d 2236 3630 2e33  1793.4" y="660.3
+00006d60: 2220 7769 6474 683d 2231 3039 2e38 2220  " width="109.8" 
+00006d70: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006d80: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006d90: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006da0: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00006db0: 2220 783d 2231 3930 332e 3222 2079 3d22  " x="1903.2" y="
+00006dc0: 3636 302e 3322 2077 6964 7468 3d22 3234  660.3" width="24
+00006dd0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00006de0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00006df0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00006e00: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00006e10: 3536 3862 2220 783d 2231 3932 372e 3622  568b" x="1927.6"
+00006e20: 2079 3d22 3636 302e 3322 2077 6964 7468   y="660.3" width
+00006e30: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00006e40: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00006e50: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00006e60: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00006e70: 2223 3234 3239 3266 2220 783d 2230 2220  "#24292f" x="0" 
+00006e80: 793d 2236 3834 2e37 2220 7769 6474 683d  y="684.7" width=
+00006e90: 2234 3531 2e34 2220 6865 6967 6874 3d22  "451.4" height="
+00006ea0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00006eb0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00006ec0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00006ed0: 2223 3064 3064 3064 2220 783d 2234 3531  "#0d0d0d" x="451
+00006ee0: 2e34 2220 793d 2236 3834 2e37 2220 7769  .4" y="684.7" wi
+00006ef0: 6474 683d 2236 3935 2e34 2220 6865 6967  dth="695.4" heig
+00006f00: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00006f10: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00006f20: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00006f30: 696c 6c3d 2223 3462 3465 3535 2220 783d  ill="#4b4e55" x=
+00006f40: 2231 3134 362e 3822 2079 3d22 3638 342e  "1146.8" y="684.
+00006f50: 3722 2077 6964 7468 3d22 3835 2e34 2220  7" width="85.4" 
+00006f60: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006f70: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006f80: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006f90: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00006fa0: 2220 783d 2231 3233 322e 3222 2079 3d22  " x="1232.2" y="
+00006fb0: 3638 342e 3722 2077 6964 7468 3d22 3330  684.7" width="30
+00006fc0: 3522 2068 6569 6768 743d 2232 342e 3635  5" height="24.65
+00006fd0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00006fe0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00006ff0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00007000: 6430 6422 2078 3d22 3135 3337 2e32 2220  d0d" x="1537.2" 
+00007010: 793d 2236 3834 2e37 2220 7769 6474 683d  y="684.7" width=
+00007020: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
+00007030: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007040: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007050: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007060: 2330 6430 6430 6422 2078 3d22 3135 3439  #0d0d0d" x="1549
+00007070: 2e34 2220 793d 2236 3834 2e37 2220 7769  .4" y="684.7" wi
+00007080: 6474 683d 2232 3434 2220 6865 6967 6874  dth="244" height
+00007090: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000070a0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000070b0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000070c0: 6c3d 2223 3462 3465 3535 2220 783d 2231  l="#4b4e55" x="1
+000070d0: 3739 332e 3422 2079 3d22 3638 342e 3722  793.4" y="684.7"
+000070e0: 2077 6964 7468 3d22 3336 2e36 2220 6865   width="36.6" he
+000070f0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00007100: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00007110: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00007120: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00007130: 783d 2231 3833 3022 2079 3d22 3638 342e  x="1830" y="684.
+00007140: 3722 2077 6964 7468 3d22 3835 2e34 2220  7" width="85.4" 
+00007150: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00007160: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00007170: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00007180: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00007190: 2220 783d 2231 3931 352e 3422 2079 3d22  " x="1915.4" y="
+000071a0: 3638 342e 3722 2077 6964 7468 3d22 3132  684.7" width="12
+000071b0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000071c0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000071d0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000071e0: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+000071f0: 3536 3862 2220 783d 2231 3932 372e 3622  568b" x="1927.6"
+00007200: 2079 3d22 3638 342e 3722 2077 6964 7468   y="684.7" width
+00007210: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00007220: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00007230: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00007240: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00007250: 2223 3234 3239 3266 2220 783d 2230 2220  "#24292f" x="0" 
+00007260: 793d 2237 3039 2e31 2220 7769 6474 683d  y="709.1" width=
+00007270: 2234 3531 2e34 2220 6865 6967 6874 3d22  "451.4" height="
+00007280: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00007290: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000072a0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000072b0: 2223 3064 3064 3064 2220 783d 2234 3531  "#0d0d0d" x="451
+000072c0: 2e34 2220 793d 2237 3039 2e31 2220 7769  .4" y="709.1" wi
+000072d0: 6474 683d 2232 3638 2e34 2220 6865 6967  dth="268.4" heig
+000072e0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+000072f0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00007300: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00007310: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+00007320: 2237 3139 2e38 2220 793d 2237 3039 2e31  "719.8" y="709.1
+00007330: 2220 7769 6474 683d 2231 3230 372e 3822  " width="1207.8"
+00007340: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00007350: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00007360: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00007370: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
+00007380: 6222 2078 3d22 3139 3237 2e36 2220 793d  b" x="1927.6" y=
+00007390: 2237 3039 2e31 2220 7769 6474 683d 2232  "709.1" width="2
+000073a0: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+000073b0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000073c0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000073d0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+000073e0: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
+000073f0: 3733 332e 3522 2077 6964 7468 3d22 3435  733.5" width="45
+00007400: 312e 3422 2068 6569 6768 743d 2232 342e  1.4" height="24.
+00007410: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00007420: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00007430: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00007440: 6430 6430 6422 2078 3d22 3435 312e 3422  d0d0d" x="451.4"
+00007450: 2079 3d22 3733 332e 3522 2077 6964 7468   y="733.5" width
+00007460: 3d22 3134 3736 2e32 2220 6865 6967 6874  ="1476.2" height
+00007470: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00007480: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00007490: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000074a0: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
+000074b0: 3932 372e 3622 2079 3d22 3733 332e 3522  927.6" y="733.5"
+000074c0: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+000074d0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000074e0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000074f0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00007500: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00007510: 783d 2230 2220 793d 2237 3537 2e39 2220  x="0" y="757.9" 
+00007520: 7769 6474 683d 2234 3531 2e34 2220 6865  width="451.4" he
+00007530: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00007540: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00007550: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00007560: 2066 696c 6c3d 2223 3237 3238 3232 2220   fill="#272822" 
+00007570: 783d 2234 3531 2e34 2220 793d 2237 3537  x="451.4" y="757
+00007580: 2e39 2220 7769 6474 683d 2231 3437 362e  .9" width="1476.
+00007590: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+000075a0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+000075b0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000075c0: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
+000075d0: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
+000075e0: 793d 2237 3537 2e39 2220 7769 6474 683d  y="757.9" width=
+000075f0: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00007600: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007610: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007620: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007630: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
+00007640: 3d22 3738 322e 3322 2077 6964 7468 3d22  ="782.3" width="
+00007650: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
+00007660: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007670: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007680: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007690: 2332 3732 3832 3222 2078 3d22 3435 312e  #272822" x="451.
+000076a0: 3422 2079 3d22 3738 322e 3322 2077 6964  4" y="782.3" wid
+000076b0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+000076c0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000076d0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000076e0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000076f0: 6c3d 2223 3237 3238 3232 2220 783d 2234  l="#272822" x="4
+00007700: 3633 2e36 2220 793d 2237 3832 2e33 2220  63.6" y="782.3" 
+00007710: 7769 6474 683d 2234 382e 3822 2068 6569  width="48.8" hei
+00007720: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00007730: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00007740: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00007750: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
+00007760: 3d22 3531 322e 3422 2079 3d22 3738 322e  ="512.4" y="782.
+00007770: 3322 2077 6964 7468 3d22 3132 2e32 2220  3" width="12.2" 
+00007780: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00007790: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000077a0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000077b0: 6374 2066 696c 6c3d 2223 3237 3238 3232  ct fill="#272822
+000077c0: 2220 783d 2235 3234 2e36 2220 793d 2237  " x="524.6" y="7
+000077d0: 3832 2e33 2220 7769 6474 683d 2238 352e  82.3" width="85.
+000077e0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+000077f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00007800: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00007810: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
+00007820: 3832 3222 2078 3d22 3631 3022 2079 3d22  822" x="610" y="
+00007830: 3738 322e 3322 2077 6964 7468 3d22 3132  782.3" width="12
+00007840: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00007850: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00007860: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00007870: 3e3c 7265 6374 2066 696c 6c3d 2223 3237  ><rect fill="#27
+00007880: 3238 3232 2220 783d 2236 3232 2e32 2220  2822" x="622.2" 
+00007890: 793d 2237 3832 2e33 2220 7769 6474 683d  y="782.3" width=
+000078a0: 2231 3538 2e36 2220 6865 6967 6874 3d22  "158.6" height="
+000078b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000078c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000078d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000078e0: 2223 3237 3238 3232 2220 783d 2237 3830  "#272822" x="780
+000078f0: 2e38 2220 793d 2237 3832 2e33 2220 7769  .8" y="782.3" wi
+00007900: 6474 683d 2231 3133 342e 3622 2068 6569  dth="1134.6" hei
+00007910: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00007920: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00007930: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00007940: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
+00007950: 3d22 3139 3135 2e34 2220 793d 2237 3832  ="1915.4" y="782
+00007960: 2e33 2220 7769 6474 683d 2231 322e 3222  .3" width="12.2"
+00007970: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00007980: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00007990: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+000079a0: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
+000079b0: 6222 2078 3d22 3139 3237 2e36 2220 793d  b" x="1927.6" y=
+000079c0: 2237 3832 2e33 2220 7769 6474 683d 2232  "782.3" width="2
+000079d0: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+000079e0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000079f0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00007a00: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00007a10: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
+00007a20: 3830 362e 3722 2077 6964 7468 3d22 3435  806.7" width="45
+00007a30: 312e 3422 2068 6569 6768 743d 2232 342e  1.4" height="24.
+00007a40: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00007a50: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00007a60: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00007a70: 3732 3832 3222 2078 3d22 3435 312e 3422  72822" x="451.4"
+00007a80: 2079 3d22 3830 362e 3722 2077 6964 7468   y="806.7" width
+00007a90: 3d22 3134 3736 2e32 2220 6865 6967 6874  ="1476.2" height
+00007aa0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00007ab0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00007ac0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00007ad0: 6c3d 2223 3233 3536 3862 2220 783d 2231  l="#23568b" x="1
+00007ae0: 3932 372e 3622 2079 3d22 3830 362e 3722  927.6" y="806.7"
+00007af0: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+00007b00: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00007b10: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00007b20: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00007b30: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
+00007b40: 783d 2230 2220 793d 2238 3331 2e31 2220  x="0" y="831.1" 
+00007b50: 7769 6474 683d 2234 3531 2e34 2220 6865  width="451.4" he
+00007b60: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00007b70: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00007b80: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00007b90: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00007ba0: 783d 2234 3531 2e34 2220 793d 2238 3331  x="451.4" y="831
+00007bb0: 2e31 2220 7769 6474 683d 2231 3437 362e  .1" width="1476.
+00007bc0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00007bd0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00007be0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00007bf0: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
+00007c00: 3638 6222 2078 3d22 3139 3237 2e36 2220  68b" x="1927.6" 
+00007c10: 793d 2238 3331 2e31 2220 7769 6474 683d  y="831.1" width=
+00007c20: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00007c30: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007c40: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007c50: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007c60: 2332 3432 3932 6622 2078 3d22 3022 2079  #24292f" x="0" y
+00007c70: 3d22 3835 352e 3522 2077 6964 7468 3d22  ="855.5" width="
+00007c80: 3435 312e 3422 2068 6569 6768 743d 2232  451.4" height="2
+00007c90: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007ca0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007cb0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007cc0: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
+00007cd0: 3422 2079 3d22 3835 352e 3522 2077 6964  4" y="855.5" wid
+00007ce0: 7468 3d22 3022 2068 6569 6768 743d 2232  th="0" height="2
+00007cf0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007d00: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007d10: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007d20: 2330 6430 6430 6422 2078 3d22 3435 312e  #0d0d0d" x="451.
+00007d30: 3422 2079 3d22 3835 352e 3522 2077 6964  4" y="855.5" wid
+00007d40: 7468 3d22 3134 3736 2e32 2220 6865 6967  th="1476.2" heig
+00007d50: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00007d60: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00007d70: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00007d80: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00007d90: 2231 3932 372e 3622 2079 3d22 3835 352e  "1927.6" y="855.
+00007da0: 3522 2077 6964 7468 3d22 3234 2e34 2220  5" width="24.4" 
+00007db0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00007dc0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00007dd0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00007de0: 6374 2066 696c 6c3d 2223 3234 3239 3266  ct fill="#24292f
+00007df0: 2220 783d 2230 2220 793d 2238 3739 2e39  " x="0" y="879.9
+00007e00: 2220 7769 6474 683d 2234 3531 2e34 2220  " width="451.4" 
+00007e10: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00007e20: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00007e30: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00007e40: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00007e50: 2220 783d 2234 3531 2e34 2220 793d 2238  " x="451.4" y="8
+00007e60: 3739 2e39 2220 7769 6474 683d 2237 3037  79.9" width="707
+00007e70: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
+00007e80: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00007e90: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00007ea0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00007eb0: 3064 3064 2220 783d 2231 3135 3922 2079  0d0d" x="1159" y
+00007ec0: 3d22 3837 392e 3922 2077 6964 7468 3d22  ="879.9" width="
+00007ed0: 3631 2220 6865 6967 6874 3d22 3234 2e36  61" height="24.6
+00007ee0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00007ef0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00007f00: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00007f10: 3064 3064 2220 783d 2231 3232 3022 2079  0d0d" x="1220" y
+00007f20: 3d22 3837 392e 3922 2077 6964 7468 3d22  ="879.9" width="
+00007f30: 3730 372e 3622 2068 6569 6768 743d 2232  707.6" height="2
+00007f40: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007f50: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007f60: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007f70: 2332 3335 3638 6222 2078 3d22 3139 3237  #23568b" x="1927
+00007f80: 2e36 2220 793d 2238 3739 2e39 2220 7769  .6" y="879.9" wi
+00007f90: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+00007fa0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00007fb0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00007fc0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00007fd0: 6c6c 3d22 2332 3432 3932 6622 2078 3d22  ll="#24292f" x="
+00007fe0: 3022 2079 3d22 3930 342e 3322 2077 6964  0" y="904.3" wid
+00007ff0: 7468 3d22 3435 312e 3422 2068 6569 6768  th="451.4" heigh
+00008000: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00008010: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00008020: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00008030: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00008040: 3435 312e 3422 2079 3d22 3930 342e 3322  451.4" y="904.3"
+00008050: 2077 6964 7468 3d22 3134 3736 2e32 2220   width="1476.2" 
+00008060: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00008070: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00008080: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00008090: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+000080a0: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+000080b0: 3930 342e 3322 2077 6964 7468 3d22 3234  904.3" width="24
+000080c0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+000080d0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000080e0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000080f0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
+00008100: 3239 3266 2220 783d 2230 2220 793d 2239  292f" x="0" y="9
+00008110: 3238 2e37 2220 7769 6474 683d 2234 3531  28.7" width="451
+00008120: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00008130: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00008140: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00008150: 3e3c 7265 6374 2066 696c 6c3d 2223 3237  ><rect fill="#27
+00008160: 3238 3232 2220 783d 2234 3531 2e34 2220  2822" x="451.4" 
+00008170: 793d 2239 3238 2e37 2220 7769 6474 683d  y="928.7" width=
+00008180: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
+00008190: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000081a0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000081b0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+000081c0: 3d22 2332 3335 3638 6222 2078 3d22 3139  ="#23568b" x="19
+000081d0: 3237 2e36 2220 793d 2239 3238 2e37 2220  27.6" y="928.7" 
+000081e0: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
+000081f0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00008200: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00008210: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00008220: 6669 6c6c 3d22 2332 3432 3932 6622 2078  fill="#24292f" x
+00008230: 3d22 3022 2079 3d22 3935 332e 3122 2077  ="0" y="953.1" w
+00008240: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
+00008250: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00008260: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00008270: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00008280: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
+00008290: 3d22 3435 312e 3422 2079 3d22 3935 332e  ="451.4" y="953.
+000082a0: 3122 2077 6964 7468 3d22 3132 2e32 2220  1" width="12.2" 
+000082b0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000082c0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000082d0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000082e0: 6374 2066 696c 6c3d 2223 3237 3238 3232  ct fill="#272822
+000082f0: 2220 783d 2234 3633 2e36 2220 793d 2239  " x="463.6" y="9
+00008300: 3533 2e31 2220 7769 6474 683d 2237 332e  53.1" width="73.
+00008310: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00008320: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00008330: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00008340: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
+00008350: 3832 3222 2078 3d22 3533 362e 3822 2079  822" x="536.8" y
+00008360: 3d22 3935 332e 3122 2077 6964 7468 3d22  ="953.1" width="
+00008370: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00008380: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00008390: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+000083a0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+000083b0: 3237 3238 3232 2220 783d 2235 3439 2220  272822" x="549" 
+000083c0: 793d 2239 3533 2e31 2220 7769 6474 683d  y="953.1" width=
+000083d0: 2231 3436 2e34 2220 6865 6967 6874 3d22  "146.4" height="
+000083e0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000083f0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00008400: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00008410: 2223 3237 3238 3232 2220 783d 2236 3935  "#272822" x="695
+00008420: 2e34 2220 793d 2239 3533 2e31 2220 7769  .4" y="953.1" wi
+00008430: 6474 683d 2231 3232 3022 2068 6569 6768  dth="1220" heigh
+00008440: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00008450: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00008460: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00008470: 6c6c 3d22 2332 3732 3832 3222 2078 3d22  ll="#272822" x="
+00008480: 3139 3135 2e34 2220 793d 2239 3533 2e31  1915.4" y="953.1
+00008490: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
+000084a0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+000084b0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+000084c0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+000084d0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+000084e0: 2078 3d22 3139 3237 2e36 2220 793d 2239   x="1927.6" y="9
+000084f0: 3533 2e31 2220 7769 6474 683d 2232 342e  53.1" width="24.
+00008500: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+00008510: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00008520: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00008530: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
+00008540: 3932 6622 2078 3d22 3022 2079 3d22 3937  92f" x="0" y="97
+00008550: 372e 3522 2077 6964 7468 3d22 3435 312e  7.5" width="451.
+00008560: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+00008570: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00008580: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00008590: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
+000085a0: 3832 3222 2078 3d22 3435 312e 3422 2079  822" x="451.4" y
+000085b0: 3d22 3937 372e 3522 2077 6964 7468 3d22  ="977.5" width="
+000085c0: 3134 3736 2e32 2220 6865 6967 6874 3d22  1476.2" height="
+000085d0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000085e0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000085f0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00008600: 2223 3134 3139 3166 2220 783d 2231 3932  "#14191f" x="192
+00008610: 372e 3622 2079 3d22 3937 372e 3522 2077  7.6" y="977.5" w
+00008620: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
+00008630: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00008640: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00008650: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00008660: 696c 6c3d 2223 3234 3239 3266 2220 783d  ill="#24292f" x=
+00008670: 2230 2220 793d 2231 3030 312e 3922 2077  "0" y="1001.9" w
+00008680: 6964 7468 3d22 3435 312e 3422 2068 6569  idth="451.4" hei
 00008690: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
 000086a0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
 000086b0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000086c0: 6669 6c6c 3d22 2334 6234 6535 3522 2078  fill="#4b4e55" x
-000086d0: 3d22 3539 372e 3822 2079 3d22 3130 3236  ="597.8" y="1026
-000086e0: 2e33 2220 7769 6474 683d 2237 332e 3222  .3" width="73.2"
-000086f0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00008700: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00008710: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00008720: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00008730: 6422 2078 3d22 3637 3122 2079 3d22 3130  d" x="671" y="10
-00008740: 3236 2e33 2220 7769 6474 683d 2237 3434  26.3" width="744
-00008750: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-00008760: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00008770: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00008780: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00008790: 3064 3064 2220 783d 2231 3431 352e 3222  0d0d" x="1415.2"
-000087a0: 2079 3d22 3130 3236 2e33 2220 7769 6474   y="1026.3" widt
-000087b0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
+000086c0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
+000086d0: 3d22 3435 312e 3422 2079 3d22 3130 3031  ="451.4" y="1001
+000086e0: 2e39 2220 7769 6474 683d 2231 3437 362e  .9" width="1476.
+000086f0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00008700: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00008710: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00008720: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00008730: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
+00008740: 793d 2231 3030 312e 3922 2077 6964 7468  y="1001.9" width
+00008750: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00008760: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00008770: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00008780: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00008790: 2223 3234 3239 3266 2220 783d 2230 2220  "#24292f" x="0" 
+000087a0: 793d 2231 3032 362e 3322 2077 6964 7468  y="1026.3" width
+000087b0: 3d22 3435 312e 3422 2068 6569 6768 743d  ="451.4" height=
 000087c0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
 000087d0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
 000087e0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000087f0: 3d22 2330 6430 6430 6422 2078 3d22 3134  ="#0d0d0d" x="14
-00008800: 3237 2e34 2220 793d 2231 3032 362e 3322  27.4" y="1026.3"
-00008810: 2077 6964 7468 3d22 3530 302e 3222 2068   width="500.2" h
-00008820: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00008830: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00008840: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00008850: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00008860: 2078 3d22 3139 3237 2e36 2220 793d 2231   x="1927.6" y="1
-00008870: 3032 362e 3322 2077 6964 7468 3d22 3234  026.3" width="24
-00008880: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00008890: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000088a0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000088b0: 3e3c 7265 6374 2066 696c 6c3d 2223 3234  ><rect fill="#24
-000088c0: 3239 3266 2220 783d 2230 2220 793d 2231  292f" x="0" y="1
-000088d0: 3035 302e 3722 2077 6964 7468 3d22 3435  050.7" width="45
-000088e0: 312e 3422 2068 6569 6768 743d 2232 342e  1.4" height="24.
+000087f0: 3d22 2330 6430 6430 6422 2078 3d22 3435  ="#0d0d0d" x="45
+00008800: 312e 3422 2079 3d22 3130 3236 2e33 2220  1.4" y="1026.3" 
+00008810: 7769 6474 683d 2231 3436 2e34 2220 6865  width="146.4" he
+00008820: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00008830: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00008840: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00008850: 2066 696c 6c3d 2223 3462 3465 3535 2220   fill="#4b4e55" 
+00008860: 783d 2235 3937 2e38 2220 793d 2231 3032  x="597.8" y="102
+00008870: 362e 3322 2077 6964 7468 3d22 3733 2e32  6.3" width="73.2
+00008880: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00008890: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000088a0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000088b0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+000088c0: 3064 2220 783d 2236 3731 2220 793d 2231  0d" x="671" y="1
+000088d0: 3032 362e 3322 2077 6964 7468 3d22 3734  026.3" width="74
+000088e0: 342e 3222 2068 6569 6768 743d 2232 342e  4.2" height="24.
 000088f0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
 00008900: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
 00008910: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00008920: 6430 6430 6422 2078 3d22 3435 312e 3422  d0d0d" x="451.4"
-00008930: 2079 3d22 3130 3530 2e37 2220 7769 6474   y="1050.7" widt
-00008940: 683d 2235 3234 2e36 2220 6865 6967 6874  h="524.6" height
+00008920: 6430 6430 6422 2078 3d22 3134 3135 2e32  d0d0d" x="1415.2
+00008930: 2220 793d 2231 3032 362e 3322 2077 6964  " y="1026.3" wid
+00008940: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
 00008950: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
 00008960: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
 00008970: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00008980: 6c3d 2223 3064 3064 3064 2220 783d 2239  l="#0d0d0d" x="9
-00008990: 3736 2220 793d 2231 3035 302e 3722 2077  76" y="1050.7" w
-000089a0: 6964 7468 3d22 3935 312e 3622 2068 6569  idth="951.6" hei
-000089b0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000089c0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000089d0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000089e0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-000089f0: 3d22 3139 3237 2e36 2220 793d 2231 3035  ="1927.6" y="105
-00008a00: 302e 3722 2077 6964 7468 3d22 3234 2e34  0.7" width="24.4
-00008a10: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00008a20: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00008a30: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00008a40: 7265 6374 2066 696c 6c3d 2223 3234 3239  rect fill="#2429
-00008a50: 3266 2220 783d 2230 2220 793d 2231 3037  2f" x="0" y="107
-00008a60: 352e 3122 2077 6964 7468 3d22 3435 312e  5.1" width="451.
-00008a70: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00008a80: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00008a90: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00008aa0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00008ab0: 6430 6422 2078 3d22 3435 312e 3422 2079  d0d" x="451.4" y
-00008ac0: 3d22 3130 3735 2e31 2220 7769 6474 683d  ="1075.1" width=
-00008ad0: 2231 3437 362e 3222 2068 6569 6768 743d  "1476.2" height=
-00008ae0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00008af0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00008b00: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00008b10: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
-00008b20: 3237 2e36 2220 793d 2231 3037 352e 3122  27.6" y="1075.1"
-00008b30: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+00008980: 6c3d 2223 3064 3064 3064 2220 783d 2231  l="#0d0d0d" x="1
+00008990: 3432 372e 3422 2079 3d22 3130 3236 2e33  427.4" y="1026.3
+000089a0: 2220 7769 6474 683d 2235 3030 2e32 2220  " width="500.2" 
+000089b0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000089c0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000089d0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000089e0: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+000089f0: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+00008a00: 3130 3236 2e33 2220 7769 6474 683d 2232  1026.3" width="2
+00008a10: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+00008a20: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00008a30: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00008a40: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00008a50: 3432 3932 6622 2078 3d22 3022 2079 3d22  4292f" x="0" y="
+00008a60: 3130 3530 2e37 2220 7769 6474 683d 2234  1050.7" width="4
+00008a70: 3531 2e34 2220 6865 6967 6874 3d22 3234  51.4" height="24
+00008a80: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00008a90: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00008aa0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00008ab0: 3064 3064 3064 2220 783d 2234 3531 2e34  0d0d0d" x="451.4
+00008ac0: 2220 793d 2231 3035 302e 3722 2077 6964  " y="1050.7" wid
+00008ad0: 7468 3d22 3532 342e 3622 2068 6569 6768  th="524.6" heigh
+00008ae0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00008af0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00008b00: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00008b10: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00008b20: 3937 3622 2079 3d22 3130 3530 2e37 2220  976" y="1050.7" 
+00008b30: 7769 6474 683d 2239 3531 2e36 2220 6865  width="951.6" he
 00008b40: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
 00008b50: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
 00008b60: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00008b70: 2066 696c 6c3d 2223 3234 3239 3266 2220   fill="#24292f" 
-00008b80: 783d 2230 2220 793d 2231 3039 392e 3522  x="0" y="1099.5"
-00008b90: 2077 6964 7468 3d22 3435 312e 3422 2068   width="451.4" h
-00008ba0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00008bb0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00008bc0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00008bd0: 7420 6669 6c6c 3d22 2332 3732 3832 3222  t fill="#272822"
-00008be0: 2078 3d22 3435 312e 3422 2079 3d22 3130   x="451.4" y="10
-00008bf0: 3939 2e35 2220 7769 6474 683d 2231 3437  99.5" width="147
-00008c00: 362e 3222 2068 6569 6768 743d 2232 342e  6.2" height="24.
-00008c10: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00008c20: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00008c30: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00008c40: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
-00008c50: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
-00008c60: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
+00008b70: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00008b80: 783d 2231 3932 372e 3622 2079 3d22 3130  x="1927.6" y="10
+00008b90: 3530 2e37 2220 7769 6474 683d 2232 342e  50.7" width="24.
+00008ba0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+00008bb0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00008bc0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00008bd0: 3c72 6563 7420 6669 6c6c 3d22 2332 3432  <rect fill="#242
+00008be0: 3932 6622 2078 3d22 3022 2079 3d22 3130  92f" x="0" y="10
+00008bf0: 3735 2e31 2220 7769 6474 683d 2234 3531  75.1" width="451
+00008c00: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00008c10: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00008c20: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00008c30: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00008c40: 3064 3064 2220 783d 2234 3531 2e34 2220  0d0d" x="451.4" 
+00008c50: 793d 2231 3037 352e 3122 2077 6964 7468  y="1075.1" width
+00008c60: 3d22 3134 3736 2e32 2220 6865 6967 6874  ="1476.2" height
 00008c70: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
 00008c80: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
 00008c90: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00008ca0: 6c3d 2223 3030 3432 3935 2220 783d 2230  l="#004295" x="0
-00008cb0: 2220 793d 2231 3132 332e 3922 2077 6964  " y="1123.9" wid
-00008cc0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00008cd0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00008ce0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00008cf0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00008d00: 6c3d 2223 3030 3432 3935 2220 783d 2231  l="#004295" x="1
-00008d10: 322e 3222 2079 3d22 3131 3233 2e39 2220  2.2" y="1123.9" 
-00008d20: 7769 6474 683d 2235 3733 2e34 2220 6865  width="573.4" he
-00008d30: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00008d40: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00008d50: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00008d60: 2066 696c 6c3d 2223 3030 3432 3935 2220   fill="#004295" 
-00008d70: 783d 2235 3835 2e36 2220 793d 2231 3132  x="585.6" y="112
-00008d80: 332e 3922 2077 6964 7468 3d22 3133 3534  3.9" width="1354
-00008d90: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-00008da0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00008db0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00008dc0: 3e3c 7265 6374 2066 696c 6c3d 2223 3030  ><rect fill="#00
-00008dd0: 3432 3935 2220 783d 2231 3933 392e 3822  4295" x="1939.8"
-00008de0: 2079 3d22 3131 3233 2e39 2220 7769 6474   y="1123.9" widt
-00008df0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00008e00: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00008e10: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00008e20: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00008e30: 3d22 2330 3035 3361 6122 2078 3d22 3022  ="#0053aa" x="0"
-00008e40: 2079 3d22 3131 3438 2e33 2220 7769 6474   y="1148.3" widt
-00008e50: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
-00008e60: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00008e70: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00008e80: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00008e90: 3d22 2330 3137 3864 3422 2078 3d22 3336  ="#0178d4" x="36
-00008ea0: 2e36 2220 793d 2231 3134 382e 3322 2077  .6" y="1148.3" w
-00008eb0: 6964 7468 3d22 3733 2e32 2220 6865 6967  idth="73.2" heig
-00008ec0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00008ed0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00008ee0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00008ef0: 696c 6c3d 2223 3030 3533 6161 2220 783d  ill="#0053aa" x=
-00008f00: 2231 3039 2e38 2220 793d 2231 3134 382e  "109.8" y="1148.
-00008f10: 3322 2077 6964 7468 3d22 3336 2e36 2220  3" width="36.6" 
-00008f20: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00008f30: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00008f40: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00008f50: 6374 2066 696c 6c3d 2223 3031 3738 6434  ct fill="#0178d4
-00008f60: 2220 783d 2231 3436 2e34 2220 793d 2231  " x="146.4" y="1
-00008f70: 3134 382e 3322 2077 6964 7468 3d22 3137  148.3" width="17
-00008f80: 302e 3822 2068 6569 6768 743d 2232 342e  0.8" height="24.
-00008f90: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00008fa0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00008fb0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00008fc0: 3035 3361 6122 2078 3d22 3331 372e 3222  053aa" x="317.2"
-00008fd0: 2079 3d22 3131 3438 2e33 2220 7769 6474   y="1148.3" widt
-00008fe0: 683d 2233 362e 3622 2068 6569 6768 743d  h="36.6" height=
-00008ff0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00009000: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00009010: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00009020: 3d22 2330 3137 3864 3422 2078 3d22 3335  ="#0178d4" x="35
-00009030: 332e 3822 2079 3d22 3131 3438 2e33 2220  3.8" y="1148.3" 
-00009040: 7769 6474 683d 2231 3730 2e38 2220 6865  width="170.8" he
-00009050: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00009060: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00009070: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00009080: 2066 696c 6c3d 2223 3030 3533 6161 2220   fill="#0053aa" 
-00009090: 783d 2235 3234 2e36 2220 793d 2231 3134  x="524.6" y="114
-000090a0: 382e 3322 2077 6964 7468 3d22 3336 2e36  8.3" width="36.6
-000090b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000090c0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000090d0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000090e0: 7265 6374 2066 696c 6c3d 2223 3031 3738  rect fill="#0178
-000090f0: 6434 2220 783d 2235 3631 2e32 2220 793d  d4" x="561.2" y=
-00009100: 2231 3134 382e 3322 2077 6964 7468 3d22  "1148.3" width="
-00009110: 3235 362e 3222 2068 6569 6768 743d 2232  256.2" height="2
-00009120: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00009130: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00009140: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00009150: 2330 3035 3361 6122 2078 3d22 3831 372e  #0053aa" x="817.
-00009160: 3422 2079 3d22 3131 3438 2e33 2220 7769  4" y="1148.3" wi
-00009170: 6474 683d 2233 362e 3622 2068 6569 6768  dth="36.6" heigh
-00009180: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00009190: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000091a0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000091b0: 6c6c 3d22 2330 3137 3864 3422 2078 3d22  ll="#0178d4" x="
-000091c0: 3835 3422 2079 3d22 3131 3438 2e33 2220  854" y="1148.3" 
-000091d0: 7769 6474 683d 2232 3139 2e36 2220 6865  width="219.6" he
-000091e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-000091f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00009200: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00009210: 2066 696c 6c3d 2223 3030 3533 6161 2220   fill="#0053aa" 
-00009220: 783d 2231 3037 332e 3622 2079 3d22 3131  x="1073.6" y="11
+00008ca0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+00008cb0: 3932 372e 3622 2079 3d22 3130 3735 2e31  927.6" y="1075.1
+00008cc0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+00008cd0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00008ce0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00008cf0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00008d00: 7420 6669 6c6c 3d22 2332 3432 3932 6622  t fill="#24292f"
+00008d10: 2078 3d22 3022 2079 3d22 3130 3939 2e35   x="0" y="1099.5
+00008d20: 2220 7769 6474 683d 2234 3531 2e34 2220  " width="451.4" 
+00008d30: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00008d40: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00008d50: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00008d60: 6374 2066 696c 6c3d 2223 3237 3238 3232  ct fill="#272822
+00008d70: 2220 783d 2234 3531 2e34 2220 793d 2231  " x="451.4" y="1
+00008d80: 3039 392e 3522 2077 6964 7468 3d22 3134  099.5" width="14
+00008d90: 3736 2e32 2220 6865 6967 6874 3d22 3234  76.2" height="24
+00008da0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00008db0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00008dc0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00008dd0: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
+00008de0: 3622 2079 3d22 3130 3939 2e35 2220 7769  6" y="1099.5" wi
+00008df0: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+00008e00: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00008e10: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00008e20: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00008e30: 6c6c 3d22 2330 3034 3239 3522 2078 3d22  ll="#004295" x="
+00008e40: 3022 2079 3d22 3131 3233 2e39 2220 7769  0" y="1123.9" wi
+00008e50: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00008e60: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00008e70: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00008e80: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00008e90: 6c6c 3d22 2330 3034 3239 3522 2078 3d22  ll="#004295" x="
+00008ea0: 3132 2e32 2220 793d 2231 3132 332e 3922  12.2" y="1123.9"
+00008eb0: 2077 6964 7468 3d22 3537 332e 3422 2068   width="573.4" h
+00008ec0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00008ed0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00008ee0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00008ef0: 7420 6669 6c6c 3d22 2330 3034 3239 3522  t fill="#004295"
+00008f00: 2078 3d22 3538 352e 3622 2079 3d22 3131   x="585.6" y="11
+00008f10: 3233 2e39 2220 7769 6474 683d 2231 3335  23.9" width="135
+00008f20: 342e 3222 2068 6569 6768 743d 2232 342e  4.2" height="24.
+00008f30: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00008f40: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00008f50: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00008f60: 3034 3239 3522 2078 3d22 3139 3339 2e38  04295" x="1939.8
+00008f70: 2220 793d 2231 3132 332e 3922 2077 6964  " y="1123.9" wid
+00008f80: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00008f90: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00008fa0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00008fb0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00008fc0: 6c3d 2223 3030 3533 6161 2220 783d 2230  l="#0053aa" x="0
+00008fd0: 2220 793d 2231 3134 382e 3322 2077 6964  " y="1148.3" wid
+00008fe0: 7468 3d22 3336 2e36 2220 6865 6967 6874  th="36.6" height
+00008ff0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00009000: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00009010: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00009020: 6c3d 2223 3031 3738 6434 2220 783d 2233  l="#0178d4" x="3
+00009030: 362e 3622 2079 3d22 3131 3438 2e33 2220  6.6" y="1148.3" 
+00009040: 7769 6474 683d 2237 332e 3222 2068 6569  width="73.2" hei
+00009050: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00009060: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00009070: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00009080: 6669 6c6c 3d22 2330 3035 3361 6122 2078  fill="#0053aa" x
+00009090: 3d22 3130 392e 3822 2079 3d22 3131 3438  ="109.8" y="1148
+000090a0: 2e33 2220 7769 6474 683d 2233 362e 3622  .3" width="36.6"
+000090b0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+000090c0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+000090d0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+000090e0: 6563 7420 6669 6c6c 3d22 2330 3137 3864  ect fill="#0178d
+000090f0: 3422 2078 3d22 3134 362e 3422 2079 3d22  4" x="146.4" y="
+00009100: 3131 3438 2e33 2220 7769 6474 683d 2231  1148.3" width="1
+00009110: 3730 2e38 2220 6865 6967 6874 3d22 3234  70.8" height="24
+00009120: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00009130: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00009140: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00009150: 3030 3533 6161 2220 783d 2233 3137 2e32  0053aa" x="317.2
+00009160: 2220 793d 2231 3134 382e 3322 2077 6964  " y="1148.3" wid
+00009170: 7468 3d22 3336 2e36 2220 6865 6967 6874  th="36.6" height
+00009180: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00009190: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000091a0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000091b0: 6c3d 2223 3031 3738 6434 2220 783d 2233  l="#0178d4" x="3
+000091c0: 3533 2e38 2220 793d 2231 3134 382e 3322  53.8" y="1148.3"
+000091d0: 2077 6964 7468 3d22 3137 302e 3822 2068   width="170.8" h
+000091e0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+000091f0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00009200: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00009210: 7420 6669 6c6c 3d22 2330 3035 3361 6122  t fill="#0053aa"
+00009220: 2078 3d22 3532 342e 3622 2079 3d22 3131   x="524.6" y="11
 00009230: 3438 2e33 2220 7769 6474 683d 2233 362e  48.3" width="36.
 00009240: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
 00009250: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
 00009260: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
 00009270: 3c72 6563 7420 6669 6c6c 3d22 2330 3137  <rect fill="#017
-00009280: 3864 3422 2078 3d22 3131 3130 2e32 2220  8d4" x="1110.2" 
-00009290: 793d 2231 3134 382e 3322 2077 6964 7468  y="1148.3" width
-000092a0: 3d22 3138 3322 2068 6569 6768 743d 2232  ="183" height="2
-000092b0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000092c0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000092d0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000092e0: 2330 3137 3864 3422 2078 3d22 3132 3933  #0178d4" x="1293
-000092f0: 2e32 2220 793d 2231 3134 382e 3322 2077  .2" y="1148.3" w
-00009300: 6964 7468 3d22 3635 382e 3822 2068 6569  idth="658.8" hei
-00009310: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00009320: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00009330: 7370 4564 6765 7322 2f3e 0a20 2020 203c  spEdges"/>.    <
-00009340: 6720 636c 6173 733d 2274 6572 6d69 6e61  g class="termina
-00009350: 6c2d 3137 3234 3735 3934 3635 2d6d 6174  l-1724759465-mat
-00009360: 7269 7822 3e0a 2020 2020 3c74 6578 7420  rix">.    <text 
-00009370: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-00009380: 3137 3234 3735 3934 3635 2d72 3222 2078  1724759465-r2" x
-00009390: 3d22 3132 2e32 2220 793d 2232 3022 2074  ="12.2" y="20" t
-000093a0: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
-000093b0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-000093c0: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-000093d0: 3934 3635 2d6c 696e 652d 3029 223e e2ad  9465-line-0)">..
-000093e0: 983c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
-000093f0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-00009400: 3234 3735 3934 3635 2d72 3222 2078 3d22  24759465-r2" x="
-00009410: 3631 3022 2079 3d22 3230 2220 7465 7874  610" y="20" text
-00009420: 4c65 6e67 7468 3d22 3130 392e 3822 2063  Length="109.8" c
-00009430: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-00009440: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-00009450: 3635 2d6c 696e 652d 3029 223e 6272 6f77  65-line-0)">brow
-00009460: 7372 2623 3136 303b e280 9426 2331 3630  sr&#160;...&#160
-00009470: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-00009480: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-00009490: 3234 3735 3934 3635 2d72 3322 2078 3d22  24759465-r3" x="
-000094a0: 3731 392e 3822 2079 3d22 3230 2220 7465  719.8" y="20" te
-000094b0: 7874 4c65 6e67 7468 3d22 3539 372e 3822  xtLength="597.8"
-000094c0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-000094d0: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-000094e0: 3934 3635 2d6c 696e 652d 3029 223e 6769  9465-line-0)">gi
-000094f0: 7468 7562 3a2f 2f6a 7566 7469 6e3a 6272  thub://juftin:br
-00009500: 6f77 7372 4076 312e 362e 302f 5245 4144  owsr@v1.6.0/READ
-00009510: 4d45 2e6d 6426 2331 3630 3b5b 6d6f 6e6f  ME.md&#160;[mono
-00009520: 6b61 695d 3c2f 7465 7874 3e3c 7465 7874  kai]</text><text
-00009530: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-00009540: 2d31 3732 3437 3539 3436 352d 7231 2220  -1724759465-r1" 
-00009550: 783d 2231 3935 3222 2079 3d22 3230 2220  x="1952" y="20" 
-00009560: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-00009570: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-00009580: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-00009590: 3539 3436 352d 6c69 6e65 2d30 2922 3e0a  59465-line-0)">.
-000095a0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-000095b0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-000095c0: 3437 3539 3436 352d 7234 2220 783d 2230  4759465-r4" x="0
-000095d0: 2220 793d 2234 342e 3422 2074 6578 744c  " y="44.4" textL
-000095e0: 656e 6774 683d 2232 342e 3422 2063 6c69  ength="24.4" cli
-000095f0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-00009600: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-00009610: 2d6c 696e 652d 3129 223e f09f 9382 2623  -line-1)">....&#
-00009620: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
-00009630: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-00009640: 2d31 3732 3437 3539 3436 352d 7235 2220  -1724759465-r5" 
-00009650: 783d 2233 362e 3622 2079 3d22 3434 2e34  x="36.6" y="44.4
-00009660: 2220 7465 7874 4c65 6e67 7468 3d22 3336  " textLength="36
-00009670: 3622 2063 6c69 702d 7061 7468 3d22 7572  6" clip-path="ur
-00009680: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-00009690: 3735 3934 3635 2d6c 696e 652d 3129 223e  759465-line-1)">
-000096a0: 6769 7468 7562 3a2f 2f6a 7566 7469 6e3a  github://juftin:
-000096b0: 6272 6f77 7372 4076 312e 362e 302f 3c2f  browsr@v1.6.0/</
-000096c0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-000096d0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-000096e0: 3539 3436 352d 7236 2220 783d 2234 3531  59465-r6" x="451
-000096f0: 2e34 2220 793d 2234 342e 3422 2074 6578  .4" y="44.4" tex
-00009700: 744c 656e 6774 683d 2231 3437 362e 3222  tLength="1476.2"
-00009710: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00009720: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-00009730: 3934 3635 2d6c 696e 652d 3129 223e e294  9465-line-1)">..
-00009740: 8fe2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009750: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009760: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009770: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009780: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009790: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000097a0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-000097b0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-000097c0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000097d0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-000097e0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-000097f0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009800: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009810: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009820: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009830: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009840: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009850: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009860: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009870: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009880: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009890: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-000098a0: e294 81e2 9481 e294 933c 2f74 6578 743e  .........</text>
-000098b0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-000098c0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-000098d0: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
-000098e0: 2234 342e 3422 2074 6578 744c 656e 6774  "44.4" textLengt
-000098f0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-00009900: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-00009910: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-00009920: 652d 3129 223e 0a3c 2f74 6578 743e 3c74  e-1)">.</text><t
-00009930: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-00009940: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-00009950: 3722 2078 3d22 3022 2079 3d22 3638 2e38  7" x="0" y="68.8
-00009960: 2220 7465 7874 4c65 6e67 7468 3d22 3438  " textLength="48
-00009970: 2e38 2220 636c 6970 2d70 6174 683d 2275  .8" clip-path="u
-00009980: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-00009990: 3437 3539 3436 352d 6c69 6e65 2d32 2922  4759465-line-2)"
-000099a0: 3ee2 949c e294 80e2 9480 2623 3136 303b  >.........&#160;
-000099b0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-000099c0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-000099d0: 3437 3539 3436 352d 7234 2220 783d 2234  4759465-r4" x="4
-000099e0: 382e 3822 2079 3d22 3638 2e38 2220 7465  8.8" y="68.8" te
-000099f0: 7874 4c65 6e67 7468 3d22 3234 2e34 2220  xtLength="24.4" 
-00009a00: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00009a10: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-00009a20: 3436 352d 6c69 6e65 2d32 2922 3ef0 9f93  465-line-2)">...
-00009a30: 8126 2331 3630 3b3c 2f74 6578 743e 3c74  .&#160;</text><t
-00009a40: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-00009a50: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-00009a60: 3822 2078 3d22 3835 2e34 2220 793d 2236  8" x="85.4" y="6
-00009a70: 382e 3822 2074 6578 744c 656e 6774 683d  8.8" textLength=
-00009a80: 2238 352e 3422 2063 6c69 702d 7061 7468  "85.4" clip-path
-00009a90: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-00009aa0: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-00009ab0: 3229 223e 2e67 6974 6875 623c 2f74 6578  2)">.github</tex
-00009ac0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-00009ad0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-00009ae0: 3635 2d72 3622 2078 3d22 3435 312e 3422  65-r6" x="451.4"
-00009af0: 2079 3d22 3638 2e38 2220 7465 7874 4c65   y="68.8" textLe
-00009b00: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
-00009b10: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-00009b20: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-00009b30: 6c69 6e65 2d32 2922 3ee2 9483 3c2f 7465  line-2)">...</te
-00009b40: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-00009b50: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-00009b60: 3436 352d 7239 2220 783d 2231 3134 362e  465-r9" x="1146.
-00009b70: 3822 2079 3d22 3638 2e38 2220 7465 7874  8" y="68.8" text
-00009b80: 4c65 6e67 7468 3d22 3733 2e32 2220 636c  Length="73.2" cl
-00009b90: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-00009ba0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00009bb0: 352d 6c69 6e65 2d32 2922 3e62 726f 7773  5-line-2)">brows
-00009bc0: 723c 2f74 6578 743e 3c74 6578 7420 636c  r</text><text cl
-00009bd0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-00009be0: 3234 3735 3934 3635 2d72 3622 2078 3d22  24759465-r6" x="
-00009bf0: 3139 3135 2e34 2220 793d 2236 382e 3822  1915.4" y="68.8"
-00009c00: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
-00009c10: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
-00009c20: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-00009c30: 3735 3934 3635 2d6c 696e 652d 3229 223e  759465-line-2)">
-00009c40: e294 833c 2f74 6578 743e 3c74 6578 7420  ...</text><text 
-00009c50: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-00009c60: 3137 3234 3735 3934 3635 2d72 3122 2078  1724759465-r1" x
-00009c70: 3d22 3139 3532 2220 793d 2236 382e 3822  ="1952" y="68.8"
-00009c80: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
-00009c90: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
-00009ca0: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-00009cb0: 3735 3934 3635 2d6c 696e 652d 3229 223e  759465-line-2)">
-00009cc0: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
-00009cd0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-00009ce0: 3234 3735 3934 3635 2d72 3722 2078 3d22  24759465-r7" x="
-00009cf0: 3022 2079 3d22 3933 2e32 2220 7465 7874  0" y="93.2" text
-00009d00: 4c65 6e67 7468 3d22 3438 2e38 2220 636c  Length="48.8" cl
-00009d10: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-00009d20: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00009d30: 352d 6c69 6e65 2d33 2922 3ee2 949c e294  5-line-3)">.....
-00009d40: 80e2 9480 2623 3136 303b 3c2f 7465 7874  ....&#160;</text
-00009d50: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-00009d60: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-00009d70: 352d 7234 2220 783d 2234 382e 3822 2079  5-r4" x="48.8" y
-00009d80: 3d22 3933 2e32 2220 7465 7874 4c65 6e67  ="93.2" textLeng
-00009d90: 7468 3d22 3234 2e34 2220 636c 6970 2d70  th="24.4" clip-p
-00009da0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-00009db0: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-00009dc0: 6e65 2d33 2922 3ef0 9f93 8126 2331 3630  ne-3)">....&#160
-00009dd0: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-00009de0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-00009df0: 3234 3735 3934 3635 2d72 3130 2220 783d  24759465-r10" x=
-00009e00: 2238 352e 3422 2079 3d22 3933 2e32 2220  "85.4" y="93.2" 
-00009e10: 7465 7874 4c65 6e67 7468 3d22 3733 2e32  textLength="73.2
-00009e20: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-00009e30: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-00009e40: 3539 3436 352d 6c69 6e65 2d33 2922 3e62  59465-line-3)">b
-00009e50: 726f 7773 723c 2f74 6578 743e 3c74 6578  rowsr</text><tex
-00009e60: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-00009e70: 6c2d 3137 3234 3735 3934 3635 2d72 3622  l-1724759465-r6"
-00009e80: 2078 3d22 3435 312e 3422 2079 3d22 3933   x="451.4" y="93
-00009e90: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
-00009ea0: 3134 3736 2e32 2220 636c 6970 2d70 6174  1476.2" clip-pat
-00009eb0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-00009ec0: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-00009ed0: 2d33 2922 3ee2 9497 e294 81e2 9481 e294  -3)">...........
-00009ee0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009ef0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009f00: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009f10: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009f20: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009f30: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009f40: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009f50: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009f60: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009f70: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009f80: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009f90: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009fa0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009fb0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009fc0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00009fd0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00009fe0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00009ff0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-0000a000: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-0000a010: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-0000a020: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-0000a030: 81e2 9481 e294 81e2 9481 e294 81e2 949b  ................
-0000a040: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000a050: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000a060: 3437 3539 3436 352d 7231 2220 783d 2231  4759465-r1" x="1
-0000a070: 3935 3222 2079 3d22 3933 2e32 2220 7465  952" y="93.2" te
-0000a080: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
-0000a090: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000a0a0: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000a0b0: 3436 352d 6c69 6e65 2d33 2922 3e0a 3c2f  465-line-3)">.</
-0000a0c0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000a0d0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000a0e0: 3539 3436 352d 7237 2220 783d 2230 2220  59465-r7" x="0" 
-0000a0f0: 793d 2231 3137 2e36 2220 7465 7874 4c65  y="117.6" textLe
-0000a100: 6e67 7468 3d22 3438 2e38 2220 636c 6970  ngth="48.8" clip
-0000a110: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000a120: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000a130: 6c69 6e65 2d34 2922 3ee2 949c e294 80e2  line-4)">.......
-0000a140: 9480 2623 3136 303b 3c2f 7465 7874 3e3c  ..&#160;</text><
-0000a150: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000a160: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000a170: 7234 2220 783d 2234 382e 3822 2079 3d22  r4" x="48.8" y="
-0000a180: 3131 372e 3622 2074 6578 744c 656e 6774  117.6" textLengt
-0000a190: 683d 2232 342e 3422 2063 6c69 702d 7061  h="24.4" clip-pa
-0000a1a0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000a1b0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000a1c0: 652d 3429 223e f09f 9381 2623 3136 303b  e-4)">....&#160;
-0000a1d0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000a1e0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000a1f0: 3437 3539 3436 352d 7231 3022 2078 3d22  4759465-r10" x="
-0000a200: 3835 2e34 2220 793d 2231 3137 2e36 2220  85.4" y="117.6" 
-0000a210: 7465 7874 4c65 6e67 7468 3d22 3438 2e38  textLength="48.8
-0000a220: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000a230: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-0000a240: 3539 3436 352d 6c69 6e65 2d34 2922 3e64  59465-line-4)">d
-0000a250: 6f63 733c 2f74 6578 743e 3c74 6578 7420  ocs</text><text 
-0000a260: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000a270: 3137 3234 3735 3934 3635 2d72 3122 2078  1724759465-r1" x
-0000a280: 3d22 3139 3532 2220 793d 2231 3137 2e36  ="1952" y="117.6
-0000a290: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000a2a0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000a2b0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000a2c0: 3437 3539 3436 352d 6c69 6e65 2d34 2922  4759465-line-4)"
-0000a2d0: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
-0000a2e0: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000a2f0: 3732 3437 3539 3436 352d 7237 2220 783d  724759465-r7" x=
-0000a300: 2230 2220 793d 2231 3432 2220 7465 7874  "0" y="142" text
-0000a310: 4c65 6e67 7468 3d22 3438 2e38 2220 636c  Length="48.8" cl
-0000a320: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000a330: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000a340: 352d 6c69 6e65 2d35 2922 3ee2 949c e294  5-line-5)">.....
-0000a350: 80e2 9480 2623 3136 303b 3c2f 7465 7874  ....&#160;</text
-0000a360: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000a370: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000a380: 352d 7234 2220 783d 2234 382e 3822 2079  5-r4" x="48.8" y
-0000a390: 3d22 3134 3222 2074 6578 744c 656e 6774  ="142" textLengt
-0000a3a0: 683d 2232 342e 3422 2063 6c69 702d 7061  h="24.4" clip-pa
-0000a3b0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000a3c0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000a3d0: 652d 3529 223e f09f 9381 2623 3136 303b  e-5)">....&#160;
-0000a3e0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000a3f0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000a400: 3437 3539 3436 352d 7231 3022 2078 3d22  4759465-r10" x="
-0000a410: 3835 2e34 2220 793d 2231 3432 2220 7465  85.4" y="142" te
-0000a420: 7874 4c65 6e67 7468 3d22 3134 362e 3422  xtLength="146.4"
-0000a430: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000a440: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-0000a450: 3934 3635 2d6c 696e 652d 3529 223e 7265  9465-line-5)">re
-0000a460: 7175 6972 656d 656e 7473 3c2f 7465 7874  quirements</text
-0000a470: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000a480: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000a490: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
-0000a4a0: 3d22 3134 3222 2074 6578 744c 656e 6774  ="142" textLengt
-0000a4b0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000a4c0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000a4d0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000a4e0: 652d 3529 223e 0a3c 2f74 6578 743e 3c74  e-5)">.</text><t
-0000a4f0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000a500: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000a510: 3722 2078 3d22 3022 2079 3d22 3136 362e  7" x="0" y="166.
-0000a520: 3422 2074 6578 744c 656e 6774 683d 2234  4" textLength="4
-0000a530: 382e 3822 2063 6c69 702d 7061 7468 3d22  8.8" clip-path="
-0000a540: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000a550: 3234 3735 3934 3635 2d6c 696e 652d 3629  24759465-line-6)
-0000a560: 223e e294 9ce2 9480 e294 8026 2331 3630  ">.........&#160
+00009280: 3864 3422 2078 3d22 3536 312e 3222 2079  8d4" x="561.2" y
+00009290: 3d22 3131 3438 2e33 2220 7769 6474 683d  ="1148.3" width=
+000092a0: 2232 3536 2e32 2220 6865 6967 6874 3d22  "256.2" height="
+000092b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000092c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000092d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000092e0: 2223 3030 3533 6161 2220 783d 2238 3137  "#0053aa" x="817
+000092f0: 2e34 2220 793d 2231 3134 382e 3322 2077  .4" y="1148.3" w
+00009300: 6964 7468 3d22 3336 2e36 2220 6865 6967  idth="36.6" heig
+00009310: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00009320: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00009330: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00009340: 696c 6c3d 2223 3031 3738 6434 2220 783d  ill="#0178d4" x=
+00009350: 2238 3534 2220 793d 2231 3134 382e 3322  "854" y="1148.3"
+00009360: 2077 6964 7468 3d22 3231 392e 3622 2068   width="219.6" h
+00009370: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00009380: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00009390: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+000093a0: 7420 6669 6c6c 3d22 2330 3035 3361 6122  t fill="#0053aa"
+000093b0: 2078 3d22 3130 3733 2e36 2220 793d 2231   x="1073.6" y="1
+000093c0: 3134 382e 3322 2077 6964 7468 3d22 3336  148.3" width="36
+000093d0: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
+000093e0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000093f0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00009400: 3e3c 7265 6374 2066 696c 6c3d 2223 3031  ><rect fill="#01
+00009410: 3738 6434 2220 783d 2231 3131 302e 3222  78d4" x="1110.2"
+00009420: 2079 3d22 3131 3438 2e33 2220 7769 6474   y="1148.3" widt
+00009430: 683d 2231 3833 2220 6865 6967 6874 3d22  h="183" height="
+00009440: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00009450: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00009460: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00009470: 2223 3031 3738 6434 2220 783d 2231 3239  "#0178d4" x="129
+00009480: 332e 3222 2079 3d22 3131 3438 2e33 2220  3.2" y="1148.3" 
+00009490: 7769 6474 683d 2236 3538 2e38 2220 6865  width="658.8" he
+000094a0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000094b0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000094c0: 6973 7045 6467 6573 222f 3e0a 2020 2020  ispEdges"/>.    
+000094d0: 3c67 2063 6c61 7373 3d22 7465 726d 696e  <g class="termin
+000094e0: 616c 2d32 3136 3730 3831 3336 302d 6d61  al-2167081360-ma
+000094f0: 7472 6978 223e 0a20 2020 203c 7465 7874  trix">.    <text
+00009500: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+00009510: 2d32 3136 3730 3831 3336 302d 7232 2220  -2167081360-r2" 
+00009520: 783d 2231 322e 3222 2079 3d22 3230 2220  x="12.2" y="20" 
+00009530: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
+00009540: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+00009550: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+00009560: 3831 3336 302d 6c69 6e65 2d30 2922 3ee2  81360-line-0)">.
+00009570: ad98 3c2f 7465 7874 3e3c 7465 7874 2063  ..</text><text c
+00009580: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+00009590: 3136 3730 3831 3336 302d 7232 2220 783d  167081360-r2" x=
+000095a0: 2236 3130 2220 793d 2232 3022 2074 6578  "610" y="20" tex
+000095b0: 744c 656e 6774 683d 2231 3039 2e38 2220  tLength="109.8" 
+000095c0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+000095d0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+000095e0: 3336 302d 6c69 6e65 2d30 2922 3e62 726f  360-line-0)">bro
+000095f0: 7773 7226 2331 3630 3be2 8094 2623 3136  wsr&#160;...&#16
+00009600: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
+00009610: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+00009620: 3136 3730 3831 3336 302d 7233 2220 783d  167081360-r3" x=
+00009630: 2237 3139 2e38 2220 793d 2232 3022 2074  "719.8" y="20" t
+00009640: 6578 744c 656e 6774 683d 2235 3937 2e38  extLength="597.8
+00009650: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+00009660: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+00009670: 3831 3336 302d 6c69 6e65 2d30 2922 3e67  81360-line-0)">g
+00009680: 6974 6875 623a 2f2f 6a75 6674 696e 3a62  ithub://juftin:b
+00009690: 726f 7773 7240 7631 2e36 2e30 2f52 4541  rowsr@v1.6.0/REA
+000096a0: 444d 452e 6d64 2623 3136 303b 5b6d 6f6e  DME.md&#160;[mon
+000096b0: 6f6b 6169 5d3c 2f74 6578 743e 3c74 6578  okai]</text><tex
+000096c0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+000096d0: 6c2d 3231 3637 3038 3133 3630 2d72 3122  l-2167081360-r1"
+000096e0: 2078 3d22 3139 3532 2220 793d 2232 3022   x="1952" y="20"
+000096f0: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+00009700: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+00009710: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+00009720: 3038 3133 3630 2d6c 696e 652d 3029 223e  081360-line-0)">
+00009730: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+00009740: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+00009750: 3637 3038 3133 3630 2d72 3422 2078 3d22  67081360-r4" x="
+00009760: 3022 2079 3d22 3434 2e34 2220 7465 7874  0" y="44.4" text
+00009770: 4c65 6e67 7468 3d22 3234 2e34 2220 636c  Length="24.4" cl
+00009780: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+00009790: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+000097a0: 302d 6c69 6e65 2d31 2922 3ef0 9f93 8226  0-line-1)">....&
+000097b0: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+000097c0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+000097d0: 6c2d 3231 3637 3038 3133 3630 2d72 3522  l-2167081360-r5"
+000097e0: 2078 3d22 3336 2e36 2220 793d 2234 342e   x="36.6" y="44.
+000097f0: 3422 2074 6578 744c 656e 6774 683d 2233  4" textLength="3
+00009800: 3636 2220 636c 6970 2d70 6174 683d 2275  66" clip-path="u
+00009810: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+00009820: 3730 3831 3336 302d 6c69 6e65 2d31 2922  7081360-line-1)"
+00009830: 3e67 6974 6875 623a 2f2f 6a75 6674 696e  >github://juftin
+00009840: 3a62 726f 7773 7240 7631 2e36 2e30 2f3c  :browsr@v1.6.0/<
+00009850: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+00009860: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+00009870: 3038 3133 3630 2d72 3622 2078 3d22 3435  081360-r6" x="45
+00009880: 312e 3422 2079 3d22 3434 2e34 2220 7465  1.4" y="44.4" te
+00009890: 7874 4c65 6e67 7468 3d22 3134 3736 2e32  xtLength="1476.2
+000098a0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+000098b0: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+000098c0: 3831 3336 302d 6c69 6e65 2d31 2922 3ee2  81360-line-1)">.
+000098d0: 948f e294 81e2 9481 e294 81e2 9481 e294  ................
+000098e0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000098f0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00009900: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00009910: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00009920: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00009930: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00009940: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00009950: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00009960: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00009970: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00009980: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00009990: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000099a0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000099b0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+000099c0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000099d0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000099e0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+000099f0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00009a00: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00009a10: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00009a20: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00009a30: 81e2 9481 e294 81e2 9493 3c2f 7465 7874  ..........</text
+00009a40: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+00009a50: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+00009a60: 302d 7231 2220 783d 2231 3935 3222 2079  0-r1" x="1952" y
+00009a70: 3d22 3434 2e34 2220 7465 7874 4c65 6e67  ="44.4" textLeng
+00009a80: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+00009a90: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+00009aa0: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+00009ab0: 6e65 2d31 2922 3e0a 3c2f 7465 7874 3e3c  ne-1)">.</text><
+00009ac0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+00009ad0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+00009ae0: 7237 2220 783d 2230 2220 793d 2236 382e  r7" x="0" y="68.
+00009af0: 3822 2074 6578 744c 656e 6774 683d 2234  8" textLength="4
+00009b00: 382e 3822 2063 6c69 702d 7061 7468 3d22  8.8" clip-path="
+00009b10: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+00009b20: 3637 3038 3133 3630 2d6c 696e 652d 3229  67081360-line-2)
+00009b30: 223e e294 a3e2 9481 e294 8126 2331 3630  ">.........&#160
+00009b40: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
+00009b50: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+00009b60: 3637 3038 3133 3630 2d72 3422 2078 3d22  67081360-r4" x="
+00009b70: 3438 2e38 2220 793d 2236 382e 3822 2074  48.8" y="68.8" t
+00009b80: 6578 744c 656e 6774 683d 2232 342e 3422  extLength="24.4"
+00009b90: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+00009ba0: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+00009bb0: 3133 3630 2d6c 696e 652d 3229 223e f09f  1360-line-2)">..
+00009bc0: 9381 2623 3136 303b 3c2f 7465 7874 3e3c  ..&#160;</text><
+00009bd0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+00009be0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+00009bf0: 7238 2220 783d 2238 352e 3422 2079 3d22  r8" x="85.4" y="
+00009c00: 3638 2e38 2220 7465 7874 4c65 6e67 7468  68.8" textLength
+00009c10: 3d22 3835 2e34 2220 636c 6970 2d70 6174  ="85.4" clip-pat
+00009c20: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+00009c30: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+00009c40: 2d32 2922 3e2e 6769 7468 7562 3c2f 7465  -2)">.github</te
+00009c50: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+00009c60: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+00009c70: 3336 302d 7236 2220 783d 2234 3531 2e34  360-r6" x="451.4
+00009c80: 2220 793d 2236 382e 3822 2074 6578 744c  " y="68.8" textL
+00009c90: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+00009ca0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+00009cb0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+00009cc0: 2d6c 696e 652d 3229 223e e294 833c 2f74  -line-2)">...</t
+00009cd0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+00009ce0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+00009cf0: 3133 3630 2d72 3922 2078 3d22 3131 3436  1360-r9" x="1146
+00009d00: 2e38 2220 793d 2236 382e 3822 2074 6578  .8" y="68.8" tex
+00009d10: 744c 656e 6774 683d 2237 332e 3222 2063  tLength="73.2" c
+00009d20: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+00009d30: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00009d40: 3630 2d6c 696e 652d 3229 223e 6272 6f77  60-line-2)">brow
+00009d50: 7372 3c2f 7465 7874 3e3c 7465 7874 2063  sr</text><text c
+00009d60: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+00009d70: 3136 3730 3831 3336 302d 7236 2220 783d  167081360-r6" x=
+00009d80: 2231 3931 352e 3422 2079 3d22 3638 2e38  "1915.4" y="68.8
+00009d90: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
+00009da0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
+00009db0: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+00009dc0: 3730 3831 3336 302d 6c69 6e65 2d32 2922  7081360-line-2)"
+00009dd0: 3ee2 9483 3c2f 7465 7874 3e3c 7465 7874  >...</text><text
+00009de0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+00009df0: 2d32 3136 3730 3831 3336 302d 7231 2220  -2167081360-r1" 
+00009e00: 783d 2231 3935 3222 2079 3d22 3638 2e38  x="1952" y="68.8
+00009e10: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
+00009e20: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
+00009e30: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+00009e40: 3730 3831 3336 302d 6c69 6e65 2d32 2922  7081360-line-2)"
+00009e50: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
+00009e60: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+00009e70: 3136 3730 3831 3336 302d 7237 2220 783d  167081360-r7" x=
+00009e80: 2230 2220 793d 2239 332e 3222 2074 6578  "0" y="93.2" tex
+00009e90: 744c 656e 6774 683d 2234 382e 3822 2063  tLength="48.8" c
+00009ea0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+00009eb0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00009ec0: 3630 2d6c 696e 652d 3329 223e e294 a3e2  60-line-3)">....
+00009ed0: 9481 e294 8126 2331 3630 3b3c 2f74 6578  .....&#160;</tex
+00009ee0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+00009ef0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+00009f00: 3630 2d72 3422 2078 3d22 3438 2e38 2220  60-r4" x="48.8" 
+00009f10: 793d 2239 332e 3222 2074 6578 744c 656e  y="93.2" textLen
+00009f20: 6774 683d 2232 342e 3422 2063 6c69 702d  gth="24.4" clip-
+00009f30: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+00009f40: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+00009f50: 696e 652d 3329 223e f09f 9381 2623 3136  ine-3)">....&#16
+00009f60: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
+00009f70: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+00009f80: 3136 3730 3831 3336 302d 7231 3022 2078  167081360-r10" x
+00009f90: 3d22 3835 2e34 2220 793d 2239 332e 3222  ="85.4" y="93.2"
+00009fa0: 2074 6578 744c 656e 6774 683d 2237 332e   textLength="73.
+00009fb0: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+00009fc0: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+00009fd0: 3038 3133 3630 2d6c 696e 652d 3329 223e  081360-line-3)">
+00009fe0: 6272 6f77 7372 3c2f 7465 7874 3e3c 7465  browsr</text><te
+00009ff0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000a000: 616c 2d32 3136 3730 3831 3336 302d 7236  al-2167081360-r6
+0000a010: 2220 783d 2234 3531 2e34 2220 793d 2239  " x="451.4" y="9
+0000a020: 332e 3222 2074 6578 744c 656e 6774 683d  3.2" textLength=
+0000a030: 2231 3437 362e 3222 2063 6c69 702d 7061  "1476.2" clip-pa
+0000a040: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000a050: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000a060: 652d 3329 223e e294 97e2 9481 e294 81e2  e-3)">..........
+0000a070: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a080: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a090: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a0a0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a0b0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a0c0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a0d0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a0e0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a0f0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a100: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a110: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a120: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a130: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a140: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a150: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a160: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a170: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a180: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a190: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a1a0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+0000a1b0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+0000a1c0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+0000a1d0: 9b3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000a1e0: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000a1f0: 3637 3038 3133 3630 2d72 3122 2078 3d22  67081360-r1" x="
+0000a200: 3139 3532 2220 793d 2239 332e 3222 2074  1952" y="93.2" t
+0000a210: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000a220: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000a230: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000a240: 3133 3630 2d6c 696e 652d 3329 223e 0a3c  1360-line-3)">.<
+0000a250: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000a260: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000a270: 3038 3133 3630 2d72 3722 2078 3d22 3022  081360-r7" x="0"
+0000a280: 2079 3d22 3131 372e 3622 2074 6578 744c   y="117.6" textL
+0000a290: 656e 6774 683d 2234 382e 3822 2063 6c69  ength="48.8" cli
+0000a2a0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000a2b0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000a2c0: 2d6c 696e 652d 3429 223e e294 a3e2 9481  -line-4)">......
+0000a2d0: e294 8126 2331 3630 3b3c 2f74 6578 743e  ...&#160;</text>
+0000a2e0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000a2f0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000a300: 2d72 3422 2078 3d22 3438 2e38 2220 793d  -r4" x="48.8" y=
+0000a310: 2231 3137 2e36 2220 7465 7874 4c65 6e67  "117.6" textLeng
+0000a320: 7468 3d22 3234 2e34 2220 636c 6970 2d70  th="24.4" clip-p
+0000a330: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000a340: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000a350: 6e65 2d34 2922 3ef0 9f93 8126 2331 3630  ne-4)">....&#160
+0000a360: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
+0000a370: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000a380: 3637 3038 3133 3630 2d72 3130 2220 783d  67081360-r10" x=
+0000a390: 2238 352e 3422 2079 3d22 3131 372e 3622  "85.4" y="117.6"
+0000a3a0: 2074 6578 744c 656e 6774 683d 2234 382e   textLength="48.
+0000a3b0: 3822 2063 6c69 702d 7061 7468 3d22 7572  8" clip-path="ur
+0000a3c0: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+0000a3d0: 3038 3133 3630 2d6c 696e 652d 3429 223e  081360-line-4)">
+0000a3e0: 646f 6373 3c2f 7465 7874 3e3c 7465 7874  docs</text><text
+0000a3f0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000a400: 2d32 3136 3730 3831 3336 302d 7231 2220  -2167081360-r1" 
+0000a410: 783d 2231 3935 3222 2079 3d22 3131 372e  x="1952" y="117.
+0000a420: 3622 2074 6578 744c 656e 6774 683d 2231  6" textLength="1
+0000a430: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000a440: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000a450: 3637 3038 3133 3630 2d6c 696e 652d 3429  67081360-line-4)
+0000a460: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
+0000a470: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000a480: 3231 3637 3038 3133 3630 2d72 3722 2078  2167081360-r7" x
+0000a490: 3d22 3022 2079 3d22 3134 3222 2074 6578  ="0" y="142" tex
+0000a4a0: 744c 656e 6774 683d 2234 382e 3822 2063  tLength="48.8" c
+0000a4b0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000a4c0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000a4d0: 3630 2d6c 696e 652d 3529 223e e294 a3e2  60-line-5)">....
+0000a4e0: 9481 e294 8126 2331 3630 3b3c 2f74 6578  .....&#160;</tex
+0000a4f0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000a500: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000a510: 3630 2d72 3422 2078 3d22 3438 2e38 2220  60-r4" x="48.8" 
+0000a520: 793d 2231 3432 2220 7465 7874 4c65 6e67  y="142" textLeng
+0000a530: 7468 3d22 3234 2e34 2220 636c 6970 2d70  th="24.4" clip-p
+0000a540: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000a550: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000a560: 6e65 2d35 2922 3ef0 9f93 8126 2331 3630  ne-5)">....&#160
 0000a570: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-0000a580: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000a590: 3234 3735 3934 3635 2d72 3422 2078 3d22  24759465-r4" x="
-0000a5a0: 3438 2e38 2220 793d 2231 3636 2e34 2220  48.8" y="166.4" 
-0000a5b0: 7465 7874 4c65 6e67 7468 3d22 3234 2e34  textLength="24.4
+0000a580: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000a590: 3637 3038 3133 3630 2d72 3130 2220 783d  67081360-r10" x=
+0000a5a0: 2238 352e 3422 2079 3d22 3134 3222 2074  "85.4" y="142" t
+0000a5b0: 6578 744c 656e 6774 683d 2231 3436 2e34  extLength="146.4
 0000a5c0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000a5d0: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-0000a5e0: 3539 3436 352d 6c69 6e65 2d36 2922 3ef0  59465-line-6)">.
-0000a5f0: 9f93 8126 2331 3630 3b3c 2f74 6578 743e  ...&#160;</text>
-0000a600: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-0000a610: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000a620: 2d72 3130 2220 783d 2238 352e 3422 2079  -r10" x="85.4" y
-0000a630: 3d22 3136 362e 3422 2074 6578 744c 656e  ="166.4" textLen
-0000a640: 6774 683d 2236 3122 2063 6c69 702d 7061  gth="61" clip-pa
-0000a650: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000a660: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000a670: 652d 3629 223e 7465 7374 733c 2f74 6578  e-6)">tests</tex
-0000a680: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000a690: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000a6a0: 3635 2d72 3622 2078 3d22 3435 312e 3422  65-r6" x="451.4"
-0000a6b0: 2079 3d22 3136 362e 3422 2074 6578 744c   y="166.4" textL
-0000a6c0: 656e 6774 683d 2232 342e 3422 2063 6c69  ength="24.4" cli
-0000a6d0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000a6e0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000a6f0: 2d6c 696e 652d 3629 223e f09f 8c86 2623  -line-6)">....&#
-0000a700: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
-0000a710: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000a720: 2d31 3732 3437 3539 3436 352d 7231 3122  -1724759465-r11"
-0000a730: 2078 3d22 3438 3822 2079 3d22 3136 362e   x="488" y="166.
-0000a740: 3422 2074 6578 744c 656e 6774 683d 2231  4" textLength="1
-0000a750: 3730 2e38 2220 636c 6970 2d70 6174 683d  70.8" clip-path=
-0000a760: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000a770: 3732 3437 3539 3436 352d 6c69 6e65 2d36  724759465-line-6
-0000a780: 2922 3e62 726f 7773 7226 2331 3630 3b56  )">browsr&#160;V
-0000a790: 6572 7369 6f6e 3c2f 7465 7874 3e3c 7465  ersion</text><te
-0000a7a0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000a7b0: 616c 2d31 3732 3437 3539 3436 352d 7236  al-1724759465-r6
-0000a7c0: 2220 783d 2236 3731 2220 793d 2231 3636  " x="671" y="166
-0000a7d0: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
-0000a7e0: 3234 2e34 2220 636c 6970 2d70 6174 683d  24.4" clip-path=
-0000a7f0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000a800: 3732 3437 3539 3436 352d 6c69 6e65 2d36  724759465-line-6
-0000a810: 2922 3ef0 9f8c 8626 2331 3630 3b3c 2f74  )">....&#160;</t
-0000a820: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000a830: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000a840: 3934 3635 2d72 3131 2220 783d 2237 3037  9465-r11" x="707
-0000a850: 2e36 2220 793d 2231 3636 2e34 2220 7465  .6" y="166.4" te
-0000a860: 7874 4c65 6e67 7468 3d22 3438 2e38 2220  xtLength="48.8" 
-0000a870: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000a880: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000a890: 3436 352d 6c69 6e65 2d36 2922 3e50 7950  465-line-6)">PyP
-0000a8a0: 493c 2f74 6578 743e 3c74 6578 7420 636c  I</text><text cl
-0000a8b0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000a8c0: 3234 3735 3934 3635 2d72 3622 2078 3d22  24759465-r6" x="
-0000a8d0: 3736 382e 3622 2079 3d22 3136 362e 3422  768.6" y="166.4"
-0000a8e0: 2074 6578 744c 656e 6774 683d 2232 342e   textLength="24.
-0000a8f0: 3422 2063 6c69 702d 7061 7468 3d22 7572  4" clip-path="ur
-0000a900: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000a910: 3735 3934 3635 2d6c 696e 652d 3629 223e  759465-line-6)">
-0000a920: f09f 8c86 2623 3136 303b 3c2f 7465 7874  ....&#160;</text
-0000a930: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000a940: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000a950: 352d 7231 3122 2078 3d22 3830 352e 3222  5-r11" x="805.2"
-0000a960: 2079 3d22 3136 362e 3422 2074 6578 744c   y="166.4" textL
-0000a970: 656e 6774 683d 2231 3730 2e38 2220 636c  ength="170.8" cl
-0000a980: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000a990: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000a9a0: 352d 6c69 6e65 2d36 2922 3e54 6573 7469  5-line-6)">Testi
-0000a9b0: 6e67 2623 3136 303b 5374 6174 7573 3c2f  ng&#160;Status</
-0000a9c0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000a9d0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000a9e0: 3539 3436 352d 7236 2220 783d 2239 3838  59465-r6" x="988
-0000a9f0: 2e32 2220 793d 2231 3636 2e34 2220 7465  .2" y="166.4" te
-0000aa00: 7874 4c65 6e67 7468 3d22 3234 2e34 2220  xtLength="24.4" 
-0000aa10: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000aa20: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000aa30: 3436 352d 6c69 6e65 2d36 2922 3ef0 9f8c  465-line-6)">...
-0000aa40: 8626 2331 3630 3b3c 2f74 6578 743e 3c74  .&#160;</text><t
-0000aa50: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000aa60: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000aa70: 3131 2220 783d 2231 3032 342e 3822 2079  11" x="1024.8" y
-0000aa80: 3d22 3136 362e 3422 2074 6578 744c 656e  ="166.4" textLen
-0000aa90: 6774 683d 2231 3730 2e38 2220 636c 6970  gth="170.8" clip
-0000aaa0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000aab0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000aac0: 6c69 6e65 2d36 2922 3e47 6974 4875 6226  line-6)">GitHub&
-0000aad0: 2331 3630 3b4c 6963 656e 7365 3c2f 7465  #160;License</te
-0000aae0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000aaf0: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000ab00: 3436 352d 7231 2220 783d 2231 3935 3222  465-r1" x="1952"
-0000ab10: 2079 3d22 3136 362e 3422 2074 6578 744c   y="166.4" textL
-0000ab20: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
-0000ab30: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000ab40: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000ab50: 2d6c 696e 652d 3629 223e 0a3c 2f74 6578  -line-6)">.</tex
-0000ab60: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000ab70: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000ab80: 3635 2d72 3722 2078 3d22 3022 2079 3d22  65-r7" x="0" y="
-0000ab90: 3139 302e 3822 2074 6578 744c 656e 6774  190.8" textLengt
-0000aba0: 683d 2234 382e 3822 2063 6c69 702d 7061  h="48.8" clip-pa
-0000abb0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000abc0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000abd0: 652d 3729 223e e294 9ce2 9480 e294 8026  e-7)">.........&
-0000abe0: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
-0000abf0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000ac00: 6c2d 3137 3234 3735 3934 3635 2d72 3422  l-1724759465-r4"
-0000ac10: 2078 3d22 3438 2e38 2220 793d 2231 3930   x="48.8" y="190
-0000ac20: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
-0000ac30: 3234 2e34 2220 636c 6970 2d70 6174 683d  24.4" clip-path=
-0000ac40: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000ac50: 3732 3437 3539 3436 352d 6c69 6e65 2d37  724759465-line-7
-0000ac60: 2922 3ef0 9f93 8426 2331 3630 3b3c 2f74  )">....&#160;</t
+0000a5d0: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+0000a5e0: 3831 3336 302d 6c69 6e65 2d35 2922 3e72  81360-line-5)">r
+0000a5f0: 6571 7569 7265 6d65 6e74 733c 2f74 6578  equirements</tex
+0000a600: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000a610: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000a620: 3630 2d72 3122 2078 3d22 3139 3532 2220  60-r1" x="1952" 
+0000a630: 793d 2231 3432 2220 7465 7874 4c65 6e67  y="142" textLeng
+0000a640: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000a650: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000a660: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000a670: 6e65 2d35 2922 3e0a 3c2f 7465 7874 3e3c  ne-5)">.</text><
+0000a680: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000a690: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000a6a0: 7237 2220 783d 2230 2220 793d 2231 3636  r7" x="0" y="166
+0000a6b0: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
+0000a6c0: 3438 2e38 2220 636c 6970 2d70 6174 683d  48.8" clip-path=
+0000a6d0: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000a6e0: 3136 3730 3831 3336 302d 6c69 6e65 2d36  167081360-line-6
+0000a6f0: 2922 3ee2 94a3 e294 81e2 9481 2623 3136  )">.........&#16
+0000a700: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
+0000a710: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000a720: 3136 3730 3831 3336 302d 7234 2220 783d  167081360-r4" x=
+0000a730: 2234 382e 3822 2079 3d22 3136 362e 3422  "48.8" y="166.4"
+0000a740: 2074 6578 744c 656e 6774 683d 2232 342e   textLength="24.
+0000a750: 3422 2063 6c69 702d 7061 7468 3d22 7572  4" clip-path="ur
+0000a760: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+0000a770: 3038 3133 3630 2d6c 696e 652d 3629 223e  081360-line-6)">
+0000a780: f09f 9381 2623 3136 303b 3c2f 7465 7874  ....&#160;</text
+0000a790: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+0000a7a0: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000a7b0: 302d 7231 3022 2078 3d22 3835 2e34 2220  0-r10" x="85.4" 
+0000a7c0: 793d 2231 3636 2e34 2220 7465 7874 4c65  y="166.4" textLe
+0000a7d0: 6e67 7468 3d22 3631 2220 636c 6970 2d70  ngth="61" clip-p
+0000a7e0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000a7f0: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000a800: 6e65 2d36 2922 3e74 6573 7473 3c2f 7465  ne-6)">tests</te
+0000a810: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000a820: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000a830: 3336 302d 7236 2220 783d 2234 3531 2e34  360-r6" x="451.4
+0000a840: 2220 793d 2231 3636 2e34 2220 7465 7874  " y="166.4" text
+0000a850: 4c65 6e67 7468 3d22 3234 2e34 2220 636c  Length="24.4" cl
+0000a860: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000a870: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000a880: 302d 6c69 6e65 2d36 2922 3ef0 9f8c 8626  0-line-6)">....&
+0000a890: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+0000a8a0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000a8b0: 6c2d 3231 3637 3038 3133 3630 2d72 3131  l-2167081360-r11
+0000a8c0: 2220 783d 2234 3838 2220 793d 2231 3636  " x="488" y="166
+0000a8d0: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
+0000a8e0: 3137 302e 3822 2063 6c69 702d 7061 7468  170.8" clip-path
+0000a8f0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000a900: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000a910: 3629 223e 6272 6f77 7372 2623 3136 303b  6)">browsr&#160;
+0000a920: 5665 7273 696f 6e3c 2f74 6578 743e 3c74  Version</text><t
+0000a930: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000a940: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000a950: 3622 2078 3d22 3637 3122 2079 3d22 3136  6" x="671" y="16
+0000a960: 362e 3422 2074 6578 744c 656e 6774 683d  6.4" textLength=
+0000a970: 2232 342e 3422 2063 6c69 702d 7061 7468  "24.4" clip-path
+0000a980: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000a990: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000a9a0: 3629 223e f09f 8c86 2623 3136 303b 3c2f  6)">....&#160;</
+0000a9b0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000a9c0: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000a9d0: 3831 3336 302d 7231 3122 2078 3d22 3730  81360-r11" x="70
+0000a9e0: 372e 3622 2079 3d22 3136 362e 3422 2074  7.6" y="166.4" t
+0000a9f0: 6578 744c 656e 6774 683d 2234 382e 3822  extLength="48.8"
+0000aa00: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000aa10: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000aa20: 3133 3630 2d6c 696e 652d 3629 223e 5079  1360-line-6)">Py
+0000aa30: 5049 3c2f 7465 7874 3e3c 7465 7874 2063  PI</text><text c
+0000aa40: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000aa50: 3136 3730 3831 3336 302d 7236 2220 783d  167081360-r6" x=
+0000aa60: 2237 3638 2e36 2220 793d 2231 3636 2e34  "768.6" y="166.4
+0000aa70: 2220 7465 7874 4c65 6e67 7468 3d22 3234  " textLength="24
+0000aa80: 2e34 2220 636c 6970 2d70 6174 683d 2275  .4" clip-path="u
+0000aa90: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000aaa0: 3730 3831 3336 302d 6c69 6e65 2d36 2922  7081360-line-6)"
+0000aab0: 3ef0 9f8c 8626 2331 3630 3b3c 2f74 6578  >....&#160;</tex
+0000aac0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000aad0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000aae0: 3630 2d72 3131 2220 783d 2238 3035 2e32  60-r11" x="805.2
+0000aaf0: 2220 793d 2231 3636 2e34 2220 7465 7874  " y="166.4" text
+0000ab00: 4c65 6e67 7468 3d22 3137 302e 3822 2063  Length="170.8" c
+0000ab10: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000ab20: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000ab30: 3630 2d6c 696e 652d 3629 223e 5465 7374  60-line-6)">Test
+0000ab40: 696e 6726 2331 3630 3b53 7461 7475 733c  ing&#160;Status<
+0000ab50: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000ab60: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000ab70: 3038 3133 3630 2d72 3622 2078 3d22 3938  081360-r6" x="98
+0000ab80: 382e 3222 2079 3d22 3136 362e 3422 2074  8.2" y="166.4" t
+0000ab90: 6578 744c 656e 6774 683d 2232 342e 3422  extLength="24.4"
+0000aba0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000abb0: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000abc0: 3133 3630 2d6c 696e 652d 3629 223e f09f  1360-line-6)">..
+0000abd0: 8c86 2623 3136 303b 3c2f 7465 7874 3e3c  ..&#160;</text><
+0000abe0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000abf0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000ac00: 7231 3122 2078 3d22 3130 3234 2e38 2220  r11" x="1024.8" 
+0000ac10: 793d 2231 3636 2e34 2220 7465 7874 4c65  y="166.4" textLe
+0000ac20: 6e67 7468 3d22 3137 302e 3822 2063 6c69  ngth="170.8" cli
+0000ac30: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000ac40: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000ac50: 2d6c 696e 652d 3629 223e 4769 7448 7562  -line-6)">GitHub
+0000ac60: 2623 3136 303b 4c69 6365 6e73 653c 2f74  &#160;License</t
 0000ac70: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000ac80: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000ac90: 3934 3635 2d72 3132 2220 783d 2238 352e  9465-r12" x="85.
-0000aca0: 3422 2079 3d22 3139 302e 3822 2074 6578  4" y="190.8" tex
-0000acb0: 744c 656e 6774 683d 2231 3232 2220 636c  tLength="122" cl
+0000ac80: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000ac90: 3133 3630 2d72 3122 2078 3d22 3139 3532  1360-r1" x="1952
+0000aca0: 2220 793d 2231 3636 2e34 2220 7465 7874  " y="166.4" text
+0000acb0: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
 0000acc0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000acd0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000ace0: 352d 6c69 6e65 2d37 2922 3e2e 6769 7469  5-line-7)">.giti
-0000acf0: 676e 6f72 653c 2f74 6578 743e 3c74 6578  gnore</text><tex
-0000ad00: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000ad10: 6c2d 3137 3234 3735 3934 3635 2d72 3122  l-1724759465-r1"
-0000ad20: 2078 3d22 3139 3532 2220 793d 2231 3930   x="1952" y="190
-0000ad30: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
-0000ad40: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000ad50: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000ad60: 3732 3437 3539 3436 352d 6c69 6e65 2d37  724759465-line-7
-0000ad70: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000ad80: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000ad90: 2d31 3732 3437 3539 3436 352d 7237 2220  -1724759465-r7" 
-0000ada0: 783d 2230 2220 793d 2232 3135 2e32 2220  x="0" y="215.2" 
-0000adb0: 7465 7874 4c65 6e67 7468 3d22 3438 2e38  textLength="48.8
-0000adc0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000add0: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-0000ade0: 3539 3436 352d 6c69 6e65 2d38 2922 3ee2  59465-line-8)">.
-0000adf0: 949c e294 80e2 9480 2623 3136 303b 3c2f  ........&#160;</
+0000acd0: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000ace0: 302d 6c69 6e65 2d36 2922 3e0a 3c2f 7465  0-line-6)">.</te
+0000acf0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000ad00: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000ad10: 3336 302d 7237 2220 783d 2230 2220 793d  360-r7" x="0" y=
+0000ad20: 2231 3930 2e38 2220 7465 7874 4c65 6e67  "190.8" textLeng
+0000ad30: 7468 3d22 3438 2e38 2220 636c 6970 2d70  th="48.8" clip-p
+0000ad40: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000ad50: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000ad60: 6e65 2d37 2922 3ee2 94a3 e294 81e2 9481  ne-7)">.........
+0000ad70: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
+0000ad80: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000ad90: 616c 2d32 3136 3730 3831 3336 302d 7234  al-2167081360-r4
+0000ada0: 2220 783d 2234 382e 3822 2079 3d22 3139  " x="48.8" y="19
+0000adb0: 302e 3822 2074 6578 744c 656e 6774 683d  0.8" textLength=
+0000adc0: 2232 342e 3422 2063 6c69 702d 7061 7468  "24.4" clip-path
+0000add0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000ade0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000adf0: 3729 223e f09f 9384 2623 3136 303b 3c2f  7)">....&#160;</
 0000ae00: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000ae10: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000ae20: 3539 3436 352d 7234 2220 783d 2234 382e  59465-r4" x="48.
-0000ae30: 3822 2079 3d22 3231 352e 3222 2074 6578  8" y="215.2" tex
-0000ae40: 744c 656e 6774 683d 2232 342e 3422 2063  tLength="24.4" c
+0000ae10: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000ae20: 3831 3336 302d 7231 3222 2078 3d22 3835  81360-r12" x="85
+0000ae30: 2e34 2220 793d 2231 3930 2e38 2220 7465  .4" y="190.8" te
+0000ae40: 7874 4c65 6e67 7468 3d22 3132 3222 2063  xtLength="122" c
 0000ae50: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000ae60: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000ae70: 3635 2d6c 696e 652d 3829 223e f09f 9384  65-line-8)">....
-0000ae80: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
+0000ae60: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000ae70: 3630 2d6c 696e 652d 3729 223e 2e67 6974  60-line-7)">.git
+0000ae80: 6967 6e6f 7265 3c2f 7465 7874 3e3c 7465  ignore</text><te
 0000ae90: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000aea0: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000aeb0: 3222 2078 3d22 3835 2e34 2220 793d 2232  2" x="85.4" y="2
-0000aec0: 3135 2e32 2220 7465 7874 4c65 6e67 7468  15.2" textLength
-0000aed0: 3d22 3238 302e 3622 2063 6c69 702d 7061  ="280.6" clip-pa
-0000aee0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000aef0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000af00: 652d 3829 223e 2e70 7265 2d63 6f6d 6d69  e-8)">.pre-commi
-0000af10: 742d 636f 6e66 6967 2e79 616d 6c3c 2f74  t-config.yaml</t
-0000af20: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000af30: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000af40: 3934 3635 2d72 3133 2220 783d 2234 3531  9465-r13" x="451
-0000af50: 2e34 2220 793d 2232 3135 2e32 2220 7465  .4" y="215.2" te
-0000af60: 7874 4c65 6e67 7468 3d22 3733 2e32 2220  xtLength="73.2" 
-0000af70: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000af80: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000af90: 3436 352d 6c69 6e65 2d38 2922 3e62 726f  465-line-8)">bro
-0000afa0: 7773 723c 2f74 6578 743e 3c74 6578 7420  wsr</text><text 
-0000afb0: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000afc0: 3137 3234 3735 3934 3635 2d72 3622 2078  1724759465-r6" x
-0000afd0: 3d22 3532 342e 3622 2079 3d22 3231 352e  ="524.6" y="215.
-0000afe0: 3222 2074 6578 744c 656e 6774 683d 2238  2" textLength="8
-0000aff0: 3431 2e38 2220 636c 6970 2d70 6174 683d  41.8" clip-path=
-0000b000: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000b010: 3732 3437 3539 3436 352d 6c69 6e65 2d38  724759465-line-8
-0000b020: 2922 3e26 2331 3630 3b69 7326 2331 3630  )">&#160;is&#160
-0000b030: 3b61 2623 3136 303b 5455 4926 2331 3630  ;a&#160;TUI&#160
-0000b040: 3b28 7465 7874 2d62 6173 6564 2623 3136  ;(text-based&#16
-0000b050: 303b 7573 6572 2623 3136 303b 696e 7465  0;user&#160;inte
-0000b060: 7266 6163 6529 2623 3136 303b 6669 6c65  rface)&#160;file
-0000b070: 2623 3136 303b 6272 6f77 7365 7226 2331  &#160;browser&#1
-0000b080: 3630 3b66 6f72 2623 3136 303b 796f 7572  60;for&#160;your
-0000b090: 2623 3136 303b 7465 726d 696e 616c 2e3c  &#160;terminal.<
-0000b0a0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000b0b0: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000b0c0: 3735 3934 3635 2d72 3622 2078 3d22 3133  759465-r6" x="13
-0000b0d0: 3738 2e36 2220 793d 2232 3135 2e32 2220  78.6" y="215.2" 
-0000b0e0: 7465 7874 4c65 6e67 7468 3d22 3532 342e  textLength="524.
-0000b0f0: 3622 2063 6c69 702d 7061 7468 3d22 7572  6" clip-path="ur
-0000b100: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000b110: 3735 3934 3635 2d6c 696e 652d 3829 223e  759465-line-8)">
-0000b120: 4974 2623 7832 373b 7326 2331 3630 3b61  It&#x27;s&#160;a
-0000b130: 2623 3136 303b 7369 6d70 6c65 2623 3136  &#160;simple&#16
-0000b140: 303b 7761 7926 2331 3630 3b74 6f26 2331  0;way&#160;to&#1
-0000b150: 3630 3b62 726f 7773 6526 2331 3630 3b79  60;browse&#160;y
-0000b160: 6f75 7226 2331 3630 3b66 696c 6573 2623  our&#160;files&#
-0000b170: 3136 303b 616e 6426 2331 3630 3b3c 2f74  160;and&#160;</t
-0000b180: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000b190: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000b1a0: 3934 3635 2d72 3122 2078 3d22 3139 3532  9465-r1" x="1952
-0000b1b0: 2220 793d 2232 3135 2e32 2220 7465 7874  " y="215.2" text
-0000b1c0: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000b1d0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000b1e0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000b1f0: 352d 6c69 6e65 2d38 2922 3e0a 3c2f 7465  5-line-8)">.</te
-0000b200: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000b210: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000b220: 3436 352d 7237 2220 783d 2230 2220 793d  465-r7" x="0" y=
-0000b230: 2232 3339 2e36 2220 7465 7874 4c65 6e67  "239.6" textLeng
-0000b240: 7468 3d22 3438 2e38 2220 636c 6970 2d70  th="48.8" clip-p
-0000b250: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000b260: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000b270: 6e65 2d39 2922 3ee2 949c e294 80e2 9480  ne-9)">.........
-0000b280: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000b290: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000b2a0: 616c 2d31 3732 3437 3539 3436 352d 7234  al-1724759465-r4
-0000b2b0: 2220 783d 2234 382e 3822 2079 3d22 3233  " x="48.8" y="23
-0000b2c0: 392e 3622 2074 6578 744c 656e 6774 683d  9.6" textLength=
-0000b2d0: 2232 342e 3422 2063 6c69 702d 7061 7468  "24.4" clip-path
-0000b2e0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000b2f0: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000b300: 3929 223e f09f 9384 2623 3136 303b 3c2f  9)">....&#160;</
+0000aea0: 616c 2d32 3136 3730 3831 3336 302d 7231  al-2167081360-r1
+0000aeb0: 2220 783d 2231 3935 3222 2079 3d22 3139  " x="1952" y="19
+0000aec0: 302e 3822 2074 6578 744c 656e 6774 683d  0.8" textLength=
+0000aed0: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000aee0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000aef0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000af00: 3729 223e 0a3c 2f74 6578 743e 3c74 6578  7)">.</text><tex
+0000af10: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000af20: 6c2d 3231 3637 3038 3133 3630 2d72 3722  l-2167081360-r7"
+0000af30: 2078 3d22 3022 2079 3d22 3231 352e 3222   x="0" y="215.2"
+0000af40: 2074 6578 744c 656e 6774 683d 2234 382e   textLength="48.
+0000af50: 3822 2063 6c69 702d 7061 7468 3d22 7572  8" clip-path="ur
+0000af60: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+0000af70: 3038 3133 3630 2d6c 696e 652d 3829 223e  081360-line-8)">
+0000af80: e294 a3e2 9481 e294 8126 2331 3630 3b3c  .........&#160;<
+0000af90: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000afa0: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000afb0: 3038 3133 3630 2d72 3422 2078 3d22 3438  081360-r4" x="48
+0000afc0: 2e38 2220 793d 2232 3135 2e32 2220 7465  .8" y="215.2" te
+0000afd0: 7874 4c65 6e67 7468 3d22 3234 2e34 2220  xtLength="24.4" 
+0000afe0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000aff0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000b000: 3336 302d 6c69 6e65 2d38 2922 3ef0 9f93  360-line-8)">...
+0000b010: 8426 2331 3630 3b3c 2f74 6578 743e 3c74  .&#160;</text><t
+0000b020: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000b030: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000b040: 3132 2220 783d 2238 352e 3422 2079 3d22  12" x="85.4" y="
+0000b050: 3231 352e 3222 2074 6578 744c 656e 6774  215.2" textLengt
+0000b060: 683d 2232 3830 2e36 2220 636c 6970 2d70  h="280.6" clip-p
+0000b070: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000b080: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000b090: 6e65 2d38 2922 3e2e 7072 652d 636f 6d6d  ne-8)">.pre-comm
+0000b0a0: 6974 2d63 6f6e 6669 672e 7961 6d6c 3c2f  it-config.yaml</
+0000b0b0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000b0c0: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000b0d0: 3831 3336 302d 7231 3322 2078 3d22 3435  81360-r13" x="45
+0000b0e0: 312e 3422 2079 3d22 3231 352e 3222 2074  1.4" y="215.2" t
+0000b0f0: 6578 744c 656e 6774 683d 2237 332e 3222  extLength="73.2"
+0000b100: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000b110: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000b120: 3133 3630 2d6c 696e 652d 3829 223e 6272  1360-line-8)">br
+0000b130: 6f77 7372 3c2f 7465 7874 3e3c 7465 7874  owsr</text><text
+0000b140: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000b150: 2d32 3136 3730 3831 3336 302d 7236 2220  -2167081360-r6" 
+0000b160: 783d 2235 3234 2e36 2220 793d 2232 3135  x="524.6" y="215
+0000b170: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
+0000b180: 3834 312e 3822 2063 6c69 702d 7061 7468  841.8" clip-path
+0000b190: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000b1a0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000b1b0: 3829 223e 2623 3136 303b 6973 2623 3136  8)">&#160;is&#16
+0000b1c0: 303b 6126 2331 3630 3b54 5549 2623 3136  0;a&#160;TUI&#16
+0000b1d0: 303b 2874 6578 742d 6261 7365 6426 2331  0;(text-based&#1
+0000b1e0: 3630 3b75 7365 7226 2331 3630 3b69 6e74  60;user&#160;int
+0000b1f0: 6572 6661 6365 2926 2331 3630 3b66 696c  erface)&#160;fil
+0000b200: 6526 2331 3630 3b62 726f 7773 6572 2623  e&#160;browser&#
+0000b210: 3136 303b 666f 7226 2331 3630 3b79 6f75  160;for&#160;you
+0000b220: 7226 2331 3630 3b74 6572 6d69 6e61 6c2e  r&#160;terminal.
+0000b230: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000b240: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000b250: 3730 3831 3336 302d 7236 2220 783d 2231  7081360-r6" x="1
+0000b260: 3337 382e 3622 2079 3d22 3231 352e 3222  378.6" y="215.2"
+0000b270: 2074 6578 744c 656e 6774 683d 2235 3234   textLength="524
+0000b280: 2e36 2220 636c 6970 2d70 6174 683d 2275  .6" clip-path="u
+0000b290: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000b2a0: 3730 3831 3336 302d 6c69 6e65 2d38 2922  7081360-line-8)"
+0000b2b0: 3e49 7426 2378 3237 3b73 2623 3136 303b  >It&#x27;s&#160;
+0000b2c0: 6126 2331 3630 3b73 696d 706c 6526 2331  a&#160;simple&#1
+0000b2d0: 3630 3b77 6179 2623 3136 303b 746f 2623  60;way&#160;to&#
+0000b2e0: 3136 303b 6272 6f77 7365 2623 3136 303b  160;browse&#160;
+0000b2f0: 796f 7572 2623 3136 303b 6669 6c65 7326  your&#160;files&
+0000b300: 2331 3630 3b61 6e64 2623 3136 303b 3c2f  #160;and&#160;</
 0000b310: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000b320: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000b330: 3539 3436 352d 7231 3222 2078 3d22 3835  59465-r12" x="85
-0000b340: 2e34 2220 793d 2232 3339 2e36 2220 7465  .4" y="239.6" te
-0000b350: 7874 4c65 6e67 7468 3d22 3135 382e 3622  xtLength="158.6"
-0000b360: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000b370: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-0000b380: 3934 3635 2d6c 696e 652d 3929 223e 2e72  9465-line-9)">.r
-0000b390: 656c 6561 7365 7263 2e6a 733c 2f74 6578  eleaserc.js</tex
-0000b3a0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000b3b0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000b3c0: 3635 2d72 3622 2078 3d22 3435 312e 3422  65-r6" x="451.4"
-0000b3d0: 2079 3d22 3233 392e 3622 2074 6578 744c   y="239.6" textL
-0000b3e0: 656e 6774 683d 2234 3633 2e36 2220 636c  ength="463.6" cl
-0000b3f0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000b400: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000b410: 352d 6c69 6e65 2d39 2922 3e74 616b 6526  5-line-9)">take&
-0000b420: 2331 3630 3b61 2623 3136 303b 7065 656b  #160;a&#160;peek
-0000b430: 2623 3136 303b 6174 2623 3136 303b 7468  &#160;at&#160;th
-0000b440: 6569 7226 2331 3630 3b63 6f6e 7465 6e74  eir&#160;content
-0000b450: 732e 2623 3136 303b 506c 7573 2623 3136  s.&#160;Plus&#16
-0000b460: 303b 6974 3c2f 7465 7874 3e3c 7465 7874  0;it</text><text
-0000b470: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000b480: 2d31 3732 3437 3539 3436 352d 7236 2220  -1724759465-r6" 
-0000b490: 783d 2239 3237 2e32 2220 793d 2232 3339  x="927.2" y="239
-0000b4a0: 2e36 2220 7465 7874 4c65 6e67 7468 3d22  .6" textLength="
-0000b4b0: 3437 352e 3822 2063 6c69 702d 7061 7468  475.8" clip-path
-0000b4c0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000b4d0: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000b4e0: 3929 223e 776f 726b 7326 2331 3630 3b6f  9)">works&#160;o
-0000b4f0: 6e26 2331 3630 3b6c 6f63 616c 2623 3136  n&#160;local&#16
-0000b500: 303b 616e 6426 2331 3630 3b72 656d 6f74  0;and&#160;remot
-0000b510: 6526 2331 3630 3b66 696c 6526 2331 3630  e&#160;file&#160
-0000b520: 3b73 7973 7465 6d73 2e3c 2f74 6578 743e  ;systems.</text>
-0000b530: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-0000b540: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000b550: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
-0000b560: 2232 3339 2e36 2220 7465 7874 4c65 6e67  "239.6" textLeng
-0000b570: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
-0000b580: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000b590: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000b5a0: 6e65 2d39 2922 3e0a 3c2f 7465 7874 3e3c  ne-9)">.</text><
-0000b5b0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000b5c0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000b5d0: 7237 2220 783d 2230 2220 793d 2232 3634  r7" x="0" y="264
-0000b5e0: 2220 7465 7874 4c65 6e67 7468 3d22 3438  " textLength="48
-0000b5f0: 2e38 2220 636c 6970 2d70 6174 683d 2275  .8" clip-path="u
-0000b600: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000b610: 3437 3539 3436 352d 6c69 6e65 2d31 3029  4759465-line-10)
-0000b620: 223e e294 9ce2 9480 e294 8026 2331 3630  ">.........&#160
-0000b630: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-0000b640: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000b650: 3234 3735 3934 3635 2d72 3422 2078 3d22  24759465-r4" x="
-0000b660: 3438 2e38 2220 793d 2232 3634 2220 7465  48.8" y="264" te
-0000b670: 7874 4c65 6e67 7468 3d22 3234 2e34 2220  xtLength="24.4" 
-0000b680: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000b690: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000b6a0: 3436 352d 6c69 6e65 2d31 3029 223e f09f  465-line-10)">..
-0000b6b0: 9384 2623 3136 303b 3c2f 7465 7874 3e3c  ..&#160;</text><
-0000b6c0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000b6d0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000b6e0: 7234 2220 783d 2238 352e 3422 2079 3d22  r4" x="85.4" y="
-0000b6f0: 3236 3422 2074 6578 744c 656e 6774 683d  264" textLength=
-0000b700: 2238 352e 3422 2063 6c69 702d 7061 7468  "85.4" clip-path
-0000b710: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000b720: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000b730: 3130 2922 3e4c 4943 454e 5345 3c2f 7465  10)">LICENSE</te
-0000b740: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000b750: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000b760: 3436 352d 7231 2220 783d 2231 3935 3222  465-r1" x="1952"
-0000b770: 2079 3d22 3236 3422 2074 6578 744c 656e   y="264" textLen
-0000b780: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
-0000b790: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000b7a0: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000b7b0: 696e 652d 3130 2922 3e0a 3c2f 7465 7874  ine-10)">.</text
-0000b7c0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000b7d0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000b7e0: 352d 7237 2220 783d 2230 2220 793d 2232  5-r7" x="0" y="2
-0000b7f0: 3838 2e34 2220 7465 7874 4c65 6e67 7468  88.4" textLength
-0000b800: 3d22 3438 2e38 2220 636c 6970 2d70 6174  ="48.8" clip-pat
-0000b810: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000b820: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000b830: 2d31 3129 223e e294 9ce2 9480 e294 8026  -11)">.........&
-0000b840: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
-0000b850: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000b860: 6c2d 3137 3234 3735 3934 3635 2d72 3422  l-1724759465-r4"
-0000b870: 2078 3d22 3438 2e38 2220 793d 2232 3838   x="48.8" y="288
-0000b880: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
-0000b890: 3234 2e34 2220 636c 6970 2d70 6174 683d  24.4" clip-path=
-0000b8a0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000b8b0: 3732 3437 3539 3436 352d 6c69 6e65 2d31  724759465-line-1
-0000b8c0: 3129 223e f09f 9384 2623 3136 303b 3c2f  1)">....&#160;</
-0000b8d0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000b8e0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000b8f0: 3539 3436 352d 7234 2220 783d 2238 352e  59465-r4" x="85.
-0000b900: 3422 2079 3d22 3238 382e 3422 2074 6578  4" y="288.4" tex
-0000b910: 744c 656e 6774 683d 2237 332e 3222 2063  tLength="73.2" c
-0000b920: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000b930: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000b940: 3635 2d6c 696e 652d 3131 2922 3e6d 6b64  65-line-11)">mkd
-0000b950: 6f63 733c 2f74 6578 743e 3c74 6578 7420  ocs</text><text 
-0000b960: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000b970: 3137 3234 3735 3934 3635 2d72 3134 2220  1724759465-r14" 
-0000b980: 783d 2231 3538 2e36 2220 793d 2232 3838  x="158.6" y="288
-0000b990: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
-0000b9a0: 3631 2220 636c 6970 2d70 6174 683d 2275  61" clip-path="u
-0000b9b0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000b9c0: 3437 3539 3436 352d 6c69 6e65 2d31 3129  4759465-line-11)
-0000b9d0: 223e 2e79 616d 6c3c 2f74 6578 743e 3c74  ">.yaml</text><t
-0000b9e0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000b9f0: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000ba00: 3122 2078 3d22 3139 3532 2220 793d 2232  1" x="1952" y="2
-0000ba10: 3838 2e34 2220 7465 7874 4c65 6e67 7468  88.4" textLength
-0000ba20: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000ba30: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000ba40: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000ba50: 2d31 3129 223e 0a3c 2f74 6578 743e 3c74  -11)">.</text><t
-0000ba60: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000ba70: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000ba80: 3722 2078 3d22 3022 2079 3d22 3331 322e  7" x="0" y="312.
-0000ba90: 3822 2074 6578 744c 656e 6774 683d 2234  8" textLength="4
-0000baa0: 382e 3822 2063 6c69 702d 7061 7468 3d22  8.8" clip-path="
-0000bab0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000bac0: 3234 3735 3934 3635 2d6c 696e 652d 3132  24759465-line-12
-0000bad0: 2922 3ee2 949c e294 80e2 9480 2623 3136  )">.........&#16
-0000bae0: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
-0000baf0: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000bb00: 3732 3437 3539 3436 352d 7234 2220 783d  724759465-r4" x=
-0000bb10: 2234 382e 3822 2079 3d22 3331 322e 3822  "48.8" y="312.8"
-0000bb20: 2074 6578 744c 656e 6774 683d 2232 342e   textLength="24.
-0000bb30: 3422 2063 6c69 702d 7061 7468 3d22 7572  4" clip-path="ur
-0000bb40: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000bb50: 3735 3934 3635 2d6c 696e 652d 3132 2922  759465-line-12)"
-0000bb60: 3ef0 9f93 8426 2331 3630 3b3c 2f74 6578  >....&#160;</tex
-0000bb70: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000bb80: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000bb90: 3635 2d72 3422 2078 3d22 3835 2e34 2220  65-r4" x="85.4" 
-0000bba0: 793d 2233 3132 2e38 2220 7465 7874 4c65  y="312.8" textLe
-0000bbb0: 6e67 7468 3d22 3130 392e 3822 2063 6c69  ngth="109.8" cli
-0000bbc0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000bbd0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000bbe0: 2d6c 696e 652d 3132 2922 3e70 7970 726f  -line-12)">pypro
-0000bbf0: 6a65 6374 3c2f 7465 7874 3e3c 7465 7874  ject</text><text
-0000bc00: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000bc10: 2d31 3732 3437 3539 3436 352d 7231 3422  -1724759465-r14"
-0000bc20: 2078 3d22 3139 352e 3222 2079 3d22 3331   x="195.2" y="31
-0000bc30: 322e 3822 2074 6578 744c 656e 6774 683d  2.8" textLength=
-0000bc40: 2236 3122 2063 6c69 702d 7061 7468 3d22  "61" clip-path="
-0000bc50: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000bc60: 3234 3735 3934 3635 2d6c 696e 652d 3132  24759465-line-12
-0000bc70: 2922 3e2e 746f 6d6c 3c2f 7465 7874 3e3c  )">.toml</text><
-0000bc80: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000bc90: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000bca0: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000bcb0: 3331 322e 3822 2074 6578 744c 656e 6774  312.8" textLengt
-0000bcc0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000bcd0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000bce0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000bcf0: 652d 3132 2922 3e0a 3c2f 7465 7874 3e3c  e-12)">.</text><
-0000bd00: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000bd10: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000bd20: 7237 2220 783d 2230 2220 793d 2233 3337  r7" x="0" y="337
-0000bd30: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
-0000bd40: 3438 2e38 2220 636c 6970 2d70 6174 683d  48.8" clip-path=
-0000bd50: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000bd60: 3732 3437 3539 3436 352d 6c69 6e65 2d31  724759465-line-1
-0000bd70: 3329 223e e294 94e2 9480 e294 8026 2331  3)">.........&#1
-0000bd80: 3630 3b3c 2f74 6578 743e 3c74 6578 7420  60;</text><text 
-0000bd90: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000bda0: 3137 3234 3735 3934 3635 2d72 3422 2078  1724759465-r4" x
-0000bdb0: 3d22 3438 2e38 2220 793d 2233 3337 2e32  ="48.8" y="337.2
-0000bdc0: 2220 7465 7874 4c65 6e67 7468 3d22 3234  " textLength="24
-0000bdd0: 2e34 2220 636c 6970 2d70 6174 683d 2275  .4" clip-path="u
-0000bde0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000bdf0: 3437 3539 3436 352d 6c69 6e65 2d31 3329  4759465-line-13)
-0000be00: 223e f09f 9384 2623 3136 303b 3c2f 7465  ">....&#160;</te
-0000be10: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000be20: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000be30: 3436 352d 7234 2220 783d 2238 352e 3422  465-r4" x="85.4"
-0000be40: 2079 3d22 3333 372e 3222 2074 6578 744c   y="337.2" textL
-0000be50: 656e 6774 683d 2237 332e 3222 2063 6c69  ength="73.2" cli
-0000be60: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000be70: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000be80: 2d6c 696e 652d 3133 2922 3e52 4541 444d  -line-13)">READM
-0000be90: 453c 2f74 6578 743e 3c74 6578 7420 636c  E</text><text cl
-0000bea0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000beb0: 3234 3735 3934 3635 2d72 3134 2220 783d  24759465-r14" x=
-0000bec0: 2231 3538 2e36 2220 793d 2233 3337 2e32  "158.6" y="337.2
-0000bed0: 2220 7465 7874 4c65 6e67 7468 3d22 3336  " textLength="36
-0000bee0: 2e36 2220 636c 6970 2d70 6174 683d 2275  .6" clip-path="u
-0000bef0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000bf00: 3437 3539 3436 352d 6c69 6e65 2d31 3329  4759465-line-13)
-0000bf10: 223e 2e6d 643c 2f74 6578 743e 3c74 6578  ">.md</text><tex
-0000bf20: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000bf30: 6c2d 3137 3234 3735 3934 3635 2d72 3122  l-1724759465-r1"
-0000bf40: 2078 3d22 3139 3532 2220 793d 2233 3337   x="1952" y="337
-0000bf50: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
-0000bf60: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000bf70: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000bf80: 3732 3437 3539 3436 352d 6c69 6e65 2d31  724759465-line-1
-0000bf90: 3329 223e 0a3c 2f74 6578 743e 3c74 6578  3)">.</text><tex
-0000bfa0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000bfb0: 6c2d 3137 3234 3735 3934 3635 2d72 3122  l-1724759465-r1"
-0000bfc0: 2078 3d22 3139 3532 2220 793d 2233 3631   x="1952" y="361
-0000bfd0: 2e36 2220 7465 7874 4c65 6e67 7468 3d22  .6" textLength="
-0000bfe0: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000bff0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000c000: 3732 3437 3539 3436 352d 6c69 6e65 2d31  724759465-line-1
-0000c010: 3429 223e 0a3c 2f74 6578 743e 3c74 6578  4)">.</text><tex
-0000c020: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000c030: 6c2d 3137 3234 3735 3934 3635 2d72 3135  l-1724759465-r15
-0000c040: 2220 783d 2231 3131 302e 3222 2079 3d22  " x="1110.2" y="
-0000c050: 3338 3622 2074 6578 744c 656e 6774 683d  386" textLength=
-0000c060: 2231 3436 2e34 2220 636c 6970 2d70 6174  "146.4" clip-pat
-0000c070: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000c080: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000c090: 2d31 3529 223e 496e 7374 616c 6c61 7469  -15)">Installati
-0000c0a0: 6f6e 3c2f 7465 7874 3e3c 7465 7874 2063  on</text><text c
-0000c0b0: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000c0c0: 3732 3437 3539 3436 352d 7231 2220 783d  724759465-r1" x=
-0000c0d0: 2231 3935 3222 2079 3d22 3338 3622 2074  "1952" y="386" t
-0000c0e0: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
-0000c0f0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000c100: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-0000c110: 3934 3635 2d6c 696e 652d 3135 2922 3e0a  9465-line-15)">.
-0000c120: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000c130: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000c140: 3437 3539 3436 352d 7231 2220 783d 2231  4759465-r1" x="1
-0000c150: 3935 3222 2079 3d22 3431 302e 3422 2074  952" y="410.4" t
-0000c160: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
-0000c170: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000c180: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-0000c190: 3934 3635 2d6c 696e 652d 3136 2922 3e0a  9465-line-16)">.
-0000c1a0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000c1b0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000c1c0: 3437 3539 3436 352d 7236 2220 783d 2234  4759465-r6" x="4
-0000c1d0: 3531 2e34 2220 793d 2234 3334 2e38 2220  51.4" y="434.8" 
-0000c1e0: 7465 7874 4c65 6e67 7468 3d22 3335 332e  textLength="353.
-0000c1f0: 3822 2063 6c69 702d 7061 7468 3d22 7572  8" clip-path="ur
-0000c200: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000c210: 3735 3934 3635 2d6c 696e 652d 3137 2922  759465-line-17)"
-0000c220: 3e54 6865 2623 3136 303b 6265 6c6f 7726  >The&#160;below&
-0000c230: 2331 3630 3b63 6f6d 6d61 6e64 2623 3136  #160;command&#16
-0000c240: 303b 7265 636f 6d6d 656e 6473 2623 3136  0;recommends&#16
-0000c250: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
-0000c260: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000c270: 3732 3437 3539 3436 352d 7231 3122 2078  724759465-r11" x
-0000c280: 3d22 3830 352e 3222 2079 3d22 3433 342e  ="805.2" y="434.
-0000c290: 3822 2074 6578 744c 656e 6774 683d 2234  8" textLength="4
-0000c2a0: 382e 3822 2063 6c69 702d 7061 7468 3d22  8.8" clip-path="
-0000c2b0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000c2c0: 3234 3735 3934 3635 2d6c 696e 652d 3137  24759465-line-17
-0000c2d0: 2922 3e70 6970 783c 2f74 6578 743e 3c74  )">pipx</text><t
-0000c2e0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000c2f0: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000c300: 3622 2078 3d22 3835 3422 2079 3d22 3433  6" x="854" y="43
-0000c310: 342e 3822 2074 6578 744c 656e 6774 683d  4.8" textLength=
-0000c320: 2232 3037 2e34 2220 636c 6970 2d70 6174  "207.4" clip-pat
-0000c330: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000c340: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000c350: 2d31 3729 223e 2623 3136 303b 696e 7374  -17)">&#160;inst
-0000c360: 6561 6426 2331 3630 3b6f 6626 2331 3630  ead&#160;of&#160
-0000c370: 3b70 6970 2e26 2331 3630 3b3c 2f74 6578  ;pip.&#160;</tex
-0000c380: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000c390: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000c3a0: 3635 2d72 3133 2220 783d 2231 3036 312e  65-r13" x="1061.
-0000c3b0: 3422 2079 3d22 3433 342e 3822 2074 6578  4" y="434.8" tex
-0000c3c0: 744c 656e 6774 683d 2234 382e 3822 2063  tLength="48.8" c
-0000c3d0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000c3e0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000c3f0: 3635 2d6c 696e 652d 3137 2922 3e70 6970  65-line-17)">pip
-0000c400: 783c 2f74 6578 743e 3c74 6578 7420 636c  x</text><text cl
-0000c410: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000c420: 3234 3735 3934 3635 2d72 3622 2078 3d22  24759465-r6" x="
-0000c430: 3131 3130 2e32 2220 793d 2234 3334 2e38  1110.2" y="434.8
-0000c440: 2220 7465 7874 4c65 6e67 7468 3d22 3239  " textLength="29
-0000c450: 322e 3822 2063 6c69 702d 7061 7468 3d22  2.8" clip-path="
-0000c460: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000c470: 3234 3735 3934 3635 2d6c 696e 652d 3137  24759465-line-17
-0000c480: 2922 3e26 2331 3630 3b69 6e73 7461 6c6c  )">&#160;install
-0000c490: 7326 2331 3630 3b74 6865 2623 3136 303b  s&#160;the&#160;
-0000c4a0: 7061 636b 6167 6526 2331 3630 3b69 6e3c  package&#160;in<
-0000c4b0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000c4c0: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000c4d0: 3735 3934 3635 2d72 3622 2078 3d22 3134  759465-r6" x="14
-0000c4e0: 3135 2e32 2220 793d 2234 3334 2e38 2220  15.2" y="434.8" 
-0000c4f0: 7465 7874 4c65 6e67 7468 3d22 3531 322e  textLength="512.
-0000c500: 3422 2063 6c69 702d 7061 7468 3d22 7572  4" clip-path="ur
-0000c510: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000c520: 3735 3934 3635 2d6c 696e 652d 3137 2922  759465-line-17)"
-0000c530: 3e61 6e26 2331 3630 3b69 736f 6c61 7465  >an&#160;isolate
-0000c540: 6426 2331 3630 3b65 6e76 6972 6f6e 6d65  d&#160;environme
-0000c550: 6e74 2623 3136 303b 616e 6426 2331 3630  nt&#160;and&#160
-0000c560: 3b6d 616b 6573 2623 3136 303b 6974 2623  ;makes&#160;it&#
-0000c570: 3136 303b 6561 7379 2623 3136 303b 3c2f  160;easy&#160;</
-0000c580: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000c590: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000c5a0: 3539 3436 352d 7231 2220 783d 2231 3935  59465-r1" x="195
-0000c5b0: 3222 2079 3d22 3433 342e 3822 2074 6578  2" y="434.8" tex
-0000c5c0: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
-0000c5d0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000c5e0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000c5f0: 3635 2d6c 696e 652d 3137 2922 3e0a 3c2f  65-line-17)">.</
-0000c600: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000c610: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000c620: 3539 3436 352d 7236 2220 783d 2234 3531  59465-r6" x="451
-0000c630: 2e34 2220 793d 2234 3539 2e32 2220 7465  .4" y="459.2" te
-0000c640: 7874 4c65 6e67 7468 3d22 3432 3722 2063  xtLength="427" c
-0000c650: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000c660: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000c670: 3635 2d6c 696e 652d 3138 2922 3e74 6f26  65-line-18)">to&
-0000c680: 2331 3630 3b75 6e69 6e73 7461 6c6c 2e26  #160;uninstall.&
-0000c690: 2331 3630 3b49 6626 2331 3630 3b79 6f75  #160;If&#160;you
-0000c6a0: 2623 7832 373b 6426 2331 3630 3b6c 696b  &#x27;d&#160;lik
-0000c6b0: 6526 2331 3630 3b74 6f26 2331 3630 3b75  e&#160;to&#160;u
-0000c6c0: 7365 2623 3136 303b 3c2f 7465 7874 3e3c  se&#160;</text><
-0000c6d0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000c6e0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000c6f0: 7231 3322 2078 3d22 3837 382e 3422 2079  r13" x="878.4" y
-0000c700: 3d22 3435 392e 3222 2074 6578 744c 656e  ="459.2" textLen
-0000c710: 6774 683d 2233 362e 3622 2063 6c69 702d  gth="36.6" clip-
-0000c720: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000c730: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000c740: 696e 652d 3138 2922 3e70 6970 3c2f 7465  ine-18)">pip</te
-0000c750: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000c760: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000c770: 3436 352d 7236 2220 783d 2239 3135 2220  465-r6" x="915" 
-0000c780: 793d 2234 3539 2e32 2220 7465 7874 4c65  y="459.2" textLe
-0000c790: 6e67 7468 3d22 3238 302e 3622 2063 6c69  ngth="280.6" cli
-0000c7a0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000c7b0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000c7c0: 2d6c 696e 652d 3138 2922 3e26 2331 3630  -line-18)">&#160
-0000c7d0: 3b69 6e73 7465 6164 2c26 2331 3630 3b6a  ;instead,&#160;j
-0000c7e0: 7573 7426 2331 3630 3b72 6570 6c61 6365  ust&#160;replace
-0000c7f0: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000c800: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000c810: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000c820: 3322 2078 3d22 3131 3935 2e36 2220 793d  3" x="1195.6" y=
-0000c830: 2234 3539 2e32 2220 7465 7874 4c65 6e67  "459.2" textLeng
-0000c840: 7468 3d22 3438 2e38 2220 636c 6970 2d70  th="48.8" clip-p
-0000c850: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000c860: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000c870: 6e65 2d31 3829 223e 7069 7078 3c2f 7465  ne-18)">pipx</te
-0000c880: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000c890: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000c8a0: 3436 352d 7236 2220 783d 2231 3235 362e  465-r6" x="1256.
-0000c8b0: 3622 2079 3d22 3435 392e 3222 2074 6578  6" y="459.2" tex
-0000c8c0: 744c 656e 6774 683d 2236 3122 2063 6c69  tLength="61" cli
-0000c8d0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000c8e0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000c8f0: 2d6c 696e 652d 3138 2922 3e77 6974 6826  -line-18)">with&
-0000c900: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
-0000c910: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000c920: 6c2d 3137 3234 3735 3934 3635 2d72 3133  l-1724759465-r13
-0000c930: 2220 783d 2231 3331 372e 3622 2079 3d22  " x="1317.6" y="
-0000c940: 3435 392e 3222 2074 6578 744c 656e 6774  459.2" textLengt
-0000c950: 683d 2233 362e 3622 2063 6c69 702d 7061  h="36.6" clip-pa
-0000c960: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000c970: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000c980: 652d 3138 2922 3e70 6970 3c2f 7465 7874  e-18)">pip</text
-0000c990: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000c9a0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000c9b0: 352d 7236 2220 783d 2231 3335 342e 3222  5-r6" x="1354.2"
-0000c9c0: 2079 3d22 3435 392e 3222 2074 6578 744c   y="459.2" textL
-0000c9d0: 656e 6774 683d 2232 3638 2e34 2220 636c  ength="268.4" cl
-0000c9e0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000c9f0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000ca00: 352d 6c69 6e65 2d31 3829 223e 2623 3136  5-line-18)">&#16
-0000ca10: 303b 696e 2623 3136 303b 7468 6526 2331  0;in&#160;the&#1
-0000ca20: 3630 3b62 656c 6f77 2623 3136 303b 636f  60;below&#160;co
-0000ca30: 6d6d 616e 642e 3c2f 7465 7874 3e3c 7465  mmand.</text><te
-0000ca40: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000ca50: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000ca60: 2220 783d 2231 3935 3222 2079 3d22 3435  " x="1952" y="45
-0000ca70: 392e 3222 2074 6578 744c 656e 6774 683d  9.2" textLength=
-0000ca80: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
-0000ca90: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000caa0: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000cab0: 3138 2922 3e0a 3c2f 7465 7874 3e3c 7465  18)">.</text><te
-0000cac0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000cad0: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000cae0: 2220 783d 2231 3935 3222 2079 3d22 3438  " x="1952" y="48
-0000caf0: 332e 3622 2074 6578 744c 656e 6774 683d  3.6" textLength=
-0000cb00: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
-0000cb10: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000cb20: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000cb30: 3139 2922 3e0a 3c2f 7465 7874 3e3c 7465  19)">.</text><te
-0000cb40: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000cb50: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000cb60: 2220 783d 2231 3935 3222 2079 3d22 3530  " x="1952" y="50
-0000cb70: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
-0000cb80: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
-0000cb90: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000cba0: 3234 3735 3934 3635 2d6c 696e 652d 3230  24759465-line-20
-0000cbb0: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000cbc0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000cbd0: 2d31 3732 3437 3539 3436 352d 7231 3622  -1724759465-r16"
-0000cbe0: 2078 3d22 3436 332e 3622 2079 3d22 3533   x="463.6" y="53
-0000cbf0: 322e 3422 2074 6578 744c 656e 6774 683d  2.4" textLength=
-0000cc00: 2234 382e 3822 2063 6c69 702d 7061 7468  "48.8" clip-path
-0000cc10: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000cc20: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000cc30: 3231 2922 3e70 6970 783c 2f74 6578 743e  21)">pipx</text>
-0000cc40: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-0000cc50: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000cc60: 2d72 3136 2220 783d 2235 3234 2e36 2220  -r16" x="524.6" 
-0000cc70: 793d 2235 3332 2e34 2220 7465 7874 4c65  y="532.4" textLe
-0000cc80: 6e67 7468 3d22 3835 2e34 2220 636c 6970  ngth="85.4" clip
-0000cc90: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000cca0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000ccb0: 6c69 6e65 2d32 3129 223e 696e 7374 616c  line-21)">instal
-0000ccc0: 6c3c 2f74 6578 743e 3c74 6578 7420 636c  l</text><text cl
-0000ccd0: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000cce0: 3234 3735 3934 3635 2d72 3136 2220 783d  24759465-r16" x=
-0000ccf0: 2236 3232 2e32 2220 793d 2235 3332 2e34  "622.2" y="532.4
-0000cd00: 2220 7465 7874 4c65 6e67 7468 3d22 3733  " textLength="73
-0000cd10: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000cd20: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000cd30: 3437 3539 3436 352d 6c69 6e65 2d32 3129  4759465-line-21)
-0000cd40: 223e 6272 6f77 7372 3c2f 7465 7874 3e3c  ">browsr</text><
-0000cd50: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000cd60: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000cd70: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000cd80: 3533 322e 3422 2074 6578 744c 656e 6774  532.4" textLengt
-0000cd90: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000cda0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000cdb0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000cdc0: 652d 3231 2922 3e0a 3c2f 7465 7874 3e3c  e-21)">.</text><
-0000cdd0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000cde0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000cdf0: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000ce00: 3535 362e 3822 2074 6578 744c 656e 6774  556.8" textLengt
-0000ce10: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000ce20: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000ce30: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000ce40: 652d 3232 2922 3e0a 3c2f 7465 7874 3e3c  e-22)">.</text><
-0000ce50: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000ce60: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000ce70: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000ce80: 3538 312e 3222 2074 6578 744c 656e 6774  581.2" textLengt
-0000ce90: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000cea0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000ceb0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000cec0: 652d 3233 2922 3e0a 3c2f 7465 7874 3e3c  e-23)">.</text><
-0000ced0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000cee0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000cef0: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000cf00: 3630 352e 3622 2074 6578 744c 656e 6774  605.6" textLengt
-0000cf10: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000cf20: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000cf30: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000cf40: 652d 3234 2922 3e0a 3c2f 7465 7874 3e3c  e-24)">.</text><
-0000cf50: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000cf60: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000cf70: 7231 3522 2078 3d22 3130 3733 2e36 2220  r15" x="1073.6" 
-0000cf80: 793d 2236 3330 2220 7465 7874 4c65 6e67  y="630" textLeng
-0000cf90: 7468 3d22 3231 392e 3622 2063 6c69 702d  th="219.6" clip-
-0000cfa0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000cfb0: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000cfc0: 696e 652d 3235 2922 3e45 7874 7261 2623  ine-25)">Extra&#
-0000cfd0: 3136 303b 496e 7374 616c 6c61 7469 6f6e  160;Installation
-0000cfe0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000cff0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000d000: 3437 3539 3436 352d 7231 2220 783d 2231  4759465-r1" x="1
-0000d010: 3935 3222 2079 3d22 3633 3022 2074 6578  952" y="630" tex
-0000d020: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
-0000d030: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000d040: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000d050: 3635 2d6c 696e 652d 3235 2922 3e0a 3c2f  65-line-25)">.</
-0000d060: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000d070: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000d080: 3539 3436 352d 7231 2220 783d 2231 3935  59465-r1" x="195
-0000d090: 3222 2079 3d22 3635 342e 3422 2074 6578  2" y="654.4" tex
-0000d0a0: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
-0000d0b0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000d0c0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000d0d0: 3635 2d6c 696e 652d 3236 2922 3e0a 3c2f  65-line-26)">.</
-0000d0e0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000d0f0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000d100: 3539 3436 352d 7236 2220 783d 2234 3531  59465-r6" x="451
-0000d110: 2e34 2220 793d 2236 3738 2e38 2220 7465  .4" y="678.8" te
-0000d120: 7874 4c65 6e67 7468 3d22 3330 3522 2063  xtLength="305" c
-0000d130: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000d140: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000d150: 3635 2d6c 696e 652d 3237 2922 3e49 6626  65-line-27)">If&
-0000d160: 2331 3630 3b79 6f75 2623 7832 373b 7265  #160;you&#x27;re
-0000d170: 2623 3136 303b 6c6f 6f6b 696e 6726 2331  &#160;looking&#1
-0000d180: 3630 3b74 6f26 2331 3630 3b75 7365 2623  60;to&#160;use&#
-0000d190: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
-0000d1a0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000d1b0: 2d31 3732 3437 3539 3436 352d 7231 3322  -1724759465-r13"
-0000d1c0: 2078 3d22 3735 362e 3422 2079 3d22 3637   x="756.4" y="67
-0000d1d0: 382e 3822 2074 6578 744c 656e 6774 683d  8.8" textLength=
-0000d1e0: 2237 332e 3222 2063 6c69 702d 7061 7468  "73.2" clip-path
-0000d1f0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000d200: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000d210: 3237 2922 3e62 726f 7773 723c 2f74 6578  27)">browsr</tex
-0000d220: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000d230: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000d240: 3635 2d72 3622 2078 3d22 3832 392e 3622  65-r6" x="829.6"
-0000d250: 2079 3d22 3637 382e 3822 2074 6578 744c   y="678.8" textL
-0000d260: 656e 6774 683d 2237 3933 2220 636c 6970  ength="793" clip
-0000d270: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000d280: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000d290: 6c69 6e65 2d32 3729 223e 2623 3136 303b  line-27)">&#160;
-0000d2a0: 6f6e 2623 3136 303b 7265 6d6f 7465 2623  on&#160;remote&#
-0000d2b0: 3136 303b 6669 6c65 2623 3136 303b 7379  160;file&#160;sy
-0000d2c0: 7374 656d 732c 2623 3136 303b 6c69 6b65  stems,&#160;like
-0000d2d0: 2623 3136 303b 4157 5326 2331 3630 3b53  &#160;AWS&#160;S
-0000d2e0: 332c 2623 3136 303b 796f 7526 2378 3237  3,&#160;you&#x27
-0000d2f0: 3b6c 6c26 2331 3630 3b6e 6565 6426 2331  ;ll&#160;need&#1
-0000d300: 3630 3b74 6f26 2331 3630 3b69 6e73 7461  60;to&#160;insta
-0000d310: 6c6c 2623 3136 303b 7468 6526 2331 3630  ll&#160;the&#160
-0000d320: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-0000d330: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000d340: 3234 3735 3934 3635 2d72 3133 2220 783d  24759465-r13" x=
-0000d350: 2231 3632 322e 3622 2079 3d22 3637 382e  "1622.6" y="678.
-0000d360: 3822 2074 6578 744c 656e 6774 683d 2237  8" textLength="7
-0000d370: 332e 3222 2063 6c69 702d 7061 7468 3d22  3.2" clip-path="
-0000d380: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000d390: 3234 3735 3934 3635 2d6c 696e 652d 3237  24759465-line-27
-0000d3a0: 2922 3e72 656d 6f74 653c 2f74 6578 743e  )">remote</text>
-0000d3b0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-0000d3c0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000d3d0: 2d72 3622 2078 3d22 3136 3935 2e38 2220  -r6" x="1695.8" 
-0000d3e0: 793d 2236 3738 2e38 2220 7465 7874 4c65  y="678.8" textLe
-0000d3f0: 6e67 7468 3d22 3835 2e34 2220 636c 6970  ngth="85.4" clip
-0000d400: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000d410: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000d420: 6c69 6e65 2d32 3729 223e 2623 3136 303b  line-27)">&#160;
-0000d430: 6578 7472 612e 3c2f 7465 7874 3e3c 7465  extra.</text><te
-0000d440: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000d450: 616c 2d31 3732 3437 3539 3436 352d 7236  al-1724759465-r6
-0000d460: 2220 783d 2231 3739 332e 3422 2079 3d22  " x="1793.4" y="
-0000d470: 3637 382e 3822 2074 6578 744c 656e 6774  678.8" textLengt
-0000d480: 683d 2231 3039 2e38 2220 636c 6970 2d70  h="109.8" clip-p
-0000d490: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000d4a0: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000d4b0: 6e65 2d32 3729 223e 4966 2623 3136 303b  ne-27)">If&#160;
-0000d4c0: 796f 7526 2378 3237 3b64 2623 3136 303b  you&#x27;d&#160;
-0000d4d0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000d4e0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000d4f0: 3437 3539 3436 352d 7231 2220 783d 2231  4759465-r1" x="1
-0000d500: 3935 3222 2079 3d22 3637 382e 3822 2074  952" y="678.8" t
-0000d510: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
-0000d520: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000d530: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-0000d540: 3934 3635 2d6c 696e 652d 3237 2922 3e0a  9465-line-27)">.
-0000d550: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000d560: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000d570: 3437 3539 3436 352d 7236 2220 783d 2234  4759465-r6" x="4
-0000d580: 3531 2e34 2220 793d 2237 3033 2e32 2220  51.4" y="703.2" 
-0000d590: 7465 7874 4c65 6e67 7468 3d22 3639 352e  textLength="695.
-0000d5a0: 3422 2063 6c69 702d 7061 7468 3d22 7572  4" clip-path="ur
-0000d5b0: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000d5c0: 3735 3934 3635 2d6c 696e 652d 3238 2922  759465-line-28)"
-0000d5d0: 3e6c 696b 6526 2331 3630 3b74 6f26 2331  >like&#160;to&#1
-0000d5e0: 3630 3b62 726f 7773 6526 2331 3630 3b70  60;browse&#160;p
-0000d5f0: 6172 7175 6574 2623 3136 303b 6669 6c65  arquet&#160;file
-0000d600: 732c 2623 3136 303b 796f 7526 2378 3237  s,&#160;you&#x27
-0000d610: 3b6c 6c26 2331 3630 3b6e 6565 6426 2331  ;ll&#160;need&#1
-0000d620: 3630 3b74 6f26 2331 3630 3b69 6e73 7461  60;to&#160;insta
-0000d630: 6c6c 2623 3136 303b 7468 6526 2331 3630  ll&#160;the&#160
-0000d640: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-0000d650: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000d660: 3234 3735 3934 3635 2d72 3133 2220 783d  24759465-r13" x=
-0000d670: 2231 3134 362e 3822 2079 3d22 3730 332e  "1146.8" y="703.
-0000d680: 3222 2074 6578 744c 656e 6774 683d 2238  2" textLength="8
-0000d690: 352e 3422 2063 6c69 702d 7061 7468 3d22  5.4" clip-path="
-0000d6a0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000d6b0: 3234 3735 3934 3635 2d6c 696e 652d 3238  24759465-line-28
-0000d6c0: 2922 3e70 6172 7175 6574 3c2f 7465 7874  )">parquet</text
-0000d6d0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000d6e0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000d6f0: 352d 7236 2220 783d 2231 3233 322e 3222  5-r6" x="1232.2"
-0000d700: 2079 3d22 3730 332e 3222 2074 6578 744c   y="703.2" textL
-0000d710: 656e 6774 683d 2233 3035 2220 636c 6970  ength="305" clip
-0000d720: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000d730: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000d740: 6c69 6e65 2d32 3829 223e 2623 3136 303b  line-28)">&#160;
-0000d750: 6578 7472 612e 2623 3136 303b 4f72 2c26  extra.&#160;Or,&
-0000d760: 2331 3630 3b65 7665 6e26 2331 3630 3b73  #160;even&#160;s
-0000d770: 696d 706c 6572 2c3c 2f74 6578 743e 3c74  impler,</text><t
-0000d780: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000d790: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000d7a0: 3622 2078 3d22 3135 3439 2e34 2220 793d  6" x="1549.4" y=
-0000d7b0: 2237 3033 2e32 2220 7465 7874 4c65 6e67  "703.2" textLeng
-0000d7c0: 7468 3d22 3234 3422 2063 6c69 702d 7061  th="244" clip-pa
-0000d7d0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000d7e0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000d7f0: 652d 3238 2922 3e79 6f75 2623 3136 303b  e-28)">you&#160;
-0000d800: 6361 6e26 2331 3630 3b69 6e73 7461 6c6c  can&#160;install
-0000d810: 2623 3136 303b 7468 6526 2331 3630 3b3c  &#160;the&#160;<
-0000d820: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000d830: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000d840: 3735 3934 3635 2d72 3133 2220 783d 2231  759465-r13" x="1
-0000d850: 3739 332e 3422 2079 3d22 3730 332e 3222  793.4" y="703.2"
-0000d860: 2074 6578 744c 656e 6774 683d 2233 362e   textLength="36.
-0000d870: 3622 2063 6c69 702d 7061 7468 3d22 7572  6" clip-path="ur
-0000d880: 6c28 2374 6572 6d69 6e61 6c2d 3137 3234  l(#terminal-1724
-0000d890: 3735 3934 3635 2d6c 696e 652d 3238 2922  759465-line-28)"
-0000d8a0: 3e61 6c6c 3c2f 7465 7874 3e3c 7465 7874  >all</text><text
-0000d8b0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000d8c0: 2d31 3732 3437 3539 3436 352d 7236 2220  -1724759465-r6" 
-0000d8d0: 783d 2231 3833 3022 2079 3d22 3730 332e  x="1830" y="703.
-0000d8e0: 3222 2074 6578 744c 656e 6774 683d 2238  2" textLength="8
-0000d8f0: 352e 3422 2063 6c69 702d 7061 7468 3d22  5.4" clip-path="
-0000d900: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000d910: 3234 3735 3934 3635 2d6c 696e 652d 3238  24759465-line-28
-0000d920: 2922 3e26 2331 3630 3b65 7874 7261 2623  )">&#160;extra&#
-0000d930: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
-0000d940: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000d950: 2d31 3732 3437 3539 3436 352d 7231 2220  -1724759465-r1" 
-0000d960: 783d 2231 3935 3222 2079 3d22 3730 332e  x="1952" y="703.
-0000d970: 3222 2074 6578 744c 656e 6774 683d 2231  2" textLength="1
-0000d980: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
-0000d990: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000d9a0: 3234 3735 3934 3635 2d6c 696e 652d 3238  24759465-line-28
-0000d9b0: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000d9c0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000d9d0: 2d31 3732 3437 3539 3436 352d 7236 2220  -1724759465-r6" 
-0000d9e0: 783d 2234 3531 2e34 2220 793d 2237 3237  x="451.4" y="727
-0000d9f0: 2e36 2220 7465 7874 4c65 6e67 7468 3d22  .6" textLength="
-0000da00: 3236 382e 3422 2063 6c69 702d 7061 7468  268.4" clip-path
-0000da10: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000da20: 3137 3234 3735 3934 3635 2d6c 696e 652d  1724759465-line-
-0000da30: 3239 2922 3e74 6f26 2331 3630 3b67 6574  29)">to&#160;get
-0000da40: 2623 3136 303b 616c 6c26 2331 3630 3b74  &#160;all&#160;t
-0000da50: 6865 2623 3136 303b 6578 7472 6173 2e3c  he&#160;extras.<
-0000da60: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000da70: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000da80: 3735 3934 3635 2d72 3122 2078 3d22 3139  759465-r1" x="19
-0000da90: 3532 2220 793d 2237 3237 2e36 2220 7465  52" y="727.6" te
-0000daa0: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
-0000dab0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000dac0: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000dad0: 3436 352d 6c69 6e65 2d32 3929 223e 0a3c  465-line-29)">.<
-0000dae0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000daf0: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000db00: 3735 3934 3635 2d72 3122 2078 3d22 3139  759465-r1" x="19
-0000db10: 3532 2220 793d 2237 3532 2220 7465 7874  52" y="752" text
-0000db20: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000db30: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000db40: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000db50: 352d 6c69 6e65 2d33 3029 223e 0a3c 2f74  5-line-30)">.</t
-0000db60: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000db70: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000db80: 3934 3635 2d72 3122 2078 3d22 3139 3532  9465-r1" x="1952
-0000db90: 2220 793d 2237 3736 2e34 2220 7465 7874  " y="776.4" text
-0000dba0: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000dbb0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000dbc0: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000dbd0: 352d 6c69 6e65 2d33 3129 223e 0a3c 2f74  5-line-31)">.</t
-0000dbe0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000dbf0: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000dc00: 3934 3635 2d72 3136 2220 783d 2234 3633  9465-r16" x="463
-0000dc10: 2e36 2220 793d 2238 3030 2e38 2220 7465  .6" y="800.8" te
-0000dc20: 7874 4c65 6e67 7468 3d22 3438 2e38 2220  xtLength="48.8" 
-0000dc30: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000dc40: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000dc50: 3436 352d 6c69 6e65 2d33 3229 223e 7069  465-line-32)">pi
-0000dc60: 7078 3c2f 7465 7874 3e3c 7465 7874 2063  px</text><text c
-0000dc70: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000dc80: 3732 3437 3539 3436 352d 7231 3622 2078  724759465-r16" x
-0000dc90: 3d22 3532 342e 3622 2079 3d22 3830 302e  ="524.6" y="800.
-0000dca0: 3822 2074 6578 744c 656e 6774 683d 2238  8" textLength="8
-0000dcb0: 352e 3422 2063 6c69 702d 7061 7468 3d22  5.4" clip-path="
-0000dcc0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000dcd0: 3234 3735 3934 3635 2d6c 696e 652d 3332  24759465-line-32
-0000dce0: 2922 3e69 6e73 7461 6c6c 3c2f 7465 7874  )">install</text
-0000dcf0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000dd00: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000dd10: 352d 7231 3722 2078 3d22 3632 322e 3222  5-r17" x="622.2"
-0000dd20: 2079 3d22 3830 302e 3822 2074 6578 744c   y="800.8" textL
-0000dd30: 656e 6774 683d 2231 3538 2e36 2220 636c  ength="158.6" cl
-0000dd40: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000dd50: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000dd60: 352d 6c69 6e65 2d33 3229 223e 2671 756f  5-line-32)">&quo
-0000dd70: 743b 6272 6f77 7372 5b61 6c6c 5d26 7175  t;browsr[all]&qu
-0000dd80: 6f74 3b3c 2f74 6578 743e 3c74 6578 7420  ot;</text><text 
-0000dd90: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000dda0: 3137 3234 3735 3934 3635 2d72 3122 2078  1724759465-r1" x
-0000ddb0: 3d22 3139 3532 2220 793d 2238 3030 2e38  ="1952" y="800.8
-0000ddc0: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000ddd0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000dde0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000ddf0: 3437 3539 3436 352d 6c69 6e65 2d33 3229  4759465-line-32)
-0000de00: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
-0000de10: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000de20: 3137 3234 3735 3934 3635 2d72 3122 2078  1724759465-r1" x
-0000de30: 3d22 3139 3532 2220 793d 2238 3235 2e32  ="1952" y="825.2
-0000de40: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000de50: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000de60: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000de70: 3437 3539 3436 352d 6c69 6e65 2d33 3329  4759465-line-33)
-0000de80: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
-0000de90: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000dea0: 3137 3234 3735 3934 3635 2d72 3122 2078  1724759465-r1" x
-0000deb0: 3d22 3139 3532 2220 793d 2238 3439 2e36  ="1952" y="849.6
-0000dec0: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000ded0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000dee0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000def0: 3437 3539 3436 352d 6c69 6e65 2d33 3429  4759465-line-34)
-0000df00: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
-0000df10: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000df20: 3137 3234 3735 3934 3635 2d72 3122 2078  1724759465-r1" x
-0000df30: 3d22 3139 3532 2220 793d 2238 3734 2220  ="1952" y="874" 
-0000df40: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-0000df50: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000df60: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-0000df70: 3539 3436 352d 6c69 6e65 2d33 3529 223e  59465-line-35)">
-0000df80: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
-0000df90: 6173 733d 2274 6572 6d69 6e61 6c2d 3137  ass="terminal-17
-0000dfa0: 3234 3735 3934 3635 2d72 3135 2220 783d  24759465-r15" x=
-0000dfb0: 2231 3135 3922 2079 3d22 3839 382e 3422  "1159" y="898.4"
-0000dfc0: 2074 6578 744c 656e 6774 683d 2236 3122   textLength="61"
-0000dfd0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000dfe0: 2374 6572 6d69 6e61 6c2d 3137 3234 3735  #terminal-172475
-0000dff0: 3934 3635 2d6c 696e 652d 3336 2922 3e55  9465-line-36)">U
-0000e000: 7361 6765 3c2f 7465 7874 3e3c 7465 7874  sage</text><text
-0000e010: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000e020: 2d31 3732 3437 3539 3436 352d 7231 2220  -1724759465-r1" 
-0000e030: 783d 2231 3935 3222 2079 3d22 3839 382e  x="1952" y="898.
-0000e040: 3422 2074 6578 744c 656e 6774 683d 2231  4" textLength="1
-0000e050: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
-0000e060: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000e070: 3234 3735 3934 3635 2d6c 696e 652d 3336  24759465-line-36
-0000e080: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000e090: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000e0a0: 2d31 3732 3437 3539 3436 352d 7231 2220  -1724759465-r1" 
-0000e0b0: 783d 2231 3935 3222 2079 3d22 3932 322e  x="1952" y="922.
-0000e0c0: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
-0000e0d0: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
-0000e0e0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000e0f0: 3234 3735 3934 3635 2d6c 696e 652d 3337  24759465-line-37
-0000e100: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000e110: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000e120: 2d31 3732 3437 3539 3436 352d 7231 3822  -1724759465-r18"
-0000e130: 2078 3d22 3139 3237 2e36 2220 793d 2239   x="1927.6" y="9
-0000e140: 3437 2e32 2220 7465 7874 4c65 6e67 7468  47.2" textLength
-0000e150: 3d22 3234 2e34 2220 636c 6970 2d70 6174  ="24.4" clip-pat
-0000e160: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000e170: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000e180: 2d33 3829 223e e296 84e2 9684 3c2f 7465  -38)">......</te
-0000e190: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000e1a0: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000e1b0: 3436 352d 7231 2220 783d 2231 3935 3222  465-r1" x="1952"
-0000e1c0: 2079 3d22 3934 372e 3222 2074 6578 744c   y="947.2" textL
-0000e1d0: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
-0000e1e0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000e1f0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000e200: 2d6c 696e 652d 3338 2922 3e0a 3c2f 7465  -line-38)">.</te
-0000e210: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000e220: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000e230: 3436 352d 7231 3622 2078 3d22 3436 332e  465-r16" x="463.
-0000e240: 3622 2079 3d22 3937 312e 3622 2074 6578  6" y="971.6" tex
-0000e250: 744c 656e 6774 683d 2237 332e 3222 2063  tLength="73.2" c
-0000e260: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000e270: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000e280: 3635 2d6c 696e 652d 3339 2922 3e62 726f  65-line-39)">bro
-0000e290: 7773 723c 2f74 6578 743e 3c74 6578 7420  wsr</text><text 
-0000e2a0: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000e2b0: 3137 3234 3735 3934 3635 2d72 3136 2220  1724759465-r16" 
-0000e2c0: 783d 2235 3439 2220 793d 2239 3731 2e36  x="549" y="971.6
-0000e2d0: 2220 7465 7874 4c65 6e67 7468 3d22 3134  " textLength="14
-0000e2e0: 362e 3422 2063 6c69 702d 7061 7468 3d22  6.4" clip-path="
-0000e2f0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3137  url(#terminal-17
-0000e300: 3234 3735 3934 3635 2d6c 696e 652d 3339  24759465-line-39
-0000e310: 2922 3e7e 2f44 6f77 6e6c 6f61 6473 2f3c  )">~/Downloads/<
-0000e320: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000e330: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000e340: 3735 3934 3635 2d72 3122 2078 3d22 3139  759465-r1" x="19
-0000e350: 3532 2220 793d 2239 3731 2e36 2220 7465  52" y="971.6" te
-0000e360: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
-0000e370: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000e380: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000e390: 3436 352d 6c69 6e65 2d33 3929 223e 0a3c  465-line-39)">.<
-0000e3a0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000e3b0: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000e3c0: 3735 3934 3635 2d72 3122 2078 3d22 3139  759465-r1" x="19
-0000e3d0: 3532 2220 793d 2239 3936 2220 7465 7874  52" y="996" text
-0000e3e0: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000e3f0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000e400: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000e410: 352d 6c69 6e65 2d34 3029 223e 0a3c 2f74  5-line-40)">.</t
-0000e420: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000e430: 2274 6572 6d69 6e61 6c2d 3137 3234 3735  "terminal-172475
-0000e440: 3934 3635 2d72 3122 2078 3d22 3139 3532  9465-r1" x="1952
-0000e450: 2220 793d 2231 3032 302e 3422 2074 6578  " y="1020.4" tex
-0000e460: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
-0000e470: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-0000e480: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000e490: 3635 2d6c 696e 652d 3431 2922 3e0a 3c2f  65-line-41)">.</
-0000e4a0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000e4b0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000e4c0: 3539 3436 352d 7236 2220 783d 2234 3531  59465-r6" x="451
-0000e4d0: 2e34 2220 793d 2231 3034 342e 3822 2074  .4" y="1044.8" t
-0000e4e0: 6578 744c 656e 6774 683d 2231 3436 2e34  extLength="146.4
-0000e4f0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000e500: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-0000e510: 3539 3436 352d 6c69 6e65 2d34 3229 223e  59465-line-42)">
-0000e520: 5369 6d70 6c79 2623 3136 303b 6769 7665  Simply&#160;give
-0000e530: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000e540: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000e550: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000e560: 3322 2078 3d22 3539 372e 3822 2079 3d22  3" x="597.8" y="
-0000e570: 3130 3434 2e38 2220 7465 7874 4c65 6e67  1044.8" textLeng
-0000e580: 7468 3d22 3733 2e32 2220 636c 6970 2d70  th="73.2" clip-p
-0000e590: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000e5a0: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000e5b0: 6e65 2d34 3229 223e 6272 6f77 7372 3c2f  ne-42)">browsr</
-0000e5c0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000e5d0: 3d22 7465 726d 696e 616c 2d31 3732 3437  ="terminal-17247
-0000e5e0: 3539 3436 352d 7236 2220 783d 2236 3731  59465-r6" x="671
-0000e5f0: 2220 793d 2231 3034 342e 3822 2074 6578  " y="1044.8" tex
-0000e600: 744c 656e 6774 683d 2237 3434 2e32 2220  tLength="744.2" 
-0000e610: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000e620: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000e630: 3436 352d 6c69 6e65 2d34 3229 223e 2623  465-line-42)">&#
-0000e640: 3136 303b 6126 2331 3630 3b70 6174 6826  160;a&#160;path&
-0000e650: 2331 3630 3b74 6f26 2331 3630 3b61 2623  #160;to&#160;a&#
-0000e660: 3136 303b 6669 6c65 2f64 6972 6563 746f  160;file/directo
-0000e670: 7279 2623 3136 303b 616e 6426 2331 3630  ry&#160;and&#160
-0000e680: 3b69 7426 2331 3630 3b77 696c 6c26 2331  ;it&#160;will&#1
-0000e690: 3630 3b6f 7065 6e26 2331 3630 3b61 2623  60;open&#160;a&#
-0000e6a0: 3136 303b 6272 6f77 7365 7226 2331 3630  160;browser&#160
-0000e6b0: 3b77 696e 646f 773c 2f74 6578 743e 3c74  ;window</text><t
-0000e6c0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000e6d0: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000e6e0: 3622 2078 3d22 3134 3237 2e34 2220 793d  6" x="1427.4" y=
-0000e6f0: 2231 3034 342e 3822 2074 6578 744c 656e  "1044.8" textLen
-0000e700: 6774 683d 2235 3030 2e32 2220 636c 6970  gth="500.2" clip
-0000e710: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000e720: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000e730: 6c69 6e65 2d34 3229 223e 7769 7468 2623  line-42)">with&#
-0000e740: 3136 303b 6126 2331 3630 3b66 696c 6526  160;a&#160;file&
-0000e750: 2331 3630 3b62 726f 7773 6572 2e26 2331  #160;browser.&#1
-0000e760: 3630 3b59 6f75 2623 3136 303b 6361 6e26  60;You&#160;can&
-0000e770: 2331 3630 3b61 6c73 6f26 2331 3630 3b67  #160;also&#160;g
-0000e780: 6976 6526 2331 3630 3b69 743c 2f74 6578  ive&#160;it</tex
-0000e790: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000e7a0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000e7b0: 3635 2d72 3122 2078 3d22 3139 3532 2220  65-r1" x="1952" 
-0000e7c0: 793d 2231 3034 342e 3822 2074 6578 744c  y="1044.8" textL
-0000e7d0: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
-0000e7e0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000e7f0: 6d69 6e61 6c2d 3137 3234 3735 3934 3635  minal-1724759465
-0000e800: 2d6c 696e 652d 3432 2922 3e0a 3c2f 7465  -line-42)">.</te
-0000e810: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000e820: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000e830: 3436 352d 7236 2220 783d 2234 3531 2e34  465-r6" x="451.4
-0000e840: 2220 793d 2231 3036 392e 3222 2074 6578  " y="1069.2" tex
-0000e850: 744c 656e 6774 683d 2235 3234 2e36 2220  tLength="524.6" 
-0000e860: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000e870: 7465 726d 696e 616c 2d31 3732 3437 3539  terminal-1724759
-0000e880: 3436 352d 6c69 6e65 2d34 3329 223e 6126  465-line-43)">a&
-0000e890: 2331 3630 3b55 524c 2623 3136 303b 746f  #160;URL&#160;to
-0000e8a0: 2623 3136 303b 6126 2331 3630 3b72 656d  &#160;a&#160;rem
-0000e8b0: 6f74 6526 2331 3630 3b66 696c 6526 2331  ote&#160;file&#1
-0000e8c0: 3630 3b73 7973 7465 6d2c 2623 3136 303b  60;system,&#160;
-0000e8d0: 6c69 6b65 2623 3136 303b 4157 5326 2331  like&#160;AWS&#1
-0000e8e0: 3630 3b53 332e 3c2f 7465 7874 3e3c 7465  60;S3.</text><te
-0000e8f0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000e900: 616c 2d31 3732 3437 3539 3436 352d 7231  al-1724759465-r1
-0000e910: 2220 783d 2231 3935 3222 2079 3d22 3130  " x="1952" y="10
-0000e920: 3639 2e32 2220 7465 7874 4c65 6e67 7468  69.2" textLength
-0000e930: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000e940: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000e950: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000e960: 2d34 3329 223e 0a3c 2f74 6578 743e 3c74  -43)">.</text><t
-0000e970: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000e980: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000e990: 3122 2078 3d22 3139 3532 2220 793d 2231  1" x="1952" y="1
-0000e9a0: 3039 332e 3622 2074 6578 744c 656e 6774  093.6" textLengt
-0000e9b0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
-0000e9c0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000e9d0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000e9e0: 652d 3434 2922 3e0a 3c2f 7465 7874 3e3c  e-44)">.</text><
-0000e9f0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000ea00: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000ea10: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000ea20: 3131 3138 2220 7465 7874 4c65 6e67 7468  1118" textLength
-0000ea30: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000ea40: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000ea50: 2d31 3732 3437 3539 3436 352d 6c69 6e65  -1724759465-line
-0000ea60: 2d34 3529 223e 0a3c 2f74 6578 743e 3c74  -45)">.</text><t
-0000ea70: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000ea80: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000ea90: 3139 2220 783d 2231 322e 3222 2079 3d22  19" x="12.2" y="
-0000eaa0: 3131 3432 2e34 2220 7465 7874 4c65 6e67  1142.4" textLeng
-0000eab0: 7468 3d22 3538 352e 3622 2063 6c69 702d  th="585.6" clip-
-0000eac0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000ead0: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000eae0: 696e 652d 3436 2922 3ef0 9f97 84ef b88f  ine-46)">.......
-0000eaf0: efb8 8fef b88f 2623 3136 303b 2623 3136  ......&#160;&#16
-0000eb00: 303b 334b 4226 2331 3630 3b26 2331 3630  0;3KB&#160;&#160
-0000eb10: 3bf0 9f92 be26 2331 3630 3b26 2331 3630  ;....&#160;&#160
-0000eb20: 3b52 4541 444d 452e 6d64 2623 3136 303b  ;README.md&#160;
-0000eb30: 2623 3136 303b f09f 9382 2623 3136 303b  &#160;....&#160;
-0000eb40: 2623 3136 303b 6a75 6674 696e 3a62 726f  &#160;juftin:bro
-0000eb50: 7773 7240 7631 2e36 2e30 3c2f 7465 7874  wsr@v1.6.0</text
-0000eb60: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000eb70: 726d 696e 616c 2d31 3732 3437 3539 3436  rminal-172475946
-0000eb80: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
-0000eb90: 3d22 3131 3432 2e34 2220 7465 7874 4c65  ="1142.4" textLe
-0000eba0: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
-0000ebb0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000ebc0: 696e 616c 2d31 3732 3437 3539 3436 352d  inal-1724759465-
-0000ebd0: 6c69 6e65 2d34 3629 223e 0a3c 2f74 6578  line-46)">.</tex
-0000ebe0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000ebf0: 6572 6d69 6e61 6c2d 3137 3234 3735 3934  erminal-17247594
-0000ec00: 3635 2d72 3230 2220 783d 2230 2220 793d  65-r20" x="0" y=
-0000ec10: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
-0000ec20: 6774 683d 2233 362e 3622 2063 6c69 702d  gth="36.6" clip-
-0000ec30: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000ec40: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000ec50: 696e 652d 3437 2922 3e26 2331 3630 3b51  ine-47)">&#160;Q
-0000ec60: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000ec70: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000ec80: 616c 2d31 3732 3437 3539 3436 352d 7232  al-1724759465-r2
-0000ec90: 3122 2078 3d22 3336 2e36 2220 793d 2231  1" x="36.6" y="1
-0000eca0: 3136 362e 3822 2074 6578 744c 656e 6774  166.8" textLengt
-0000ecb0: 683d 2237 332e 3222 2063 6c69 702d 7061  h="73.2" clip-pa
-0000ecc0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000ecd0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000ece0: 652d 3437 2922 3e26 2331 3630 3b51 7569  e-47)">&#160;Qui
-0000ecf0: 7426 2331 3630 3b3c 2f74 6578 743e 3c74  t&#160;</text><t
-0000ed00: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-0000ed10: 6e61 6c2d 3137 3234 3735 3934 3635 2d72  nal-1724759465-r
-0000ed20: 3230 2220 783d 2231 3039 2e38 2220 793d  20" x="109.8" y=
-0000ed30: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
-0000ed40: 6774 683d 2233 362e 3622 2063 6c69 702d  gth="36.6" clip-
-0000ed50: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000ed60: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000ed70: 696e 652d 3437 2922 3e26 2331 3630 3b46  ine-47)">&#160;F
-0000ed80: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000ed90: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000eda0: 616c 2d31 3732 3437 3539 3436 352d 7232  al-1724759465-r2
-0000edb0: 3122 2078 3d22 3134 362e 3422 2079 3d22  1" x="146.4" y="
-0000edc0: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
-0000edd0: 7468 3d22 3137 302e 3822 2063 6c69 702d  th="170.8" clip-
-0000ede0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000edf0: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000ee00: 696e 652d 3437 2922 3e26 2331 3630 3b54  ine-47)">&#160;T
-0000ee10: 6f67 676c 6526 2331 3630 3b46 696c 6573  oggle&#160;Files
-0000ee20: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000ee30: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000ee40: 616c 2d31 3732 3437 3539 3436 352d 7232  al-1724759465-r2
-0000ee50: 3022 2078 3d22 3331 372e 3222 2079 3d22  0" x="317.2" y="
-0000ee60: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
-0000ee70: 7468 3d22 3336 2e36 2220 636c 6970 2d70  th="36.6" clip-p
-0000ee80: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000ee90: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000eea0: 6e65 2d34 3729 223e 2623 3136 303b 5426  ne-47)">&#160;T&
-0000eeb0: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
-0000eec0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000eed0: 6c2d 3137 3234 3735 3934 3635 2d72 3231  l-1724759465-r21
-0000eee0: 2220 783d 2233 3533 2e38 2220 793d 2231  " x="353.8" y="1
-0000eef0: 3136 362e 3822 2074 6578 744c 656e 6774  166.8" textLengt
-0000ef00: 683d 2231 3730 2e38 2220 636c 6970 2d70  h="170.8" clip-p
-0000ef10: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000ef20: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000ef30: 6e65 2d34 3729 223e 2623 3136 303b 546f  ne-47)">&#160;To
-0000ef40: 6767 6c65 2623 3136 303b 5468 656d 6526  ggle&#160;Theme&
-0000ef50: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
-0000ef60: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000ef70: 6c2d 3137 3234 3735 3934 3635 2d72 3230  l-1724759465-r20
-0000ef80: 2220 783d 2235 3234 2e36 2220 793d 2231  " x="524.6" y="1
-0000ef90: 3136 362e 3822 2074 6578 744c 656e 6774  166.8" textLengt
-0000efa0: 683d 2233 362e 3622 2063 6c69 702d 7061  h="36.6" clip-pa
-0000efb0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000efc0: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000efd0: 652d 3437 2922 3e26 2331 3630 3b4e 2623  e-47)">&#160;N&#
-0000efe0: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
-0000eff0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000f000: 2d31 3732 3437 3539 3436 352d 7232 3122  -1724759465-r21"
-0000f010: 2078 3d22 3536 312e 3222 2079 3d22 3131   x="561.2" y="11
-0000f020: 3636 2e38 2220 7465 7874 4c65 6e67 7468  66.8" textLength
-0000f030: 3d22 3235 362e 3222 2063 6c69 702d 7061  ="256.2" clip-pa
-0000f040: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000f050: 6c2d 3137 3234 3735 3934 3635 2d6c 696e  l-1724759465-lin
-0000f060: 652d 3437 2922 3e26 2331 3630 3b54 6f67  e-47)">&#160;Tog
-0000f070: 676c 6526 2331 3630 3b4c 696e 6526 2331  gle&#160;Line&#1
-0000f080: 3630 3b4e 756d 6265 7273 2623 3136 303b  60;Numbers&#160;
-0000f090: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000f0a0: 7373 3d22 7465 726d 696e 616c 2d31 3732  ss="terminal-172
-0000f0b0: 3437 3539 3436 352d 7232 3022 2078 3d22  4759465-r20" x="
-0000f0c0: 3831 372e 3422 2079 3d22 3131 3636 2e38  817.4" y="1166.8
-0000f0d0: 2220 7465 7874 4c65 6e67 7468 3d22 3336  " textLength="36
-0000f0e0: 2e36 2220 636c 6970 2d70 6174 683d 2275  .6" clip-path="u
-0000f0f0: 726c 2823 7465 726d 696e 616c 2d31 3732  rl(#terminal-172
-0000f100: 3437 3539 3436 352d 6c69 6e65 2d34 3729  4759465-line-47)
-0000f110: 223e 2623 3136 303b 4426 2331 3630 3b3c  ">&#160;D&#160;<
-0000f120: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000f130: 733d 2274 6572 6d69 6e61 6c2d 3137 3234  s="terminal-1724
-0000f140: 3735 3934 3635 2d72 3231 2220 783d 2238  759465-r21" x="8
-0000f150: 3534 2220 793d 2231 3136 362e 3822 2074  54" y="1166.8" t
-0000f160: 6578 744c 656e 6774 683d 2232 3139 2e36  extLength="219.6
-0000f170: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000f180: 2823 7465 726d 696e 616c 2d31 3732 3437  (#terminal-17247
-0000f190: 3539 3436 352d 6c69 6e65 2d34 3729 223e  59465-line-47)">
-0000f1a0: 2623 3136 303b 546f 6767 6c65 2623 3136  &#160;Toggle&#16
-0000f1b0: 303b 4461 726b 2623 3136 303b 4d6f 6465  0;Dark&#160;Mode
-0000f1c0: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000f1d0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000f1e0: 616c 2d31 3732 3437 3539 3436 352d 7232  al-1724759465-r2
-0000f1f0: 3022 2078 3d22 3130 3733 2e36 2220 793d  0" x="1073.6" y=
-0000f200: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
-0000f210: 6774 683d 2233 362e 3622 2063 6c69 702d  gth="36.6" clip-
-0000f220: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000f230: 6e61 6c2d 3137 3234 3735 3934 3635 2d6c  nal-1724759465-l
-0000f240: 696e 652d 3437 2922 3e26 2331 3630 3b58  ine-47)">&#160;X
-0000f250: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000f260: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000f270: 616c 2d31 3732 3437 3539 3436 352d 7232  al-1724759465-r2
-0000f280: 3122 2078 3d22 3131 3130 2e32 2220 793d  1" x="1110.2" y=
-0000f290: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
-0000f2a0: 6774 683d 2231 3833 2220 636c 6970 2d70  gth="183" clip-p
-0000f2b0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000f2c0: 616c 2d31 3732 3437 3539 3436 352d 6c69  al-1724759465-li
-0000f2d0: 6e65 2d34 3729 223e 2623 3136 303b 446f  ne-47)">&#160;Do
-0000f2e0: 776e 6c6f 6164 2623 3136 303b 4669 6c65  wnload&#160;File
-0000f2f0: 2623 3136 303b 3c2f 7465 7874 3e0a 2020  &#160;</text>.  
-0000f300: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
-0000f310: 3c2f 7376 673e 0a                        </svg>.
+0000b320: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000b330: 3831 3336 302d 7231 2220 783d 2231 3935  81360-r1" x="195
+0000b340: 3222 2079 3d22 3231 352e 3222 2074 6578  2" y="215.2" tex
+0000b350: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+0000b360: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000b370: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000b380: 3630 2d6c 696e 652d 3829 223e 0a3c 2f74  60-line-8)">.</t
+0000b390: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000b3a0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000b3b0: 3133 3630 2d72 3722 2078 3d22 3022 2079  1360-r7" x="0" y
+0000b3c0: 3d22 3233 392e 3622 2074 6578 744c 656e  ="239.6" textLen
+0000b3d0: 6774 683d 2234 382e 3822 2063 6c69 702d  gth="48.8" clip-
+0000b3e0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000b3f0: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000b400: 696e 652d 3929 223e e294 a3e2 9481 e294  ine-9)">........
+0000b410: 8126 2331 3630 3b3c 2f74 6578 743e 3c74  .&#160;</text><t
+0000b420: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000b430: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000b440: 3422 2078 3d22 3438 2e38 2220 793d 2232  4" x="48.8" y="2
+0000b450: 3339 2e36 2220 7465 7874 4c65 6e67 7468  39.6" textLength
+0000b460: 3d22 3234 2e34 2220 636c 6970 2d70 6174  ="24.4" clip-pat
+0000b470: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000b480: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000b490: 2d39 2922 3ef0 9f93 8426 2331 3630 3b3c  -9)">....&#160;<
+0000b4a0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000b4b0: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000b4c0: 3038 3133 3630 2d72 3132 2220 783d 2238  081360-r12" x="8
+0000b4d0: 352e 3422 2079 3d22 3233 392e 3622 2074  5.4" y="239.6" t
+0000b4e0: 6578 744c 656e 6774 683d 2231 3538 2e36  extLength="158.6
+0000b4f0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+0000b500: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+0000b510: 3831 3336 302d 6c69 6e65 2d39 2922 3e2e  81360-line-9)">.
+0000b520: 7265 6c65 6173 6572 632e 6a73 3c2f 7465  releaserc.js</te
+0000b530: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000b540: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000b550: 3336 302d 7236 2220 783d 2234 3531 2e34  360-r6" x="451.4
+0000b560: 2220 793d 2232 3339 2e36 2220 7465 7874  " y="239.6" text
+0000b570: 4c65 6e67 7468 3d22 3436 332e 3622 2063  Length="463.6" c
+0000b580: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000b590: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000b5a0: 3630 2d6c 696e 652d 3929 223e 7461 6b65  60-line-9)">take
+0000b5b0: 2623 3136 303b 6126 2331 3630 3b70 6565  &#160;a&#160;pee
+0000b5c0: 6b26 2331 3630 3b61 7426 2331 3630 3b74  k&#160;at&#160;t
+0000b5d0: 6865 6972 2623 3136 303b 636f 6e74 656e  heir&#160;conten
+0000b5e0: 7473 2e26 2331 3630 3b50 6c75 7326 2331  ts.&#160;Plus&#1
+0000b5f0: 3630 3b69 743c 2f74 6578 743e 3c74 6578  60;it</text><tex
+0000b600: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000b610: 6c2d 3231 3637 3038 3133 3630 2d72 3622  l-2167081360-r6"
+0000b620: 2078 3d22 3932 372e 3222 2079 3d22 3233   x="927.2" y="23
+0000b630: 392e 3622 2074 6578 744c 656e 6774 683d  9.6" textLength=
+0000b640: 2234 3735 2e38 2220 636c 6970 2d70 6174  "475.8" clip-pat
+0000b650: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000b660: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000b670: 2d39 2922 3e77 6f72 6b73 2623 3136 303b  -9)">works&#160;
+0000b680: 6f6e 2623 3136 303b 6c6f 6361 6c26 2331  on&#160;local&#1
+0000b690: 3630 3b61 6e64 2623 3136 303b 7265 6d6f  60;and&#160;remo
+0000b6a0: 7465 2623 3136 303b 6669 6c65 2623 3136  te&#160;file&#16
+0000b6b0: 303b 7379 7374 656d 732e 3c2f 7465 7874  0;systems.</text
+0000b6c0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+0000b6d0: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000b6e0: 302d 7231 2220 783d 2231 3935 3222 2079  0-r1" x="1952" y
+0000b6f0: 3d22 3233 392e 3622 2074 6578 744c 656e  ="239.6" textLen
+0000b700: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
+0000b710: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000b720: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000b730: 696e 652d 3929 223e 0a3c 2f74 6578 743e  ine-9)">.</text>
+0000b740: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000b750: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000b760: 2d72 3722 2078 3d22 3022 2079 3d22 3236  -r7" x="0" y="26
+0000b770: 3422 2074 6578 744c 656e 6774 683d 2234  4" textLength="4
+0000b780: 382e 3822 2063 6c69 702d 7061 7468 3d22  8.8" clip-path="
+0000b790: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000b7a0: 3637 3038 3133 3630 2d6c 696e 652d 3130  67081360-line-10
+0000b7b0: 2922 3ee2 94a3 e294 81e2 9481 2623 3136  )">.........&#16
+0000b7c0: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
+0000b7d0: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000b7e0: 3136 3730 3831 3336 302d 7234 2220 783d  167081360-r4" x=
+0000b7f0: 2234 382e 3822 2079 3d22 3236 3422 2074  "48.8" y="264" t
+0000b800: 6578 744c 656e 6774 683d 2232 342e 3422  extLength="24.4"
+0000b810: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000b820: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000b830: 3133 3630 2d6c 696e 652d 3130 2922 3ef0  1360-line-10)">.
+0000b840: 9f93 8426 2331 3630 3b3c 2f74 6578 743e  ...&#160;</text>
+0000b850: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000b860: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000b870: 2d72 3422 2078 3d22 3835 2e34 2220 793d  -r4" x="85.4" y=
+0000b880: 2232 3634 2220 7465 7874 4c65 6e67 7468  "264" textLength
+0000b890: 3d22 3835 2e34 2220 636c 6970 2d70 6174  ="85.4" clip-pat
+0000b8a0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000b8b0: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000b8c0: 2d31 3029 223e 4c49 4345 4e53 453c 2f74  -10)">LICENSE</t
+0000b8d0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000b8e0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000b8f0: 3133 3630 2d72 3122 2078 3d22 3139 3532  1360-r1" x="1952
+0000b900: 2220 793d 2232 3634 2220 7465 7874 4c65  " y="264" textLe
+0000b910: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
+0000b920: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000b930: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000b940: 6c69 6e65 2d31 3029 223e 0a3c 2f74 6578  line-10)">.</tex
+0000b950: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000b960: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000b970: 3630 2d72 3722 2078 3d22 3022 2079 3d22  60-r7" x="0" y="
+0000b980: 3238 382e 3422 2074 6578 744c 656e 6774  288.4" textLengt
+0000b990: 683d 2234 382e 3822 2063 6c69 702d 7061  h="48.8" clip-pa
+0000b9a0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000b9b0: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000b9c0: 652d 3131 2922 3ee2 94a3 e294 81e2 9481  e-11)">.........
+0000b9d0: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
+0000b9e0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000b9f0: 616c 2d32 3136 3730 3831 3336 302d 7234  al-2167081360-r4
+0000ba00: 2220 783d 2234 382e 3822 2079 3d22 3238  " x="48.8" y="28
+0000ba10: 382e 3422 2074 6578 744c 656e 6774 683d  8.4" textLength=
+0000ba20: 2232 342e 3422 2063 6c69 702d 7061 7468  "24.4" clip-path
+0000ba30: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000ba40: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000ba50: 3131 2922 3ef0 9f93 8426 2331 3630 3b3c  11)">....&#160;<
+0000ba60: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000ba70: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000ba80: 3038 3133 3630 2d72 3422 2078 3d22 3835  081360-r4" x="85
+0000ba90: 2e34 2220 793d 2232 3838 2e34 2220 7465  .4" y="288.4" te
+0000baa0: 7874 4c65 6e67 7468 3d22 3733 2e32 2220  xtLength="73.2" 
+0000bab0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000bac0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000bad0: 3336 302d 6c69 6e65 2d31 3129 223e 6d6b  360-line-11)">mk
+0000bae0: 646f 6373 3c2f 7465 7874 3e3c 7465 7874  docs</text><text
+0000baf0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000bb00: 2d32 3136 3730 3831 3336 302d 7231 3422  -2167081360-r14"
+0000bb10: 2078 3d22 3135 382e 3622 2079 3d22 3238   x="158.6" y="28
+0000bb20: 382e 3422 2074 6578 744c 656e 6774 683d  8.4" textLength=
+0000bb30: 2236 3122 2063 6c69 702d 7061 7468 3d22  "61" clip-path="
+0000bb40: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000bb50: 3637 3038 3133 3630 2d6c 696e 652d 3131  67081360-line-11
+0000bb60: 2922 3e2e 7961 6d6c 3c2f 7465 7874 3e3c  )">.yaml</text><
+0000bb70: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000bb80: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000bb90: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
+0000bba0: 3238 382e 3422 2074 6578 744c 656e 6774  288.4" textLengt
+0000bbb0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000bbc0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000bbd0: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000bbe0: 652d 3131 2922 3e0a 3c2f 7465 7874 3e3c  e-11)">.</text><
+0000bbf0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000bc00: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000bc10: 7237 2220 783d 2230 2220 793d 2233 3132  r7" x="0" y="312
+0000bc20: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
+0000bc30: 3438 2e38 2220 636c 6970 2d70 6174 683d  48.8" clip-path=
+0000bc40: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000bc50: 3136 3730 3831 3336 302d 6c69 6e65 2d31  167081360-line-1
+0000bc60: 3229 223e e294 a3e2 9481 e294 8126 2331  2)">.........&#1
+0000bc70: 3630 3b3c 2f74 6578 743e 3c74 6578 7420  60;</text><text 
+0000bc80: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000bc90: 3231 3637 3038 3133 3630 2d72 3422 2078  2167081360-r4" x
+0000bca0: 3d22 3438 2e38 2220 793d 2233 3132 2e38  ="48.8" y="312.8
+0000bcb0: 2220 7465 7874 4c65 6e67 7468 3d22 3234  " textLength="24
+0000bcc0: 2e34 2220 636c 6970 2d70 6174 683d 2275  .4" clip-path="u
+0000bcd0: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000bce0: 3730 3831 3336 302d 6c69 6e65 2d31 3229  7081360-line-12)
+0000bcf0: 223e f09f 9384 2623 3136 303b 3c2f 7465  ">....&#160;</te
+0000bd00: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000bd10: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000bd20: 3336 302d 7234 2220 783d 2238 352e 3422  360-r4" x="85.4"
+0000bd30: 2079 3d22 3331 322e 3822 2074 6578 744c   y="312.8" textL
+0000bd40: 656e 6774 683d 2231 3039 2e38 2220 636c  ength="109.8" cl
+0000bd50: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000bd60: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000bd70: 302d 6c69 6e65 2d31 3229 223e 7079 7072  0-line-12)">pypr
+0000bd80: 6f6a 6563 743c 2f74 6578 743e 3c74 6578  oject</text><tex
+0000bd90: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000bda0: 6c2d 3231 3637 3038 3133 3630 2d72 3134  l-2167081360-r14
+0000bdb0: 2220 783d 2231 3935 2e32 2220 793d 2233  " x="195.2" y="3
+0000bdc0: 3132 2e38 2220 7465 7874 4c65 6e67 7468  12.8" textLength
+0000bdd0: 3d22 3631 2220 636c 6970 2d70 6174 683d  ="61" clip-path=
+0000bde0: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000bdf0: 3136 3730 3831 3336 302d 6c69 6e65 2d31  167081360-line-1
+0000be00: 3229 223e 2e74 6f6d 6c3c 2f74 6578 743e  2)">.toml</text>
+0000be10: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000be20: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000be30: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000be40: 2233 3132 2e38 2220 7465 7874 4c65 6e67  "312.8" textLeng
+0000be50: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000be60: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000be70: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000be80: 6e65 2d31 3229 223e 0a3c 2f74 6578 743e  ne-12)">.</text>
+0000be90: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000bea0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000beb0: 2d72 3722 2078 3d22 3022 2079 3d22 3333  -r7" x="0" y="33
+0000bec0: 372e 3222 2074 6578 744c 656e 6774 683d  7.2" textLength=
+0000bed0: 2234 382e 3822 2063 6c69 702d 7061 7468  "48.8" clip-path
+0000bee0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000bef0: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000bf00: 3133 2922 3ee2 9497 e294 81e2 9481 2623  13)">.........&#
+0000bf10: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
+0000bf20: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000bf30: 2d32 3136 3730 3831 3336 302d 7234 2220  -2167081360-r4" 
+0000bf40: 783d 2234 382e 3822 2079 3d22 3333 372e  x="48.8" y="337.
+0000bf50: 3222 2074 6578 744c 656e 6774 683d 2232  2" textLength="2
+0000bf60: 342e 3422 2063 6c69 702d 7061 7468 3d22  4.4" clip-path="
+0000bf70: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000bf80: 3637 3038 3133 3630 2d6c 696e 652d 3133  67081360-line-13
+0000bf90: 2922 3ef0 9f93 8426 2331 3630 3b3c 2f74  )">....&#160;</t
+0000bfa0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000bfb0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000bfc0: 3133 3630 2d72 3422 2078 3d22 3835 2e34  1360-r4" x="85.4
+0000bfd0: 2220 793d 2233 3337 2e32 2220 7465 7874  " y="337.2" text
+0000bfe0: 4c65 6e67 7468 3d22 3733 2e32 2220 636c  Length="73.2" cl
+0000bff0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000c000: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000c010: 302d 6c69 6e65 2d31 3329 223e 5245 4144  0-line-13)">READ
+0000c020: 4d45 3c2f 7465 7874 3e3c 7465 7874 2063  ME</text><text c
+0000c030: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000c040: 3136 3730 3831 3336 302d 7231 3422 2078  167081360-r14" x
+0000c050: 3d22 3135 382e 3622 2079 3d22 3333 372e  ="158.6" y="337.
+0000c060: 3222 2074 6578 744c 656e 6774 683d 2233  2" textLength="3
+0000c070: 362e 3622 2063 6c69 702d 7061 7468 3d22  6.6" clip-path="
+0000c080: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000c090: 3637 3038 3133 3630 2d6c 696e 652d 3133  67081360-line-13
+0000c0a0: 2922 3e2e 6d64 3c2f 7465 7874 3e3c 7465  )">.md</text><te
+0000c0b0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000c0c0: 616c 2d32 3136 3730 3831 3336 302d 7231  al-2167081360-r1
+0000c0d0: 2220 783d 2231 3935 3222 2079 3d22 3333  " x="1952" y="33
+0000c0e0: 372e 3222 2074 6578 744c 656e 6774 683d  7.2" textLength=
+0000c0f0: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000c100: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000c110: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000c120: 3133 2922 3e0a 3c2f 7465 7874 3e3c 7465  13)">.</text><te
+0000c130: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000c140: 616c 2d32 3136 3730 3831 3336 302d 7231  al-2167081360-r1
+0000c150: 2220 783d 2231 3935 3222 2079 3d22 3336  " x="1952" y="36
+0000c160: 312e 3622 2074 6578 744c 656e 6774 683d  1.6" textLength=
+0000c170: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000c180: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000c190: 3231 3637 3038 3133 3630 2d6c 696e 652d  2167081360-line-
+0000c1a0: 3134 2922 3e0a 3c2f 7465 7874 3e3c 7465  14)">.</text><te
+0000c1b0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000c1c0: 616c 2d32 3136 3730 3831 3336 302d 7231  al-2167081360-r1
+0000c1d0: 3522 2078 3d22 3131 3130 2e32 2220 793d  5" x="1110.2" y=
+0000c1e0: 2233 3836 2220 7465 7874 4c65 6e67 7468  "386" textLength
+0000c1f0: 3d22 3134 362e 3422 2063 6c69 702d 7061  ="146.4" clip-pa
+0000c200: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000c210: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000c220: 652d 3135 2922 3e49 6e73 7461 6c6c 6174  e-15)">Installat
+0000c230: 696f 6e3c 2f74 6578 743e 3c74 6578 7420  ion</text><text 
+0000c240: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000c250: 3231 3637 3038 3133 3630 2d72 3122 2078  2167081360-r1" x
+0000c260: 3d22 3139 3532 2220 793d 2233 3836 2220  ="1952" y="386" 
+0000c270: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
+0000c280: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+0000c290: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+0000c2a0: 3831 3336 302d 6c69 6e65 2d31 3529 223e  81360-line-15)">
+0000c2b0: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000c2c0: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000c2d0: 3637 3038 3133 3630 2d72 3122 2078 3d22  67081360-r1" x="
+0000c2e0: 3139 3532 2220 793d 2234 3130 2e34 2220  1952" y="410.4" 
+0000c2f0: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
+0000c300: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+0000c310: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+0000c320: 3831 3336 302d 6c69 6e65 2d31 3629 223e  81360-line-16)">
+0000c330: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000c340: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000c350: 3637 3038 3133 3630 2d72 3622 2078 3d22  67081360-r6" x="
+0000c360: 3435 312e 3422 2079 3d22 3433 342e 3822  451.4" y="434.8"
+0000c370: 2074 6578 744c 656e 6774 683d 2233 3533   textLength="353
+0000c380: 2e38 2220 636c 6970 2d70 6174 683d 2275  .8" clip-path="u
+0000c390: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000c3a0: 3730 3831 3336 302d 6c69 6e65 2d31 3729  7081360-line-17)
+0000c3b0: 223e 5468 6526 2331 3630 3b62 656c 6f77  ">The&#160;below
+0000c3c0: 2623 3136 303b 636f 6d6d 616e 6426 2331  &#160;command&#1
+0000c3d0: 3630 3b72 6563 6f6d 6d65 6e64 7326 2331  60;recommends&#1
+0000c3e0: 3630 3b3c 2f74 6578 743e 3c74 6578 7420  60;</text><text 
+0000c3f0: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000c400: 3231 3637 3038 3133 3630 2d72 3131 2220  2167081360-r11" 
+0000c410: 783d 2238 3035 2e32 2220 793d 2234 3334  x="805.2" y="434
+0000c420: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
+0000c430: 3438 2e38 2220 636c 6970 2d70 6174 683d  48.8" clip-path=
+0000c440: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000c450: 3136 3730 3831 3336 302d 6c69 6e65 2d31  167081360-line-1
+0000c460: 3729 223e 7069 7078 3c2f 7465 7874 3e3c  7)">pipx</text><
+0000c470: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000c480: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000c490: 7236 2220 783d 2238 3534 2220 793d 2234  r6" x="854" y="4
+0000c4a0: 3334 2e38 2220 7465 7874 4c65 6e67 7468  34.8" textLength
+0000c4b0: 3d22 3230 372e 3422 2063 6c69 702d 7061  ="207.4" clip-pa
+0000c4c0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000c4d0: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000c4e0: 652d 3137 2922 3e26 2331 3630 3b69 6e73  e-17)">&#160;ins
+0000c4f0: 7465 6164 2623 3136 303b 6f66 2623 3136  tead&#160;of&#16
+0000c500: 303b 7069 702e 2623 3136 303b 3c2f 7465  0;pip.&#160;</te
+0000c510: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000c520: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000c530: 3336 302d 7231 3322 2078 3d22 3130 3631  360-r13" x="1061
+0000c540: 2e34 2220 793d 2234 3334 2e38 2220 7465  .4" y="434.8" te
+0000c550: 7874 4c65 6e67 7468 3d22 3438 2e38 2220  xtLength="48.8" 
+0000c560: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000c570: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000c580: 3336 302d 6c69 6e65 2d31 3729 223e 7069  360-line-17)">pi
+0000c590: 7078 3c2f 7465 7874 3e3c 7465 7874 2063  px</text><text c
+0000c5a0: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000c5b0: 3136 3730 3831 3336 302d 7236 2220 783d  167081360-r6" x=
+0000c5c0: 2231 3131 302e 3222 2079 3d22 3433 342e  "1110.2" y="434.
+0000c5d0: 3822 2074 6578 744c 656e 6774 683d 2232  8" textLength="2
+0000c5e0: 3932 2e38 2220 636c 6970 2d70 6174 683d  92.8" clip-path=
+0000c5f0: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000c600: 3136 3730 3831 3336 302d 6c69 6e65 2d31  167081360-line-1
+0000c610: 3729 223e 2623 3136 303b 696e 7374 616c  7)">&#160;instal
+0000c620: 6c73 2623 3136 303b 7468 6526 2331 3630  ls&#160;the&#160
+0000c630: 3b70 6163 6b61 6765 2623 3136 303b 696e  ;package&#160;in
+0000c640: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000c650: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000c660: 3730 3831 3336 302d 7236 2220 783d 2231  7081360-r6" x="1
+0000c670: 3431 352e 3222 2079 3d22 3433 342e 3822  415.2" y="434.8"
+0000c680: 2074 6578 744c 656e 6774 683d 2235 3132   textLength="512
+0000c690: 2e34 2220 636c 6970 2d70 6174 683d 2275  .4" clip-path="u
+0000c6a0: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000c6b0: 3730 3831 3336 302d 6c69 6e65 2d31 3729  7081360-line-17)
+0000c6c0: 223e 616e 2623 3136 303b 6973 6f6c 6174  ">an&#160;isolat
+0000c6d0: 6564 2623 3136 303b 656e 7669 726f 6e6d  ed&#160;environm
+0000c6e0: 656e 7426 2331 3630 3b61 6e64 2623 3136  ent&#160;and&#16
+0000c6f0: 303b 6d61 6b65 7326 2331 3630 3b69 7426  0;makes&#160;it&
+0000c700: 2331 3630 3b65 6173 7926 2331 3630 3b3c  #160;easy&#160;<
+0000c710: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000c720: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000c730: 3038 3133 3630 2d72 3122 2078 3d22 3139  081360-r1" x="19
+0000c740: 3532 2220 793d 2234 3334 2e38 2220 7465  52" y="434.8" te
+0000c750: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
+0000c760: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000c770: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000c780: 3336 302d 6c69 6e65 2d31 3729 223e 0a3c  360-line-17)">.<
+0000c790: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000c7a0: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000c7b0: 3038 3133 3630 2d72 3622 2078 3d22 3435  081360-r6" x="45
+0000c7c0: 312e 3422 2079 3d22 3435 392e 3222 2074  1.4" y="459.2" t
+0000c7d0: 6578 744c 656e 6774 683d 2234 3237 2220  extLength="427" 
+0000c7e0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000c7f0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000c800: 3336 302d 6c69 6e65 2d31 3829 223e 746f  360-line-18)">to
+0000c810: 2623 3136 303b 756e 696e 7374 616c 6c2e  &#160;uninstall.
+0000c820: 2623 3136 303b 4966 2623 3136 303b 796f  &#160;If&#160;yo
+0000c830: 7526 2378 3237 3b64 2623 3136 303b 6c69  u&#x27;d&#160;li
+0000c840: 6b65 2623 3136 303b 746f 2623 3136 303b  ke&#160;to&#160;
+0000c850: 7573 6526 2331 3630 3b3c 2f74 6578 743e  use&#160;</text>
+0000c860: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000c870: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000c880: 2d72 3133 2220 783d 2238 3738 2e34 2220  -r13" x="878.4" 
+0000c890: 793d 2234 3539 2e32 2220 7465 7874 4c65  y="459.2" textLe
+0000c8a0: 6e67 7468 3d22 3336 2e36 2220 636c 6970  ngth="36.6" clip
+0000c8b0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000c8c0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000c8d0: 6c69 6e65 2d31 3829 223e 7069 703c 2f74  line-18)">pip</t
+0000c8e0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000c8f0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000c900: 3133 3630 2d72 3622 2078 3d22 3931 3522  1360-r6" x="915"
+0000c910: 2079 3d22 3435 392e 3222 2074 6578 744c   y="459.2" textL
+0000c920: 656e 6774 683d 2232 3830 2e36 2220 636c  ength="280.6" cl
+0000c930: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000c940: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000c950: 302d 6c69 6e65 2d31 3829 223e 2623 3136  0-line-18)">&#16
+0000c960: 303b 696e 7374 6561 642c 2623 3136 303b  0;instead,&#160;
+0000c970: 6a75 7374 2623 3136 303b 7265 706c 6163  just&#160;replac
+0000c980: 6526 2331 3630 3b3c 2f74 6578 743e 3c74  e&#160;</text><t
+0000c990: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000c9a0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000c9b0: 3133 2220 783d 2231 3139 352e 3622 2079  13" x="1195.6" y
+0000c9c0: 3d22 3435 392e 3222 2074 6578 744c 656e  ="459.2" textLen
+0000c9d0: 6774 683d 2234 382e 3822 2063 6c69 702d  gth="48.8" clip-
+0000c9e0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000c9f0: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000ca00: 696e 652d 3138 2922 3e70 6970 783c 2f74  ine-18)">pipx</t
+0000ca10: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000ca20: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000ca30: 3133 3630 2d72 3622 2078 3d22 3132 3536  1360-r6" x="1256
+0000ca40: 2e36 2220 793d 2234 3539 2e32 2220 7465  .6" y="459.2" te
+0000ca50: 7874 4c65 6e67 7468 3d22 3631 2220 636c  xtLength="61" cl
+0000ca60: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000ca70: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000ca80: 302d 6c69 6e65 2d31 3829 223e 7769 7468  0-line-18)">with
+0000ca90: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
+0000caa0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000cab0: 616c 2d32 3136 3730 3831 3336 302d 7231  al-2167081360-r1
+0000cac0: 3322 2078 3d22 3133 3137 2e36 2220 793d  3" x="1317.6" y=
+0000cad0: 2234 3539 2e32 2220 7465 7874 4c65 6e67  "459.2" textLeng
+0000cae0: 7468 3d22 3336 2e36 2220 636c 6970 2d70  th="36.6" clip-p
+0000caf0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000cb00: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000cb10: 6e65 2d31 3829 223e 7069 703c 2f74 6578  ne-18)">pip</tex
+0000cb20: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000cb30: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000cb40: 3630 2d72 3622 2078 3d22 3133 3534 2e32  60-r6" x="1354.2
+0000cb50: 2220 793d 2234 3539 2e32 2220 7465 7874  " y="459.2" text
+0000cb60: 4c65 6e67 7468 3d22 3236 382e 3422 2063  Length="268.4" c
+0000cb70: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000cb80: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000cb90: 3630 2d6c 696e 652d 3138 2922 3e26 2331  60-line-18)">&#1
+0000cba0: 3630 3b69 6e26 2331 3630 3b74 6865 2623  60;in&#160;the&#
+0000cbb0: 3136 303b 6265 6c6f 7726 2331 3630 3b63  160;below&#160;c
+0000cbc0: 6f6d 6d61 6e64 2e3c 2f74 6578 743e 3c74  ommand.</text><t
+0000cbd0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000cbe0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000cbf0: 3122 2078 3d22 3139 3532 2220 793d 2234  1" x="1952" y="4
+0000cc00: 3539 2e32 2220 7465 7874 4c65 6e67 7468  59.2" textLength
+0000cc10: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
+0000cc20: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000cc30: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000cc40: 2d31 3829 223e 0a3c 2f74 6578 743e 3c74  -18)">.</text><t
+0000cc50: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000cc60: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000cc70: 3122 2078 3d22 3139 3532 2220 793d 2234  1" x="1952" y="4
+0000cc80: 3833 2e36 2220 7465 7874 4c65 6e67 7468  83.6" textLength
+0000cc90: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
+0000cca0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000ccb0: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000ccc0: 2d31 3929 223e 0a3c 2f74 6578 743e 3c74  -19)">.</text><t
+0000ccd0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000cce0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000ccf0: 3122 2078 3d22 3139 3532 2220 793d 2235  1" x="1952" y="5
+0000cd00: 3038 2220 7465 7874 4c65 6e67 7468 3d22  08" textLength="
+0000cd10: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
+0000cd20: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000cd30: 3136 3730 3831 3336 302d 6c69 6e65 2d32  167081360-line-2
+0000cd40: 3029 223e 0a3c 2f74 6578 743e 3c74 6578  0)">.</text><tex
+0000cd50: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000cd60: 6c2d 3231 3637 3038 3133 3630 2d72 3136  l-2167081360-r16
+0000cd70: 2220 783d 2234 3633 2e36 2220 793d 2235  " x="463.6" y="5
+0000cd80: 3332 2e34 2220 7465 7874 4c65 6e67 7468  32.4" textLength
+0000cd90: 3d22 3438 2e38 2220 636c 6970 2d70 6174  ="48.8" clip-pat
+0000cda0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000cdb0: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000cdc0: 2d32 3129 223e 7069 7078 3c2f 7465 7874  -21)">pipx</text
+0000cdd0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+0000cde0: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000cdf0: 302d 7231 3622 2078 3d22 3532 342e 3622  0-r16" x="524.6"
+0000ce00: 2079 3d22 3533 322e 3422 2074 6578 744c   y="532.4" textL
+0000ce10: 656e 6774 683d 2238 352e 3422 2063 6c69  ength="85.4" cli
+0000ce20: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000ce30: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000ce40: 2d6c 696e 652d 3231 2922 3e69 6e73 7461  -line-21)">insta
+0000ce50: 6c6c 3c2f 7465 7874 3e3c 7465 7874 2063  ll</text><text c
+0000ce60: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000ce70: 3136 3730 3831 3336 302d 7231 3622 2078  167081360-r16" x
+0000ce80: 3d22 3632 322e 3222 2079 3d22 3533 322e  ="622.2" y="532.
+0000ce90: 3422 2074 6578 744c 656e 6774 683d 2237  4" textLength="7
+0000cea0: 332e 3222 2063 6c69 702d 7061 7468 3d22  3.2" clip-path="
+0000ceb0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000cec0: 3637 3038 3133 3630 2d6c 696e 652d 3231  67081360-line-21
+0000ced0: 2922 3e62 726f 7773 723c 2f74 6578 743e  )">browsr</text>
+0000cee0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000cef0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000cf00: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000cf10: 2235 3332 2e34 2220 7465 7874 4c65 6e67  "532.4" textLeng
+0000cf20: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000cf30: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000cf40: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000cf50: 6e65 2d32 3129 223e 0a3c 2f74 6578 743e  ne-21)">.</text>
+0000cf60: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000cf70: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000cf80: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000cf90: 2235 3536 2e38 2220 7465 7874 4c65 6e67  "556.8" textLeng
+0000cfa0: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000cfb0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000cfc0: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000cfd0: 6e65 2d32 3229 223e 0a3c 2f74 6578 743e  ne-22)">.</text>
+0000cfe0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000cff0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000d000: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000d010: 2235 3831 2e32 2220 7465 7874 4c65 6e67  "581.2" textLeng
+0000d020: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000d030: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000d040: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000d050: 6e65 2d32 3329 223e 0a3c 2f74 6578 743e  ne-23)">.</text>
+0000d060: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000d070: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000d080: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000d090: 2236 3035 2e36 2220 7465 7874 4c65 6e67  "605.6" textLeng
+0000d0a0: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000d0b0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000d0c0: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000d0d0: 6e65 2d32 3429 223e 0a3c 2f74 6578 743e  ne-24)">.</text>
+0000d0e0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000d0f0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000d100: 2d72 3135 2220 783d 2231 3037 332e 3622  -r15" x="1073.6"
+0000d110: 2079 3d22 3633 3022 2074 6578 744c 656e   y="630" textLen
+0000d120: 6774 683d 2232 3139 2e36 2220 636c 6970  gth="219.6" clip
+0000d130: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000d140: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000d150: 6c69 6e65 2d32 3529 223e 4578 7472 6126  line-25)">Extra&
+0000d160: 2331 3630 3b49 6e73 7461 6c6c 6174 696f  #160;Installatio
+0000d170: 6e3c 2f74 6578 743e 3c74 6578 7420 636c  n</text><text cl
+0000d180: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000d190: 3637 3038 3133 3630 2d72 3122 2078 3d22  67081360-r1" x="
+0000d1a0: 3139 3532 2220 793d 2236 3330 2220 7465  1952" y="630" te
+0000d1b0: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
+0000d1c0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000d1d0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000d1e0: 3336 302d 6c69 6e65 2d32 3529 223e 0a3c  360-line-25)">.<
+0000d1f0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000d200: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000d210: 3038 3133 3630 2d72 3122 2078 3d22 3139  081360-r1" x="19
+0000d220: 3532 2220 793d 2236 3534 2e34 2220 7465  52" y="654.4" te
+0000d230: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
+0000d240: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000d250: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000d260: 3336 302d 6c69 6e65 2d32 3629 223e 0a3c  360-line-26)">.<
+0000d270: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000d280: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000d290: 3038 3133 3630 2d72 3622 2078 3d22 3435  081360-r6" x="45
+0000d2a0: 312e 3422 2079 3d22 3637 382e 3822 2074  1.4" y="678.8" t
+0000d2b0: 6578 744c 656e 6774 683d 2233 3035 2220  extLength="305" 
+0000d2c0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000d2d0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000d2e0: 3336 302d 6c69 6e65 2d32 3729 223e 4966  360-line-27)">If
+0000d2f0: 2623 3136 303b 796f 7526 2378 3237 3b72  &#160;you&#x27;r
+0000d300: 6526 2331 3630 3b6c 6f6f 6b69 6e67 2623  e&#160;looking&#
+0000d310: 3136 303b 746f 2623 3136 303b 7573 6526  160;to&#160;use&
+0000d320: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+0000d330: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000d340: 6c2d 3231 3637 3038 3133 3630 2d72 3133  l-2167081360-r13
+0000d350: 2220 783d 2237 3536 2e34 2220 793d 2236  " x="756.4" y="6
+0000d360: 3738 2e38 2220 7465 7874 4c65 6e67 7468  78.8" textLength
+0000d370: 3d22 3733 2e32 2220 636c 6970 2d70 6174  ="73.2" clip-pat
+0000d380: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000d390: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000d3a0: 2d32 3729 223e 6272 6f77 7372 3c2f 7465  -27)">browsr</te
+0000d3b0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000d3c0: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000d3d0: 3336 302d 7236 2220 783d 2238 3239 2e36  360-r6" x="829.6
+0000d3e0: 2220 793d 2236 3738 2e38 2220 7465 7874  " y="678.8" text
+0000d3f0: 4c65 6e67 7468 3d22 3739 3322 2063 6c69  Length="793" cli
+0000d400: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000d410: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000d420: 2d6c 696e 652d 3237 2922 3e26 2331 3630  -line-27)">&#160
+0000d430: 3b6f 6e26 2331 3630 3b72 656d 6f74 6526  ;on&#160;remote&
+0000d440: 2331 3630 3b66 696c 6526 2331 3630 3b73  #160;file&#160;s
+0000d450: 7973 7465 6d73 2c26 2331 3630 3b6c 696b  ystems,&#160;lik
+0000d460: 6526 2331 3630 3b41 5753 2623 3136 303b  e&#160;AWS&#160;
+0000d470: 5333 2c26 2331 3630 3b79 6f75 2623 7832  S3,&#160;you&#x2
+0000d480: 373b 6c6c 2623 3136 303b 6e65 6564 2623  7;ll&#160;need&#
+0000d490: 3136 303b 746f 2623 3136 303b 696e 7374  160;to&#160;inst
+0000d4a0: 616c 6c26 2331 3630 3b74 6865 2623 3136  all&#160;the&#16
+0000d4b0: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
+0000d4c0: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000d4d0: 3136 3730 3831 3336 302d 7231 3322 2078  167081360-r13" x
+0000d4e0: 3d22 3136 3232 2e36 2220 793d 2236 3738  ="1622.6" y="678
+0000d4f0: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
+0000d500: 3733 2e32 2220 636c 6970 2d70 6174 683d  73.2" clip-path=
+0000d510: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000d520: 3136 3730 3831 3336 302d 6c69 6e65 2d32  167081360-line-2
+0000d530: 3729 223e 7265 6d6f 7465 3c2f 7465 7874  7)">remote</text
+0000d540: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+0000d550: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000d560: 302d 7236 2220 783d 2231 3639 352e 3822  0-r6" x="1695.8"
+0000d570: 2079 3d22 3637 382e 3822 2074 6578 744c   y="678.8" textL
+0000d580: 656e 6774 683d 2238 352e 3422 2063 6c69  ength="85.4" cli
+0000d590: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000d5a0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000d5b0: 2d6c 696e 652d 3237 2922 3e26 2331 3630  -line-27)">&#160
+0000d5c0: 3b65 7874 7261 2e3c 2f74 6578 743e 3c74  ;extra.</text><t
+0000d5d0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000d5e0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000d5f0: 3622 2078 3d22 3137 3933 2e34 2220 793d  6" x="1793.4" y=
+0000d600: 2236 3738 2e38 2220 7465 7874 4c65 6e67  "678.8" textLeng
+0000d610: 7468 3d22 3130 392e 3822 2063 6c69 702d  th="109.8" clip-
+0000d620: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000d630: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000d640: 696e 652d 3237 2922 3e49 6626 2331 3630  ine-27)">If&#160
+0000d650: 3b79 6f75 2623 7832 373b 6426 2331 3630  ;you&#x27;d&#160
+0000d660: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
+0000d670: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000d680: 3637 3038 3133 3630 2d72 3122 2078 3d22  67081360-r1" x="
+0000d690: 3139 3532 2220 793d 2236 3738 2e38 2220  1952" y="678.8" 
+0000d6a0: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
+0000d6b0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+0000d6c0: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+0000d6d0: 3831 3336 302d 6c69 6e65 2d32 3729 223e  81360-line-27)">
+0000d6e0: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000d6f0: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000d700: 3637 3038 3133 3630 2d72 3622 2078 3d22  67081360-r6" x="
+0000d710: 3435 312e 3422 2079 3d22 3730 332e 3222  451.4" y="703.2"
+0000d720: 2074 6578 744c 656e 6774 683d 2236 3935   textLength="695
+0000d730: 2e34 2220 636c 6970 2d70 6174 683d 2275  .4" clip-path="u
+0000d740: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000d750: 3730 3831 3336 302d 6c69 6e65 2d32 3829  7081360-line-28)
+0000d760: 223e 6c69 6b65 2623 3136 303b 746f 2623  ">like&#160;to&#
+0000d770: 3136 303b 6272 6f77 7365 2623 3136 303b  160;browse&#160;
+0000d780: 7061 7271 7565 7426 2331 3630 3b66 696c  parquet&#160;fil
+0000d790: 6573 2c26 2331 3630 3b79 6f75 2623 7832  es,&#160;you&#x2
+0000d7a0: 373b 6c6c 2623 3136 303b 6e65 6564 2623  7;ll&#160;need&#
+0000d7b0: 3136 303b 746f 2623 3136 303b 696e 7374  160;to&#160;inst
+0000d7c0: 616c 6c26 2331 3630 3b74 6865 2623 3136  all&#160;the&#16
+0000d7d0: 303b 3c2f 7465 7874 3e3c 7465 7874 2063  0;</text><text c
+0000d7e0: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000d7f0: 3136 3730 3831 3336 302d 7231 3322 2078  167081360-r13" x
+0000d800: 3d22 3131 3436 2e38 2220 793d 2237 3033  ="1146.8" y="703
+0000d810: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
+0000d820: 3835 2e34 2220 636c 6970 2d70 6174 683d  85.4" clip-path=
+0000d830: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000d840: 3136 3730 3831 3336 302d 6c69 6e65 2d32  167081360-line-2
+0000d850: 3829 223e 7061 7271 7565 743c 2f74 6578  8)">parquet</tex
+0000d860: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000d870: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000d880: 3630 2d72 3622 2078 3d22 3132 3332 2e32  60-r6" x="1232.2
+0000d890: 2220 793d 2237 3033 2e32 2220 7465 7874  " y="703.2" text
+0000d8a0: 4c65 6e67 7468 3d22 3330 3522 2063 6c69  Length="305" cli
+0000d8b0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000d8c0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000d8d0: 2d6c 696e 652d 3238 2922 3e26 2331 3630  -line-28)">&#160
+0000d8e0: 3b65 7874 7261 2e26 2331 3630 3b4f 722c  ;extra.&#160;Or,
+0000d8f0: 2623 3136 303b 6576 656e 2623 3136 303b  &#160;even&#160;
+0000d900: 7369 6d70 6c65 722c 3c2f 7465 7874 3e3c  simpler,</text><
+0000d910: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000d920: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000d930: 7236 2220 783d 2231 3534 392e 3422 2079  r6" x="1549.4" y
+0000d940: 3d22 3730 332e 3222 2074 6578 744c 656e  ="703.2" textLen
+0000d950: 6774 683d 2232 3434 2220 636c 6970 2d70  gth="244" clip-p
+0000d960: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000d970: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000d980: 6e65 2d32 3829 223e 796f 7526 2331 3630  ne-28)">you&#160
+0000d990: 3b63 616e 2623 3136 303b 696e 7374 616c  ;can&#160;instal
+0000d9a0: 6c26 2331 3630 3b74 6865 2623 3136 303b  l&#160;the&#160;
+0000d9b0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000d9c0: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000d9d0: 3730 3831 3336 302d 7231 3322 2078 3d22  7081360-r13" x="
+0000d9e0: 3137 3933 2e34 2220 793d 2237 3033 2e32  1793.4" y="703.2
+0000d9f0: 2220 7465 7874 4c65 6e67 7468 3d22 3336  " textLength="36
+0000da00: 2e36 2220 636c 6970 2d70 6174 683d 2275  .6" clip-path="u
+0000da10: 726c 2823 7465 726d 696e 616c 2d32 3136  rl(#terminal-216
+0000da20: 3730 3831 3336 302d 6c69 6e65 2d32 3829  7081360-line-28)
+0000da30: 223e 616c 6c3c 2f74 6578 743e 3c74 6578  ">all</text><tex
+0000da40: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000da50: 6c2d 3231 3637 3038 3133 3630 2d72 3622  l-2167081360-r6"
+0000da60: 2078 3d22 3138 3330 2220 793d 2237 3033   x="1830" y="703
+0000da70: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
+0000da80: 3835 2e34 2220 636c 6970 2d70 6174 683d  85.4" clip-path=
+0000da90: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000daa0: 3136 3730 3831 3336 302d 6c69 6e65 2d32  167081360-line-2
+0000dab0: 3829 223e 2623 3136 303b 6578 7472 6126  8)">&#160;extra&
+0000dac0: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+0000dad0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000dae0: 6c2d 3231 3637 3038 3133 3630 2d72 3122  l-2167081360-r1"
+0000daf0: 2078 3d22 3139 3532 2220 793d 2237 3033   x="1952" y="703
+0000db00: 2e32 2220 7465 7874 4c65 6e67 7468 3d22  .2" textLength="
+0000db10: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
+0000db20: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000db30: 3136 3730 3831 3336 302d 6c69 6e65 2d32  167081360-line-2
+0000db40: 3829 223e 0a3c 2f74 6578 743e 3c74 6578  8)">.</text><tex
+0000db50: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000db60: 6c2d 3231 3637 3038 3133 3630 2d72 3622  l-2167081360-r6"
+0000db70: 2078 3d22 3435 312e 3422 2079 3d22 3732   x="451.4" y="72
+0000db80: 372e 3622 2074 6578 744c 656e 6774 683d  7.6" textLength=
+0000db90: 2232 3638 2e34 2220 636c 6970 2d70 6174  "268.4" clip-pat
+0000dba0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000dbb0: 2d32 3136 3730 3831 3336 302d 6c69 6e65  -2167081360-line
+0000dbc0: 2d32 3929 223e 746f 2623 3136 303b 6765  -29)">to&#160;ge
+0000dbd0: 7426 2331 3630 3b61 6c6c 2623 3136 303b  t&#160;all&#160;
+0000dbe0: 7468 6526 2331 3630 3b65 7874 7261 732e  the&#160;extras.
+0000dbf0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000dc00: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000dc10: 3730 3831 3336 302d 7231 2220 783d 2231  7081360-r1" x="1
+0000dc20: 3935 3222 2079 3d22 3732 372e 3622 2074  952" y="727.6" t
+0000dc30: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000dc40: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000dc50: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000dc60: 3133 3630 2d6c 696e 652d 3239 2922 3e0a  1360-line-29)">.
+0000dc70: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000dc80: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000dc90: 3730 3831 3336 302d 7231 2220 783d 2231  7081360-r1" x="1
+0000dca0: 3935 3222 2079 3d22 3735 3222 2074 6578  952" y="752" tex
+0000dcb0: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+0000dcc0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000dcd0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000dce0: 3630 2d6c 696e 652d 3330 2922 3e0a 3c2f  60-line-30)">.</
+0000dcf0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000dd00: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000dd10: 3831 3336 302d 7231 2220 783d 2231 3935  81360-r1" x="195
+0000dd20: 3222 2079 3d22 3737 362e 3422 2074 6578  2" y="776.4" tex
+0000dd30: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+0000dd40: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000dd50: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000dd60: 3630 2d6c 696e 652d 3331 2922 3e0a 3c2f  60-line-31)">.</
+0000dd70: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000dd80: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000dd90: 3831 3336 302d 7231 3622 2078 3d22 3436  81360-r16" x="46
+0000dda0: 332e 3622 2079 3d22 3830 302e 3822 2074  3.6" y="800.8" t
+0000ddb0: 6578 744c 656e 6774 683d 2234 382e 3822  extLength="48.8"
+0000ddc0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000ddd0: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000dde0: 3133 3630 2d6c 696e 652d 3332 2922 3e70  1360-line-32)">p
+0000ddf0: 6970 783c 2f74 6578 743e 3c74 6578 7420  ipx</text><text 
+0000de00: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000de10: 3231 3637 3038 3133 3630 2d72 3136 2220  2167081360-r16" 
+0000de20: 783d 2235 3234 2e36 2220 793d 2238 3030  x="524.6" y="800
+0000de30: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
+0000de40: 3835 2e34 2220 636c 6970 2d70 6174 683d  85.4" clip-path=
+0000de50: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000de60: 3136 3730 3831 3336 302d 6c69 6e65 2d33  167081360-line-3
+0000de70: 3229 223e 696e 7374 616c 6c3c 2f74 6578  2)">install</tex
+0000de80: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000de90: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000dea0: 3630 2d72 3137 2220 783d 2236 3232 2e32  60-r17" x="622.2
+0000deb0: 2220 793d 2238 3030 2e38 2220 7465 7874  " y="800.8" text
+0000dec0: 4c65 6e67 7468 3d22 3135 382e 3622 2063  Length="158.6" c
+0000ded0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000dee0: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000def0: 3630 2d6c 696e 652d 3332 2922 3e26 7175  60-line-32)">&qu
+0000df00: 6f74 3b62 726f 7773 725b 616c 6c5d 2671  ot;browsr[all]&q
+0000df10: 756f 743b 3c2f 7465 7874 3e3c 7465 7874  uot;</text><text
+0000df20: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000df30: 2d32 3136 3730 3831 3336 302d 7231 2220  -2167081360-r1" 
+0000df40: 783d 2231 3935 3222 2079 3d22 3830 302e  x="1952" y="800.
+0000df50: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
+0000df60: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000df70: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000df80: 3637 3038 3133 3630 2d6c 696e 652d 3332  67081360-line-32
+0000df90: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
+0000dfa0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000dfb0: 2d32 3136 3730 3831 3336 302d 7231 2220  -2167081360-r1" 
+0000dfc0: 783d 2231 3935 3222 2079 3d22 3832 352e  x="1952" y="825.
+0000dfd0: 3222 2074 6578 744c 656e 6774 683d 2231  2" textLength="1
+0000dfe0: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000dff0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000e000: 3637 3038 3133 3630 2d6c 696e 652d 3333  67081360-line-33
+0000e010: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
+0000e020: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000e030: 2d32 3136 3730 3831 3336 302d 7231 2220  -2167081360-r1" 
+0000e040: 783d 2231 3935 3222 2079 3d22 3834 392e  x="1952" y="849.
+0000e050: 3622 2074 6578 744c 656e 6774 683d 2231  6" textLength="1
+0000e060: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000e070: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000e080: 3637 3038 3133 3630 2d6c 696e 652d 3334  67081360-line-34
+0000e090: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
+0000e0a0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000e0b0: 2d32 3136 3730 3831 3336 302d 7231 2220  -2167081360-r1" 
+0000e0c0: 783d 2231 3935 3222 2079 3d22 3837 3422  x="1952" y="874"
+0000e0d0: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+0000e0e0: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+0000e0f0: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+0000e100: 3038 3133 3630 2d6c 696e 652d 3335 2922  081360-line-35)"
+0000e110: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
+0000e120: 6c61 7373 3d22 7465 726d 696e 616c 2d32  lass="terminal-2
+0000e130: 3136 3730 3831 3336 302d 7231 3522 2078  167081360-r15" x
+0000e140: 3d22 3131 3539 2220 793d 2238 3938 2e34  ="1159" y="898.4
+0000e150: 2220 7465 7874 4c65 6e67 7468 3d22 3631  " textLength="61
+0000e160: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+0000e170: 2823 7465 726d 696e 616c 2d32 3136 3730  (#terminal-21670
+0000e180: 3831 3336 302d 6c69 6e65 2d33 3629 223e  81360-line-36)">
+0000e190: 5573 6167 653c 2f74 6578 743e 3c74 6578  Usage</text><tex
+0000e1a0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000e1b0: 6c2d 3231 3637 3038 3133 3630 2d72 3122  l-2167081360-r1"
+0000e1c0: 2078 3d22 3139 3532 2220 793d 2238 3938   x="1952" y="898
+0000e1d0: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
+0000e1e0: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
+0000e1f0: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000e200: 3136 3730 3831 3336 302d 6c69 6e65 2d33  167081360-line-3
+0000e210: 3629 223e 0a3c 2f74 6578 743e 3c74 6578  6)">.</text><tex
+0000e220: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000e230: 6c2d 3231 3637 3038 3133 3630 2d72 3122  l-2167081360-r1"
+0000e240: 2078 3d22 3139 3532 2220 793d 2239 3232   x="1952" y="922
+0000e250: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
+0000e260: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
+0000e270: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000e280: 3136 3730 3831 3336 302d 6c69 6e65 2d33  167081360-line-3
+0000e290: 3729 223e 0a3c 2f74 6578 743e 3c74 6578  7)">.</text><tex
+0000e2a0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000e2b0: 6c2d 3231 3637 3038 3133 3630 2d72 3138  l-2167081360-r18
+0000e2c0: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+0000e2d0: 3934 372e 3222 2074 6578 744c 656e 6774  947.2" textLengt
+0000e2e0: 683d 2232 342e 3422 2063 6c69 702d 7061  h="24.4" clip-pa
+0000e2f0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000e300: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000e310: 652d 3338 2922 3ee2 9684 e296 843c 2f74  e-38)">......</t
+0000e320: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000e330: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000e340: 3133 3630 2d72 3122 2078 3d22 3139 3532  1360-r1" x="1952
+0000e350: 2220 793d 2239 3437 2e32 2220 7465 7874  " y="947.2" text
+0000e360: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
+0000e370: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000e380: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000e390: 302d 6c69 6e65 2d33 3829 223e 0a3c 2f74  0-line-38)">.</t
+0000e3a0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000e3b0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000e3c0: 3133 3630 2d72 3136 2220 783d 2234 3633  1360-r16" x="463
+0000e3d0: 2e36 2220 793d 2239 3731 2e36 2220 7465  .6" y="971.6" te
+0000e3e0: 7874 4c65 6e67 7468 3d22 3733 2e32 2220  xtLength="73.2" 
+0000e3f0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000e400: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000e410: 3336 302d 6c69 6e65 2d33 3929 223e 6272  360-line-39)">br
+0000e420: 6f77 7372 3c2f 7465 7874 3e3c 7465 7874  owsr</text><text
+0000e430: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000e440: 2d32 3136 3730 3831 3336 302d 7231 3622  -2167081360-r16"
+0000e450: 2078 3d22 3534 3922 2079 3d22 3937 312e   x="549" y="971.
+0000e460: 3622 2074 6578 744c 656e 6774 683d 2231  6" textLength="1
+0000e470: 3436 2e34 2220 636c 6970 2d70 6174 683d  46.4" clip-path=
+0000e480: 2275 726c 2823 7465 726d 696e 616c 2d32  "url(#terminal-2
+0000e490: 3136 3730 3831 3336 302d 6c69 6e65 2d33  167081360-line-3
+0000e4a0: 3929 223e 7e2f 446f 776e 6c6f 6164 732f  9)">~/Downloads/
+0000e4b0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000e4c0: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000e4d0: 3730 3831 3336 302d 7231 2220 783d 2231  7081360-r1" x="1
+0000e4e0: 3935 3222 2079 3d22 3937 312e 3622 2074  952" y="971.6" t
+0000e4f0: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000e500: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000e510: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000e520: 3133 3630 2d6c 696e 652d 3339 2922 3e0a  1360-line-39)">.
+0000e530: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000e540: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000e550: 3730 3831 3336 302d 7231 2220 783d 2231  7081360-r1" x="1
+0000e560: 3935 3222 2079 3d22 3939 3622 2074 6578  952" y="996" tex
+0000e570: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+0000e580: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000e590: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000e5a0: 3630 2d6c 696e 652d 3430 2922 3e0a 3c2f  60-line-40)">.</
+0000e5b0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000e5c0: 3d22 7465 726d 696e 616c 2d32 3136 3730  ="terminal-21670
+0000e5d0: 3831 3336 302d 7231 2220 783d 2231 3935  81360-r1" x="195
+0000e5e0: 3222 2079 3d22 3130 3230 2e34 2220 7465  2" y="1020.4" te
+0000e5f0: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
+0000e600: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000e610: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000e620: 3336 302d 6c69 6e65 2d34 3129 223e 0a3c  360-line-41)">.<
+0000e630: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000e640: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000e650: 3038 3133 3630 2d72 3622 2078 3d22 3435  081360-r6" x="45
+0000e660: 312e 3422 2079 3d22 3130 3434 2e38 2220  1.4" y="1044.8" 
+0000e670: 7465 7874 4c65 6e67 7468 3d22 3134 362e  textLength="146.
+0000e680: 3422 2063 6c69 702d 7061 7468 3d22 7572  4" clip-path="ur
+0000e690: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+0000e6a0: 3038 3133 3630 2d6c 696e 652d 3432 2922  081360-line-42)"
+0000e6b0: 3e53 696d 706c 7926 2331 3630 3b67 6976  >Simply&#160;giv
+0000e6c0: 6526 2331 3630 3b3c 2f74 6578 743e 3c74  e&#160;</text><t
+0000e6d0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000e6e0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000e6f0: 3133 2220 783d 2235 3937 2e38 2220 793d  13" x="597.8" y=
+0000e700: 2231 3034 342e 3822 2074 6578 744c 656e  "1044.8" textLen
+0000e710: 6774 683d 2237 332e 3222 2063 6c69 702d  gth="73.2" clip-
+0000e720: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000e730: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000e740: 696e 652d 3432 2922 3e62 726f 7773 723c  ine-42)">browsr<
+0000e750: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000e760: 733d 2274 6572 6d69 6e61 6c2d 3231 3637  s="terminal-2167
+0000e770: 3038 3133 3630 2d72 3622 2078 3d22 3637  081360-r6" x="67
+0000e780: 3122 2079 3d22 3130 3434 2e38 2220 7465  1" y="1044.8" te
+0000e790: 7874 4c65 6e67 7468 3d22 3734 342e 3222  xtLength="744.2"
+0000e7a0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000e7b0: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000e7c0: 3133 3630 2d6c 696e 652d 3432 2922 3e26  1360-line-42)">&
+0000e7d0: 2331 3630 3b61 2623 3136 303b 7061 7468  #160;a&#160;path
+0000e7e0: 2623 3136 303b 746f 2623 3136 303b 6126  &#160;to&#160;a&
+0000e7f0: 2331 3630 3b66 696c 652f 6469 7265 6374  #160;file/direct
+0000e800: 6f72 7926 2331 3630 3b61 6e64 2623 3136  ory&#160;and&#16
+0000e810: 303b 6974 2623 3136 303b 7769 6c6c 2623  0;it&#160;will&#
+0000e820: 3136 303b 6f70 656e 2623 3136 303b 6126  160;open&#160;a&
+0000e830: 2331 3630 3b62 726f 7773 6572 2623 3136  #160;browser&#16
+0000e840: 303b 7769 6e64 6f77 3c2f 7465 7874 3e3c  0;window</text><
+0000e850: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000e860: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000e870: 7236 2220 783d 2231 3432 372e 3422 2079  r6" x="1427.4" y
+0000e880: 3d22 3130 3434 2e38 2220 7465 7874 4c65  ="1044.8" textLe
+0000e890: 6e67 7468 3d22 3530 302e 3222 2063 6c69  ngth="500.2" cli
+0000e8a0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000e8b0: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000e8c0: 2d6c 696e 652d 3432 2922 3e77 6974 6826  -line-42)">with&
+0000e8d0: 2331 3630 3b61 2623 3136 303b 6669 6c65  #160;a&#160;file
+0000e8e0: 2623 3136 303b 6272 6f77 7365 722e 2623  &#160;browser.&#
+0000e8f0: 3136 303b 596f 7526 2331 3630 3b63 616e  160;You&#160;can
+0000e900: 2623 3136 303b 616c 736f 2623 3136 303b  &#160;also&#160;
+0000e910: 6769 7665 2623 3136 303b 6974 3c2f 7465  give&#160;it</te
+0000e920: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000e930: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000e940: 3336 302d 7231 2220 783d 2231 3935 3222  360-r1" x="1952"
+0000e950: 2079 3d22 3130 3434 2e38 2220 7465 7874   y="1044.8" text
+0000e960: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
+0000e970: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+0000e980: 726d 696e 616c 2d32 3136 3730 3831 3336  rminal-216708136
+0000e990: 302d 6c69 6e65 2d34 3229 223e 0a3c 2f74  0-line-42)">.</t
+0000e9a0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000e9b0: 2274 6572 6d69 6e61 6c2d 3231 3637 3038  "terminal-216708
+0000e9c0: 3133 3630 2d72 3622 2078 3d22 3435 312e  1360-r6" x="451.
+0000e9d0: 3422 2079 3d22 3130 3639 2e32 2220 7465  4" y="1069.2" te
+0000e9e0: 7874 4c65 6e67 7468 3d22 3532 342e 3622  xtLength="524.6"
+0000e9f0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000ea00: 2374 6572 6d69 6e61 6c2d 3231 3637 3038  #terminal-216708
+0000ea10: 3133 3630 2d6c 696e 652d 3433 2922 3e61  1360-line-43)">a
+0000ea20: 2623 3136 303b 5552 4c26 2331 3630 3b74  &#160;URL&#160;t
+0000ea30: 6f26 2331 3630 3b61 2623 3136 303b 7265  o&#160;a&#160;re
+0000ea40: 6d6f 7465 2623 3136 303b 6669 6c65 2623  mote&#160;file&#
+0000ea50: 3136 303b 7379 7374 656d 2c26 2331 3630  160;system,&#160
+0000ea60: 3b6c 696b 6526 2331 3630 3b41 5753 2623  ;like&#160;AWS&#
+0000ea70: 3136 303b 5333 2e3c 2f74 6578 743e 3c74  160;S3.</text><t
+0000ea80: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000ea90: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000eaa0: 3122 2078 3d22 3139 3532 2220 793d 2231  1" x="1952" y="1
+0000eab0: 3036 392e 3222 2074 6578 744c 656e 6774  069.2" textLengt
+0000eac0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000ead0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000eae0: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000eaf0: 652d 3433 2922 3e0a 3c2f 7465 7874 3e3c  e-43)">.</text><
+0000eb00: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000eb10: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000eb20: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
+0000eb30: 3130 3933 2e36 2220 7465 7874 4c65 6e67  1093.6" textLeng
+0000eb40: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000eb50: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000eb60: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000eb70: 6e65 2d34 3429 223e 0a3c 2f74 6578 743e  ne-44)">.</text>
+0000eb80: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000eb90: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000eba0: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000ebb0: 2231 3131 3822 2074 6578 744c 656e 6774  "1118" textLengt
+0000ebc0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000ebd0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000ebe0: 6c2d 3231 3637 3038 3133 3630 2d6c 696e  l-2167081360-lin
+0000ebf0: 652d 3435 2922 3e0a 3c2f 7465 7874 3e3c  e-45)">.</text><
+0000ec00: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000ec10: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000ec20: 7231 3922 2078 3d22 3132 2e32 2220 793d  r19" x="12.2" y=
+0000ec30: 2231 3134 322e 3422 2074 6578 744c 656e  "1142.4" textLen
+0000ec40: 6774 683d 2235 3835 2e36 2220 636c 6970  gth="585.6" clip
+0000ec50: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000ec60: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000ec70: 6c69 6e65 2d34 3629 223e f09f 9784 efb8  line-46)">......
+0000ec80: 8fef b88f efb8 8f26 2331 3630 3b26 2331  .......&#160;&#1
+0000ec90: 3630 3b33 4b42 2623 3136 303b 2623 3136  60;3KB&#160;&#16
+0000eca0: 303b f09f 92be 2623 3136 303b 2623 3136  0;....&#160;&#16
+0000ecb0: 303b 5245 4144 4d45 2e6d 6426 2331 3630  0;README.md&#160
+0000ecc0: 3b26 2331 3630 3bf0 9f93 8226 2331 3630  ;&#160;....&#160
+0000ecd0: 3b26 2331 3630 3b6a 7566 7469 6e3a 6272  ;&#160;juftin:br
+0000ece0: 6f77 7372 4076 312e 362e 303c 2f74 6578  owsr@v1.6.0</tex
+0000ecf0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000ed00: 6572 6d69 6e61 6c2d 3231 3637 3038 3133  erminal-21670813
+0000ed10: 3630 2d72 3122 2078 3d22 3139 3532 2220  60-r1" x="1952" 
+0000ed20: 793d 2231 3134 322e 3422 2074 6578 744c  y="1142.4" textL
+0000ed30: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+0000ed40: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000ed50: 6d69 6e61 6c2d 3231 3637 3038 3133 3630  minal-2167081360
+0000ed60: 2d6c 696e 652d 3436 2922 3e0a 3c2f 7465  -line-46)">.</te
+0000ed70: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000ed80: 7465 726d 696e 616c 2d32 3136 3730 3831  terminal-2167081
+0000ed90: 3336 302d 7232 3022 2078 3d22 3022 2079  360-r20" x="0" y
+0000eda0: 3d22 3131 3636 2e38 2220 7465 7874 4c65  ="1166.8" textLe
+0000edb0: 6e67 7468 3d22 3336 2e36 2220 636c 6970  ngth="36.6" clip
+0000edc0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000edd0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000ede0: 6c69 6e65 2d34 3729 223e 2623 3136 303b  line-47)">&#160;
+0000edf0: 5126 2331 3630 3b3c 2f74 6578 743e 3c74  Q&#160;</text><t
+0000ee00: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000ee10: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000ee20: 3231 2220 783d 2233 362e 3622 2079 3d22  21" x="36.6" y="
+0000ee30: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
+0000ee40: 7468 3d22 3733 2e32 2220 636c 6970 2d70  th="73.2" clip-p
+0000ee50: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000ee60: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000ee70: 6e65 2d34 3729 223e 2623 3136 303b 5175  ne-47)">&#160;Qu
+0000ee80: 6974 2623 3136 303b 3c2f 7465 7874 3e3c  it&#160;</text><
+0000ee90: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000eea0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000eeb0: 7232 3022 2078 3d22 3130 392e 3822 2079  r20" x="109.8" y
+0000eec0: 3d22 3131 3636 2e38 2220 7465 7874 4c65  ="1166.8" textLe
+0000eed0: 6e67 7468 3d22 3336 2e36 2220 636c 6970  ngth="36.6" clip
+0000eee0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000eef0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000ef00: 6c69 6e65 2d34 3729 223e 2623 3136 303b  line-47)">&#160;
+0000ef10: 4626 2331 3630 3b3c 2f74 6578 743e 3c74  F&#160;</text><t
+0000ef20: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000ef30: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000ef40: 3231 2220 783d 2231 3436 2e34 2220 793d  21" x="146.4" y=
+0000ef50: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
+0000ef60: 6774 683d 2231 3730 2e38 2220 636c 6970  gth="170.8" clip
+0000ef70: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000ef80: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000ef90: 6c69 6e65 2d34 3729 223e 2623 3136 303b  line-47)">&#160;
+0000efa0: 546f 6767 6c65 2623 3136 303b 4669 6c65  Toggle&#160;File
+0000efb0: 7326 2331 3630 3b3c 2f74 6578 743e 3c74  s&#160;</text><t
+0000efc0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000efd0: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000efe0: 3230 2220 783d 2233 3137 2e32 2220 793d  20" x="317.2" y=
+0000eff0: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
+0000f000: 6774 683d 2233 362e 3622 2063 6c69 702d  gth="36.6" clip-
+0000f010: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000f020: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000f030: 696e 652d 3437 2922 3e26 2331 3630 3b54  ine-47)">&#160;T
+0000f040: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
+0000f050: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000f060: 616c 2d32 3136 3730 3831 3336 302d 7232  al-2167081360-r2
+0000f070: 3122 2078 3d22 3335 332e 3822 2079 3d22  1" x="353.8" y="
+0000f080: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
+0000f090: 7468 3d22 3137 302e 3822 2063 6c69 702d  th="170.8" clip-
+0000f0a0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000f0b0: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000f0c0: 696e 652d 3437 2922 3e26 2331 3630 3b54  ine-47)">&#160;T
+0000f0d0: 6f67 676c 6526 2331 3630 3b54 6865 6d65  oggle&#160;Theme
+0000f0e0: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
+0000f0f0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+0000f100: 616c 2d32 3136 3730 3831 3336 302d 7232  al-2167081360-r2
+0000f110: 3022 2078 3d22 3532 342e 3622 2079 3d22  0" x="524.6" y="
+0000f120: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
+0000f130: 7468 3d22 3336 2e36 2220 636c 6970 2d70  th="36.6" clip-p
+0000f140: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000f150: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000f160: 6e65 2d34 3729 223e 2623 3136 303b 4e26  ne-47)">&#160;N&
+0000f170: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+0000f180: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000f190: 6c2d 3231 3637 3038 3133 3630 2d72 3231  l-2167081360-r21
+0000f1a0: 2220 783d 2235 3631 2e32 2220 793d 2231  " x="561.2" y="1
+0000f1b0: 3136 362e 3822 2074 6578 744c 656e 6774  166.8" textLengt
+0000f1c0: 683d 2232 3536 2e32 2220 636c 6970 2d70  h="256.2" clip-p
+0000f1d0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000f1e0: 616c 2d32 3136 3730 3831 3336 302d 6c69  al-2167081360-li
+0000f1f0: 6e65 2d34 3729 223e 2623 3136 303b 546f  ne-47)">&#160;To
+0000f200: 6767 6c65 2623 3136 303b 4c69 6e65 2623  ggle&#160;Line&#
+0000f210: 3136 303b 4e75 6d62 6572 7326 2331 3630  160;Numbers&#160
+0000f220: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
+0000f230: 6173 733d 2274 6572 6d69 6e61 6c2d 3231  ass="terminal-21
+0000f240: 3637 3038 3133 3630 2d72 3230 2220 783d  67081360-r20" x=
+0000f250: 2238 3137 2e34 2220 793d 2231 3136 362e  "817.4" y="1166.
+0000f260: 3822 2074 6578 744c 656e 6774 683d 2233  8" textLength="3
+0000f270: 362e 3622 2063 6c69 702d 7061 7468 3d22  6.6" clip-path="
+0000f280: 7572 6c28 2374 6572 6d69 6e61 6c2d 3231  url(#terminal-21
+0000f290: 3637 3038 3133 3630 2d6c 696e 652d 3437  67081360-line-47
+0000f2a0: 2922 3e26 2331 3630 3b44 2623 3136 303b  )">&#160;D&#160;
+0000f2b0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000f2c0: 7373 3d22 7465 726d 696e 616c 2d32 3136  ss="terminal-216
+0000f2d0: 3730 3831 3336 302d 7232 3122 2078 3d22  7081360-r21" x="
+0000f2e0: 3835 3422 2079 3d22 3131 3636 2e38 2220  854" y="1166.8" 
+0000f2f0: 7465 7874 4c65 6e67 7468 3d22 3231 392e  textLength="219.
+0000f300: 3622 2063 6c69 702d 7061 7468 3d22 7572  6" clip-path="ur
+0000f310: 6c28 2374 6572 6d69 6e61 6c2d 3231 3637  l(#terminal-2167
+0000f320: 3038 3133 3630 2d6c 696e 652d 3437 2922  081360-line-47)"
+0000f330: 3e26 2331 3630 3b54 6f67 676c 6526 2331  >&#160;Toggle&#1
+0000f340: 3630 3b44 6172 6b26 2331 3630 3b4d 6f64  60;Dark&#160;Mod
+0000f350: 6526 2331 3630 3b3c 2f74 6578 743e 3c74  e&#160;</text><t
+0000f360: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000f370: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000f380: 3230 2220 783d 2231 3037 332e 3622 2079  20" x="1073.6" y
+0000f390: 3d22 3131 3636 2e38 2220 7465 7874 4c65  ="1166.8" textLe
+0000f3a0: 6e67 7468 3d22 3336 2e36 2220 636c 6970  ngth="36.6" clip
+0000f3b0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000f3c0: 696e 616c 2d32 3136 3730 3831 3336 302d  inal-2167081360-
+0000f3d0: 6c69 6e65 2d34 3729 223e 2623 3136 303b  line-47)">&#160;
+0000f3e0: 5826 2331 3630 3b3c 2f74 6578 743e 3c74  X&#160;</text><t
+0000f3f0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000f400: 6e61 6c2d 3231 3637 3038 3133 3630 2d72  nal-2167081360-r
+0000f410: 3231 2220 783d 2231 3131 302e 3222 2079  21" x="1110.2" y
+0000f420: 3d22 3131 3636 2e38 2220 7465 7874 4c65  ="1166.8" textLe
+0000f430: 6e67 7468 3d22 3138 3322 2063 6c69 702d  ngth="183" clip-
+0000f440: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000f450: 6e61 6c2d 3231 3637 3038 3133 3630 2d6c  nal-2167081360-l
+0000f460: 696e 652d 3437 2922 3e26 2331 3630 3b44  ine-47)">&#160;D
+0000f470: 6f77 6e6c 6f61 6426 2331 3630 3b46 696c  ownload&#160;Fil
+0000f480: 6526 2331 3630 3b3c 2f74 6578 743e 0a20  e&#160;</text>. 
+0000f490: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
+0000f4a0: 0a3c 2f73 7667 3e0a                      .</svg>.
```

### Comparing `browsr-1.8.0/tests/screenshots/test_github_screenshot_license.svg` & `browsr-1.9.0/tests/screenshots/test_github_screenshot_license.svg`

 * *Files 6% similar despite different names*

```diff
@@ -54,420 +54,420 @@
 00000350: 302f 776f 6666 2f46 6972 6143 6f64 652d  0/woff/FiraCode-
 00000360: 426f 6c64 2e77 6f66 6622 2920 666f 726d  Bold.woff") form
 00000370: 6174 2822 776f 6666 2229 3b0a 2020 2020  at("woff");.    
 00000380: 2020 2020 666f 6e74 2d73 7479 6c65 3a20      font-style: 
 00000390: 626f 6c64 3b0a 2020 2020 2020 2020 666f  bold;.        fo
 000003a0: 6e74 2d77 6569 6768 743a 2037 3030 3b0a  nt-weight: 700;.
 000003b0: 2020 2020 7d0a 0a20 2020 202e 7465 726d      }..    .term
-000003c0: 696e 616c 2d31 3633 3036 3736 3734 2d6d  inal-163067674-m
+000003c0: 696e 616c 2d31 3530 3832 3936 3235 2d6d  inal-150829625-m
 000003d0: 6174 7269 7820 7b0a 2020 2020 2020 2020  atrix {.        
 000003e0: 666f 6e74 2d66 616d 696c 793a 2046 6972  font-family: Fir
 000003f0: 6120 436f 6465 2c20 6d6f 6e6f 7370 6163  a Code, monospac
 00000400: 653b 0a20 2020 2020 2020 2066 6f6e 742d  e;.        font-
 00000410: 7369 7a65 3a20 3230 7078 3b0a 2020 2020  size: 20px;.    
 00000420: 2020 2020 6c69 6e65 2d68 6569 6768 743a      line-height:
 00000430: 2032 342e 3470 783b 0a20 2020 2020 2020   24.4px;.       
 00000440: 2066 6f6e 742d 7661 7269 616e 742d 6561   font-variant-ea
 00000450: 7374 2d61 7369 616e 3a20 6675 6c6c 2d77  st-asian: full-w
 00000460: 6964 7468 3b0a 2020 2020 7d0a 0a20 2020  idth;.    }..   
-00000470: 202e 7465 726d 696e 616c 2d31 3633 3036   .terminal-16306
-00000480: 3736 3734 2d74 6974 6c65 207b 0a20 2020  7674-title {.   
+00000470: 202e 7465 726d 696e 616c 2d31 3530 3832   .terminal-15082
+00000480: 3936 3235 2d74 6974 6c65 207b 0a20 2020  9625-title {.   
 00000490: 2020 2020 2066 6f6e 742d 7369 7a65 3a20       font-size: 
 000004a0: 3138 7078 3b0a 2020 2020 2020 2020 666f  18px;.        fo
 000004b0: 6e74 2d77 6569 6768 743a 2062 6f6c 643b  nt-weight: bold;
 000004c0: 0a20 2020 2020 2020 2066 6f6e 742d 6661  .        font-fa
 000004d0: 6d69 6c79 3a20 6172 6961 6c3b 0a20 2020  mily: arial;.   
 000004e0: 207d 0a0a 2020 2020 2e74 6572 6d69 6e61   }..    .termina
-000004f0: 6c2d 3136 3330 3637 3637 342d 7231 207b  l-163067674-r1 {
+000004f0: 6c2d 3135 3038 3239 3632 352d 7231 207b  l-150829625-r1 {
 00000500: 2066 696c 6c3a 2023 6335 6338 6336 207d   fill: #c5c8c6 }
-00000510: 0a2e 7465 726d 696e 616c 2d31 3633 3036  ..terminal-16306
-00000520: 3736 3734 2d72 3220 7b20 6669 6c6c 3a20  7674-r2 { fill: 
+00000510: 0a2e 7465 726d 696e 616c 2d31 3530 3832  ..terminal-15082
+00000520: 3936 3235 2d72 3220 7b20 6669 6c6c 3a20  9625-r2 { fill: 
 00000530: 2365 3065 3065 3020 7d0a 2e74 6572 6d69  #e0e0e0 }..termi
-00000540: 6e61 6c2d 3136 3330 3637 3637 342d 7233  nal-163067674-r3
+00000540: 6e61 6c2d 3135 3038 3239 3632 352d 7233  nal-150829625-r3
 00000550: 207b 2066 696c 6c3a 2023 3930 3930 3930   { fill: #909090
-00000560: 207d 0a2e 7465 726d 696e 616c 2d31 3633   }..terminal-163
-00000570: 3036 3736 3734 2d72 3420 7b20 6669 6c6c  067674-r4 { fill
+00000560: 207d 0a2e 7465 726d 696e 616c 2d31 3530   }..terminal-150
+00000570: 3832 3936 3235 2d72 3420 7b20 6669 6c6c  829625-r4 { fill
 00000580: 3a20 2364 6664 6664 6620 7d0a 2e74 6572  : #dfdfdf }..ter
-00000590: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
+00000590: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
 000005a0: 7235 207b 2066 696c 6c3a 2023 3233 3536  r5 { fill: #2356
 000005b0: 3862 207d 0a2e 7465 726d 696e 616c 2d31  8b }..terminal-1
-000005c0: 3633 3036 3736 3734 2d72 3620 7b20 6669  63067674-r6 { fi
+000005c0: 3530 3832 3936 3235 2d72 3620 7b20 6669  50829625-r6 { fi
 000005d0: 6c6c 3a20 2338 3461 3463 6320 7d0a 2e74  ll: #84a4cc }..t
-000005e0: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-000005f0: 342d 7237 207b 2066 696c 6c3a 2023 6464  4-r7 { fill: #dd
+000005e0: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+000005f0: 352d 7237 207b 2066 696c 6c3a 2023 6464  5-r7 { fill: #dd
 00000600: 6538 6633 3b66 6f6e 742d 7765 6967 6874  e8f3;font-weight
 00000610: 3a20 626f 6c64 207d 0a2e 7465 726d 696e  : bold }..termin
-00000620: 616c 2d31 3633 3036 3736 3734 2d72 3820  al-163067674-r8 
+00000620: 616c 2d31 3530 3832 3936 3235 2d72 3820  al-150829625-r8 
 00000630: 7b20 6669 6c6c 3a20 2364 6465 6466 3920  { fill: #ddedf9 
 00000640: 7d0a 2020 2020 3c2f 7374 796c 653e 0a0a  }.    </style>..
 00000650: 2020 2020 3c64 6566 733e 0a20 2020 203c      <defs>.    <
 00000660: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00000670: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
+00000670: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
 00000680: 636c 6970 2d74 6572 6d69 6e61 6c22 3e0a  clip-terminal">.
 00000690: 2020 2020 2020 3c72 6563 7420 783d 2230        <rect x="0
 000006a0: 2220 793d 2230 2220 7769 6474 683d 2231  " y="0" width="1
 000006b0: 3935 312e 3022 2068 6569 6768 743d 2231  951.0" height="1
 000006c0: 3137 302e 3139 3939 3939 3939 3939 3939  170.199999999999
 000006d0: 3822 202f 3e0a 2020 2020 3c2f 636c 6970  8" />.    </clip
 000006e0: 5061 7468 3e0a 2020 2020 3c63 6c69 7050  Path>.    <clipP
 000006f0: 6174 6820 6964 3d22 7465 726d 696e 616c  ath id="terminal
-00000700: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
+00000700: 2d31 3530 3832 3936 3235 2d6c 696e 652d  -150829625-line-
 00000710: 3022 3e0a 2020 2020 3c72 6563 7420 783d  0">.    <rect x=
 00000720: 2230 2220 793d 2231 2e35 2220 7769 6474  "0" y="1.5" widt
 00000730: 683d 2231 3935 3222 2068 6569 6768 743d  h="1952" height=
 00000740: 2232 342e 3635 222f 3e0a 2020 2020 2020  "24.65"/>.      
 00000750: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
 00000760: 3e0a 3c63 6c69 7050 6174 6820 6964 3d22  >.<clipPath id="
-00000770: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-00000780: 3734 2d6c 696e 652d 3122 3e0a 2020 2020  74-line-1">.    
+00000770: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+00000780: 3235 2d6c 696e 652d 3122 3e0a 2020 2020  25-line-1">.    
 00000790: 3c72 6563 7420 783d 2230 2220 793d 2232  <rect x="0" y="2
 000007a0: 352e 3922 2077 6964 7468 3d22 3139 3532  5.9" width="1952
 000007b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
 000007c0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
 000007d0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
 000007e0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-000007f0: 6c2d 3136 3330 3637 3637 342d 6c69 6e65  l-163067674-line
+000007f0: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
 00000800: 2d32 223e 0a20 2020 203c 7265 6374 2078  -2">.    <rect x
 00000810: 3d22 3022 2079 3d22 3530 2e33 2220 7769  ="0" y="50.3" wi
 00000820: 6474 683d 2231 3935 3222 2068 6569 6768  dth="1952" heigh
 00000830: 743d 2232 342e 3635 222f 3e0a 2020 2020  t="24.65"/>.    
 00000840: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
 00000850: 7468 3e0a 3c63 6c69 7050 6174 6820 6964  th>.<clipPath id
-00000860: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00000870: 3736 3734 2d6c 696e 652d 3322 3e0a 2020  7674-line-3">.  
+00000860: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+00000870: 3936 3235 2d6c 696e 652d 3322 3e0a 2020  9625-line-3">.  
 00000880: 2020 3c72 6563 7420 783d 2230 2220 793d    <rect x="0" y=
 00000890: 2237 342e 3722 2077 6964 7468 3d22 3139  "74.7" width="19
 000008a0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
 000008b0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
 000008c0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
 000008d0: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
-000008e0: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
+000008e0: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
 000008f0: 6e65 2d34 223e 0a20 2020 203c 7265 6374  ne-4">.    <rect
 00000900: 2078 3d22 3022 2079 3d22 3939 2e31 2220   x="0" y="99.1" 
 00000910: 7769 6474 683d 2231 3935 3222 2068 6569  width="1952" hei
 00000920: 6768 743d 2232 342e 3635 222f 3e0a 2020  ght="24.65"/>.  
 00000930: 2020 2020 2020 2020 2020 3c2f 636c 6970            </clip
 00000940: 5061 7468 3e0a 3c63 6c69 7050 6174 6820  Path>.<clipPath 
-00000950: 6964 3d22 7465 726d 696e 616c 2d31 3633  id="terminal-163
-00000960: 3036 3736 3734 2d6c 696e 652d 3522 3e0a  067674-line-5">.
+00000950: 6964 3d22 7465 726d 696e 616c 2d31 3530  id="terminal-150
+00000960: 3832 3936 3235 2d6c 696e 652d 3522 3e0a  829625-line-5">.
 00000970: 2020 2020 3c72 6563 7420 783d 2230 2220      <rect x="0" 
 00000980: 793d 2231 3233 2e35 2220 7769 6474 683d  y="123.5" width=
 00000990: 2231 3935 3222 2068 6569 6768 743d 2232  "1952" height="2
 000009a0: 342e 3635 222f 3e0a 2020 2020 2020 2020  4.65"/>.        
 000009b0: 2020 2020 3c2f 636c 6970 5061 7468 3e0a      </clipPath>.
 000009c0: 3c63 6c69 7050 6174 6820 6964 3d22 7465  <clipPath id="te
-000009d0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
+000009d0: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
 000009e0: 2d6c 696e 652d 3622 3e0a 2020 2020 3c72  -line-6">.    <r
 000009f0: 6563 7420 783d 2230 2220 793d 2231 3437  ect x="0" y="147
 00000a00: 2e39 2220 7769 6474 683d 2231 3935 3222  .9" width="1952"
 00000a10: 2068 6569 6768 743d 2232 342e 3635 222f   height="24.65"/
 00000a20: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
 00000a30: 636c 6970 5061 7468 3e0a 3c63 6c69 7050  clipPath>.<clipP
 00000a40: 6174 6820 6964 3d22 7465 726d 696e 616c  ath id="terminal
-00000a50: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
+00000a50: 2d31 3530 3832 3936 3235 2d6c 696e 652d  -150829625-line-
 00000a60: 3722 3e0a 2020 2020 3c72 6563 7420 783d  7">.    <rect x=
 00000a70: 2230 2220 793d 2231 3732 2e33 2220 7769  "0" y="172.3" wi
 00000a80: 6474 683d 2231 3935 3222 2068 6569 6768  dth="1952" heigh
 00000a90: 743d 2232 342e 3635 222f 3e0a 2020 2020  t="24.65"/>.    
 00000aa0: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
 00000ab0: 7468 3e0a 3c63 6c69 7050 6174 6820 6964  th>.<clipPath id
-00000ac0: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00000ad0: 3736 3734 2d6c 696e 652d 3822 3e0a 2020  7674-line-8">.  
+00000ac0: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+00000ad0: 3936 3235 2d6c 696e 652d 3822 3e0a 2020  9625-line-8">.  
 00000ae0: 2020 3c72 6563 7420 783d 2230 2220 793d    <rect x="0" y=
 00000af0: 2231 3936 2e37 2220 7769 6474 683d 2231  "196.7" width="1
 00000b00: 3935 3222 2068 6569 6768 743d 2232 342e  952" height="24.
 00000b10: 3635 222f 3e0a 2020 2020 2020 2020 2020  65"/>.          
 00000b20: 2020 3c2f 636c 6970 5061 7468 3e0a 3c63    </clipPath>.<c
 00000b30: 6c69 7050 6174 6820 6964 3d22 7465 726d  lipPath id="term
-00000b40: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
+00000b40: 696e 616c 2d31 3530 3832 3936 3235 2d6c  inal-150829625-l
 00000b50: 696e 652d 3922 3e0a 2020 2020 3c72 6563  ine-9">.    <rec
 00000b60: 7420 783d 2230 2220 793d 2232 3231 2e31  t x="0" y="221.1
 00000b70: 2220 7769 6474 683d 2231 3935 3222 2068  " width="1952" h
 00000b80: 6569 6768 743d 2232 342e 3635 222f 3e0a  eight="24.65"/>.
 00000b90: 2020 2020 2020 2020 2020 2020 3c2f 636c              </cl
 00000ba0: 6970 5061 7468 3e0a 3c63 6c69 7050 6174  ipPath>.<clipPat
 00000bb0: 6820 6964 3d22 7465 726d 696e 616c 2d31  h id="terminal-1
-00000bc0: 3633 3036 3736 3734 2d6c 696e 652d 3130  63067674-line-10
+00000bc0: 3530 3832 3936 3235 2d6c 696e 652d 3130  50829625-line-10
 00000bd0: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
 00000be0: 3022 2079 3d22 3234 352e 3522 2077 6964  0" y="245.5" wid
 00000bf0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
 00000c00: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
 00000c10: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
 00000c20: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-00000c30: 2274 6572 6d69 6e61 6c2d 3136 3330 3637  "terminal-163067
-00000c40: 3637 342d 6c69 6e65 2d31 3122 3e0a 2020  674-line-11">.  
+00000c30: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+00000c40: 3632 352d 6c69 6e65 2d31 3122 3e0a 2020  625-line-11">.  
 00000c50: 2020 3c72 6563 7420 783d 2230 2220 793d    <rect x="0" y=
 00000c60: 2232 3639 2e39 2220 7769 6474 683d 2231  "269.9" width="1
 00000c70: 3935 3222 2068 6569 6768 743d 2232 342e  952" height="24.
 00000c80: 3635 222f 3e0a 2020 2020 2020 2020 2020  65"/>.          
 00000c90: 2020 3c2f 636c 6970 5061 7468 3e0a 3c63    </clipPath>.<c
 00000ca0: 6c69 7050 6174 6820 6964 3d22 7465 726d  lipPath id="term
-00000cb0: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
+00000cb0: 696e 616c 2d31 3530 3832 3936 3235 2d6c  inal-150829625-l
 00000cc0: 696e 652d 3132 223e 0a20 2020 203c 7265  ine-12">.    <re
 00000cd0: 6374 2078 3d22 3022 2079 3d22 3239 342e  ct x="0" y="294.
 00000ce0: 3322 2077 6964 7468 3d22 3139 3532 2220  3" width="1952" 
 00000cf0: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
 00000d00: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
 00000d10: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
 00000d20: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
-00000d30: 3136 3330 3637 3637 342d 6c69 6e65 2d31  163067674-line-1
+00000d30: 3135 3038 3239 3632 352d 6c69 6e65 2d31  150829625-line-1
 00000d40: 3322 3e0a 2020 2020 3c72 6563 7420 783d  3">.    <rect x=
 00000d50: 2230 2220 793d 2233 3138 2e37 2220 7769  "0" y="318.7" wi
 00000d60: 6474 683d 2231 3935 3222 2068 6569 6768  dth="1952" heigh
 00000d70: 743d 2232 342e 3635 222f 3e0a 2020 2020  t="24.65"/>.    
 00000d80: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
 00000d90: 7468 3e0a 3c63 6c69 7050 6174 6820 6964  th>.<clipPath id
-00000da0: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00000db0: 3736 3734 2d6c 696e 652d 3134 223e 0a20  7674-line-14">. 
+00000da0: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+00000db0: 3936 3235 2d6c 696e 652d 3134 223e 0a20  9625-line-14">. 
 00000dc0: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
 00000dd0: 3d22 3334 332e 3122 2077 6964 7468 3d22  ="343.1" width="
 00000de0: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
 00000df0: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
 00000e00: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
 00000e10: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-00000e20: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
+00000e20: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
 00000e30: 6c69 6e65 2d31 3522 3e0a 2020 2020 3c72  line-15">.    <r
 00000e40: 6563 7420 783d 2230 2220 793d 2233 3637  ect x="0" y="367
 00000e50: 2e35 2220 7769 6474 683d 2231 3935 3222  .5" width="1952"
 00000e60: 2068 6569 6768 743d 2232 342e 3635 222f   height="24.65"/
 00000e70: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
 00000e80: 636c 6970 5061 7468 3e0a 3c63 6c69 7050  clipPath>.<clipP
 00000e90: 6174 6820 6964 3d22 7465 726d 696e 616c  ath id="terminal
-00000ea0: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
+00000ea0: 2d31 3530 3832 3936 3235 2d6c 696e 652d  -150829625-line-
 00000eb0: 3136 223e 0a20 2020 203c 7265 6374 2078  16">.    <rect x
 00000ec0: 3d22 3022 2079 3d22 3339 312e 3922 2077  ="0" y="391.9" w
 00000ed0: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
 00000ee0: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
 00000ef0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
 00000f00: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
-00000f10: 643d 2274 6572 6d69 6e61 6c2d 3136 3330  d="terminal-1630
-00000f20: 3637 3637 342d 6c69 6e65 2d31 3722 3e0a  67674-line-17">.
+00000f10: 643d 2274 6572 6d69 6e61 6c2d 3135 3038  d="terminal-1508
+00000f20: 3239 3632 352d 6c69 6e65 2d31 3722 3e0a  29625-line-17">.
 00000f30: 2020 2020 3c72 6563 7420 783d 2230 2220      <rect x="0" 
 00000f40: 793d 2234 3136 2e33 2220 7769 6474 683d  y="416.3" width=
 00000f50: 2231 3935 3222 2068 6569 6768 743d 2232  "1952" height="2
 00000f60: 342e 3635 222f 3e0a 2020 2020 2020 2020  4.65"/>.        
 00000f70: 2020 2020 3c2f 636c 6970 5061 7468 3e0a      </clipPath>.
 00000f80: 3c63 6c69 7050 6174 6820 6964 3d22 7465  <clipPath id="te
-00000f90: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
+00000f90: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
 00000fa0: 2d6c 696e 652d 3138 223e 0a20 2020 203c  -line-18">.    <
 00000fb0: 7265 6374 2078 3d22 3022 2079 3d22 3434  rect x="0" y="44
 00000fc0: 302e 3722 2077 6964 7468 3d22 3139 3532  0.7" width="1952
 00000fd0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
 00000fe0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
 00000ff0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
 00001000: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-00001010: 6c2d 3136 3330 3637 3637 342d 6c69 6e65  l-163067674-line
+00001010: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
 00001020: 2d31 3922 3e0a 2020 2020 3c72 6563 7420  -19">.    <rect 
 00001030: 783d 2230 2220 793d 2234 3635 2e31 2220  x="0" y="465.1" 
 00001040: 7769 6474 683d 2231 3935 3222 2068 6569  width="1952" hei
 00001050: 6768 743d 2232 342e 3635 222f 3e0a 2020  ght="24.65"/>.  
 00001060: 2020 2020 2020 2020 2020 3c2f 636c 6970            </clip
 00001070: 5061 7468 3e0a 3c63 6c69 7050 6174 6820  Path>.<clipPath 
-00001080: 6964 3d22 7465 726d 696e 616c 2d31 3633  id="terminal-163
-00001090: 3036 3736 3734 2d6c 696e 652d 3230 223e  067674-line-20">
+00001080: 6964 3d22 7465 726d 696e 616c 2d31 3530  id="terminal-150
+00001090: 3832 3936 3235 2d6c 696e 652d 3230 223e  829625-line-20">
 000010a0: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
 000010b0: 2079 3d22 3438 392e 3522 2077 6964 7468   y="489.5" width
 000010c0: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
 000010d0: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
 000010e0: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
 000010f0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
-00001100: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-00001110: 342d 6c69 6e65 2d32 3122 3e0a 2020 2020  4-line-21">.    
+00001100: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+00001110: 352d 6c69 6e65 2d32 3122 3e0a 2020 2020  5-line-21">.    
 00001120: 3c72 6563 7420 783d 2230 2220 793d 2235  <rect x="0" y="5
 00001130: 3133 2e39 2220 7769 6474 683d 2231 3935  13.9" width="195
 00001140: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
 00001150: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
 00001160: 3c2f 636c 6970 5061 7468 3e0a 3c63 6c69  </clipPath>.<cli
 00001170: 7050 6174 6820 6964 3d22 7465 726d 696e  pPath id="termin
-00001180: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
+00001180: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
 00001190: 652d 3232 223e 0a20 2020 203c 7265 6374  e-22">.    <rect
 000011a0: 2078 3d22 3022 2079 3d22 3533 382e 3322   x="0" y="538.3"
 000011b0: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
 000011c0: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
 000011d0: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
 000011e0: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-000011f0: 2069 643d 2274 6572 6d69 6e61 6c2d 3136   id="terminal-16
-00001200: 3330 3637 3637 342d 6c69 6e65 2d32 3322  3067674-line-23"
+000011f0: 2069 643d 2274 6572 6d69 6e61 6c2d 3135   id="terminal-15
+00001200: 3038 3239 3632 352d 6c69 6e65 2d32 3322  0829625-line-23"
 00001210: 3e0a 2020 2020 3c72 6563 7420 783d 2230  >.    <rect x="0
 00001220: 2220 793d 2235 3632 2e37 2220 7769 6474  " y="562.7" widt
 00001230: 683d 2231 3935 3222 2068 6569 6768 743d  h="1952" height=
 00001240: 2232 342e 3635 222f 3e0a 2020 2020 2020  "24.65"/>.      
 00001250: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
 00001260: 3e0a 3c63 6c69 7050 6174 6820 6964 3d22  >.<clipPath id="
-00001270: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-00001280: 3734 2d6c 696e 652d 3234 223e 0a20 2020  74-line-24">.   
+00001270: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+00001280: 3235 2d6c 696e 652d 3234 223e 0a20 2020  25-line-24">.   
 00001290: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
 000012a0: 3538 372e 3122 2077 6964 7468 3d22 3139  587.1" width="19
 000012b0: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
 000012c0: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
 000012d0: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
 000012e0: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
-000012f0: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
+000012f0: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
 00001300: 6e65 2d32 3522 3e0a 2020 2020 3c72 6563  ne-25">.    <rec
 00001310: 7420 783d 2230 2220 793d 2236 3131 2e35  t x="0" y="611.5
 00001320: 2220 7769 6474 683d 2231 3935 3222 2068  " width="1952" h
 00001330: 6569 6768 743d 2232 342e 3635 222f 3e0a  eight="24.65"/>.
 00001340: 2020 2020 2020 2020 2020 2020 3c2f 636c              </cl
 00001350: 6970 5061 7468 3e0a 3c63 6c69 7050 6174  ipPath>.<clipPat
 00001360: 6820 6964 3d22 7465 726d 696e 616c 2d31  h id="terminal-1
-00001370: 3633 3036 3736 3734 2d6c 696e 652d 3236  63067674-line-26
+00001370: 3530 3832 3936 3235 2d6c 696e 652d 3236  50829625-line-26
 00001380: 223e 0a20 2020 203c 7265 6374 2078 3d22  ">.    <rect x="
 00001390: 3022 2079 3d22 3633 352e 3922 2077 6964  0" y="635.9" wid
 000013a0: 7468 3d22 3139 3532 2220 6865 6967 6874  th="1952" height
 000013b0: 3d22 3234 2e36 3522 2f3e 0a20 2020 2020  ="24.65"/>.     
 000013c0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
 000013d0: 683e 0a3c 636c 6970 5061 7468 2069 643d  h>.<clipPath id=
-000013e0: 2274 6572 6d69 6e61 6c2d 3136 3330 3637  "terminal-163067
-000013f0: 3637 342d 6c69 6e65 2d32 3722 3e0a 2020  674-line-27">.  
+000013e0: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+000013f0: 3632 352d 6c69 6e65 2d32 3722 3e0a 2020  625-line-27">.  
 00001400: 2020 3c72 6563 7420 783d 2230 2220 793d    <rect x="0" y=
 00001410: 2236 3630 2e33 2220 7769 6474 683d 2231  "660.3" width="1
 00001420: 3935 3222 2068 6569 6768 743d 2232 342e  952" height="24.
 00001430: 3635 222f 3e0a 2020 2020 2020 2020 2020  65"/>.          
 00001440: 2020 3c2f 636c 6970 5061 7468 3e0a 3c63    </clipPath>.<c
 00001450: 6c69 7050 6174 6820 6964 3d22 7465 726d  lipPath id="term
-00001460: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
+00001460: 696e 616c 2d31 3530 3832 3936 3235 2d6c  inal-150829625-l
 00001470: 696e 652d 3238 223e 0a20 2020 203c 7265  ine-28">.    <re
 00001480: 6374 2078 3d22 3022 2079 3d22 3638 342e  ct x="0" y="684.
 00001490: 3722 2077 6964 7468 3d22 3139 3532 2220  7" width="1952" 
 000014a0: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
 000014b0: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
 000014c0: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
 000014d0: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
-000014e0: 3136 3330 3637 3637 342d 6c69 6e65 2d32  163067674-line-2
+000014e0: 3135 3038 3239 3632 352d 6c69 6e65 2d32  150829625-line-2
 000014f0: 3922 3e0a 2020 2020 3c72 6563 7420 783d  9">.    <rect x=
 00001500: 2230 2220 793d 2237 3039 2e31 2220 7769  "0" y="709.1" wi
 00001510: 6474 683d 2231 3935 3222 2068 6569 6768  dth="1952" heigh
 00001520: 743d 2232 342e 3635 222f 3e0a 2020 2020  t="24.65"/>.    
 00001530: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
 00001540: 7468 3e0a 3c63 6c69 7050 6174 6820 6964  th>.<clipPath id
-00001550: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00001560: 3736 3734 2d6c 696e 652d 3330 223e 0a20  7674-line-30">. 
+00001550: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+00001560: 3936 3235 2d6c 696e 652d 3330 223e 0a20  9625-line-30">. 
 00001570: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
 00001580: 3d22 3733 332e 3522 2077 6964 7468 3d22  ="733.5" width="
 00001590: 3139 3532 2220 6865 6967 6874 3d22 3234  1952" height="24
 000015a0: 2e36 3522 2f3e 0a20 2020 2020 2020 2020  .65"/>.         
 000015b0: 2020 203c 2f63 6c69 7050 6174 683e 0a3c     </clipPath>.<
 000015c0: 636c 6970 5061 7468 2069 643d 2274 6572  clipPath id="ter
-000015d0: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
+000015d0: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
 000015e0: 6c69 6e65 2d33 3122 3e0a 2020 2020 3c72  line-31">.    <r
 000015f0: 6563 7420 783d 2230 2220 793d 2237 3537  ect x="0" y="757
 00001600: 2e39 2220 7769 6474 683d 2231 3935 3222  .9" width="1952"
 00001610: 2068 6569 6768 743d 2232 342e 3635 222f   height="24.65"/
 00001620: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
 00001630: 636c 6970 5061 7468 3e0a 3c63 6c69 7050  clipPath>.<clipP
 00001640: 6174 6820 6964 3d22 7465 726d 696e 616c  ath id="terminal
-00001650: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
+00001650: 2d31 3530 3832 3936 3235 2d6c 696e 652d  -150829625-line-
 00001660: 3332 223e 0a20 2020 203c 7265 6374 2078  32">.    <rect x
 00001670: 3d22 3022 2079 3d22 3738 322e 3322 2077  ="0" y="782.3" w
 00001680: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
 00001690: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
 000016a0: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
 000016b0: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
-000016c0: 643d 2274 6572 6d69 6e61 6c2d 3136 3330  d="terminal-1630
-000016d0: 3637 3637 342d 6c69 6e65 2d33 3322 3e0a  67674-line-33">.
+000016c0: 643d 2274 6572 6d69 6e61 6c2d 3135 3038  d="terminal-1508
+000016d0: 3239 3632 352d 6c69 6e65 2d33 3322 3e0a  29625-line-33">.
 000016e0: 2020 2020 3c72 6563 7420 783d 2230 2220      <rect x="0" 
 000016f0: 793d 2238 3036 2e37 2220 7769 6474 683d  y="806.7" width=
 00001700: 2231 3935 3222 2068 6569 6768 743d 2232  "1952" height="2
 00001710: 342e 3635 222f 3e0a 2020 2020 2020 2020  4.65"/>.        
 00001720: 2020 2020 3c2f 636c 6970 5061 7468 3e0a      </clipPath>.
 00001730: 3c63 6c69 7050 6174 6820 6964 3d22 7465  <clipPath id="te
-00001740: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
+00001740: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
 00001750: 2d6c 696e 652d 3334 223e 0a20 2020 203c  -line-34">.    <
 00001760: 7265 6374 2078 3d22 3022 2079 3d22 3833  rect x="0" y="83
 00001770: 312e 3122 2077 6964 7468 3d22 3139 3532  1.1" width="1952
 00001780: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
 00001790: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
 000017a0: 2f63 6c69 7050 6174 683e 0a3c 636c 6970  /clipPath>.<clip
 000017b0: 5061 7468 2069 643d 2274 6572 6d69 6e61  Path id="termina
-000017c0: 6c2d 3136 3330 3637 3637 342d 6c69 6e65  l-163067674-line
+000017c0: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
 000017d0: 2d33 3522 3e0a 2020 2020 3c72 6563 7420  -35">.    <rect 
 000017e0: 783d 2230 2220 793d 2238 3535 2e35 2220  x="0" y="855.5" 
 000017f0: 7769 6474 683d 2231 3935 3222 2068 6569  width="1952" hei
 00001800: 6768 743d 2232 342e 3635 222f 3e0a 2020  ght="24.65"/>.  
 00001810: 2020 2020 2020 2020 2020 3c2f 636c 6970            </clip
 00001820: 5061 7468 3e0a 3c63 6c69 7050 6174 6820  Path>.<clipPath 
-00001830: 6964 3d22 7465 726d 696e 616c 2d31 3633  id="terminal-163
-00001840: 3036 3736 3734 2d6c 696e 652d 3336 223e  067674-line-36">
+00001830: 6964 3d22 7465 726d 696e 616c 2d31 3530  id="terminal-150
+00001840: 3832 3936 3235 2d6c 696e 652d 3336 223e  829625-line-36">
 00001850: 0a20 2020 203c 7265 6374 2078 3d22 3022  .    <rect x="0"
 00001860: 2079 3d22 3837 392e 3922 2077 6964 7468   y="879.9" width
 00001870: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
 00001880: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
 00001890: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
 000018a0: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
-000018b0: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-000018c0: 342d 6c69 6e65 2d33 3722 3e0a 2020 2020  4-line-37">.    
+000018b0: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+000018c0: 352d 6c69 6e65 2d33 3722 3e0a 2020 2020  5-line-37">.    
 000018d0: 3c72 6563 7420 783d 2230 2220 793d 2239  <rect x="0" y="9
 000018e0: 3034 2e33 2220 7769 6474 683d 2231 3935  04.3" width="195
 000018f0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
 00001900: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
 00001910: 3c2f 636c 6970 5061 7468 3e0a 3c63 6c69  </clipPath>.<cli
 00001920: 7050 6174 6820 6964 3d22 7465 726d 696e  pPath id="termin
-00001930: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
+00001930: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
 00001940: 652d 3338 223e 0a20 2020 203c 7265 6374  e-38">.    <rect
 00001950: 2078 3d22 3022 2079 3d22 3932 382e 3722   x="0" y="928.7"
 00001960: 2077 6964 7468 3d22 3139 3532 2220 6865   width="1952" he
 00001970: 6967 6874 3d22 3234 2e36 3522 2f3e 0a20  ight="24.65"/>. 
 00001980: 2020 2020 2020 2020 2020 203c 2f63 6c69             </cli
 00001990: 7050 6174 683e 0a3c 636c 6970 5061 7468  pPath>.<clipPath
-000019a0: 2069 643d 2274 6572 6d69 6e61 6c2d 3136   id="terminal-16
-000019b0: 3330 3637 3637 342d 6c69 6e65 2d33 3922  3067674-line-39"
+000019a0: 2069 643d 2274 6572 6d69 6e61 6c2d 3135   id="terminal-15
+000019b0: 3038 3239 3632 352d 6c69 6e65 2d33 3922  0829625-line-39"
 000019c0: 3e0a 2020 2020 3c72 6563 7420 783d 2230  >.    <rect x="0
 000019d0: 2220 793d 2239 3533 2e31 2220 7769 6474  " y="953.1" widt
 000019e0: 683d 2231 3935 3222 2068 6569 6768 743d  h="1952" height=
 000019f0: 2232 342e 3635 222f 3e0a 2020 2020 2020  "24.65"/>.      
 00001a00: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
 00001a10: 3e0a 3c63 6c69 7050 6174 6820 6964 3d22  >.<clipPath id="
-00001a20: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-00001a30: 3734 2d6c 696e 652d 3430 223e 0a20 2020  74-line-40">.   
+00001a20: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+00001a30: 3235 2d6c 696e 652d 3430 223e 0a20 2020  25-line-40">.   
 00001a40: 203c 7265 6374 2078 3d22 3022 2079 3d22   <rect x="0" y="
 00001a50: 3937 372e 3522 2077 6964 7468 3d22 3139  977.5" width="19
 00001a60: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
 00001a70: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
 00001a80: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
 00001a90: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
-00001aa0: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
+00001aa0: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
 00001ab0: 6e65 2d34 3122 3e0a 2020 2020 3c72 6563  ne-41">.    <rec
 00001ac0: 7420 783d 2230 2220 793d 2231 3030 312e  t x="0" y="1001.
 00001ad0: 3922 2077 6964 7468 3d22 3139 3532 2220  9" width="1952" 
 00001ae0: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
 00001af0: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
 00001b00: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
 00001b10: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
-00001b20: 3136 3330 3637 3637 342d 6c69 6e65 2d34  163067674-line-4
+00001b20: 3135 3038 3239 3632 352d 6c69 6e65 2d34  150829625-line-4
 00001b30: 3222 3e0a 2020 2020 3c72 6563 7420 783d  2">.    <rect x=
 00001b40: 2230 2220 793d 2231 3032 362e 3322 2077  "0" y="1026.3" w
 00001b50: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
 00001b60: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
 00001b70: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
 00001b80: 6174 683e 0a3c 636c 6970 5061 7468 2069  ath>.<clipPath i
-00001b90: 643d 2274 6572 6d69 6e61 6c2d 3136 3330  d="terminal-1630
-00001ba0: 3637 3637 342d 6c69 6e65 2d34 3322 3e0a  67674-line-43">.
+00001b90: 643d 2274 6572 6d69 6e61 6c2d 3135 3038  d="terminal-1508
+00001ba0: 3239 3632 352d 6c69 6e65 2d34 3322 3e0a  29625-line-43">.
 00001bb0: 2020 2020 3c72 6563 7420 783d 2230 2220      <rect x="0" 
 00001bc0: 793d 2231 3035 302e 3722 2077 6964 7468  y="1050.7" width
 00001bd0: 3d22 3139 3532 2220 6865 6967 6874 3d22  ="1952" height="
 00001be0: 3234 2e36 3522 2f3e 0a20 2020 2020 2020  24.65"/>.       
 00001bf0: 2020 2020 203c 2f63 6c69 7050 6174 683e       </clipPath>
 00001c00: 0a3c 636c 6970 5061 7468 2069 643d 2274  .<clipPath id="t
-00001c10: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-00001c20: 342d 6c69 6e65 2d34 3422 3e0a 2020 2020  4-line-44">.    
+00001c10: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+00001c20: 352d 6c69 6e65 2d34 3422 3e0a 2020 2020  5-line-44">.    
 00001c30: 3c72 6563 7420 783d 2230 2220 793d 2231  <rect x="0" y="1
 00001c40: 3037 352e 3122 2077 6964 7468 3d22 3139  075.1" width="19
 00001c50: 3532 2220 6865 6967 6874 3d22 3234 2e36  52" height="24.6
 00001c60: 3522 2f3e 0a20 2020 2020 2020 2020 2020  5"/>.           
 00001c70: 203c 2f63 6c69 7050 6174 683e 0a3c 636c   </clipPath>.<cl
 00001c80: 6970 5061 7468 2069 643d 2274 6572 6d69  ipPath id="termi
-00001c90: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
+00001c90: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
 00001ca0: 6e65 2d34 3522 3e0a 2020 2020 3c72 6563  ne-45">.    <rec
 00001cb0: 7420 783d 2230 2220 793d 2231 3039 392e  t x="0" y="1099.
 00001cc0: 3522 2077 6964 7468 3d22 3139 3532 2220  5" width="1952" 
 00001cd0: 6865 6967 6874 3d22 3234 2e36 3522 2f3e  height="24.65"/>
 00001ce0: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
 00001cf0: 6c69 7050 6174 683e 0a3c 636c 6970 5061  lipPath>.<clipPa
 00001d00: 7468 2069 643d 2274 6572 6d69 6e61 6c2d  th id="terminal-
-00001d10: 3136 3330 3637 3637 342d 6c69 6e65 2d34  163067674-line-4
+00001d10: 3135 3038 3239 3632 352d 6c69 6e65 2d34  150829625-line-4
 00001d20: 3622 3e0a 2020 2020 3c72 6563 7420 783d  6">.    <rect x=
 00001d30: 2230 2220 793d 2231 3132 332e 3922 2077  "0" y="1123.9" w
 00001d40: 6964 7468 3d22 3139 3532 2220 6865 6967  idth="1952" heig
 00001d50: 6874 3d22 3234 2e36 3522 2f3e 0a20 2020  ht="24.65"/>.   
 00001d60: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
 00001d70: 6174 683e 0a20 2020 203c 2f64 6566 733e  ath>.    </defs>
 00001d80: 0a0a 2020 2020 3c72 6563 7420 6669 6c6c  ..    <rect fill
@@ -475,15 +475,15 @@
 00001da0: 653d 2272 6762 6128 3235 352c 3235 352c  e="rgba(255,255,
 00001db0: 3235 352c 302e 3335 2922 2073 7472 6f6b  255,0.35)" strok
 00001dc0: 652d 7769 6474 683d 2231 2220 783d 2231  e-width="1" x="1
 00001dd0: 2220 793d 2231 2220 7769 6474 683d 2231  " y="1" width="1
 00001de0: 3936 3822 2068 6569 6768 743d 2231 3231  968" height="121
 00001df0: 392e 3222 2072 783d 2238 222f 3e3c 7465  9.2" rx="8"/><te
 00001e00: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-00001e10: 616c 2d31 3633 3036 3736 3734 2d74 6974  al-163067674-tit
+00001e10: 616c 2d31 3530 3832 3936 3235 2d74 6974  al-150829625-tit
 00001e20: 6c65 2220 6669 6c6c 3d22 2363 3563 3863  le" fill="#c5c8c
 00001e30: 3622 2074 6578 742d 616e 6368 6f72 3d22  6" text-anchor="
 00001e40: 6d69 6464 6c65 2220 783d 2239 3834 2220  middle" x="984" 
 00001e50: 793d 2232 3722 3e62 726f 7773 723c 2f74  y="27">browsr</t
 00001e60: 6578 743e 0a20 2020 2020 2020 2020 2020  ext>.           
 00001e70: 203c 6720 7472 616e 7366 6f72 6d3d 2274   <g transform="t
 00001e80: 7261 6e73 6c61 7465 2832 362c 3232 2922  ranslate(26,22)"
@@ -499,15 +499,15 @@
 00001f20: 2063 793d 2230 2220 723d 2237 2220 6669   cy="0" r="7" fi
 00001f30: 6c6c 3d22 2332 3863 3834 3022 2f3e 0a20  ll="#28c840"/>. 
 00001f40: 2020 2020 2020 2020 2020 203c 2f67 3e0a             </g>.
 00001f50: 2020 2020 2020 2020 0a20 2020 203c 6720          .    <g 
 00001f60: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
 00001f70: 6c61 7465 2839 2c20 3431 2922 2063 6c69  late(9, 41)" cli
 00001f80: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-00001f90: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
+00001f90: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
 00001fa0: 636c 6970 2d74 6572 6d69 6e61 6c29 223e  clip-terminal)">
 00001fb0: 0a20 2020 203c 7265 6374 2066 696c 6c3d  .    <rect fill=
 00001fc0: 2223 3138 3138 3138 2220 783d 2230 2220  "#181818" x="0" 
 00001fd0: 793d 2231 2e35 2220 7769 6474 683d 2231  y="1.5" width="1
 00001fe0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
 00001ff0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
 00002000: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
@@ -558,2389 +558,2395 @@
 000022d0: 3330 2220 793d 2231 2e35 2220 7769 6474  30" y="1.5" widt
 000022e0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
 000022f0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
 00002300: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
 00002310: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
 00002320: 3d22 2331 3831 3831 3822 2078 3d22 3138  ="#181818" x="18
 00002330: 3432 2e32 2220 793d 2231 2e35 2220 7769  42.2" y="1.5" wi
-00002340: 6474 683d 2239 372e 3622 2068 6569 6768  dth="97.6" heigh
-00002350: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00002360: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00002370: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00002380: 6c6c 3d22 2331 3831 3831 3822 2078 3d22  ll="#181818" x="
-00002390: 3139 3339 2e38 2220 793d 2231 2e35 2220  1939.8" y="1.5" 
-000023a0: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-000023b0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000023c0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000023d0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000023e0: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
-000023f0: 3d22 3022 2079 3d22 3235 2e39 2220 7769  ="0" y="25.9" wi
-00002400: 6474 683d 2231 3932 372e 3622 2068 6569  dth="1927.6" hei
-00002410: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00002420: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00002430: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00002440: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00002450: 3d22 3139 3237 2e36 2220 793d 2232 352e  ="1927.6" y="25.
-00002460: 3922 2077 6964 7468 3d22 3234 2e34 2220  9" width="24.4" 
-00002470: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00002480: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00002490: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-000024a0: 6374 2066 696c 6c3d 2223 3237 3238 3232  ct fill="#272822
-000024b0: 2220 783d 2230 2220 793d 2235 302e 3322  " x="0" y="50.3"
-000024c0: 2077 6964 7468 3d22 3139 3237 2e36 2220   width="1927.6" 
-000024d0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-000024e0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-000024f0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00002500: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-00002510: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00002520: 3530 2e33 2220 7769 6474 683d 2232 342e  50.3" width="24.
-00002530: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00002540: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00002550: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00002560: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
-00002570: 3832 3222 2078 3d22 3022 2079 3d22 3734  822" x="0" y="74
-00002580: 2e37 2220 7769 6474 683d 2231 3932 372e  .7" width="1927.
-00002590: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
-000025a0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000025b0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000025c0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-000025d0: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
-000025e0: 793d 2237 342e 3722 2077 6964 7468 3d22  y="74.7" width="
-000025f0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-00002600: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00002610: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00002620: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00002630: 3237 3238 3232 2220 783d 2230 2220 793d  272822" x="0" y=
-00002640: 2239 392e 3122 2077 6964 7468 3d22 3139  "99.1" width="19
-00002650: 3237 2e36 2220 6865 6967 6874 3d22 3234  27.6" height="24
-00002660: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00002670: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00002680: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00002690: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
-000026a0: 3622 2079 3d22 3939 2e31 2220 7769 6474  6" y="99.1" widt
-000026b0: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
-000026c0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000026d0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000026e0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000026f0: 3d22 2332 3732 3832 3222 2078 3d22 3022  ="#272822" x="0"
-00002700: 2079 3d22 3132 332e 3522 2077 6964 7468   y="123.5" width
-00002710: 3d22 3139 3237 2e36 2220 6865 6967 6874  ="1927.6" height
-00002720: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00002730: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00002740: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00002750: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00002760: 3932 372e 3622 2079 3d22 3132 332e 3522  927.6" y="123.5"
-00002770: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-00002780: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00002790: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-000027a0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-000027b0: 2066 696c 6c3d 2223 3237 3238 3232 2220   fill="#272822" 
-000027c0: 783d 2230 2220 793d 2231 3437 2e39 2220  x="0" y="147.9" 
-000027d0: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
-000027e0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000027f0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00002800: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00002810: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00002820: 2078 3d22 3139 3237 2e36 2220 793d 2231   x="1927.6" y="1
-00002830: 3437 2e39 2220 7769 6474 683d 2232 342e  47.9" width="24.
-00002840: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-00002850: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00002860: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00002870: 3c72 6563 7420 6669 6c6c 3d22 2332 3732  <rect fill="#272
-00002880: 3832 3222 2078 3d22 3022 2079 3d22 3137  822" x="0" y="17
-00002890: 322e 3322 2077 6964 7468 3d22 3139 3237  2.3" width="1927
-000028a0: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
-000028b0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000028c0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000028d0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-000028e0: 3139 3166 2220 783d 2231 3932 372e 3622  191f" x="1927.6"
-000028f0: 2079 3d22 3137 322e 3322 2077 6964 7468   y="172.3" width
-00002900: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
-00002910: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00002920: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00002930: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00002940: 2223 3237 3238 3232 2220 783d 2230 2220  "#272822" x="0" 
-00002950: 793d 2231 3936 2e37 2220 7769 6474 683d  y="196.7" width=
-00002960: 2231 3932 372e 3622 2068 6569 6768 743d  "1927.6" height=
-00002970: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00002980: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00002990: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000029a0: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
-000029b0: 3237 2e36 2220 793d 2231 3936 2e37 2220  27.6" y="196.7" 
-000029c0: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-000029d0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000029e0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000029f0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00002a00: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
-00002a10: 3d22 3022 2079 3d22 3232 312e 3122 2077  ="0" y="221.1" w
-00002a20: 6964 7468 3d22 3139 3237 2e36 2220 6865  idth="1927.6" he
-00002a30: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00002a40: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00002a50: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00002a60: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-00002a70: 783d 2231 3932 372e 3622 2079 3d22 3232  x="1927.6" y="22
-00002a80: 312e 3122 2077 6964 7468 3d22 3234 2e34  1.1" width="24.4
-00002a90: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00002aa0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00002ab0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00002ac0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00002ad0: 3064 2220 783d 2230 2220 793d 2232 3435  0d" x="0" y="245
-00002ae0: 2e35 2220 7769 6474 683d 2231 3932 372e  .5" width="1927.
-00002af0: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
-00002b00: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00002b10: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00002b20: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00002b30: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
-00002b40: 793d 2232 3435 2e35 2220 7769 6474 683d  y="245.5" width=
-00002b50: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
-00002b60: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00002b70: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00002b80: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00002b90: 2330 6430 6430 6422 2078 3d22 3022 2079  #0d0d0d" x="0" y
-00002ba0: 3d22 3236 392e 3922 2077 6964 7468 3d22  ="269.9" width="
-00002bb0: 3139 3237 2e36 2220 6865 6967 6874 3d22  1927.6" height="
-00002bc0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00002bd0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00002be0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00002bf0: 2223 3134 3139 3166 2220 783d 2231 3932  "#14191f" x="192
-00002c00: 372e 3622 2079 3d22 3236 392e 3922 2077  7.6" y="269.9" w
-00002c10: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
-00002c20: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00002c30: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00002c40: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00002c50: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
-00002c60: 2230 2220 793d 2232 3934 2e33 2220 7769  "0" y="294.3" wi
-00002c70: 6474 683d 2231 3932 372e 3622 2068 6569  dth="1927.6" hei
-00002c80: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00002c90: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00002ca0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00002cb0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00002cc0: 3d22 3139 3237 2e36 2220 793d 2232 3934  ="1927.6" y="294
-00002cd0: 2e33 2220 7769 6474 683d 2232 342e 3422  .3" width="24.4"
-00002ce0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00002cf0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00002d00: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00002d10: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00002d20: 6422 2078 3d22 3022 2079 3d22 3331 382e  d" x="0" y="318.
-00002d30: 3722 2077 6964 7468 3d22 3139 3237 2e36  7" width="1927.6
-00002d40: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00002d50: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00002d60: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00002d70: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-00002d80: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
-00002d90: 3d22 3331 382e 3722 2077 6964 7468 3d22  ="318.7" width="
-00002da0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-00002db0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00002dc0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00002dd0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00002de0: 3064 3064 3064 2220 783d 2230 2220 793d  0d0d0d" x="0" y=
-00002df0: 2233 3433 2e31 2220 7769 6474 683d 2231  "343.1" width="1
-00002e00: 3932 372e 3622 2068 6569 6768 743d 2232  927.6" height="2
-00002e10: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00002e20: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00002e30: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00002e40: 2331 3431 3931 6622 2078 3d22 3139 3237  #14191f" x="1927
-00002e50: 2e36 2220 793d 2233 3433 2e31 2220 7769  .6" y="343.1" wi
-00002e60: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
-00002e70: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00002e80: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00002e90: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00002ea0: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-00002eb0: 3022 2079 3d22 3336 372e 3522 2077 6964  0" y="367.5" wid
-00002ec0: 7468 3d22 3139 3237 2e36 2220 6865 6967  th="1927.6" heig
-00002ed0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00002ee0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00002ef0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00002f00: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-00002f10: 2231 3932 372e 3622 2079 3d22 3336 372e  "1927.6" y="367.
-00002f20: 3522 2077 6964 7468 3d22 3234 2e34 2220  5" width="24.4" 
-00002f30: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00002f40: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00002f50: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00002f60: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
-00002f70: 2220 783d 2230 2220 793d 2233 3931 2e39  " x="0" y="391.9
-00002f80: 2220 7769 6474 683d 2231 3932 372e 3622  " width="1927.6"
-00002f90: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00002fa0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00002fb0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00002fc0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00002fd0: 6622 2078 3d22 3139 3237 2e36 2220 793d  f" x="1927.6" y=
-00002fe0: 2233 3931 2e39 2220 7769 6474 683d 2232  "391.9" width="2
-00002ff0: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
-00003000: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00003010: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00003020: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00003030: 6430 6430 6422 2078 3d22 3022 2079 3d22  d0d0d" x="0" y="
-00003040: 3431 362e 3322 2077 6964 7468 3d22 3139  416.3" width="19
-00003050: 3237 2e36 2220 6865 6967 6874 3d22 3234  27.6" height="24
-00003060: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00003070: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00003080: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00003090: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
-000030a0: 3622 2079 3d22 3431 362e 3322 2077 6964  6" y="416.3" wid
-000030b0: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
-000030c0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000030d0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000030e0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000030f0: 6c3d 2223 3064 3064 3064 2220 783d 2230  l="#0d0d0d" x="0
-00003100: 2220 793d 2234 3430 2e37 2220 7769 6474  " y="440.7" widt
-00003110: 683d 2231 3932 372e 3622 2068 6569 6768  h="1927.6" heigh
-00003120: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00003130: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00003140: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00003150: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00003160: 3139 3237 2e36 2220 793d 2234 3430 2e37  1927.6" y="440.7
-00003170: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
-00003180: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003190: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000031a0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000031b0: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-000031c0: 2078 3d22 3022 2079 3d22 3436 352e 3122   x="0" y="465.1"
-000031d0: 2077 6964 7468 3d22 3139 3237 2e36 2220   width="1927.6" 
-000031e0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-000031f0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00003200: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00003210: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-00003220: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00003230: 3436 352e 3122 2077 6964 7468 3d22 3234  465.1" width="24
-00003240: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00003250: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00003260: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00003270: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00003280: 3064 3064 2220 783d 2230 2220 793d 2234  0d0d" x="0" y="4
-00003290: 3839 2e35 2220 7769 6474 683d 2231 3932  89.5" width="192
-000032a0: 372e 3622 2068 6569 6768 743d 2232 342e  7.6" height="24.
-000032b0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000032c0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000032d0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-000032e0: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
-000032f0: 2220 793d 2234 3839 2e35 2220 7769 6474  " y="489.5" widt
-00003300: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
-00003310: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00003320: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00003330: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00003340: 3d22 2330 6430 6430 6422 2078 3d22 3022  ="#0d0d0d" x="0"
-00003350: 2079 3d22 3531 332e 3922 2077 6964 7468   y="513.9" width
-00003360: 3d22 3139 3237 2e36 2220 6865 6967 6874  ="1927.6" height
-00003370: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00003380: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00003390: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000033a0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-000033b0: 3932 372e 3622 2079 3d22 3531 332e 3922  927.6" y="513.9"
-000033c0: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-000033d0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-000033e0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-000033f0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00003400: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
-00003410: 783d 2230 2220 793d 2235 3338 2e33 2220  x="0" y="538.3" 
-00003420: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
-00003430: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003440: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00003450: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00003460: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00003470: 2078 3d22 3139 3237 2e36 2220 793d 2235   x="1927.6" y="5
-00003480: 3338 2e33 2220 7769 6474 683d 2232 342e  38.3" width="24.
-00003490: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-000034a0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-000034b0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000034c0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-000034d0: 6430 6422 2078 3d22 3022 2079 3d22 3536  d0d" x="0" y="56
-000034e0: 322e 3722 2077 6964 7468 3d22 3139 3237  2.7" width="1927
-000034f0: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
-00003500: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00003510: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00003520: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-00003530: 3139 3166 2220 783d 2231 3932 372e 3622  191f" x="1927.6"
-00003540: 2079 3d22 3536 322e 3722 2077 6964 7468   y="562.7" width
-00003550: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
-00003560: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00003570: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00003580: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00003590: 2223 3064 3064 3064 2220 783d 2230 2220  "#0d0d0d" x="0" 
-000035a0: 793d 2235 3837 2e31 2220 7769 6474 683d  y="587.1" width=
-000035b0: 2231 3932 372e 3622 2068 6569 6768 743d  "1927.6" height=
-000035c0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000035d0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000035e0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000035f0: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
-00003600: 3237 2e36 2220 793d 2235 3837 2e31 2220  27.6" y="587.1" 
-00003610: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-00003620: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00003630: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00003640: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00003650: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-00003660: 3d22 3022 2079 3d22 3631 312e 3522 2077  ="0" y="611.5" w
-00003670: 6964 7468 3d22 3139 3237 2e36 2220 6865  idth="1927.6" he
-00003680: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00003690: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-000036a0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-000036b0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-000036c0: 783d 2231 3932 372e 3622 2079 3d22 3631  x="1927.6" y="61
-000036d0: 312e 3522 2077 6964 7468 3d22 3234 2e34  1.5" width="24.4
-000036e0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000036f0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00003700: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00003710: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00003720: 3064 2220 783d 2230 2220 793d 2236 3335  0d" x="0" y="635
-00003730: 2e39 2220 7769 6474 683d 2231 3932 372e  .9" width="1927.
-00003740: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
-00003750: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00003760: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00003770: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00003780: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
-00003790: 793d 2236 3335 2e39 2220 7769 6474 683d  y="635.9" width=
-000037a0: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
-000037b0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000037c0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000037d0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000037e0: 2330 6430 6430 6422 2078 3d22 3022 2079  #0d0d0d" x="0" y
-000037f0: 3d22 3636 302e 3322 2077 6964 7468 3d22  ="660.3" width="
-00003800: 3139 3237 2e36 2220 6865 6967 6874 3d22  1927.6" height="
-00003810: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00003820: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00003830: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00003840: 2223 3134 3139 3166 2220 783d 2231 3932  "#14191f" x="192
-00003850: 372e 3622 2079 3d22 3636 302e 3322 2077  7.6" y="660.3" w
-00003860: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
-00003870: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00003880: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00003890: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-000038a0: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
-000038b0: 2230 2220 793d 2236 3834 2e37 2220 7769  "0" y="684.7" wi
-000038c0: 6474 683d 2231 3932 372e 3622 2068 6569  dth="1927.6" hei
-000038d0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000038e0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000038f0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00003900: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00003910: 3d22 3139 3237 2e36 2220 793d 2236 3834  ="1927.6" y="684
-00003920: 2e37 2220 7769 6474 683d 2232 342e 3422  .7" width="24.4"
-00003930: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00003940: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00003950: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00003960: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
-00003970: 6422 2078 3d22 3022 2079 3d22 3730 392e  d" x="0" y="709.
-00003980: 3122 2077 6964 7468 3d22 3139 3237 2e36  1" width="1927.6
-00003990: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000039a0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000039b0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000039c0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-000039d0: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
-000039e0: 3d22 3730 392e 3122 2077 6964 7468 3d22  ="709.1" width="
-000039f0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
-00003a00: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00003a10: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00003a20: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00003a30: 3064 3064 3064 2220 783d 2230 2220 793d  0d0d0d" x="0" y=
-00003a40: 2237 3333 2e35 2220 7769 6474 683d 2231  "733.5" width="1
-00003a50: 3932 372e 3622 2068 6569 6768 743d 2232  927.6" height="2
-00003a60: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00003a70: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00003a80: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00003a90: 2331 3431 3931 6622 2078 3d22 3139 3237  #14191f" x="1927
-00003aa0: 2e36 2220 793d 2237 3333 2e35 2220 7769  .6" y="733.5" wi
-00003ab0: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
-00003ac0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00003ad0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00003ae0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00003af0: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-00003b00: 3022 2079 3d22 3735 372e 3922 2077 6964  0" y="757.9" wid
-00003b10: 7468 3d22 3139 3237 2e36 2220 6865 6967  th="1927.6" heig
-00003b20: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00003b30: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00003b40: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00003b50: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-00003b60: 2231 3932 372e 3622 2079 3d22 3735 372e  "1927.6" y="757.
-00003b70: 3922 2077 6964 7468 3d22 3234 2e34 2220  9" width="24.4" 
-00003b80: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00003b90: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00003ba0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00003bb0: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
-00003bc0: 2220 783d 2230 2220 793d 2237 3832 2e33  " x="0" y="782.3
-00003bd0: 2220 7769 6474 683d 2231 3932 372e 3622  " width="1927.6"
-00003be0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00003bf0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00003c00: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00003c10: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00003c20: 6622 2078 3d22 3139 3237 2e36 2220 793d  f" x="1927.6" y=
-00003c30: 2237 3832 2e33 2220 7769 6474 683d 2232  "782.3" width="2
-00003c40: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
-00003c50: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00003c60: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00003c70: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00003c80: 6430 6430 6422 2078 3d22 3022 2079 3d22  d0d0d" x="0" y="
-00003c90: 3830 362e 3722 2077 6964 7468 3d22 3139  806.7" width="19
-00003ca0: 3237 2e36 2220 6865 6967 6874 3d22 3234  27.6" height="24
-00003cb0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00003cc0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00003cd0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00003ce0: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
-00003cf0: 3622 2079 3d22 3830 362e 3722 2077 6964  6" y="806.7" wid
-00003d00: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
-00003d10: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00003d20: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00003d30: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00003d40: 6c3d 2223 3064 3064 3064 2220 783d 2230  l="#0d0d0d" x="0
-00003d50: 2220 793d 2238 3331 2e31 2220 7769 6474  " y="831.1" widt
-00003d60: 683d 2231 3932 372e 3622 2068 6569 6768  h="1927.6" heigh
-00003d70: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00003d80: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00003d90: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00003da0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00003db0: 3139 3237 2e36 2220 793d 2238 3331 2e31  1927.6" y="831.1
-00003dc0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
-00003dd0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00003de0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00003df0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00003e00: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
-00003e10: 2078 3d22 3022 2079 3d22 3835 352e 3522   x="0" y="855.5"
-00003e20: 2077 6964 7468 3d22 3139 3237 2e36 2220   width="1927.6" 
-00003e30: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00003e40: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00003e50: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00003e60: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-00003e70: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
-00003e80: 3835 352e 3522 2077 6964 7468 3d22 3234  855.5" width="24
-00003e90: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00003ea0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00003eb0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00003ec0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00003ed0: 3064 3064 2220 783d 2230 2220 793d 2238  0d0d" x="0" y="8
-00003ee0: 3739 2e39 2220 7769 6474 683d 2231 3932  79.9" width="192
-00003ef0: 372e 3622 2068 6569 6768 743d 2232 342e  7.6" height="24.
-00003f00: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00003f10: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00003f20: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00003f30: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
-00003f40: 2220 793d 2238 3739 2e39 2220 7769 6474  " y="879.9" widt
-00003f50: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
-00003f60: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00003f70: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00003f80: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00003f90: 3d22 2330 6430 6430 6422 2078 3d22 3022  ="#0d0d0d" x="0"
-00003fa0: 2079 3d22 3930 342e 3322 2077 6964 7468   y="904.3" width
-00003fb0: 3d22 3139 3237 2e36 2220 6865 6967 6874  ="1927.6" height
-00003fc0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00003fd0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00003fe0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00003ff0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00004000: 3932 372e 3622 2079 3d22 3930 342e 3322  927.6" y="904.3"
-00004010: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
-00004020: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00004030: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00004040: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00004050: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
-00004060: 783d 2230 2220 793d 2239 3238 2e37 2220  x="0" y="928.7" 
-00004070: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
-00004080: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00004090: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000040a0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000040b0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-000040c0: 2078 3d22 3139 3237 2e36 2220 793d 2239   x="1927.6" y="9
-000040d0: 3238 2e37 2220 7769 6474 683d 2232 342e  28.7" width="24.
-000040e0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
-000040f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00004100: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00004110: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
-00004120: 6430 6422 2078 3d22 3022 2079 3d22 3935  d0d" x="0" y="95
-00004130: 332e 3122 2077 6964 7468 3d22 3139 3237  3.1" width="1927
-00004140: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
-00004150: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00004160: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00004170: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-00004180: 3139 3166 2220 783d 2231 3932 372e 3622  191f" x="1927.6"
-00004190: 2079 3d22 3935 332e 3122 2077 6964 7468   y="953.1" width
-000041a0: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
-000041b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000041c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000041d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-000041e0: 2223 3064 3064 3064 2220 783d 2230 2220  "#0d0d0d" x="0" 
-000041f0: 793d 2239 3737 2e35 2220 7769 6474 683d  y="977.5" width=
-00004200: 2231 3932 372e 3622 2068 6569 6768 743d  "1927.6" height=
-00004210: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004220: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004230: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004240: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
-00004250: 3237 2e36 2220 793d 2239 3737 2e35 2220  27.6" y="977.5" 
-00004260: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
-00004270: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00004280: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00004290: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000042a0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
-000042b0: 3d22 3022 2079 3d22 3130 3031 2e39 2220  ="0" y="1001.9" 
-000042c0: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
-000042d0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000042e0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000042f0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00004300: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00004310: 2078 3d22 3139 3237 2e36 2220 793d 2231   x="1927.6" y="1
-00004320: 3030 312e 3922 2077 6964 7468 3d22 3234  001.9" width="24
-00004330: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
-00004340: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00004350: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00004360: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
-00004370: 3064 3064 2220 783d 2230 2220 793d 2231  0d0d" x="0" y="1
-00004380: 3032 362e 3322 2077 6964 7468 3d22 3139  026.3" width="19
-00004390: 3237 2e36 2220 6865 6967 6874 3d22 3234  27.6" height="24
-000043a0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-000043b0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-000043c0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-000043d0: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
-000043e0: 3622 2079 3d22 3130 3236 2e33 2220 7769  6" y="1026.3" wi
-000043f0: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
-00004400: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00004410: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00004420: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00004430: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
-00004440: 3022 2079 3d22 3130 3530 2e37 2220 7769  0" y="1050.7" wi
-00004450: 6474 683d 2231 3932 372e 3622 2068 6569  dth="1927.6" hei
-00004460: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00004470: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00004480: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00004490: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-000044a0: 3d22 3139 3237 2e36 2220 793d 2231 3035  ="1927.6" y="105
-000044b0: 302e 3722 2077 6964 7468 3d22 3234 2e34  0.7" width="24.4
-000044c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-000044d0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000044e0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000044f0: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
-00004500: 3064 2220 783d 2230 2220 793d 2231 3037  0d" x="0" y="107
-00004510: 352e 3122 2077 6964 7468 3d22 3139 3237  5.1" width="1927
-00004520: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
-00004530: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00004540: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00004550: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-00004560: 3139 3166 2220 783d 2231 3932 372e 3622  191f" x="1927.6"
-00004570: 2079 3d22 3130 3735 2e31 2220 7769 6474   y="1075.1" widt
-00004580: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
-00004590: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000045a0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000045b0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000045c0: 3d22 2332 3335 3638 6222 2078 3d22 3022  ="#23568b" x="0"
-000045d0: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-000045e0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-000045f0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004600: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004610: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004620: 3d22 2332 3335 3638 6222 2078 3d22 3132  ="#23568b" x="12
-00004630: 2e32 2220 793d 2231 3039 392e 3522 2077  .2" y="1099.5" w
-00004640: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-00004650: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00004660: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00004670: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00004680: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
-00004690: 2232 342e 3422 2079 3d22 3130 3939 2e35  "24.4" y="1099.5
-000046a0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-000046b0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000046c0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000046d0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000046e0: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-000046f0: 2078 3d22 3336 2e36 2220 793d 2231 3039   x="36.6" y="109
-00004700: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
-00004710: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00004720: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00004730: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00004740: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
-00004750: 3862 2220 783d 2234 382e 3822 2079 3d22  8b" x="48.8" y="
-00004760: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00004770: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00004780: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00004790: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000047a0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-000047b0: 3335 3638 6222 2078 3d22 3631 2220 793d  3568b" x="61" y=
-000047c0: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
-000047d0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-000047e0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-000047f0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00004800: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00004810: 3233 3536 3862 2220 783d 2237 332e 3222  23568b" x="73.2"
-00004820: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00004830: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00004840: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004850: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004860: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004870: 3d22 2332 3335 3638 6222 2078 3d22 3835  ="#23568b" x="85
-00004880: 2e34 2220 793d 2231 3039 392e 3522 2077  .4" y="1099.5" w
-00004890: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-000048a0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-000048b0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-000048c0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-000048d0: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
-000048e0: 2239 372e 3622 2079 3d22 3130 3939 2e35  "97.6" y="1099.5
-000048f0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00004900: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00004910: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00004920: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00004930: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-00004940: 2078 3d22 3130 392e 3822 2079 3d22 3130   x="109.8" y="10
-00004950: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00004960: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00004970: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00004980: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00004990: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-000049a0: 3638 6222 2078 3d22 3132 3222 2079 3d22  68b" x="122" y="
-000049b0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-000049c0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-000049d0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000049e0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000049f0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00004a00: 3335 3638 6222 2078 3d22 3133 342e 3222  3568b" x="134.2"
-00004a10: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00004a20: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00004a30: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004a40: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004a50: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004a60: 3d22 2332 3335 3638 6222 2078 3d22 3134  ="#23568b" x="14
-00004a70: 362e 3422 2079 3d22 3130 3939 2e35 2220  6.4" y="1099.5" 
-00004a80: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00004a90: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00004aa0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00004ab0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00004ac0: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00004ad0: 3d22 3135 382e 3622 2079 3d22 3130 3939  ="158.6" y="1099
-00004ae0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00004af0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00004b00: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00004b10: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00004b20: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-00004b30: 6222 2078 3d22 3137 302e 3822 2079 3d22  b" x="170.8" y="
-00004b40: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00004b50: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00004b60: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00004b70: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00004b80: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00004b90: 3335 3638 6222 2078 3d22 3138 3322 2079  3568b" x="183" y
-00004ba0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00004bb0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00004bc0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00004bd0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00004be0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00004bf0: 2332 3335 3638 6222 2078 3d22 3139 352e  #23568b" x="195.
-00004c00: 3222 2079 3d22 3130 3939 2e35 2220 7769  2" y="1099.5" wi
-00004c10: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00004c20: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00004c30: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00004c40: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00004c50: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-00004c60: 3230 372e 3422 2079 3d22 3130 3939 2e35  207.4" y="1099.5
-00004c70: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00004c80: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00004c90: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00004ca0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00004cb0: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-00004cc0: 2078 3d22 3231 392e 3622 2079 3d22 3130   x="219.6" y="10
-00004cd0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00004ce0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00004cf0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00004d00: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00004d10: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-00004d20: 3638 6222 2078 3d22 3233 312e 3822 2079  68b" x="231.8" y
-00004d30: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00004d40: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00004d50: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00004d60: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00004d70: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00004d80: 2332 3335 3638 6222 2078 3d22 3234 3422  #23568b" x="244"
-00004d90: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00004da0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00004db0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004dc0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004dd0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004de0: 3d22 2332 3335 3638 6222 2078 3d22 3235  ="#23568b" x="25
-00004df0: 362e 3222 2079 3d22 3130 3939 2e35 2220  6.2" y="1099.5" 
-00004e00: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00004e10: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00004e20: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00004e30: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00004e40: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00004e50: 3d22 3236 382e 3422 2079 3d22 3130 3939  ="268.4" y="1099
-00004e60: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00004e70: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00004e80: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00004e90: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00004ea0: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-00004eb0: 6222 2078 3d22 3238 302e 3622 2079 3d22  b" x="280.6" y="
-00004ec0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00004ed0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00004ee0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00004ef0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00004f00: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00004f10: 3335 3638 6222 2078 3d22 3239 322e 3822  3568b" x="292.8"
-00004f20: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00004f30: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00004f40: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00004f50: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00004f60: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00004f70: 3d22 2332 3335 3638 6222 2078 3d22 3330  ="#23568b" x="30
-00004f80: 3522 2079 3d22 3130 3939 2e35 2220 7769  5" y="1099.5" wi
-00004f90: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00004fa0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00004fb0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00004fc0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00004fd0: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-00004fe0: 3331 372e 3222 2079 3d22 3130 3939 2e35  317.2" y="1099.5
-00004ff0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00005000: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00005010: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00005020: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00005030: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-00005040: 2078 3d22 3332 392e 3422 2079 3d22 3130   x="329.4" y="10
-00005050: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00005060: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00005070: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00005080: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00005090: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-000050a0: 3638 6222 2078 3d22 3334 312e 3622 2079  68b" x="341.6" y
-000050b0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-000050c0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-000050d0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000050e0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000050f0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00005100: 2332 3335 3638 6222 2078 3d22 3335 332e  #23568b" x="353.
-00005110: 3822 2079 3d22 3130 3939 2e35 2220 7769  8" y="1099.5" wi
-00005120: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00005130: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00005140: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00005150: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00005160: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-00005170: 3336 3622 2079 3d22 3130 3939 2e35 2220  366" y="1099.5" 
-00005180: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00005190: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000051a0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000051b0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000051c0: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-000051d0: 3d22 3337 382e 3222 2079 3d22 3130 3939  ="378.2" y="1099
-000051e0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-000051f0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00005200: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00005210: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00005220: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-00005230: 6222 2078 3d22 3339 302e 3422 2079 3d22  b" x="390.4" y="
-00005240: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00005250: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00005260: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00005270: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00005280: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00005290: 3335 3638 6222 2078 3d22 3430 322e 3622  3568b" x="402.6"
-000052a0: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-000052b0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-000052c0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000052d0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000052e0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000052f0: 3d22 2332 3335 3638 6222 2078 3d22 3431  ="#23568b" x="41
-00005300: 342e 3822 2079 3d22 3130 3939 2e35 2220  4.8" y="1099.5" 
-00005310: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00005320: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005330: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005340: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005350: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00005360: 3d22 3432 3722 2079 3d22 3130 3939 2e35  ="427" y="1099.5
-00005370: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00005380: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00005390: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000053a0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000053b0: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-000053c0: 2078 3d22 3433 392e 3222 2079 3d22 3130   x="439.2" y="10
-000053d0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-000053e0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-000053f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00005400: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00005410: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-00005420: 3638 6222 2078 3d22 3435 312e 3422 2079  68b" x="451.4" y
-00005430: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00005440: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00005450: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00005460: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00005470: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00005480: 2332 3335 3638 6222 2078 3d22 3436 332e  #23568b" x="463.
-00005490: 3622 2079 3d22 3130 3939 2e35 2220 7769  6" y="1099.5" wi
-000054a0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-000054b0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-000054c0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000054d0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000054e0: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-000054f0: 3437 352e 3822 2079 3d22 3130 3939 2e35  475.8" y="1099.5
-00005500: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00005510: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00005520: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00005530: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00005540: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-00005550: 2078 3d22 3438 3822 2079 3d22 3130 3939   x="488" y="1099
-00005560: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00005570: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00005580: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00005590: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000055a0: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-000055b0: 6222 2078 3d22 3530 302e 3222 2079 3d22  b" x="500.2" y="
-000055c0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-000055d0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-000055e0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000055f0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00005600: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00005610: 3335 3638 6222 2078 3d22 3531 322e 3422  3568b" x="512.4"
-00005620: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00005630: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00005640: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005650: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005660: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005670: 3d22 2332 3335 3638 6222 2078 3d22 3532  ="#23568b" x="52
-00005680: 342e 3622 2079 3d22 3130 3939 2e35 2220  4.6" y="1099.5" 
-00005690: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-000056a0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000056b0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000056c0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000056d0: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-000056e0: 3d22 3533 362e 3822 2079 3d22 3130 3939  ="536.8" y="1099
-000056f0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00005700: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00005710: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00005720: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00005730: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
-00005740: 6222 2078 3d22 3534 3922 2079 3d22 3130  b" x="549" y="10
-00005750: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00005760: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00005770: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00005780: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00005790: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-000057a0: 3638 6222 2078 3d22 3536 312e 3222 2079  68b" x="561.2" y
-000057b0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-000057c0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-000057d0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000057e0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000057f0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00005800: 2332 3335 3638 6222 2078 3d22 3537 332e  #23568b" x="573.
-00005810: 3422 2079 3d22 3130 3939 2e35 2220 7769  4" y="1099.5" wi
-00005820: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00005830: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00005840: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00005850: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00005860: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
-00005870: 3538 352e 3622 2079 3d22 3130 3939 2e35  585.6" y="1099.5
-00005880: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00005890: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000058a0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000058b0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000058c0: 7420 6669 6c6c 3d22 2332 3335 3638 6222  t fill="#23568b"
-000058d0: 2078 3d22 3539 372e 3822 2079 3d22 3130   x="597.8" y="10
-000058e0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-000058f0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00005900: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00005910: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00005920: 3c72 6563 7420 6669 6c6c 3d22 2332 3335  <rect fill="#235
-00005930: 3638 6222 2078 3d22 3631 3022 2079 3d22  68b" x="610" y="
-00005940: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00005950: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00005960: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00005970: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00005980: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
-00005990: 3335 3638 6222 2078 3d22 3632 322e 3222  3568b" x="622.2"
-000059a0: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-000059b0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-000059c0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-000059d0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000059e0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000059f0: 3d22 2332 3335 3638 6222 2078 3d22 3633  ="#23568b" x="63
-00005a00: 342e 3422 2079 3d22 3130 3939 2e35 2220  4.4" y="1099.5" 
-00005a10: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00005a20: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005a30: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005a40: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005a50: 6669 6c6c 3d22 2332 3335 3638 6222 2078  fill="#23568b" x
-00005a60: 3d22 3634 362e 3622 2079 3d22 3130 3939  ="646.6" y="1099
-00005a70: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00005a80: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00005a90: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00005aa0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00005ab0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00005ac0: 6622 2078 3d22 3635 382e 3822 2079 3d22  f" x="658.8" y="
-00005ad0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00005ae0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00005af0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00005b00: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00005b10: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00005b20: 3431 3931 6622 2078 3d22 3637 3122 2079  4191f" x="671" y
-00005b30: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00005b40: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00005b50: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00005b60: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00005b70: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00005b80: 2331 3431 3931 6622 2078 3d22 3638 332e  #14191f" x="683.
-00005b90: 3222 2079 3d22 3130 3939 2e35 2220 7769  2" y="1099.5" wi
-00005ba0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00005bb0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00005bc0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00005bd0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00005be0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00005bf0: 3639 352e 3422 2079 3d22 3130 3939 2e35  695.4" y="1099.5
-00005c00: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00005c10: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00005c20: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00005c30: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00005c40: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00005c50: 2078 3d22 3730 372e 3622 2079 3d22 3130   x="707.6" y="10
-00005c60: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00005c70: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00005c80: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00005c90: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00005ca0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00005cb0: 3931 6622 2078 3d22 3731 392e 3822 2079  91f" x="719.8" y
-00005cc0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00005cd0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00005ce0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00005cf0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00005d00: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00005d10: 2331 3431 3931 6622 2078 3d22 3733 3222  #14191f" x="732"
-00005d20: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00005d30: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00005d40: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005d50: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005d60: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005d70: 3d22 2331 3431 3931 6622 2078 3d22 3734  ="#14191f" x="74
-00005d80: 342e 3222 2079 3d22 3130 3939 2e35 2220  4.2" y="1099.5" 
-00005d90: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00005da0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00005db0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00005dc0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00005dd0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00005de0: 3d22 3735 362e 3422 2079 3d22 3130 3939  ="756.4" y="1099
-00005df0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00005e00: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00005e10: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00005e20: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00005e30: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00005e40: 6622 2078 3d22 3736 382e 3622 2079 3d22  f" x="768.6" y="
-00005e50: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00005e60: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00005e70: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00005e80: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00005e90: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00005ea0: 3431 3931 6622 2078 3d22 3738 302e 3822  4191f" x="780.8"
-00005eb0: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00005ec0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00005ed0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00005ee0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00005ef0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00005f00: 3d22 2331 3431 3931 6622 2078 3d22 3739  ="#14191f" x="79
-00005f10: 3322 2079 3d22 3130 3939 2e35 2220 7769  3" y="1099.5" wi
-00005f20: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00005f30: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00005f40: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00005f50: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00005f60: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00005f70: 3830 352e 3222 2079 3d22 3130 3939 2e35  805.2" y="1099.5
-00005f80: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00005f90: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00005fa0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00005fb0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00005fc0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00005fd0: 2078 3d22 3831 372e 3422 2079 3d22 3130   x="817.4" y="10
-00005fe0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00005ff0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00006000: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006010: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006020: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00006030: 3931 6622 2078 3d22 3832 392e 3622 2079  91f" x="829.6" y
-00006040: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00006050: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00006060: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00006070: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00006080: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00006090: 2331 3431 3931 6622 2078 3d22 3834 312e  #14191f" x="841.
-000060a0: 3822 2079 3d22 3130 3939 2e35 2220 7769  8" y="1099.5" wi
-000060b0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-000060c0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-000060d0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000060e0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000060f0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00006100: 3835 3422 2079 3d22 3130 3939 2e35 2220  854" y="1099.5" 
-00006110: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00006120: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00006130: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00006140: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00006150: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00006160: 3d22 3836 362e 3222 2079 3d22 3130 3939  ="866.2" y="1099
-00006170: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00006180: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00006190: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000061a0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000061b0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-000061c0: 6622 2078 3d22 3837 382e 3422 2079 3d22  f" x="878.4" y="
-000061d0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-000061e0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-000061f0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00006200: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00006210: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00006220: 3431 3931 6622 2078 3d22 3839 302e 3622  4191f" x="890.6"
-00006230: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00006240: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00006250: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00006260: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00006270: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00006280: 3d22 2331 3431 3931 6622 2078 3d22 3930  ="#14191f" x="90
-00006290: 322e 3822 2079 3d22 3130 3939 2e35 2220  2.8" y="1099.5" 
-000062a0: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-000062b0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-000062c0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-000062d0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-000062e0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-000062f0: 3d22 3931 3522 2079 3d22 3130 3939 2e35  ="915" y="1099.5
-00006300: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00006310: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006320: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00006330: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00006340: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00006350: 2078 3d22 3932 372e 3222 2079 3d22 3130   x="927.2" y="10
-00006360: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00006370: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00006380: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006390: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-000063a0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-000063b0: 3931 6622 2078 3d22 3933 392e 3422 2079  91f" x="939.4" y
-000063c0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-000063d0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-000063e0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000063f0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00006400: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00006410: 2331 3431 3931 6622 2078 3d22 3935 312e  #14191f" x="951.
-00006420: 3622 2079 3d22 3130 3939 2e35 2220 7769  6" y="1099.5" wi
-00006430: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00006440: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00006450: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00006460: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00006470: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00006480: 3936 332e 3822 2079 3d22 3130 3939 2e35  963.8" y="1099.5
-00006490: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-000064a0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000064b0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000064c0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000064d0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-000064e0: 2078 3d22 3937 3622 2079 3d22 3130 3939   x="976" y="1099
-000064f0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00006500: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00006510: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00006520: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00006530: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00006540: 6622 2078 3d22 3938 382e 3222 2079 3d22  f" x="988.2" y="
-00006550: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00006560: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00006570: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00006580: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00006590: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-000065a0: 3431 3931 6622 2078 3d22 3130 3030 2e34  4191f" x="1000.4
-000065b0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
-000065c0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-000065d0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000065e0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000065f0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00006600: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00006610: 3031 322e 3622 2079 3d22 3130 3939 2e35  012.6" y="1099.5
-00006620: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00006630: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006640: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00006650: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00006660: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00006670: 2078 3d22 3130 3234 2e38 2220 793d 2231   x="1024.8" y="1
-00006680: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
-00006690: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-000066a0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000066b0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000066c0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-000066d0: 3139 3166 2220 783d 2231 3033 3722 2079  191f" x="1037" y
-000066e0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-000066f0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00006700: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00006710: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00006720: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00006730: 2331 3431 3931 6622 2078 3d22 3130 3439  #14191f" x="1049
-00006740: 2e32 2220 793d 2231 3039 392e 3522 2077  .2" y="1099.5" w
-00006750: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-00006760: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00006770: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00006780: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00006790: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-000067a0: 2231 3036 312e 3422 2079 3d22 3130 3939  "1061.4" y="1099
-000067b0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-000067c0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000067d0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000067e0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000067f0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00006800: 6622 2078 3d22 3130 3733 2e36 2220 793d  f" x="1073.6" y=
-00006810: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
-00006820: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-00006830: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00006840: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00006850: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00006860: 3134 3139 3166 2220 783d 2231 3038 352e  14191f" x="1085.
-00006870: 3822 2079 3d22 3130 3939 2e35 2220 7769  8" y="1099.5" wi
-00006880: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00006890: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-000068a0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000068b0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000068c0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-000068d0: 3130 3938 2220 793d 2231 3039 392e 3522  1098" y="1099.5"
-000068e0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
-000068f0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00006900: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00006910: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00006920: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-00006930: 783d 2231 3131 302e 3222 2079 3d22 3130  x="1110.2" y="10
-00006940: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00006950: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00006960: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006970: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006980: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00006990: 3931 6622 2078 3d22 3131 3232 2e34 2220  91f" x="1122.4" 
-000069a0: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
-000069b0: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
-000069c0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000069d0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000069e0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-000069f0: 2223 3134 3139 3166 2220 783d 2231 3133  "#14191f" x="113
-00006a00: 342e 3622 2079 3d22 3130 3939 2e35 2220  4.6" y="1099.5" 
-00006a10: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00006a20: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00006a30: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00006a40: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00006a50: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00006a60: 3d22 3131 3436 2e38 2220 793d 2231 3039  ="1146.8" y="109
-00006a70: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
-00006a80: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00006a90: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00006aa0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00006ab0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-00006ac0: 3166 2220 783d 2231 3135 3922 2079 3d22  1f" x="1159" y="
-00006ad0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00006ae0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00006af0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00006b00: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00006b10: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00006b20: 3431 3931 6622 2078 3d22 3131 3731 2e32  4191f" x="1171.2
-00006b30: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
-00006b40: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00006b50: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00006b60: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00006b70: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00006b80: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00006b90: 3138 332e 3422 2079 3d22 3130 3939 2e35  183.4" y="1099.5
-00006ba0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00006bb0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00006bc0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00006bd0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00006be0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00006bf0: 2078 3d22 3131 3935 2e36 2220 793d 2231   x="1195.6" y="1
-00006c00: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
-00006c10: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-00006c20: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00006c30: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00006c40: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-00006c50: 3139 3166 2220 783d 2231 3230 372e 3822  191f" x="1207.8"
-00006c60: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00006c70: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00006c80: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00006c90: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00006ca0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00006cb0: 3d22 2331 3431 3931 6622 2078 3d22 3132  ="#14191f" x="12
-00006cc0: 3230 2220 793d 2231 3039 392e 3522 2077  20" y="1099.5" w
-00006cd0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-00006ce0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00006cf0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00006d00: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00006d10: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-00006d20: 2231 3233 322e 3222 2079 3d22 3130 3939  "1232.2" y="1099
-00006d30: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00006d40: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00006d50: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00006d60: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00006d70: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00006d80: 6622 2078 3d22 3132 3434 2e34 2220 793d  f" x="1244.4" y=
-00006d90: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
-00006da0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-00006db0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00006dc0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00006dd0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00006de0: 3134 3139 3166 2220 783d 2231 3235 362e  14191f" x="1256.
-00006df0: 3622 2079 3d22 3130 3939 2e35 2220 7769  6" y="1099.5" wi
-00006e00: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00006e10: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00006e20: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00006e30: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00006e40: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00006e50: 3132 3638 2e38 2220 793d 2231 3039 392e  1268.8" y="1099.
-00006e60: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
-00006e70: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00006e80: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00006e90: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00006ea0: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-00006eb0: 2220 783d 2231 3238 3122 2079 3d22 3130  " x="1281" y="10
-00006ec0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00006ed0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00006ee0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00006ef0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00006f00: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00006f10: 3931 6622 2078 3d22 3132 3933 2e32 2220  91f" x="1293.2" 
-00006f20: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
-00006f30: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
-00006f40: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00006f50: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00006f60: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00006f70: 2223 3134 3139 3166 2220 783d 2231 3330  "#14191f" x="130
-00006f80: 352e 3422 2079 3d22 3130 3939 2e35 2220  5.4" y="1099.5" 
-00006f90: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00006fa0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00006fb0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00006fc0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00006fd0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00006fe0: 3d22 3133 3137 2e36 2220 793d 2231 3039  ="1317.6" y="109
-00006ff0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
-00007000: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00007010: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00007020: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00007030: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-00007040: 3166 2220 783d 2231 3332 392e 3822 2079  1f" x="1329.8" y
-00007050: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00007060: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00007070: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00007080: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00007090: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000070a0: 2331 3431 3931 6622 2078 3d22 3133 3432  #14191f" x="1342
-000070b0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
-000070c0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-000070d0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000070e0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000070f0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00007100: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00007110: 3335 342e 3222 2079 3d22 3130 3939 2e35  354.2" y="1099.5
-00007120: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00007130: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00007140: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00007150: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00007160: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00007170: 2078 3d22 3133 3636 2e34 2220 793d 2231   x="1366.4" y="1
-00007180: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
-00007190: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-000071a0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-000071b0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-000071c0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-000071d0: 3139 3166 2220 783d 2231 3337 382e 3622  191f" x="1378.6"
-000071e0: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-000071f0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00007200: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00007210: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00007220: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00007230: 3d22 2331 3431 3931 6622 2078 3d22 3133  ="#14191f" x="13
-00007240: 3930 2e38 2220 793d 2231 3039 392e 3522  90.8" y="1099.5"
-00007250: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
-00007260: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00007270: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00007280: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00007290: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-000072a0: 783d 2231 3430 3322 2079 3d22 3130 3939  x="1403" y="1099
-000072b0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-000072c0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000072d0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000072e0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000072f0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00007300: 6622 2078 3d22 3134 3135 2e32 2220 793d  f" x="1415.2" y=
-00007310: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
-00007320: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-00007330: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00007340: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00007350: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00007360: 3134 3139 3166 2220 783d 2231 3432 372e  14191f" x="1427.
-00007370: 3422 2079 3d22 3130 3939 2e35 2220 7769  4" y="1099.5" wi
-00007380: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00007390: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-000073a0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-000073b0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-000073c0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-000073d0: 3134 3339 2e36 2220 793d 2231 3039 392e  1439.6" y="1099.
-000073e0: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
-000073f0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00007400: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00007410: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00007420: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-00007430: 2220 783d 2231 3435 312e 3822 2079 3d22  " x="1451.8" y="
-00007440: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00007450: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00007460: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00007470: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00007480: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00007490: 3431 3931 6622 2078 3d22 3134 3634 2220  4191f" x="1464" 
-000074a0: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
-000074b0: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
-000074c0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000074d0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000074e0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-000074f0: 2223 3134 3139 3166 2220 783d 2231 3437  "#14191f" x="147
-00007500: 362e 3222 2079 3d22 3130 3939 2e35 2220  6.2" y="1099.5" 
-00007510: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00007520: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00007530: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00007540: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00007550: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00007560: 3d22 3134 3838 2e34 2220 793d 2231 3039  ="1488.4" y="109
-00007570: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
-00007580: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00007590: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000075a0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000075b0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-000075c0: 3166 2220 783d 2231 3530 302e 3622 2079  1f" x="1500.6" y
-000075d0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-000075e0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-000075f0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00007600: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00007610: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00007620: 2331 3431 3931 6622 2078 3d22 3135 3132  #14191f" x="1512
-00007630: 2e38 2220 793d 2231 3039 392e 3522 2077  .8" y="1099.5" w
-00007640: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-00007650: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00007660: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00007670: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00007680: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-00007690: 2231 3532 3522 2079 3d22 3130 3939 2e35  "1525" y="1099.5
-000076a0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-000076b0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-000076c0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000076d0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000076e0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-000076f0: 2078 3d22 3135 3337 2e32 2220 793d 2231   x="1537.2" y="1
-00007700: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
-00007710: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-00007720: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00007730: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00007740: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-00007750: 3139 3166 2220 783d 2231 3534 392e 3422  191f" x="1549.4"
-00007760: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00007770: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00007780: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00007790: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000077a0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000077b0: 3d22 2331 3431 3931 6622 2078 3d22 3135  ="#14191f" x="15
-000077c0: 3631 2e36 2220 793d 2231 3039 392e 3522  61.6" y="1099.5"
-000077d0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
-000077e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-000077f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00007800: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00007810: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-00007820: 783d 2231 3537 332e 3822 2079 3d22 3130  x="1573.8" y="10
-00007830: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00007840: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00007850: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007860: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007870: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00007880: 3931 6622 2078 3d22 3135 3836 2220 793d  91f" x="1586" y=
-00007890: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
-000078a0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-000078b0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-000078c0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-000078d0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-000078e0: 3134 3139 3166 2220 783d 2231 3539 382e  14191f" x="1598.
-000078f0: 3222 2079 3d22 3130 3939 2e35 2220 7769  2" y="1099.5" wi
-00007900: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00007910: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00007920: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00007930: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00007940: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00007950: 3136 3130 2e34 2220 793d 2231 3039 392e  1610.4" y="1099.
-00007960: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
-00007970: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00007980: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00007990: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-000079a0: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-000079b0: 2220 783d 2231 3632 322e 3622 2079 3d22  " x="1622.6" y="
-000079c0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-000079d0: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-000079e0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000079f0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00007a00: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00007a10: 3431 3931 6622 2078 3d22 3136 3334 2e38  4191f" x="1634.8
-00007a20: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
-00007a30: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00007a40: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00007a50: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00007a60: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00007a70: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00007a80: 3634 3722 2079 3d22 3130 3939 2e35 2220  647" y="1099.5" 
-00007a90: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
-00007aa0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
-00007ab0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
-00007ac0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
-00007ad0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
-00007ae0: 3d22 3136 3539 2e32 2220 793d 2231 3039  ="1659.2" y="109
-00007af0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
-00007b00: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00007b10: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-00007b20: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-00007b30: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-00007b40: 3166 2220 783d 2231 3637 312e 3422 2079  1f" x="1671.4" y
-00007b50: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-00007b60: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-00007b70: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00007b80: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00007b90: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00007ba0: 2331 3431 3931 6622 2078 3d22 3136 3833  #14191f" x="1683
-00007bb0: 2e36 2220 793d 2231 3039 392e 3522 2077  .6" y="1099.5" w
-00007bc0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-00007bd0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00007be0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00007bf0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00007c00: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-00007c10: 2231 3639 352e 3822 2079 3d22 3130 3939  "1695.8" y="1099
-00007c20: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-00007c30: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-00007c40: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-00007c50: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-00007c60: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-00007c70: 6622 2078 3d22 3137 3038 2220 793d 2231  f" x="1708" y="1
-00007c80: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
-00007c90: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
-00007ca0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
-00007cb0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
-00007cc0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
-00007cd0: 3139 3166 2220 783d 2231 3732 302e 3222  191f" x="1720.2"
-00007ce0: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00007cf0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00007d00: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00007d10: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00007d20: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-00007d30: 3d22 2331 3431 3931 6622 2078 3d22 3137  ="#14191f" x="17
-00007d40: 3332 2e34 2220 793d 2231 3039 392e 3522  32.4" y="1099.5"
-00007d50: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
-00007d60: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00007d70: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00007d80: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00007d90: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-00007da0: 783d 2231 3734 342e 3622 2079 3d22 3130  x="1744.6" y="10
-00007db0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00007dc0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00007dd0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00007de0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00007df0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00007e00: 3931 6622 2078 3d22 3137 3536 2e38 2220  91f" x="1756.8" 
-00007e10: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
-00007e20: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
-00007e30: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00007e40: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00007e50: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00007e60: 2223 3134 3139 3166 2220 783d 2231 3736  "#14191f" x="176
-00007e70: 3922 2079 3d22 3130 3939 2e35 2220 7769  9" y="1099.5" wi
-00007e80: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
-00007e90: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
-00007ea0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
-00007eb0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
-00007ec0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
-00007ed0: 3137 3831 2e32 2220 793d 2231 3039 392e  1781.2" y="1099.
-00007ee0: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
-00007ef0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-00007f00: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-00007f10: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00007f20: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
-00007f30: 2220 783d 2231 3739 332e 3422 2079 3d22  " x="1793.4" y="
-00007f40: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
-00007f50: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00007f60: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00007f70: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00007f80: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
-00007f90: 3431 3931 6622 2078 3d22 3138 3035 2e36  4191f" x="1805.6
-00007fa0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
-00007fb0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
-00007fc0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00007fd0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00007fe0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00007ff0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
-00008000: 3831 372e 3822 2079 3d22 3130 3939 2e35  817.8" y="1099.5
-00008010: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
-00008020: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00008030: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-00008040: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-00008050: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
-00008060: 2078 3d22 3138 3330 2220 793d 2231 3039   x="1830" y="109
-00008070: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
-00008080: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
-00008090: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
-000080a0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
-000080b0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
-000080c0: 3166 2220 783d 2231 3834 322e 3222 2079  1f" x="1842.2" y
-000080d0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
-000080e0: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
-000080f0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-00008100: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-00008110: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-00008120: 2331 3431 3931 6622 2078 3d22 3138 3534  #14191f" x="1854
-00008130: 2e34 2220 793d 2231 3039 392e 3522 2077  .4" y="1099.5" w
-00008140: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
-00008150: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00008160: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00008170: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00008180: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
-00008190: 2231 3836 362e 3622 2079 3d22 3130 3939  "1866.6" y="1099
-000081a0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
-000081b0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000081c0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000081d0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000081e0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
-000081f0: 6622 2078 3d22 3138 3738 2e38 2220 793d  f" x="1878.8" y=
-00008200: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
-00008210: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
-00008220: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
-00008230: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
-00008240: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
-00008250: 3134 3139 3166 2220 783d 2231 3839 3122  14191f" x="1891"
-00008260: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
-00008270: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
-00008280: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00008290: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-000082a0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
-000082b0: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
-000082c0: 3033 2e32 2220 793d 2231 3039 392e 3522  03.2" y="1099.5"
-000082d0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
-000082e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-000082f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00008300: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00008310: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
-00008320: 783d 2231 3931 352e 3422 2079 3d22 3130  x="1915.4" y="10
-00008330: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
-00008340: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00008350: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00008360: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00008370: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
-00008380: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
-00008390: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
-000083a0: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
-000083b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-000083c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-000083d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-000083e0: 2223 3030 3432 3935 2220 783d 2230 2220  "#004295" x="0" 
-000083f0: 793d 2231 3132 332e 3922 2077 6964 7468  y="1123.9" width
-00008400: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
-00008410: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00008420: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00008430: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00008440: 2223 3030 3432 3935 2220 783d 2231 322e  "#004295" x="12.
-00008450: 3222 2079 3d22 3131 3233 2e39 2220 7769  2" y="1123.9" wi
-00008460: 6474 683d 2235 3439 2220 6865 6967 6874  dth="549" height
-00008470: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00008480: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00008490: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000084a0: 6c3d 2223 3030 3432 3935 2220 783d 2235  l="#004295" x="5
-000084b0: 3631 2e32 2220 793d 2231 3132 332e 3922  61.2" y="1123.9"
-000084c0: 2077 6964 7468 3d22 3133 3738 2e36 2220   width="1378.6" 
-000084d0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
-000084e0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
-000084f0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
-00008500: 6374 2066 696c 6c3d 2223 3030 3432 3935  ct fill="#004295
-00008510: 2220 783d 2231 3933 392e 3822 2079 3d22  " x="1939.8" y="
-00008520: 3131 3233 2e39 2220 7769 6474 683d 2231  1123.9" width="1
-00008530: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
-00008540: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00008550: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00008560: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00008570: 3035 3361 6122 2078 3d22 3022 2079 3d22  053aa" x="0" y="
-00008580: 3131 3438 2e33 2220 7769 6474 683d 2233  1148.3" width="3
-00008590: 362e 3622 2068 6569 6768 743d 2232 342e  6.6" height="24.
-000085a0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-000085b0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-000085c0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-000085d0: 3137 3864 3422 2078 3d22 3336 2e36 2220  178d4" x="36.6" 
-000085e0: 793d 2231 3134 382e 3322 2077 6964 7468  y="1148.3" width
-000085f0: 3d22 3733 2e32 2220 6865 6967 6874 3d22  ="73.2" height="
-00008600: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
-00008610: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
-00008620: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
-00008630: 2223 3030 3533 6161 2220 783d 2231 3039  "#0053aa" x="109
-00008640: 2e38 2220 793d 2231 3134 382e 3322 2077  .8" y="1148.3" w
-00008650: 6964 7468 3d22 3336 2e36 2220 6865 6967  idth="36.6" heig
-00008660: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
-00008670: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
-00008680: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
-00008690: 696c 6c3d 2223 3031 3738 6434 2220 783d  ill="#0178d4" x=
-000086a0: 2231 3436 2e34 2220 793d 2231 3134 382e  "146.4" y="1148.
-000086b0: 3322 2077 6964 7468 3d22 3137 302e 3822  3" width="170.8"
-000086c0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
-000086d0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
-000086e0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
-000086f0: 6563 7420 6669 6c6c 3d22 2330 3035 3361  ect fill="#0053a
-00008700: 6122 2078 3d22 3331 372e 3222 2079 3d22  a" x="317.2" y="
-00008710: 3131 3438 2e33 2220 7769 6474 683d 2233  1148.3" width="3
-00008720: 362e 3622 2068 6569 6768 743d 2232 342e  6.6" height="24.
-00008730: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
-00008740: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
-00008750: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
-00008760: 3137 3864 3422 2078 3d22 3335 332e 3822  178d4" x="353.8"
-00008770: 2079 3d22 3131 3438 2e33 2220 7769 6474   y="1148.3" widt
-00008780: 683d 2231 3730 2e38 2220 6865 6967 6874  h="170.8" height
-00008790: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-000087a0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-000087b0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-000087c0: 6c3d 2223 3030 3533 6161 2220 783d 2235  l="#0053aa" x="5
-000087d0: 3234 2e36 2220 793d 2231 3134 382e 3322  24.6" y="1148.3"
-000087e0: 2077 6964 7468 3d22 3336 2e36 2220 6865   width="36.6" he
-000087f0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
-00008800: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
-00008810: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
-00008820: 2066 696c 6c3d 2223 3031 3738 6434 2220   fill="#0178d4" 
-00008830: 783d 2235 3631 2e32 2220 793d 2231 3134  x="561.2" y="114
-00008840: 382e 3322 2077 6964 7468 3d22 3235 362e  8.3" width="256.
-00008850: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
-00008860: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00008870: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00008880: 3c72 6563 7420 6669 6c6c 3d22 2330 3035  <rect fill="#005
-00008890: 3361 6122 2078 3d22 3831 372e 3422 2079  3aa" x="817.4" y
-000088a0: 3d22 3131 3438 2e33 2220 7769 6474 683d  ="1148.3" width=
-000088b0: 2233 362e 3622 2068 6569 6768 743d 2232  "36.6" height="2
-000088c0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
-000088d0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
-000088e0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
-000088f0: 2330 3137 3864 3422 2078 3d22 3835 3422  #0178d4" x="854"
-00008900: 2079 3d22 3131 3438 2e33 2220 7769 6474   y="1148.3" widt
-00008910: 683d 2232 3139 2e36 2220 6865 6967 6874  h="219.6" height
-00008920: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
-00008930: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
-00008940: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
-00008950: 6c3d 2223 3030 3533 6161 2220 783d 2231  l="#0053aa" x="1
-00008960: 3037 332e 3622 2079 3d22 3131 3438 2e33  073.6" y="1148.3
-00008970: 2220 7769 6474 683d 2233 362e 3622 2068  " width="36.6" h
-00008980: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
-00008990: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
-000089a0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
-000089b0: 7420 6669 6c6c 3d22 2330 3137 3864 3422  t fill="#0178d4"
-000089c0: 2078 3d22 3131 3130 2e32 2220 793d 2231   x="1110.2" y="1
-000089d0: 3134 382e 3322 2077 6964 7468 3d22 3138  148.3" width="18
-000089e0: 3322 2068 6569 6768 743d 2232 342e 3635  3" height="24.65
-000089f0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
-00008a00: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
-00008a10: 3c72 6563 7420 6669 6c6c 3d22 2330 3137  <rect fill="#017
-00008a20: 3864 3422 2078 3d22 3132 3933 2e32 2220  8d4" x="1293.2" 
-00008a30: 793d 2231 3134 382e 3322 2077 6964 7468  y="1148.3" width
-00008a40: 3d22 3635 382e 3822 2068 6569 6768 743d  ="658.8" height=
-00008a50: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
-00008a60: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
-00008a70: 6765 7322 2f3e 0a20 2020 203c 6720 636c  ges"/>.    <g cl
-00008a80: 6173 733d 2274 6572 6d69 6e61 6c2d 3136  ass="terminal-16
-00008a90: 3330 3637 3637 342d 6d61 7472 6978 223e  3067674-matrix">
-00008aa0: 0a20 2020 203c 7465 7874 2063 6c61 7373  .    <text class
-00008ab0: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00008ac0: 3736 3734 2d72 3222 2078 3d22 3132 2e32  7674-r2" x="12.2
-00008ad0: 2220 793d 2232 3022 2074 6578 744c 656e  " y="20" textLen
-00008ae0: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
-00008af0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-00008b00: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
-00008b10: 6e65 2d30 2922 3ee2 ad98 3c2f 7465 7874  ne-0)">...</text
-00008b20: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-00008b30: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-00008b40: 2d72 3222 2078 3d22 3632 322e 3222 2079  -r2" x="622.2" y
-00008b50: 3d22 3230 2220 7465 7874 4c65 6e67 7468  ="20" textLength
-00008b60: 3d22 3130 392e 3822 2063 6c69 702d 7061  ="109.8" clip-pa
-00008b70: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-00008b80: 6c2d 3136 3330 3637 3637 342d 6c69 6e65  l-163067674-line
-00008b90: 2d30 2922 3e62 726f 7773 7226 2331 3630  -0)">browsr&#160
-00008ba0: 3be2 8094 2623 3136 303b 3c2f 7465 7874  ;...&#160;</text
-00008bb0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-00008bc0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-00008bd0: 2d72 3322 2078 3d22 3733 3222 2079 3d22  -r3" x="732" y="
-00008be0: 3230 2220 7465 7874 4c65 6e67 7468 3d22  20" textLength="
-00008bf0: 3537 332e 3422 2063 6c69 702d 7061 7468  573.4" clip-path
-00008c00: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-00008c10: 3136 3330 3637 3637 342d 6c69 6e65 2d30  163067674-line-0
-00008c20: 2922 3e67 6974 6875 623a 2f2f 6a75 6674  )">github://juft
-00008c30: 696e 3a62 726f 7773 7240 7631 2e36 2e30  in:browsr@v1.6.0
-00008c40: 2f4c 4943 454e 5345 2623 3136 303b 5b6d  /LICENSE&#160;[m
-00008c50: 6f6e 6f6b 6169 5d3c 2f74 6578 743e 3c74  onokai]</text><t
-00008c60: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
-00008c70: 6e61 6c2d 3136 3330 3637 3637 342d 7231  nal-163067674-r1
-00008c80: 2220 783d 2231 3935 3222 2079 3d22 3230  " x="1952" y="20
-00008c90: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-00008ca0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-00008cb0: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-00008cc0: 3036 3736 3734 2d6c 696e 652d 3029 223e  067674-line-0)">
-00008cd0: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
-00008ce0: 6173 733d 2274 6572 6d69 6e61 6c2d 3136  ass="terminal-16
-00008cf0: 3330 3637 3637 342d 7234 2220 783d 2230  3067674-r4" x="0
-00008d00: 2220 793d 2234 342e 3422 2074 6578 744c  " y="44.4" textL
-00008d10: 656e 6774 683d 2231 3932 372e 3622 2063  ength="1927.6" c
-00008d20: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-00008d30: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-00008d40: 342d 6c69 6e65 2d31 2922 3e4d 4954 2623  4-line-1)">MIT&#
-00008d50: 3136 303b 4c69 6365 6e73 6526 2331 3630  160;License&#160
-00008d60: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008d70: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008d80: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008d90: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008da0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008db0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008dc0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008dd0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008de0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008df0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008e00: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008e10: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008e20: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008e30: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008e40: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008e50: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008e60: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008e70: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008e80: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008e90: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008ea0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008eb0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008ec0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008ed0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008ee0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008ef0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008f00: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008f10: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008f20: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008f30: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008f40: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008f50: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008f60: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008f70: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008f80: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008f90: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008fa0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008fb0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008fc0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00008fd0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00008fe0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00008ff0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009000: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009010: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009020: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009030: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009040: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009050: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009060: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009070: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009080: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009090: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-000090a0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-000090b0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-000090c0: 3b26 2331 3630 3b26 2331 3630 3b3c 2f74  ;&#160;&#160;</t
-000090d0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-000090e0: 2274 6572 6d69 6e61 6c2d 3136 3330 3637  "terminal-163067
-000090f0: 3637 342d 7231 2220 783d 2231 3935 3222  674-r1" x="1952"
-00009100: 2079 3d22 3434 2e34 2220 7465 7874 4c65   y="44.4" textLe
-00009110: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
-00009120: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-00009130: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
-00009140: 696e 652d 3129 223e 0a3c 2f74 6578 743e  ine-1)">.</text>
-00009150: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-00009160: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
-00009170: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-00009180: 3638 2e38 2220 7465 7874 4c65 6e67 7468  68.8" textLength
-00009190: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-000091a0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-000091b0: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
-000091c0: 3229 223e 0a3c 2f74 6578 743e 3c74 6578  2)">.</text><tex
-000091d0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-000091e0: 6c2d 3136 3330 3637 3637 342d 7234 2220  l-163067674-r4" 
-000091f0: 783d 2230 2220 793d 2239 332e 3222 2074  x="0" y="93.2" t
-00009200: 6578 744c 656e 6774 683d 2231 3932 372e  extLength="1927.
-00009210: 3622 2063 6c69 702d 7061 7468 3d22 7572  6" clip-path="ur
-00009220: 6c28 2374 6572 6d69 6e61 6c2d 3136 3330  l(#terminal-1630
-00009230: 3637 3637 342d 6c69 6e65 2d33 2922 3e43  67674-line-3)">C
-00009240: 6f70 7972 6967 6874 2623 3136 303b 2863  opyright&#160;(c
-00009250: 2926 2331 3630 3b32 3032 332d 7072 6573  )&#160;2023-pres
-00009260: 656e 7426 2331 3630 3b4a 7573 7469 6e26  ent&#160;Justin&
-00009270: 2331 3630 3b46 6c61 6e6e 6572 7926 2331  #160;Flannery&#1
-00009280: 3630 3b26 6c74 3b6a 7573 7469 6e2e 666c  60;&lt;justin.fl
-00009290: 616e 6e65 7279 406a 7566 7469 6e2e 636f  annery@juftin.co
-000092a0: 6d26 6774 3b26 2331 3630 3b26 2331 3630  m&gt;&#160;&#160
-000092b0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-000092c0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-000092d0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-000092e0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-000092f0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009300: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009310: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009320: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009330: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009340: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009350: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009360: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009370: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009380: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009390: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-000093a0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-000093b0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-000093c0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-000093d0: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-000093e0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-000093f0: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009400: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009410: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009420: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009430: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009440: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009450: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009460: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-00009470: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
-00009480: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
-00009490: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
-000094a0: 3630 3b26 2331 3630 3b26 2331 3630 3b3c  60;&#160;&#160;<
-000094b0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-000094c0: 733d 2274 6572 6d69 6e61 6c2d 3136 3330  s="terminal-1630
-000094d0: 3637 3637 342d 7231 2220 783d 2231 3935  67674-r1" x="195
-000094e0: 3222 2079 3d22 3933 2e32 2220 7465 7874  2" y="93.2" text
-000094f0: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-00009500: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-00009510: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-00009520: 2d6c 696e 652d 3329 223e 0a3c 2f74 6578  -line-3)">.</tex
-00009530: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-00009540: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-00009550: 342d 7231 2220 783d 2231 3935 3222 2079  4-r1" x="1952" y
-00009560: 3d22 3131 372e 3622 2074 6578 744c 656e  ="117.6" textLen
-00009570: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
-00009580: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-00009590: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
-000095a0: 6e65 2d34 2922 3e0a 3c2f 7465 7874 3e3c  ne-4)">.</text><
-000095b0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-000095c0: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-000095d0: 3422 2078 3d22 3022 2079 3d22 3134 3222  4" x="0" y="142"
-000095e0: 2074 6578 744c 656e 6774 683d 2231 3932   textLength="192
-000095f0: 372e 3622 2063 6c69 702d 7061 7468 3d22  7.6" clip-path="
-00009600: 7572 6c28 2374 6572 6d69 6e61 6c2d 3136  url(#terminal-16
-00009610: 3330 3637 3637 342d 6c69 6e65 2d35 2922  3067674-line-5)"
-00009620: 3e50 6572 6d69 7373 696f 6e26 2331 3630  >Permission&#160
-00009630: 3b69 7326 2331 3630 3b68 6572 6562 7926  ;is&#160;hereby&
-00009640: 2331 3630 3b67 7261 6e74 6564 2c26 2331  #160;granted,&#1
-00009650: 3630 3b66 7265 6526 2331 3630 3b6f 6626  60;free&#160;of&
-00009660: 2331 3630 3b63 6861 7267 652c 2623 3136  #160;charge,&#16
-00009670: 303b 746f 2623 3136 303b 616e 7926 2331  0;to&#160;any&#1
-00009680: 3630 3b70 6572 736f 6e26 2331 3630 3b6f  60;person&#160;o
-00009690: 6274 6169 6e69 6e67 2623 3136 303b 6126  btaining&#160;a&
-000096a0: 2331 3630 3b63 6f70 7926 2331 3630 3b6f  #160;copy&#160;o
-000096b0: 6626 2331 3630 3b74 6869 7326 2331 3630  f&#160;this&#160
-000096c0: 3b73 6f66 7477 6172 6526 2331 3630 3b61  ;software&#160;a
-000096d0: 6e64 2623 3136 303b 6173 736f 6369 6174  nd&#160;associat
-000096e0: 6564 2623 3136 303b 646f 6375 6d65 6e74  ed&#160;document
-000096f0: 6174 696f 6e26 2331 3630 3b66 696c 6573  ation&#160;files
-00009700: 2623 3136 303b 2874 6865 2623 3136 303b  &#160;(the&#160;
-00009710: 2671 756f 743b 536f 6674 7761 7265 2671  &quot;Software&q
-00009720: 756f 743b 292c 2623 3136 303b 746f 2623  uot;),&#160;to&#
-00009730: 3136 303b 6465 616c 2623 3136 303b 696e  160;deal&#160;in
-00009740: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-00009750: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-00009760: 616c 2d31 3633 3036 3736 3734 2d72 3122  al-163067674-r1"
-00009770: 2078 3d22 3139 3532 2220 793d 2231 3432   x="1952" y="142
-00009780: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-00009790: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-000097a0: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-000097b0: 3036 3736 3734 2d6c 696e 652d 3529 223e  067674-line-5)">
-000097c0: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
-000097d0: 6173 733d 2274 6572 6d69 6e61 6c2d 3136  ass="terminal-16
-000097e0: 3330 3637 3637 342d 7231 2220 783d 2231  3067674-r1" x="1
-000097f0: 3935 3222 2079 3d22 3136 362e 3422 2074  952" y="166.4" t
-00009800: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
-00009810: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00009820: 2374 6572 6d69 6e61 6c2d 3136 3330 3637  #terminal-163067
-00009830: 3637 342d 6c69 6e65 2d36 2922 3e0a 3c2f  674-line-6)">.</
-00009840: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-00009850: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00009860: 3736 3734 2d72 3422 2078 3d22 3022 2079  7674-r4" x="0" y
-00009870: 3d22 3139 302e 3822 2074 6578 744c 656e  ="190.8" textLen
-00009880: 6774 683d 2231 3932 372e 3622 2063 6c69  gth="1927.6" cli
-00009890: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-000098a0: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
-000098b0: 6c69 6e65 2d37 2922 3e54 6865 2623 3136  line-7)">The&#16
-000098c0: 303b 6162 6f76 6526 2331 3630 3b63 6f70  0;above&#160;cop
-000098d0: 7972 6967 6874 2623 3136 303b 6e6f 7469  yright&#160;noti
-000098e0: 6365 2623 3136 303b 616e 6426 2331 3630  ce&#160;and&#160
-000098f0: 3b74 6869 7326 2331 3630 3b70 6572 6d69  ;this&#160;permi
-00009900: 7373 696f 6e26 2331 3630 3b6e 6f74 6963  ssion&#160;notic
-00009910: 6526 2331 3630 3b73 6861 6c6c 2623 3136  e&#160;shall&#16
-00009920: 303b 6265 2623 3136 303b 696e 636c 7564  0;be&#160;includ
-00009930: 6564 2623 3136 303b 696e 2623 3136 303b  ed&#160;in&#160;
-00009940: 616c 6c26 2331 3630 3b63 6f70 6965 7326  all&#160;copies&
-00009950: 2331 3630 3b6f 7226 2331 3630 3b73 7562  #160;or&#160;sub
-00009960: 7374 616e 7469 616c 2623 3136 303b 706f  stantial&#160;po
-00009970: 7274 696f 6e73 2623 3136 303b 6f66 2623  rtions&#160;of&#
-00009980: 3136 303b 7468 6526 2331 3630 3b53 6f66  160;the&#160;Sof
-00009990: 7477 6172 652e 2623 3136 303b 2623 3136  tware.&#160;&#16
-000099a0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
-000099b0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
-000099c0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
-000099d0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
-000099e0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
-000099f0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
-00009a00: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
-00009a10: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
-00009a20: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
-00009a30: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
-00009a40: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
-00009a50: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-00009a60: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-00009a70: 616c 2d31 3633 3036 3736 3734 2d72 3122  al-163067674-r1"
-00009a80: 2078 3d22 3139 3532 2220 793d 2231 3930   x="1952" y="190
-00009a90: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
-00009aa0: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-00009ab0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-00009ac0: 3633 3036 3736 3734 2d6c 696e 652d 3729  63067674-line-7)
-00009ad0: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
-00009ae0: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-00009af0: 3136 3330 3637 3637 342d 7231 2220 783d  163067674-r1" x=
-00009b00: 2231 3935 3222 2079 3d22 3231 352e 3222  "1952" y="215.2"
-00009b10: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
-00009b20: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
-00009b30: 6c28 2374 6572 6d69 6e61 6c2d 3136 3330  l(#terminal-1630
-00009b40: 3637 3637 342d 6c69 6e65 2d38 2922 3e0a  67674-line-8)">.
-00009b50: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-00009b60: 7373 3d22 7465 726d 696e 616c 2d31 3633  ss="terminal-163
-00009b70: 3036 3736 3734 2d72 3422 2078 3d22 3022  067674-r4" x="0"
-00009b80: 2079 3d22 3233 392e 3622 2074 6578 744c   y="239.6" textL
-00009b90: 656e 6774 683d 2231 3932 372e 3622 2063  ength="1927.6" c
-00009ba0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
-00009bb0: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-00009bc0: 342d 6c69 6e65 2d39 2922 3e54 4845 2623  4-line-9)">THE&#
-00009bd0: 3136 303b 534f 4654 5741 5245 2623 3136  160;SOFTWARE&#16
-00009be0: 303b 4953 2623 3136 303b 5052 4f56 4944  0;IS&#160;PROVID
-00009bf0: 4544 2623 3136 303b 2671 756f 743b 4153  ED&#160;&quot;AS
-00009c00: 2623 3136 303b 4953 2671 756f 743b 2c26  &#160;IS&quot;,&
-00009c10: 2331 3630 3b57 4954 484f 5554 2623 3136  #160;WITHOUT&#16
-00009c20: 303b 5741 5252 414e 5459 2623 3136 303b  0;WARRANTY&#160;
-00009c30: 4f46 2623 3136 303b 414e 5926 2331 3630  OF&#160;ANY&#160
-00009c40: 3b4b 494e 442c 2623 3136 303b 4558 5052  ;KIND,&#160;EXPR
-00009c50: 4553 5326 2331 3630 3b4f 5226 2331 3630  ESS&#160;OR&#160
-00009c60: 3b49 4d50 4c49 4544 2c26 2331 3630 3b49  ;IMPLIED,&#160;I
-00009c70: 4e43 4c55 4449 4e47 2623 3136 303b 4255  NCLUDING&#160;BU
-00009c80: 5426 2331 3630 3b4e 4f54 2623 3136 303b  T&#160;NOT&#160;
-00009c90: 4c49 4d49 5445 4426 2331 3630 3b54 4f26  LIMITED&#160;TO&
-00009ca0: 2331 3630 3b54 4845 2623 3136 303b 5741  #160;THE&#160;WA
-00009cb0: 5252 414e 5449 4553 2623 3136 303b 4f46  RRANTIES&#160;OF
-00009cc0: 2623 3136 303b 4d45 5243 4841 4e54 4142  &#160;MERCHANTAB
-00009cd0: 494c 4954 592c 2623 3136 303b 4649 544e  ILITY,&#160;FITN
-00009ce0: 4553 5326 2331 3630 3b46 4f3c 2f74 6578  ESS&#160;FO</tex
-00009cf0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-00009d00: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-00009d10: 342d 7231 2220 783d 2231 3935 3222 2079  4-r1" x="1952" y
-00009d20: 3d22 3233 392e 3622 2074 6578 744c 656e  ="239.6" textLen
-00009d30: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
-00009d40: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-00009d50: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
-00009d60: 6e65 2d39 2922 3e0a 3c2f 7465 7874 3e3c  ne-9)">.</text><
-00009d70: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-00009d80: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-00009d90: 3122 2078 3d22 3139 3532 2220 793d 2232  1" x="1952" y="2
-00009da0: 3634 2220 7465 7874 4c65 6e67 7468 3d22  64" textLength="
-00009db0: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-00009dc0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-00009dd0: 3633 3036 3736 3734 2d6c 696e 652d 3130  63067674-line-10
-00009de0: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-00009df0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-00009e00: 2d31 3633 3036 3736 3734 2d72 3122 2078  -163067674-r1" x
-00009e10: 3d22 3139 3532 2220 793d 2232 3838 2e34  ="1952" y="288.4
-00009e20: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-00009e30: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-00009e40: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-00009e50: 3036 3736 3734 2d6c 696e 652d 3131 2922  067674-line-11)"
-00009e60: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
-00009e70: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-00009e80: 3633 3036 3736 3734 2d72 3122 2078 3d22  63067674-r1" x="
-00009e90: 3139 3532 2220 793d 2233 3132 2e38 2220  1952" y="312.8" 
-00009ea0: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-00009eb0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-00009ec0: 2823 7465 726d 696e 616c 2d31 3633 3036  (#terminal-16306
-00009ed0: 3736 3734 2d6c 696e 652d 3132 2922 3e0a  7674-line-12)">.
-00009ee0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-00009ef0: 7373 3d22 7465 726d 696e 616c 2d31 3633  ss="terminal-163
-00009f00: 3036 3736 3734 2d72 3122 2078 3d22 3139  067674-r1" x="19
-00009f10: 3532 2220 793d 2233 3337 2e32 2220 7465  52" y="337.2" te
-00009f20: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
-00009f30: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00009f40: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-00009f50: 3734 2d6c 696e 652d 3133 2922 3e0a 3c2f  74-line-13)">.</
-00009f60: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-00009f70: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-00009f80: 3736 3734 2d72 3122 2078 3d22 3139 3532  7674-r1" x="1952
-00009f90: 2220 793d 2233 3631 2e36 2220 7465 7874  " y="361.6" text
-00009fa0: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-00009fb0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-00009fc0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-00009fd0: 2d6c 696e 652d 3134 2922 3e0a 3c2f 7465  -line-14)">.</te
-00009fe0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-00009ff0: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000a000: 3734 2d72 3122 2078 3d22 3139 3532 2220  74-r1" x="1952" 
-0000a010: 793d 2233 3836 2220 7465 7874 4c65 6e67  y="386" textLeng
-0000a020: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
-0000a030: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000a040: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
-0000a050: 652d 3135 2922 3e0a 3c2f 7465 7874 3e3c  e-15)">.</text><
-0000a060: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000a070: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000a080: 3122 2078 3d22 3139 3532 2220 793d 2234  1" x="1952" y="4
-0000a090: 3130 2e34 2220 7465 7874 4c65 6e67 7468  10.4" textLength
-0000a0a0: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000a0b0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000a0c0: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
-0000a0d0: 3136 2922 3e0a 3c2f 7465 7874 3e3c 7465  16)">.</text><te
-0000a0e0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000a0f0: 616c 2d31 3633 3036 3736 3734 2d72 3122  al-163067674-r1"
-0000a100: 2078 3d22 3139 3532 2220 793d 2234 3334   x="1952" y="434
-0000a110: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
-0000a120: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000a130: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000a140: 3633 3036 3736 3734 2d6c 696e 652d 3137  63067674-line-17
-0000a150: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000a160: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000a170: 2d31 3633 3036 3736 3734 2d72 3122 2078  -163067674-r1" x
-0000a180: 3d22 3139 3532 2220 793d 2234 3539 2e32  ="1952" y="459.2
-0000a190: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000a1a0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000a1b0: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-0000a1c0: 3036 3736 3734 2d6c 696e 652d 3138 2922  067674-line-18)"
-0000a1d0: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
-0000a1e0: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000a1f0: 3633 3036 3736 3734 2d72 3122 2078 3d22  63067674-r1" x="
-0000a200: 3139 3532 2220 793d 2234 3833 2e36 2220  1952" y="483.6" 
-0000a210: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-0000a220: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000a230: 2823 7465 726d 696e 616c 2d31 3633 3036  (#terminal-16306
-0000a240: 3736 3734 2d6c 696e 652d 3139 2922 3e0a  7674-line-19)">.
-0000a250: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000a260: 7373 3d22 7465 726d 696e 616c 2d31 3633  ss="terminal-163
-0000a270: 3036 3736 3734 2d72 3122 2078 3d22 3139  067674-r1" x="19
-0000a280: 3532 2220 793d 2235 3038 2220 7465 7874  52" y="508" text
-0000a290: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000a2a0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000a2b0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000a2c0: 2d6c 696e 652d 3230 2922 3e0a 3c2f 7465  -line-20)">.</te
-0000a2d0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000a2e0: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000a2f0: 3734 2d72 3122 2078 3d22 3139 3532 2220  74-r1" x="1952" 
-0000a300: 793d 2235 3332 2e34 2220 7465 7874 4c65  y="532.4" textLe
-0000a310: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
-0000a320: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000a330: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
-0000a340: 696e 652d 3231 2922 3e0a 3c2f 7465 7874  ine-21)">.</text
-0000a350: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000a360: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000a370: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
-0000a380: 2235 3536 2e38 2220 7465 7874 4c65 6e67  "556.8" textLeng
-0000a390: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
-0000a3a0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000a3b0: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
-0000a3c0: 652d 3232 2922 3e0a 3c2f 7465 7874 3e3c  e-22)">.</text><
-0000a3d0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000a3e0: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000a3f0: 3122 2078 3d22 3139 3532 2220 793d 2235  1" x="1952" y="5
-0000a400: 3831 2e32 2220 7465 7874 4c65 6e67 7468  81.2" textLength
-0000a410: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000a420: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000a430: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
-0000a440: 3233 2922 3e0a 3c2f 7465 7874 3e3c 7465  23)">.</text><te
-0000a450: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000a460: 616c 2d31 3633 3036 3736 3734 2d72 3122  al-163067674-r1"
-0000a470: 2078 3d22 3139 3532 2220 793d 2236 3035   x="1952" y="605
-0000a480: 2e36 2220 7465 7874 4c65 6e67 7468 3d22  .6" textLength="
-0000a490: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000a4a0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000a4b0: 3633 3036 3736 3734 2d6c 696e 652d 3234  63067674-line-24
-0000a4c0: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000a4d0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000a4e0: 2d31 3633 3036 3736 3734 2d72 3122 2078  -163067674-r1" x
-0000a4f0: 3d22 3139 3532 2220 793d 2236 3330 2220  ="1952" y="630" 
-0000a500: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-0000a510: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000a520: 2823 7465 726d 696e 616c 2d31 3633 3036  (#terminal-16306
-0000a530: 3736 3734 2d6c 696e 652d 3235 2922 3e0a  7674-line-25)">.
-0000a540: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000a550: 7373 3d22 7465 726d 696e 616c 2d31 3633  ss="terminal-163
-0000a560: 3036 3736 3734 2d72 3122 2078 3d22 3139  067674-r1" x="19
-0000a570: 3532 2220 793d 2236 3534 2e34 2220 7465  52" y="654.4" te
-0000a580: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
-0000a590: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000a5a0: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000a5b0: 3734 2d6c 696e 652d 3236 2922 3e0a 3c2f  74-line-26)">.</
-0000a5c0: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000a5d0: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-0000a5e0: 3736 3734 2d72 3122 2078 3d22 3139 3532  7674-r1" x="1952
-0000a5f0: 2220 793d 2236 3738 2e38 2220 7465 7874  " y="678.8" text
-0000a600: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000a610: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000a620: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000a630: 2d6c 696e 652d 3237 2922 3e0a 3c2f 7465  -line-27)">.</te
-0000a640: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000a650: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000a660: 3734 2d72 3122 2078 3d22 3139 3532 2220  74-r1" x="1952" 
-0000a670: 793d 2237 3033 2e32 2220 7465 7874 4c65  y="703.2" textLe
-0000a680: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
-0000a690: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000a6a0: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
-0000a6b0: 696e 652d 3238 2922 3e0a 3c2f 7465 7874  ine-28)">.</text
-0000a6c0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000a6d0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000a6e0: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
-0000a6f0: 2237 3237 2e36 2220 7465 7874 4c65 6e67  "727.6" textLeng
-0000a700: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
-0000a710: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000a720: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
-0000a730: 652d 3239 2922 3e0a 3c2f 7465 7874 3e3c  e-29)">.</text><
-0000a740: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000a750: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000a760: 3122 2078 3d22 3139 3532 2220 793d 2237  1" x="1952" y="7
-0000a770: 3532 2220 7465 7874 4c65 6e67 7468 3d22  52" textLength="
-0000a780: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000a790: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000a7a0: 3633 3036 3736 3734 2d6c 696e 652d 3330  63067674-line-30
-0000a7b0: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000a7c0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000a7d0: 2d31 3633 3036 3736 3734 2d72 3122 2078  -163067674-r1" x
-0000a7e0: 3d22 3139 3532 2220 793d 2237 3736 2e34  ="1952" y="776.4
-0000a7f0: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000a800: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000a810: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-0000a820: 3036 3736 3734 2d6c 696e 652d 3331 2922  067674-line-31)"
-0000a830: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
-0000a840: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000a850: 3633 3036 3736 3734 2d72 3122 2078 3d22  63067674-r1" x="
-0000a860: 3139 3532 2220 793d 2238 3030 2e38 2220  1952" y="800.8" 
-0000a870: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-0000a880: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000a890: 2823 7465 726d 696e 616c 2d31 3633 3036  (#terminal-16306
-0000a8a0: 3736 3734 2d6c 696e 652d 3332 2922 3e0a  7674-line-32)">.
-0000a8b0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000a8c0: 7373 3d22 7465 726d 696e 616c 2d31 3633  ss="terminal-163
-0000a8d0: 3036 3736 3734 2d72 3122 2078 3d22 3139  067674-r1" x="19
-0000a8e0: 3532 2220 793d 2238 3235 2e32 2220 7465  52" y="825.2" te
-0000a8f0: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
-0000a900: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000a910: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000a920: 3734 2d6c 696e 652d 3333 2922 3e0a 3c2f  74-line-33)">.</
-0000a930: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
-0000a940: 3d22 7465 726d 696e 616c 2d31 3633 3036  ="terminal-16306
-0000a950: 3736 3734 2d72 3122 2078 3d22 3139 3532  7674-r1" x="1952
-0000a960: 2220 793d 2238 3439 2e36 2220 7465 7874  " y="849.6" text
-0000a970: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000a980: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000a990: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000a9a0: 2d6c 696e 652d 3334 2922 3e0a 3c2f 7465  -line-34)">.</te
-0000a9b0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000a9c0: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000a9d0: 3734 2d72 3122 2078 3d22 3139 3532 2220  74-r1" x="1952" 
-0000a9e0: 793d 2238 3734 2220 7465 7874 4c65 6e67  y="874" textLeng
-0000a9f0: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
-0000aa00: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000aa10: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
-0000aa20: 652d 3335 2922 3e0a 3c2f 7465 7874 3e3c  e-35)">.</text><
-0000aa30: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000aa40: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000aa50: 3122 2078 3d22 3139 3532 2220 793d 2238  1" x="1952" y="8
-0000aa60: 3938 2e34 2220 7465 7874 4c65 6e67 7468  98.4" textLength
-0000aa70: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000aa80: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000aa90: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
-0000aaa0: 3336 2922 3e0a 3c2f 7465 7874 3e3c 7465  36)">.</text><te
-0000aab0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000aac0: 616c 2d31 3633 3036 3736 3734 2d72 3122  al-163067674-r1"
-0000aad0: 2078 3d22 3139 3532 2220 793d 2239 3232   x="1952" y="922
-0000aae0: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
-0000aaf0: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
-0000ab00: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
-0000ab10: 3633 3036 3736 3734 2d6c 696e 652d 3337  63067674-line-37
-0000ab20: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
-0000ab30: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000ab40: 2d31 3633 3036 3736 3734 2d72 3122 2078  -163067674-r1" x
-0000ab50: 3d22 3139 3532 2220 793d 2239 3437 2e32  ="1952" y="947.2
-0000ab60: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000ab70: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000ab80: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-0000ab90: 3036 3736 3734 2d6c 696e 652d 3338 2922  067674-line-38)"
-0000aba0: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
-0000abb0: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000abc0: 3633 3036 3736 3734 2d72 3122 2078 3d22  63067674-r1" x="
-0000abd0: 3139 3532 2220 793d 2239 3731 2e36 2220  1952" y="971.6" 
-0000abe0: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
-0000abf0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000ac00: 2823 7465 726d 696e 616c 2d31 3633 3036  (#terminal-16306
-0000ac10: 3736 3734 2d6c 696e 652d 3339 2922 3e0a  7674-line-39)">.
-0000ac20: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
-0000ac30: 7373 3d22 7465 726d 696e 616c 2d31 3633  ss="terminal-163
-0000ac40: 3036 3736 3734 2d72 3122 2078 3d22 3139  067674-r1" x="19
-0000ac50: 3532 2220 793d 2239 3936 2220 7465 7874  52" y="996" text
-0000ac60: 4c65 6e67 7468 3d22 3132 2e32 2220 636c  Length="12.2" cl
-0000ac70: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000ac80: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000ac90: 2d6c 696e 652d 3430 2922 3e0a 3c2f 7465  -line-40)">.</te
-0000aca0: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000acb0: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000acc0: 3734 2d72 3122 2078 3d22 3139 3532 2220  74-r1" x="1952" 
-0000acd0: 793d 2231 3032 302e 3422 2074 6578 744c  y="1020.4" textL
-0000ace0: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
-0000acf0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
-0000ad00: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
-0000ad10: 6c69 6e65 2d34 3129 223e 0a3c 2f74 6578  line-41)">.</tex
-0000ad20: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000ad30: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-0000ad40: 342d 7231 2220 783d 2231 3935 3222 2079  4-r1" x="1952" y
-0000ad50: 3d22 3130 3434 2e38 2220 7465 7874 4c65  ="1044.8" textLe
-0000ad60: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
-0000ad70: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000ad80: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
-0000ad90: 696e 652d 3432 2922 3e0a 3c2f 7465 7874  ine-42)">.</text
-0000ada0: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000adb0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000adc0: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
-0000add0: 2231 3036 392e 3222 2074 6578 744c 656e  "1069.2" textLen
-0000ade0: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
-0000adf0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000ae00: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
-0000ae10: 6e65 2d34 3329 223e 0a3c 2f74 6578 743e  ne-43)">.</text>
-0000ae20: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
-0000ae30: 6d69 6e61 6c2d 3136 3330 3637 3637 342d  minal-163067674-
-0000ae40: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
-0000ae50: 3130 3933 2e36 2220 7465 7874 4c65 6e67  1093.6" textLeng
-0000ae60: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
-0000ae70: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000ae80: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
-0000ae90: 652d 3434 2922 3e0a 3c2f 7465 7874 3e3c  e-44)">.</text><
-0000aea0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000aeb0: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000aec0: 3522 2078 3d22 3635 382e 3822 2079 3d22  5" x="658.8" y="
-0000aed0: 3131 3138 2220 7465 7874 4c65 6e67 7468  1118" textLength
-0000aee0: 3d22 3132 2e32 2220 636c 6970 2d70 6174  ="12.2" clip-pat
-0000aef0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
-0000af00: 2d31 3633 3036 3736 3734 2d6c 696e 652d  -163067674-line-
-0000af10: 3435 2922 3ee2 968d 3c2f 7465 7874 3e3c  45)">...</text><
-0000af20: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000af30: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000af40: 3122 2078 3d22 3139 3532 2220 793d 2231  1" x="1952" y="1
-0000af50: 3131 3822 2074 6578 744c 656e 6774 683d  118" textLength=
-0000af60: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
-0000af70: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000af80: 3136 3330 3637 3637 342d 6c69 6e65 2d34  163067674-line-4
-0000af90: 3529 223e 0a3c 2f74 6578 743e 3c74 6578  5)">.</text><tex
-0000afa0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
-0000afb0: 6c2d 3136 3330 3637 3637 342d 7236 2220  l-163067674-r6" 
-0000afc0: 783d 2231 322e 3222 2079 3d22 3131 3432  x="12.2" y="1142
-0000afd0: 2e34 2220 7465 7874 4c65 6e67 7468 3d22  .4" textLength="
-0000afe0: 3536 312e 3222 2063 6c69 702d 7061 7468  561.2" clip-path
-0000aff0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000b000: 3136 3330 3637 3637 342d 6c69 6e65 2d34  163067674-line-4
-0000b010: 3629 223e f09f 9784 efb8 8fef b88f efb8  6)">............
-0000b020: 8f26 2331 3630 3b26 2331 3630 3b31 4b42  .&#160;&#160;1KB
-0000b030: 2623 3136 303b 2623 3136 303b f09f 92be  &#160;&#160;....
-0000b040: 2623 3136 303b 2623 3136 303b 4c49 4345  &#160;&#160;LICE
-0000b050: 4e53 4526 2331 3630 3b26 2331 3630 3bf0  NSE&#160;&#160;.
-0000b060: 9f93 8226 2331 3630 3b26 2331 3630 3b6a  ...&#160;&#160;j
-0000b070: 7566 7469 6e3a 6272 6f77 7372 4076 312e  uftin:browsr@v1.
-0000b080: 362e 303c 2f74 6578 743e 3c74 6578 7420  6.0</text><text 
-0000b090: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
-0000b0a0: 3136 3330 3637 3637 342d 7231 2220 783d  163067674-r1" x=
-0000b0b0: 2231 3935 3222 2079 3d22 3131 3432 2e34  "1952" y="1142.4
-0000b0c0: 2220 7465 7874 4c65 6e67 7468 3d22 3132  " textLength="12
-0000b0d0: 2e32 2220 636c 6970 2d70 6174 683d 2275  .2" clip-path="u
-0000b0e0: 726c 2823 7465 726d 696e 616c 2d31 3633  rl(#terminal-163
-0000b0f0: 3036 3736 3734 2d6c 696e 652d 3436 2922  067674-line-46)"
-0000b100: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
-0000b110: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
-0000b120: 3633 3036 3736 3734 2d72 3722 2078 3d22  63067674-r7" x="
-0000b130: 3022 2079 3d22 3131 3636 2e38 2220 7465  0" y="1166.8" te
-0000b140: 7874 4c65 6e67 7468 3d22 3336 2e36 2220  xtLength="36.6" 
-0000b150: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000b160: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000b170: 3734 2d6c 696e 652d 3437 2922 3e26 2331  74-line-47)">&#1
-0000b180: 3630 3b51 2623 3136 303b 3c2f 7465 7874  60;Q&#160;</text
-0000b190: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000b1a0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000b1b0: 2d72 3822 2078 3d22 3336 2e36 2220 793d  -r8" x="36.6" y=
-0000b1c0: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
-0000b1d0: 6774 683d 2237 332e 3222 2063 6c69 702d  gth="73.2" clip-
-0000b1e0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
-0000b1f0: 6e61 6c2d 3136 3330 3637 3637 342d 6c69  nal-163067674-li
-0000b200: 6e65 2d34 3729 223e 2623 3136 303b 5175  ne-47)">&#160;Qu
-0000b210: 6974 2623 3136 303b 3c2f 7465 7874 3e3c  it&#160;</text><
-0000b220: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
-0000b230: 696e 616c 2d31 3633 3036 3736 3734 2d72  inal-163067674-r
-0000b240: 3722 2078 3d22 3130 392e 3822 2079 3d22  7" x="109.8" y="
-0000b250: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
-0000b260: 7468 3d22 3336 2e36 2220 636c 6970 2d70  th="36.6" clip-p
-0000b270: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
-0000b280: 616c 2d31 3633 3036 3736 3734 2d6c 696e  al-163067674-lin
-0000b290: 652d 3437 2922 3e26 2331 3630 3b46 2623  e-47)">&#160;F&#
-0000b2a0: 3136 303b 3c2f 7465 7874 3e3c 7465 7874  160;</text><text
-0000b2b0: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
-0000b2c0: 2d31 3633 3036 3736 3734 2d72 3822 2078  -163067674-r8" x
-0000b2d0: 3d22 3134 362e 3422 2079 3d22 3131 3636  ="146.4" y="1166
-0000b2e0: 2e38 2220 7465 7874 4c65 6e67 7468 3d22  .8" textLength="
-0000b2f0: 3137 302e 3822 2063 6c69 702d 7061 7468  170.8" clip-path
-0000b300: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
-0000b310: 3136 3330 3637 3637 342d 6c69 6e65 2d34  163067674-line-4
-0000b320: 3729 223e 2623 3136 303b 546f 6767 6c65  7)">&#160;Toggle
-0000b330: 2623 3136 303b 4669 6c65 7326 2331 3630  &#160;Files&#160
-0000b340: 3b3c 2f74 6578 743e 3c74 6578 7420 636c  ;</text><text cl
-0000b350: 6173 733d 2274 6572 6d69 6e61 6c2d 3136  ass="terminal-16
-0000b360: 3330 3637 3637 342d 7237 2220 783d 2233  3067674-r7" x="3
-0000b370: 3137 2e32 2220 793d 2231 3136 362e 3822  17.2" y="1166.8"
-0000b380: 2074 6578 744c 656e 6774 683d 2233 362e   textLength="36.
-0000b390: 3622 2063 6c69 702d 7061 7468 3d22 7572  6" clip-path="ur
-0000b3a0: 6c28 2374 6572 6d69 6e61 6c2d 3136 3330  l(#terminal-1630
-0000b3b0: 3637 3637 342d 6c69 6e65 2d34 3729 223e  67674-line-47)">
-0000b3c0: 2623 3136 303b 5426 2331 3630 3b3c 2f74  &#160;T&#160;</t
-0000b3d0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
-0000b3e0: 2274 6572 6d69 6e61 6c2d 3136 3330 3637  "terminal-163067
-0000b3f0: 3637 342d 7238 2220 783d 2233 3533 2e38  674-r8" x="353.8
-0000b400: 2220 793d 2231 3136 362e 3822 2074 6578  " y="1166.8" tex
-0000b410: 744c 656e 6774 683d 2231 3730 2e38 2220  tLength="170.8" 
-0000b420: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-0000b430: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000b440: 3734 2d6c 696e 652d 3437 2922 3e26 2331  74-line-47)">&#1
-0000b450: 3630 3b54 6f67 676c 6526 2331 3630 3b54  60;Toggle&#160;T
-0000b460: 6865 6d65 2623 3136 303b 3c2f 7465 7874  heme&#160;</text
-0000b470: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
-0000b480: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000b490: 2d72 3722 2078 3d22 3532 342e 3622 2079  -r7" x="524.6" y
-0000b4a0: 3d22 3131 3636 2e38 2220 7465 7874 4c65  ="1166.8" textLe
-0000b4b0: 6e67 7468 3d22 3336 2e36 2220 636c 6970  ngth="36.6" clip
-0000b4c0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000b4d0: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
-0000b4e0: 696e 652d 3437 2922 3e26 2331 3630 3b4e  ine-47)">&#160;N
-0000b4f0: 2623 3136 303b 3c2f 7465 7874 3e3c 7465  &#160;</text><te
-0000b500: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
-0000b510: 616c 2d31 3633 3036 3736 3734 2d72 3822  al-163067674-r8"
-0000b520: 2078 3d22 3536 312e 3222 2079 3d22 3131   x="561.2" y="11
-0000b530: 3636 2e38 2220 7465 7874 4c65 6e67 7468  66.8" textLength
-0000b540: 3d22 3235 362e 3222 2063 6c69 702d 7061  ="256.2" clip-pa
-0000b550: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
-0000b560: 6c2d 3136 3330 3637 3637 342d 6c69 6e65  l-163067674-line
-0000b570: 2d34 3729 223e 2623 3136 303b 546f 6767  -47)">&#160;Togg
-0000b580: 6c65 2623 3136 303b 4c69 6e65 2623 3136  le&#160;Line&#16
-0000b590: 303b 4e75 6d62 6572 7326 2331 3630 3b3c  0;Numbers&#160;<
-0000b5a0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000b5b0: 733d 2274 6572 6d69 6e61 6c2d 3136 3330  s="terminal-1630
-0000b5c0: 3637 3637 342d 7237 2220 783d 2238 3137  67674-r7" x="817
-0000b5d0: 2e34 2220 793d 2231 3136 362e 3822 2074  .4" y="1166.8" t
-0000b5e0: 6578 744c 656e 6774 683d 2233 362e 3622  extLength="36.6"
-0000b5f0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000b600: 2374 6572 6d69 6e61 6c2d 3136 3330 3637  #terminal-163067
-0000b610: 3637 342d 6c69 6e65 2d34 3729 223e 2623  674-line-47)">&#
-0000b620: 3136 303b 4426 2331 3630 3b3c 2f74 6578  160;D&#160;</tex
-0000b630: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
-0000b640: 6572 6d69 6e61 6c2d 3136 3330 3637 3637  erminal-16306767
-0000b650: 342d 7238 2220 783d 2238 3534 2220 793d  4-r8" x="854" y=
-0000b660: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
-0000b670: 6774 683d 2232 3139 2e36 2220 636c 6970  gth="219.6" clip
-0000b680: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
-0000b690: 696e 616c 2d31 3633 3036 3736 3734 2d6c  inal-163067674-l
-0000b6a0: 696e 652d 3437 2922 3e26 2331 3630 3b54  ine-47)">&#160;T
-0000b6b0: 6f67 676c 6526 2331 3630 3b44 6172 6b26  oggle&#160;Dark&
-0000b6c0: 2331 3630 3b4d 6f64 6526 2331 3630 3b3c  #160;Mode&#160;<
-0000b6d0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
-0000b6e0: 733d 2274 6572 6d69 6e61 6c2d 3136 3330  s="terminal-1630
-0000b6f0: 3637 3637 342d 7237 2220 783d 2231 3037  67674-r7" x="107
-0000b700: 332e 3622 2079 3d22 3131 3636 2e38 2220  3.6" y="1166.8" 
-0000b710: 7465 7874 4c65 6e67 7468 3d22 3336 2e36  textLength="36.6
-0000b720: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-0000b730: 2823 7465 726d 696e 616c 2d31 3633 3036  (#terminal-16306
-0000b740: 3736 3734 2d6c 696e 652d 3437 2922 3e26  7674-line-47)">&
-0000b750: 2331 3630 3b58 2623 3136 303b 3c2f 7465  #160;X&#160;</te
-0000b760: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
-0000b770: 7465 726d 696e 616c 2d31 3633 3036 3736  terminal-1630676
-0000b780: 3734 2d72 3822 2078 3d22 3131 3130 2e32  74-r8" x="1110.2
-0000b790: 2220 793d 2231 3136 362e 3822 2074 6578  " y="1166.8" tex
-0000b7a0: 744c 656e 6774 683d 2231 3833 2220 636c  tLength="183" cl
-0000b7b0: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
-0000b7c0: 726d 696e 616c 2d31 3633 3036 3736 3734  rminal-163067674
-0000b7d0: 2d6c 696e 652d 3437 2922 3e26 2331 3630  -line-47)">&#160
-0000b7e0: 3b44 6f77 6e6c 6f61 6426 2331 3630 3b46  ;Download&#160;F
-0000b7f0: 696c 6526 2331 3630 3b3c 2f74 6578 743e  ile&#160;</text>
-0000b800: 0a20 2020 203c 2f67 3e0a 2020 2020 3c2f  .    </g>.    </
-0000b810: 673e 0a3c 2f73 7667 3e0a                 g>.</svg>.
+00002340: 6474 683d 2230 2220 6865 6967 6874 3d22  dth="0" height="
+00002350: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00002360: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00002370: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00002380: 2223 3138 3138 3138 2220 783d 2231 3834  "#181818" x="184
+00002390: 322e 3222 2079 3d22 312e 3522 2077 6964  2.2" y="1.5" wid
+000023a0: 7468 3d22 3937 2e36 2220 6865 6967 6874  th="97.6" height
+000023b0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000023c0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000023d0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000023e0: 6c3d 2223 3138 3138 3138 2220 783d 2231  l="#181818" x="1
+000023f0: 3933 392e 3822 2079 3d22 312e 3522 2077  939.8" y="1.5" w
+00002400: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00002410: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00002420: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00002430: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00002440: 696c 6c3d 2223 3237 3238 3232 2220 783d  ill="#272822" x=
+00002450: 2230 2220 793d 2232 352e 3922 2077 6964  "0" y="25.9" wid
+00002460: 7468 3d22 3139 3237 2e36 2220 6865 6967  th="1927.6" heig
+00002470: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00002480: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00002490: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000024a0: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+000024b0: 2231 3932 372e 3622 2079 3d22 3235 2e39  "1927.6" y="25.9
+000024c0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+000024d0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+000024e0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+000024f0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00002500: 7420 6669 6c6c 3d22 2332 3732 3832 3222  t fill="#272822"
+00002510: 2078 3d22 3022 2079 3d22 3530 2e33 2220   x="0" y="50.3" 
+00002520: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
+00002530: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00002540: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00002550: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00002560: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00002570: 2078 3d22 3139 3237 2e36 2220 793d 2235   x="1927.6" y="5
+00002580: 302e 3322 2077 6964 7468 3d22 3234 2e34  0.3" width="24.4
+00002590: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000025a0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000025b0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000025c0: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
+000025d0: 3232 2220 783d 2230 2220 793d 2237 342e  22" x="0" y="74.
+000025e0: 3722 2077 6964 7468 3d22 3139 3237 2e36  7" width="1927.6
+000025f0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00002600: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00002610: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00002620: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00002630: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
+00002640: 3d22 3734 2e37 2220 7769 6474 683d 2232  ="74.7" width="2
+00002650: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+00002660: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00002670: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00002680: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00002690: 3732 3832 3222 2078 3d22 3022 2079 3d22  72822" x="0" y="
+000026a0: 3939 2e31 2220 7769 6474 683d 2231 3932  99.1" width="192
+000026b0: 372e 3622 2068 6569 6768 743d 2232 342e  7.6" height="24.
+000026c0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000026d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000026e0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+000026f0: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
+00002700: 2220 793d 2239 392e 3122 2077 6964 7468  " y="99.1" width
+00002710: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00002720: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00002730: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00002740: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00002750: 2223 3237 3238 3232 2220 783d 2230 2220  "#272822" x="0" 
+00002760: 793d 2231 3233 2e35 2220 7769 6474 683d  y="123.5" width=
+00002770: 2231 3932 372e 3622 2068 6569 6768 743d  "1927.6" height=
+00002780: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00002790: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000027a0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+000027b0: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
+000027c0: 3237 2e36 2220 793d 2231 3233 2e35 2220  27.6" y="123.5" 
+000027d0: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
+000027e0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+000027f0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00002800: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00002810: 6669 6c6c 3d22 2332 3732 3832 3222 2078  fill="#272822" x
+00002820: 3d22 3022 2079 3d22 3134 372e 3922 2077  ="0" y="147.9" w
+00002830: 6964 7468 3d22 3139 3237 2e36 2220 6865  idth="1927.6" he
+00002840: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00002850: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00002860: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00002870: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00002880: 783d 2231 3932 372e 3622 2079 3d22 3134  x="1927.6" y="14
+00002890: 372e 3922 2077 6964 7468 3d22 3234 2e34  7.9" width="24.4
+000028a0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000028b0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000028c0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000028d0: 7265 6374 2066 696c 6c3d 2223 3237 3238  rect fill="#2728
+000028e0: 3232 2220 783d 2230 2220 793d 2231 3732  22" x="0" y="172
+000028f0: 2e33 2220 7769 6474 683d 2231 3932 372e  .3" width="1927.
+00002900: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+00002910: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00002920: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00002930: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00002940: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
+00002950: 793d 2231 3732 2e33 2220 7769 6474 683d  y="172.3" width=
+00002960: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00002970: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00002980: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00002990: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000029a0: 2332 3732 3832 3222 2078 3d22 3022 2079  #272822" x="0" y
+000029b0: 3d22 3139 362e 3722 2077 6964 7468 3d22  ="196.7" width="
+000029c0: 3139 3237 2e36 2220 6865 6967 6874 3d22  1927.6" height="
+000029d0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000029e0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000029f0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00002a00: 2223 3134 3139 3166 2220 783d 2231 3932  "#14191f" x="192
+00002a10: 372e 3622 2079 3d22 3139 362e 3722 2077  7.6" y="196.7" w
+00002a20: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
+00002a30: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00002a40: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00002a50: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00002a60: 696c 6c3d 2223 3237 3238 3232 2220 783d  ill="#272822" x=
+00002a70: 2230 2220 793d 2232 3231 2e31 2220 7769  "0" y="221.1" wi
+00002a80: 6474 683d 2231 3932 372e 3622 2068 6569  dth="1927.6" hei
+00002a90: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00002aa0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00002ab0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00002ac0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00002ad0: 3d22 3139 3237 2e36 2220 793d 2232 3231  ="1927.6" y="221
+00002ae0: 2e31 2220 7769 6474 683d 2232 342e 3422  .1" width="24.4"
+00002af0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00002b00: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00002b10: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00002b20: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
+00002b30: 6422 2078 3d22 3022 2079 3d22 3234 352e  d" x="0" y="245.
+00002b40: 3522 2077 6964 7468 3d22 3139 3237 2e36  5" width="1927.6
+00002b50: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00002b60: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00002b70: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00002b80: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00002b90: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
+00002ba0: 3d22 3234 352e 3522 2077 6964 7468 3d22  ="245.5" width="
+00002bb0: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
+00002bc0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00002bd0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00002be0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00002bf0: 3064 3064 3064 2220 783d 2230 2220 793d  0d0d0d" x="0" y=
+00002c00: 2232 3639 2e39 2220 7769 6474 683d 2231  "269.9" width="1
+00002c10: 3932 372e 3622 2068 6569 6768 743d 2232  927.6" height="2
+00002c20: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00002c30: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00002c40: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00002c50: 2331 3431 3931 6622 2078 3d22 3139 3237  #14191f" x="1927
+00002c60: 2e36 2220 793d 2232 3639 2e39 2220 7769  .6" y="269.9" wi
+00002c70: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+00002c80: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002c90: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002ca0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002cb0: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00002cc0: 3022 2079 3d22 3239 342e 3322 2077 6964  0" y="294.3" wid
+00002cd0: 7468 3d22 3139 3237 2e36 2220 6865 6967  th="1927.6" heig
+00002ce0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00002cf0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00002d00: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00002d10: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00002d20: 2231 3932 372e 3622 2079 3d22 3239 342e  "1927.6" y="294.
+00002d30: 3322 2077 6964 7468 3d22 3234 2e34 2220  3" width="24.4" 
+00002d40: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00002d50: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00002d60: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00002d70: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+00002d80: 2220 783d 2230 2220 793d 2233 3138 2e37  " x="0" y="318.7
+00002d90: 2220 7769 6474 683d 2231 3932 372e 3622  " width="1927.6"
+00002da0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00002db0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00002dc0: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00002dd0: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+00002de0: 6622 2078 3d22 3139 3237 2e36 2220 793d  f" x="1927.6" y=
+00002df0: 2233 3138 2e37 2220 7769 6474 683d 2232  "318.7" width="2
+00002e00: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+00002e10: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00002e20: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00002e30: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00002e40: 6430 6430 6422 2078 3d22 3022 2079 3d22  d0d0d" x="0" y="
+00002e50: 3334 332e 3122 2077 6964 7468 3d22 3139  343.1" width="19
+00002e60: 3237 2e36 2220 6865 6967 6874 3d22 3234  27.6" height="24
+00002e70: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00002e80: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00002e90: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00002ea0: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
+00002eb0: 3622 2079 3d22 3334 332e 3122 2077 6964  6" y="343.1" wid
+00002ec0: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
+00002ed0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00002ee0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00002ef0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00002f00: 6c3d 2223 3064 3064 3064 2220 783d 2230  l="#0d0d0d" x="0
+00002f10: 2220 793d 2233 3637 2e35 2220 7769 6474  " y="367.5" widt
+00002f20: 683d 2231 3932 372e 3622 2068 6569 6768  h="1927.6" heigh
+00002f30: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00002f40: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00002f50: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00002f60: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+00002f70: 3139 3237 2e36 2220 793d 2233 3637 2e35  1927.6" y="367.5
+00002f80: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+00002f90: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00002fa0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00002fb0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00002fc0: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
+00002fd0: 2078 3d22 3022 2079 3d22 3339 312e 3922   x="0" y="391.9"
+00002fe0: 2077 6964 7468 3d22 3139 3237 2e36 2220   width="1927.6" 
+00002ff0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00003000: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00003010: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00003020: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00003030: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+00003040: 3339 312e 3922 2077 6964 7468 3d22 3234  391.9" width="24
+00003050: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00003060: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00003070: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00003080: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00003090: 3064 3064 2220 783d 2230 2220 793d 2234  0d0d" x="0" y="4
+000030a0: 3136 2e33 2220 7769 6474 683d 2231 3932  16.3" width="192
+000030b0: 372e 3622 2068 6569 6768 743d 2232 342e  7.6" height="24.
+000030c0: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000030d0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000030e0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+000030f0: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
+00003100: 2220 793d 2234 3136 2e33 2220 7769 6474  " y="416.3" widt
+00003110: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
+00003120: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00003130: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00003140: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00003150: 3d22 2330 6430 6430 6422 2078 3d22 3022  ="#0d0d0d" x="0"
+00003160: 2079 3d22 3434 302e 3722 2077 6964 7468   y="440.7" width
+00003170: 3d22 3139 3237 2e36 2220 6865 6967 6874  ="1927.6" height
+00003180: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00003190: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000031a0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000031b0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+000031c0: 3932 372e 3622 2079 3d22 3434 302e 3722  927.6" y="440.7"
+000031d0: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+000031e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000031f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00003200: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00003210: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00003220: 783d 2230 2220 793d 2234 3635 2e31 2220  x="0" y="465.1" 
+00003230: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
+00003240: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00003250: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00003260: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00003270: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00003280: 2078 3d22 3139 3237 2e36 2220 793d 2234   x="1927.6" y="4
+00003290: 3635 2e31 2220 7769 6474 683d 2232 342e  65.1" width="24.
+000032a0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+000032b0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+000032c0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000032d0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+000032e0: 6430 6422 2078 3d22 3022 2079 3d22 3438  d0d" x="0" y="48
+000032f0: 392e 3522 2077 6964 7468 3d22 3139 3237  9.5" width="1927
+00003300: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
+00003310: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00003320: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00003330: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00003340: 3139 3166 2220 783d 2231 3932 372e 3622  191f" x="1927.6"
+00003350: 2079 3d22 3438 392e 3522 2077 6964 7468   y="489.5" width
+00003360: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00003370: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00003380: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00003390: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000033a0: 2223 3064 3064 3064 2220 783d 2230 2220  "#0d0d0d" x="0" 
+000033b0: 793d 2235 3133 2e39 2220 7769 6474 683d  y="513.9" width=
+000033c0: 2231 3932 372e 3622 2068 6569 6768 743d  "1927.6" height=
+000033d0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000033e0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000033f0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00003400: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
+00003410: 3237 2e36 2220 793d 2235 3133 2e39 2220  27.6" y="513.9" 
+00003420: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
+00003430: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00003440: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00003450: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00003460: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
+00003470: 3d22 3022 2079 3d22 3533 382e 3322 2077  ="0" y="538.3" w
+00003480: 6964 7468 3d22 3139 3237 2e36 2220 6865  idth="1927.6" he
+00003490: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000034a0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000034b0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000034c0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+000034d0: 783d 2231 3932 372e 3622 2079 3d22 3533  x="1927.6" y="53
+000034e0: 382e 3322 2077 6964 7468 3d22 3234 2e34  8.3" width="24.4
+000034f0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00003500: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00003510: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00003520: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+00003530: 3064 2220 783d 2230 2220 793d 2235 3632  0d" x="0" y="562
+00003540: 2e37 2220 7769 6474 683d 2231 3932 372e  .7" width="1927.
+00003550: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+00003560: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00003570: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00003580: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00003590: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
+000035a0: 793d 2235 3632 2e37 2220 7769 6474 683d  y="562.7" width=
+000035b0: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+000035c0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+000035d0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+000035e0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000035f0: 2330 6430 6430 6422 2078 3d22 3022 2079  #0d0d0d" x="0" y
+00003600: 3d22 3538 372e 3122 2077 6964 7468 3d22  ="587.1" width="
+00003610: 3139 3237 2e36 2220 6865 6967 6874 3d22  1927.6" height="
+00003620: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00003630: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00003640: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00003650: 2223 3134 3139 3166 2220 783d 2231 3932  "#14191f" x="192
+00003660: 372e 3622 2079 3d22 3538 372e 3122 2077  7.6" y="587.1" w
+00003670: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
+00003680: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00003690: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000036a0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000036b0: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+000036c0: 2230 2220 793d 2236 3131 2e35 2220 7769  "0" y="611.5" wi
+000036d0: 6474 683d 2231 3932 372e 3622 2068 6569  dth="1927.6" hei
+000036e0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+000036f0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00003700: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00003710: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00003720: 3d22 3139 3237 2e36 2220 793d 2236 3131  ="1927.6" y="611
+00003730: 2e35 2220 7769 6474 683d 2232 342e 3422  .5" width="24.4"
+00003740: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00003750: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00003760: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00003770: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
+00003780: 6422 2078 3d22 3022 2079 3d22 3633 352e  d" x="0" y="635.
+00003790: 3922 2077 6964 7468 3d22 3139 3237 2e36  9" width="1927.6
+000037a0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000037b0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000037c0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000037d0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+000037e0: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
+000037f0: 3d22 3633 352e 3922 2077 6964 7468 3d22  ="635.9" width="
+00003800: 3234 2e34 2220 6865 6967 6874 3d22 3234  24.4" height="24
+00003810: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00003820: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00003830: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00003840: 3064 3064 3064 2220 783d 2230 2220 793d  0d0d0d" x="0" y=
+00003850: 2236 3630 2e33 2220 7769 6474 683d 2231  "660.3" width="1
+00003860: 3932 372e 3622 2068 6569 6768 743d 2232  927.6" height="2
+00003870: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00003880: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00003890: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000038a0: 2331 3431 3931 6622 2078 3d22 3139 3237  #14191f" x="1927
+000038b0: 2e36 2220 793d 2236 3630 2e33 2220 7769  .6" y="660.3" wi
+000038c0: 6474 683d 2232 342e 3422 2068 6569 6768  dth="24.4" heigh
+000038d0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000038e0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000038f0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003900: 6c6c 3d22 2330 6430 6430 6422 2078 3d22  ll="#0d0d0d" x="
+00003910: 3022 2079 3d22 3638 342e 3722 2077 6964  0" y="684.7" wid
+00003920: 7468 3d22 3139 3237 2e36 2220 6865 6967  th="1927.6" heig
+00003930: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00003940: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00003950: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00003960: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00003970: 2231 3932 372e 3622 2079 3d22 3638 342e  "1927.6" y="684.
+00003980: 3722 2077 6964 7468 3d22 3234 2e34 2220  7" width="24.4" 
+00003990: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000039a0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000039b0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+000039c0: 6374 2066 696c 6c3d 2223 3064 3064 3064  ct fill="#0d0d0d
+000039d0: 2220 783d 2230 2220 793d 2237 3039 2e31  " x="0" y="709.1
+000039e0: 2220 7769 6474 683d 2231 3932 372e 3622  " width="1927.6"
+000039f0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00003a00: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00003a10: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00003a20: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+00003a30: 6622 2078 3d22 3139 3237 2e36 2220 793d  f" x="1927.6" y=
+00003a40: 2237 3039 2e31 2220 7769 6474 683d 2232  "709.1" width="2
+00003a50: 342e 3422 2068 6569 6768 743d 2232 342e  4.4" height="24.
+00003a60: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00003a70: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00003a80: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2330  /><rect fill="#0
+00003a90: 6430 6430 6422 2078 3d22 3022 2079 3d22  d0d0d" x="0" y="
+00003aa0: 3733 332e 3522 2077 6964 7468 3d22 3139  733.5" width="19
+00003ab0: 3237 2e36 2220 6865 6967 6874 3d22 3234  27.6" height="24
+00003ac0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00003ad0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00003ae0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00003af0: 3134 3139 3166 2220 783d 2231 3932 372e  14191f" x="1927.
+00003b00: 3622 2079 3d22 3733 332e 3522 2077 6964  6" y="733.5" wid
+00003b10: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
+00003b20: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00003b30: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00003b40: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00003b50: 6c3d 2223 3064 3064 3064 2220 783d 2230  l="#0d0d0d" x="0
+00003b60: 2220 793d 2237 3537 2e39 2220 7769 6474  " y="757.9" widt
+00003b70: 683d 2231 3932 372e 3622 2068 6569 6768  h="1927.6" heigh
+00003b80: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00003b90: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00003ba0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00003bb0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+00003bc0: 3139 3237 2e36 2220 793d 2237 3537 2e39  1927.6" y="757.9
+00003bd0: 2220 7769 6474 683d 2232 342e 3422 2068  " width="24.4" h
+00003be0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00003bf0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00003c00: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00003c10: 7420 6669 6c6c 3d22 2330 6430 6430 6422  t fill="#0d0d0d"
+00003c20: 2078 3d22 3022 2079 3d22 3738 322e 3322   x="0" y="782.3"
+00003c30: 2077 6964 7468 3d22 3139 3237 2e36 2220   width="1927.6" 
+00003c40: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00003c50: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00003c60: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00003c70: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00003c80: 2220 783d 2231 3932 372e 3622 2079 3d22  " x="1927.6" y="
+00003c90: 3738 322e 3322 2077 6964 7468 3d22 3234  782.3" width="24
+00003ca0: 2e34 2220 6865 6967 6874 3d22 3234 2e36  .4" height="24.6
+00003cb0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00003cc0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00003cd0: 3e3c 7265 6374 2066 696c 6c3d 2223 3064  ><rect fill="#0d
+00003ce0: 3064 3064 2220 783d 2230 2220 793d 2238  0d0d" x="0" y="8
+00003cf0: 3036 2e37 2220 7769 6474 683d 2231 3932  06.7" width="192
+00003d00: 372e 3622 2068 6569 6768 743d 2232 342e  7.6" height="24.
+00003d10: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00003d20: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00003d30: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+00003d40: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
+00003d50: 2220 793d 2238 3036 2e37 2220 7769 6474  " y="806.7" widt
+00003d60: 683d 2232 342e 3422 2068 6569 6768 743d  h="24.4" height=
+00003d70: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00003d80: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00003d90: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00003da0: 3d22 2330 6430 6430 6422 2078 3d22 3022  ="#0d0d0d" x="0"
+00003db0: 2079 3d22 3833 312e 3122 2077 6964 7468   y="831.1" width
+00003dc0: 3d22 3139 3237 2e36 2220 6865 6967 6874  ="1927.6" height
+00003dd0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00003de0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00003df0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00003e00: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+00003e10: 3932 372e 3622 2079 3d22 3833 312e 3122  927.6" y="831.1"
+00003e20: 2077 6964 7468 3d22 3234 2e34 2220 6865   width="24.4" he
+00003e30: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00003e40: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00003e50: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00003e60: 2066 696c 6c3d 2223 3064 3064 3064 2220   fill="#0d0d0d" 
+00003e70: 783d 2230 2220 793d 2238 3535 2e35 2220  x="0" y="855.5" 
+00003e80: 7769 6474 683d 2231 3932 372e 3622 2068  width="1927.6" h
+00003e90: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00003ea0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00003eb0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00003ec0: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00003ed0: 2078 3d22 3139 3237 2e36 2220 793d 2238   x="1927.6" y="8
+00003ee0: 3535 2e35 2220 7769 6474 683d 2232 342e  55.5" width="24.
+00003ef0: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+00003f00: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00003f10: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00003f20: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+00003f30: 6430 6422 2078 3d22 3022 2079 3d22 3837  d0d" x="0" y="87
+00003f40: 392e 3922 2077 6964 7468 3d22 3139 3237  9.9" width="1927
+00003f50: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
+00003f60: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00003f70: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00003f80: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00003f90: 3139 3166 2220 783d 2231 3932 372e 3622  191f" x="1927.6"
+00003fa0: 2079 3d22 3837 392e 3922 2077 6964 7468   y="879.9" width
+00003fb0: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+00003fc0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00003fd0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00003fe0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00003ff0: 2223 3064 3064 3064 2220 783d 2230 2220  "#0d0d0d" x="0" 
+00004000: 793d 2239 3034 2e33 2220 7769 6474 683d  y="904.3" width=
+00004010: 2231 3932 372e 3622 2068 6569 6768 743d  "1927.6" height=
+00004020: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00004030: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00004040: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00004050: 3d22 2331 3431 3931 6622 2078 3d22 3139  ="#14191f" x="19
+00004060: 3237 2e36 2220 793d 2239 3034 2e33 2220  27.6" y="904.3" 
+00004070: 7769 6474 683d 2232 342e 3422 2068 6569  width="24.4" hei
+00004080: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00004090: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+000040a0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+000040b0: 6669 6c6c 3d22 2330 6430 6430 6422 2078  fill="#0d0d0d" x
+000040c0: 3d22 3022 2079 3d22 3932 382e 3722 2077  ="0" y="928.7" w
+000040d0: 6964 7468 3d22 3139 3237 2e36 2220 6865  idth="1927.6" he
+000040e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000040f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004100: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004110: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00004120: 783d 2231 3932 372e 3622 2079 3d22 3932  x="1927.6" y="92
+00004130: 382e 3722 2077 6964 7468 3d22 3234 2e34  8.7" width="24.4
+00004140: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00004150: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00004160: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00004170: 7265 6374 2066 696c 6c3d 2223 3064 3064  rect fill="#0d0d
+00004180: 3064 2220 783d 2230 2220 793d 2239 3533  0d" x="0" y="953
+00004190: 2e31 2220 7769 6474 683d 2231 3932 372e  .1" width="1927.
+000041a0: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+000041b0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+000041c0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000041d0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+000041e0: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
+000041f0: 793d 2239 3533 2e31 2220 7769 6474 683d  y="953.1" width=
+00004200: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00004210: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00004220: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00004230: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00004240: 2330 6430 6430 6422 2078 3d22 3022 2079  #0d0d0d" x="0" y
+00004250: 3d22 3937 372e 3522 2077 6964 7468 3d22  ="977.5" width="
+00004260: 3139 3237 2e36 2220 6865 6967 6874 3d22  1927.6" height="
+00004270: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004280: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004290: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000042a0: 2223 3134 3139 3166 2220 783d 2231 3932  "#14191f" x="192
+000042b0: 372e 3622 2079 3d22 3937 372e 3522 2077  7.6" y="977.5" w
+000042c0: 6964 7468 3d22 3234 2e34 2220 6865 6967  idth="24.4" heig
+000042d0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+000042e0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000042f0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00004300: 696c 6c3d 2223 3064 3064 3064 2220 783d  ill="#0d0d0d" x=
+00004310: 2230 2220 793d 2231 3030 312e 3922 2077  "0" y="1001.9" w
+00004320: 6964 7468 3d22 3139 3237 2e36 2220 6865  idth="1927.6" he
+00004330: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00004340: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004350: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004360: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00004370: 783d 2231 3932 372e 3622 2079 3d22 3130  x="1927.6" y="10
+00004380: 3031 2e39 2220 7769 6474 683d 2232 342e  01.9" width="24.
+00004390: 3422 2068 6569 6768 743d 2232 342e 3635  4" height="24.65
+000043a0: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+000043b0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000043c0: 3c72 6563 7420 6669 6c6c 3d22 2330 6430  <rect fill="#0d0
+000043d0: 6430 6422 2078 3d22 3022 2079 3d22 3130  d0d" x="0" y="10
+000043e0: 3236 2e33 2220 7769 6474 683d 2231 3932  26.3" width="192
+000043f0: 372e 3622 2068 6569 6768 743d 2232 342e  7.6" height="24.
+00004400: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00004410: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00004420: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+00004430: 3431 3931 6622 2078 3d22 3139 3237 2e36  4191f" x="1927.6
+00004440: 2220 793d 2231 3032 362e 3322 2077 6964  " y="1026.3" wid
+00004450: 7468 3d22 3234 2e34 2220 6865 6967 6874  th="24.4" height
+00004460: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00004470: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00004480: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00004490: 6c3d 2223 3064 3064 3064 2220 783d 2230  l="#0d0d0d" x="0
+000044a0: 2220 793d 2231 3035 302e 3722 2077 6964  " y="1050.7" wid
+000044b0: 7468 3d22 3139 3237 2e36 2220 6865 6967  th="1927.6" heig
+000044c0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+000044d0: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000044e0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000044f0: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00004500: 2231 3932 372e 3622 2079 3d22 3130 3530  "1927.6" y="1050
+00004510: 2e37 2220 7769 6474 683d 2232 342e 3422  .7" width="24.4"
+00004520: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00004530: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00004540: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00004550: 6563 7420 6669 6c6c 3d22 2330 6430 6430  ect fill="#0d0d0
+00004560: 6422 2078 3d22 3022 2079 3d22 3130 3735  d" x="0" y="1075
+00004570: 2e31 2220 7769 6474 683d 2231 3932 372e  .1" width="1927.
+00004580: 3622 2068 6569 6768 743d 2232 342e 3635  6" height="24.65
+00004590: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+000045a0: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000045b0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+000045c0: 3931 6622 2078 3d22 3139 3237 2e36 2220  91f" x="1927.6" 
+000045d0: 793d 2231 3037 352e 3122 2077 6964 7468  y="1075.1" width
+000045e0: 3d22 3234 2e34 2220 6865 6967 6874 3d22  ="24.4" height="
+000045f0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004600: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004610: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004620: 2223 3233 3536 3862 2220 783d 2230 2220  "#23568b" x="0" 
+00004630: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00004640: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00004650: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004660: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004670: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004680: 2223 3233 3536 3862 2220 783d 2231 322e  "#23568b" x="12.
+00004690: 3222 2079 3d22 3130 3939 2e35 2220 7769  2" y="1099.5" wi
+000046a0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+000046b0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000046c0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000046d0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+000046e0: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
+000046f0: 3234 2e34 2220 793d 2231 3039 392e 3522  24.4" y="1099.5"
+00004700: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00004710: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00004720: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004730: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004740: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00004750: 783d 2233 362e 3622 2079 3d22 3130 3939  x="36.6" y="1099
+00004760: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+00004770: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00004780: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00004790: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+000047a0: 6563 7420 6669 6c6c 3d22 2332 3335 3638  ect fill="#23568
+000047b0: 6222 2078 3d22 3438 2e38 2220 793d 2231  b" x="48.8" y="1
+000047c0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+000047d0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000047e0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000047f0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004800: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00004810: 3536 3862 2220 783d 2236 3122 2079 3d22  568b" x="61" y="
+00004820: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00004830: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
+00004840: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00004850: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00004860: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2332  /><rect fill="#2
+00004870: 3335 3638 6222 2078 3d22 3733 2e32 2220  3568b" x="73.2" 
+00004880: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00004890: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+000048a0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000048b0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000048c0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000048d0: 2223 3233 3536 3862 2220 783d 2238 352e  "#23568b" x="85.
+000048e0: 3422 2079 3d22 3130 3939 2e35 2220 7769  4" y="1099.5" wi
+000048f0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00004900: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00004910: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00004920: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00004930: 6c6c 3d22 2332 3335 3638 6222 2078 3d22  ll="#23568b" x="
+00004940: 3937 2e36 2220 793d 2231 3039 392e 3522  97.6" y="1099.5"
+00004950: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00004960: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00004970: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004980: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004990: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+000049a0: 783d 2231 3039 2e38 2220 793d 2231 3039  x="109.8" y="109
+000049b0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000049c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000049d0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000049e0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000049f0: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00004a00: 3862 2220 783d 2231 3232 2220 793d 2231  8b" x="122" y="1
+00004a10: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00004a20: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00004a30: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00004a40: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004a50: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00004a60: 3536 3862 2220 783d 2231 3334 2e32 2220  568b" x="134.2" 
+00004a70: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00004a80: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00004a90: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004aa0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004ab0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004ac0: 2223 3233 3536 3862 2220 783d 2231 3436  "#23568b" x="146
+00004ad0: 2e34 2220 793d 2231 3039 392e 3522 2077  .4" y="1099.5" w
+00004ae0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00004af0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00004b00: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00004b10: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00004b20: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00004b30: 2231 3538 2e36 2220 793d 2231 3039 392e  "158.6" y="1099.
+00004b40: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00004b50: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00004b60: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00004b70: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00004b80: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+00004b90: 2220 783d 2231 3730 2e38 2220 793d 2231  " x="170.8" y="1
+00004ba0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00004bb0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00004bc0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00004bd0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004be0: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00004bf0: 3536 3862 2220 783d 2231 3833 2220 793d  568b" x="183" y=
+00004c00: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00004c10: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00004c20: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00004c30: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00004c40: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00004c50: 3233 3536 3862 2220 783d 2231 3935 2e32  23568b" x="195.2
+00004c60: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00004c70: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00004c80: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00004c90: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00004ca0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00004cb0: 6c3d 2223 3233 3536 3862 2220 783d 2232  l="#23568b" x="2
+00004cc0: 3037 2e34 2220 793d 2231 3039 392e 3522  07.4" y="1099.5"
+00004cd0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00004ce0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00004cf0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00004d00: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00004d10: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00004d20: 783d 2232 3139 2e36 2220 793d 2231 3039  x="219.6" y="109
+00004d30: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00004d40: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00004d50: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00004d60: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00004d70: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00004d80: 3862 2220 783d 2232 3331 2e38 2220 793d  8b" x="231.8" y=
+00004d90: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00004da0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00004db0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00004dc0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00004dd0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00004de0: 3233 3536 3862 2220 783d 2232 3434 2220  23568b" x="244" 
+00004df0: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00004e00: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00004e10: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004e20: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004e30: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004e40: 2223 3233 3536 3862 2220 783d 2232 3536  "#23568b" x="256
+00004e50: 2e32 2220 793d 2231 3039 392e 3522 2077  .2" y="1099.5" w
+00004e60: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00004e70: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00004e80: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00004e90: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00004ea0: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00004eb0: 2232 3638 2e34 2220 793d 2231 3039 392e  "268.4" y="1099.
+00004ec0: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00004ed0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00004ee0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00004ef0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00004f00: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+00004f10: 2220 783d 2232 3830 2e36 2220 793d 2231  " x="280.6" y="1
+00004f20: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00004f30: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00004f40: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00004f50: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00004f60: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00004f70: 3536 3862 2220 783d 2232 3932 2e38 2220  568b" x="292.8" 
+00004f80: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00004f90: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00004fa0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00004fb0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00004fc0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00004fd0: 2223 3233 3536 3862 2220 783d 2233 3035  "#23568b" x="305
+00004fe0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00004ff0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00005000: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005010: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005020: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005030: 6c3d 2223 3233 3536 3862 2220 783d 2233  l="#23568b" x="3
+00005040: 3137 2e32 2220 793d 2231 3039 392e 3522  17.2" y="1099.5"
+00005050: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00005060: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005070: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005080: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005090: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+000050a0: 783d 2233 3239 2e34 2220 793d 2231 3039  x="329.4" y="109
+000050b0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000050c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000050d0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000050e0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000050f0: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00005100: 3862 2220 783d 2233 3431 2e36 2220 793d  8b" x="341.6" y=
+00005110: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00005120: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00005130: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00005140: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00005150: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00005160: 3233 3536 3862 2220 783d 2233 3533 2e38  23568b" x="353.8
+00005170: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00005180: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00005190: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000051a0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000051b0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000051c0: 6c3d 2223 3233 3536 3862 2220 783d 2233  l="#23568b" x="3
+000051d0: 3636 2220 793d 2231 3039 392e 3522 2077  66" y="1099.5" w
+000051e0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+000051f0: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00005200: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00005210: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00005220: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00005230: 2233 3738 2e32 2220 793d 2231 3039 392e  "378.2" y="1099.
+00005240: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00005250: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00005260: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00005270: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00005280: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+00005290: 2220 783d 2233 3930 2e34 2220 793d 2231  " x="390.4" y="1
+000052a0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+000052b0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000052c0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000052d0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000052e0: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+000052f0: 3536 3862 2220 783d 2234 3032 2e36 2220  568b" x="402.6" 
+00005300: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00005310: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00005320: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00005330: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00005340: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00005350: 2223 3233 3536 3862 2220 783d 2234 3134  "#23568b" x="414
+00005360: 2e38 2220 793d 2231 3039 392e 3522 2077  .8" y="1099.5" w
+00005370: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00005380: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00005390: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000053a0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000053b0: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+000053c0: 2234 3237 2220 793d 2231 3039 392e 3522  "427" y="1099.5"
+000053d0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+000053e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000053f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005400: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005410: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00005420: 783d 2234 3339 2e32 2220 793d 2231 3039  x="439.2" y="109
+00005430: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00005440: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00005450: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00005460: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00005470: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00005480: 3862 2220 783d 2234 3531 2e34 2220 793d  8b" x="451.4" y=
+00005490: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+000054a0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+000054b0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+000054c0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+000054d0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+000054e0: 3233 3536 3862 2220 783d 2234 3633 2e36  23568b" x="463.6
+000054f0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00005500: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00005510: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005520: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005530: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005540: 6c3d 2223 3233 3536 3862 2220 783d 2234  l="#23568b" x="4
+00005550: 3735 2e38 2220 793d 2231 3039 392e 3522  75.8" y="1099.5"
+00005560: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00005570: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005580: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005590: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000055a0: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+000055b0: 783d 2234 3838 2220 793d 2231 3039 392e  x="488" y="1099.
+000055c0: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+000055d0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000055e0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+000055f0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00005600: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+00005610: 2220 783d 2235 3030 2e32 2220 793d 2231  " x="500.2" y="1
+00005620: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00005630: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00005640: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00005650: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00005660: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+00005670: 3536 3862 2220 783d 2235 3132 2e34 2220  568b" x="512.4" 
+00005680: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00005690: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+000056a0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000056b0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000056c0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000056d0: 2223 3233 3536 3862 2220 783d 2235 3234  "#23568b" x="524
+000056e0: 2e36 2220 793d 2231 3039 392e 3522 2077  .6" y="1099.5" w
+000056f0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00005700: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00005710: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00005720: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00005730: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00005740: 2235 3336 2e38 2220 793d 2231 3039 392e  "536.8" y="1099.
+00005750: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00005760: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00005770: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00005780: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00005790: 6374 2066 696c 6c3d 2223 3233 3536 3862  ct fill="#23568b
+000057a0: 2220 783d 2235 3439 2220 793d 2231 3039  " x="549" y="109
+000057b0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000057c0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000057d0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000057e0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000057f0: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00005800: 3862 2220 783d 2235 3631 2e32 2220 793d  8b" x="561.2" y=
+00005810: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00005820: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00005830: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00005840: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00005850: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00005860: 3233 3536 3862 2220 783d 2235 3733 2e34  23568b" x="573.4
+00005870: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00005880: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00005890: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000058a0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000058b0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000058c0: 6c3d 2223 3233 3536 3862 2220 783d 2235  l="#23568b" x="5
+000058d0: 3835 2e36 2220 793d 2231 3039 392e 3522  85.6" y="1099.5"
+000058e0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+000058f0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005900: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005910: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005920: 2066 696c 6c3d 2223 3233 3536 3862 2220   fill="#23568b" 
+00005930: 783d 2235 3937 2e38 2220 793d 2231 3039  x="597.8" y="109
+00005940: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00005950: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00005960: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00005970: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00005980: 7265 6374 2066 696c 6c3d 2223 3233 3536  rect fill="#2356
+00005990: 3862 2220 783d 2236 3130 2220 793d 2231  8b" x="610" y="1
+000059a0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+000059b0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000059c0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000059d0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000059e0: 3e3c 7265 6374 2066 696c 6c3d 2223 3233  ><rect fill="#23
+000059f0: 3536 3862 2220 783d 2236 3232 2e32 2220  568b" x="622.2" 
+00005a00: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00005a10: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00005a20: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00005a30: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00005a40: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00005a50: 2223 3233 3536 3862 2220 783d 2236 3334  "#23568b" x="634
+00005a60: 2e34 2220 793d 2231 3039 392e 3522 2077  .4" y="1099.5" w
+00005a70: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00005a80: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00005a90: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00005aa0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00005ab0: 696c 6c3d 2223 3233 3536 3862 2220 783d  ill="#23568b" x=
+00005ac0: 2236 3436 2e36 2220 793d 2231 3039 392e  "646.6" y="1099.
+00005ad0: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00005ae0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00005af0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00005b00: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00005b10: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00005b20: 2220 783d 2236 3538 2e38 2220 793d 2231  " x="658.8" y="1
+00005b30: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00005b40: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00005b50: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00005b60: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00005b70: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00005b80: 3139 3166 2220 783d 2236 3731 2220 793d  191f" x="671" y=
+00005b90: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00005ba0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00005bb0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00005bc0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00005bd0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00005be0: 3134 3139 3166 2220 783d 2236 3833 2e32  14191f" x="683.2
+00005bf0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00005c00: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00005c10: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005c20: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005c30: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005c40: 6c3d 2223 3134 3139 3166 2220 783d 2236  l="#14191f" x="6
+00005c50: 3935 2e34 2220 793d 2231 3039 392e 3522  95.4" y="1099.5"
+00005c60: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00005c70: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00005c80: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00005c90: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00005ca0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00005cb0: 783d 2237 3037 2e36 2220 793d 2231 3039  x="707.6" y="109
+00005cc0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00005cd0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00005ce0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00005cf0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00005d00: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00005d10: 3166 2220 783d 2237 3139 2e38 2220 793d  1f" x="719.8" y=
+00005d20: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00005d30: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00005d40: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00005d50: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00005d60: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00005d70: 3134 3139 3166 2220 783d 2237 3332 2220  14191f" x="732" 
+00005d80: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00005d90: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00005da0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00005db0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00005dc0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00005dd0: 2223 3134 3139 3166 2220 783d 2237 3434  "#14191f" x="744
+00005de0: 2e32 2220 793d 2231 3039 392e 3522 2077  .2" y="1099.5" w
+00005df0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00005e00: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00005e10: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00005e20: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00005e30: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00005e40: 2237 3536 2e34 2220 793d 2231 3039 392e  "756.4" y="1099.
+00005e50: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00005e60: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00005e70: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00005e80: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00005e90: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00005ea0: 2220 783d 2237 3638 2e36 2220 793d 2231  " x="768.6" y="1
+00005eb0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00005ec0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00005ed0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00005ee0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00005ef0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00005f00: 3139 3166 2220 783d 2237 3830 2e38 2220  191f" x="780.8" 
+00005f10: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00005f20: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00005f30: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00005f40: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00005f50: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00005f60: 2223 3134 3139 3166 2220 783d 2237 3933  "#14191f" x="793
+00005f70: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00005f80: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00005f90: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00005fa0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00005fb0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00005fc0: 6c3d 2223 3134 3139 3166 2220 783d 2238  l="#14191f" x="8
+00005fd0: 3035 2e32 2220 793d 2231 3039 392e 3522  05.2" y="1099.5"
+00005fe0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00005ff0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00006000: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00006010: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00006020: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00006030: 783d 2238 3137 2e34 2220 793d 2231 3039  x="817.4" y="109
+00006040: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00006050: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00006060: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00006070: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00006080: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00006090: 3166 2220 783d 2238 3239 2e36 2220 793d  1f" x="829.6" y=
+000060a0: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+000060b0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+000060c0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+000060d0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+000060e0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+000060f0: 3134 3139 3166 2220 783d 2238 3431 2e38  14191f" x="841.8
+00006100: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00006110: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00006120: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00006130: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00006140: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00006150: 6c3d 2223 3134 3139 3166 2220 783d 2238  l="#14191f" x="8
+00006160: 3534 2220 793d 2231 3039 392e 3522 2077  54" y="1099.5" w
+00006170: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00006180: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00006190: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000061a0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000061b0: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+000061c0: 2238 3636 2e32 2220 793d 2231 3039 392e  "866.2" y="1099.
+000061d0: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+000061e0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+000061f0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006200: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006210: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00006220: 2220 783d 2238 3738 2e34 2220 793d 2231  " x="878.4" y="1
+00006230: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00006240: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00006250: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00006260: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00006270: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00006280: 3139 3166 2220 783d 2238 3930 2e36 2220  191f" x="890.6" 
+00006290: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+000062a0: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+000062b0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000062c0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+000062d0: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+000062e0: 2223 3134 3139 3166 2220 783d 2239 3032  "#14191f" x="902
+000062f0: 2e38 2220 793d 2231 3039 392e 3522 2077  .8" y="1099.5" w
+00006300: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00006310: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00006320: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00006330: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00006340: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00006350: 2239 3135 2220 793d 2231 3039 392e 3522  "915" y="1099.5"
+00006360: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00006370: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00006380: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00006390: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000063a0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+000063b0: 783d 2239 3237 2e32 2220 793d 2231 3039  x="927.2" y="109
+000063c0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000063d0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000063e0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000063f0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00006400: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00006410: 3166 2220 783d 2239 3339 2e34 2220 793d  1f" x="939.4" y=
+00006420: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00006430: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00006440: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00006450: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00006460: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00006470: 3134 3139 3166 2220 783d 2239 3531 2e36  14191f" x="951.6
+00006480: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00006490: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+000064a0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+000064b0: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+000064c0: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000064d0: 6c3d 2223 3134 3139 3166 2220 783d 2239  l="#14191f" x="9
+000064e0: 3633 2e38 2220 793d 2231 3039 392e 3522  63.8" y="1099.5"
+000064f0: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00006500: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00006510: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00006520: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00006530: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00006540: 783d 2239 3736 2220 793d 2231 3039 392e  x="976" y="1099.
+00006550: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00006560: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006570: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006580: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006590: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+000065a0: 2220 783d 2239 3838 2e32 2220 793d 2231  " x="988.2" y="1
+000065b0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+000065c0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000065d0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000065e0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000065f0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00006600: 3139 3166 2220 783d 2231 3030 302e 3422  191f" x="1000.4"
+00006610: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
+00006620: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
+00006630: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00006640: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00006650: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00006660: 3d22 2331 3431 3931 6622 2078 3d22 3130  ="#14191f" x="10
+00006670: 3132 2e36 2220 793d 2231 3039 392e 3522  12.6" y="1099.5"
+00006680: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00006690: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000066a0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000066b0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000066c0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+000066d0: 783d 2231 3032 342e 3822 2079 3d22 3130  x="1024.8" y="10
+000066e0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
+000066f0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00006700: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00006710: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00006720: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00006730: 3931 6622 2078 3d22 3130 3337 2220 793d  91f" x="1037" y=
+00006740: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00006750: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00006760: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00006770: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00006780: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00006790: 3134 3139 3166 2220 783d 2231 3034 392e  14191f" x="1049.
+000067a0: 3222 2079 3d22 3130 3939 2e35 2220 7769  2" y="1099.5" wi
+000067b0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+000067c0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000067d0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000067e0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+000067f0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+00006800: 3130 3631 2e34 2220 793d 2231 3039 392e  1061.4" y="1099.
+00006810: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00006820: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006830: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006840: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006850: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00006860: 2220 783d 2231 3037 332e 3622 2079 3d22  " x="1073.6" y="
+00006870: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00006880: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
+00006890: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000068a0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000068b0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+000068c0: 3431 3931 6622 2078 3d22 3130 3835 2e38  4191f" x="1085.8
+000068d0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+000068e0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+000068f0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00006900: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00006910: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00006920: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+00006930: 3039 3822 2079 3d22 3130 3939 2e35 2220  098" y="1099.5" 
+00006940: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+00006950: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00006960: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00006970: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00006980: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00006990: 3d22 3131 3130 2e32 2220 793d 2231 3039  ="1110.2" y="109
+000069a0: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000069b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000069c0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000069d0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000069e0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+000069f0: 3166 2220 783d 2231 3132 322e 3422 2079  1f" x="1122.4" y
+00006a00: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
+00006a10: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
+00006a20: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00006a30: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00006a40: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00006a50: 2331 3431 3931 6622 2078 3d22 3131 3334  #14191f" x="1134
+00006a60: 2e36 2220 793d 2231 3039 392e 3522 2077  .6" y="1099.5" w
+00006a70: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00006a80: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00006a90: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00006aa0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00006ab0: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00006ac0: 2231 3134 362e 3822 2079 3d22 3130 3939  "1146.8" y="1099
+00006ad0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+00006ae0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00006af0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00006b00: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00006b10: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+00006b20: 6622 2078 3d22 3131 3539 2220 793d 2231  f" x="1159" y="1
+00006b30: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00006b40: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00006b50: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00006b60: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00006b70: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00006b80: 3139 3166 2220 783d 2231 3137 312e 3222  191f" x="1171.2"
+00006b90: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
+00006ba0: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
+00006bb0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00006bc0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00006bd0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00006be0: 3d22 2331 3431 3931 6622 2078 3d22 3131  ="#14191f" x="11
+00006bf0: 3833 2e34 2220 793d 2231 3039 392e 3522  83.4" y="1099.5"
+00006c00: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00006c10: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00006c20: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00006c30: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00006c40: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00006c50: 783d 2231 3139 352e 3622 2079 3d22 3130  x="1195.6" y="10
+00006c60: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
+00006c70: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00006c80: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00006c90: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00006ca0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00006cb0: 3931 6622 2078 3d22 3132 3037 2e38 2220  91f" x="1207.8" 
+00006cc0: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00006cd0: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00006ce0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00006cf0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00006d00: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00006d10: 2223 3134 3139 3166 2220 783d 2231 3232  "#14191f" x="122
+00006d20: 3022 2079 3d22 3130 3939 2e35 2220 7769  0" y="1099.5" wi
+00006d30: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00006d40: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00006d50: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00006d60: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00006d70: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+00006d80: 3132 3332 2e32 2220 793d 2231 3039 392e  1232.2" y="1099.
+00006d90: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00006da0: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00006db0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00006dc0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00006dd0: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00006de0: 2220 783d 2231 3234 342e 3422 2079 3d22  " x="1244.4" y="
+00006df0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00006e00: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
+00006e10: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00006e20: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00006e30: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+00006e40: 3431 3931 6622 2078 3d22 3132 3536 2e36  4191f" x="1256.6
+00006e50: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00006e60: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00006e70: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00006e80: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00006e90: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00006ea0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+00006eb0: 3236 382e 3822 2079 3d22 3130 3939 2e35  268.8" y="1099.5
+00006ec0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
+00006ed0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00006ee0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00006ef0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00006f00: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00006f10: 2078 3d22 3132 3831 2220 793d 2231 3039   x="1281" y="109
+00006f20: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00006f30: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00006f40: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00006f50: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00006f60: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00006f70: 3166 2220 783d 2231 3239 332e 3222 2079  1f" x="1293.2" y
+00006f80: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
+00006f90: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
+00006fa0: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00006fb0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00006fc0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00006fd0: 2331 3431 3931 6622 2078 3d22 3133 3035  #14191f" x="1305
+00006fe0: 2e34 2220 793d 2231 3039 392e 3522 2077  .4" y="1099.5" w
+00006ff0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00007000: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00007010: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00007020: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00007030: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00007040: 2231 3331 372e 3622 2079 3d22 3130 3939  "1317.6" y="1099
+00007050: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+00007060: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00007070: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00007080: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00007090: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+000070a0: 6622 2078 3d22 3133 3239 2e38 2220 793d  f" x="1329.8" y=
+000070b0: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+000070c0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+000070d0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+000070e0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+000070f0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00007100: 3134 3139 3166 2220 783d 2231 3334 3222  14191f" x="1342"
+00007110: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
+00007120: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
+00007130: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00007140: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00007150: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00007160: 3d22 2331 3431 3931 6622 2078 3d22 3133  ="#14191f" x="13
+00007170: 3534 2e32 2220 793d 2231 3039 392e 3522  54.2" y="1099.5"
+00007180: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00007190: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000071a0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000071b0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000071c0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+000071d0: 783d 2231 3336 362e 3422 2079 3d22 3130  x="1366.4" y="10
+000071e0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
+000071f0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00007200: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00007210: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00007220: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00007230: 3931 6622 2078 3d22 3133 3738 2e36 2220  91f" x="1378.6" 
+00007240: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00007250: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00007260: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00007270: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00007280: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00007290: 2223 3134 3139 3166 2220 783d 2231 3339  "#14191f" x="139
+000072a0: 302e 3822 2079 3d22 3130 3939 2e35 2220  0.8" y="1099.5" 
+000072b0: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+000072c0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+000072d0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+000072e0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+000072f0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00007300: 3d22 3134 3033 2220 793d 2231 3039 392e  ="1403" y="1099.
+00007310: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00007320: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00007330: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00007340: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00007350: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00007360: 2220 783d 2231 3431 352e 3222 2079 3d22  " x="1415.2" y="
+00007370: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00007380: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
+00007390: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+000073a0: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000073b0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+000073c0: 3431 3931 6622 2078 3d22 3134 3237 2e34  4191f" x="1427.4
+000073d0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+000073e0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+000073f0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00007400: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00007410: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00007420: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+00007430: 3433 392e 3622 2079 3d22 3130 3939 2e35  439.6" y="1099.5
+00007440: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
+00007450: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00007460: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00007470: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00007480: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00007490: 2078 3d22 3134 3531 2e38 2220 793d 2231   x="1451.8" y="1
+000074a0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+000074b0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000074c0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000074d0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000074e0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+000074f0: 3139 3166 2220 783d 2231 3436 3422 2079  191f" x="1464" y
+00007500: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
+00007510: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
+00007520: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007530: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007540: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007550: 2331 3431 3931 6622 2078 3d22 3134 3736  #14191f" x="1476
+00007560: 2e32 2220 793d 2231 3039 392e 3522 2077  .2" y="1099.5" w
+00007570: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00007580: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00007590: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+000075a0: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+000075b0: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+000075c0: 2231 3438 382e 3422 2079 3d22 3130 3939  "1488.4" y="1099
+000075d0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+000075e0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+000075f0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00007600: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00007610: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+00007620: 6622 2078 3d22 3135 3030 2e36 2220 793d  f" x="1500.6" y=
+00007630: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00007640: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00007650: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00007660: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00007670: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00007680: 3134 3139 3166 2220 783d 2231 3531 322e  14191f" x="1512.
+00007690: 3822 2079 3d22 3130 3939 2e35 2220 7769  8" y="1099.5" wi
+000076a0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+000076b0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000076c0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000076d0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+000076e0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+000076f0: 3135 3235 2220 793d 2231 3039 392e 3522  1525" y="1099.5"
+00007700: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00007710: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00007720: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00007730: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00007740: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+00007750: 783d 2231 3533 372e 3222 2079 3d22 3130  x="1537.2" y="10
+00007760: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
+00007770: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00007780: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00007790: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+000077a0: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+000077b0: 3931 6622 2078 3d22 3135 3439 2e34 2220  91f" x="1549.4" 
+000077c0: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+000077d0: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+000077e0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000077f0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00007800: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00007810: 2223 3134 3139 3166 2220 783d 2231 3536  "#14191f" x="156
+00007820: 312e 3622 2079 3d22 3130 3939 2e35 2220  1.6" y="1099.5" 
+00007830: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+00007840: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00007850: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00007860: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00007870: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00007880: 3d22 3135 3733 2e38 2220 793d 2231 3039  ="1573.8" y="109
+00007890: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000078a0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000078b0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000078c0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000078d0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+000078e0: 3166 2220 783d 2231 3538 3622 2079 3d22  1f" x="1586" y="
+000078f0: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00007900: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
+00007910: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00007920: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+00007930: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+00007940: 3431 3931 6622 2078 3d22 3135 3938 2e32  4191f" x="1598.2
+00007950: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00007960: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00007970: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00007980: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00007990: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+000079a0: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+000079b0: 3631 302e 3422 2079 3d22 3130 3939 2e35  610.4" y="1099.5
+000079c0: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
+000079d0: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+000079e0: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+000079f0: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00007a00: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00007a10: 2078 3d22 3136 3232 2e36 2220 793d 2231   x="1622.6" y="1
+00007a20: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00007a30: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00007a40: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00007a50: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00007a60: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00007a70: 3139 3166 2220 783d 2231 3633 342e 3822  191f" x="1634.8"
+00007a80: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
+00007a90: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
+00007aa0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00007ab0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00007ac0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00007ad0: 3d22 2331 3431 3931 6622 2078 3d22 3136  ="#14191f" x="16
+00007ae0: 3437 2220 793d 2231 3039 392e 3522 2077  47" y="1099.5" w
+00007af0: 6964 7468 3d22 3132 2e32 2220 6865 6967  idth="12.2" heig
+00007b00: 6874 3d22 3234 2e36 3522 2073 6861 7065  ht="24.65" shape
+00007b10: 2d72 656e 6465 7269 6e67 3d22 6372 6973  -rendering="cris
+00007b20: 7045 6467 6573 222f 3e3c 7265 6374 2066  pEdges"/><rect f
+00007b30: 696c 6c3d 2223 3134 3139 3166 2220 783d  ill="#14191f" x=
+00007b40: 2231 3635 392e 3222 2079 3d22 3130 3939  "1659.2" y="1099
+00007b50: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+00007b60: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+00007b70: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00007b80: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00007b90: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+00007ba0: 6622 2078 3d22 3136 3731 2e34 2220 793d  f" x="1671.4" y=
+00007bb0: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00007bc0: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00007bd0: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00007be0: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00007bf0: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00007c00: 3134 3139 3166 2220 783d 2231 3638 332e  14191f" x="1683.
+00007c10: 3622 2079 3d22 3130 3939 2e35 2220 7769  6" y="1099.5" wi
+00007c20: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+00007c30: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+00007c40: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+00007c50: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+00007c60: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+00007c70: 3136 3935 2e38 2220 793d 2231 3039 392e  1695.8" y="1099.
+00007c80: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00007c90: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00007ca0: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00007cb0: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00007cc0: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00007cd0: 2220 783d 2231 3730 3822 2079 3d22 3130  " x="1708" y="10
+00007ce0: 3939 2e35 2220 7769 6474 683d 2231 322e  99.5" width="12.
+00007cf0: 3222 2068 6569 6768 743d 2232 342e 3635  2" height="24.65
+00007d00: 2220 7368 6170 652d 7265 6e64 6572 696e  " shape-renderin
+00007d10: 673d 2263 7269 7370 4564 6765 7322 2f3e  g="crispEdges"/>
+00007d20: 3c72 6563 7420 6669 6c6c 3d22 2331 3431  <rect fill="#141
+00007d30: 3931 6622 2078 3d22 3137 3230 2e32 2220  91f" x="1720.2" 
+00007d40: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+00007d50: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+00007d60: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00007d70: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00007d80: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00007d90: 2223 3134 3139 3166 2220 783d 2231 3733  "#14191f" x="173
+00007da0: 322e 3422 2079 3d22 3130 3939 2e35 2220  2.4" y="1099.5" 
+00007db0: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+00007dc0: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00007dd0: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00007de0: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00007df0: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00007e00: 3d22 3137 3434 2e36 2220 793d 2231 3039  ="1744.6" y="109
+00007e10: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+00007e20: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00007e30: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00007e40: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00007e50: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+00007e60: 3166 2220 783d 2231 3735 362e 3822 2079  1f" x="1756.8" y
+00007e70: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
+00007e80: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
+00007e90: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00007ea0: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00007eb0: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00007ec0: 2331 3431 3931 6622 2078 3d22 3137 3639  #14191f" x="1769
+00007ed0: 2220 793d 2231 3039 392e 3522 2077 6964  " y="1099.5" wid
+00007ee0: 7468 3d22 3132 2e32 2220 6865 6967 6874  th="12.2" height
+00007ef0: 3d22 3234 2e36 3522 2073 6861 7065 2d72  ="24.65" shape-r
+00007f00: 656e 6465 7269 6e67 3d22 6372 6973 7045  endering="crispE
+00007f10: 6467 6573 222f 3e3c 7265 6374 2066 696c  dges"/><rect fil
+00007f20: 6c3d 2223 3134 3139 3166 2220 783d 2231  l="#14191f" x="1
+00007f30: 3738 312e 3222 2079 3d22 3130 3939 2e35  781.2" y="1099.5
+00007f40: 2220 7769 6474 683d 2231 322e 3222 2068  " width="12.2" h
+00007f50: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00007f60: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00007f70: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00007f80: 7420 6669 6c6c 3d22 2331 3431 3931 6622  t fill="#14191f"
+00007f90: 2078 3d22 3137 3933 2e34 2220 793d 2231   x="1793.4" y="1
+00007fa0: 3039 392e 3522 2077 6964 7468 3d22 3132  099.5" width="12
+00007fb0: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+00007fc0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00007fd0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00007fe0: 3e3c 7265 6374 2066 696c 6c3d 2223 3134  ><rect fill="#14
+00007ff0: 3139 3166 2220 783d 2231 3830 352e 3622  191f" x="1805.6"
+00008000: 2079 3d22 3130 3939 2e35 2220 7769 6474   y="1099.5" widt
+00008010: 683d 2231 322e 3222 2068 6569 6768 743d  h="12.2" height=
+00008020: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00008030: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00008040: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00008050: 3d22 2331 3431 3931 6622 2078 3d22 3138  ="#14191f" x="18
+00008060: 3137 2e38 2220 793d 2231 3039 392e 3522  17.8" y="1099.5"
+00008070: 2077 6964 7468 3d22 3132 2e32 2220 6865   width="12.2" he
+00008080: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+00008090: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+000080a0: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+000080b0: 2066 696c 6c3d 2223 3134 3139 3166 2220   fill="#14191f" 
+000080c0: 783d 2231 3833 3022 2079 3d22 3130 3939  x="1830" y="1099
+000080d0: 2e35 2220 7769 6474 683d 2231 322e 3222  .5" width="12.2"
+000080e0: 2068 6569 6768 743d 2232 342e 3635 2220   height="24.65" 
+000080f0: 7368 6170 652d 7265 6e64 6572 696e 673d  shape-rendering=
+00008100: 2263 7269 7370 4564 6765 7322 2f3e 3c72  "crispEdges"/><r
+00008110: 6563 7420 6669 6c6c 3d22 2331 3431 3931  ect fill="#14191
+00008120: 6622 2078 3d22 3138 3432 2e32 2220 793d  f" x="1842.2" y=
+00008130: 2231 3039 392e 3522 2077 6964 7468 3d22  "1099.5" width="
+00008140: 3132 2e32 2220 6865 6967 6874 3d22 3234  12.2" height="24
+00008150: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00008160: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00008170: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00008180: 3134 3139 3166 2220 783d 2231 3835 342e  14191f" x="1854.
+00008190: 3422 2079 3d22 3130 3939 2e35 2220 7769  4" y="1099.5" wi
+000081a0: 6474 683d 2231 322e 3222 2068 6569 6768  dth="12.2" heigh
+000081b0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000081c0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000081d0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+000081e0: 6c6c 3d22 2331 3431 3931 6622 2078 3d22  ll="#14191f" x="
+000081f0: 3138 3636 2e36 2220 793d 2231 3039 392e  1866.6" y="1099.
+00008200: 3522 2077 6964 7468 3d22 3132 2e32 2220  5" width="12.2" 
+00008210: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00008220: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00008230: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00008240: 6374 2066 696c 6c3d 2223 3134 3139 3166  ct fill="#14191f
+00008250: 2220 783d 2231 3837 382e 3822 2079 3d22  " x="1878.8" y="
+00008260: 3130 3939 2e35 2220 7769 6474 683d 2231  1099.5" width="1
+00008270: 322e 3222 2068 6569 6768 743d 2232 342e  2.2" height="24.
+00008280: 3635 2220 7368 6170 652d 7265 6e64 6572  65" shape-render
+00008290: 696e 673d 2263 7269 7370 4564 6765 7322  ing="crispEdges"
+000082a0: 2f3e 3c72 6563 7420 6669 6c6c 3d22 2331  /><rect fill="#1
+000082b0: 3431 3931 6622 2078 3d22 3138 3931 2220  4191f" x="1891" 
+000082c0: 793d 2231 3039 392e 3522 2077 6964 7468  y="1099.5" width
+000082d0: 3d22 3132 2e32 2220 6865 6967 6874 3d22  ="12.2" height="
+000082e0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+000082f0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00008300: 6573 222f 3e3c 7265 6374 2066 696c 6c3d  es"/><rect fill=
+00008310: 2223 3134 3139 3166 2220 783d 2231 3930  "#14191f" x="190
+00008320: 332e 3222 2079 3d22 3130 3939 2e35 2220  3.2" y="1099.5" 
+00008330: 7769 6474 683d 2231 322e 3222 2068 6569  width="12.2" hei
+00008340: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00008350: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00008360: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00008370: 6669 6c6c 3d22 2331 3431 3931 6622 2078  fill="#14191f" x
+00008380: 3d22 3139 3135 2e34 2220 793d 2231 3039  ="1915.4" y="109
+00008390: 392e 3522 2077 6964 7468 3d22 3132 2e32  9.5" width="12.2
+000083a0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000083b0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000083c0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000083d0: 7265 6374 2066 696c 6c3d 2223 3134 3139  rect fill="#1419
+000083e0: 3166 2220 783d 2231 3932 372e 3622 2079  1f" x="1927.6" y
+000083f0: 3d22 3130 3939 2e35 2220 7769 6474 683d  ="1099.5" width=
+00008400: 2232 342e 3422 2068 6569 6768 743d 2232  "24.4" height="2
+00008410: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00008420: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00008430: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00008440: 2330 3034 3239 3522 2078 3d22 3022 2079  #004295" x="0" y
+00008450: 3d22 3131 3233 2e39 2220 7769 6474 683d  ="1123.9" width=
+00008460: 2231 322e 3222 2068 6569 6768 743d 2232  "12.2" height="2
+00008470: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00008480: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00008490: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+000084a0: 2330 3034 3239 3522 2078 3d22 3132 2e32  #004295" x="12.2
+000084b0: 2220 793d 2231 3132 332e 3922 2077 6964  " y="1123.9" wid
+000084c0: 7468 3d22 3534 3922 2068 6569 6768 743d  th="549" height=
+000084d0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+000084e0: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000084f0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00008500: 3d22 2330 3034 3239 3522 2078 3d22 3536  ="#004295" x="56
+00008510: 312e 3222 2079 3d22 3131 3233 2e39 2220  1.2" y="1123.9" 
+00008520: 7769 6474 683d 2231 3337 382e 3622 2068  width="1378.6" h
+00008530: 6569 6768 743d 2232 342e 3635 2220 7368  eight="24.65" sh
+00008540: 6170 652d 7265 6e64 6572 696e 673d 2263  ape-rendering="c
+00008550: 7269 7370 4564 6765 7322 2f3e 3c72 6563  rispEdges"/><rec
+00008560: 7420 6669 6c6c 3d22 2330 3034 3239 3522  t fill="#004295"
+00008570: 2078 3d22 3139 3339 2e38 2220 793d 2231   x="1939.8" y="1
+00008580: 3132 332e 3922 2077 6964 7468 3d22 3132  123.9" width="12
+00008590: 2e32 2220 6865 6967 6874 3d22 3234 2e36  .2" height="24.6
+000085a0: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000085b0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000085c0: 3e3c 7265 6374 2066 696c 6c3d 2223 3030  ><rect fill="#00
+000085d0: 3533 6161 2220 783d 2230 2220 793d 2231  53aa" x="0" y="1
+000085e0: 3134 382e 3322 2077 6964 7468 3d22 3336  148.3" width="36
+000085f0: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
+00008600: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+00008610: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+00008620: 3e3c 7265 6374 2066 696c 6c3d 2223 3031  ><rect fill="#01
+00008630: 3738 6434 2220 783d 2233 362e 3622 2079  78d4" x="36.6" y
+00008640: 3d22 3131 3438 2e33 2220 7769 6474 683d  ="1148.3" width=
+00008650: 2237 332e 3222 2068 6569 6768 743d 2232  "73.2" height="2
+00008660: 342e 3635 2220 7368 6170 652d 7265 6e64  4.65" shape-rend
+00008670: 6572 696e 673d 2263 7269 7370 4564 6765  ering="crispEdge
+00008680: 7322 2f3e 3c72 6563 7420 6669 6c6c 3d22  s"/><rect fill="
+00008690: 2330 3035 3361 6122 2078 3d22 3130 392e  #0053aa" x="109.
+000086a0: 3822 2079 3d22 3131 3438 2e33 2220 7769  8" y="1148.3" wi
+000086b0: 6474 683d 2233 362e 3622 2068 6569 6768  dth="36.6" heigh
+000086c0: 743d 2232 342e 3635 2220 7368 6170 652d  t="24.65" shape-
+000086d0: 7265 6e64 6572 696e 673d 2263 7269 7370  rendering="crisp
+000086e0: 4564 6765 7322 2f3e 3c72 6563 7420 6669  Edges"/><rect fi
+000086f0: 6c6c 3d22 2330 3137 3864 3422 2078 3d22  ll="#0178d4" x="
+00008700: 3134 362e 3422 2079 3d22 3131 3438 2e33  146.4" y="1148.3
+00008710: 2220 7769 6474 683d 2231 3730 2e38 2220  " width="170.8" 
+00008720: 6865 6967 6874 3d22 3234 2e36 3522 2073  height="24.65" s
+00008730: 6861 7065 2d72 656e 6465 7269 6e67 3d22  hape-rendering="
+00008740: 6372 6973 7045 6467 6573 222f 3e3c 7265  crispEdges"/><re
+00008750: 6374 2066 696c 6c3d 2223 3030 3533 6161  ct fill="#0053aa
+00008760: 2220 783d 2233 3137 2e32 2220 793d 2231  " x="317.2" y="1
+00008770: 3134 382e 3322 2077 6964 7468 3d22 3336  148.3" width="36
+00008780: 2e36 2220 6865 6967 6874 3d22 3234 2e36  .6" height="24.6
+00008790: 3522 2073 6861 7065 2d72 656e 6465 7269  5" shape-renderi
+000087a0: 6e67 3d22 6372 6973 7045 6467 6573 222f  ng="crispEdges"/
+000087b0: 3e3c 7265 6374 2066 696c 6c3d 2223 3031  ><rect fill="#01
+000087c0: 3738 6434 2220 783d 2233 3533 2e38 2220  78d4" x="353.8" 
+000087d0: 793d 2231 3134 382e 3322 2077 6964 7468  y="1148.3" width
+000087e0: 3d22 3137 302e 3822 2068 6569 6768 743d  ="170.8" height=
+000087f0: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00008800: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+00008810: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+00008820: 3d22 2330 3035 3361 6122 2078 3d22 3532  ="#0053aa" x="52
+00008830: 342e 3622 2079 3d22 3131 3438 2e33 2220  4.6" y="1148.3" 
+00008840: 7769 6474 683d 2233 362e 3622 2068 6569  width="36.6" hei
+00008850: 6768 743d 2232 342e 3635 2220 7368 6170  ght="24.65" shap
+00008860: 652d 7265 6e64 6572 696e 673d 2263 7269  e-rendering="cri
+00008870: 7370 4564 6765 7322 2f3e 3c72 6563 7420  spEdges"/><rect 
+00008880: 6669 6c6c 3d22 2330 3137 3864 3422 2078  fill="#0178d4" x
+00008890: 3d22 3536 312e 3222 2079 3d22 3131 3438  ="561.2" y="1148
+000088a0: 2e33 2220 7769 6474 683d 2232 3536 2e32  .3" width="256.2
+000088b0: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+000088c0: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+000088d0: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+000088e0: 7265 6374 2066 696c 6c3d 2223 3030 3533  rect fill="#0053
+000088f0: 6161 2220 783d 2238 3137 2e34 2220 793d  aa" x="817.4" y=
+00008900: 2231 3134 382e 3322 2077 6964 7468 3d22  "1148.3" width="
+00008910: 3336 2e36 2220 6865 6967 6874 3d22 3234  36.6" height="24
+00008920: 2e36 3522 2073 6861 7065 2d72 656e 6465  .65" shape-rende
+00008930: 7269 6e67 3d22 6372 6973 7045 6467 6573  ring="crispEdges
+00008940: 222f 3e3c 7265 6374 2066 696c 6c3d 2223  "/><rect fill="#
+00008950: 3031 3738 6434 2220 783d 2238 3534 2220  0178d4" x="854" 
+00008960: 793d 2231 3134 382e 3322 2077 6964 7468  y="1148.3" width
+00008970: 3d22 3231 392e 3622 2068 6569 6768 743d  ="219.6" height=
+00008980: 2232 342e 3635 2220 7368 6170 652d 7265  "24.65" shape-re
+00008990: 6e64 6572 696e 673d 2263 7269 7370 4564  ndering="crispEd
+000089a0: 6765 7322 2f3e 3c72 6563 7420 6669 6c6c  ges"/><rect fill
+000089b0: 3d22 2330 3035 3361 6122 2078 3d22 3130  ="#0053aa" x="10
+000089c0: 3733 2e36 2220 793d 2231 3134 382e 3322  73.6" y="1148.3"
+000089d0: 2077 6964 7468 3d22 3336 2e36 2220 6865   width="36.6" he
+000089e0: 6967 6874 3d22 3234 2e36 3522 2073 6861  ight="24.65" sha
+000089f0: 7065 2d72 656e 6465 7269 6e67 3d22 6372  pe-rendering="cr
+00008a00: 6973 7045 6467 6573 222f 3e3c 7265 6374  ispEdges"/><rect
+00008a10: 2066 696c 6c3d 2223 3031 3738 6434 2220   fill="#0178d4" 
+00008a20: 783d 2231 3131 302e 3222 2079 3d22 3131  x="1110.2" y="11
+00008a30: 3438 2e33 2220 7769 6474 683d 2231 3833  48.3" width="183
+00008a40: 2220 6865 6967 6874 3d22 3234 2e36 3522  " height="24.65"
+00008a50: 2073 6861 7065 2d72 656e 6465 7269 6e67   shape-rendering
+00008a60: 3d22 6372 6973 7045 6467 6573 222f 3e3c  ="crispEdges"/><
+00008a70: 7265 6374 2066 696c 6c3d 2223 3031 3738  rect fill="#0178
+00008a80: 6434 2220 783d 2231 3239 332e 3222 2079  d4" x="1293.2" y
+00008a90: 3d22 3131 3438 2e33 2220 7769 6474 683d  ="1148.3" width=
+00008aa0: 2236 3538 2e38 2220 6865 6967 6874 3d22  "658.8" height="
+00008ab0: 3234 2e36 3522 2073 6861 7065 2d72 656e  24.65" shape-ren
+00008ac0: 6465 7269 6e67 3d22 6372 6973 7045 6467  dering="crispEdg
+00008ad0: 6573 222f 3e0a 2020 2020 3c67 2063 6c61  es"/>.    <g cla
+00008ae0: 7373 3d22 7465 726d 696e 616c 2d31 3530  ss="terminal-150
+00008af0: 3832 3936 3235 2d6d 6174 7269 7822 3e0a  829625-matrix">.
+00008b00: 2020 2020 3c74 6578 7420 636c 6173 733d      <text class=
+00008b10: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+00008b20: 3632 352d 7232 2220 783d 2231 322e 3222  625-r2" x="12.2"
+00008b30: 2079 3d22 3230 2220 7465 7874 4c65 6e67   y="20" textLeng
+00008b40: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+00008b50: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+00008b60: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
+00008b70: 652d 3029 223e e2ad 983c 2f74 6578 743e  e-0)">...</text>
+00008b80: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+00008b90: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+00008ba0: 7232 2220 783d 2236 3232 2e32 2220 793d  r2" x="622.2" y=
+00008bb0: 2232 3022 2074 6578 744c 656e 6774 683d  "20" textLength=
+00008bc0: 2231 3039 2e38 2220 636c 6970 2d70 6174  "109.8" clip-pat
+00008bd0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+00008be0: 2d31 3530 3832 3936 3235 2d6c 696e 652d  -150829625-line-
+00008bf0: 3029 223e 6272 6f77 7372 2623 3136 303b  0)">browsr&#160;
+00008c00: e280 9426 2331 3630 3b3c 2f74 6578 743e  ...&#160;</text>
+00008c10: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+00008c20: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+00008c30: 7233 2220 783d 2237 3332 2220 793d 2232  r3" x="732" y="2
+00008c40: 3022 2074 6578 744c 656e 6774 683d 2235  0" textLength="5
+00008c50: 3733 2e34 2220 636c 6970 2d70 6174 683d  73.4" clip-path=
+00008c60: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
+00008c70: 3530 3832 3936 3235 2d6c 696e 652d 3029  50829625-line-0)
+00008c80: 223e 6769 7468 7562 3a2f 2f6a 7566 7469  ">github://jufti
+00008c90: 6e3a 6272 6f77 7372 4076 312e 362e 302f  n:browsr@v1.6.0/
+00008ca0: 4c49 4345 4e53 4526 2331 3630 3b5b 6d6f  LICENSE&#160;[mo
+00008cb0: 6e6f 6b61 695d 3c2f 7465 7874 3e3c 7465  nokai]</text><te
+00008cc0: 7874 2063 6c61 7373 3d22 7465 726d 696e  xt class="termin
+00008cd0: 616c 2d31 3530 3832 3936 3235 2d72 3122  al-150829625-r1"
+00008ce0: 2078 3d22 3139 3532 2220 793d 2232 3022   x="1952" y="20"
+00008cf0: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+00008d00: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+00008d10: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+00008d20: 3239 3632 352d 6c69 6e65 2d30 2922 3e0a  29625-line-0)">.
+00008d30: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+00008d40: 7373 3d22 7465 726d 696e 616c 2d31 3530  ss="terminal-150
+00008d50: 3832 3936 3235 2d72 3422 2078 3d22 3022  829625-r4" x="0"
+00008d60: 2079 3d22 3434 2e34 2220 7465 7874 4c65   y="44.4" textLe
+00008d70: 6e67 7468 3d22 3139 3237 2e36 2220 636c  ngth="1927.6" cl
+00008d80: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+00008d90: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
+00008da0: 2d6c 696e 652d 3129 223e 4d49 5426 2331  -line-1)">MIT&#1
+00008db0: 3630 3b4c 6963 656e 7365 2623 3136 303b  60;License&#160;
+00008dc0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008dd0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008de0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008df0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008e00: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008e10: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008e20: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008e30: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008e40: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008e50: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008e60: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008e70: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008e80: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008e90: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008ea0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008eb0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008ec0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008ed0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008ee0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008ef0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008f00: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008f10: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008f20: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008f30: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008f40: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008f50: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008f60: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008f70: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008f80: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008f90: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008fa0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008fb0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008fc0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00008fd0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00008fe0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00008ff0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009000: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009010: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009020: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009030: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009040: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009050: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009060: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009070: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009080: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009090: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+000090a0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+000090b0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+000090c0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+000090d0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+000090e0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+000090f0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009100: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009110: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009120: 2623 3136 303b 2623 3136 303b 3c2f 7465  &#160;&#160;</te
+00009130: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+00009140: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+00009150: 3235 2d72 3122 2078 3d22 3139 3532 2220  25-r1" x="1952" 
+00009160: 793d 2234 342e 3422 2074 6578 744c 656e  y="44.4" textLen
+00009170: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
+00009180: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+00009190: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
+000091a0: 6e65 2d31 2922 3e0a 3c2f 7465 7874 3e3c  ne-1)">.</text><
+000091b0: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+000091c0: 696e 616c 2d31 3530 3832 3936 3235 2d72  inal-150829625-r
+000091d0: 3122 2078 3d22 3139 3532 2220 793d 2236  1" x="1952" y="6
+000091e0: 382e 3822 2074 6578 744c 656e 6774 683d  8.8" textLength=
+000091f0: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+00009200: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+00009210: 3135 3038 3239 3632 352d 6c69 6e65 2d32  150829625-line-2
+00009220: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
+00009230: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+00009240: 2d31 3530 3832 3936 3235 2d72 3422 2078  -150829625-r4" x
+00009250: 3d22 3022 2079 3d22 3933 2e32 2220 7465  ="0" y="93.2" te
+00009260: 7874 4c65 6e67 7468 3d22 3139 3237 2e36  xtLength="1927.6
+00009270: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+00009280: 2823 7465 726d 696e 616c 2d31 3530 3832  (#terminal-15082
+00009290: 3936 3235 2d6c 696e 652d 3329 223e 436f  9625-line-3)">Co
+000092a0: 7079 7269 6768 7426 2331 3630 3b28 6329  pyright&#160;(c)
+000092b0: 2623 3136 303b 3230 3233 2d70 7265 7365  &#160;2023-prese
+000092c0: 6e74 2623 3136 303b 4a75 7374 696e 2623  nt&#160;Justin&#
+000092d0: 3136 303b 466c 616e 6e65 7279 2623 3136  160;Flannery&#16
+000092e0: 303b 266c 743b 6a75 7374 696e 2e66 6c61  0;&lt;justin.fla
+000092f0: 6e6e 6572 7940 6a75 6674 696e 2e63 6f6d  nnery@juftin.com
+00009300: 2667 743b 2623 3136 303b 2623 3136 303b  &gt;&#160;&#160;
+00009310: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009320: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009330: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009340: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009350: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009360: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009370: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009380: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009390: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+000093a0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+000093b0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+000093c0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+000093d0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+000093e0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+000093f0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009400: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009410: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009420: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009430: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009440: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009450: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009460: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009470: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+00009480: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+00009490: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+000094a0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+000094b0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+000094c0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+000094d0: 303b 2623 3136 303b 2623 3136 303b 2623  0;&#160;&#160;&#
+000094e0: 3136 303b 2623 3136 303b 2623 3136 303b  160;&#160;&#160;
+000094f0: 2623 3136 303b 2623 3136 303b 2623 3136  &#160;&#160;&#16
+00009500: 303b 2623 3136 303b 2623 3136 303b 3c2f  0;&#160;&#160;</
+00009510: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+00009520: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+00009530: 3936 3235 2d72 3122 2078 3d22 3139 3532  9625-r1" x="1952
+00009540: 2220 793d 2239 332e 3222 2074 6578 744c  " y="93.2" textL
+00009550: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+00009560: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+00009570: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+00009580: 6c69 6e65 2d33 2922 3e0a 3c2f 7465 7874  line-3)">.</text
+00009590: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+000095a0: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
+000095b0: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+000095c0: 2231 3137 2e36 2220 7465 7874 4c65 6e67  "117.6" textLeng
+000095d0: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+000095e0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+000095f0: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
+00009600: 652d 3429 223e 0a3c 2f74 6578 743e 3c74  e-4)">.</text><t
+00009610: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+00009620: 6e61 6c2d 3135 3038 3239 3632 352d 7234  nal-150829625-r4
+00009630: 2220 783d 2230 2220 793d 2231 3432 2220  " x="0" y="142" 
+00009640: 7465 7874 4c65 6e67 7468 3d22 3139 3237  textLength="1927
+00009650: 2e36 2220 636c 6970 2d70 6174 683d 2275  .6" clip-path="u
+00009660: 726c 2823 7465 726d 696e 616c 2d31 3530  rl(#terminal-150
+00009670: 3832 3936 3235 2d6c 696e 652d 3529 223e  829625-line-5)">
+00009680: 5065 726d 6973 7369 6f6e 2623 3136 303b  Permission&#160;
+00009690: 6973 2623 3136 303b 6865 7265 6279 2623  is&#160;hereby&#
+000096a0: 3136 303b 6772 616e 7465 642c 2623 3136  160;granted,&#16
+000096b0: 303b 6672 6565 2623 3136 303b 6f66 2623  0;free&#160;of&#
+000096c0: 3136 303b 6368 6172 6765 2c26 2331 3630  160;charge,&#160
+000096d0: 3b74 6f26 2331 3630 3b61 6e79 2623 3136  ;to&#160;any&#16
+000096e0: 303b 7065 7273 6f6e 2623 3136 303b 6f62  0;person&#160;ob
+000096f0: 7461 696e 696e 6726 2331 3630 3b61 2623  taining&#160;a&#
+00009700: 3136 303b 636f 7079 2623 3136 303b 6f66  160;copy&#160;of
+00009710: 2623 3136 303b 7468 6973 2623 3136 303b  &#160;this&#160;
+00009720: 736f 6674 7761 7265 2623 3136 303b 616e  software&#160;an
+00009730: 6426 2331 3630 3b61 7373 6f63 6961 7465  d&#160;associate
+00009740: 6426 2331 3630 3b64 6f63 756d 656e 7461  d&#160;documenta
+00009750: 7469 6f6e 2623 3136 303b 6669 6c65 7326  tion&#160;files&
+00009760: 2331 3630 3b28 7468 6526 2331 3630 3b26  #160;(the&#160;&
+00009770: 7175 6f74 3b53 6f66 7477 6172 6526 7175  quot;Software&qu
+00009780: 6f74 3b29 2c26 2331 3630 3b74 6f26 2331  ot;),&#160;to&#1
+00009790: 3630 3b64 6561 6c26 2331 3630 3b69 6e26  60;deal&#160;in&
+000097a0: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+000097b0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+000097c0: 6c2d 3135 3038 3239 3632 352d 7231 2220  l-150829625-r1" 
+000097d0: 783d 2231 3935 3222 2079 3d22 3134 3222  x="1952" y="142"
+000097e0: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+000097f0: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+00009800: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+00009810: 3239 3632 352d 6c69 6e65 2d35 2922 3e0a  29625-line-5)">.
+00009820: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+00009830: 7373 3d22 7465 726d 696e 616c 2d31 3530  ss="terminal-150
+00009840: 3832 3936 3235 2d72 3122 2078 3d22 3139  829625-r1" x="19
+00009850: 3532 2220 793d 2231 3636 2e34 2220 7465  52" y="166.4" te
+00009860: 7874 4c65 6e67 7468 3d22 3132 2e32 2220  xtLength="12.2" 
+00009870: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+00009880: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+00009890: 3235 2d6c 696e 652d 3629 223e 0a3c 2f74  25-line-6)">.</t
+000098a0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+000098b0: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+000098c0: 3632 352d 7234 2220 783d 2230 2220 793d  625-r4" x="0" y=
+000098d0: 2231 3930 2e38 2220 7465 7874 4c65 6e67  "190.8" textLeng
+000098e0: 7468 3d22 3139 3237 2e36 2220 636c 6970  th="1927.6" clip
+000098f0: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+00009900: 696e 616c 2d31 3530 3832 3936 3235 2d6c  inal-150829625-l
+00009910: 696e 652d 3729 223e 5468 6526 2331 3630  ine-7)">The&#160
+00009920: 3b61 626f 7665 2623 3136 303b 636f 7079  ;above&#160;copy
+00009930: 7269 6768 7426 2331 3630 3b6e 6f74 6963  right&#160;notic
+00009940: 6526 2331 3630 3b61 6e64 2623 3136 303b  e&#160;and&#160;
+00009950: 7468 6973 2623 3136 303b 7065 726d 6973  this&#160;permis
+00009960: 7369 6f6e 2623 3136 303b 6e6f 7469 6365  sion&#160;notice
+00009970: 2623 3136 303b 7368 616c 6c26 2331 3630  &#160;shall&#160
+00009980: 3b62 6526 2331 3630 3b69 6e63 6c75 6465  ;be&#160;include
+00009990: 6426 2331 3630 3b69 6e26 2331 3630 3b61  d&#160;in&#160;a
+000099a0: 6c6c 2623 3136 303b 636f 7069 6573 2623  ll&#160;copies&#
+000099b0: 3136 303b 6f72 2623 3136 303b 7375 6273  160;or&#160;subs
+000099c0: 7461 6e74 6961 6c26 2331 3630 3b70 6f72  tantial&#160;por
+000099d0: 7469 6f6e 7326 2331 3630 3b6f 6626 2331  tions&#160;of&#1
+000099e0: 3630 3b74 6865 2623 3136 303b 536f 6674  60;the&#160;Soft
+000099f0: 7761 7265 2e26 2331 3630 3b26 2331 3630  ware.&#160;&#160
+00009a00: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
+00009a10: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
+00009a20: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
+00009a30: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
+00009a40: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
+00009a50: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
+00009a60: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
+00009a70: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
+00009a80: 2331 3630 3b26 2331 3630 3b26 2331 3630  #160;&#160;&#160
+00009a90: 3b26 2331 3630 3b26 2331 3630 3b26 2331  ;&#160;&#160;&#1
+00009aa0: 3630 3b26 2331 3630 3b26 2331 3630 3b26  60;&#160;&#160;&
+00009ab0: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+00009ac0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+00009ad0: 6c2d 3135 3038 3239 3632 352d 7231 2220  l-150829625-r1" 
+00009ae0: 783d 2231 3935 3222 2079 3d22 3139 302e  x="1952" y="190.
+00009af0: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
+00009b00: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+00009b10: 7572 6c28 2374 6572 6d69 6e61 6c2d 3135  url(#terminal-15
+00009b20: 3038 3239 3632 352d 6c69 6e65 2d37 2922  0829625-line-7)"
+00009b30: 3e0a 3c2f 7465 7874 3e3c 7465 7874 2063  >.</text><text c
+00009b40: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
+00009b50: 3530 3832 3936 3235 2d72 3122 2078 3d22  50829625-r1" x="
+00009b60: 3139 3532 2220 793d 2232 3135 2e32 2220  1952" y="215.2" 
+00009b70: 7465 7874 4c65 6e67 7468 3d22 3132 2e32  textLength="12.2
+00009b80: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+00009b90: 2823 7465 726d 696e 616c 2d31 3530 3832  (#terminal-15082
+00009ba0: 3936 3235 2d6c 696e 652d 3829 223e 0a3c  9625-line-8)">.<
+00009bb0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+00009bc0: 733d 2274 6572 6d69 6e61 6c2d 3135 3038  s="terminal-1508
+00009bd0: 3239 3632 352d 7234 2220 783d 2230 2220  29625-r4" x="0" 
+00009be0: 793d 2232 3339 2e36 2220 7465 7874 4c65  y="239.6" textLe
+00009bf0: 6e67 7468 3d22 3139 3237 2e36 2220 636c  ngth="1927.6" cl
+00009c00: 6970 2d70 6174 683d 2275 726c 2823 7465  ip-path="url(#te
+00009c10: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
+00009c20: 2d6c 696e 652d 3929 223e 5448 4526 2331  -line-9)">THE&#1
+00009c30: 3630 3b53 4f46 5457 4152 4526 2331 3630  60;SOFTWARE&#160
+00009c40: 3b49 5326 2331 3630 3b50 524f 5649 4445  ;IS&#160;PROVIDE
+00009c50: 4426 2331 3630 3b26 7175 6f74 3b41 5326  D&#160;&quot;AS&
+00009c60: 2331 3630 3b49 5326 7175 6f74 3b2c 2623  #160;IS&quot;,&#
+00009c70: 3136 303b 5749 5448 4f55 5426 2331 3630  160;WITHOUT&#160
+00009c80: 3b57 4152 5241 4e54 5926 2331 3630 3b4f  ;WARRANTY&#160;O
+00009c90: 4626 2331 3630 3b41 4e59 2623 3136 303b  F&#160;ANY&#160;
+00009ca0: 4b49 4e44 2c26 2331 3630 3b45 5850 5245  KIND,&#160;EXPRE
+00009cb0: 5353 2623 3136 303b 4f52 2623 3136 303b  SS&#160;OR&#160;
+00009cc0: 494d 504c 4945 442c 2623 3136 303b 494e  IMPLIED,&#160;IN
+00009cd0: 434c 5544 494e 4726 2331 3630 3b42 5554  CLUDING&#160;BUT
+00009ce0: 2623 3136 303b 4e4f 5426 2331 3630 3b4c  &#160;NOT&#160;L
+00009cf0: 494d 4954 4544 2623 3136 303b 544f 2623  IMITED&#160;TO&#
+00009d00: 3136 303b 5448 4526 2331 3630 3b57 4152  160;THE&#160;WAR
+00009d10: 5241 4e54 4945 5326 2331 3630 3b4f 4626  RANTIES&#160;OF&
+00009d20: 2331 3630 3b4d 4552 4348 414e 5441 4249  #160;MERCHANTABI
+00009d30: 4c49 5459 2c26 2331 3630 3b46 4954 4e45  LITY,&#160;FITNE
+00009d40: 5353 2623 3136 303b 464f 3c2f 7465 7874  SS&#160;FO</text
+00009d50: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+00009d60: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
+00009d70: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+00009d80: 2232 3339 2e36 2220 7465 7874 4c65 6e67  "239.6" textLeng
+00009d90: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+00009da0: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+00009db0: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
+00009dc0: 652d 3929 223e 0a3c 2f74 6578 743e 3c74  e-9)">.</text><t
+00009dd0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+00009de0: 6e61 6c2d 3135 3038 3239 3632 352d 7231  nal-150829625-r1
+00009df0: 2220 783d 2231 3935 3222 2079 3d22 3236  " x="1952" y="26
+00009e00: 3422 2074 6578 744c 656e 6774 683d 2231  4" textLength="1
+00009e10: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+00009e20: 7572 6c28 2374 6572 6d69 6e61 6c2d 3135  url(#terminal-15
+00009e30: 3038 3239 3632 352d 6c69 6e65 2d31 3029  0829625-line-10)
+00009e40: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
+00009e50: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+00009e60: 3135 3038 3239 3632 352d 7231 2220 783d  150829625-r1" x=
+00009e70: 2231 3935 3222 2079 3d22 3238 382e 3422  "1952" y="288.4"
+00009e80: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+00009e90: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+00009ea0: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+00009eb0: 3239 3632 352d 6c69 6e65 2d31 3129 223e  29625-line-11)">
+00009ec0: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+00009ed0: 6173 733d 2274 6572 6d69 6e61 6c2d 3135  ass="terminal-15
+00009ee0: 3038 3239 3632 352d 7231 2220 783d 2231  0829625-r1" x="1
+00009ef0: 3935 3222 2079 3d22 3331 322e 3822 2074  952" y="312.8" t
+00009f00: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+00009f10: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+00009f20: 2374 6572 6d69 6e61 6c2d 3135 3038 3239  #terminal-150829
+00009f30: 3632 352d 6c69 6e65 2d31 3229 223e 0a3c  625-line-12)">.<
+00009f40: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+00009f50: 733d 2274 6572 6d69 6e61 6c2d 3135 3038  s="terminal-1508
+00009f60: 3239 3632 352d 7231 2220 783d 2231 3935  29625-r1" x="195
+00009f70: 3222 2079 3d22 3333 372e 3222 2074 6578  2" y="337.2" tex
+00009f80: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+00009f90: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+00009fa0: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+00009fb0: 352d 6c69 6e65 2d31 3329 223e 0a3c 2f74  5-line-13)">.</t
+00009fc0: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+00009fd0: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+00009fe0: 3632 352d 7231 2220 783d 2231 3935 3222  625-r1" x="1952"
+00009ff0: 2079 3d22 3336 312e 3622 2074 6578 744c   y="361.6" textL
+0000a000: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+0000a010: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000a020: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000a030: 6c69 6e65 2d31 3429 223e 0a3c 2f74 6578  line-14)">.</tex
+0000a040: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000a050: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000a060: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
+0000a070: 3d22 3338 3622 2074 6578 744c 656e 6774  ="386" textLengt
+0000a080: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000a090: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000a0a0: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
+0000a0b0: 2d31 3529 223e 0a3c 2f74 6578 743e 3c74  -15)">.</text><t
+0000a0c0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000a0d0: 6e61 6c2d 3135 3038 3239 3632 352d 7231  nal-150829625-r1
+0000a0e0: 2220 783d 2231 3935 3222 2079 3d22 3431  " x="1952" y="41
+0000a0f0: 302e 3422 2074 6578 744c 656e 6774 683d  0.4" textLength=
+0000a100: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000a110: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000a120: 3135 3038 3239 3632 352d 6c69 6e65 2d31  150829625-line-1
+0000a130: 3629 223e 0a3c 2f74 6578 743e 3c74 6578  6)">.</text><tex
+0000a140: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000a150: 6c2d 3135 3038 3239 3632 352d 7231 2220  l-150829625-r1" 
+0000a160: 783d 2231 3935 3222 2079 3d22 3433 342e  x="1952" y="434.
+0000a170: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
+0000a180: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000a190: 7572 6c28 2374 6572 6d69 6e61 6c2d 3135  url(#terminal-15
+0000a1a0: 3038 3239 3632 352d 6c69 6e65 2d31 3729  0829625-line-17)
+0000a1b0: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
+0000a1c0: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000a1d0: 3135 3038 3239 3632 352d 7231 2220 783d  150829625-r1" x=
+0000a1e0: 2231 3935 3222 2079 3d22 3435 392e 3222  "1952" y="459.2"
+0000a1f0: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+0000a200: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+0000a210: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+0000a220: 3239 3632 352d 6c69 6e65 2d31 3829 223e  29625-line-18)">
+0000a230: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000a240: 6173 733d 2274 6572 6d69 6e61 6c2d 3135  ass="terminal-15
+0000a250: 3038 3239 3632 352d 7231 2220 783d 2231  0829625-r1" x="1
+0000a260: 3935 3222 2079 3d22 3438 332e 3622 2074  952" y="483.6" t
+0000a270: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000a280: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000a290: 2374 6572 6d69 6e61 6c2d 3135 3038 3239  #terminal-150829
+0000a2a0: 3632 352d 6c69 6e65 2d31 3929 223e 0a3c  625-line-19)">.<
+0000a2b0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000a2c0: 733d 2274 6572 6d69 6e61 6c2d 3135 3038  s="terminal-1508
+0000a2d0: 3239 3632 352d 7231 2220 783d 2231 3935  29625-r1" x="195
+0000a2e0: 3222 2079 3d22 3530 3822 2074 6578 744c  2" y="508" textL
+0000a2f0: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+0000a300: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000a310: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000a320: 6c69 6e65 2d32 3029 223e 0a3c 2f74 6578  line-20)">.</tex
+0000a330: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000a340: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000a350: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
+0000a360: 3d22 3533 322e 3422 2074 6578 744c 656e  ="532.4" textLen
+0000a370: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
+0000a380: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000a390: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
+0000a3a0: 6e65 2d32 3129 223e 0a3c 2f74 6578 743e  ne-21)">.</text>
+0000a3b0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000a3c0: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000a3d0: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
+0000a3e0: 3535 362e 3822 2074 6578 744c 656e 6774  556.8" textLengt
+0000a3f0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000a400: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000a410: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
+0000a420: 2d32 3229 223e 0a3c 2f74 6578 743e 3c74  -22)">.</text><t
+0000a430: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000a440: 6e61 6c2d 3135 3038 3239 3632 352d 7231  nal-150829625-r1
+0000a450: 2220 783d 2231 3935 3222 2079 3d22 3538  " x="1952" y="58
+0000a460: 312e 3222 2074 6578 744c 656e 6774 683d  1.2" textLength=
+0000a470: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000a480: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000a490: 3135 3038 3239 3632 352d 6c69 6e65 2d32  150829625-line-2
+0000a4a0: 3329 223e 0a3c 2f74 6578 743e 3c74 6578  3)">.</text><tex
+0000a4b0: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000a4c0: 6c2d 3135 3038 3239 3632 352d 7231 2220  l-150829625-r1" 
+0000a4d0: 783d 2231 3935 3222 2079 3d22 3630 352e  x="1952" y="605.
+0000a4e0: 3622 2074 6578 744c 656e 6774 683d 2231  6" textLength="1
+0000a4f0: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000a500: 7572 6c28 2374 6572 6d69 6e61 6c2d 3135  url(#terminal-15
+0000a510: 3038 3239 3632 352d 6c69 6e65 2d32 3429  0829625-line-24)
+0000a520: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
+0000a530: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000a540: 3135 3038 3239 3632 352d 7231 2220 783d  150829625-r1" x=
+0000a550: 2231 3935 3222 2079 3d22 3633 3022 2074  "1952" y="630" t
+0000a560: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000a570: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000a580: 2374 6572 6d69 6e61 6c2d 3135 3038 3239  #terminal-150829
+0000a590: 3632 352d 6c69 6e65 2d32 3529 223e 0a3c  625-line-25)">.<
+0000a5a0: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000a5b0: 733d 2274 6572 6d69 6e61 6c2d 3135 3038  s="terminal-1508
+0000a5c0: 3239 3632 352d 7231 2220 783d 2231 3935  29625-r1" x="195
+0000a5d0: 3222 2079 3d22 3635 342e 3422 2074 6578  2" y="654.4" tex
+0000a5e0: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+0000a5f0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000a600: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000a610: 352d 6c69 6e65 2d32 3629 223e 0a3c 2f74  5-line-26)">.</t
+0000a620: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000a630: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+0000a640: 3632 352d 7231 2220 783d 2231 3935 3222  625-r1" x="1952"
+0000a650: 2079 3d22 3637 382e 3822 2074 6578 744c   y="678.8" textL
+0000a660: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+0000a670: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000a680: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000a690: 6c69 6e65 2d32 3729 223e 0a3c 2f74 6578  line-27)">.</tex
+0000a6a0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000a6b0: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000a6c0: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
+0000a6d0: 3d22 3730 332e 3222 2074 6578 744c 656e  ="703.2" textLen
+0000a6e0: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
+0000a6f0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000a700: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
+0000a710: 6e65 2d32 3829 223e 0a3c 2f74 6578 743e  ne-28)">.</text>
+0000a720: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000a730: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000a740: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
+0000a750: 3732 372e 3622 2074 6578 744c 656e 6774  727.6" textLengt
+0000a760: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000a770: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000a780: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
+0000a790: 2d32 3929 223e 0a3c 2f74 6578 743e 3c74  -29)">.</text><t
+0000a7a0: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000a7b0: 6e61 6c2d 3135 3038 3239 3632 352d 7231  nal-150829625-r1
+0000a7c0: 2220 783d 2231 3935 3222 2079 3d22 3735  " x="1952" y="75
+0000a7d0: 3222 2074 6578 744c 656e 6774 683d 2231  2" textLength="1
+0000a7e0: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000a7f0: 7572 6c28 2374 6572 6d69 6e61 6c2d 3135  url(#terminal-15
+0000a800: 3038 3239 3632 352d 6c69 6e65 2d33 3029  0829625-line-30)
+0000a810: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
+0000a820: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000a830: 3135 3038 3239 3632 352d 7231 2220 783d  150829625-r1" x=
+0000a840: 2231 3935 3222 2079 3d22 3737 362e 3422  "1952" y="776.4"
+0000a850: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+0000a860: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+0000a870: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+0000a880: 3239 3632 352d 6c69 6e65 2d33 3129 223e  29625-line-31)">
+0000a890: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000a8a0: 6173 733d 2274 6572 6d69 6e61 6c2d 3135  ass="terminal-15
+0000a8b0: 3038 3239 3632 352d 7231 2220 783d 2231  0829625-r1" x="1
+0000a8c0: 3935 3222 2079 3d22 3830 302e 3822 2074  952" y="800.8" t
+0000a8d0: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000a8e0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000a8f0: 2374 6572 6d69 6e61 6c2d 3135 3038 3239  #terminal-150829
+0000a900: 3632 352d 6c69 6e65 2d33 3229 223e 0a3c  625-line-32)">.<
+0000a910: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000a920: 733d 2274 6572 6d69 6e61 6c2d 3135 3038  s="terminal-1508
+0000a930: 3239 3632 352d 7231 2220 783d 2231 3935  29625-r1" x="195
+0000a940: 3222 2079 3d22 3832 352e 3222 2074 6578  2" y="825.2" tex
+0000a950: 744c 656e 6774 683d 2231 322e 3222 2063  tLength="12.2" c
+0000a960: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000a970: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000a980: 352d 6c69 6e65 2d33 3329 223e 0a3c 2f74  5-line-33)">.</t
+0000a990: 6578 743e 3c74 6578 7420 636c 6173 733d  ext><text class=
+0000a9a0: 2274 6572 6d69 6e61 6c2d 3135 3038 3239  "terminal-150829
+0000a9b0: 3632 352d 7231 2220 783d 2231 3935 3222  625-r1" x="1952"
+0000a9c0: 2079 3d22 3834 392e 3622 2074 6578 744c   y="849.6" textL
+0000a9d0: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+0000a9e0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000a9f0: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000aa00: 6c69 6e65 2d33 3429 223e 0a3c 2f74 6578  line-34)">.</tex
+0000aa10: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000aa20: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000aa30: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
+0000aa40: 3d22 3837 3422 2074 6578 744c 656e 6774  ="874" textLengt
+0000aa50: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000aa60: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000aa70: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
+0000aa80: 2d33 3529 223e 0a3c 2f74 6578 743e 3c74  -35)">.</text><t
+0000aa90: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000aaa0: 6e61 6c2d 3135 3038 3239 3632 352d 7231  nal-150829625-r1
+0000aab0: 2220 783d 2231 3935 3222 2079 3d22 3839  " x="1952" y="89
+0000aac0: 382e 3422 2074 6578 744c 656e 6774 683d  8.4" textLength=
+0000aad0: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000aae0: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000aaf0: 3135 3038 3239 3632 352d 6c69 6e65 2d33  150829625-line-3
+0000ab00: 3629 223e 0a3c 2f74 6578 743e 3c74 6578  6)">.</text><tex
+0000ab10: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000ab20: 6c2d 3135 3038 3239 3632 352d 7231 2220  l-150829625-r1" 
+0000ab30: 783d 2231 3935 3222 2079 3d22 3932 322e  x="1952" y="922.
+0000ab40: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
+0000ab50: 322e 3222 2063 6c69 702d 7061 7468 3d22  2.2" clip-path="
+0000ab60: 7572 6c28 2374 6572 6d69 6e61 6c2d 3135  url(#terminal-15
+0000ab70: 3038 3239 3632 352d 6c69 6e65 2d33 3729  0829625-line-37)
+0000ab80: 223e 0a3c 2f74 6578 743e 3c74 6578 7420  ">.</text><text 
+0000ab90: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000aba0: 3135 3038 3239 3632 352d 7231 2220 783d  150829625-r1" x=
+0000abb0: 2231 3935 3222 2079 3d22 3934 372e 3222  "1952" y="947.2"
+0000abc0: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+0000abd0: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+0000abe0: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+0000abf0: 3239 3632 352d 6c69 6e65 2d33 3829 223e  29625-line-38)">
+0000ac00: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000ac10: 6173 733d 2274 6572 6d69 6e61 6c2d 3135  ass="terminal-15
+0000ac20: 3038 3239 3632 352d 7231 2220 783d 2231  0829625-r1" x="1
+0000ac30: 3935 3222 2079 3d22 3937 312e 3622 2074  952" y="971.6" t
+0000ac40: 6578 744c 656e 6774 683d 2231 322e 3222  extLength="12.2"
+0000ac50: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000ac60: 2374 6572 6d69 6e61 6c2d 3135 3038 3239  #terminal-150829
+0000ac70: 3632 352d 6c69 6e65 2d33 3929 223e 0a3c  625-line-39)">.<
+0000ac80: 2f74 6578 743e 3c74 6578 7420 636c 6173  /text><text clas
+0000ac90: 733d 2274 6572 6d69 6e61 6c2d 3135 3038  s="terminal-1508
+0000aca0: 3239 3632 352d 7231 2220 783d 2231 3935  29625-r1" x="195
+0000acb0: 3222 2079 3d22 3939 3622 2074 6578 744c  2" y="996" textL
+0000acc0: 656e 6774 683d 2231 322e 3222 2063 6c69  ength="12.2" cli
+0000acd0: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000ace0: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000acf0: 6c69 6e65 2d34 3029 223e 0a3c 2f74 6578  line-40)">.</tex
+0000ad00: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000ad10: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000ad20: 352d 7231 2220 783d 2231 3935 3222 2079  5-r1" x="1952" y
+0000ad30: 3d22 3130 3230 2e34 2220 7465 7874 4c65  ="1020.4" textLe
+0000ad40: 6e67 7468 3d22 3132 2e32 2220 636c 6970  ngth="12.2" clip
+0000ad50: 2d70 6174 683d 2275 726c 2823 7465 726d  -path="url(#term
+0000ad60: 696e 616c 2d31 3530 3832 3936 3235 2d6c  inal-150829625-l
+0000ad70: 696e 652d 3431 2922 3e0a 3c2f 7465 7874  ine-41)">.</text
+0000ad80: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+0000ad90: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
+0000ada0: 2d72 3122 2078 3d22 3139 3532 2220 793d  -r1" x="1952" y=
+0000adb0: 2231 3034 342e 3822 2074 6578 744c 656e  "1044.8" textLen
+0000adc0: 6774 683d 2231 322e 3222 2063 6c69 702d  gth="12.2" clip-
+0000add0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000ade0: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
+0000adf0: 6e65 2d34 3229 223e 0a3c 2f74 6578 743e  ne-42)">.</text>
+0000ae00: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000ae10: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000ae20: 7231 2220 783d 2231 3935 3222 2079 3d22  r1" x="1952" y="
+0000ae30: 3130 3639 2e32 2220 7465 7874 4c65 6e67  1069.2" textLeng
+0000ae40: 7468 3d22 3132 2e32 2220 636c 6970 2d70  th="12.2" clip-p
+0000ae50: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000ae60: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
+0000ae70: 652d 3433 2922 3e0a 3c2f 7465 7874 3e3c  e-43)">.</text><
+0000ae80: 7465 7874 2063 6c61 7373 3d22 7465 726d  text class="term
+0000ae90: 696e 616c 2d31 3530 3832 3936 3235 2d72  inal-150829625-r
+0000aea0: 3122 2078 3d22 3139 3532 2220 793d 2231  1" x="1952" y="1
+0000aeb0: 3039 332e 3622 2074 6578 744c 656e 6774  093.6" textLengt
+0000aec0: 683d 2231 322e 3222 2063 6c69 702d 7061  h="12.2" clip-pa
+0000aed0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000aee0: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
+0000aef0: 2d34 3429 223e 0a3c 2f74 6578 743e 3c74  -44)">.</text><t
+0000af00: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000af10: 6e61 6c2d 3135 3038 3239 3632 352d 7235  nal-150829625-r5
+0000af20: 2220 783d 2236 3538 2e38 2220 793d 2231  " x="658.8" y="1
+0000af30: 3131 3822 2074 6578 744c 656e 6774 683d  118" textLength=
+0000af40: 2231 322e 3222 2063 6c69 702d 7061 7468  "12.2" clip-path
+0000af50: 3d22 7572 6c28 2374 6572 6d69 6e61 6c2d  ="url(#terminal-
+0000af60: 3135 3038 3239 3632 352d 6c69 6e65 2d34  150829625-line-4
+0000af70: 3529 223e e296 8d3c 2f74 6578 743e 3c74  5)">...</text><t
+0000af80: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000af90: 6e61 6c2d 3135 3038 3239 3632 352d 7231  nal-150829625-r1
+0000afa0: 2220 783d 2231 3935 3222 2079 3d22 3131  " x="1952" y="11
+0000afb0: 3138 2220 7465 7874 4c65 6e67 7468 3d22  18" textLength="
+0000afc0: 3132 2e32 2220 636c 6970 2d70 6174 683d  12.2" clip-path=
+0000afd0: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
+0000afe0: 3530 3832 3936 3235 2d6c 696e 652d 3435  50829625-line-45
+0000aff0: 2922 3e0a 3c2f 7465 7874 3e3c 7465 7874  )">.</text><text
+0000b000: 2063 6c61 7373 3d22 7465 726d 696e 616c   class="terminal
+0000b010: 2d31 3530 3832 3936 3235 2d72 3622 2078  -150829625-r6" x
+0000b020: 3d22 3132 2e32 2220 793d 2231 3134 322e  ="12.2" y="1142.
+0000b030: 3422 2074 6578 744c 656e 6774 683d 2235  4" textLength="5
+0000b040: 3631 2e32 2220 636c 6970 2d70 6174 683d  61.2" clip-path=
+0000b050: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
+0000b060: 3530 3832 3936 3235 2d6c 696e 652d 3436  50829625-line-46
+0000b070: 2922 3ef0 9f97 84ef b88f efb8 8fef b88f  )">.............
+0000b080: 2623 3136 303b 2623 3136 303b 314b 4226  &#160;&#160;1KB&
+0000b090: 2331 3630 3b26 2331 3630 3bf0 9f92 be26  #160;&#160;....&
+0000b0a0: 2331 3630 3b26 2331 3630 3b4c 4943 454e  #160;&#160;LICEN
+0000b0b0: 5345 2623 3136 303b 2623 3136 303b f09f  SE&#160;&#160;..
+0000b0c0: 9382 2623 3136 303b 2623 3136 303b 6a75  ..&#160;&#160;ju
+0000b0d0: 6674 696e 3a62 726f 7773 7240 7631 2e36  ftin:browsr@v1.6
+0000b0e0: 2e30 3c2f 7465 7874 3e3c 7465 7874 2063  .0</text><text c
+0000b0f0: 6c61 7373 3d22 7465 726d 696e 616c 2d31  lass="terminal-1
+0000b100: 3530 3832 3936 3235 2d72 3122 2078 3d22  50829625-r1" x="
+0000b110: 3139 3532 2220 793d 2231 3134 322e 3422  1952" y="1142.4"
+0000b120: 2074 6578 744c 656e 6774 683d 2231 322e   textLength="12.
+0000b130: 3222 2063 6c69 702d 7061 7468 3d22 7572  2" clip-path="ur
+0000b140: 6c28 2374 6572 6d69 6e61 6c2d 3135 3038  l(#terminal-1508
+0000b150: 3239 3632 352d 6c69 6e65 2d34 3629 223e  29625-line-46)">
+0000b160: 0a3c 2f74 6578 743e 3c74 6578 7420 636c  .</text><text cl
+0000b170: 6173 733d 2274 6572 6d69 6e61 6c2d 3135  ass="terminal-15
+0000b180: 3038 3239 3632 352d 7237 2220 783d 2230  0829625-r7" x="0
+0000b190: 2220 793d 2231 3136 362e 3822 2074 6578  " y="1166.8" tex
+0000b1a0: 744c 656e 6774 683d 2233 362e 3622 2063  tLength="36.6" c
+0000b1b0: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000b1c0: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000b1d0: 352d 6c69 6e65 2d34 3729 223e 2623 3136  5-line-47)">&#16
+0000b1e0: 303b 5126 2331 3630 3b3c 2f74 6578 743e  0;Q&#160;</text>
+0000b1f0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000b200: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000b210: 7238 2220 783d 2233 362e 3622 2079 3d22  r8" x="36.6" y="
+0000b220: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
+0000b230: 7468 3d22 3733 2e32 2220 636c 6970 2d70  th="73.2" clip-p
+0000b240: 6174 683d 2275 726c 2823 7465 726d 696e  ath="url(#termin
+0000b250: 616c 2d31 3530 3832 3936 3235 2d6c 696e  al-150829625-lin
+0000b260: 652d 3437 2922 3e26 2331 3630 3b51 7569  e-47)">&#160;Qui
+0000b270: 7426 2331 3630 3b3c 2f74 6578 743e 3c74  t&#160;</text><t
+0000b280: 6578 7420 636c 6173 733d 2274 6572 6d69  ext class="termi
+0000b290: 6e61 6c2d 3135 3038 3239 3632 352d 7237  nal-150829625-r7
+0000b2a0: 2220 783d 2231 3039 2e38 2220 793d 2231  " x="109.8" y="1
+0000b2b0: 3136 362e 3822 2074 6578 744c 656e 6774  166.8" textLengt
+0000b2c0: 683d 2233 362e 3622 2063 6c69 702d 7061  h="36.6" clip-pa
+0000b2d0: 7468 3d22 7572 6c28 2374 6572 6d69 6e61  th="url(#termina
+0000b2e0: 6c2d 3135 3038 3239 3632 352d 6c69 6e65  l-150829625-line
+0000b2f0: 2d34 3729 223e 2623 3136 303b 4626 2331  -47)">&#160;F&#1
+0000b300: 3630 3b3c 2f74 6578 743e 3c74 6578 7420  60;</text><text 
+0000b310: 636c 6173 733d 2274 6572 6d69 6e61 6c2d  class="terminal-
+0000b320: 3135 3038 3239 3632 352d 7238 2220 783d  150829625-r8" x=
+0000b330: 2231 3436 2e34 2220 793d 2231 3136 362e  "146.4" y="1166.
+0000b340: 3822 2074 6578 744c 656e 6774 683d 2231  8" textLength="1
+0000b350: 3730 2e38 2220 636c 6970 2d70 6174 683d  70.8" clip-path=
+0000b360: 2275 726c 2823 7465 726d 696e 616c 2d31  "url(#terminal-1
+0000b370: 3530 3832 3936 3235 2d6c 696e 652d 3437  50829625-line-47
+0000b380: 2922 3e26 2331 3630 3b54 6f67 676c 6526  )">&#160;Toggle&
+0000b390: 2331 3630 3b46 696c 6573 2623 3136 303b  #160;Files&#160;
+0000b3a0: 3c2f 7465 7874 3e3c 7465 7874 2063 6c61  </text><text cla
+0000b3b0: 7373 3d22 7465 726d 696e 616c 2d31 3530  ss="terminal-150
+0000b3c0: 3832 3936 3235 2d72 3722 2078 3d22 3331  829625-r7" x="31
+0000b3d0: 372e 3222 2079 3d22 3131 3636 2e38 2220  7.2" y="1166.8" 
+0000b3e0: 7465 7874 4c65 6e67 7468 3d22 3336 2e36  textLength="36.6
+0000b3f0: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+0000b400: 2823 7465 726d 696e 616c 2d31 3530 3832  (#terminal-15082
+0000b410: 3936 3235 2d6c 696e 652d 3437 2922 3e26  9625-line-47)">&
+0000b420: 2331 3630 3b54 2623 3136 303b 3c2f 7465  #160;T&#160;</te
+0000b430: 7874 3e3c 7465 7874 2063 6c61 7373 3d22  xt><text class="
+0000b440: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+0000b450: 3235 2d72 3822 2078 3d22 3335 332e 3822  25-r8" x="353.8"
+0000b460: 2079 3d22 3131 3636 2e38 2220 7465 7874   y="1166.8" text
+0000b470: 4c65 6e67 7468 3d22 3137 302e 3822 2063  Length="170.8" c
+0000b480: 6c69 702d 7061 7468 3d22 7572 6c28 2374  lip-path="url(#t
+0000b490: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000b4a0: 352d 6c69 6e65 2d34 3729 223e 2623 3136  5-line-47)">&#16
+0000b4b0: 303b 546f 6767 6c65 2623 3136 303b 5468  0;Toggle&#160;Th
+0000b4c0: 656d 6526 2331 3630 3b3c 2f74 6578 743e  eme&#160;</text>
+0000b4d0: 3c74 6578 7420 636c 6173 733d 2274 6572  <text class="ter
+0000b4e0: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000b4f0: 7237 2220 783d 2235 3234 2e36 2220 793d  r7" x="524.6" y=
+0000b500: 2231 3136 362e 3822 2074 6578 744c 656e  "1166.8" textLen
+0000b510: 6774 683d 2233 362e 3622 2063 6c69 702d  gth="36.6" clip-
+0000b520: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000b530: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
+0000b540: 6e65 2d34 3729 223e 2623 3136 303b 4e26  ne-47)">&#160;N&
+0000b550: 2331 3630 3b3c 2f74 6578 743e 3c74 6578  #160;</text><tex
+0000b560: 7420 636c 6173 733d 2274 6572 6d69 6e61  t class="termina
+0000b570: 6c2d 3135 3038 3239 3632 352d 7238 2220  l-150829625-r8" 
+0000b580: 783d 2235 3631 2e32 2220 793d 2231 3136  x="561.2" y="116
+0000b590: 362e 3822 2074 6578 744c 656e 6774 683d  6.8" textLength=
+0000b5a0: 2232 3536 2e32 2220 636c 6970 2d70 6174  "256.2" clip-pat
+0000b5b0: 683d 2275 726c 2823 7465 726d 696e 616c  h="url(#terminal
+0000b5c0: 2d31 3530 3832 3936 3235 2d6c 696e 652d  -150829625-line-
+0000b5d0: 3437 2922 3e26 2331 3630 3b54 6f67 676c  47)">&#160;Toggl
+0000b5e0: 6526 2331 3630 3b4c 696e 6526 2331 3630  e&#160;Line&#160
+0000b5f0: 3b4e 756d 6265 7273 2623 3136 303b 3c2f  ;Numbers&#160;</
+0000b600: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000b610: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+0000b620: 3936 3235 2d72 3722 2078 3d22 3831 372e  9625-r7" x="817.
+0000b630: 3422 2079 3d22 3131 3636 2e38 2220 7465  4" y="1166.8" te
+0000b640: 7874 4c65 6e67 7468 3d22 3336 2e36 2220  xtLength="36.6" 
+0000b650: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
+0000b660: 7465 726d 696e 616c 2d31 3530 3832 3936  terminal-1508296
+0000b670: 3235 2d6c 696e 652d 3437 2922 3e26 2331  25-line-47)">&#1
+0000b680: 3630 3b44 2623 3136 303b 3c2f 7465 7874  60;D&#160;</text
+0000b690: 3e3c 7465 7874 2063 6c61 7373 3d22 7465  ><text class="te
+0000b6a0: 726d 696e 616c 2d31 3530 3832 3936 3235  rminal-150829625
+0000b6b0: 2d72 3822 2078 3d22 3835 3422 2079 3d22  -r8" x="854" y="
+0000b6c0: 3131 3636 2e38 2220 7465 7874 4c65 6e67  1166.8" textLeng
+0000b6d0: 7468 3d22 3231 392e 3622 2063 6c69 702d  th="219.6" clip-
+0000b6e0: 7061 7468 3d22 7572 6c28 2374 6572 6d69  path="url(#termi
+0000b6f0: 6e61 6c2d 3135 3038 3239 3632 352d 6c69  nal-150829625-li
+0000b700: 6e65 2d34 3729 223e 2623 3136 303b 546f  ne-47)">&#160;To
+0000b710: 6767 6c65 2623 3136 303b 4461 726b 2623  ggle&#160;Dark&#
+0000b720: 3136 303b 4d6f 6465 2623 3136 303b 3c2f  160;Mode&#160;</
+0000b730: 7465 7874 3e3c 7465 7874 2063 6c61 7373  text><text class
+0000b740: 3d22 7465 726d 696e 616c 2d31 3530 3832  ="terminal-15082
+0000b750: 3936 3235 2d72 3722 2078 3d22 3130 3733  9625-r7" x="1073
+0000b760: 2e36 2220 793d 2231 3136 362e 3822 2074  .6" y="1166.8" t
+0000b770: 6578 744c 656e 6774 683d 2233 362e 3622  extLength="36.6"
+0000b780: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
+0000b790: 2374 6572 6d69 6e61 6c2d 3135 3038 3239  #terminal-150829
+0000b7a0: 3632 352d 6c69 6e65 2d34 3729 223e 2623  625-line-47)">&#
+0000b7b0: 3136 303b 5826 2331 3630 3b3c 2f74 6578  160;X&#160;</tex
+0000b7c0: 743e 3c74 6578 7420 636c 6173 733d 2274  t><text class="t
+0000b7d0: 6572 6d69 6e61 6c2d 3135 3038 3239 3632  erminal-15082962
+0000b7e0: 352d 7238 2220 783d 2231 3131 302e 3222  5-r8" x="1110.2"
+0000b7f0: 2079 3d22 3131 3636 2e38 2220 7465 7874   y="1166.8" text
+0000b800: 4c65 6e67 7468 3d22 3138 3322 2063 6c69  Length="183" cli
+0000b810: 702d 7061 7468 3d22 7572 6c28 2374 6572  p-path="url(#ter
+0000b820: 6d69 6e61 6c2d 3135 3038 3239 3632 352d  minal-150829625-
+0000b830: 6c69 6e65 2d34 3729 223e 2623 3136 303b  line-47)">&#160;
+0000b840: 446f 776e 6c6f 6164 2623 3136 303b 4669  Download&#160;Fi
+0000b850: 6c65 2623 3136 303b 3c2f 7465 7874 3e0a  le&#160;</text>.
+0000b860: 2020 2020 3c2f 673e 0a20 2020 203c 2f67      </g>.    </g
+0000b870: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
```

### Comparing `browsr-1.8.0/.gitignore` & `browsr-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/LICENSE` & `browsr-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/README.md` & `browsr-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `browsr-1.8.0/pyproject.toml` & `browsr-1.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "art~=5.7",
   "click~=8.1.3",
   "fsspec~=2023.1.0",
   "pandas~=1.5.2",
   "rich~=13.3.5",
   "rich-click~=1.5.2",
   "rich-pixels~=2.1.1",
-  "textual~=0.24.1",
+  "textual~=0.25.0",
   "universal-pathlib~=0.0.21",
   "Pillow>=9.1.0",
   "PyMuPDF~=1.22.3"
 ]
 description = "TUI File Browser App"
 dynamic = ["version"]
 keywords = []
@@ -84,15 +84,15 @@
   "mkdocs-literate-nav~=0.6.0",
   "mkdocs-section-index~=0.3.5",
   "black~=23.3.0",
   "ruff~=0.0.261",
   "mypy~=1.2.0",
   "pandas-stubs~=2.0.0.230412",
   "pip-tools~=6.13.0",
-  "textual[dev]~=0.24.1"
+  "textual[dev]~=0.25.0"
 ]
 features = ["all"]
 pre-install-commands = ["pip install -U --no-deps -r requirements/requirements-dev.txt"]
 python = "3.10"
 
 [tool.hatch.envs.default.env-vars]
 GITHUB_TOKEN = "{env:GITHUB_TOKEN:placeholder}"
```

### Comparing `browsr-1.8.0/PKG-INFO` & `browsr-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.8.0
+Version: 1.9.0
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Requires-Dist: fsspec~=2023.1.0
 Requires-Dist: pandas~=1.5.2
 Requires-Dist: pillow>=9.1.0
 Requires-Dist: pymupdf~=1.22.3
 Requires-Dist: rich-click~=1.5.2
 Requires-Dist: rich-pixels~=2.1.1
 Requires-Dist: rich~=13.3.5
-Requires-Dist: textual~=0.24.1
+Requires-Dist: textual~=0.25.0
 Requires-Dist: universal-pathlib~=0.0.21
 Provides-Extra: all
 Requires-Dist: adlfs~=2023.1.0; extra == 'all'
 Requires-Dist: aiohttp~=3.8.3; extra == 'all'
 Requires-Dist: gcsfs~=2023.1.0; extra == 'all'
 Requires-Dist: pyarrow~=10.0.0; extra == 'all'
 Requires-Dist: requests~=2.28.2; extra == 'all'
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.8.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.9.0 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: <4.0,>=3.8
 Requires-Dist: art~=5.7 Requires-Dist: click~=8.1.3 Requires-Dist:
 fsspec~=2023.1.0 Requires-Dist: pandas~=1.5.2 Requires-Dist: pillow>=9.1.0
 Requires-Dist: pymupdf~=1.22.3 Requires-Dist: rich-click~=1.5.2 Requires-Dist:
-rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.24.1
+rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.25.0
 Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all Requires-Dist:
 adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3; extra == 'all'
 Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist: pyarrow~=10.0.0;
 extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all' Requires-Dist:
 s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-Dist:
 pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
 adlfs~=2023.1.0; extra == 'remote' Requires-Dist: aiohttp~=3.8.3; extra ==
```

