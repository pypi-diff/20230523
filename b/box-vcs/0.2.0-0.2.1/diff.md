# Comparing `tmp/box-vcs-0.2.0.tar.gz` & `tmp/box-vcs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box-vcs-0.2.0.tar", last modified: Tue May 23 00:35:37 2023, max compression
+gzip compressed data, was "box-vcs-0.2.1.tar", last modified: Tue May 23 01:02:47 2023, max compression
```

## Comparing `box-vcs-0.2.0.tar` & `box-vcs-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.726440 box-vcs-0.2.0/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-05-21 21:52:01.000000 box-vcs-0.2.0/LICENSE
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 00:35:37.718440 box-vcs-0.2.0/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1935 2023-05-23 00:35:25.000000 box-vcs-0.2.0/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.678440 box-vcs-0.2.0/box/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-05-23 00:35:07.000000 box-vcs-0.2.0/box/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9410 2023-05-23 00:12:33.000000 box-vcs-0.2.0/box/__main__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/_config.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/commit.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/exceptions.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2128 2023-05-22 23:40:23.000000 box-vcs-0.2.0/box/ignore.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/tracker.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/utils.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.714440 box-vcs-0.2.0/box_vcs.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      353 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/entry_points.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/requires.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-05-23 00:35:37.726440 box-vcs-0.2.0/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1083 2023-05-23 00:34:50.000000 box-vcs-0.2.0/setup.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.718440 box-vcs-0.2.0/tests/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-05-21 21:52:01.000000 box-vcs-0.2.0/tests/test_box.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.239831 box-vcs-0.2.1/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-05-21 21:52:01.000000 box-vcs-0.2.1/LICENSE
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 01:02:47.235831 box-vcs-0.2.1/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1935 2023-05-23 00:35:25.000000 box-vcs-0.2.1/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.215831 box-vcs-0.2.1/box/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-05-23 01:00:30.000000 box-vcs-0.2.1/box/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9430 2023-05-23 00:59:04.000000 box-vcs-0.2.1/box/__main__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/_config.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/commit.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/exceptions.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2128 2023-05-22 23:40:23.000000 box-vcs-0.2.1/box/ignore.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/tracker.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-05-21 21:52:01.000000 box-vcs-0.2.1/box/utils.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.231831 box-vcs-0.2.1/box_vcs.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      353 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/entry_points.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/requires.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-05-23 01:02:47.000000 box-vcs-0.2.1/box_vcs.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-05-23 01:02:47.239831 box-vcs-0.2.1/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1083 2023-05-23 00:34:50.000000 box-vcs-0.2.1/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 01:02:47.235831 box-vcs-0.2.1/tests/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-05-21 21:52:01.000000 box-vcs-0.2.1/tests/test_box.py
```

### Comparing `box-vcs-0.2.0/LICENSE` & `box-vcs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/PKG-INFO` & `box-vcs-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple and fast file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.2.0 Summary: Simple and fast
+Metadata-Version: 2.1 Name: box-vcs Version: 0.2.1 Summary: Simple and fast
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
```

### Comparing `box-vcs-0.2.0/README.md` & `box-vcs-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box/__init__.py` & `box-vcs-0.2.1/box/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

### Comparing `box-vcs-0.2.0/box/__main__.py` & `box-vcs-0.2.1/box/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     parser.add_flag('--email', 'Set author email')
 
     parser.add_flag('--filter-by-name', 'Filter log commit by author name')
     parser.add_flag('--filter-by-email', 'Filter log commit by author email')
 
     args = parser.parse()
 
-    if not args.init and not path.isdir(OBJECTS_PATH):
+    if not path.isdir(OBJECTS_PATH) and not any((args.init, args.config)):
         print('\033[1;31mRepository not found\033[m')
         print('\033[33mCreate a repository with "init" command\033[m')
         sys.exit(1)
 
     if args.init:
         _init()
     elif args.add is not None:
```

### Comparing `box-vcs-0.2.0/box/_config.py` & `box-vcs-0.2.1/box/_config.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box/commit.py` & `box-vcs-0.2.1/box/commit.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box/exceptions.py` & `box-vcs-0.2.1/box/exceptions.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box/ignore.py` & `box-vcs-0.2.1/box/ignore.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box/tracker.py` & `box-vcs-0.2.1/box/tracker.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box/utils.py` & `box-vcs-0.2.1/box/utils.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/box_vcs.egg-info/PKG-INFO` & `box-vcs-0.2.1/box_vcs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple and fast file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.2.0 Summary: Simple and fast
+Metadata-Version: 2.1 Name: box-vcs Version: 0.2.1 Summary: Simple and fast
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
```

### Comparing `box-vcs-0.2.0/setup.py` & `box-vcs-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.2.0/tests/test_box.py` & `box-vcs-0.2.1/tests/test_box.py`

 * *Files identical despite different names*

