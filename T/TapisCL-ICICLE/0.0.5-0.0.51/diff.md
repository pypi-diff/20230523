# Comparing `tmp/TapisCL-ICICLE-0.0.5.tar.gz` & `tmp/TapisCL-ICICLE-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.5.tar", last modified: Mon May 22 23:07:57 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.51.tar", last modified: Mon May 22 23:23:25 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.5.tar` & `TapisCL-ICICLE-0.0.51.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.761915 TapisCL-ICICLE-0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    44552 2023-05-22 23:07:57.760914 TapisCL-ICICLE-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-05-06 23:32:02.000000 TapisCL-ICICLE-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.738050 TapisCL-ICICLE-0.0.5/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      179 2023-05-20 02:11:42.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.741554 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0        0 2023-05-22 18:07:08.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     5345 2023-05-22 22:44:28.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     4514 2023-05-22 22:51:51.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/connectionInitializer.py
--rw-rw-rw-   0        0        0     1223 2023-05-22 22:02:30.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/formatters.py
--rw-rw-rw-   0        0        0     2854 2023-05-22 17:32:14.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/handlers.py
--rw-rw-rw-   0        0        0      895 2023-05-22 17:33:12.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/parsers.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.748057 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3420 2023-05-22 22:11:32.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/appCommands.py
--rw-rw-rw-   0        0        0     8167 2023-05-22 22:25:22.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     5271 2023-05-22 22:15:59.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2977 2023-05-22 22:16:59.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     2189 2023-05-22 22:09:31.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     4429 2023-05-22 22:09:56.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.750408 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-12 00:56:17.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1401 2023-05-22 19:18:23.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      845 2023-05-22 19:18:29.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     1997 2023-05-22 22:13:09.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     4479 2023-05-22 22:36:26.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/systemCommands.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.751408 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-22 18:06:58.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0     8718 2023-05-22 22:59:25.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      527 2023-05-22 17:16:29.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/serverConnection.py
--rw-rw-rw-   0        0        0      161 2023-05-22 18:14:34.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.756410 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-05-16 02:10:29.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/args.py
--rw-rw-rw-   0        0        0     8565 2023-05-22 22:18:35.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/decorators.py
--rw-rw-rw-   0        0        0     2141 2023-05-21 18:27:51.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1201 2023-05-22 17:13:08.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/logger.py
--rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/schemas.py
--rw-rw-rw-   0        0        0     2504 2023-05-18 17:55:40.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.759914 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44552 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-05-22 23:04:46.000000 TapisCL-ICICLE-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 23:07:57.761915 TapisCL-ICICLE-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.977568 TapisCL-ICICLE-0.0.51/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.51/LICENSE
+-rw-rw-rw-   0        0        0    44553 2023-05-22 23:23:25.977568 TapisCL-ICICLE-0.0.51/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-05-06 23:32:02.000000 TapisCL-ICICLE-0.0.51/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.954491 TapisCL-ICICLE-0.0.51/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-05-20 02:11:42.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.958996 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0        0 2023-05-22 18:07:08.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     5345 2023-05-22 22:44:28.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     4514 2023-05-22 22:51:51.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/connectionInitializer.py
+-rw-rw-rw-   0        0        0     1223 2023-05-22 22:02:30.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/formatters.py
+-rw-rw-rw-   0        0        0     2854 2023-05-22 17:32:14.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/handlers.py
+-rw-rw-rw-   0        0        0      895 2023-05-22 17:33:12.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/parsers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.963996 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3420 2023-05-22 22:11:32.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/appCommands.py
+-rw-rw-rw-   0        0        0     8167 2023-05-22 22:25:22.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     5271 2023-05-22 22:15:59.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2977 2023-05-22 22:16:59.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     2189 2023-05-22 22:09:31.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     4429 2023-05-22 22:09:56.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.965996 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-12 00:56:17.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1401 2023-05-22 19:18:23.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      845 2023-05-22 19:18:29.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     1997 2023-05-22 22:13:09.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     4479 2023-05-22 22:36:26.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/systemCommands.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.967498 TapisCL-ICICLE-0.0.51/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-22 18:06:58.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0     8718 2023-05-22 22:59:25.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      527 2023-05-22 17:16:29.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/server/serverConnection.py
+-rw-rw-rw-   0        0        0      161 2023-05-22 18:14:34.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.972500 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-05-16 02:10:29.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/args.py
+-rw-rw-rw-   0        0        0     8565 2023-05-22 22:18:35.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/decorators.py
+-rw-rw-rw-   0        0        0     2141 2023-05-21 18:27:51.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1201 2023-05-22 17:13:08.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/logger.py
+-rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/schemas.py
+-rw-rw-rw-   0        0        0     2504 2023-05-18 17:55:40.000000 TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:23:25.976501 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44553 2023-05-22 23:23:25.000000 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-22 23:23:25.000000 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 23:23:25.000000 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-22 23:23:25.000000 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-22 23:23:25.000000 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 23:23:25.000000 TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-05-22 23:23:19.000000 TapisCL-ICICLE-0.0.51/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 23:23:25.977568 TapisCL-ICICLE-0.0.51/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.5/LICENSE` & `TapisCL-ICICLE-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/PKG-INFO` & `TapisCL-ICICLE-0.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.5
+Version: 0.0.51
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.5/README.md` & `TapisCL-ICICLE-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/connectionInitializer.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/connectionInitializer.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/formatters.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/formatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/parsers.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/client/parsers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/commands/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/serverConnection.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/server/serverConnection.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/args.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/decorators.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/schemas.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/socketOpts.py` & `TapisCL-ICICLE-0.0.51/TapisCLICICLE/utilities/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.5
+Version: 0.0.51
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.51/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.5/pyproject.toml` & `TapisCL-ICICLE-0.0.51/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.5"
+version = "0.0.51"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

