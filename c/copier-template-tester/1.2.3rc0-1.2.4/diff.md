# Comparing `tmp/copier_template_tester-1.2.3rc0.tar.gz` & `tmp/copier_template_tester-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier_template_tester-1.2.3rc0.tar", max compression
+gzip compressed data, was "copier_template_tester-1.2.4.tar", max compression
```

## Comparing `copier_template_tester-1.2.3rc0.tar` & `copier_template_tester-1.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-17 11:20:16.811483 copier_template_tester-1.2.3rc0/LICENSE
--rw-r--r--   0        0        0      200 2023-05-17 11:24:07.672585 copier_template_tester-1.2.3rc0/copier_template_tester/__init__.py
--rw-r--r--   0        0        0      918 2023-04-27 21:50:31.592600 copier_template_tester-1.2.3rc0/copier_template_tester/_config.py
--rw-r--r--   0        0        0     1201 2023-05-11 23:45:19.757850 copier_template_tester-1.2.3rc0/copier_template_tester/_pre_commit_support.py
--rw-r--r--   0        0        0     4354 2023-05-17 11:19:33.279962 copier_template_tester-1.2.3rc0/copier_template_tester/_write_output.py
--rw-r--r--   0        0        0     2212 2023-05-12 01:59:30.983501 copier_template_tester-1.2.3rc0/copier_template_tester/main.py
--rw-r--r--   0        0        0     3438 2023-05-17 11:24:14.083001 copier_template_tester-1.2.3rc0/docs/README.md
--rw-r--r--   0        0        0     1511 2023-05-17 11:24:07.687798 copier_template_tester-1.2.3rc0/pyproject.toml
--rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 copier_template_tester-1.2.3rc0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-17 11:20:16.811483 copier_template_tester-1.2.4/LICENSE
+-rw-r--r--   0        0        0      197 2023-05-22 22:55:29.631298 copier_template_tester-1.2.4/copier_template_tester/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-27 21:50:31.592600 copier_template_tester-1.2.4/copier_template_tester/_config.py
+-rw-r--r--   0        0        0     1201 2023-05-11 23:45:19.757850 copier_template_tester-1.2.4/copier_template_tester/_pre_commit_support.py
+-rw-r--r--   0        0        0     4613 2023-05-22 22:51:17.412858 copier_template_tester-1.2.4/copier_template_tester/_write_output.py
+-rw-r--r--   0        0        0     2212 2023-05-17 11:34:19.004765 copier_template_tester-1.2.4/copier_template_tester/main.py
+-rw-r--r--   0        0        0     3438 2023-05-22 22:55:35.130704 copier_template_tester-1.2.4/docs/README.md
+-rw-r--r--   0        0        0     1505 2023-05-22 22:55:29.647798 copier_template_tester-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 copier_template_tester-1.2.4/PKG-INFO
```

### Comparing `copier_template_tester-1.2.3rc0/LICENSE` & `copier_template_tester-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.3rc0/copier_template_tester/_config.py` & `copier_template_tester-1.2.4/copier_template_tester/_config.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.3rc0/copier_template_tester/_pre_commit_support.py` & `copier_template_tester-1.2.4/copier_template_tester/_pre_commit_support.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.3rc0/copier_template_tester/_write_output.py` & `copier_template_tester-1.2.4/copier_template_tester/_write_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,24 +64,26 @@
     return Path(output.strip())
 
 
 @beartype
 def _stabilize(line: str, answers_path: Path) -> str:  # noqa: CFQ004
     # Convert _src_path to a deterministic relative path
     if line.startswith('_src_path'):
+        logger.info('Replacing with deterministic value', line=line)
         raw_path = Path(line.split('_src_path:')[-1].strip())
         ans_dir = answers_path.parent
         if ans_dir.is_relative_to(raw_path):
             count_rel = len(ans_dir.relative_to(raw_path).parts)
             rel_path = '/'.join([*(['..'] * count_rel), raw_path.name])
             return f'_src_path: {rel_path}'
         return line
     # Create a stable tag for '_commit' that copier will still utilize
     if line.startswith('_commit'):
-        return f'{line.split("-")[0]}-0'
+        logger.info('Replacing with deterministic value', line=line)
+        return '_commit: HEAD'
     return line
 
 
 @beartype
 def _stabilize_answers_file(*, src_path: Path, dst_path: Path) -> None:  # noqa: CFQ004
     """Ensure that the answers file is deterministic."""
     answers_path = _find_answers_file(src_path=src_path, dst_path=dst_path)
@@ -105,16 +107,19 @@
     kwargs.setdefault('cleanup_on_error', False)
     kwargs.setdefault('data', data or {})
     kwargs.setdefault('defaults', True)
     kwargs.setdefault('overwrite', True)
     kwargs.setdefault('quiet', False)
     kwargs.setdefault('vcs_ref', 'HEAD')
     copier.run_auto(str(src_path), dst_path, **kwargs)
+
+    # Remove any .git directory created by copier script
     git_path = dst_path / '.git'
     if git_path.is_dir():  # pragma: no cover
+        logger.info('Removing git created by copier', git_path=git_path)
         shutil.rmtree(git_path)
 
     # Reduce variability in the output
     try:
         _stabilize_answers_file(src_path=src_path, dst_path=dst_path)
     except FileNotFoundError as exc:  # pragma: no cover
         logger.warning(str(exc))  # noqa: TRY400
```

### Comparing `copier_template_tester-1.2.3rc0/copier_template_tester/main.py` & `copier_template_tester-1.2.4/copier_template_tester/main.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.3rc0/docs/README.md` & `copier_template_tester-1.2.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.2.3rc0/pyproject.toml` & `copier_template_tester-1.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.3rc0"
+version = "1.2.4"
 version_files = ["copier_template_tester/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -20,15 +20,15 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "copier_template_tester"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/copier-template-tester"
-version = "1.2.3rc0"
+version = "1.2.4"
 
 [tool.poetry.dependencies]
 python = "^3.10.5"
 copier = ">=7.0.1"
 corallium = ">=0.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `copier_template_tester-1.2.3rc0/PKG-INFO` & `copier_template_tester-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copier-template-tester
-Version: 1.2.3rc0
+Version: 1.2.4
 Summary: Test copier templates
 Home-page: https://github.com/kyleking/copier-template-tester
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

