# Comparing `tmp/jade_config-1.0.1.tar.gz` & `tmp/jade_config-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jade_config-1.0.1.tar", last modified: Wed Jan  4 19:03:19 2023, max compression
+gzip compressed data, was "jade_config-1.1.1.tar", last modified: Tue May 23 16:14:00 2023, max compression
```

## Comparing `jade_config-1.0.1.tar` & `jade_config-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 19:03:19.533868 jade_config-1.0.1/
--rw-rw-rw-   0        0        0     3062 2023-01-04 19:03:19.533868 jade_config-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2540 2023-01-04 18:57:53.000000 jade_config-1.0.1/README.md
--rw-rw-rw-   0        0        0     1113 2023-01-04 19:03:02.000000 jade_config-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-04 19:03:19.533868 jade_config-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-04 19:03:19.507775 jade_config-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-04 19:03:19.517930 jade_config-1.0.1/src/jade_config/
--rw-rw-rw-   0        0        0      367 2023-01-04 19:02:56.000000 jade_config-1.0.1/src/jade_config/__init__.py
--rw-rw-rw-   0        0        0      147 2023-01-04 18:30:42.000000 jade_config-1.0.1/src/jade_config/__main__.py
--rw-rw-rw-   0        0        0     2105 2023-01-04 18:54:41.000000 jade_config-1.0.1/src/jade_config/config.py
-drwxrwxrwx   0        0        0        0 2023-01-04 19:03:19.532868 jade_config-1.0.1/src/jade_config.egg-info/
--rw-rw-rw-   0        0        0     3062 2023-01-04 19:03:19.000000 jade_config-1.0.1/src/jade_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-01-04 19:03:19.000000 jade_config-1.0.1/src/jade_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 19:03:19.000000 jade_config-1.0.1/src/jade_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-04 19:03:19.000000 jade_config-1.0.1/src/jade_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-04 19:03:19.000000 jade_config-1.0.1/src/jade_config.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.589257 jade_config-1.1.1/
+-rw-rw-rw-   0        0        0     3456 2023-05-23 16:14:00.588255 jade_config-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-05-23 16:13:41.000000 jade_config-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1113 2023-05-23 16:13:36.000000 jade_config-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 16:14:00.589257 jade_config-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.572763 jade_config-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.576763 jade_config-1.1.1/src/jade_config/
+-rw-rw-rw-   0        0        0      367 2023-01-04 19:02:56.000000 jade_config-1.1.1/src/jade_config/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-01-04 18:30:42.000000 jade_config-1.1.1/src/jade_config/__main__.py
+-rw-rw-rw-   0        0        0     2771 2023-05-23 15:57:44.000000 jade_config-1.1.1/src/jade_config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.587255 jade_config-1.1.1/src/jade_config.egg-info/
+-rw-rw-rw-   0        0        0     3456 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/top_level.txt
```

### Comparing `jade_config-1.0.1/PKG-INFO` & `jade_config-1.1.1/src/jade_config.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jade_config
-Version: 1.0.1
+Name: jade-config
+Version: 1.1.1
 Summary: A python package to quickly and easily make configs, or other things that your program needs to remember.
 Author-email: nfoert <jadesoftware1@gmail.com>
 Project-URL: Homepage, https://github.com/nfoert/jade_config
 Keywords: jade,jade_config,jade config,config,remember
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -61,26 +61,41 @@
 ```
 >>> get = file.getValue("username")
 >>> print(get)
 "nfoert"
 ```
 You can use `.getValue` for any key in your file.
 
+**You can also remove a key from the file.**
+```
+>>> file.removeKey("username")
+[fileName] Removed key 'username'
+```
+
 **The full example**
 ```
 from jade_config import config
 
 file = config.Config("test", True)
 file.setValue("username", "nfoert")
 get = file.getValue("username")
 print(get)
+
+file.removeKey("username")
 ```
 
 ## Future updates
 <hr>
 
 <ul>
   <li>CLI Support</li>
   <li>The ability to choose the file location (may need to use a different library than shelve.)</li>
 </ul>
 
 **Warning: The files created by this library can still be read by others, eg. hackers, by using Jade Config, shelve or others. Don't store sensitive data like passwords or API Keys! It's certainly more secure than text files, but be careful!**
+
+## Changelog
+<hr>
+
+- [1.1.1] [5/23/23] Made errors more descriptive, added `removeKey()`, and made the database correctly close after it's done being used.
+- [1.0.1] Patch fixing a small logging confusion
+- [1.0.0] Initial release
```

### Comparing `jade_config-1.0.1/README.md` & `jade_config-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -48,26 +48,41 @@
 ```
 >>> get = file.getValue("username")
 >>> print(get)
 "nfoert"
 ```
 You can use `.getValue` for any key in your file.
 
+**You can also remove a key from the file.**
+```
+>>> file.removeKey("username")
+[fileName] Removed key 'username'
+```
+
 **The full example**
 ```
 from jade_config import config
 
 file = config.Config("test", True)
 file.setValue("username", "nfoert")
 get = file.getValue("username")
 print(get)
+
+file.removeKey("username")
 ```
 
 ## Future updates
 <hr>
 
 <ul>
   <li>CLI Support</li>
   <li>The ability to choose the file location (may need to use a different library than shelve.)</li>
 </ul>
 
 **Warning: The files created by this library can still be read by others, eg. hackers, by using Jade Config, shelve or others. Don't store sensitive data like passwords or API Keys! It's certainly more secure than text files, but be careful!**
+
+## Changelog
+<hr>
+
+- [1.1.1] [5/23/23] Made errors more descriptive, added `removeKey()`, and made the database correctly close after it's done being used.
+- [1.0.1] Patch fixing a small logging confusion
+- [1.0.0] Initial release
```

### Comparing `jade_config-1.0.1/pyproject.toml` & `jade_config-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jade_config"
-version = "1.0.1"
+version = "1.1.1"
 description = "A python package to quickly and easily make configs, or other things that your program needs to remember."
 readme = "README.md"
 authors = [{ name = "nfoert", email = "jadesoftware1@gmail.com" }]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `jade_config-1.0.1/src/jade_config/config.py` & `jade_config-1.1.1/src/jade_config/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 class UnableToGetValue(Exception):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
+class UnableToRemoveKey(Exception):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
+
 
 class Config:
     '''
     -- Jade Config --\n
     file = config.Config(name, log=False)\n
         Setting log to True enables logging. Setting it to False or ommiting the argument disables logging.\n
         Logging is not reccomended in production due to security vulnerabilities.\n
@@ -41,25 +45,39 @@
         
 
     def setValue(self, key, value):
         '''Sets the value of the file'''
         try:
             db = shelve.open(self.name)
             db[key] = value
+            db.close()
             self.logAndPrint(f"Set key '{key}' to value '{value}'")
             return True
 
         except:
-            self.logAndPrint("Unable to set value.")
-            raise UnableToSetValue("Unable to set the value.")
+            self.logAndPrint(f"Unable to set value '{value}' to key '{key}'")
+            raise UnableToSetValue(f"Unable to set value '{value}' to key '{key}'")
 
     def getValue(self, key):
         '''Gets the value of a key in the file.'''
         try:
             db = shelve.open(self.name)
             value = db[key]
+            db.close()
             self.logAndPrint(f"Got value '{value}' from key '{key}'")
             return value
 
         except:
-            self.logAndPrint("Unable to get value.")
-            raise UnableToGetValue("Unable to get the value.")
+            self.logAndPrint(f"Unable to get the value '{value}' from key '{key}'")
+            raise UnableToGetValue(f"Unable to get the value '{value}' from key '{key}'")
+        
+    def removeKey(self, key):
+        '''Removes a key from the file'''
+        try:
+            db = shelve.open(self.name)
+            del db[key]
+            db.close()
+            self.logAndPrint(f"Removed key '{key}'")
+
+        except:
+            self.logAndPrint(f"Unable to remove key '{key}'")
+            raise UnableToRemoveKey(f"Unable to remove key '{key}'")
```

### Comparing `jade_config-1.0.1/src/jade_config.egg-info/PKG-INFO` & `jade_config-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jade-config
-Version: 1.0.1
+Name: jade_config
+Version: 1.1.1
 Summary: A python package to quickly and easily make configs, or other things that your program needs to remember.
 Author-email: nfoert <jadesoftware1@gmail.com>
 Project-URL: Homepage, https://github.com/nfoert/jade_config
 Keywords: jade,jade_config,jade config,config,remember
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -61,26 +61,41 @@
 ```
 >>> get = file.getValue("username")
 >>> print(get)
 "nfoert"
 ```
 You can use `.getValue` for any key in your file.
 
+**You can also remove a key from the file.**
+```
+>>> file.removeKey("username")
+[fileName] Removed key 'username'
+```
+
 **The full example**
 ```
 from jade_config import config
 
 file = config.Config("test", True)
 file.setValue("username", "nfoert")
 get = file.getValue("username")
 print(get)
+
+file.removeKey("username")
 ```
 
 ## Future updates
 <hr>
 
 <ul>
   <li>CLI Support</li>
   <li>The ability to choose the file location (may need to use a different library than shelve.)</li>
 </ul>
 
 **Warning: The files created by this library can still be read by others, eg. hackers, by using Jade Config, shelve or others. Don't store sensitive data like passwords or API Keys! It's certainly more secure than text files, but be careful!**
+
+## Changelog
+<hr>
+
+- [1.1.1] [5/23/23] Made errors more descriptive, added `removeKey()`, and made the database correctly close after it's done being used.
+- [1.0.1] Patch fixing a small logging confusion
+- [1.0.0] Initial release
```

