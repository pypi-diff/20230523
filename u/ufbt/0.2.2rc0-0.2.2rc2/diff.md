# Comparing `tmp/ufbt-0.2.2rc0.tar.gz` & `tmp/ufbt-0.2.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.2rc0.tar", last modified: Sun May  7 15:17:13 2023, max compression
+gzip compressed data, was "ufbt-0.2.2rc2.tar", last modified: Mon May 22 22:39:50 2023, max compression
```

## Comparing `ufbt-0.2.2rc0.tar` & `ufbt-0.2.2rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:13.476405 ufbt-0.2.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-07 15:17:13.472404 ufbt-0.2.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 15:17:13.476405 ufbt-0.2.2rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:13.472404 ufbt-0.2.2rc0/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26425 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:13.472404 ufbt-0.2.2rc0/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:39:50.221113 ufbt-0.2.2rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-05-22 22:39:38.000000 ufbt-0.2.2rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-22 22:39:50.221113 ufbt-0.2.2rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-22 22:39:38.000000 ufbt-0.2.2rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 22:39:38.000000 ufbt-0.2.2rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:39:50.221113 ufbt-0.2.2rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:39:50.217112 ufbt-0.2.2rc2/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-22 22:39:38.000000 ufbt-0.2.2rc2/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-22 22:39:38.000000 ufbt-0.2.2rc2/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26454 2023-05-22 22:39:38.000000 ufbt-0.2.2rc2/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:39:50.217112 ufbt-0.2.2rc2/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-22 22:39:50.000000 ufbt-0.2.2rc2/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 22:39:50.000000 ufbt-0.2.2rc2/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:39:50.000000 ufbt-0.2.2rc2/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 22:39:50.000000 ufbt-0.2.2rc2/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 22:39:50.000000 ufbt-0.2.2rc2/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.2rc0/LICENSE.md` & `ufbt-0.2.2rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.2rc0/PKG-INFO` & `ufbt-0.2.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.2rc0
+Version: 0.2.2rc2
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.2rc0/README.md` & `ufbt-0.2.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.2rc0/pyproject.toml` & `ufbt-0.2.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.2rc0/ufbt/__init__.py` & `ufbt-0.2.2rc2/ufbt/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,41 +44,39 @@
     ufbt_state_dir = pathlib.Path(os.environ["UFBT_STATE_DIR"])
 
     # if any of bootstrap subcommands are in the arguments - call it instead
     # kept for compatibility with old scripts, better use `ufbt-bootstrap` directly
     if any(map(sys.argv.__contains__, bootstrap_subcommands)):
         return bootstrap_cli()
 
-    if not os.path.exists(ufbt_state_dir):
-        bootstrap_cli()
+    if not os.path.exists(ufbt_state_dir / "current"):
+        bootstrap_cli(["update"])
 
     if not (ufbt_state_dir / "current" / "scripts" / "ufbt").exists():
         print("SDK is missing scripts distribution!")
         print("You might be trying to use an SDK in an outdated format.")
         print("Run `ufbt update -h` for more information on how to update.")
         return 1
 
     UFBT_APP_DIR = os.getcwd()
 
     if platform.system() == "Windows":
         commandline = (
             r'call "%UFBT_STATE_DIR%/current/scripts/toolchain/fbtenv.cmd" env & '
-            'python -m SCons -Q --warn=target-not-built '
+            "python -m SCons -Q --warn=target-not-built "
             r'-C "%UFBT_STATE_DIR%/current/scripts/ufbt" '
-            f'"UFBT_APP_DIR={UFBT_APP_DIR}" '
-            + " ".join(sys.argv[1:])
+            f'"UFBT_APP_DIR={UFBT_APP_DIR}" ' + " ".join(sys.argv[1:])
         )
 
     else:
         commandline = (
             '. "$UFBT_STATE_DIR/current/scripts/toolchain/fbtenv.sh" && '
-            'python3 -m SCons -Q --warn=target-not-built '
+            "python3 -m SCons -Q --warn=target-not-built "
             '-C "$UFBT_STATE_DIR/current/scripts/ufbt" '
-            f'"UFBT_APP_DIR={UFBT_APP_DIR}" '
-            + " ".join(sys.argv[1:])
+            f'"UFBT_APP_DIR={UFBT_APP_DIR}" ' + " ".join(sys.argv[1:])
         )
 
     # print(commandline)
     retcode = os.system(commandline)
     if platform.system() != "Windows":
         # low byte is signal number, high byte is exit code
         retcode = retcode >> 8
```

### Comparing `ufbt-0.2.2rc0/ufbt/__main__.py` & `ufbt-0.2.2rc2/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.2rc0/ufbt/bootstrap.py` & `ufbt-0.2.2rc2/ufbt/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,15 +733,15 @@
 bootstrap_subcommand_classes = (UpdateSubcommand, CleanSubcommand, StatusSubcommand)
 
 bootstrap_subcommands = (
     subcommand_cls.COMMAND for subcommand_cls in bootstrap_subcommand_classes
 )
 
 
-def bootstrap_cli() -> Optional[int]:
+def bootstrap_cli(cmdline_args=None) -> Optional[int]:
     logging.basicConfig(
         format="%(asctime)s.%(msecs)03d [%(levelname).1s] %(message)s",
         level=logging.INFO,
         datefmt="%H:%M:%S",
     )
 
     root_parser = argparse.ArgumentParser()
@@ -771,15 +771,15 @@
         default=False,
     )
 
     parsers = root_parser.add_subparsers()
     for subcommand_cls in bootstrap_subcommand_classes:
         subcommand_cls().add_to_parser(parsers)
 
-    args = root_parser.parse_args()
+    args = root_parser.parse_args(cmdline_args)
     if args.verbose:
         logging.getLogger().setLevel(logging.DEBUG)
 
     if args.no_check_certificate:
         # Temporary fix for SSL negotiation failure on Mac
         import ssl
```

### Comparing `ufbt-0.2.2rc0/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.2rc2/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.2rc0
+Version: 0.2.2rc2
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

