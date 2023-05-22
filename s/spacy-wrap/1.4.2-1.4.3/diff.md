# Comparing `tmp/spacy_wrap-1.4.2.tar.gz` & `tmp/spacy_wrap-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_wrap-1.4.2.tar", last modified: Mon May  1 20:30:26 2023, max compression
+gzip compressed data, was "spacy_wrap-1.4.3.tar", last modified: Mon May 22 23:41:08 2023, max compression
```

## Comparing `spacy_wrap-1.4.2.tar` & `spacy_wrap-1.4.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      617 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2842 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      213 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     2879 2023-05-01 20:30:15.000000 spacy_wrap-1.4.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2760 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.614149 spacy_wrap-1.4.2/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     4286 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   289957 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   289957 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     4325 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)     1768 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)      930 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/docs/wrap.pipeline_component.rst
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-01 20:30:15.000000 spacy_wrap-1.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     7395 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.610149 spacy_wrap-1.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/src/spacy_wrap/
--rw-r--r--   0 root         (0) root         (0)      486 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/about.py
--rw-r--r--   0 root         (0) root         (0)     5999 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/architectures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/src/spacy_wrap/layers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/layers/clf_transformer_model.py
--rw-r--r--   0 root         (0) root         (0)    15473 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_seq_clf.py
--rw-r--r--   0 root         (0) root         (0)    20386 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_tok_clf.py
--rw-r--r--   0 root         (0) root         (0)     5022 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/src/spacy_wrap/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2760 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-01 20:30:26.000000 spacy_wrap-1.4.2/src/spacy_wrap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:30:26.618149 spacy_wrap-1.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3480 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/tests/test_seq_clf_transformer.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-05-01 20:30:14.000000 spacy_wrap-1.4.2/tests/test_tok_clf_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.682875 spacy_wrap-1.4.3/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.682875 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      617 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.682875 spacy_wrap-1.4.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      213 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-05-22 23:40:57.000000 spacy_wrap-1.4.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.686876 spacy_wrap-1.4.3/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.686876 spacy_wrap-1.4.3/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   289957 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   289957 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     4325 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      584 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)      930 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/docs/wrap.pipeline_component.rst
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-05-22 23:40:57.000000 spacy_wrap-1.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.678875 spacy_wrap-1.4.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.686876 spacy_wrap-1.4.3/src/spacy_wrap/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/about.py
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/architectures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/src/spacy_wrap/layers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/layers/clf_transformer_model.py
+-rw-r--r--   0 root         (0) root         (0)    15473 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_seq_clf.py
+-rw-r--r--   0 root         (0) root         (0)    20552 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_tok_clf.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/src/spacy_wrap/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      647 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-22 23:41:08.000000 spacy_wrap-1.4.3/src/spacy_wrap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:41:08.690876 spacy_wrap-1.4.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/tests/test_seq_clf_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-05-22 23:40:56.000000 spacy_wrap-1.4.3/tests/test_tok_clf_transformer.py
```

### Comparing `spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/01_bugs.md` & `spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/ISSUE_TEMPLATE/config.yml` & `spacy_wrap-1.4.3/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/dependabot.yml` & `spacy_wrap-1.4.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/workflows/dependabot_automerge.yml` & `spacy_wrap-1.4.3/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/workflows/documentation.yml` & `spacy_wrap-1.4.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/workflows/release.yml` & `spacy_wrap-1.4.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/workflows/stale.yml` & `spacy_wrap-1.4.3/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.github/workflows/tests.yml` & `spacy_wrap-1.4.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/.pre-commit-config.yaml` & `spacy_wrap-1.4.3/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 default_stages: [commit, push]
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
 
   - repo: https://github.com/bwhmather/ssort
     rev: v0.11.6
     hooks:
       - id: ssort
 
   - repo: https://github.com/asottile/add-trailing-comma
     rev: v2.4.0
     hooks:
       - id: add-trailing-comma
 
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.6.4
+    rev: v1.7.1
     hooks:
       - id: docformatter
         args: [--in-place]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         args: [--line-length, "88"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.269
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
```

### Comparing `spacy_wrap-1.4.2/CHANGELOG.md` & `spacy_wrap-1.4.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.4.3 (2023-05-22)
+### Fix
+* Ensure no Nones in iob tokens ([`8fa954a`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/8fa954a70a1cb76ff350b6c32ea461fd85ad369b))
+
 ## v1.4.2 (2023-05-01)
 ### Fix
 * Relaxed upper bound of dev. dependencies ([`f9c8a87`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/f9c8a878ef0d4a03019925bb97af658a4a2bf658))
 
 ### Documentation
 * Update errors in example in readme ([`25063be`](https://github.com/KennethEnevoldsen/spacy-wrap/commit/25063bee591c70ce6b335e46acbef4ea8dea103b))
```

### Comparing `spacy_wrap-1.4.2/LICENSE` & `spacy_wrap-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/PKG-INFO` & `spacy_wrap-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy_wrap
-Version: 1.4.2
+Version: 1.4.3
 Summary: Wrappers for including pre-trained transformers in spaCy pipelines
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spacy_wrap-1.4.2/docs/Makefile` & `spacy_wrap-1.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/_static/favicon.ico` & `spacy_wrap-1.4.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/_static/icon.png` & `spacy_wrap-1.4.3/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/_static/icon_dark.png` & `spacy_wrap-1.4.3/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/conf.py` & `spacy_wrap-1.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/faq.rst` & `spacy_wrap-1.4.3/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/index.rst` & `spacy_wrap-1.4.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/installation.rst` & `spacy_wrap-1.4.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/news.rst` & `spacy_wrap-1.4.3/docs/news.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/docs/wrap.pipeline_component.rst` & `spacy_wrap-1.4.3/docs/wrap.pipeline_component.rst`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/pyproject.toml` & `spacy_wrap-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spacy_wrap"
-version = "1.4.2"
+version = "1.4.3"
 description = "Wrappers for including pre-trained transformers in spaCy pipelines"
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -44,16 +44,16 @@
 style = [
     "black==22.12.0",
     "pre-commit>=2.20.0,<2.21.0",
     "ruff==0.0.263",
     "mypy==0.991"
 ]
 tests = [
-    "pytest>=7.1.3,<7.3.0",
-    "pytest-cov>=3.0.0,<3.0.1",
+    "pytest>=7.1.3",
+    "pytest-cov>=3.0.0",
 ]
 docs = [
     "sphinx>=5.3.0",
     "furo>=2022.12.7",
     "sphinx-copybutton>=0.5.1",
     "sphinxext-opengraph>=0.7.3",
     "sphinx_design>=0.3.0",
```

### Comparing `spacy_wrap-1.4.2/readme.md` & `spacy_wrap-1.4.3/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 ![github coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/KennethEnevoldsen/33fb85a2c440013df494c1fce884633c/raw/3813a0369fdd61b39a806b7b91839ff405ef809a/badge-spacy-wrap-coverage.json)
 
 
 spaCy-wrap is a minimal library intended for wrapping fine-tuned transformers from the [Huggingface model hub](https://huggingface.co/models?pipeline_tag=text-classification&sort=downloads) in your spaCy pipeline allowing the inclusion of existing models within [SpaCy](https://spacy.io) workflows. 
 
 As for as possible it follows a similar API as [spacy-transformers](https://github.com/explosion/spacy-transformers).
 
+**NOTE**: Since the release of spaCy-wrap, Explosion released the [spacy-huggingface-pipelines](https://github.com/explosion/spacy-huggingface-pipelines) it takes the approach of wrapping the Huggingface pipeline as opposed to the transformer. That means token aggregation and conversion into spans happens at
+the Huggingface pipeline, while in spaCy-wrap it happens at the logits of the model which can sometimes lead to unfortunate differences in results.
+I generally recommend using the spacy-huggingface-pipelines for most use cases, but if you need to use the transformer output more directly 
+spaCy-wrap can have its uses.
+
 ## Installation
 
 Installing spacy-wrap is simple using pip:
 
 ```
 pip install spacy_wrap
 ```
```

#### html2text {}

```diff
@@ -14,21 +14,30 @@
 KennethEnevoldsen/33fb85a2c440013df494c1fce884633c/raw/
 3813a0369fdd61b39a806b7b91839ff405ef809a/badge-spacy-wrap-coverage.json) spaCy-
 wrap is a minimal library intended for wrapping fine-tuned transformers from
 the [Huggingface model hub](https://huggingface.co/models?pipeline_tag=text-
 classification&sort=downloads) in your spaCy pipeline allowing the inclusion of
 existing models within [SpaCy](https://spacy.io) workflows. As for as possible
 it follows a similar API as [spacy-transformers](https://github.com/explosion/
-spacy-transformers). ## Installation Installing spacy-wrap is simple using pip:
-``` pip install spacy_wrap ``` ## Examples The following shows a simple example
-of how you can quickly add a fine-tuned transformer model from the Huggingface
-model hub for either [text classification](https://huggingface.co/
-models?pipeline_tag=text-classification&sort=downloads), [named entity](https:/
-/huggingface.co/models?pipeline_tag=token-classification&sort=downloads) or
-[token classification](https://huggingface.co/models?pipeline_tag=token-
+spacy-transformers). **NOTE**: Since the release of spaCy-wrap, Explosion
+released the [spacy-huggingface-pipelines](https://github.com/explosion/spacy-
+huggingface-pipelines) it takes the approach of wrapping the Huggingface
+pipeline as opposed to the transformer. That means token aggregation and
+conversion into spans happens at the Huggingface pipeline, while in spaCy-wrap
+it happens at the logits of the model which can sometimes lead to unfortunate
+differences in results. I generally recommend using the spacy-huggingface-
+pipelines for most use cases, but if you need to use the transformer output
+more directly spaCy-wrap can have its uses. ## Installation Installing spacy-
+wrap is simple using pip: ``` pip install spacy_wrap ``` ## Examples The
+following shows a simple example of how you can quickly add a fine-tuned
+transformer model from the Huggingface model hub for either [text
+classification](https://huggingface.co/models?pipeline_tag=text-
+classification&sort=downloads), [named entity](https://huggingface.co/
+models?pipeline_tag=token-classification&sort=downloads) or [token
+classification](https://huggingface.co/models?pipeline_tag=token-
 classification&sort=downloads). ### Sequence Classification In this example, we
 will use a [model](https://huggingface.co/distilbert-base-uncased-finetuned-
 sst-2-english) fine-tuned for sentiment classification on SST2. This model
 classifies whether a text is positive or negative. We will add this model to a
 blank English pipeline: ```python import spacy import spacy_wrap nlp =
 spacy.blank("en") config = { "doc_extension_trf_data": "clf_trf_data", #
 document extention for the forward pass "doc_extension_prediction":
```

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap/architectures.py` & `spacy_wrap-1.4.3/src/spacy_wrap/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap/layers/clf_transformer_model.py` & `spacy_wrap-1.4.3/src/spacy_wrap/layers/clf_transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_seq_clf.py` & `spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_seq_clf.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap/pipeline_component_tok_clf.py` & `spacy_wrap-1.4.3/src/spacy_wrap/pipeline_component_tok_clf.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,16 @@
             setattr(doc._, self.doc_extension_trf_data, data)
 
             iob_tags, iob_prob = self.convert_to_token_predictions(
                 data,
                 self.aggregation_strategy,
                 self.model_labels,
             )
+            # ensure no Nones (if spacy has a token which does not correspond to any wp)
+            iob_tags = [tag if tag is not None else "O" for tag in iob_tags]
             setattr(doc._, self.doc_extension_prediction, iob_tags)
             setattr(doc._, f"{self.doc_extension_prediction}_prob", iob_prob)
             if "ents" in self.predictions_to:
                 doc = add_iob_tags(doc, iob_tags)
             if "pos" in self.predictions_to:
                 doc = add_pos_tags(doc, iob_tags, extension="pos")
             if "tag" in self.predictions_to:
```

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap/util.py` & `spacy_wrap-1.4.3/src/spacy_wrap/util.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap.egg-info/PKG-INFO` & `spacy_wrap-1.4.3/src/spacy_wrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-wrap
-Version: 1.4.2
+Version: 1.4.3
 Summary: Wrappers for including pre-trained transformers in spaCy pipelines
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap.egg-info/SOURCES.txt` & `spacy_wrap-1.4.3/src/spacy_wrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/src/spacy_wrap.egg-info/requires.txt` & `spacy_wrap-1.4.3/src/spacy_wrap.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -45,9 +45,9 @@
 [style]
 black==22.12.0
 pre-commit<2.21.0,>=2.20.0
 ruff==0.0.263
 mypy==0.991
 
 [tests]
-pytest<7.3.0,>=7.1.3
-pytest-cov<3.0.1,>=3.0.0
+pytest>=7.1.3
+pytest-cov>=3.0.0
```

### Comparing `spacy_wrap-1.4.2/tests/test_seq_clf_transformer.py` & `spacy_wrap-1.4.3/tests/test_seq_clf_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy_wrap-1.4.2/tests/test_tok_clf_transformer.py` & `spacy_wrap-1.4.3/tests/test_tok_clf_transformer.py`

 * *Files identical despite different names*

