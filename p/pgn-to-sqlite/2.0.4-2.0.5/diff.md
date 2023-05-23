# Comparing `tmp/pgn_to_sqlite-2.0.4.tar.gz` & `tmp/pgn_to_sqlite-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_to_sqlite-2.0.4.tar", last modified: Sat May  6 01:28:32 2023, max compression
+gzip compressed data, was "pgn_to_sqlite-2.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pgn_to_sqlite-2.0.4.tar` & `pgn_to_sqlite-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.coveragerc
--rw-r--r--   0        0        0      620 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      694 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       84 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.gitignore
--rw-r--r--   0        0        0     1078 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/LICENSE
--rw-r--r--   0        0        0     2867 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/README.md
--rw-r--r--   0        0        0      111 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pgn_to_sqlite/__init__.py
--rw-r--r--   0        0        0     8071 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pgn_to_sqlite/cli.py
--rw-r--r--   0        0        0      896 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      155 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pytest.ini
--rw-r--r--   0        0        0      265 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/requirements.in
--rw-r--r--   0        0        0    22534 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/__init__.py
--rw-r--r--   0        0        0      506 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/game_files/test_pgn_file_chess_dotcom.pgn
--rw-r--r--   0        0        0      885 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/game_files/test_pgn_file_lichess.pgn
--rw-r--r--   0        0        0     1369 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/test_cli.py
--rw-r--r--   0        0        0      159 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tox.ini
--rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-05-23 21:46:10.993140 pgn_to_sqlite-2.0.5/.coveragerc
+-rw-r--r--   0        0        0      620 2023-05-23 21:46:10.993140 pgn_to_sqlite-2.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      694 2023-05-23 21:46:10.993140 pgn_to_sqlite-2.0.5/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       84 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1078 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2867 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/README.md
+-rw-r--r--   0        0        0      111 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pgn_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     8071 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pgn_to_sqlite/cli.py
+-rw-r--r--   0        0        0      919 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pytest.ini
+-rw-r--r--   0        0        0      265 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/requirements.in
+-rw-r--r--   0        0        0    22534 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      506 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/game_files/test_pgn_file_chess_dotcom.pgn
+-rw-r--r--   0        0        0      885 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/game_files/test_pgn_file_lichess.pgn
+-rw-r--r--   0        0        0     1369 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/test_cli.py
+-rw-r--r--   0        0        0      159 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tox.ini
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.0.5/PKG-INFO
```

### Comparing `pgn_to_sqlite-2.0.4/.github/workflows/publish.yml` & `pgn_to_sqlite-2.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/.github/workflows/run_tests.yml` & `pgn_to_sqlite-2.0.5/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/LICENSE` & `pgn_to_sqlite-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/README.md` & `pgn_to_sqlite-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/pgn_to_sqlite/cli.py` & `pgn_to_sqlite-2.0.5/pgn_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/pyproject.toml` & `pgn_to_sqlite-2.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ] 
 description-file = "README.md"
 requires = [
-    "click",
-    "requests",
-    "berserk"
+    "click==8.1.3",
+    "requests==2.31.0",
+    "berserk==0.10.0"
 ]
 requires-python=">=3.7"
 
 [tool.flit.metadata.urls]
 Documentation = "https://github.com/EndlessTrax/pgn-to-sqlite/blob/master/README.md"
 Issues = "https://github.com/EndlessTrax/pgn-to-sqlite/issues"
```

### Comparing `pgn_to_sqlite-2.0.4/requirements.txt` & `pgn_to_sqlite-2.0.5/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -187,17 +187,17 @@
     # via
     #   -r requirements.in
     #   pytest-cov
 pytest-cov==4.0.0 \
     --hash=sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b \
     --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
     # via -r requirements.in
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   -r requirements.in
     #   berserk
     #   flit
 ruff==0.0.86 \
     --hash=sha256:0da330ff6d0a993d9a2fd86792600676b63be2a82fbe1d8dddb5971ceec51838 \
     --hash=sha256:17738ac99d7a7ba09a1907d15c48e80dcdf616744f1557ef8abb773353bee2c3 \
```

### Comparing `pgn_to_sqlite-2.0.4/tests/game_files/test_pgn_file_lichess.pgn` & `pgn_to_sqlite-2.0.5/tests/game_files/test_pgn_file_lichess.pgn`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/tests/test_cli.py` & `pgn_to_sqlite-2.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.4/PKG-INFO` & `pgn_to_sqlite-2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pgn_to_sqlite
-Version: 2.0.4
+Version: 2.0.5
 Summary: Fetch your games from chess.com and lichess.org and add them to a sqlite database
 Home-page: https://github.com/EndlessTrax/pgn-to-sqlite
 Author: Ricky White
 Author-email: ricky@whitelionmedia.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click
-Requires-Dist: requests
-Requires-Dist: berserk
+Requires-Dist: click==8.1.3
+Requires-Dist: requests==2.31.0
+Requires-Dist: berserk==0.10.0
 Project-URL: Documentation, https://github.com/EndlessTrax/pgn-to-sqlite/blob/master/README.md
 Project-URL: Issues, https://github.com/EndlessTrax/pgn-to-sqlite/issues
 
 # PGN to Sqlite
 
 ![PyPI version](https://img.shields.io/pypi/v/pgn-to-sqlite)
 ![GitHub](https://img.shields.io/github/license/endlesstrax/pgn-to-sqlite)
```

