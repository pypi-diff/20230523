# Comparing `tmp/changedetector-0.6.1.tar.gz` & `tmp/changedetector-0.6.2.tar.gz`

## Comparing `changedetector-0.6.1.tar` & `changedetector-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,18 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/GLOBALS.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/__init__.py
--rw-r--r--   0        0        0    16477 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/detectchange.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/makeParser.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/menu.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/versionControl.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/wrapperComponents.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/wrm.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/wro.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/wrs.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/wtch.py
--rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/scripts/detectchange.fish
--rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/scripts/detectchange.sh
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/TEST.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/attrDatas.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/requirements.txt
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/test.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/testfile.c
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/testfile.cpp
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/testfile.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/testfile.rb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 changedetector-0.6.1/changedetector/tests/testfile.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 changedetector-0.6.1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.1/LICENCE
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.1/README.md
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 changedetector-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 changedetector-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/__init__.py
+-rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/detectchange.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/gobals_variables.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/makeParser.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/menu.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/versionControl.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wrapperComponents.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wrm.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wro.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wrs.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/wtch.py
+-rwxr-xr-x   0        0        0     1558 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/scripts/detectchange.fish
+-rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 changedetector-0.6.2/changedetector/scripts/detectchange.sh
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 changedetector-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 changedetector-0.6.2/LICENCE
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 changedetector-0.6.2/README.md
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 changedetector-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 changedetector-0.6.2/PKG-INFO
```

### Comparing `changedetector-0.6.1/changedetector/__init__.py` & `changedetector-0.6.2/changedetector/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 CHANGE DETECTOR
 ~~~~~~~~~~~~~~~
 This module detect all the change in a selected directory.
 And execute a program chosen on saved changes. (Python, Ruby, C++)
 Two modes of execution are available to you:
-    * Based on observing a specific file for changes and executing another file. (Watch and Run Other) `WRO`
-    * Observing a certain file and using the same file to conduct the test. (Watch and Run Self) `WRS`
+    * Based on observing a specific file for changes
+      and executing another file. (Watch and Run Other) `WRO`
+    * Observing a certain file and using the same file to
+      conduct the test. (Watch and Run Self) `WRS`
 
 
 :copyright (c) 2023 LuxLuth
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = "changedetector"
 __author__ = "LuxLuth"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2023 LuxLuth"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
```

### Comparing `changedetector-0.6.1/changedetector/detectchange.py` & `changedetector-0.6.2/changedetector/detectchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,82 @@
-import time
-import os
-import sys
-from rich import print as rprint
-from rich.console import Console
-import typer
-
-from watchdog.observers import Observer
-from pyfiglet import Figlet
-
-# add the base directory to the path
-sys.path.append(os.path.dirname(os.path.realpath(__file__)))
-
+"""
+detectchange CLI module
+===
+"""
 from menu import menu
 from wrapperComponents import WrapperComponents as wp
 from makeParser import Parser
 
 # handlers
 from wrs import WrsHandler
 from wro import WroHandler
 from wtch import WatchForHandler
 from wrm import WrmHandler
 
 # Version Control
 from versionControl import VersionControl
-from GLOBALS import VARS as v
+from gobals_variables import VARS as v
+
+import time
+import os
+
+import sys
+from rich import print as rprint
+from rich.console import Console
+import typer
+
+from watchdog.observers import Observer
+from pyfiglet import Figlet
 import tomli
 
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 
 class Entries:
-    def __init__(self):
+    """
+    Save all the data values
+    """
+    def __init__(self, is_empty=False):
         self.entries = {}
         self.c = Console()
+        self.is_empty = is_empty
 
     def add(self, name: str, value):
+        """Add a new element"""
         self.entries[name] = value
 
     def get(self, name: str) -> str | list | None | bool | int | list[str]:
+        """Get an Element"""
         return self.entries.get(name, None)
 
     def makeMode(self):
+        """Function to get the running mode"""
         MODE = menu(
             "Choose the mode you want to use:",
             "select",
-            [("Watch and Run Self (WRS)", "wrs"), ("Watch and Run Other (WRO)", "wro"), ("Makefile", "mk")],
+            [("Watch and Run Self (WRS)", "wrs"),
+             ("Watch and Run Other (WRO)", "wro"),
+             ("Makefile", "mk")],
         )
         self.add("mode", MODE)
 
     def makeLang(self):
+        """Get the language"""
         self.language = menu(
             "Choose the language you want to use:",
             "select",
             [("python", "python"), ("ruby", "ruby"), ("c", "c"), ("c++", "c++")],
         )
         self.add("lang", self.language)
 
     def makeCParams(self):
+        """Get C parameters"""
         wywu = wp.textWrapBold("Enter the compiler name you want to use : ")
         ccho = wp.textWrapBold("( g++ | gcc | ...) ", "green")
         CMD = self.c.input(f"{wywu}{ccho}")
-        self.add("cmd", CMD)
+        self.add("cmd", [CMD])
         opt1 = wp.textWrapBold("Enter flags you want to use : ")
         default = wp.textWrapBold("(none) ", "green")
         FLAGS = self.c.input(f"{opt1}{default}").split(" ")
         if FLAGS in ["none", "", " "]:
             FLAGS = [""]
         self.add("flags", FLAGS)
         output = wp.textWrapBold("Enter the output attributes you want to use: ")
@@ -75,14 +89,15 @@
         default = wp.textWrapBold("(out) ", "green")
         OUTPUT_FILE = self.c.input(f"{output_name}{default}").lower()
         if OUTPUT_FILE in ["", " "]:
             OUTPUT_FILE = "out"
         self.add("output_file", OUTPUT_FILE)
 
     def makeCommand(self):
+        """Initialise Command array"""
         try:
             if self.language == "python":
                 CMD = ["py", "python3"]
                 self.add("cmd", CMD)
             elif self.language == "ruby":
                 CMD = ["ruby", "ruby"]
                 self.add("cmd", CMD)
@@ -96,14 +111,18 @@
             rprint(
                 f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrapBold('KeyboardInterrupt')}"
             )
             sys.exit(1)
 
     def makePaths(self):
         BASE_DIR = os.getcwd()
+        FILE = ""
+        THE_FILE = ""
+        FILE_TO_WATCH = ""
+        THE_FILE_TO_WATCH = ""
         self.add("base_dir", BASE_DIR)
         try:
             if self.get("mode") != "mk":
                 if self.get("lang") == "python":
                     # print(python_files)
                     FILE = menu("Choose the file you want to run:", "file")
                 elif self.get("lang") == "ruby":
@@ -121,15 +140,16 @@
                     # print(all_files)
                     FILE_TO_WATCH = menu("Choose the file you want to watch:", "file")
             else:
                 p = Parser()
                 cmds = p.parse()
                 if len(cmds) == 0:
                     rprint(
-                        f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrapBold('No make command found')}"
+                        f"{wp.textWrapBold('Error: ', 'red')} \
+                        {wp.textWrapBold('No make command found')}"
                     )
                     sys.exit(1)
                 choices = [(c, c) for c in cmds]
                 MK_TO_RUN = menu("Choose the make command to run:", "select", choices)
                 self.add("mk_cmd", MK_TO_RUN)
 
                 FILE_TO_WATCH = menu("Choose the file you want to watch:", "file")
@@ -137,19 +157,20 @@
                 # sys.exit(0)
 
         except KeyboardInterrupt:
             rprint(
                 f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrapBold('KeyboardInterrupt')}"
             )
             sys.exit(1)
+        _base = str(self.get("base_dir"))
         if self.get("mode") != "mk":
-            THE_FILE = os.path.join(self.get("base_dir"), f"{FILE}")
+            THE_FILE = os.path.join(_base, f"{FILE}")
             self.add("the_file", THE_FILE)
         if self.get("mode") in ["wro", "mk"]:
-            THE_FILE_TO_WATCH = os.path.join(self.get("base_dir"), f"{FILE_TO_WATCH}")
+            THE_FILE_TO_WATCH = os.path.join(_base, f"{FILE_TO_WATCH}")
             self.add("the_file_to_watch", THE_FILE_TO_WATCH)
         if self.get("mode") != "mk":
             rprint(self.get("the_file"))
         # Check if the file's path is valid exist
         if self.get("mode") != "mk":
             if not os.path.exists(THE_FILE):
                 err = wp.textWrapBold(f"The file {THE_FILE} doesn't exist", "red")
@@ -162,28 +183,35 @@
                 f"The file {THE_FILE_TO_WATCH} doesn'tOUTPUT_FILE exist", "red"
             )
             rprint(f"❌ {err}")
             sys.exit(1)
 
         self.make_command_list()
 
-    def make_command_list(self):
+    def make_command_list(self) -> list[str]:
+        COMMAND_LIST: list[str] = []
         if self.get("lang") in ["c++", "c"]:
-            COMMAND_LIST = [self.get("cmd")]
-            if self.get("flags")[0] != "":
-                COMMAND_LIST.extend(iter(self.get("flags")))
-            COMMAND_LIST.append(self.get("the_file"))
-            COMMAND_LIST.append(self.get("output_attr"))
-            COMMAND_LIST.append(self.get("output_file"))
-            self.add("command_list", COMMAND_LIST)
+            _cmd : list[str]= []
+            _c = self.get("cmd")
+            if isinstance(_c, list): _cmd = _c
+            COMMAND_LIST = [*_cmd]
+            _flags = self.get("flags")
+            if isinstance(_flags, list):
+                if _flags[0] != "":
+                    COMMAND_LIST += [*_flags]
+                COMMAND_LIST.append(str(self.get("the_file")))
+                COMMAND_LIST.append(str(self.get("output_attr")))
+                COMMAND_LIST.append(str(self.get("output_file")))
+                self.add("command_list", COMMAND_LIST)
         elif self.get("mode") == "mk":
-            COMMAND_LIST = ["make", self.get("mk_cmd")]
+            COMMAND_LIST = ["make", str(self.get("mk_cmd"))]
             self.add("command_list", COMMAND_LIST)
         else:
             self.add("command_list", None)
+        return COMMAND_LIST
 
     def make(self):
         self.makeMode()
         if self.get("mode") != "mk":
             self.makeLang()
             self.makeCommand()
             self.makePaths()
@@ -194,47 +222,49 @@
         return str(self.entries)
 
     def __repr__(self):
         return str(self.entries)
 
 
 class BeautifulOutput:
-    def __init__(self, e: Entries = None) -> None:
-        self.lang = e.get("lang") if e else None
-        self.mode = e.get("mode") if e else None
-        self.the_file = e.get("the_file") if e else None
-        self.the_file_to_watch = e.get("the_file_to_watch") if e else None
+    def __init__(self, e: Entries =Entries(True)) -> None:
+        self.lang = e.get("lang") if not e.is_empty else None
+        self.mode = e.get("mode") if not e.is_empty else None
+        self.the_file = str(e.get("the_file"))
+        self.the_file_to_watch = str(e.get("the_file_to_watch"))
 
 
     def _start(self):
         os.system("cls" if os.name == "nt" else "clear")
         f = Figlet(font="colossal", width=80)
         print(f.renderText("Change"))
         print(f.renderText("Detect"))
 
     def _out(self, lang: str):
-        if v.verbose:
+        if v.verbose == True:
             custom_fig = Figlet(font="colossal")
             print(custom_fig.renderText(lang))
             if self.mode != "mk":
                 rprint(
                     f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file)}"
                 )
             else:
                 rprint(
-                    f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file_to_watch)}"
+                    f"{wp.textWrapBold('[FILE] ')}\
+                        {wp.format_file_path_link(self.the_file_to_watch)}"
                 )
         else:
             if self.mode != "mk":
                 rprint(
                     f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file)}"
                 )
             else:
                 rprint(
-                    f"{wp.textWrapBold('[FILE] ')}{wp.format_file_path_link(self.the_file_to_watch)}"
+                    f"{wp.textWrapBold('[FILE] ')}\
+                        {wp.format_file_path_link(self.the_file_to_watch)}"
                 )
 
     def _run(self):
         # clear the terminal
         os.system("cls" if os.name == "nt" else "clear")
         if self.lang in ["ruby", "rb"]:
             self._out("Ruby")
@@ -248,102 +278,117 @@
             self._out("Makefile")
 
     def __str__(self):
         return f"BeautifulOutput({self.lang}, {self.the_file})"
 
 
 class _Watcher:
-    def __init__(self, handler_type: WrsHandler, dir_to_watch: str = os.getcwd()):
+    def __init__(
+            self,
+            handler_type: WrsHandler | WrmHandler | WroHandler | WatchForHandler,
+            dir_to_watch: str = os.getcwd()
+        ):
         self.DIRECTORY_TO_WATCH = dir_to_watch
         self.observer = Observer()
         self.handler_type = handler_type
 
     def run(self):
         event_handler = self.handler_type
         self.observer.schedule(event_handler, self.DIRECTORY_TO_WATCH, recursive=True)
         self.observer.start()
         try:
             while True:
                 time.sleep(5)
-        except Exception or KeyboardInterrupt as e:
+        except Exception as e:
             self.observer.stop()
-            rprint(f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap(e)}")
+            rprint(f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap(str(e))}")
 
-    def runFor(self, seconds: int):
+    def runFor(self, seconds: float):
         event_handler = self.handler_type
         self.observer.schedule(event_handler, self.DIRECTORY_TO_WATCH, recursive=True)
         self.observer.start()
         try:
             time.sleep(seconds + 3)
             self.observer.stop()
-        except Exception or KeyboardInterrupt as e:
+        except Exception as e:
             self.observer.stop()
-            rprint(f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap(e)}")
+            rprint(f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap(str(e))}")
 
         self.observer.join()
 
 
 def activate() -> None:
     """
     ACTIVATE
     --------
     Detect change in the working directory and execute the program chosen.
     Two modes of execution are available to you:
-            * Based on observing a specific file for changes and executing another file. (Watch and Run Other) `WRO`
-            * Observing a certain file and using the same file to conduct the test. (Watch and Run Self) `WRS`
+            * Based on observing a specific file for changes
+              and executing another file. (Watch and Run Other) `WRO`
+            * Observing a certain file and using the same file
+              to conduct the test. (Watch and Run Self) `WRS`
     """
 
     BeautifulOutput()._start()
 
     try:
         e = Entries()
         e.make()
-
+        _the_file = str(e.get("the_file"))
+        _cmd_list: list[str] = []
+        _tmp = e.get("command_list")
+        if isinstance(_tmp, list): _cmd_list = _tmp
+        _lang = str(e.get("lang"))
+        _base_dir = str(e.get("base_dir"))
+        _cmd: list[str] = []
+        _tmp = e.get("cmd")
+        if isinstance(_tmp, list): _cmd = _tmp
+        wh: WrsHandler | WrmHandler | WroHandler | WatchForHandler
         if e.get("mode") == "wrs":
             wh = WrsHandler(
-                the_file=e.get("the_file"),
-                command_list=e.get("command_list"),
-                language=e.get("lang"),
-                base_dir=e.get("base_dir"),
-                cmd=e.get("cmd"),
+                the_file=_the_file,
+                command_list=_cmd_list,
+                language=_lang,
+                base_dir=_base_dir,
+                cmd=_cmd,
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(WRS)", "green")
         elif e.get("mode") == "wro":
             wh = WroHandler(
-                the_file=e.get("the_file"),
-                the_file_to_watch=e.get("the_file_to_watch"),
-                command_list=e.get("command_list"),
-                language=e.get("lang"),
-                base_dir=e.get("base_dir"),
-                cmd=e.get("cmd"),
+                the_file=_the_file,
+                the_file_to_watch=str(e.get("the_file_to_watch")),
+                command_list=_cmd_list,
+                language=_lang,
+                base_dir=_base_dir,
+                cmd=_cmd,
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(WRO)", "green")
         else:
             wh = WrmHandler(
-                the_file_to_watch=e.get("the_file_to_watch"),
-                command_list=e.get("command_list")
+                the_file_to_watch=str(e.get("the_file_to_watch")),
+                command_list=_cmd_list
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(MAKEFILE)", "green")
 
-        w = _Watcher(wh, e.get("base_dir"))
+        w = _Watcher(wh, str(e.get("base_dir")))
         print(" ")
         rprint(f"Watching in {mode} mode...")
         print(" ")
         w.run()
     except KeyboardInterrupt:
         # pipe the error number to the shell
         rprint(
             f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap('Keyboard Interrupt')}"
         )
         sys.exit(0)
 
-def make_path(base_dir: str, file: str) -> str:
+def make_path(base_dir: str, file: str) -> str | None:
     if file == None:
         return None
     if file.startswith(f".{os.sep}"):
         file = file[2:]
     return os.path.join(base_dir, file)
 
 def cfg_activate() -> None:
@@ -362,26 +407,28 @@
     with open(".detectchange", "rb") as f:
         config = tomli.load(f)
 
     mode = config.get("mode", "wrs")
     lang = config.get("lang", "python")
     the_file = make_path(os.getcwd(), config.get("file", "main.py"))
     the_file_to_watch = make_path(os.getcwd(), config.get("file_to_watch", None))
+    cmd: list[str] = []
+    wh: WrsHandler | WrmHandler | WroHandler | WatchForHandler
     verbose = config.get("verbose", False)
     if lang in ["python", "py", "python3"]:
         cmd = config.get("cmd", ["py", "python3"])
     elif lang in ["ruby", "rb"]:
         cmd = config.get("cmd", ["ruby", "ruby"])
     c = config.get("c", {})
     if lang in ["c", "c++", "cpp"]:
         cmd = c.get("cc", None)
     flags = c.get("cflags", " ").split(" ")
     output_attr = c.get("output_attr", "-o")
     output_file = make_path(os.getcwd(), c.get("output", "a.out"))
-    if cmd is None and lang in ["c", "c++", "cpp"]:
+    if len(cmd) == 0 and lang in ["c", "c++", "cpp"]:
         rprint(
             f"{wp.textWrapBold('Error: ', 'red')}{wp.textWrap('No C compiler found')}"
         )
         sys.exit(1)
 
     try:
         e = Entries()
@@ -390,31 +437,32 @@
         e.add("the_file", the_file)
         e.add("the_file_to_watch", the_file_to_watch)
         e.add("base_dir", base_dir)
         e.add("cmd", cmd)
         e.add("flags", flags)
         e.add("output_attr", output_attr)
         e.add("output_file", output_file)
-        e.make_command_list()
-        v.verbose = verbose
+        cmd_list = e.make_command_list()
+        v._verbose = verbose
+
         if mode == "wrs":
             wh = WrsHandler(
-                the_file=the_file,
-                command_list=e.get("command_list"),
+                the_file=str(the_file),
+                command_list=cmd_list,
                 language=lang,
                 base_dir=base_dir,
                 cmd=cmd,
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(WRS)", "green")
         else:
             wh = WroHandler(
-                the_file=the_file,
-                the_file_to_watch=the_file_to_watch,
-                command_list=e.get("command_list"),
+                the_file=str(the_file),
+                the_file_to_watch=str(the_file_to_watch),
+                command_list=cmd_list,
                 language=lang,
                 base_dir=base_dir,
                 cmd=cmd,
             )
             BeautifulOutput(e)._run()
             mode = wp.textWrapBold("(WRO)", "green")
         w = _Watcher(wh, base_dir)
@@ -483,17 +531,17 @@
         False,
         "--config",
         "-c",
         help="Use the `.detectchange` config file when you launch the program with this flag"
     ),
 ):
     if verbose:
-        v.verbose = True
+        v._verbose = True
     else:
-        v.verbose = False
+        v._verbose = False
     if config:
         cfg_activate()
     else:
         activate()
 
 
 if __name__ == "__main__":
```

### Comparing `changedetector-0.6.1/changedetector/makeParser.py` & `changedetector-0.6.2/changedetector/makeParser.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/changedetector/menu.py` & `changedetector-0.6.2/changedetector/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import sys
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 from InquirerPy.validator import PathValidator
 from rich import print as rprint
 from wrapperComponents import WrapperComponents as wp
 import os
+from typing import Any
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__))
 THEMES_DIR = os.path.join(BASE_DIR, "themes")
 THEME = os.path.join(THEMES_DIR, "inquirer.json")
 
 
-def read_file(file_path: str) -> list:
+def read_file(file_path: str) -> str:
     """
     Reads a file and returns a list of lines.
     :param file_path: The path to the file.
     :return: A list of lines.
     """
     with open(file_path, "r") as file:
         return file.read()
 
 
-def make_choices(options: list[tuple[str, any]]) -> list[Choice]:
+def make_choices(options: list[tuple[str, Any]] | None) -> list[Choice]:
     """
     Makes a list of choices for the menu.
     :param options: The options to make choices from.
     :return: A list of choices.
     """
-    choices = []
-    for option in options:
-        choices.append(Choice(name=option[0], value=option[1]))
+    choices: list[Choice] = []
+    if options:
+        for option in options:
+            choices.append(Choice(name=option[0], value=option[1]))
     return choices
 
 
+
 def menu(
-    title: str, mode="select", options: list[tuple[str, any]] = None, base_path=None
+    title: str, mode="select", options: list[tuple[str, Any]] | None = None, base_path=None
 ):
     """
     A simple menu for the user to choose from.
     :param title: The title of the menu.
     :param mode: The type of menu to use.
     :param options: The options the user can choose from.
     :param base_path: The base path to use for the file menu.
@@ -60,15 +63,15 @@
                 message=title,
                 default=home_path,
                 validate=PathValidator(is_file=True, message="Input is not a file"),
                 only_files=True,
             ).execute()
 
     except Exception as e:
-        rprint(f"{wp.textWrapBold('An error occured: ', 'red')}{wp.textWrap(e, 'red')}")
+        rprint(f"{wp.textWrapBold('An error occured: ', 'red')}{wp.textWrap(str(e), 'red')}")
         rprint(f"{wp.textWrapBold('Exiting program...', 'red')}")
         sys.exit(1)
     return res
 
 
 if __name__ == "__main__":
     MODE = menu(
```

### Comparing `changedetector-0.6.1/changedetector/versionControl.py` & `changedetector-0.6.2/changedetector/versionControl.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/changedetector/wrapperComponents.py` & `changedetector-0.6.2/changedetector/wrapperComponents.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from os import sep
 
 
 class WrapperComponents:
     @staticmethod
-    def textWrap(text, color: str = "white", bold=False) -> str:
+    def textWrap(text: str, color: str = "white", bold=False) -> str:
         return f"[{color}][b]{text}[/b][/]" if bold else f"[{color}]{text}[/]"
 
     @staticmethod
-    def textWrapBold(text, color: str = "white") -> str:
+    def textWrapBold(text: str, color: str = "white") -> str:
         return WrapperComponents.textWrap(text, color, bold=True)
 
     @staticmethod
-    def textWrapUnderline(text, color: str = "white", bold=False) -> str:
+    def textWrapUnderline(text: str, color: str = "white", bold=False) -> str:
         return f"[{color}][u]{text}[/u][/]" if bold else f"[{color}][u]{text}[/u][/]"
 
     @staticmethod
-    def textWrapBoldUnderline(text, color: str = "white") -> str:
+    def textWrapBoldUnderline(text: str, color: str = "white") -> str:
         return WrapperComponents.textWrapUnderline(text, color, bold=True)
 
     @staticmethod
-    def link(text, link: str) -> str:
+    def link(text: str, link: str) -> str:
         return f"[link={link}]{text}[/link]"
 
     @staticmethod
     def format_file_path_link(file_path: str, color: str = "white") -> str:
         return WrapperComponents.textWrap(
             f"[link=file:{sep}{sep}{file_path}]{file_path}[/link]", color
         )
```

### Comparing `changedetector-0.6.1/changedetector/wrm.py` & `changedetector-0.6.2/changedetector/wrm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from watchdog.events import FileSystemEventHandler
 import subprocess
 import time
-import os
 from rich import print as rprint
 from wrapperComponents import WrapperComponents as wp
-from GLOBALS import VARS as v
+from gobals_variables import VARS as v
 
 
 class WrmHandler(FileSystemEventHandler):
     def __init__(
         self,
         the_file_to_watch: str,
         command_list: list[str],
@@ -19,39 +18,39 @@
         self.command_list = command_list
 
     def on_any_event(self, event):
         if event.is_directory:
             return None
 
         elif event.event_type == "created":
-            if v.verbose:
+            if v.verbose == True:
                 rprint(
                     f"{wp.textWrapBold('+ A', 'green')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                 )
 
         elif event.event_type == "modified":
             # Taken any action here when a file is modified.
             if event.src_path == self.the_file_to_watch:
                 print()
                 print("---")
                 now = time.perf_counter()
                 subprocess.call(self.command_list)
                 end = time.perf_counter()
-                if v.verbose:
+                if v.verbose == True:
                     print("---")
                     rprint(wp.textWrapBold(f"{round(end-now, 2)}s", "bright_magenta"))
 
                 print("---")
                 print(f"[{self.language}]", "Listening for changes...")
 
             else:
-                if v.verbose:
+                if v.verbose == True:
                     rprint(
                         f"{wp.textWrapBold('= M', 'green')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                     )
 
         elif event.event_type == "deleted":
             # Taken any action here when a file is deleted.
-            if v.verbose:
+            if v.verbose == True:
                 rprint(
                     f"{wp.textWrapBold('- D', 'red')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                 )
```

### Comparing `changedetector-0.6.1/changedetector/wro.py` & `changedetector-0.6.2/changedetector/wro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from watchdog.events import FileSystemEventHandler
 import subprocess
 import time
 import os
 from rich import print as rprint
 from wrapperComponents import WrapperComponents as wp
-from GLOBALS import VARS as v
+from gobals_variables import VARS as v
 
 
 class WroHandler(FileSystemEventHandler):
     def __init__(
         self,
         the_file: str,
         the_file_to_watch: str,
@@ -26,15 +26,15 @@
         self.cmd = cmd
 
     def on_any_event(self, event):
         if event.is_directory:
             return None
 
         elif event.event_type == "created":
-            if v.verbose:
+            if v.verbose == True:
                 rprint(
                     f"{wp.textWrapBold('+ A', 'green')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                 )
 
         elif event.event_type == "modified":
             # Taken any action here when a file is modified.
             if event.src_path == self.the_file_to_watch:
@@ -47,34 +47,34 @@
                     subprocess.call([cm, f"{self.the_file}"])
                     end = time.perf_counter()
                 else:
                     now = time.perf_counter()
                     subprocess.call(self.command_list)
                     rprint(self.command_list)
                     end = time.perf_counter()
-                if v.verbose:
+                if v.verbose == True:
                     print("---")
                     rprint(wp.textWrapBold(f"{round(end-now, 2)}s", "bright_magenta"))
 
                 print()
                 print("---")
                 print(f"[{self.language}]", "Listening for changes...")
             elif event.src_path == f"{self.base_dir}/detectchange.py":
-                if v.verbose:
+                if v.verbose == True:
                     rprint(
                         wp.textWrapBold(
                             "Detectchange.py has been modified. Please restart the program.",
                             "red",
                         )
                     )
             else:
-                if v.verbose:
+                if v.verbose == True:
                     rprint(
                         f"{wp.textWrapBold('= M', 'green')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                     )
 
         elif event.event_type == "deleted":
             # Taken any action here when a file is deleted.
-            if v.verbose:
+            if v.verbose == True:
                 rprint(
                     f"{wp.textWrapBold('- D', 'red')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                 )
```

### Comparing `changedetector-0.6.1/changedetector/wrs.py` & `changedetector-0.6.2/changedetector/wrs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from watchdog.events import FileSystemEventHandler
 import subprocess
 import time
 import os
 from rich import print as rprint
 from wrapperComponents import WrapperComponents as wp
-from GLOBALS import VARS as v
+from gobals_variables import VARS as v
 
 
 class WrsHandler(FileSystemEventHandler):
     def __init__(
         self,
         the_file: str,
         language: str,
@@ -24,15 +24,15 @@
         self.cmd = cmd
 
     def on_any_event(self, event):
         if event.is_directory:
             return None
 
         elif event.event_type == "created":
-            if v.verbose:
+            if v.verbose == True:
                 rprint(
                     f"{wp.textWrapBold('+ A', 'green')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                 )
 
         elif event.event_type == "modified":
             # Taken any action here when a file is modified.
             if event.src_path == self.the_file:
@@ -47,36 +47,36 @@
                 else:
                     now = time.perf_counter()
                     subprocess.call(self.command_list)
                     rprint(self.command_list)
                     end = time.perf_counter()
                     rprint(f"{wp.textWrapBold('COMPLILATON COMPLETED', 'green')}")
 
-                if v.verbose:
+                if v.verbose == True:
                     print("---")
                     rprint(
                         wp.textWrapBold(
                             f"Time taken: {round(end-now, 2)}s", "bright_magenta"
                         )
                     )
 
                 print()
                 print("---")
                 print(f"[{self.language}]", "Listening for changes...")
             elif event.src_path == f"{self.base_dir}/detectchange.py":
-                if v.verbose:
+                if v.verbose == True:
                     rprint(
                         wp.textWrapBold(
                             "Detectchange.py has been modified. Please restart the program.",
                             "red",
                         )
                     )
             else:
-                if v.verbose:
+                if v.verbose == True:
                     rprint(
                         f"{wp.textWrapBold('= M', 'green')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                     )
         elif event.event_type == "deleted":
-            if v.verbose:
+            if v.verbose == True:
                 rprint(
                     f"{wp.textWrapBold('- D', 'red')} {wp.textWrapBold(' - {}'.format(wp.format_file_path_link(event.src_path)))}"
                 )
```

### Comparing `changedetector-0.6.1/changedetector/wtch.py` & `changedetector-0.6.2/changedetector/wtch.py`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/changedetector/scripts/detectchange.fish` & `changedetector-0.6.2/changedetector/scripts/detectchange.fish`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/changedetector/scripts/detectchange.sh` & `changedetector-0.6.2/changedetector/scripts/detectchange.sh`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/LICENCE` & `changedetector-0.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/README.md` & `changedetector-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `changedetector-0.6.1/PKG-INFO` & `changedetector-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changedetector
-Version: 0.6.1
+Version: 0.6.2
 Summary: A basic change detector for the Python, Ruby and C++.
 Project-URL: Bug Tracker, https://github.com/luxluth/changedetector/issues
 Project-URL: Homepage, https://github.com/luxluth/changedetector
 Author-email: Lux Luth <luxusluth@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,37 +18,35 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Requires-Dist: blessed==1.20.0
-Requires-Dist: certifi==2022.12.7
+Requires-Python: >=3.7
+Requires-Dist: certifi==2023.5.7; python_version >= '3.6'
 Requires-Dist: charset-normalizer==3.1.0
-Requires-Dist: click==8.1.3
+Requires-Dist: click==8.1.3; python_version >= '3.7'
 Requires-Dist: colorama==0.4.6
-Requires-Dist: commonmark==0.9.1
-Requires-Dist: idna==3.4
+Requires-Dist: idna==3.4; python_version >= '3.5'
 Requires-Dist: inquirerpy==0.3.4
-Requires-Dist: pfzy==0.3.4
-Requires-Dist: prompt-toolkit==3.0.38
+Requires-Dist: markdown-it-py==2.2.0; python_version >= '3.7'
+Requires-Dist: mdurl==0.1.2; python_version >= '3.7'
+Requires-Dist: pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
+Requires-Dist: prompt-toolkit==3.0.38; python_full_version >= '3.7.0'
 Requires-Dist: pyfiglet==0.8.post1
-Requires-Dist: pygments==2.14.0
-Requires-Dist: python-editor==1.0.4
-Requires-Dist: readchar==4.0.5
-Requires-Dist: requests==2.28.2
-Requires-Dist: rich==12.6.0
-Requires-Dist: setuptools==67.6.1
+Requires-Dist: pygments==2.15.1; python_version >= '3.7'
+Requires-Dist: requests==2.31.0
+Requires-Dist: rich==13.3.5
 Requires-Dist: shellingham==1.5.0.post1
-Requires-Dist: six==1.16.0
 Requires-Dist: tomli==2.0.1
-Requires-Dist: typer[all]==0.7.0
-Requires-Dist: urllib3==1.26.15
+Requires-Dist: typer[all]==0.9.0
+Requires-Dist: typing-extensions==4.6.0; python_version >= '3.7'
+Requires-Dist: typing==3.7.4.3
+Requires-Dist: urllib3==2.0.2
 Requires-Dist: watchdog==3.0.0
 Requires-Dist: wcwidth==0.2.6
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # changedetector
```

