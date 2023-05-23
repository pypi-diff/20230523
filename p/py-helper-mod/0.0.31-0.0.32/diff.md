# Comparing `tmp/py-helper-mod-0.0.31.tar.gz` & `tmp/py-helper-mod-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmpsys_7wde/py-helper-mod-0.0.31.tar", last modified: Mon May 22 20:23:26 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp15x93tsh/py-helper-mod-0.0.32.tar", last modified: Tue May 23 02:29:44 2023, max compression
```

## Comparing `py-helper-mod-0.0.31.tar` & `py-helper-mod-0.0.32.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.31/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.31/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.31/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.31/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-22 20:23:26.000000 py-helper-mod-0.0.31/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    81048 2023-05-22 20:22:33.000000 py-helper-mod-0.0.31/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.32/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.32/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.32/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.32/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-23 02:29:44.000000 py-helper-mod-0.0.32/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    81136 2023-05-23 02:27:38.000000 py-helper-mod-0.0.32/py_helper.py
```

### Comparing `py-helper-mod-0.0.31/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.32/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.31
+Version: 0.0.32
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.31/LICENSE` & `py-helper-mod-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.31/PKG-INFO` & `py-helper-mod-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.31
+Version: 0.0.32
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.31/py_helper.py` & `py-helper-mod-0.0.32/py_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -899,25 +899,26 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,31)
+VERSION=(0,0,32)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
 
 # Debug/Breakpoint Flags
 DebugEnabled = None
+DebugLabelExists = False
 
 # Signals Module is being used in Cmd Line Mode
 __CmdLineMode__ = False
 
 # Notes:
 # DebugMode puts the module in DebugMode, i.e. it activates DbgMsg() to output
 # 	when DebugMode is false, DbgMsg does nothing.
@@ -1126,31 +1127,31 @@
 
 		with open(filename,"r",newline='') as csvfile:
 			reader = csv.reader(csvfile)
 
 			for row in reader:
 				DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","Yes","yes","y","Y" ] else False
 
-def IsDebugEnabled(dbglabel):
+def IsDebugLabelEnabled(dbglabel):
 	"""Check if Debug Label is Enabled"""
 
-	global DebugEnabled
+	global DebugEnabled, DebugLabelExists
 
-	enabled = True
+	enabled = True if not DebugLabelExists else False
 
 	if DebugEnabled is not None and dbglabel is not None:
 		if dbglabel in DebugEnabled and test:
 			enabled = DebugEnabled[dbglabel]
 
 	return enabled
 
 def Breakpoint(dbglabel,test_flag=True):
 	"""Check if Debug Label is Enabled AND We Are In DebugMode"""
 
-	enabled = IsDebugEnabled(dbglabel)
+	enabled = IsDebugLabelEnabled(dbglabel)
 
 	return (DebugMode() and enabled and test_flag)
 
 # A Centrally Controlled Debug Messaging System
 # msg : Message to print
 # func : A simple function to pass the message to (optional)
 # If "func" is supplied, DbgMsg uses it for output instead of printing to stdout
```

