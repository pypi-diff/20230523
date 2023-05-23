# Comparing `tmp/pf_fpga_tools-0.0.5.tar.gz` & `tmp/pf_fpga_tools-0.0.6.tar.gz`

## Comparing `pf_fpga_tools-0.0.5.tar` & `pf_fpga_tools-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/.flake8
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/exceptions.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/utils.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/__main__.py
--rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/pfBuildCore.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/__main__.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/__main__.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/pfConvertImage.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/__main__.py
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/pfInstallCore.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfQuartusEdit/__main__.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
--rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/__main__.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/LICENSE
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/README.md
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/.flake8
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/exceptions.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/utils.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/__main__.py
+-rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/pfBuildCore.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/__main__.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/__main__.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/pfConvertImage.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/__main__.py
+-rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/pfInstallCore.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/__main__.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py
+-rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/__main__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/README.md
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.6/PKG-INFO
```

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/utils.py` & `pf_fpga_tools-0.0.6/pfFPGATools/utils.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/__main__.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfBuildCore/pfBuildCore.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfBuildCore/pfBuildCore.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,35 +29,33 @@
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         self.short_name: str = None
 
         try:
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hv', ['debug', 'help', 'version', 'corefilename', 'bitstreamfile', 'debug'])
+            opts, arguments = getopt.getopt(args, 'dhv', ['debug', 'help', 'version', 'corefilename', 'bitstreamfile'])
 
             print_core_filename: bool = False
             print_bitstream_file: bool = False
 
             for o, a in opts:
-                if o in ('--debug'):
+                if o in ('-d', '--debug'):
+                    # -- We ignore this argument because it was already dealt with in the calling main() code.
                     continue
                 elif o in ('-h', '--help'):
                     pfBuildCore.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfBuildCore.printVersion()
                     sys.exit(0)
                 elif o in ('--corefilename'):
                     print_core_filename = True
                 elif o in ('--bitstreamfile'):
                     print_bitstream_file = True
-                elif o in ('--debug'):
-                    # -- We ignore this argument because it was already dealt with in the calling main() code.
-                    continue
 
             nb_of_arguments: int = len(arguments)
             if print_core_filename is False and print_bitstream_file is False and nb_of_arguments != 2:
                 raise RuntimeError('Invalid arguments. Maybe start with `pfBuildCore --help?')
 
             self.config_filename: str = arguments[0]
 
@@ -328,13 +326,13 @@
         print('')
         print('usage: pfBuildCore <options> config_file destination_folder')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h          - Show a help message.')
         print('   --version/-v       - Display the app\'s version.')
-        print('   --debug            - Enable extra debugging information.')
+        print('   --debug/-d         - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfBuildCore v' + __version__ + ' 🛠️')
```

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/__main__.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfCloneCoreTemplate/pfCloneCoreTemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,19 @@
         """Constructor based on command line arguments."""
 
         try:
             self.branch_name = None
             self.tag_name = None
 
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hvb:t:', ['debug', 'help', 'version', 'branch=', 'tag='])
+            opts, arguments = getopt.getopt(args, 'dhvb:t:', ['debug', 'help', 'version', 'branch=', 'tag='])
 
             for o, a in opts:
-                if o in ('--debug'):
+                if o in ('-d', '--debug'):
+                    # -- We ignore this argument because it was already dealt with in the calling main() code.
                     continue
                 elif o in ('-h', '--help'):
                     pfCloneCoreTemplate.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfCloneCoreTemplate.printVersion()
                     sys.exit(0)
@@ -89,13 +90,13 @@
         print('')
         print('usage: pfCloneCoreTemplate <options> destination_folder')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h          - Show a help message.')
         print('   --version/-v       - Display the app\'s version.')
-        print('   --debug            - Enable extra debugging information.')
+        print('   --debug/-d         - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfCloneCoreTemplate v' + __version__ + ' 🛠️')
```

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/__main__.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfConvertImage/pfConvertImage.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfConvertImage/pfConvertImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,26 @@
     """A tool to install a zipped up core file onto a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hv', ['debug', 'help', 'version', 'debug'])
+            opts, arguments = getopt.getopt(args, 'dhv', ['debug', 'help', 'version'])
 
             for o, a in opts:
-                if o in ('--debug'):
+                if o in ('-d', '--debug'):
+                    # -- We ignore this argument because it was already dealt with in the calling main() code.
                     continue
                 elif o in ('-h', '--help'):
                     pfConvertImage.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfConvertImage.printVersion()
                     sys.exit(0)
-                elif o in ('--debug'):
-                    # -- We ignore this argument because it was already dealt with in the calling main() code.
-                    continue
 
             nb_of_arguments: int = len(arguments)
             if nb_of_arguments != 2:
                 raise RuntimeError('Invalid arguments. Maybe start with `pfConvertImage --help?')
 
             self.img_filename: str = arguments[0]
             self.bin_filename: str = arguments[1]
@@ -92,13 +90,13 @@
         print('')
         print('usage: pfConvertImage <options> src_filename dest_filename')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h          - Show a help message.')
         print('   --version/-v       - Display the app\'s version.')
-        print('   --debug            - Enable extra debugging information.')
+        print('   --debug/-d         - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfConvertImage v' + __version__ + ' 🛠️')
```

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/__main__.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfInstallCore/pfInstallCore.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfInstallCore/pfInstallCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,35 +28,35 @@
         try:
             self.name_of_core_to_delete: str = None
             self.volume_name: str = None
             self.zip_filename: str = None
             self.eject_after_install: bool = False
 
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hved:', ['debug', 'help', 'version', 'eject', 'delete='])
+            opts, arguments = getopt.getopt(args, 'dhver:', ['debug', 'help', 'version', 'eject', 'remove='])
 
             for o, a in opts:
-                if o in ('--debug'):
+                if o in ('-d', '--debug'):
+                    # -- We ignore this argument because it was already dealt with in the calling main() code.
                     continue
                 elif o in ('-h', '--help'):
                     pfInstallCore.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfInstallCore.printVersion()
-                    sys.exit(0)
                 elif o in ('-e', '--eject'):
                     self.eject_after_install = True
-                elif o in ('-d', '--delete'):
+                elif o in ('-r', '--remove'):
                     self.name_of_core_to_delete = a
 
             nb_of_arguments: int = len(arguments)
 
             if self.name_of_core_to_delete is None:
                 if nb_of_arguments != 2:
-                    raise RuntimeError('Invalid arguments.Maybe start with `pfInstallCore --help?')
+                    raise RuntimeError('Invalid arguments. Maybe start with `pfInstallCore --help?')
 
                 self.zip_filename = arguments[0]
                 self.volume_name = arguments[1]
 
                 components = os.path.splitext(self.zip_filename)
                 if len(components) != 2 or components[1] != '.zip':
                     raise RuntimeError('Can only install zipped up core files.')
@@ -182,14 +182,14 @@
         print('usage: pfInstallCore <options> zip_file dest_volume')
         print('usage: pfInstallCore --delete core_name dest_volume')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h             - Show a help message.')
         print('   --version/-v          - Display the app\'s version.')
-        print('   --debug               - Enable extra debugging information.')
-        print('   --delete/-d <name>    - Delete a core on the given volume.')
+        print('   --debug/-d            - Enable extra debugging information.')
+        print('   --remove/-r <name>    - Delete a core on the given volume.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfInstallCore v' + __version__ + ' 🛠️')
```

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfQuartusEdit/__main__.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfQuartusEdit/pfQuartusEdit.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 
         try:
             self.qsf_file: str = None
             self.verilog_files: List[str] = []
             self.number_of_cpus: int = 0
 
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hvq:n:r:', ['debug', 'help', 'version', 'qsf=', 'numcpus='])
+            opts, arguments = getopt.getopt(args, 'dhvq:n:', ['debug', 'help', 'version', 'qsf=', 'numcpus='])
 
             for o, a in opts:
-                if o in ('--debug'):
+                if o in ('-d', '--debug'):
+                    # -- We ignore this argument because it was already dealt with in the calling main() code.
                     continue
                 elif o in ('-h', '--help'):
                     pfQuartusEdit.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfQuartusEdit.printVersion()
                     sys.exit(0)
@@ -145,15 +146,15 @@
         print('')
         print('usage: pfQuartusEdit <options> project_files')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h             - Show a help message.')
         print('   --version/-v          - Display the app\'s version.')
-        print('   --debug               - Enable extra debugging information.')
+        print('   --debug/-d            - Enable extra debugging information.')
         print('   --qsf/-q <file>       - Name of the QSF file to edit.')
         print('   --numcpus/-n <num>    - Number of CPU cores to use, or \'max\' to use all of them.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfQuartusEdit v' + __version__ + ' 🛠️')
```

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/__main__.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py` & `pf_fpga_tools-0.0.6/pfFPGATools/pfReverseBitstream/pfReverseBitstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     """A tool to reverse the bitstream of an rbf file for an Analog Pocket core."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hv', ['debug', 'help', 'version'])
+            opts, arguments = getopt.getopt(args, 'dhv', ['debug', 'help', 'version'])
 
             for o, a in opts:
-                if o in ('--debug'):
+                if o in ('-d', '--debug'):
+                    # -- We ignore this argument because it was already dealt with in the calling main() code.
                     continue
                 elif o in ('-h', '--help'):
                     pfReverseBitstream.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfReverseBitstream.printVersion()
                     sys.exit(0)
@@ -71,13 +72,13 @@
         print('')
         print('usage: pfReverseBitstream <options> src_filename dest_filename')
         print('')
         print('The following options are supported:')
         print('')
         print('   --help/-h          - Show a help message.')
         print('   --version/-v       - Display the app\'s version.')
-        print('   --debug            - Enable extra debugging information.')
+        print('   --debug/-d         - Enable extra debugging information.')
         print('')
 
     @classmethod
     def printVersion(cls) -> None:
         print('🛠️  pfReverseBitstream v' + __version__ + ' 🛠️')
```

### Comparing `pf_fpga_tools-0.0.5/LICENSE` & `pf_fpga_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.5/README.md` & `pf_fpga_tools-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 openFPGA is a registered trademark of [**Analogue**](https://analogue.co).
 
 -----
 
 ### Installation
 
-**pfFPGATools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
+**pfFPGATools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
 You can then install **pfFPGATools** by typing the following in a terminal window:
 ```console
 pip install pf-fpga-tools
 ```
 
 ### Installation (macOS)
```

### Comparing `pf_fpga_tools-0.0.5/pyproject.toml` & `pf_fpga_tools-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pf-fpga-tools"
 description = "A collection of tools for openFPGA projects"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 license = "GPL-3.0-or-later"
 keywords = ["openFPGA", "fpga", "analoguepocket"]
 authors = [
   { name = "Didier Malenfant", email = "coding@malenfant.net" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['Pillow',
                 'tomli >= 1.1.0 ; python_version < "3.11"']
 dynamic = ["version"]
```

### Comparing `pf_fpga_tools-0.0.5/PKG-INFO` & `pf_fpga_tools-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: pf-fpga-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of tools for openFPGA projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfFPGATools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfFPGATools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfFPGATools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: analoguepocket,fpga,openFPGA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Requires-Dist: pillow
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # pfFPGATools
 
 [![GPL-v3.0](https://img.shields.io/github/license/DidierMalenfant/pfFPGATools)](https://spdx.org/licenses/GPL-3.0-or-later.html) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pfFPGATools.svg)](https://python.org) [![PyPI - Version](https://img.shields.io/pypi/v/pfFPGATools.svg)](https://pypi.org/project/pfFPGATools)
@@ -33,15 +30,15 @@
 
 openFPGA is a registered trademark of [**Analogue**](https://analogue.co).
 
 -----
 
 ### Installation
 
-**pfFPGATools** requires at least [Python](https://python.org) 3.7. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
+**pfFPGATools** requires at least [Python](https://python.org) 3.10. Make sure you have a [supported version](http://didier.malenfant.net/blog/nerdy/2022/08/17/installing-python.html) of **Python** before proceeding.
 
 You can then install **pfFPGATools** by typing the following in a terminal window:
 ```console
 pip install pf-fpga-tools
 ```
 
 ### Installation (macOS)
```

