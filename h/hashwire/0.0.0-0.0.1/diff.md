# Comparing `tmp/hashwire-0.0.0.tar.gz` & `tmp/hashwire-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashwire-0.0.0.tar", last modified: Tue May 23 10:05:39 2023, max compression
+gzip compressed data, was "hashwire-0.0.1.tar", last modified: Tue May 23 14:21:01 2023, max compression
```

## Comparing `hashwire-0.0.0.tar` & `hashwire-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:05:39.221888 hashwire-0.0.0/
--rw-rw-rw-   0        0        0     1071 2023-05-23 09:09:27.000000 hashwire-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     1952 2023-05-23 10:05:39.220888 hashwire-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-23 09:12:24.000000 hashwire-0.0.0/README.md
--rw-rw-rw-   0        0        0      742 2023-05-23 09:55:56.000000 hashwire-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 10:05:39.221888 hashwire-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 10:05:39.191892 hashwire-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 10:05:39.204899 hashwire-0.0.0/src/hashwire/
--rw-rw-rw-   0        0        0       21 2023-05-22 12:25:57.000000 hashwire-0.0.0/src/hashwire/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-05-23 08:00:11.000000 hashwire-0.0.0/src/hashwire/hash.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:05:39.218888 hashwire-0.0.0/src/hashwire.egg-info/
--rw-rw-rw-   0        0        0     1952 2023-05-23 10:05:39.000000 hashwire-0.0.0/src/hashwire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-23 10:05:39.000000 hashwire-0.0.0/src/hashwire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:05:39.000000 hashwire-0.0.0/src/hashwire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 10:05:39.000000 hashwire-0.0.0/src/hashwire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.301603 hashwire-0.0.1/
+-rw-rw-rw-   0        0        0     1071 2023-05-23 09:09:27.000000 hashwire-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1956 2023-05-23 14:21:01.299602 hashwire-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-05-23 09:12:24.000000 hashwire-0.0.1/README.md
+-rw-rw-rw-   0        0        0      809 2023-05-23 14:19:33.000000 hashwire-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 14:21:01.302604 hashwire-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.269442 hashwire-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.283639 hashwire-0.0.1/src/hashwire/
+-rw-rw-rw-   0        0        0        0 2023-05-23 14:08:00.000000 hashwire-0.0.1/src/hashwire/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-05-23 08:00:11.000000 hashwire-0.0.1/src/hashwire/hash.py
+drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.297604 hashwire-0.0.1/src/hashwire.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/top_level.txt
```

### Comparing `hashwire-0.0.0/LICENSE` & `hashwire-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashwire-0.0.0/PKG-INFO` & `hashwire-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashwire
-Version: 0.0.0
+Version: 0.0.1
 Summary: Hashwire creates a optimized hash multichain commitment
 Author-email: Hugo Labraaten <hugokinner@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hugo Labraaten
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,14 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/Hugloss/hashWire
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DISCLAIMER
 The author is not liable for any damages or losses that may result from using this code, including but not limited to rocket crashes, explosions or lunar landings gone wrong.
```

### Comparing `hashwire-0.0.0/pyproject.toml` & `hashwire-0.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,30 +4,32 @@
     "setuptools>=61.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'hashwire'
-dynamic = [
-    'version'
-]
+version = '0.0.1'
 description = 'Hashwire creates a optimized hash multichain commitment'
 readme = 'README.md'
 authors = [
     { name = 'Hugo Labraaten', email='hugokinner@gmail.com' }
 ]
 license = {file = 'LICENSE'}
 dependencies = [
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
-    "Programming Language :: Python",
     'Programming Language :: Python :: 3',
+    'Operating System :: OS Independent',
 ]
 
 [tool.poetry]
 readme = 'README.md'
 
 [project.urls]
 repository = 'https://github.com/Hugloss/hashWire'
+
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["hashwire*"]
```

### Comparing `hashwire-0.0.0/src/hashwire/hash.py` & `hashwire-0.0.1/src/hashwire/hash.py`

 * *Files identical despite different names*

### Comparing `hashwire-0.0.0/src/hashwire.egg-info/PKG-INFO` & `hashwire-0.0.1/src/hashwire.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashwire
-Version: 0.0.0
+Version: 0.0.1
 Summary: Hashwire creates a optimized hash multichain commitment
 Author-email: Hugo Labraaten <hugokinner@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hugo Labraaten
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,14 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/Hugloss/hashWire
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DISCLAIMER
 The author is not liable for any damages or losses that may result from using this code, including but not limited to rocket crashes, explosions or lunar landings gone wrong.
```

