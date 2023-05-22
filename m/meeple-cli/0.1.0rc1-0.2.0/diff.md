# Comparing `tmp/meeple_cli-0.1.0rc1.tar.gz` & `tmp/meeple_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeple_cli-0.1.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "meeple_cli-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meeple_cli-0.1.0rc1.tar` & `meeple_cli-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,60 @@
--rw-r--r--   0        0        0       66 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.flake8
--rw-r--r--   0        0        0     1090 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1279 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      289 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.gitignore
--rw-r--r--   0        0        0      168 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.markdownlint.yaml
--rw-r--r--   0        0        0     1358 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     4915 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/README.md
--rw-r--r--   0        0        0      249 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/codecov.yml
--rw-r--r--   0        0        0     7919 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/docs/changelog.md
--rw-r--r--   0        0        0      837 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/justfile
--rw-r--r--   0        0        0     1014 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/__init__.py
--rw-r--r--   0        0        0      639 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/__init__.py
--rw-r--r--   0        0        0     1915 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/add.py
--rw-r--r--   0        0        0     2584 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/collections.py
--rw-r--r--   0        0        0      948 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/completions.py
--rw-r--r--   0        0        0     1434 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/delete.py
--rw-r--r--   0        0        0     1903 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/drop.py
--rw-r--r--   0        0        0     5726 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/find.py
--rw-r--r--   0        0        0      701 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/hot.py
--rw-r--r--   0        0        0     1604 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/info.py
--rw-r--r--   0        0        0     4072 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/list.py
--rw-r--r--   0        0        0     3464 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/move.py
--rw-r--r--   0        0        0      684 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/new.py
--rw-r--r--   0        0        0     1186 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/open.py
--rw-r--r--   0        0        0     1238 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/rename.py
--rw-r--r--   0        0        0     1233 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/search.py
--rw-r--r--   0        0        0     3917 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/command/stats.py
--rw-r--r--   0        0        0     3652 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/command/update.py
--rw-r--r--   0        0        0     1153 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/root.py
--rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/type/__init__.py
--rw-r--r--   0        0        0      286 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/type/collection.py
--rw-r--r--   0        0        0     4385 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/type/item.py
--rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/__init__.py
--rw-r--r--   0        0        0     1460 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/api_util.py
--rw-r--r--   0        0        0      702 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/cmd_util.py
--rw-r--r--   0        0        0     3255 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/collection_util.py
--rw-r--r--   0        0        0      235 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/completion_util.py
--rw-r--r--   0        0        0     2877 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/data_util.py
--rw-r--r--   0        0        0      927 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/filter_util.py
--rw-r--r--   0        0        0     2298 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/fmt_util.py
--rw-r--r--   0        0        0      617 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/fs_util.py
--rw-r--r--   0        0        0      357 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/input_util.py
--rw-r--r--   0        0        0      945 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/message_util.py
--rw-r--r--   0        0        0     2614 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/sort_util.py
--rw-r--r--   0        0        0     1323 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/table_util.py
--rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      313 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/test_root.py
--rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/__init__.py
--rw-r--r--   0        0        0     1879 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_filter_util.py
--rw-r--r--   0        0        0     2296 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_fmt_util.py
--rw-r--r--   0        0        0     2188 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_fs_util.py
--rw-r--r--   0        0        0     2525 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_sort_util.py
--rw-r--r--   0        0        0     5915 1970-01-01 00:00:00.000000 meeple_cli-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/.flake8
+-rw-r--r--   0        0        0     1090 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1279 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      289 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/.gitignore
+-rw-r--r--   0        0        0      168 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     1358 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5058 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      249 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/codecov.yml
+-rw-r--r--   0        0        0     8970 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/docs/changelog.md
+-rw-r--r--   0        0        0      837 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/justfile
+-rw-r--r--   0        0        0     1014 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/__init__.py
+-rw-r--r--   0        0        0     1915 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/add.py
+-rw-r--r--   0        0        0     2649 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/collections.py
+-rw-r--r--   0        0        0      948 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/completions.py
+-rw-r--r--   0        0        0     2419 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/delete.py
+-rw-r--r--   0        0        0     1903 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/drop.py
+-rw-r--r--   0        0        0     5768 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/find.py
+-rw-r--r--   0        0        0      701 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/hot.py
+-rw-r--r--   0        0        0     4044 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/import_.py
+-rw-r--r--   0        0        0     1604 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/info.py
+-rw-r--r--   0        0        0     4062 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/list_.py
+-rw-r--r--   0        0        0     3464 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/move.py
+-rw-r--r--   0        0        0     1463 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/new.py
+-rw-r--r--   0        0        0     1131 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/open_.py
+-rw-r--r--   0        0        0     1232 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/rename.py
+-rw-r--r--   0        0        0     1233 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/search.py
+-rw-r--r--   0        0        0     3917 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/stats.py
+-rw-r--r--   0        0        0     5070 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/command/update.py
+-rw-r--r--   0        0        0     1143 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/root.py
+-rw-r--r--   0        0        0      186 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/type/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/type/bgg_collection_item.py
+-rw-r--r--   0        0        0     1217 2023-05-22 23:26:36.984406 meeple_cli-0.2.0/src/meeple/type/bgg_user.py
+-rw-r--r--   0        0        0      286 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/type/collection.py
+-rw-r--r--   0        0        0     4748 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/type/item.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/__init__.py
+-rw-r--r--   0        0        0     3415 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/api_util.py
+-rw-r--r--   0        0        0      703 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/cmd_util.py
+-rw-r--r--   0        0        0     3785 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/collection_util.py
+-rw-r--r--   0        0        0      245 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/completion_util.py
+-rw-r--r--   0        0        0     2842 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/data_util.py
+-rw-r--r--   0        0        0      927 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/filter_util.py
+-rw-r--r--   0        0        0     2298 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/fmt_util.py
+-rw-r--r--   0        0        0     1160 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/fs_util.py
+-rw-r--r--   0        0        0      704 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/input_util.py
+-rw-r--r--   0        0        0     1102 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/message_util.py
+-rw-r--r--   0        0        0     2614 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/sort_util.py
+-rw-r--r--   0        0        0     1323 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/src/meeple/util/table_util.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/test_root.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/test_completion_util.py
+-rw-r--r--   0        0        0     1879 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/test_filter_util.py
+-rw-r--r--   0        0        0     2665 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/test_fmt_util.py
+-rw-r--r--   0        0        0     2188 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/test_fs_util.py
+-rw-r--r--   0        0        0      405 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/test_input_util.py
+-rw-r--r--   0        0        0     2525 2023-05-22 23:26:36.988406 meeple_cli-0.2.0/tests/util/test_sort_util.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 meeple_cli-0.2.0/PKG-INFO
```

### Comparing `meeple_cli-0.1.0rc1/.github/workflows/python-publish.yml` & `meeple_cli-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/.github/workflows/python-test.yml` & `meeple_cli-0.2.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/.pre-commit-config.yaml` & `meeple_cli-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/LICENSE` & `meeple_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/README.md` & `meeple_cli-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -49,26 +49,27 @@
 Options:
   -h, --help     Show this message and exit.
   -v, --version  Show the version and exit.
 
 Collection Commands:
   add          Add an item to a collection.
   collections  List all collections.
-  delete       Delete a collection.
+  delete       Delete collections.
   drop         Remove an item from a collection.
   find         Search collections for items.
   list         List contents of a collection.
   move         Move an item from one collection to another.
-  new          Create a new collection.
-  rename       Rename a local collection.
+  new          Create new collections.
+  rename       Rename a collection.
   stats        Print out the details of a collection.
-  update       Update local collection data.
+  update       Update collection data.
 
 BoardGameGeek Commands:
   hot     List current BoardGameGeek trending items.
+  import  Import BoardGameGeek user collections.
   info    Print out the details of an item.
   open    Open an item on BoardGameGeek.
   search  Search BoardGameGeek for items.
 
 Other Commands:
   completions  Setup meeple shell completions.
 ```
@@ -126,19 +127,22 @@
 
 ## FAQ
 
 ### Why local only collections?
 
 Currently, the
 [BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
-provides limited _read-only_ data about user collections/GeekLists.
+provides limited _read-only_ data about user Collections and GeekLists.
 
-While it is _technically_ feasible to interface with GeekLists via
-webscrapers/spiders, this kind of practice would be both complex and also
-violate [BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
+While it is _technically_ feasible to interface with Collections and GeekLists
+via webscrapers or spiders, these approaches would be complex and also violate
+[BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
+
+For now, it is possible to import BGG user collections into `meeple-cli` via
+`meeple import`.
 
 ### Why do some items show a weight of `NA` when boardgamegeek.com has a value?
 
 This is a known and occasionally recurring bug in the BoardGameGeek database. It
 usually resolves itself within a day. For more info or additional support, read
 this [thread](https://boardgamegeek.com/thread/3049286/some-games-show-weight-000).
```

### Comparing `meeple_cli-0.1.0rc1/docs/changelog.md` & `meeple_cli-0.2.0/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,42 @@
 The format is based on
 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/ "Keep a Changelog"),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html "Semantic Versioning").
 
 ## [Unreleased]
 
+## [v0.2.0] - 2023-05-22
+
+### Added
+
+- `meeple import` - Import BoardGameGeek user collections. ([#46](https://github.com/boldandbrad/meeple-cli/issues/46))
+  - Import as either one large collection or as separate collections based on item status.
+  - `--one` - Import as one collection.
+  - `--many` - Import as separate collections by status.
+  - `--dry-run` - Simulate import operations without persisting.
+  - `-v/--verbose` - Output additional details.
+
+### Changed
+
+- `meeple delete` - Delete multiple collections at once. ([#69](https://github.com/boldandbrad/meeple-cli/issues/69))
+- `meeple new` - Create multiple collections at once. ([#70](https://github.com/boldandbrad/meeple-cli/issues/70))
+- `meeple update` - Update multiple specific collections at once. ([#66](https://github.com/boldandbrad/meeple-cli/issues/66))
+
+### Fixed
+
+- `meeple find` - Fix error message collection name formatting.
+- `meeple rename` - Fix help message wording.
+
+## [v0.1.0] - 2023-05-16
+
+### Changed
+
+- `GENERAL` - Code cleanup and increased test coverage.
+
 ## [v0.1.0rc1] - 2023-05-15
 
 ### Added
 
 - `meeple list` - Show warning message when the collection has pending changes.
 - `meeple move`
   - Gracefully handle the re-removal of items slated to be added to the source collection.
```

### Comparing `meeple_cli-0.1.0rc1/justfile` & `meeple_cli-0.2.0/justfile`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/pyproject.toml` & `meeple_cli-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/__init__.py` & `meeple_cli-0.2.0/src/meeple/command/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from .add import add
 from .collections import collections
 from .completions import completions
 from .delete import delete
 from .drop import drop
 from .find import find
 from .hot import hot
+from .import_ import import_
 from .info import info
-from .list import list_collection
+from .list_ import list_
 from .move import move
 from .new import new
-from .open import open_on_bgg
+from .open_ import open_
 from .rename import rename
 from .search import search
 from .stats import stats
 from .update import update
 
 __all__ = (
     add,
     collections,
     completions,
     delete,
     drop,
     find,
     hot,
+    import_,
     info,
-    list_collection,
+    list_,
     move,
     new,
-    open_on_bgg,
+    open_,
     rename,
     search,
     stats,
     update,
 )
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/add.py` & `meeple_cli-0.2.0/src/meeple/command/add.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/collections.py` & `meeple_cli-0.2.0/src/meeple/command/collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
 from meeple.type.collection import Collection
-from meeple.util.collection_util import get_collections, is_pending_updates
+from meeple.util.collection_util import get_collection_names, is_pending_updates
 from meeple.util.data_util import get_collection_data, last_updated
 from meeple.util.fmt_util import fmt_collection_name, fmt_headers
 from meeple.util.message_util import no_collections_exist_error, warn_msg
 from meeple.util.sort_util import COLLECTION_SORT_KEYS, sort_collections
 from meeple.util.table_util import CollectionHeader, print_table
 
 
@@ -17,33 +17,35 @@
     show_default=True,
     help="Sort output by the provided column.",
 )
 @click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
 def collections(sort: str, verbose: bool) -> None:
     """List all collections."""
-    # attempt to retrieve collections
-    collections = get_collections()
+    # attempt to retrieve collection names
+    collection_names = get_collection_names()
 
     # check that local collections exist
-    if not collections:
+    if not collection_names:
         no_collections_exist_error()
 
-    collection_list = []
+    collections = []
     pending_changes = False
-    for collection in collections:
-        board_games, expansions = get_collection_data(collection)
-        collection_list.append(
-            Collection(collection, board_games, expansions, last_updated(collection))
+    for collection_name in collection_names:
+        board_games, expansions = get_collection_data(collection_name)
+        collections.append(
+            Collection(
+                collection_name, board_games, expansions, last_updated(collection_name)
+            )
         )
-        if is_pending_updates(collection):
+        if is_pending_updates(collection_name):
             pending_changes = True
 
     # sort output
-    collection_list, sort_direction = sort_collections(collection_list, sort)
+    collections, sort_direction = sort_collections(collections, sort)
 
     # prepare table data
     headers = [CollectionHeader.NAME]
     if verbose:
         headers.extend(
             [
                 CollectionHeader.BOARDGAMES,
@@ -52,15 +54,15 @@
             ]
         )
 
     # format headers
     headers = fmt_headers(headers, sort, sort_direction)
 
     rows = []
-    for collection in collection_list:
+    for collection in collections:
         cols = [fmt_collection_name(collection.name)]
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
                     str(len(collection.board_games)),
                     str(len(collection.expansions)),
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/completions.py` & `meeple_cli-0.2.0/src/meeple/command/completions.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/drop.py` & `meeple_cli-0.2.0/src/meeple/command/drop.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/find.py` & `meeple_cli-0.2.0/src/meeple/command/find.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
 from meeple.type.collection import Collection
-from meeple.util.collection_util import are_collections, get_collections
+from meeple.util.collection_util import are_collections, get_collection_names
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
 from meeple.util.filter_util import filterby_players, filterby_playtime, filterby_weight
 from meeple.util.fmt_util import (
     fmt_headers,
     fmt_item_type,
     fmt_players,
@@ -69,23 +69,23 @@
     sort: str,
     max_time: int,
     verbose: bool,
     weight: int,
 ) -> None:
     """Search collections for items.
 
-    - COLLECTIONS are the names of a collections to query. [default: all]
+    - COLLECTIONS are names of the collections to query. [default: all]
     """
     # check if provided collections exist
     if not are_collections(collections):
         error_msg("Not all provided collections are valid collections.")
 
     # if no collections provided, default to all local collections
     if not collections:
-        collections = get_collections()
+        collections = get_collection_names()
 
     # check that local collections exist
     if not collections:
         no_collections_exist_error()
 
     # get collection items
     result_items = []
@@ -112,15 +112,15 @@
         result_items = filterby_playtime(result_items, max_time)
     if weight:
         result_items = filterby_weight(result_items, weight)
 
     # check that data exists after applied filters
     if not result_items:
         error_msg(
-            f"No items found matching provided filters for collection(s) [u magenta]{collections}[/u magenta]."
+            f"No items found matching provided filters for collection(s) [u magenta]{'[/u magenta], [u magenta]'.join(collections)}[/u magenta]."
         )
 
     # sort output
     result_items, sort_direction = sort_items(result_items, sort)
 
     # prepare table headers
     headers = [ItemHeader.ID, ItemHeader.NAME]
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/hot.py` & `meeple_cli-0.2.0/src/meeple/command/hot.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/info.py` & `meeple_cli-0.2.0/src/meeple/command/info.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/list.py` & `meeple_cli-0.2.0/src/meeple/command/list_.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     default="rating",
     show_default=True,
     help="Sort output by the provided column.",
 )
 @click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
 # TODO: add option to show grid lines or not in the table
-def list_collection(collection: str, item_type: str, sort: str, verbose: bool) -> None:
+def list_(collection: str, item_type: str, sort: str, verbose: bool) -> None:
     """List contents of a collection.
 
     - COLLECTION is the name of the collection to be listed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
         invalid_collection_error(collection)
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/move.py` & `meeple_cli-0.2.0/src/meeple/command/move.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/new.py` & `meeple_cli-0.2.0/src/meeple/command/new.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,41 @@
+from typing import List
+
 import click
 
 from meeple.util.collection_util import create_collection, is_collection
-from meeple.util.message_util import error_msg, info_msg
+from meeple.util.message_util import error_msg, info_msg, under_msg
 
 
 @click.command()
-@click.argument("collection")
+@click.argument("collections", nargs=-1)
 @click.help_option("-h", "--help")
-def new(collection: str) -> None:
-    """Create a new collection.
+def new(collections: List[str]) -> None:
+    """Create new collections.
 
-    - COLLECTION is the name of the collection to be created.
+    - COLLECTIONS are names of the collections to create.
     """
-    # check that the given collection doesn't already exist
-    if is_collection(collection):
-        error_msg(f"Collection [u magenta]{collection}[/u magenta] already exists.")
-
-    # create new collection
-    create_collection(collection)
-    info_msg(f"Created new collection [u magenta]{collection}[/u magenta].")
+    if len(collections) > 1:
+        info_msg("Creating new collections...")
+        for collection in collections:
+            # check that the given collection doesn't already exist
+            if is_collection(collection):
+                under_msg(
+                    f"[dim]Skipped collection [u magenta]{collection}[/u magenta]. It already exists.[/dim]"
+                )
+            else:
+                # create new collection
+                create_collection(collection)
+                under_msg(
+                    f"Created new collection [u magenta]{collection}[/u magenta]."
+                )
+
+        info_msg("Created new collection(s).")
+    else:
+        collection = collections[0]
+        # check that the given collection doesn't already exist
+        if is_collection(collection):
+            error_msg(f"Collection [u magenta]{collection}[/u magenta] already exists.")
+
+        # create new collection
+        create_collection(collection)
+        info_msg(f"Created new collection [u magenta]{collection}[/u magenta].")
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/open.py` & `meeple_cli-0.2.0/src/meeple/command/open_.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import webbrowser
 
 import click
 
-from meeple.util.api_util import BGG_DOMAIN, get_bgg_items
+from meeple.util.api_util import BGG_DOMAIN, get_bgg_item
 from meeple.util.input_util import bool_input
-from meeple.util.message_util import info_msg, invalid_id_error, print_msg
+from meeple.util.message_util import info_msg, invalid_id_error, under_msg
 
 
 @click.command(name="open")
 @click.argument("id", type=int)
 @click.option("-y", "--yes", is_flag=True, help="Bypass confirmation.")
 @click.help_option("-h", "--help")
-def open_on_bgg(id: int, yes: bool) -> None:
+def open_(id: int, yes: bool) -> None:
     """Open an item on BoardGameGeek.
 
     - ID is the BoardGameGeek ID of the board game/expansion to be opened on boardgamegeek.com.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
-    api_result = get_bgg_items([bgg_id])
-    if not api_result:
+    item = get_bgg_item(bgg_id)
+    if not item:
         invalid_id_error(bgg_id)
 
     # confirm the user wants to open the board game/expansion on BoardGameGeek website
-    item = api_result[0]
     url = f"https://{BGG_DOMAIN}/{item.type}/{bgg_id}"
     name = item.name
     if yes or bool_input(f"Open [i blue]{name}[/i blue] on {BGG_DOMAIN}?"):
-        print_msg(f" ╰╴ Opening [i blue]{name}[/i blue] on {BGG_DOMAIN} ...")
+        under_msg(f"Opening [i blue]{name}[/i blue] on {BGG_DOMAIN} ...")
         webbrowser.open(url)
     else:
         info_msg(f"View [i blue]{name}[/i blue] at {url}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/rename.py` & `meeple_cli-0.2.0/src/meeple/command/rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.argument("new_name")
 @click.help_option("-h", "--help")
 def rename(collection: str, new_name: str) -> None:
-    """Rename a local collection.
+    """Rename a collection.
 
     - COLLECTION is the name of the collection to be renamed.
     - NEW_NAME is the new name to assign to the collection.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
         invalid_collection_error(collection)
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/search.py` & `meeple_cli-0.2.0/src/meeple/command/search.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/stats.py` & `meeple_cli-0.2.0/src/meeple/command/stats.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/command/update.py` & `meeple_cli-0.2.0/src/meeple/command/import_.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,116 @@
-from datetime import date
+from typing import List
 
 import click
 
-from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE, get_bgg_items
-from meeple.util.collection_util import (
-    get_collections,
-    is_collection,
-    is_pending_updates,
-    read_collection,
-    update_collection,
-)
-from meeple.util.completion_util import complete_collections
-from meeple.util.data_util import last_updated, write_collection_data
-from meeple.util.message_util import (
-    info_msg,
-    invalid_collection_error,
-    no_collections_exist_error,
-    print_msg,
-)
-from meeple.util.sort_util import sort_items
+from meeple.type import BGG_COLLECTION_STATUSES, BGGCollectionItem
+from meeple.util.api_util import get_bgg_user, get_bgg_user_collection
+from meeple.util.collection_util import create_collection, unique_collection_name
+from meeple.util.input_util import choice_input
+from meeple.util.message_util import error_msg, info_msg, under_msg
+
+ONE_IMPORT_METHOD = "one"
+MANY_IMPORT_METHOD = "many"
+
+
+def _import_collection(
+    collection_items: List[BGGCollectionItem],
+    collection_name: str,
+    dry_run: bool,
+    verbose: bool,
+):
+    # assign a unique collection name
+    collection_name = unique_collection_name(collection_name)
+    # simulate import
+    if dry_run:
+        under_msg(
+            f"Import collection [u magenta]{collection_name}[/u magenta] containing {len(collection_items)} item(s)."
+        )
+    # perform import
+    else:
+        collection_ids = [item.bgg_id for item in collection_items]
+        create_collection(collection_name, to_add_ids=collection_ids)
+        under_msg(
+            f"Imported collection [u magenta]{collection_name}[/u magenta] containing {len(collection_items)} item(s)."
+        )
+    if verbose:
+        for item in collection_items:
+            under_msg(
+                f"[i blue]{item.name}[/i blue] ([dim]{item.bgg_id}[/dim])",
+                indents=2,
+            )
 
 
-@click.command()
-@click.argument("collection", required=False, shell_complete=complete_collections)
-@click.option("-f", "--force", is_flag=True, help="Force update.")
+@click.command(name="import")
+@click.argument("bgg-user")
+@click.option(
+    "--one",
+    "import_method",
+    flag_value=ONE_IMPORT_METHOD,
+    help="Import as one collection.",
+)
+@click.option(
+    "--many",
+    "import_method",
+    flag_value=MANY_IMPORT_METHOD,
+    help="Import as separate collections by status.",
+)
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    help="Simulate import operations without persisting.",
+)
+@click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
-def update(collection: str, force: bool) -> None:
-    """Update local collection data.
+def import_(bgg_user: str, import_method: bool, dry_run: bool, verbose: bool) -> None:
+    """Import BoardGameGeek user collections.
 
-    - COLLECTION (optional) is the name of the collection to be updated. If not provided, update all collections.
+    - BGG_USER is a BoardGameGeek username.
     """
-    info_msg("Updating collection data...")
+    # check that the given BoardGameGeek username is a valid
+    user = get_bgg_user(bgg_user)
+    if not user.user_id:
+        error_msg(f"[yellow]{bgg_user}[/yellow] is not a valid BoardGameGeek username.")
+
+    # get user collection items
+    collection_items = get_bgg_user_collection(bgg_user)
+
+    # check that the user collection is not empty
+    if not collection_items:
+        error_msg(
+            f"Nothing to import. BoardGameGeek user [yellow]{bgg_user}[/yellow]'s collection is empty."
+        )
+
+    # prompt the user for import method
+    if not import_method:
+        import_method = choice_input(
+            f"Would you like to import [magenta]{bgg_user}[/magenta]'s user collection items into one collection or many by item status?",
+            [ONE_IMPORT_METHOD, MANY_IMPORT_METHOD],
+        )
 
-    # update only a specific collection, if given. otherwise, attempt to udpate all
-    if collection:
-        # check that the given collection is a valid collection
-        if not is_collection(collection):
-            invalid_collection_error(collection)
-        collections = [collection]
+    if dry_run:
+        info_msg("Simulating collection import...")
     else:
-        collections = get_collections()
-
-    # check that local collections exist
-    if not collections:
-        no_collections_exist_error()
-
-    # update collection data
-    for collection in collections:
-        # get collection item ids
-        item_ids, to_add_ids, to_drop_ids = read_collection(collection)
-
-        # print warning and skip if collection is empty
-        if not item_ids and not to_add_ids and not to_drop_ids:
-            print_msg(
-                f" ╰╴ [yellow]Warning[/yellow]: Could not update collection [u magenta]{collection}[/u magenta] because it is empty. To add to it, run: [green]meeple add[/green]"
-            )
-            continue
-
-        # skip if collection not pending updates, has been updated today, and force flag not provided
-        updated = last_updated(collection)
-        if (
-            not force
-            and not is_pending_updates(collection)
-            and updated == str(date.today())
-        ):
-            print_msg(
-                f" ╰╴ [dim]Skipped collection [u magenta]{collection}[/u magenta]. Already up to date.[/dim]"
-            )
-            continue
+        info_msg("Importing collection(s)...")
 
-        # resolve pending updates, if any
-        if to_add_ids:
-            item_ids.extend(to_add_ids)
-            item_ids.sort()
-            to_add_ids = []
-        if to_drop_ids:
-            # nothing to resolve, just dump the pending update indicator
-            to_drop_ids = []
-        update_collection(collection, item_ids, to_add_ids, to_drop_ids)
-
-        # get items from BoardGameGeek
-        api_result = get_bgg_items(item_ids)
-        board_games, expansions = [], []
-        for item in api_result:
-            item_type = item.type
-            if item_type == BOARDGAME_TYPE:
-                board_games.append(item)
-            if item_type == EXPANSION_TYPE:
-                expansions.append(item)
-
-        # sort board games by rank and expansions by rating
-        if board_games:
-            board_games, _ = sort_items(board_games, "rank")
-        if expansions:
-            expansions, _ = sort_items(expansions, "rating")
-
-        # persist results
-        write_collection_data(collection, board_games, expansions)
-        print_msg(f" ╰╴ Updated collection [u magenta]{collection}[/u magenta].")
+    # create new collection(s) using the chosen import method or preform dry run
+    match import_method:
+        # import single collection with all items
+        case "one":
+            _import_collection(collection_items, bgg_user, dry_run, verbose)
+
+        # import a separate collection for each used item status
+        case "many":
+            # separate items into their respective status collections and import each
+            for status in BGG_COLLECTION_STATUSES:
+                # get items with status
+                status_items = [
+                    item for item in collection_items if status in item.statuses
+                ]
+                # import the collection if it contains items
+                if status_items:
+                    _import_collection(
+                        status_items, f"{bgg_user}-{status}", dry_run, verbose
+                    )
 
-    info_msg("Updated collection data.")
+    if not dry_run:
+        info_msg("Imported collection(s). To update, run [green]meeple update[/green]")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/root.py` & `meeple_cli-0.2.0/src/meeple/root.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,41 +4,42 @@
     add,
     collections,
     completions,
     delete,
     drop,
     find,
     hot,
+    import_,
     info,
-    list_collection,
+    list_,
     move,
     new,
-    open_on_bgg,
+    open_,
     rename,
     search,
     stats,
     update,
 )
 from meeple.util.cmd_util import SectionedHelpGroup
 
 commands = {
     "Collection Commands": [
         add,
         collections,
         delete,
         drop,
         find,
-        list_collection,
+        list_,
         move,
         new,
         rename,
         stats,
         update,
     ],
-    "BoardGameGeek Commands": [hot, info, open_on_bgg, search],
+    "BoardGameGeek Commands": [hot, import_, info, open_, search],
     "Other Commands": [completions],
 }
 
 
 @click.group(
     cls=SectionedHelpGroup,
     help="Local board game collection manager. Powered by BoardGameGeek.",
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/type/item.py` & `meeple_cli-0.2.0/src/meeple/type/item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import html
 import json
 
 
-def _grab_first(key_dict: dict) -> str:
+def _parse_sub_dict(key_dict: dict) -> str:
     if isinstance(key_dict, list):
-        return key_dict[0]["@value"]
-    return key_dict["@value"]
+        key_dict = key_dict[0]
+    if key_dict.get("@value"):
+        return key_dict["@value"]
+    elif key_dict.get("#text"):
+        return key_dict["#text"]
+    return None
 
 
 def _parse_item_float_val(key_dict: dict) -> float:
     value = key_dict["@value"]
     if value != "":
         return float(value)
     return 0.0
 
 
 def _parse_item_rank(ranks_dict: dict) -> str:
     if isinstance(ranks_dict, dict):
-        rank = _grab_first(ranks_dict["rank"])
+        rank = _parse_sub_dict(ranks_dict["rank"])
         if rank.isdigit():
             return rank
     return "NA"
 
 
 class Item:
     """Board Game or Expansion."""
@@ -114,16 +118,24 @@
         Args:
             bgg_dict (dict): dictionary to parse.
 
         Returns:
             Item: Item
         """
         rating = weight = rank = minplayers = maxplayers = playtime = minage = 0
-        item_id = int(bgg_dict["@id"])
-        name = _grab_first(bgg_dict["name"])
+        if bgg_dict.get("@id"):
+            item_id = int(bgg_dict["@id"])
+        elif bgg_dict.get("@objectid"):
+            item_id = int(bgg_dict["@objectid"])
+        else:
+            item_id = None
+        if bgg_dict.get("name"):
+            name = _parse_sub_dict(bgg_dict["name"])
+        else:
+            name = None
         if bgg_dict.get("@type"):
             item_type = bgg_dict["@type"]
         else:
             item_type = None
         if bgg_dict.get("yearpublished"):
             year = bgg_dict["yearpublished"]["@value"]
         else:
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/util/cmd_util.py` & `meeple_cli-0.2.0/src/meeple/util/cmd_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 
 from click import Group
 
 
 class SectionedHelpGroup(Group):
-    """Organize commands as sections"""
+    """Organize commands in sections."""
 
     def __init__(self, *args, **kwargs):
         self.section_commands = collections.defaultdict(list)
         super().__init__(*args, **kwargs)
 
     def add_command(self, cmd, name=None, section=None):
         self.section_commands[section].append(cmd)
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/util/data_util.py` & `meeple_cli-0.2.0/src/meeple/util/data_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import date
 from os import rename, walk
 from os.path import basename, join, splitext
 from pathlib import Path
 from typing import List
 
 from meeple.type.item import Item
-from meeple.util.fs_util import get_data_dir
+from meeple.util.fs_util import get_data_dir, read_json_file, write_json_file
 
 DATA_DIR = get_data_dir()
 
 _BOARD_GAME_LIST_KEY = "boardgames"
 _EXPANSION_LIST_KEY = "expansions"
 
 
@@ -48,23 +48,22 @@
 def get_collection_data(collection_name: str) -> (List[Item], List[Item]):
     data_path = _latest_data_file(collection_name)
     board_games, expansions = [], []
     if not data_path:
         return board_games, expansions
 
     # get latest collection data
-    with open(data_path, "r") as f:
-        data = json.load(f)
+    data_dict = read_json_file(data_path)
 
-    for dict_item in data[_BOARD_GAME_LIST_KEY]:
+    for item_dict in data_dict[_BOARD_GAME_LIST_KEY]:
         board_games.append(
-            json.loads(json.dumps(dict_item), object_hook=Item.from_json)
+            json.loads(json.dumps(item_dict), object_hook=Item.from_json)
         )
-    for dict_item in data[_EXPANSION_LIST_KEY]:
-        expansions.append(json.loads(json.dumps(dict_item), object_hook=Item.from_json))
+    for item_dict in data_dict[_EXPANSION_LIST_KEY]:
+        expansions.append(json.loads(json.dumps(item_dict), object_hook=Item.from_json))
     return board_games, expansions
 
 
 def write_collection_data(
     collection_name: str, board_games: List[Item], expansions: List[Item]
 ) -> None:
     today = date.today()
@@ -78,13 +77,12 @@
     # build data dictionary
     data_dict = {
         _BOARD_GAME_LIST_KEY: [board_game.__dict__ for board_game in board_games],
         _EXPANSION_LIST_KEY: [expansion.__dict__ for expansion in expansions],
     }
 
     # persist data
-    with open(join(data_path, filename), "w") as f:
-        json.dump(data_dict, f, indent=4, ensure_ascii=False)
+    write_json_file(join(data_path, filename), data_dict)
 
 
 def delete_collection_data(collection_name: str) -> None:
     shutil.rmtree(_collection_data_dir(collection_name))
```

### Comparing `meeple_cli-0.1.0rc1/src/meeple/util/filter_util.py` & `meeple_cli-0.2.0/src/meeple/util/filter_util.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/util/fmt_util.py` & `meeple_cli-0.2.0/src/meeple/util/fmt_util.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/util/sort_util.py` & `meeple_cli-0.2.0/src/meeple/util/sort_util.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/src/meeple/util/table_util.py` & `meeple_cli-0.2.0/src/meeple/util/table_util.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/tests/util/test_filter_util.py` & `meeple_cli-0.2.0/tests/util/test_filter_util.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/tests/util/test_fmt_util.py` & `meeple_cli-0.2.0/tests/util/test_fmt_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE
 from meeple.util.fmt_util import (
     NA_VALUE,
     fmt_avg_rank,
+    fmt_collection_name,
     fmt_item_type,
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
     fmt_weight,
     fmt_year,
 )
 
 
+def test_fmt_collection_name(mocker):
+    mocker.patch("meeple.util.fmt_util.is_pending_updates", side_effect=[True, False])
+
+    pending_output = fmt_collection_name("collection")
+    assert pending_output == "collection ([red]*[/red])"
+
+    no_pending_output = fmt_collection_name("collection")
+    assert no_pending_output == "collection"
+
+
 def test_fmt_players():
     na_output = fmt_players(0, 0)
     assert na_output == NA_VALUE
 
     output = fmt_players(1, 2)
     assert output == "1-2"
```

### Comparing `meeple_cli-0.1.0rc1/tests/util/test_fs_util.py` & `meeple_cli-0.2.0/tests/util/test_fs_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from meeple.util.fs_util import CONFIG_DIR_NAME, get_collection_dir, get_data_dir
+from meeple.util.fs_util import CONFIG_DIR_ROOT, get_collection_dir, get_data_dir
 
 
 def test_linux_collection_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["Linux"])
 
     collection_dir = get_collection_dir()
-    assert collection_dir == f"/home/user/{CONFIG_DIR_NAME}/collections"
+    assert collection_dir == f"/home/user/{CONFIG_DIR_ROOT}/collections"
 
 
 def test_mac_collection_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["Darwin"])
 
     collection_dir = get_collection_dir()
-    assert collection_dir == f"/Users/user/{CONFIG_DIR_NAME}/collections"
+    assert collection_dir == f"/Users/user/{CONFIG_DIR_ROOT}/collections"
 
 
 def test_win_collection_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["Windows"])
 
     collection_dir = get_collection_dir()
-    assert collection_dir == f"C:\\Users\\user\\{CONFIG_DIR_NAME}/collections"
+    assert collection_dir == f"C:\\Users\\user\\{CONFIG_DIR_ROOT}/collections"
 
 
 def test_other_collection_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["other"])
 
     collection_dir = get_collection_dir()
-    assert collection_dir == f"{CONFIG_DIR_NAME}/collections"
+    assert collection_dir == f"{CONFIG_DIR_ROOT}/collections"
 
 
 def test_linux_data_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["Linux"])
 
     collection_dir = get_data_dir()
-    assert collection_dir == f"/home/user/{CONFIG_DIR_NAME}/data"
+    assert collection_dir == f"/home/user/{CONFIG_DIR_ROOT}/data"
 
 
 def test_mac_data_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["Darwin"])
 
     collection_dir = get_data_dir()
-    assert collection_dir == f"/Users/user/{CONFIG_DIR_NAME}/data"
+    assert collection_dir == f"/Users/user/{CONFIG_DIR_ROOT}/data"
 
 
 def test_win_data_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["Windows"])
 
     collection_dir = get_data_dir()
-    assert collection_dir == f"C:\\Users\\user\\{CONFIG_DIR_NAME}/data"
+    assert collection_dir == f"C:\\Users\\user\\{CONFIG_DIR_ROOT}/data"
 
 
 def test_other_data_dir(mocker):
     mocker.patch("getpass.getuser", side_effect=["user"])
     mocker.patch("platform.system", side_effect=["other"])
 
     collection_dir = get_data_dir()
-    assert collection_dir == f"{CONFIG_DIR_NAME}/data"
+    assert collection_dir == f"{CONFIG_DIR_ROOT}/data"
```

### Comparing `meeple_cli-0.1.0rc1/tests/util/test_sort_util.py` & `meeple_cli-0.2.0/tests/util/test_sort_util.py`

 * *Files identical despite different names*

### Comparing `meeple_cli-0.1.0rc1/PKG-INFO` & `meeple_cli-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeple-cli
-Version: 0.1.0rc1
+Version: 0.2.0
 Summary: Local board game collection manager. Powered by BoardGameGeek.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >=8
 Requires-Dist: rich >=13
@@ -77,26 +77,27 @@
 Options:
   -h, --help     Show this message and exit.
   -v, --version  Show the version and exit.
 
 Collection Commands:
   add          Add an item to a collection.
   collections  List all collections.
-  delete       Delete a collection.
+  delete       Delete collections.
   drop         Remove an item from a collection.
   find         Search collections for items.
   list         List contents of a collection.
   move         Move an item from one collection to another.
-  new          Create a new collection.
-  rename       Rename a local collection.
+  new          Create new collections.
+  rename       Rename a collection.
   stats        Print out the details of a collection.
-  update       Update local collection data.
+  update       Update collection data.
 
 BoardGameGeek Commands:
   hot     List current BoardGameGeek trending items.
+  import  Import BoardGameGeek user collections.
   info    Print out the details of an item.
   open    Open an item on BoardGameGeek.
   search  Search BoardGameGeek for items.
 
 Other Commands:
   completions  Setup meeple shell completions.
 ```
@@ -154,19 +155,22 @@
 
 ## FAQ
 
 ### Why local only collections?
 
 Currently, the
 [BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
-provides limited _read-only_ data about user collections/GeekLists.
+provides limited _read-only_ data about user Collections and GeekLists.
 
-While it is _technically_ feasible to interface with GeekLists via
-webscrapers/spiders, this kind of practice would be both complex and also
-violate [BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
+While it is _technically_ feasible to interface with Collections and GeekLists
+via webscrapers or spiders, these approaches would be complex and also violate
+[BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
+
+For now, it is possible to import BGG user collections into `meeple-cli` via
+`meeple import`.
 
 ### Why do some items show a weight of `NA` when boardgamegeek.com has a value?
 
 This is a known and occasionally recurring bug in the BoardGameGeek database. It
 usually resolves itself within a day. For more info or additional support, read
 this [thread](https://boardgamegeek.com/thread/3049286/some-games-show-weight-000).
```

