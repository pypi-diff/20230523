# Comparing `tmp/nwebclient-1.0.98.tar.gz` & `tmp/nwebclient-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.98.tar", last modified: Mon May 22 12:51:56 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.99.tar", last modified: Mon May 22 14:25:59 2023, max compression
```

## Comparing `nwebclient-1.0.98.tar` & `nwebclient-1.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 12:51:56.373321 nwebclient-1.0.98/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.98/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-22 12:51:56.373321 nwebclient-1.0.98/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.98/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 12:51:56.373321 nwebclient-1.0.98/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.98/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.98/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.98/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.98/nwebclient/nlp.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13678 2023-05-19 11:42:51.000000 nwebclient-1.0.98/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7104 2023-05-22 12:51:19.000000 nwebclient-1.0.98/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.98/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 12:51:56.373321 nwebclient-1.0.98/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-22 12:51:56.000000 nwebclient-1.0.98/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-22 12:51:56.373321 nwebclient-1.0.98/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-22 12:51:51.000000 nwebclient-1.0.98/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 14:25:59.084649 nwebclient-1.0.99/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.99/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-22 14:25:59.084649 nwebclient-1.0.99/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.99/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 14:25:59.084649 nwebclient-1.0.99/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6483 2023-05-12 07:26:49.000000 nwebclient-1.0.99/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.99/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.99/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3545 2023-05-14 17:14:29.000000 nwebclient-1.0.99/nwebclient/nlp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13678 2023-05-19 11:42:51.000000 nwebclient-1.0.99/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7115 2023-05-22 14:25:32.000000 nwebclient-1.0.99/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.99/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-22 14:25:59.084649 nwebclient-1.0.99/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-22 14:25:58.000000 nwebclient-1.0.99/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      382 2023-05-22 14:25:58.000000 nwebclient-1.0.99/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-22 14:25:58.000000 nwebclient-1.0.99/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-22 14:25:58.000000 nwebclient-1.0.99/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-22 14:25:58.000000 nwebclient-1.0.99/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-22 14:25:58.000000 nwebclient-1.0.99/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-22 14:25:59.094649 nwebclient-1.0.99/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-22 14:25:43.000000 nwebclient-1.0.99/setup.py
```

### Comparing `nwebclient-1.0.98/LICENSE` & `nwebclient-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/PKG-INFO` & `nwebclient-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.98
+Version: 1.0.99
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.98/README.md` & `nwebclient-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient/__init__.py` & `nwebclient-1.0.99/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient/__main__.py` & `nwebclient-1.0.99/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient/crypt.py` & `nwebclient-1.0.99/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient/nlp.py` & `nwebclient-1.0.99/nwebclient/nlp.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient/sd.py` & `nwebclient-1.0.99/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient/sdb.py` & `nwebclient-1.0.99/nwebclient/sdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             print("Id = ", row[0], "Name = ", row[1])
             name = row[1]
             id = row[0]
             data = row[2]
             i = 0
             os.mkdir(name)
             filename = name+"/"+str(id)+".jpg"
-            while os.path.isfile(file):
+            while os.path.isfile(filename):
                 i = i+1
                 filename = name+"/"+str(id+i)+".jpg"
             print("Write File: " + filename)
             writeTofile(data, filename)
 
         cursor.close()
 
@@ -183,15 +183,15 @@
     finally:
         if sqliteConnection:
             sqliteConnection.close()
         
         
 def main():
     print("SDB")
-    print("Usage nx-sdb (show|extract|from|count|clear)")
+    print("Usage nx-sdb (show|extract|from|count|clear|sortin)")
     #print(str(sys.argv)) # 0-path
     if len(sys.argv)>1:
         op = sys.argv[1]
         if op == 'count':
             count()
         elif op=='extract':
             sdb_extract()
```

### Comparing `nwebclient-1.0.98/nwebclient/ticker.py` & `nwebclient-1.0.99/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.98/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.99/nwebclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.98
+Version: 1.0.99
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.98/setup.py` & `nwebclient-1.0.99/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.98",
+    version="1.0.99",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

