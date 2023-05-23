# Comparing `tmp/ipxact2systemverilog-1.0.8.tar.gz` & `tmp/ipxact2systemverilog-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipxact2systemverilog-1.0.8.tar", last modified: Sat Mar  6 13:47:53 2021, max compression
+gzip compressed data, was "dist/ipxact2systemverilog-1.0.9.tar", last modified: Fri Apr  9 20:31:19 2021, max compression
```

## Comparing `ipxact2systemverilog-1.0.8.tar` & `ipxact2systemverilog-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/
--rw-r--r--   0 andreas    (501) staff       (20)     3714 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/PKG-INFO
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/bin/
--rwxr-xr-x   0 andreas    (501) staff       (20)     1259 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/bin/ipxact2rst
--rwxr-xr-x   0 andreas    (501) staff       (20)     1255 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/bin/ipxact2md
--rwxr-xr-x   0 andreas    (501) staff       (20)     1265 2021-03-06 13:45:54.000000 ipxact2systemverilog-1.0.8/bin/ipxact2systemverilog
--rwxr-xr-x   0 andreas    (501) staff       (20)     1237 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/bin/ipxact2vhdl
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/
--rw-r--r--   0 andreas    (501) staff       (20)    41371 2021-03-06 13:45:54.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/ipxact2hdlCommon.py
--rw-r--r--   0 andreas    (501) staff       (20)        0 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/__init__.py
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/
--rw-r--r--   0 andreas    (501) staff       (20)    58990 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/memoryMap.xsd
--rw-r--r--   0 andreas    (501) staff       (20)     6193 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/configurable.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    15223 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/component.xsd
--rw-r--r--   0 andreas    (501) staff       (20)     5517 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/fileType.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    13611 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/generator.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    10423 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/commonStructures.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    14154 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/autoConfigure.xsd
--rw-r--r--   0 andreas    (501) staff       (20)     5687 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/identifier.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    25819 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/port.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    10356 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/signalDrivers.xsd
--rw-r--r--   0 andreas    (501) staff       (20)     6266 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/simpleTypes.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    43912 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/busInterface.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    19026 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/model.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    15935 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/constraints.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    15424 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/subInstances.xsd
--rw-r--r--   0 andreas    (501) staff       (20)    36522 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/file.xsd
--rw-r--r--   0 andreas    (501) staff       (20)      366 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog/validate.py
--rw-r--r--   0 andreas    (501) staff       (20)       58 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/MANIFEST.in
--rw-r--r--   0 andreas    (501) staff       (20)     1045 2021-03-06 13:47:09.000000 ipxact2systemverilog-1.0.8/setup.py
--rw-r--r--   0 andreas    (501) staff       (20)       38 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/setup.cfg
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/
--rw-r--r--   0 andreas    (501) staff       (20)     3714 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)        1 2021-03-06 13:47:43.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/not-zip-safe
--rw-r--r--   0 andreas    (501) staff       (20)     1108 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/SOURCES.txt
--rw-r--r--   0 andreas    (501) staff       (20)       31 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/requires.txt
--rw-r--r--   0 andreas    (501) staff       (20)       21 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/top_level.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2021-03-06 13:47:53.000000 ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/dependency_links.txt
--rw-r--r--   0 andreas    (501) staff       (20)     2360 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.8/README.rst
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/
+-rw-r--r--   0 andreas    (501) staff       (20)     3714 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/PKG-INFO
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/bin/
+-rwxr-xr-x   0 andreas    (501) staff       (20)     1215 2021-04-09 20:29:49.000000 ipxact2systemverilog-1.0.9/bin/ipxact2rst
+-rwxr-xr-x   0 andreas    (501) staff       (20)     1211 2021-04-09 20:29:49.000000 ipxact2systemverilog-1.0.9/bin/ipxact2md
+-rwxr-xr-x   0 andreas    (501) staff       (20)     1247 2021-04-09 20:29:49.000000 ipxact2systemverilog-1.0.9/bin/ipxact2systemverilog
+-rwxr-xr-x   0 andreas    (501) staff       (20)     1219 2021-04-09 20:29:49.000000 ipxact2systemverilog-1.0.9/bin/ipxact2vhdl
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/
+-rw-r--r--   0 andreas    (501) staff       (20)    44442 2021-04-09 20:29:49.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/ipxact2hdlCommon.py
+-rw-r--r--   0 andreas    (501) staff       (20)        0 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/__init__.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/
+-rw-r--r--   0 andreas    (501) staff       (20)    58990 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/memoryMap.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)     6193 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/configurable.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    15223 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/component.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)     5517 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/fileType.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    13611 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/generator.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    10423 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/commonStructures.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    14154 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/autoConfigure.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)     5687 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/identifier.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    25819 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/port.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    10356 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/signalDrivers.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)     6266 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/simpleTypes.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    43912 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/busInterface.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    19026 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/model.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    15935 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/constraints.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    15424 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/subInstances.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)    36522 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/file.xsd
+-rw-r--r--   0 andreas    (501) staff       (20)      366 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog/validate.py
+-rw-r--r--   0 andreas    (501) staff       (20)       58 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/MANIFEST.in
+-rw-r--r--   0 andreas    (501) staff       (20)     1045 2021-04-09 20:30:01.000000 ipxact2systemverilog-1.0.9/setup.py
+-rw-r--r--   0 andreas    (501) staff       (20)       38 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/setup.cfg
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/
+-rw-r--r--   0 andreas    (501) staff       (20)     3714 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2021-03-06 13:47:43.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/not-zip-safe
+-rw-r--r--   0 andreas    (501) staff       (20)     1108 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       31 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/requires.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       21 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/top_level.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2021-04-09 20:31:19.000000 ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas    (501) staff       (20)     2360 2021-02-22 20:39:28.000000 ipxact2systemverilog-1.0.9/README.rst
```

### Comparing `ipxact2systemverilog-1.0.8/PKG-INFO` & `ipxact2systemverilog-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ipxact2systemverilog
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generate VHDL, SystemVerilog, html, rst, md, pdf from an IPXACT description
 Home-page: https://github.com/oddball/ipxact2systemverilog
 Author: oddball
 License: GPL
 Description: xact2systemverilog ipxact2rst ipxact2md ipxact2vhdl
         ---------------------------------------------------
```

### Comparing `ipxact2systemverilog-1.0.8/bin/ipxact2rst` & `ipxact2systemverilog-1.0.9/bin/ipxact2vhdl`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
 
 import configparser
 import sys
-import os
 import argparse
-from pprint import pprint
 
 from ipxact2systemverilog.ipxact2hdlCommon import ipxactParser
 from ipxact2systemverilog.ipxact2hdlCommon import ipxact2otherGenerator
-from ipxact2systemverilog.ipxact2hdlCommon import rstAddressBlock
+from ipxact2systemverilog.ipxact2hdlCommon import vhdlAddressBlock
 from ipxact2systemverilog.ipxact2hdlCommon import DEFAULT_INI
 from ipxact2systemverilog.validate import validate
 
+
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ipxact2rst')
+    parser = argparse.ArgumentParser(description='ipxact2vhdl')
     parser.add_argument('-s', '--srcFile', help='ipxact xml input file', required=True)
     parser.add_argument('-d', '--destDir', help="write generated file to dir", required=True)
     parser.add_argument('-c', '--config', help="configuration ini file")
 
     args, unknown_args = parser.parse_known_args()
 
     if not validate(args.srcFile):
@@ -25,12 +24,12 @@
         sys.exit(1)
 
     config = configparser.ConfigParser()
     if args.config:
         config.read(args.config)
     else:
         config.read_dict(DEFAULT_INI)
-        
+
     e = ipxactParser(args.srcFile, config)
     document = e.returnDocument()
     generator = ipxact2otherGenerator(args.destDir)
-    generator.generate(rstAddressBlock, document)
+    generator.generate(vhdlAddressBlock, document)
```

### Comparing `ipxact2systemverilog-1.0.8/bin/ipxact2md` & `ipxact2systemverilog-1.0.9/bin/ipxact2systemverilog`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python3
+
 import configparser
 import sys
-import os
 import argparse
-from pprint import pprint
 
 from ipxact2systemverilog.ipxact2hdlCommon import ipxactParser
 from ipxact2systemverilog.ipxact2hdlCommon import ipxact2otherGenerator
-from ipxact2systemverilog.ipxact2hdlCommon import mdAddressBlock
+from ipxact2systemverilog.ipxact2hdlCommon import systemVerilogAddressBlock
 from ipxact2systemverilog.ipxact2hdlCommon import DEFAULT_INI
 from ipxact2systemverilog.validate import validate
 
+
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ipxact2md')
+    parser = argparse.ArgumentParser(description='ipxact2systemverilog')
     parser.add_argument('-s', '--srcFile', help='ipxact xml input file', required=True)
     parser.add_argument('-d', '--destDir', help="write generated file to dir", required=True)
     parser.add_argument('-c', '--config', help="configuration ini file")
 
     args, unknown_args = parser.parse_known_args()
 
     if not validate(args.srcFile):
         print("%s doesn't validate" % args.srcFile)
         sys.exit(1)
 
     config = configparser.ConfigParser()
     if args.config:
         config.read(args.config)
-    else:
+    else: 
         config.read_dict(DEFAULT_INI)
-        
+
     e = ipxactParser(args.srcFile, config)
     document = e.returnDocument()
     generator = ipxact2otherGenerator(args.destDir)
-    generator.generate(mdAddressBlock, document)
+    generator.generate(systemVerilogAddressBlock, document)
```

### Comparing `ipxact2systemverilog-1.0.8/bin/ipxact2systemverilog` & `ipxact2systemverilog-1.0.9/bin/ipxact2md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 #!/usr/bin/env python3
-
 import configparser
 import sys
-import os
 import argparse
 
 from ipxact2systemverilog.ipxact2hdlCommon import ipxactParser
 from ipxact2systemverilog.ipxact2hdlCommon import ipxact2otherGenerator
-from ipxact2systemverilog.ipxact2hdlCommon import systemVerilogAddressBlock
+from ipxact2systemverilog.ipxact2hdlCommon import mdAddressBlock
 from ipxact2systemverilog.ipxact2hdlCommon import DEFAULT_INI
 from ipxact2systemverilog.validate import validate
 
-
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ipxact2systemverilog')
+    parser = argparse.ArgumentParser(description='ipxact2md')
     parser.add_argument('-s', '--srcFile', help='ipxact xml input file', required=True)
     parser.add_argument('-d', '--destDir', help="write generated file to dir", required=True)
     parser.add_argument('-c', '--config', help="configuration ini file")
 
     args, unknown_args = parser.parse_known_args()
 
     if not validate(args.srcFile):
         print("%s doesn't validate" % args.srcFile)
         sys.exit(1)
 
     config = configparser.ConfigParser()
     if args.config:
         config.read(args.config)
-    else: 
+    else:
         config.read_dict(DEFAULT_INI)
-        
+
     e = ipxactParser(args.srcFile, config)
     document = e.returnDocument()
     generator = ipxact2otherGenerator(args.destDir)
-    generator.generate(systemVerilogAddressBlock, document)
+    generator.generate(mdAddressBlock, document)
```

### Comparing `ipxact2systemverilog-1.0.8/bin/ipxact2vhdl` & `ipxact2systemverilog-1.0.9/bin/ipxact2rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python3
 
 import configparser
 import sys
-import os
 import argparse
 
 from ipxact2systemverilog.ipxact2hdlCommon import ipxactParser
 from ipxact2systemverilog.ipxact2hdlCommon import ipxact2otherGenerator
-from ipxact2systemverilog.ipxact2hdlCommon import vhdlAddressBlock
+from ipxact2systemverilog.ipxact2hdlCommon import rstAddressBlock
 from ipxact2systemverilog.ipxact2hdlCommon import DEFAULT_INI
 from ipxact2systemverilog.validate import validate
 
-
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ipxact2vhdl')
+    parser = argparse.ArgumentParser(description='ipxact2rst')
     parser.add_argument('-s', '--srcFile', help='ipxact xml input file', required=True)
     parser.add_argument('-d', '--destDir', help="write generated file to dir", required=True)
     parser.add_argument('-c', '--config', help="configuration ini file")
 
     args, unknown_args = parser.parse_known_args()
 
     if not validate(args.srcFile):
@@ -25,12 +23,12 @@
         sys.exit(1)
 
     config = configparser.ConfigParser()
     if args.config:
         config.read(args.config)
     else:
         config.read_dict(DEFAULT_INI)
-        
+
     e = ipxactParser(args.srcFile, config)
     document = e.returnDocument()
     generator = ipxact2otherGenerator(args.destDir)
-    generator.generate(vhdlAddressBlock, document)
+    generator.generate(rstAddressBlock, document)
```

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/ipxact2hdlCommon.py` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/ipxact2hdlCommon.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,25 @@
                 enum.enumName = e.name
                 break
         self.listOfEnums.append(enum)
         return enum
 
 
 class enumTypeClass():
-    def __init__(self, name, bitWidth, keyList, valueList):
+    def __init__(self, name, bitWidth, keyList, valueList, descrList):
         self.name = name
         self.bitWidth = bitWidth
         matrix = list(zip(valueList, keyList))
         matrix.sort(key=lambda x: x[0])
         valueList, keyList = list(zip(*matrix))
         self.keyList = list(keyList)
         self.valueList = list(valueList)
         self.allReadyExist = False
         self.enumName = None
+        self.descrList = descrList
 
     def compare(self, other):
         result = True
         result = self.bitWidth == other.bitWidth and result
         result = self.compareLists(self.keyList, other.keyList) and result
         return result
 
@@ -209,36 +210,58 @@
         for reg in self.registerList:
             r += self.returnRstRegDesc(reg.name, reg.address, reg.size, reg.resetValue, reg.desc, reg.access)
             reg_table = []
             for fieldIndex in reversed(list(range(len(reg.fieldNameList)))):
                 bits = "[" + str(reg.bitOffsetList[fieldIndex] + reg.bitWidthList[fieldIndex] - 1) + \
                        ":" + str(reg.bitOffsetList[fieldIndex]) + "]"
                 _line = [bits,
-                         reg.fieldNameList[fieldIndex],
-                         self.returnEnumValueString(reg.enumTypeList[fieldIndex])]
+                         reg.fieldNameList[fieldIndex]]
+
                 if reg.resetValue:
                     temp = (int(reg.resetValue, 0) >> reg.bitOffsetList[fieldIndex])
                     mask = (2 ** reg.bitWidthList[fieldIndex]) - 1
                     temp &= mask
                     temp = "{value:#0{width}x}".format(value=temp,
                                                        width=math.ceil(reg.bitWidthList[fieldIndex] / 4) + 2)
                     _line.append(temp)
                 _line.append(reg.fieldDescList[fieldIndex])
                 reg_table.append(_line)
 
-            _headers = ['Bits', 'Field name', 'Type']
+            _headers = ['Bits', 'Field name']
             if reg.resetValue:
                 _headers.append('Reset')
             _headers.append('Description')
             r += tabulate.tabulate(reg_table,
                                    headers=_headers,
                                    tablefmt="grid")
             r += "\n"
             r += "\n"
 
+            # enumerations
+            for enum in reg.enumTypeList:
+                if enum:
+                    # header
+                    r += enum.name + "\n"
+                    r += ',' * len(enum.name) + "\n"
+                    r += "\n"
+                    # table
+                    enum_table = []
+                    for i in range(len(enum.keyList)):
+                        _value  = "{value:#0{width}x}".format(value=int(enum.valueList[i], 0),
+                                                              width=math.ceil(int(enum.bitWidth, 0) / 4) + 2)
+
+                        _line = [enum.keyList[i],
+                                 _value,
+                                 enum.descrList[i]]
+                        enum_table.append(_line)
+                    r += tabulate.tabulate(enum_table,
+                                           headers=['Name', 'Value', 'Description'],
+                                           tablefmt="grid")
+                    r += "\n\n"
+
         return r
 
     def returnRstTitle(self):
         r = ''
         r += "====================\n"
         r += "Register description\n"
         r += "====================\n\n"
@@ -285,15 +308,14 @@
                 l.append(enumTypeObj.keyList[i] + '=' + enumTypeObj.valueList[i])
             s = ", ".join(l)
         else:
             s = ''
         return s
 
     def returnAsString(self):
-        r = ""
         regNameList = [reg.name for reg in self.registerList]
         regAddressList = [reg.address for reg in self.registerList]
         regDescrList = [reg.desc for reg in self.registerList]
 
         self.mdFile.new_header(level=1, title="Register description")
         self.mdFile.new_header(level=2, title="Registers")
 
@@ -308,41 +330,60 @@
         self.mdFile.new_table(columns=len(header),
                               rows=len(regNameList) + 1,  # header + data
                               text=header + rows,
                               text_align='left')
 
         # all registers
         for reg in self.registerList:
-            headers=['Bits', 'Field name', 'Type']
+            headers=['Bits', 'Field name']
             if reg.resetValue:
                 headers.append('Reset')
             headers.append('Description')
 
             self.returnMdRegDesc(reg.name, reg.address, reg.size, reg.resetValue, reg.desc, reg.access)
             reg_table = []
             for fieldIndex in reversed(list(range(len(reg.fieldNameList)))):
                 bits = "[" + str(reg.bitOffsetList[fieldIndex] + reg.bitWidthList[fieldIndex] - 1) + \
                        ":" + str(reg.bitOffsetList[fieldIndex]) + "]"
                 reg_table.append(bits)
                 reg_table.append(reg.fieldNameList[fieldIndex])
-                reg_table.append(self.returnEnumValueString(reg.enumTypeList[fieldIndex]))
                 if reg.resetValue:
                     temp = (int(reg.resetValue, 0) >> reg.bitOffsetList[fieldIndex])
                     mask = (2 ** reg.bitWidthList[fieldIndex]) - 1
                     temp &= mask
                     temp = "{value:#0{width}x}".format(value=temp,
                                                        width=math.ceil(reg.bitWidthList[fieldIndex] / 4) + 2)
                     reg_table.append(temp)
                 reg_table.append(reg.fieldDescList[fieldIndex])
 
             self.mdFile.new_table(columns=len(headers),
                                   rows=len(reg.fieldNameList) + 1,
                                   text=headers + reg_table,
                                   text_align='left')
 
+
+            # enumerations
+            for enum in reg.enumTypeList:
+                if enum:
+                    self.mdFile.new_header(level=4,
+                                           title=enum.name)
+                    enum_table = []
+                    for i in range(len(enum.keyList)):
+                        _value  = "{value:#0{width}x}".format(value=int(enum.valueList[i], 0),
+                                                              width=math.ceil(int(enum.bitWidth, 0) / 4) + 2)
+                        enum_table.append(enum.keyList[i])
+                        enum_table.append(_value)
+                        enum_table.append(enum.descrList[i])
+                    headers=['Name', 'Value', 'Description']
+                    self.mdFile.new_table(columns=len(headers),
+                                          rows=len(enum.keyList) + 1,
+                                          text=headers + enum_table,
+                                          text_align='left')
+
+
         return self.mdFile.file_data_text
 
     def returnMdRegDesc(self, name, address, size, resetValue, desc, access):
         self.mdFile.new_header(level=3, title=name)
         self.mdFile.new_line("**Name** " + str(name))
         self.mdFile.new_line("**Address** " + hex(address))
         if resetValue:
@@ -434,22 +475,36 @@
         return r
 
     def returnRegFieldEnumTypeStrings(self, prototype):
         r = ''
         for reg in self.registerList:
             for enum in reg.enumTypeList:
                 if isinstance(enum, enumTypeClass) and not enum.allReadyExist:
+                    r += "  -- {}\n".format(enum.name)  # group the enums in the package
                     if prototype:
-                        s = ",".join(enum.keyList)
-                        r += "  type " + enum.name + "_enum is (" + s + ");\n\n"
+                        t = "  type " + enum.name + "_enum is ("
+                        indent = t.find('(') + 1
+                        r += t
+                        for ki in range(len(enum.keyList)):
+                            r += enum.keyList[ki]
+                            if ki != len(enum.keyList) - 1:  # no ',' for the last element
+                                r += ","
+                            else:  # last element
+                                r += ");"
+                            if enum.descrList[ki]:
+                                r += "  -- " + enum.descrList[ki]
+                            if ki != len(enum.keyList) - 1:  # no new line for the last element
+                                r += "\n"
+                            r += " " * indent  # indent the next line
+                        r += "\n"
 
                     r += "  function " + enum.name + \
                         "_enum_to_sulv(v: " + enum.name + "_enum ) return std_ulogic_vector"
                     if prototype:
-                        r += ";\n\n"
+                        r += ";\n"
                     else:
                         r += " is\n"
                         r += "    variable r : std_ulogic_vector (" + str(enum.bitWidth) + "-1 downto 0);\n"
                         r += "  begin\n"
                         r += "       case v is\n"
                         for i in range(len(enum.keyList)):
                             r += '         when {key} => r:="{value_int:0{bitwidth}b}"; -- {value}\n'.format(
@@ -461,29 +516,33 @@
                         r += "    return r;\n"
                         r += "  end function;\n\n"
 
                     r += "  function sulv_to_" + enum.name + \
                         "_enum(v: std_ulogic_vector (" + str(enum.bitWidth) + "-1 downto 0)) return " + \
                         enum.name + "_enum"
                     if prototype:
-                        r += ";\n\n"
+                        r += ";\n"
                     else:
                         r += " is\n"
                         r += "    variable r : " + enum.name + "_enum;\n"
                         r += "  begin\n"
                         r += "       case v is\n"
                         for i in range(len(enum.keyList)):
                             r += '         when "{value_int:0{bitwidth}b}" => r:={key};\n'.format(key=enum.keyList[i],
                                                                                                   value_int=int(enum.valueList[i]),
                                                                                                   bitwidth=int(enum.bitWidth))
                         r += '         when others => r:=' + enum.keyList[0] + '; -- error \n'
                         r += "       end case;\n"
                         r += "    return r;\n"
                         r += "  end function;\n\n"
 
+                    if prototype:
+                        r += "\n"
+        if prototype:
+            r += "\n"
         return r
 
     def returnRegRecordTypeString(self, reg):
         r = ''
         r += "  type " + reg.name + "_record_type is record\n"
         for i in reversed(list(range(len(reg.fieldNameList)))):
             bits = "[" + str(reg.bitOffsetList[i] + reg.bitWidthList[i] - 1) + ":" + str(reg.bitOffsetList[i]) + "]"
@@ -793,15 +852,15 @@
 
     def returnAsString(self):
         r = ''
         r += "// Automatically generated\n"
         r += "// with the command '%s'\n" % (' '.join(sys.argv))
         r += "// \n"
         r += "// Do not manually edit!\n"
-        r += "// \n"        
+        r += "// \n"
         r += "package " + self.name + "_sv_pkg;\n\n"
         r += self.returnSizeString()
         r += self.returnAddressesString()
         r += self.returnAddressListString()
         r += self.returnStructString()
         r += self.returnResetValuesString()
         r += self.returnRegistersStructString()
@@ -845,15 +904,18 @@
                     reset = registerElem.find(spiritString + "reset")
                     if reset is not None:
                         resetValue = reset.find(spiritString + "value").text
                     else:
                         resetValue = None
                     size = int(registerElem.find(spiritString + "size").text, 0)
                     access = registerElem.find(spiritString + "access").text
-                    desc = registerElem.find(spiritString + "description").text
+                    if registerElem.find(spiritString + "description") != None:
+                        desc = registerElem.find(spiritString + "description").text
+                    else:
+                        desc = ""
                     regAddress = baseAddress + int(registerElem.find(spiritString + "addressOffset").text, 0)
                     r = self.returnRegister(spiritString, registerElem, regAddress,
                                             resetValue, size, access, desc, dataWidth)
                     a.addRegister(r)
                 m.addAddressBlock(a)
             d.addMemoryMap(m)
 
@@ -871,23 +933,24 @@
             fieldElem = fieldList[index]
             bitWidth = bitWidthList[index]
             fieldName = fieldNameList[index]
             enumeratedValuesElem = fieldElem.find(spiritString + "enumeratedValues")
             if enumeratedValuesElem is not None:
                 enumeratedValueList = enumeratedValuesElem.findall(spiritString + "enumeratedValue")
                 valuesNameList = [item.find(spiritString + "name").text for item in enumeratedValueList]
+                descrList = [item.find(spiritString + "description").text if item.find(spiritString + "description") is not None else "" for item in enumeratedValueList]
                 valuesList = [item.find(spiritString + "value").text for item in enumeratedValueList]
                 if len(valuesNameList) > 0:
                     if int(bitWidth) > 1:  # if the field of a enum is longer than 1 bit, always use enums
-                        enum = enumTypeClass(fieldName, bitWidth, valuesNameList, valuesList)
+                        enum = enumTypeClass(fieldName, bitWidth, valuesNameList, valuesList, descrList)
                         enum = self.enumTypeClassRegistry.enumAllReadyExist(enum)
                         enumTypeList.append(enum)
                     else:  # bit field of 1 bit
                         if self.config['global'].getboolean('onebitenum'):  # do create one bit enums
-                            enum = enumTypeClass(fieldName, bitWidth, valuesNameList, valuesList)
+                            enum = enumTypeClass(fieldName, bitWidth, valuesNameList, valuesList, descrList)
                             enum = self.enumTypeClassRegistry.enumAllReadyExist(enum)
                             enumTypeList.append(enum)
                         else:  # dont create enums of booleans because this only decreases readability
                             enumTypeList.append(None)
                 else:
                     enumTypeList.append(None)
             else:
```

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/memoryMap.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/memoryMap.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/configurable.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/configurable.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/component.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/component.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/fileType.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/fileType.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/generator.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/generator.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/commonStructures.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/commonStructures.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/autoConfigure.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/autoConfigure.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/identifier.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/identifier.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/port.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/port.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/signalDrivers.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/signalDrivers.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/simpleTypes.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/simpleTypes.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/busInterface.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/busInterface.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/model.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/model.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/constraints.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/constraints.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/subInstances.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/subInstances.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog/xml/file.xsd` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog/xml/file.xsd`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/setup.py` & `ipxact2systemverilog-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 
 setup(name='ipxact2systemverilog',
       python_requires='>=3',
-      version='1.0.8',
+      version='1.0.9',
       description='Generate VHDL, SystemVerilog, html, rst, md, pdf from an IPXACT description',
       long_description=readme(),
       classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3',
         'Topic :: Text Processing :: Linguistic',
```

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/PKG-INFO` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ipxact2systemverilog
-Version: 1.0.8
+Version: 1.0.9
 Summary: Generate VHDL, SystemVerilog, html, rst, md, pdf from an IPXACT description
 Home-page: https://github.com/oddball/ipxact2systemverilog
 Author: oddball
 License: GPL
 Description: xact2systemverilog ipxact2rst ipxact2md ipxact2vhdl
         ---------------------------------------------------
```

### Comparing `ipxact2systemverilog-1.0.8/ipxact2systemverilog.egg-info/SOURCES.txt` & `ipxact2systemverilog-1.0.9/ipxact2systemverilog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipxact2systemverilog-1.0.8/README.rst` & `ipxact2systemverilog-1.0.9/README.rst`

 * *Files identical despite different names*

