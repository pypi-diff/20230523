# Comparing `tmp/spotipy-pandas-0.1.1.tar.gz` & `tmp/spotipy-pandas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotipy-pandas-0.1.1.tar", last modified: Thu May 11 22:53:20 2023, max compression
+gzip compressed data, was "spotipy-pandas-0.2.0.tar", last modified: Tue May 23 16:51:32 2023, max compression
```

## Comparing `spotipy-pandas-0.1.1.tar` & `spotipy-pandas-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 22:53:20.656212 spotipy-pandas-0.1.1/
--rw-rw-rw-   0        0        0     1071 2023-05-11 21:50:23.000000 spotipy-pandas-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1094 2023-05-11 22:53:20.654408 spotipy-pandas-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-05-11 21:57:08.000000 spotipy-pandas-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 22:53:20.658207 spotipy-pandas-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-05-11 22:52:04.000000 spotipy-pandas-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 22:53:20.612174 spotipy-pandas-0.1.1/spotipy_pandas/
--rw-rw-rw-   0        0        0       38 2023-05-11 22:23:11.000000 spotipy-pandas-0.1.1/spotipy_pandas/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-05-11 22:22:53.000000 spotipy-pandas-0.1.1/spotipy_pandas/spotipy_pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-11 22:53:20.648910 spotipy-pandas-0.1.1/spotipy_pandas.egg-info/
--rw-rw-rw-   0        0        0     1094 2023-05-11 22:53:20.000000 spotipy-pandas-0.1.1/spotipy_pandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-11 22:53:20.000000 spotipy-pandas-0.1.1/spotipy_pandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 22:53:20.000000 spotipy-pandas-0.1.1/spotipy_pandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 22:53:20.000000 spotipy-pandas-0.1.1/spotipy_pandas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 16:51:32.295301 spotipy-pandas-0.2.0/
+-rw-rw-rw-   0        0        0     1071 2023-05-11 21:50:23.000000 spotipy-pandas-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1094 2023-05-23 16:51:32.293301 spotipy-pandas-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-05-11 22:58:56.000000 spotipy-pandas-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 16:51:32.295301 spotipy-pandas-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-05-23 16:46:18.000000 spotipy-pandas-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:51:32.272301 spotipy-pandas-0.2.0/spotipy_pandas/
+-rw-rw-rw-   0        0        0       38 2023-05-11 22:23:11.000000 spotipy-pandas-0.2.0/spotipy_pandas/__init__.py
+-rw-rw-rw-   0        0        0     4069 2023-05-23 16:46:03.000000 spotipy-pandas-0.2.0/spotipy_pandas/spotipy_pandas.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:51:32.291305 spotipy-pandas-0.2.0/spotipy_pandas.egg-info/
+-rw-rw-rw-   0        0        0     1094 2023-05-23 16:51:32.000000 spotipy-pandas-0.2.0/spotipy_pandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-23 16:51:32.000000 spotipy-pandas-0.2.0/spotipy_pandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 16:51:32.000000 spotipy-pandas-0.2.0/spotipy_pandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 16:51:32.000000 spotipy-pandas-0.2.0/spotipy_pandas.egg-info/top_level.txt
```

### Comparing `spotipy-pandas-0.1.1/LICENSE` & `spotipy-pandas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotipy-pandas-0.1.1/PKG-INFO` & `spotipy-pandas-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy-pandas
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Spotipy-based Pandas wrapper for Spotify API calls
 Home-page: https://github.com/opbenesh/spotipy-pandas
 Author: Ben Esh
 Keywords: spotify pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spotipy-pandas-0.1.1/README.md` & `spotipy-pandas-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spotipy-pandas-0.1.1/setup.py` & `spotipy-pandas-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name='spotipy-pandas',
-    version='0.1.1',
-    description='A Spotipy-based Pandas wrapper for Spotify API calls',
-    url='https://github.com/opbenesh/spotipy-pandas',
-    author='Ben Esh',
+    name="spotipy-pandas",
+    version="0.2.0",
+    description="A Spotipy-based Pandas wrapper for Spotify API calls",
+    url="https://github.com/opbenesh/spotipy-pandas",
+    author="Ben Esh",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
     ],
-    keywords='spotify pandas',
+    keywords="spotify pandas",
     packages=find_packages(),
-    python_requires='>=3.7',
+    python_requires=">=3.7",
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type="text/markdown",
 )
```

### Comparing `spotipy-pandas-0.1.1/spotipy_pandas.egg-info/PKG-INFO` & `spotipy-pandas-0.2.0/spotipy_pandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy-pandas
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Spotipy-based Pandas wrapper for Spotify API calls
 Home-page: https://github.com/opbenesh/spotipy-pandas
 Author: Ben Esh
 Keywords: spotify pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

