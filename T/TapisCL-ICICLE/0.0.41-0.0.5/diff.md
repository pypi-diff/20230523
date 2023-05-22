# Comparing `tmp/TapisCL-ICICLE-0.0.41.tar.gz` & `tmp/TapisCL-ICICLE-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.41.tar", last modified: Fri May  5 04:55:44 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.5.tar", last modified: Mon May 22 23:07:57 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.41.tar` & `TapisCL-ICICLE-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.307656 TapisCL-ICICLE-0.0.41/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.41/LICENSE
--rw-rw-rw-   0        0        0    45182 2023-05-05 04:55:44.307656 TapisCL-ICICLE-0.0.41/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-04-29 18:49:44.000000 TapisCL-ICICLE-0.0.41/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.292088 TapisCL-ICICLE-0.0.41/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0    11616 2023-05-05 01:58:15.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.296180 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3705 2023-05-04 21:09:52.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/apps.py
--rw-rw-rw-   0        0        0     2164 2023-05-04 21:08:20.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/baseWrappers.py
--rw-rw-rw-   0        0        0     2477 2023-05-04 21:08:10.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/files.py
--rw-rw-rw-   0        0        0     5482 2023-05-04 21:07:53.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/pods.py
--rw-rw-rw-   0        0        0     2036 2023-05-04 21:06:58.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/query.py
--rw-rw-rw-   0        0        0     5089 2023-05-05 02:51:57.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     5389 2023-05-04 21:05:56.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/systems.py
--rw-rw-rw-   0        0        0     8231 2023-05-05 04:54:37.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/server.py
-drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.302159 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/args.py
--rw-rw-rw-   0        0        0     9449 2023-05-05 02:42:29.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/decorators.py
--rw-rw-rw-   0        0        0     2121 2023-04-29 18:26:16.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     6098 2023-05-05 02:34:10.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/helpers.py
--rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/logger.py
--rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/schemas.py
--rw-rw-rw-   0        0        0      493 2023-05-05 04:54:37.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/serverConnection.py
--rw-rw-rw-   0        0        0     2525 2023-05-05 02:37:18.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.306659 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    45182 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-05-05 04:54:14.000000 TapisCL-ICICLE-0.0.41/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 04:55:44.308158 TapisCL-ICICLE-0.0.41/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.761915 TapisCL-ICICLE-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    44552 2023-05-22 23:07:57.760914 TapisCL-ICICLE-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-05-06 23:32:02.000000 TapisCL-ICICLE-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.738050 TapisCL-ICICLE-0.0.5/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-05-20 02:11:42.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.741554 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0        0 2023-05-22 18:07:08.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     5345 2023-05-22 22:44:28.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     4514 2023-05-22 22:51:51.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/connectionInitializer.py
+-rw-rw-rw-   0        0        0     1223 2023-05-22 22:02:30.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/formatters.py
+-rw-rw-rw-   0        0        0     2854 2023-05-22 17:32:14.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/handlers.py
+-rw-rw-rw-   0        0        0      895 2023-05-22 17:33:12.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/client/parsers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.748057 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3420 2023-05-22 22:11:32.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/appCommands.py
+-rw-rw-rw-   0        0        0     8167 2023-05-22 22:25:22.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     5271 2023-05-22 22:15:59.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2977 2023-05-22 22:16:59.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     2189 2023-05-22 22:09:31.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     4429 2023-05-22 22:09:56.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.750408 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-12 00:56:17.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1401 2023-05-22 19:18:23.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      845 2023-05-22 19:18:29.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     1997 2023-05-22 22:13:09.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     4479 2023-05-22 22:36:26.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/systemCommands.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.751408 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-22 18:06:58.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0     8718 2023-05-22 22:59:25.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      527 2023-05-22 17:16:29.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/serverConnection.py
+-rw-rw-rw-   0        0        0      161 2023-05-22 18:14:34.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.756410 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-05-16 02:10:29.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/args.py
+-rw-rw-rw-   0        0        0     8565 2023-05-22 22:18:35.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/decorators.py
+-rw-rw-rw-   0        0        0     2141 2023-05-21 18:27:51.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1201 2023-05-22 17:13:08.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/logger.py
+-rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/schemas.py
+-rw-rw-rw-   0        0        0     2504 2023-05-18 17:55:40.000000 TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:07:57.759914 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44552 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 23:07:57.000000 TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-05-22 23:04:46.000000 TapisCL-ICICLE-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 23:07:57.761915 TapisCL-ICICLE-0.0.5/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.41/LICENSE` & `TapisCL-ICICLE-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.41/PKG-INFO` & `TapisCL-ICICLE-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.41
+Version: 0.0.5
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,18 +709,14 @@
 #### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
 2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
 3. enter your username and password when prompted
 4. if all went well the console should open. You can run `help` to see command options
 5. to exit the application, run `exit`
 
-**Running Several Instances of Client**
-
-There are some situations a user might want to have 2 or more windows of the same command line app open. For instance, you might need to be reading a static help menu at the same time as you are typing commands. TapisCLICICLE provides this capability, however, with some caveats. Since each client utilizes the same application resources, some commands are blocking. This means that if you run something that asks for authentication, or run a query to postgres or neo4j, you will have to respond to application prompts before any other commands are executed on other active clients.
-
 #### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
```

### Comparing `TapisCL-ICICLE-0.0.41/README.md` & `TapisCL-ICICLE-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,25 +19,21 @@
 #### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
 2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
 3. enter your username and password when prompted
 4. if all went well the console should open. You can run `help` to see command options
 5. to exit the application, run `exit`
 
-**Running Several Instances of Client**
-
-There are some situations a user might want to have 2 or more windows of the same command line app open. For instance, you might need to be reading a static help menu at the same time as you are typing commands. TapisCLICICLE provides this capability, however, with some caveats. Since each client utilizes the same application resources, some commands are blocking. This means that if you run something that asks for authentication, or run a query to postgres or neo4j, you will have to respond to application prompts before any other commands are executed on other active clients.
-
 #### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
 **Scripting**
 
 Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
 
 ### Known Issues
-Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
+Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/files.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/fileCommands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,51 @@
+from tapipy import tapis
+import pyperclip
+import json
 try:
-    from . import baseWrappers
+    from . import baseCommand
+    from ..utilities import decorators
 except:
-    import commands.baseWrappers as baseWrappers
+    import commands.baseCommand as baseCommand
+    import utilities.decorators as decorators
 
 
-class Files(baseWrappers.tapisObject):
+class list_files(baseCommand.BaseCommand):
     """
-    @help: Access Tapis files through the connected service
+    @help: list the files on a system 
     """
-    def __init__(self, tapis_instance, username, password, connection=None):
-        command_map = {
-            'list_files':self.list_files,
-            'upload':self.upload,
-            'download':self.download,
-            'help':self.help
-        }
-        super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
-
-    def return_formatter(self, info):
-        return f"name: {info.name}\ngroup: {info.group}\npath: {info.path}\n"
-
-    async def list_files(self, verbose: bool, id: str, file: str, connection=None) -> str: # lists files available on a tapis account
-        """
-        @help: list the files on a system 
-        """
+    async def run(self, id: str, file: str, *args, **kwargs) -> str: # lists files available on a tapis account
         file_list = self.t.files.listFiles(systemId=id, path=file)
-        if verbose:
-            return str(file_list)
-        file_list = [self.return_formatter(f) for f in file_list]
         return str(file_list)
+    
 
-    async def upload(self, file: str, id: str, connection=None) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
-        """
-        @help: upload a file to the system 
-        the source and destination files must both be in the file argument, respectively, separated by a comma
-        """
+class upload(baseCommand.BaseCommand):
+    """
+    @help: upload a file to the system 
+    the source and destination files must both be in the file argument, respectively, separated by a comma
+    @todo: make it so that this doesnt need to take both source and destination files, but have it so it retrieves the current file location on the tapis system
+    and sets that file location to be the upload point. Do the same for downloads but in reverse
+    """
+    async def run(self, file: str, id: str, *args, **kwargs) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
         source = file.split(",")[0]
         destination = file.split(",")[1]
         self.t.upload(system_id=id,
                 source_file_path=source,
                 dest_file_path=destination)
         return f'successfully uploaded {source} to {destination}'
-            
-    async def download(self, file: str, id: str, connection=None) -> str: # download a remote file using tapis, operates basically the same as upload
-        """
-        @help: download a file from the system
-        the source and destination files must both be in the file argument, respectively, separated by a comma
-        """
+
+
+class download(baseCommand.BaseCommand):
+    """
+    @help: download a file from the system
+    the source and destination files must both be in the file argument, respectively, separated by a comma
+    """
+    async def run(self, file: str, id: str, *args, **kwargs) -> str: # download a remote file using tapis, operates basically the same as upload
         source = file.split(",")[0]
         destination = file.split(",")[1]
         file_info = self.t.files.getContents(systemId=id,
                             path=source)
 
         file_info = file_info.decode('utf-8')
         with open(destination, 'w') as f:
             f.write(file_info)
-        return f'successfully downloaded {source} to {destination}'
+        return f'successfully downloaded {source} to {destination}'
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/systems.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/commands/systemCommands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,109 @@
+from tapipy import tapis
+import pyperclip
 import json
 import os
 try:
+    from . import baseCommand
     from ..utilities import decorators
-    from . import baseWrappers
 except:
+    import commands.baseCommand as baseCommand
     import utilities.decorators as decorators
-    import commands.baseWrappers as baseWrappers
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 server_path = os.path.join(__location__, '..\\server.py')
 
 
+class get_systems(baseCommand.BaseCommand):
+    """
+    @help: Gets and returns the list of systems the current Tapis service and account have access to
+    @doc: this is an example of the doc segment of the docstring. not included in help message
+    """
+    async def run(self, *args, **kwargs):
+        systems = self.t.systems.getSystems()
+        return systems
+    
 
-class Systems(baseWrappers.tapisObject):
+class get_system_info(baseCommand.BaseCommand):
     """
-    @help: Access Tapis systems through the connected service
-    @doc: provides a CLI interface to the Tapis Systems service
+    @help: get information on a selected system
     """
-    def __init__(self, tapis_instance, username, password, connection=None):
-        command_map = {
-            'get_systems':self.get_systems,
-            'get_system_info':self.get_system_info,
-            'create_system':self.create_system,
-            'set_credentials':self.system_credential_upload,
-            'set_password':self.system_password_set,
-            'delete_system':self.delete_system,
-            'help':self.help
-        }
-        super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
+    async def run(self, id:str, *args, **kwargs): 
+        system_info = self.t.systems.getSystem(systemId=id)
+        return system_info
+    
+
+class set_system_credentials(baseCommand.BaseCommand):
+    """
+    @help: upload system credentials to a system. Must generate keys first using 'ssh-keygen -m PEM -f id_rsa', and format with, 'awk -v ORS='\\n' '1' <private_key_name>
+    file argument must contain the path to the private and public keys respectively, separated by a ','
+    """
+    async def run(self, id: str, file: str, *args, **kwargs): # get information about a system given its ID
+        with open(file.split(",")[0], 'r') as f:
+            private_key = f.read()
 
-    def return_formatter(self, info):
-        return f"id: {info.id}\nhost: {info.host}\n\n"
+        with open(file.split(",")[1], 'r') as f:
+            public_key = f.read()
 
+        cred_return_value = self.t.systems.createUserCredential(systemId=id,
+                            userName=self.username,
+                            privateKey=private_key,
+                            publicKey=public_key)
+
+        return str(cred_return_value)
+
+
+class create_system(baseCommand.BaseCommand):
+    """
+    @help: create a system. Must have a properly configured system file.
+    see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
+    this command will automatically create and upload the ssh keys
+    """
+    set_system_creds = set_system_credentials()
     def __keygen(self):
         local_files = os.listdir(__location__)
         if "id_rsa" not in local_files or "id_rsa.pub" not in local_files:
             os.system(f'ssh-keygen -q -m PEM -f {__location__}\\id_rsa -N ""')
             with open(f"{__location__}\\id_rsa", 'r') as f:
                 formatted_key = ""
                 for line in f.readlines()[1:-1]:
                     formatted_key += line.strip()
 
             with open(f"{__location__}\\id_rsa", 'w') as f:
                 f.write(formatted_key)
 
-    async def get_systems(self, verbose: bool, connection=None):
-        """
-        @help: Gets and returns the list of systems the current Tapis service and account have access to
-        @doc: this is an example of the doc segment of the docstring. not included in help message
-        """
-        systems = self.t.systems.getSystems()
-        if systems and verbose:
-            return str(systems)
-        systems = [self.return_formatter(system) for system in systems]
-        systems_string = ''
-        for system in systems:
-            systems_string += system
-        return systems_string
-
-    async def get_system_info(self, verbose: bool, id:str, connection=None): # get information about a system given its ID
-        """
-        @help: get information on a selected system
-        """
-        system_info = self.t.systems.getSystem(systemId=id)
-        if verbose:
-            return str(system_info)
-        return self.return_formatter(system_info)
-    
-    async def create_system(self, file: str, connection=None) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
-        """
-        @help: create a system. Must have a properly configured system file.
-        see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
-        this command will automatically create and upload the ssh keys
-        """
+    async def run(self, file: str, *args, **kwargs) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
+        self.set_system_creds.set_t_and_creds(self.t, self.username, self.password)
+
         self.__keygen()
         with open(file, 'r') as f:
             system = json.loads(f.read())
         return_value = self.t.systems.createSystem(**system)
-        self.system_credential_upload(id=system['id'], file=f"{__location__}\\id_rsa,{__location__}\\id_rsa.pub")
-        return str(return_value)
+        self.set_system_creds(id=system['id'], file=f"{__location__}\\id_rsa,{__location__}\\id_rsa.pub")
+        return return_value
     
-    async def system_credential_upload(self, id: str, file: str, connection=None) -> str: # upload key credentials for the system
-        """
-        @help: upload system credentials to a system. Must generate keys first using 'ssh-keygen -m PEM -f id_rsa', and format with, 'awk -v ORS='\\n' '1' <private_key_name>
-        file argument must contain the path to the private and public keys respectively, separated by a ','
-        """
-        with open(file.split(",")[0], 'r') as f:
-            private_key = f.read()
 
-        with open(file.split(",")[1], 'r') as f:
-            public_key = f.read()
-
-        cred_return_value = self.t.systems.createUserCredential(systemId=id,
-                            userName=self.username,
-                            privateKey=private_key,
-                            publicKey=public_key)
-
-        return str(cred_return_value)
-
-    @decorators.SecureInput
-    async def system_password_set(self, id: str, password: str, connection=None) -> str: # set the password for a system
-        """
-        @help: set a system password
-        """
+class set_system_password(baseCommand.BaseCommand):
+    """
+    @help: set a system password
+    """
+    decorator=decorators.SecureInput()
+    async def run(self, id: str, password: str=None, *args, **kwargs) -> str: # set the password for a system
         try:
             password_return_value = self.t.systems.createUserCredential(systemId=id, # will put this in a getpass later
                                 userName=self.username,
                                 password=password)
             return str(password_return_value)
         except Exception as e:
             raise Exception(f"{e}\nTry running set_credentials if the problem persists")
+        
 
-    @decorators.NeedsConfirmation
-    async def delete_system(self, id: str, connection=None) -> str:
-        """
-        @help: delete the selected system
-        """
+class delete_system(baseCommand.BaseCommand):
+    """
+    @help: delete the selected system
+    """
+    decorator=decorators.NeedsConfirmation()
+    async def run(self, id: str, *args, **kwargs) -> str:
         return_value = self.t.systems.deleteSystem(systemId=id)
-        return return_value
+        return return_value
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,85 +7,124 @@
 import os
 import logging
 import typing
 import asyncio
 import traceback
 
 try:
-    from .utilities import exceptions
-    from .utilities import logger
-    from .utilities import socketOpts as SO
-    from .utilities import helpers
-    from .utilities import schemas
-    from .utilities import serverConnection
-    from .commands import serverCommands as serverCommands
-except:
+    from ..utilities import exceptions
+    from ..utilities import logger
+    from ..utilities import socketOpts as SO
+    from ..utilities import killableThread
+    from ..utilities import schemas
+    from . import serverConnection
+    from ..commands.query import neo4j, postgres
+    from ..commands import baseCommand
+    from ..commands import commandMap
+    from ..utilities import decorators
+except ImportError:
+    import utilities.decorators as decorators
     import utilities.exceptions as exceptions
     import utilities.logger as logger
     import utilities.socketOpts as SO
-    import utilities.helpers as helpers
+    import utilities.killableThread as killableThread
     import utilities.schemas as schemas
-    import utilities.serverConnection as serverConnection
-    import commands.serverCommands as serverCommands
+    import server.serverConnection as serverConnection
+    import commands.baseCommand as baseCommand
+    import commands.commandMap as commandMap
 
 
-class Server(helpers.OperationsHelper, serverCommands.ServerCommands, logger.ServerLogger):
+class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup):
     """
     Receives commands from the client and executes Tapis operations
     """
     def __init__(self, IP: str, PORT: int):
         super().__init__()
         self.initial = True
 
+        self.t = None
+        self.url = None
+        self.access_token = None
+        self.username = None
+        self.password = None
+
         self.__name__ = "Server"
         self.initialize_logger(self.__name__)
         # setting up socket server
         self.ip, self.port = IP, PORT
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.setblocking(False)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.bind((self.ip, self.port))
         self.sock.listen(1)
         self.end_time = time.time() + 300  # start the countdown on the timeout
 
         self.server = None
 
         self.logger.info('initialization complete')
-    
+
+    def switch_session(self, username: str, password, link: str, *args, **kwargs):
+        start = time.time()
+        try:
+            t = Tapis(base_url=f"https://{link}",
+                    username=username,
+                    password=password)
+            t.get_tokens()
+        except Exception as e:
+            self.logger.warning(e)
+            raise ValueError(f"Invalid tapis auth credentials")
+        
+        self.username = username
+        self.password = password
+        self.t = t
+        self.url = link
+        self.access_token = self.t.access_token
+
+        self.configure_decorators(self.username, self.password)
+        self.update_credentials(t, username, password)
+        # V3 Headers
+        header_dat = {"X-Tapis-token": t.access_token.access_token,
+                      "Content-Type": "application/json"}
+        # create authenticator for tapis systems
+        authenticator = t.access_token
+        # extract the access token from the authenticator
+        
+        if 'win' in sys.platform:
+            os.system(f"set JWT={self.access_token}")
+        else: # unix based
+            os.system(f"export JWT={self.access_token}")
+
+        self.logger.info(f"initiated in {time.time()-start}")
+
+        return f"Successfully initialized tapis service on {self.url}"
+
     async def handshake(self, connection):
         self.logger.info("Handshake starting")
         if self.initial:  # if this is the first time in the session that the cli is connecting
             startup_data = schemas.StartupData(initial = self.initial)
-            print("sending data")
             await connection.send(startup_data)
             self.logger.info("send the initial status update")
 
             for attempt in range(1, 4):
-                print("waiting on url")
                 url: schemas.StartupData = await connection.receive()
                 self.logger.info("received the link")
-                auth_request = schemas.AuthRequest()
-                self.logger.info("send the auth request")
-                await connection.send(auth_request)
-                auth_data: schemas.AuthData = await connection.receive()
-                url, username, password = url.url, auth_data.username, auth_data.password
                 try:
-                    await self.tapis_init(link=url, username=username, password=password, connection=connection)
-                except exceptions.InvalidCredentialsReceived as e:
+                    #await self.run_command(connection, {'command':'switch_service', 'link':url.url, 'verbose':False})
+                    await self.aggregate_command_map['switch_service'](link=url.url, connection=connection, server=self, verbose=False)
+                    self.logger.info("Verification success")
+                    break
+                except ValueError as e:
                     login_failure_data = schemas.ResponseData(response_message = (str(e), attempt))
                     await connection.send(login_failure_data)
                     self.logger.warning(f"Verification failure, {e}")
                     if attempt == 3:  
                         self.logger.error(
                             "Attempted verification too many times. Exiting")
-                        raise exceptions.InvalidCredentialsReceived(self.handshake, "tapis auth")
+                        raise ValueError("auth failure")
                     continue
-                self.commands_initializer()
-                self.logger.info("Verification success")
-                break
         else:
             self.configure_decorators(self.username, self.password)
         self.initial = False
         startup_result = schemas.StartupData(initial = self.initial, username = self.username, url = self.url)
         self.logger.info("Connection success")
         await connection.send(startup_result)
         self.logger.info("Final connection data sent")
@@ -93,22 +132,21 @@
     async def accept(self, reader, writer):
         """
         accept connection request and initialize communication with the client
         """  
         connection = serverConnection.ServerConnection(reader=reader, writer=writer)
         self.timeout_handler()
         ip, port= writer.transport.get_extra_info('socket').getsockname()
-        print(ip)
         if ip != socket.gethostbyname(socket.gethostname()):
             raise exceptions.UnauthorizedAccessError(ip)
         self.logger.info("Received connection request")
         try:
             await self.handshake(connection)
-        except exceptions.InvalidCredentialsReceived:
-            logger.warning("invalid credentials entered too many times. Cancelling request")
+        except ValueError:
+            self.logger.warning("invalid credentials entered too many times. Cancelling request")
             await connection.close()
             return
 
         self.logger.info("connection is running now")
         loop = asyncio.get_event_loop()
         await loop.create_task(self.receive_and_execute(connection))
 
@@ -116,32 +154,14 @@
     def timeout_handler(self):  
         """
         checks if the timeout has been exceeded
         """
         if time.time() > self.end_time: 
             raise exceptions.TimeoutError
 
-    async def run_command(self, connection, command_data: dict):
-        """
-        process and run command based on received kwargs
-        """
-        command_data['connection'] = connection
-        command_group = command_data['command_group']
-        if command_group in self.command_group_map:
-            command_group = self.command_group_map[command_group]
-            return await command_group(**command_data)
-        elif command_group in self.command_map:
-            command = self.command_map[command_group]
-            command_data = self.filter_kwargs(command, command_data)
-            if command_data:
-                return await command(**command_data)
-            return await command()
-        else:
-            raise exceptions.CommandNotFoundError(command_group)
-
     async def receive_and_execute(self, connection):
         """
         receive and process commands
         """
         while True:
             try:
                 message = await connection.receive()
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/decorators.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,205 +1,193 @@
 """
 DECORATORS
 These decorators are used in the tapisObjectWrappers.py file to standardize special functions. Allows for increased code reusability
 """
 import typing
+import enum
 import sys
 import time
+import abc
+import socket
 from functools import update_wrapper, partial
 try:
-    from . import helpers
+    from . import killableThread
     from . import schemas
     from . import socketOpts
     from . import exceptions
 except:
-    import utilities.helpers as helpers
-    import utilities.schemas as schemas
-    import utilities.socketOpts as socketOpts
-    import utilities.exceptions as exceptions
-
+    import killableThread
+    import schemas
+    import socketOpts
+    import exceptions
+    
 
-class BaseRequirementDecorator(helpers.OperationsHelper):
+class BaseRequirementDecorator(abc.ABC):
     username: typing.Optional[str] = None
     password: typing.Optional[str] = None
-    def __init__(self, func: typing.Callable):
-        update_wrapper(self, func)
-        self.function = func
-        self.__code__ = func.__code__
-        self.__doc__ = func.__doc__
-        self.__name__ = func.__name__
-    
-    def __get__(self, obj, objtype): 
-        """Support instance methods."""
-        part = partial(self.__call__, obj)
-        part.__code__ = self.__code__
-        part.__doc__ = self.__doc__
-        part.__name__ = self.__name__
-        return part
-    
-    def __repr__(self):
-        return str(self.function)
-    
-    def __str__(self):
-        return str(self.function)
+
+    @abc.abstractmethod
+    async def __call__(self, command: typing.Type[object], connection: socket.socket, *args, **kwargs):
+        pass
 
 
 class RequiresForm(BaseRequirementDecorator):
     """
     This is for when you want to request separate input for specific command parameters instead of taking directly from the original command input (kwargs)
     Takes the parameters list of the function in question, filters out the ones that were not received from the original request message, sends another message 
     to request the unreceived parameters, and receives a message in response from the client to execute the function
     """
-    async def __call__(self, obj, *args, **kwargs):
-        if kwargs['connection']:
-            connection = kwargs['connection']
-            fields = list(helpers.get_parameters(self.function))
-            for key, value in kwargs.items():
-                if value or value == False:
-                    fields.remove(key)
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        if connection and not kwargs['file']:
+            connection = connection
+            fields = command.keyword_arguments
             if not fields:
-                raise AttributeError(f"The decorated function {self.function} has no parameters.")
+                raise AttributeError(f"The decorated function {command} has no keyword parameters.")
             form_request = schemas.FormRequest(arguments_list=fields)
             await connection.send(form_request)
-            filled_form: schemas.FormResponse = await connection.receive().arguments_list
-            for key, value in filled_form.items():
+            filled_form: schemas.FormResponse = await connection.receive()
+            for key, value in filled_form.arguments_list.items():
                 kwargs[key] = value
 
-        return await self.function(obj, **kwargs)
+        return await command.run(**kwargs)
 
 
 class RequiresExpression(BaseRequirementDecorator):
     """
     This is for when you have something like a Neo4j or postgres interface to add to the tapisObjectWrappers file. Writing a Neo4j query directly in a command is cumbersome, its much
     easier to do if you have a blank, multiline environment to write. This will send a request for an expression, if an expression parameter exists in the decorated function.
     The client will open a new interface to type the expression. This is then sent back and fed to the function
     """
-    async def __call__(self, obj, *args, **kwargs):
-        if kwargs['connection']:
-            connection = kwargs['connection']
-            fields = list(helpers.get_parameters(self.function))
-            if 'expression' not in fields:
-                raise AttributeError(f"The function {self.function} does not contain an 'expression' parameter")
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        if connection:
+            connection = connection
+            if 'expression' not in command.keyword_arguments:
+                raise AttributeError(f"The function {command} does not contain an 'expression' keyword parameter")
             form_request = schemas.FormRequest(arguments_list=[])
             await connection.send(form_request)
             filled_form: schemas.FormResponse = await connection.receive()
             kwargs['expression'] = filled_form.arguments_list
 
-        return await self.function(obj, **kwargs)
+        return await command.run(**kwargs)
     
 
 class SecureInput(BaseRequirementDecorator):
     """
     Use this for functions where you need to hide input while typing into the cli. For instance, if you want to add a password to a service, as a user, but you dont actually
     want to authenticate. Checks if the decorated function has a password parameter, then requests secure input of a new password from the client
     """
-    async def __call__(self, obj, *args, **kwargs):
-        if kwargs['connection']:
-            connection = kwargs['connection']
-            fields = list(helpers.get_parameters(self.function))
-            if 'password' in fields:
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        if connection:
+            connection = connection
+            if 'password' in command.keyword_arguments:
                 secure_input_request = schemas.AuthRequest(secure_input=True)
                 await connection.send(secure_input_request)
                 secure_input_data: schemas.AuthData = await connection.receive()
                 kwargs['password'] = secure_input_data.password
-                return await self.function(obj, **kwargs)
-            raise AttributeError(f"The function {self.function} does not contain a 'password' parameter to securely input")
-        return await self.function(obj, **kwargs)
+                return await command.run(**kwargs)
+            raise AttributeError(f"The function {command} does not contain a 'password' parameter to securely input")
+        return await command.run(**kwargs)
 
 
 class Auth(BaseRequirementDecorator):
     """
     used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
     the client, and checks those credentials against the stored credentials in the server.
     """
-    async def __call__(self, obj, *args, **kwargs):
-        no_username = False
-        if kwargs['connection']:
-            connection = kwargs['connection']
-            if self.function.__name__ == 'tapis_init' and kwargs['username'] and kwargs['password']:
-                return await self.function(obj, **kwargs)
-            fields = list(helpers.get_parameters(self.function))
-            if kwargs['username']:
-                no_username = True
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        requires_username = True
+        if connection:
+            if 'password' not in command.keyword_arguments:
+                raise AttributeError(f"The command {command.__class__.__name__} does not have a 'password' keyword argument")
+            if 'username' not in command.keyword_arguments:
                 auth_request = schemas.AuthRequest(requires_username=False)
+                requires_username = False
             else:
                 auth_request = schemas.AuthRequest()
             await connection.send(auth_request)
-            auth_data: schemas.AuthData = await connection.receive()
-            if 'username' in fields and 'password' in fields and not no_username:
-                kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
-                return await self.function(obj, **kwargs)
-            elif 'password' in fields and no_username:
-                kwargs['password'] = auth_data.password
-            username, password = auth_data.username, auth_data.password
-            if username != BaseRequirementDecorator.username:
-                raise exceptions.InvalidCredentialsReceived(self.function, 'username')
-            elif password != BaseRequirementDecorator.password:    
-                raise exceptions.InvalidCredentialsReceived(self.function, 'password')
-
-        return await self.function(obj, **kwargs)
+            auth_data = await connection.receive()
+            if auth_data.password != self.password and self.password:
+                raise ValueError("The provided password does not match the stored password")
+            if ((requires_username and auth_data.username != self.password) or (not requires_username and kwargs['username'] != self.username)) and self.username:
+                raise ValueError("The provided username does not match the stored username")
+            print(kwargs)
+            kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
+            return await command.run(**kwargs)
+        return await command.run(**kwargs)
 
 
 class NeedsConfirmation(BaseRequirementDecorator):
     """
     add to functions that you want user confirmation to exit. If you accidentally enter a command to delete a pod, this will not let you until you confirm
     """
-    async def __call__(self, obj, *args, **kwargs):
-        if kwargs['connection']:
-            connection = kwargs['connection']
-            confirmation_request = schemas.ConfirmationRequest(message=f"YOU REQUESTED TO {self.function.__name__}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)")
+    async def __call__(self, command, *args, **kwargs):
+        connection = kwargs['connection']
+        if connection:
+            connection = connection
+            confirmation_request = schemas.ConfirmationRequest(message=f"YOU REQUESTED TO {command.__class__.__name__}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)")
             await connection.send(confirmation_request)
             confirmation_reply: schemas.ResponseData = await connection.receive()
             confirmed = confirmation_reply.response_message
             if not confirmed:
-                raise exceptions.NoConfirmationError(self.function)
-        return await self.function(obj, **kwargs)
+                raise exceptions.NoConfirmationError(command)
+        return await command.run(**kwargs)
+
 
+DECORATOR_LIST = [
+    NeedsConfirmation,
+    RequiresForm,
+    RequiresExpression,
+    SecureInput,
+    Auth
+]
     
 class DecoratorSetup:
     """
     for instantiation of the tapis wrappers, and the server, to set up decorators with user credentials and the socket connection. If you want to use the decorators in your class
     YOU WILL NEED TO USE THIS!
     """
     def configure_decorators(self, username, password):
-        BaseRequirementDecorator.username = username
-        BaseRequirementDecorator.password = password
-    
+        self.username = username
+        self.password = password
+
 
 class AnimatedLoading:
     """
     Add this if you want to print a loading animation while a function is executing
     """
     def __init__(self, func: typing.Callable):
         update_wrapper(self, func)
-        self.function = func
+        self.func = func
         self.__code__ = func.__code__
         self.animation_frames = ['|','/','-','\\']
 
     def __get__(self, obj, objtype):
         """Support instance methods."""
         return partial(self.__call__, obj)
 
     def __repr__(self):
-        return self.function
+        return self.func
     
     def __str__(self):
-        return str(self.function)
+        return str(self.func)
     
     def animation(self):
         while True:
             for frame in self.animation_frames:
-                sys.stdout.write(f'\rloading ' + frame)
-                sys.stdout.flush()
+                print(f"loading {frame}", end='', flush=True)
                 time.sleep(0.5)
     
     def __call__(self, obj, *args, **kwargs):
-        if not BaseRequirementDecorator.username:
-            animation_thread = helpers.KillableThread(target=self.animation)
-            animation_thread.start()
-            result = self.function(obj, *args, **kwargs)
-            sys.stdout.flush()
-            animation_thread.kill()
-            sys.stdout.flush()
-        else:
-            result = self.function(obj, *args, **kwargs)
-        return result
+        animation_thread = killableThread.KillableThread(target=self.animation)
+        animation_thread.start()
+        result = self.func(obj, *args, **kwargs)
+        animation_thread.kill()
+        print("", end='', flush=True)
+        return result
+    
+
+if __name__ == "__main__":
+    print(issubclass(RequiresExpression, BaseRequirementDecorator))
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     
 
 class NoConfirmationError(Exception):
     """
     raise error when no confirmation is given for a function that needs confirmation to continue
     """
     def __init__(self, function: typing.Callable):
-        super().__init__(f"Confirmation was not given to the function {function.__name__}")
+        super().__init__(f"Confirmation was not given to the function {function.__class__.__name__}")
 
 
 class InvalidCredentialsReceived(Exception):
     """
     raise error when the provided credentials fail
     """
     def __init__(self, function: typing.Callable, cred_type: str):
-        super().__init__(f"The {cred_type} provided for the command {function.__name__} was invalid")
+        super().__init__(f"The {cred_type} provided for the command {function.__class__.__name__} was invalid")
 
 
 class HelpDoesNotExist(AttributeError):
     """
     raise error when the program tries to extract help information from a method, but help is not found
     """
     def __init__(self, command_name):
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/schemas.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/socketOpts.py` & `TapisCL-ICICLE-0.0.5/TapisCLICICLE/utilities/socketOpts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import asyncio
 import typing
 import pydantic
 try:
     from . import schemas
 except:
-    import utilities.schemas as schemas
+    import schemas
 
 
 schema_types: dict = {
         'CommandData':schemas.CommandData,
         'AuthData':schemas.AuthData,
         'StartupData':schemas.StartupData,
         'ResponseData':schemas.ResponseData,
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.41
+Version: 0.0.5
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,18 +709,14 @@
 #### **Full Terminal Interface:**
 1. run ``python -m TapisCLICICLE``
 2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
 3. enter your username and password when prompted
 4. if all went well the console should open. You can run `help` to see command options
 5. to exit the application, run `exit`
 
-**Running Several Instances of Client**
-
-There are some situations a user might want to have 2 or more windows of the same command line app open. For instance, you might need to be reading a static help menu at the same time as you are typing commands. TapisCLICICLE provides this capability, however, with some caveats. Since each client utilizes the same application resources, some commands are blocking. This means that if you run something that asks for authentication, or run a query to postgres or neo4j, you will have to respond to application prompts before any other commands are executed on other active clients.
-
 #### **Bash Command Line:**
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
```

### Comparing `TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.5/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 LICENSE
 README.md
 pyproject.toml
 TapisCLICICLE/__init__.py
 TapisCLICICLE/__main__.py
-TapisCLICICLE/cli.py
-TapisCLICICLE/server.py
+TapisCLICICLE/serverRun.py
+TapisCLICICLE/client/__init__.py
+TapisCLICICLE/client/cli.py
+TapisCLICICLE/client/connectionInitializer.py
+TapisCLICICLE/client/formatters.py
+TapisCLICICLE/client/handlers.py
+TapisCLICICLE/client/parsers.py
 TapisCLICICLE/commands/__init__.py
-TapisCLICICLE/commands/apps.py
-TapisCLICICLE/commands/baseWrappers.py
-TapisCLICICLE/commands/files.py
-TapisCLICICLE/commands/pods.py
-TapisCLICICLE/commands/query.py
+TapisCLICICLE/commands/appCommands.py
+TapisCLICICLE/commands/baseCommand.py
+TapisCLICICLE/commands/commandMap.py
+TapisCLICICLE/commands/dataFormatters.py
+TapisCLICICLE/commands/fileCommands.py
+TapisCLICICLE/commands/podCommands.py
 TapisCLICICLE/commands/serverCommands.py
-TapisCLICICLE/commands/systems.py
+TapisCLICICLE/commands/systemCommands.py
+TapisCLICICLE/commands/query/__init__.py
+TapisCLICICLE/commands/query/neo4j.py
+TapisCLICICLE/commands/query/postgres.py
+TapisCLICICLE/server/__init__.py
+TapisCLICICLE/server/server.py
+TapisCLICICLE/server/serverConnection.py
 TapisCLICICLE/utilities/__init__.py
 TapisCLICICLE/utilities/args.py
 TapisCLICICLE/utilities/decorators.py
 TapisCLICICLE/utilities/exceptions.py
-TapisCLICICLE/utilities/helpers.py
+TapisCLICICLE/utilities/killableThread.py
 TapisCLICICLE/utilities/logger.py
 TapisCLICICLE/utilities/schemas.py
-TapisCLICICLE/utilities/serverConnection.py
 TapisCLICICLE/utilities/socketOpts.py
 TapisCL_ICICLE.egg-info/PKG-INFO
 TapisCL_ICICLE.egg-info/SOURCES.txt
 TapisCL_ICICLE.egg-info/dependency_links.txt
 TapisCL_ICICLE.egg-info/entry_points.txt
 TapisCL_ICICLE.egg-info/requires.txt
 TapisCL_ICICLE.egg-info/top_level.txt
```

### Comparing `TapisCL-ICICLE-0.0.41/pyproject.toml` & `TapisCL-ICICLE-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.41"
+version = "0.0.5"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

