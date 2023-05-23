# Comparing `tmp/idf_build_apps-1.0.0.dev0.tar.gz` & `tmp/idf_build_apps-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.0.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.0.dev0.tar` & `idf_build_apps-1.0.0.dev1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      351 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.editorconfig
--rw-r--r--   0        0        0      123 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.gitattributes
--rw-r--r--   0        0        0      253 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3707 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.gitignore
--rw-r--r--   0        0        0     1077 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.readthedocs.yml
--rw-r--r--   0        0        0     5226 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/CHANGELOG.md
--rw-r--r--   0        0        0     1834 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/LICENSE
--rw-r--r--   0        0        0     3843 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/README.md
--rw-r--r--   0        0        0       33 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/config_file.md
--rw-r--r--   0        0        0    10368 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/index.rst
--rw-r--r--   0        0        0     3651 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/manifest.md
--rw-r--r--   0        0        0      486 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    23074 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/config.py
--rw-r--r--   0        0        0     2187 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6751 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/log.py
--rw-r--r--   0        0        0    32197 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6144 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5956 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     6577 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/license_header.txt
--rw-r--r--   0        0        0     1874 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/conftest.py
--rw-r--r--   0        0        0     3118 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_build.py
--rw-r--r--   0        0        0    12994 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_manifest.py
--rw-r--r--   0        0        0     2394 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_utils.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev0/setup.py
--rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.editorconfig
+-rw-r--r--   0        0        0      123 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.gitattributes
+-rw-r--r--   0        0        0      253 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3707 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.gitignore
+-rw-r--r--   0        0        0     1077 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/.readthedocs.yml
+-rw-r--r--   0        0        0     4754 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0     1834 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/LICENSE
+-rw-r--r--   0        0        0     3843 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/README.md
+-rw-r--r--   0        0        0       33 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/config_file.md
+-rw-r--r--   0        0        0    10368 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/index.rst
+-rw-r--r--   0        0        0     3651 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/docs/manifest.md
+-rw-r--r--   0        0        0      486 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    26619 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2187 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6087 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/log.py
+-rw-r--r--   0        0        0    32327 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6144 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5956 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     6577 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/license_header.txt
+-rw-r--r--   0        0        0     1874 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/conftest.py
+-rw-r--r--   0        0        0     2864 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_build.py
+-rw-r--r--   0        0        0    14263 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_finder.py
+-rw-r--r--   0        0        0      995 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_manifest.py
+-rw-r--r--   0        0        0     2394 2023-05-23 05:52:55.184327 idf_build_apps-1.0.0.dev1/tests/test_utils.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev1/setup.py
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev1/PKG-INFO
```

### Comparing `idf_build_apps-1.0.0.dev0/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.0.dev1/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.0.dev1/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.0.dev1/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.0.dev1/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.0.dev1/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/.gitignore` & `idf_build_apps-1.0.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/.pre-commit-config.yaml` & `idf_build_apps-1.0.0.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/CHANGELOG.md` & `idf_build_apps-1.0.0.dev1/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,36 +2,31 @@
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased - 1.0.0]
 
 ## Added
 
-- Support keyword `depends_filepatterns` in the manfiest file
+- Support keyword `depends_filepatterns` in the manifest file
 
 ## BREAKING CHANGES
 
-- Renames
-  - Members
-    - `App.requires_components` renamed to `App.depends_components`
-    - `FolderRule.requires_components` renamed to `FolderRule.depends_components`
-    - `Manifest.requires_components()` renamed to `Manifest.depends_components()`
-  - Parameters
-    - `App.build()` parameter `depends_on_components` renamed to `modified_components`
-    - `App.is_modified()` parameter `depends_on_components` renamed to `modified_components`
-    - `find_apps()`  parameter `depends_on_components` renamed to `modified_components`
-    - `find_apps()`  parameter `depends_on_files` renamed to `modified_files`
-    - `build_apps()`  parameter `depends_on_components` renamed to `modified_components`
-    - `build_apps()`  parameter `depends_on_files` renamed to `modified_files`
-  - CLI Options
-    - `--depends-on-components` renamed to `--modified-components`
-    - `--depends-on-files` renamed to `--modified-files`
-- Reorder Parameters
+- Attributes Renamed
+  - `App.requires_components` renamed to `App.depends_components`
+  - `FolderRule.requires_components` renamed to `FolderRule.depends_components`
+- Functions Renamed
+  - `Manifest.requires_components()` renamed to `Manifest.depends_components()`
+- Signatures Changed
+  - `App.build()`
+  - `App.is_modified()`
   - `find_apps()`
   - `build_apps()`
+- CLI Options Renamed
+  - `--depends-on-components` renamed to `--modified-components`
+  - `--depends-on-files` renamed to `--modified-files`
 
 ## [0.6.1] (2023-05-10)
 
 ### Fixed
 
 - Add missing dependency `pyyaml`. It's wrongly removed in 0.6.0.
```

### Comparing `idf_build_apps-1.0.0.dev0/CONTRIBUTING.md` & `idf_build_apps-1.0.0.dev1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/LICENSE` & `idf_build_apps-1.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/README.md` & `idf_build_apps-1.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/Makefile` & `idf_build_apps-1.0.0.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.0.dev1/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.0.dev1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/conf.py` & `idf_build_apps-1.0.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/config_file.md` & `idf_build_apps-1.0.0.dev1/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/find_build.md` & `idf_build_apps-1.0.0.dev1/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/docs/manifest.md` & `idf_build_apps-1.0.0.dev1/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/app.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,27 +33,34 @@
 )
 from .manifest.manifest import (
     FolderRule,
     Manifest,
 )
 from .utils import (
     BuildError,
+    files_matches_patterns,
     find_first_match,
     rmdir,
     subprocess_run,
     to_absolute_path,
     to_list,
 )
 
 try:
     import typing as t
 except ImportError:
     pass
 
 
+class BuildOrNot:
+    YES = 'yes'
+    NO = 'no'
+    UNKNOWN = 'unknown'
+
+
 class App(object):
     TARGET_PLACEHOLDER = '@t'  # replace it with self.target
     WILDCARD_PLACEHOLDER = '@w'  # replace it with the wildcard, usually the sdkconfig
     NAME_PLACEHOLDER = '@n'  # replace it with self.name
     FULL_NAME_PLACEHOLDER = '@f'  # replace it with escaped self.app_dir
     INDEX_PLACEHOLDER = '@i'  # replace it with the build index
     PARALLEL_INDEX_PLACEHOLDER = '@p'  # replace it with the parallel index
@@ -97,14 +104,18 @@
         self.name = os.path.basename(os.path.realpath(app_dir))
         self.sdkconfig_path = sdkconfig_path
         self.config_name = config_name
         self.target = target
         self.check_warnings = check_warnings
         self.preserve = preserve
 
+        # should be built or not
+        self.should_build = BuildOrNot.UNKNOWN
+        self._checked_should_build = False
+
         # Some miscellaneous build properties which are set later, at the build stage
         self.dry_run = False
         self.index = None
         self.verbose = False
         self.parallel_index = 1
         self.parallel_count = 1
 
@@ -387,17 +398,18 @@
             )
 
         return []
 
     @abstractmethod
     def build(
         self,
+        manifest_rootpath=None,  # type: str | None
         modified_components=None,  # type: list[str] | str | None
-        check_component_dependencies=False,  # type: bool
-        is_modified=False,  # type: bool
+        modified_files=None,  # type: list[str] | str | None
+        check_app_dependencies=False,  # type: bool
     ):  # type: (...) -> bool
         pass
 
     def write_size_json(self):
         map_file = find_first_match('*.map', self.build_path)
         if not map_file:
             LOGGER.warning(
@@ -465,14 +477,76 @@
                     continue
 
                 if _app_dir_fullpath in _f_fullpath.parents:
                     return True
 
         return False
 
+    def check_should_build(
+        self,
+        manifest_rootpath,  # type: str
+        check_app_dependencies,  # type: bool
+        modified_components,  # type: list[str] | None
+        modified_files,  # type: list[str] | None
+    ):  # type: (...) -> None
+        if self.should_build != BuildOrNot.UNKNOWN:
+            return
+
+        if not check_app_dependencies:
+            self.should_build = BuildOrNot.YES
+            self._checked_should_build = True
+            return
+
+        if self.is_modified(modified_files):
+            self.should_build = BuildOrNot.YES
+            self._checked_should_build = True
+            return
+
+        # check app dependencies
+        modified_components = to_list(modified_components)
+        modified_files = to_list(modified_files)
+
+        _modified_components = BuildOrNot.UNKNOWN
+        _modified_files = BuildOrNot.UNKNOWN
+
+        # depends components?
+        if check_app_dependencies and modified_components is not None:
+            if set(self.depends_components).intersection(set(modified_components)):
+                LOGGER.debug(
+                    '=> Should be built. %s requires components: %s, modified components %s',
+                    self,
+                    ', '.join(self.depends_components),
+                    ', '.join(modified_components),
+                )
+                _modified_components = BuildOrNot.YES
+            # if not defined dependency, we left it unknown and decide with idf.py reconfigure
+            elif self.depends_components:
+                _modified_components = BuildOrNot.NO
+
+        # or depends file patterns?
+        if check_app_dependencies and modified_files is not None:
+            if files_matches_patterns(modified_files, self.depends_filepatterns, manifest_rootpath):
+                LOGGER.debug(
+                    '=> Should be built. %s depends on file patterns: %s, modified files %s',
+                    self,
+                    ', '.join(self.depends_filepatterns),
+                    ', '.join(modified_files),
+                )
+                _modified_files = BuildOrNot.YES
+            # if not defined dependency, we left it unknown and decide with idf.py reconfigure
+            elif self.depends_filepatterns:
+                _modified_files = BuildOrNot.NO
+
+        if _modified_components == BuildOrNot.YES or _modified_files == BuildOrNot.YES:
+            self.should_build = BuildOrNot.YES
+        elif _modified_components == BuildOrNot.NO or _modified_files == BuildOrNot.NO:
+            self.should_build = BuildOrNot.NO
+
+        self._checked_should_build = True
+
 
 class CMakeApp(App):
     BUILD_SYSTEM = 'cmake'
 
     # If these keys are present in sdkconfig.defaults, they will be extracted and passed to CMake
     SDKCONFIG_TEST_OPTS = [
         'EXCLUDE_COMPONENTS',
@@ -489,18 +563,22 @@
 
     def __init__(self, *args, **kwargs):
         self.cmake_vars = {}
         super(CMakeApp, self).__init__(*args, **kwargs)
 
     def build(
         self,
+        manifest_rootpath=None,  # type: str | None
         modified_components=None,  # type: list[str] | str | None
-        check_component_dependencies=False,  # type: bool
-        is_modified=False,  # type: bool
+        modified_files=None,  # type: list[str] | str | None
+        check_app_dependencies=False,  # type: bool
     ):  # type: (...) -> bool
+        modified_components = to_list(modified_components)
+        modified_files = to_list(modified_files)
+
         LOGGER.debug('=> Preparing...')
         if self.work_dir != self.app_dir:
             if os.path.exists(self.work_dir):
                 LOGGER.debug('==> Work directory %s exists, removing', self.work_dir)
                 if not self.dry_run:
                     shutil.rmtree(self.work_dir)
             LOGGER.debug('==> Copying app from %s to %s', self.app_dir, self.work_dir)
@@ -550,16 +628,23 @@
             '-C',
             self.work_dir,
             '-DIDF_TARGET={}'.format(self.target),
             # set to ";" to disable `default` when no such variable
             '-DSDKCONFIG_DEFAULTS={}'.format(';'.join(self.sdkconfig_files) if self.sdkconfig_files else ';'),
         ]
 
-        modified_components = to_list(modified_components)
-        if modified_components is not None and check_component_dependencies and not is_modified:
+        if not self._checked_should_build:
+            self.check_should_build(
+                manifest_rootpath=manifest_rootpath,
+                modified_components=modified_components,
+                modified_files=modified_files,
+                check_app_dependencies=check_app_dependencies,
+            )
+
+        if modified_components is not None and check_app_dependencies and self.should_build == BuildOrNot.UNKNOWN:
             subprocess_run(
                 common_args + ['reconfigure'],
                 log_terminal=False if self.build_log_path else True,
                 log_fs=log_file,
                 check=True,
                 additional_env_dict=additional_env_dict,
             )
@@ -571,14 +656,20 @@
                 LOGGER.info(
                     '=> Skip building... app %s depends components: %s, while current build modified components: %s',
                     self.app_dir,
                     build_components,
                     modified_components,
                 )
                 return False
+            else:
+                self.should_build = BuildOrNot.YES
+
+        if self.should_build == BuildOrNot.NO:
+            LOGGER.info('=> Skip building...')
+            return False
 
         # idf.py build
         build_args = deepcopy(common_args)
         if self.cmake_vars:
             for key, val in self.cmake_vars.items():
                 build_args.append('-D{}={}'.format(key, val))
             if 'TEST_EXCLUDE_COMPONENTS' in self.cmake_vars and 'TEST_COMPONENTS' not in self.cmake_vars:
```

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/config.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/constants.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/finder.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/finder.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 )
 
 from . import (
     LOGGER,
 )
 from .app import (
     App,
+    BuildOrNot,
     CMakeApp,
 )
 from .utils import (
     config_rules_from_str,
-    files_matches_patterns,
     to_list,
 )
 
 
 def _get_apps_from_path(
     path,  # type: str
     target,  # type: str
@@ -31,47 +31,35 @@
     build_log_path=None,  # type: str | None
     size_json_path=None,  # type: str | None
     check_warnings=False,  # type: bool
     preserve=True,  # type: bool
     manifest_rootpath=None,  # type: str | None
     modified_components=None,  # type: list[str] | str | None
     modified_files=None,  # type: list[str] | str | None,
-    check_component_dependencies=False,  # type: bool
+    check_app_dependencies=False,  # type: bool
     sdkconfig_defaults_str=None,  # type: str | None
 ):  # type: (...) -> list[App]
     modified_components = to_list(modified_components)
     modified_files = to_list(modified_files)
 
     def _validate_app(_app):  # type: (App) -> bool
         if target not in _app.supported_targets:
             LOGGER.debug('=> Skipping. %s only supports targets: %s', _app, ', '.join(_app.supported_targets))
             return False
 
-        if _app.is_modified(modified_files):
-            return True
+        _app.check_should_build(
+            manifest_rootpath=manifest_rootpath,
+            modified_components=modified_components,
+            modified_files=modified_files,
+            check_app_dependencies=check_app_dependencies,
+        )
 
-        if _app.depends_components and check_component_dependencies:
-            if not set(_app.depends_components).intersection(set(modified_components)):
-                LOGGER.debug(
-                    '=> Skipping. %s requires components: %s, but you passed "--modified-components %s"',
-                    _app,
-                    ', '.join(_app.depends_components),
-                    ', '.join(modified_components),
-                )
-                return False
-
-        if _app.depends_filepatterns and check_component_dependencies:
-            if not files_matches_patterns(modified_files, _app.depends_filepatterns, manifest_rootpath):
-                LOGGER.debug(
-                    '=> Skipping. %s depends on file patterns: %s, but you passed "--modified-files %s"',
-                    _app,
-                    ', '.join(_app.depends_filepatterns),
-                    ', '.join(modified_files),
-                )
-                return False
+        # for unknown ones, we keep them to the build stage to judge
+        if _app.should_build == BuildOrNot.NO:
+            return False
 
         return True
 
     if build_system == 'cmake':
         app_cls = CMakeApp
     else:
         raise ValueError('Only Support CMake for now')
```

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/log.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/main.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 
 try:
     import typing as t
 except ImportError:
     pass
 
 
-def _check_components_dependency(
+def _check_app_dependency(
     manifest_rootpath,  # type: str
     modified_components,  # type: list[str] | None
     modified_files,  # type: list[str] | None
     ignore_component_dependencies_file_patterns,  # type: list[str] | None
 ):  # type: (...) -> bool
-    # not check since `--modified-components` is not passed
+    # not check since modified_components and modified_files are not passed
     if modified_components is None and modified_files is None:
         return False
 
-    # not check since `--ignore-component-dependency-file-pattern` is passed and matched
+    # not check since ignore_component_dependencies_file_patterns is passed and matched
     if (
         ignore_component_dependencies_file_patterns
-        and modified_files
+        and modified_files is not None
         and files_matches_patterns(modified_files, ignore_component_dependencies_file_patterns, manifest_rootpath)
     ):
         LOGGER.debug(
             'Skipping check component dependencies for apps since files %s matches patterns: %s',
             ', '.join(modified_files),
             ', '.join(ignore_component_dependencies_file_patterns),
         )
@@ -187,22 +187,22 @@
                     build_dir=build_dir or 'build',
                     config_rules_str=config_rules_str,
                     build_log_path=build_log_path,
                     size_json_path=size_json_path,
                     check_warnings=check_warnings,
                     preserve=preserve,
                     manifest_rootpath=manifest_rootpath,
+                    check_app_dependencies=_check_app_dependency(
+                        manifest_rootpath=manifest_rootpath,
+                        modified_components=modified_components,
+                        modified_files=modified_files,
+                        ignore_component_dependencies_file_patterns=ignore_component_dependencies_file_patterns,
+                    ),
                     modified_components=modified_components,
                     modified_files=modified_files,
-                    check_component_dependencies=_check_components_dependency(
-                        manifest_rootpath,
-                        modified_components,
-                        modified_files,
-                        ignore_component_dependencies_file_patterns,
-                    ),
                     sdkconfig_defaults_str=sdkconfig_defaults,
                 )
             )
     apps.sort()
 
     LOGGER.info('Found %d apps in total', len(apps))
     return apps
@@ -344,19 +344,20 @@
         app.index = index
         app.verbose = build_verbose
 
         LOGGER.info('Building app %s: %s', index, repr(app))
         is_built = False
         try:
             is_built = app.build(
+                manifest_rootpath=manifest_rootpath,
                 modified_components=modified_components,
-                check_component_dependencies=_check_components_dependency(
+                modified_files=modified_files,
+                check_app_dependencies=_check_app_dependency(
                     manifest_rootpath, modified_components, modified_files, ignore_component_dependencies_file_patterns
                 ),
-                is_modified=app.is_modified(modified_files),
             )
         except BuildError as e:
             LOGGER.error(str(e))
             if keep_going:
                 failed_apps.append(app)
                 exit_code = 1
             else:
```

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/idf_build_apps/utils.py` & `idf_build_apps-1.0.0.dev1/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/pyproject.toml` & `idf_build_apps-1.0.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/tests/conftest.py` & `idf_build_apps-1.0.0.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/tests/test_build.py` & `idf_build_apps-1.0.0.dev1/tests/test_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,42 +20,36 @@
         CMakeApp(str(path), 'esp32', work_dir=str(tmpdir / 'test')).build()
 
         captured = capsys.readouterr()
         assert 'Configuring done' in captured.out
         assert 'Project build complete.' in captured.out
 
     @pytest.mark.parametrize(
-        'modified_components, check_component_dependencies, assert_build_done',
+        'modified_components, check_app_dependencies, should_be_built',
         [
             (None, True, True),
             ([], True, False),
             ([], False, True),
             ('fake', True, False),
             ('fake', False, True),
             ('soc', True, True),
             ('soc', False, True),
             (['soc', 'fake'], True, True),
         ],
     )
     def test_build_with_modified_components(
-        self, tmpdir, capsys, modified_components, check_component_dependencies, assert_build_done
+        self, tmpdir, capsys, modified_components, check_app_dependencies, should_be_built
     ):
         path = IDF_PATH / 'examples' / 'get-started' / 'hello_world'
 
-        CMakeApp(str(path), 'esp32', work_dir=str(tmpdir / 'test')).build(
+        is_built = CMakeApp(str(path), 'esp32', work_dir=str(tmpdir / 'test')).build(
             modified_components=modified_components,
-            check_component_dependencies=check_component_dependencies,
+            check_app_dependencies=check_app_dependencies,
         )
-
-        captured = capsys.readouterr()
-        assert 'Configuring done' in captured.out
-        if assert_build_done:
-            assert 'Project build complete.' in captured.out
-        else:
-            assert 'Project build complete.' not in captured.out
+        assert is_built == should_be_built
 
     @pytest.mark.parametrize(
         'modified_files, is_built',
         [
             ('/foo', False),
             (str(IDF_PATH / 'examples' / 'README.md'), False),
             ([str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], False),
@@ -70,16 +64,16 @@
     )
     def test_build_with_modified_files(self, modified_files, is_built):
         test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
 
         app = CMakeApp(test_dir, 'esp32')
         built = app.build(
             modified_components=[],
-            check_component_dependencies=True,
-            is_modified=app.is_modified(modified_files),
+            modified_files=modified_files,
+            check_app_dependencies=True,
         )
 
         assert built == is_built
 
 
 @pytest.mark.skipif(not shutil.which('idf.py'), reason='idf.py not found')
 def test_idf_version_keywords_type():
```

### Comparing `idf_build_apps-1.0.0.dev0/tests/test_finder.py` & `idf_build_apps-1.0.0.dev1/tests/test_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             (None, True),
             ([], False),
             ('fake', False),
             ('soc', True),
             (['soc', 'fake'], True),
         ],
     )
-    def test_with_requires_and_modified_components(self, tmpdir, modified_components, could_find_apps):
+    def test_with_depends_and_modified_components(self, tmpdir, modified_components, could_find_apps):
         test_dir = str(IDF_PATH / 'examples')
         apps = find_apps(test_dir, 'esp32', recursive=True)
         assert apps
 
         yaml_file = tmpdir / 'test.yml'
         yaml_file.write_text(
             f'''
@@ -179,29 +179,30 @@
         )
         if could_find_apps:
             assert filtered_apps == apps
         else:
             assert not filtered_apps
 
     @pytest.mark.parametrize(
-        'modified_files, could_find_apps',
+        'modified_components, modified_files, could_find_apps',
         [
-            ('/foo', True),
-            (str(IDF_PATH / 'examples' / 'README.md'), False),
-            ([str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], True),
+            ([], '/foo', True),
+            ([], str(IDF_PATH / 'examples' / 'README.md'), False),
+            (None, [str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], True),
             (
+                [],
                 [
                     str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
                     str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
                 ],
                 True,
             ),
         ],
     )
-    def test_with_depends_filepatterns(self, tmp_path, modified_files, could_find_apps):
+    def test_with_depends_filepatterns(self, tmp_path, modified_components, modified_files, could_find_apps):
         test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
         apps = find_apps(test_dir, 'esp32', recursive=True)
         assert apps
 
         yaml_file = tmp_path / 'test.yml'
         yaml_file.write_text(
             f'''
@@ -216,14 +217,47 @@
 
         filtered_apps = find_apps(
             test_dir,
             'esp32',
             recursive=True,
             manifest_rootpath=str(IDF_PATH),
             manifest_files=yaml_file,
+            modified_components=modified_components,
+            modified_files=modified_files,
+        )
+        if could_find_apps:
+            assert filtered_apps == apps
+        else:
+            assert not filtered_apps
+
+    @pytest.mark.parametrize(
+        'modified_files, could_find_apps',
+        [
+            (None, True),
+            (str(IDF_PATH / 'examples' / 'README.md'), True),
+            ([str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], True),
+            (
+                [
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
+                ],
+                True,
+            ),
+            ([str(IDF_PATH / 'examples' / 'a.c')], True),
+        ],
+    )
+    def test_with_filepattern_but_calculate_component_later(self, modified_files, could_find_apps):
+        test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
+        apps = find_apps(test_dir, 'esp32', recursive=True)
+        assert apps
+
+        filtered_apps = find_apps(
+            test_dir,
+            'esp32',
+            recursive=True,
             modified_files=modified_files,
         )
         if could_find_apps:
             assert filtered_apps == apps
         else:
             assert not filtered_apps
```

### Comparing `idf_build_apps-1.0.0.dev0/tests/test_manifest.py` & `idf_build_apps-1.0.0.dev1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/tests/test_utils.py` & `idf_build_apps-1.0.0.dev1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0.dev0/setup.py` & `idf_build_apps-1.0.0.dev1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.0.dev0',
+      version='1.0.0.dev1',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.0.dev0/PKG-INFO` & `idf_build_apps-1.0.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.0.dev0
+Version: 1.0.0.dev1
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

