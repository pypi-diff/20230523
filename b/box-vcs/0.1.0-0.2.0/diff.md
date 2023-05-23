# Comparing `tmp/box-vcs-0.1.0.tar.gz` & `tmp/box-vcs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box-vcs-0.1.0.tar", last modified: Wed May 17 16:14:03 2023, max compression
+gzip compressed data, was "box-vcs-0.2.0.tar", last modified: Tue May 23 00:35:37 2023, max compression
```

## Comparing `box-vcs-0.1.0.tar` & `box-vcs-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-17 16:14:03.033985 box-vcs-0.1.0/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-03-18 17:17:45.000000 box-vcs-0.1.0/LICENSE
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2635 2023-05-17 16:14:03.033985 box-vcs-0.1.0/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1931 2023-05-17 16:13:10.000000 box-vcs-0.1.0/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-17 16:14:03.021984 box-vcs-0.1.0/box/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-03-27 01:48:44.000000 box-vcs-0.1.0/box/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     8751 2023-04-13 13:05:52.000000 box-vcs-0.1.0/box/__main__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-03-27 01:00:59.000000 box-vcs-0.1.0/box/_config.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-05-17 16:09:52.000000 box-vcs-0.1.0/box/commit.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-03-18 17:20:59.000000 box-vcs-0.1.0/box/exceptions.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1858 2023-03-18 17:21:11.000000 box-vcs-0.1.0/box/ignore.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-04-13 02:26:47.000000 box-vcs-0.1.0/box/tracker.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-04-10 02:41:14.000000 box-vcs-0.1.0/box/utils.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-17 16:14:03.033985 box-vcs-0.1.0/box_vcs.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2635 2023-05-17 16:14:02.000000 box-vcs-0.1.0/box_vcs.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      353 2023-05-17 16:14:02.000000 box-vcs-0.1.0/box_vcs.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-05-17 16:14:02.000000 box-vcs-0.1.0/box_vcs.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-05-17 16:14:02.000000 box-vcs-0.1.0/box_vcs.egg-info/entry_points.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-05-17 16:14:02.000000 box-vcs-0.1.0/box_vcs.egg-info/requires.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-05-17 16:14:02.000000 box-vcs-0.1.0/box_vcs.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-05-17 16:14:03.033985 box-vcs-0.1.0/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1083 2023-05-17 16:09:56.000000 box-vcs-0.1.0/setup.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-17 16:14:03.033985 box-vcs-0.1.0/tests/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-04-13 12:06:17.000000 box-vcs-0.1.0/tests/test_box.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.726440 box-vcs-0.2.0/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    18092 2023-05-21 21:52:01.000000 box-vcs-0.2.0/LICENSE
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 00:35:37.718440 box-vcs-0.2.0/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1935 2023-05-23 00:35:25.000000 box-vcs-0.2.0/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.678440 box-vcs-0.2.0/box/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      783 2023-05-23 00:35:07.000000 box-vcs-0.2.0/box/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9410 2023-05-23 00:12:33.000000 box-vcs-0.2.0/box/__main__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      649 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/_config.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     9031 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/commit.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1097 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/exceptions.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2128 2023-05-22 23:40:23.000000 box-vcs-0.2.0/box/ignore.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3508 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/tracker.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2074 2023-05-21 21:52:01.000000 box-vcs-0.2.0/box/utils.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.714440 box-vcs-0.2.0/box_vcs.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2639 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      353 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       42 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/entry_points.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       15 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/requires.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        4 2023-05-23 00:35:37.000000 box-vcs-0.2.0/box_vcs.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-05-23 00:35:37.726440 box-vcs-0.2.0/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1083 2023-05-23 00:34:50.000000 box-vcs-0.2.0/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-05-23 00:35:37.718440 box-vcs-0.2.0/tests/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7205 2023-05-21 21:52:01.000000 box-vcs-0.2.0/tests/test_box.py
```

### Comparing `box-vcs-0.1.0/LICENSE` & `box-vcs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/PKG-INFO` & `box-vcs-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple and fast file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -22,15 +22,15 @@
 <p align="center">Fast and simple file versioning</p>
 
 <p align="center">
     <a href="https://github.com/firlast/box/releases">
         <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/firlast/box?include_prereleases">
     </a>
     <a href="https://github.com/firlast/box/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box-vcs">
     </a>
 </p>
 
 Box is an open-source version control system **written in Python** that allows users to manage changes to their projects efficiently and collaboratively. With Box, you can control the history of **changes made to files**, track issues and bugs, and collaborate with other developers in a safe and secure environment. With an **intuitive interface** and customizable features, Box is a complete solution for development teams looking for an affordable and easy-to-use version control system. If you are looking for an efficient and organized way to manage your project versions, Box is a smart and affordable choice.
 
 ## Getting Started with Box
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.1.0 Summary: Simple and fast
+Metadata-Version: 2.1 Name: box-vcs Version: 0.2.0 Summary: Simple and fast
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
```

### Comparing `box-vcs-0.1.0/README.md` & `box-vcs-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <p align="center">Fast and simple file versioning</p>
 
 <p align="center">
     <a href="https://github.com/firlast/box/releases">
         <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/firlast/box?include_prereleases">
     </a>
     <a href="https://github.com/firlast/box/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box-vcs">
     </a>
 </p>
 
 Box is an open-source version control system **written in Python** that allows users to manage changes to their projects efficiently and collaboratively. With Box, you can control the history of **changes made to files**, track issues and bugs, and collaborate with other developers in a safe and secure environment. With an **intuitive interface** and customizable features, Box is a complete solution for development teams looking for an affordable and easy-to-use version control system. If you are looking for an efficient and organized way to manage your project versions, Box is a smart and affordable choice.
 
 ## Getting Started with Box
```

### Comparing `box-vcs-0.1.0/box/__init__.py` & `box-vcs-0.2.0/box/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `box-vcs-0.1.0/box/__main__.py` & `box-vcs-0.2.0/box/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,23 +142,35 @@
         print(f'Commit #\033[4m{commit_id[:7]}\033[m "{message}"')
         print(f'\033[33m{len(files)} files committed in {time.time() - time_s:.3f}s\033[m')
     except exceptions.NoFilesToCommitError:
         print('\033[1;31mNo files changed to commit\033[m')
         print('\033[33mYou can only commit changed and tracked files\033[m')
 
 
-def _log() -> None:
+def _log(filter_by_name: str = None, filter_by_email: str = None) -> None:
     commits = commit.get_commits()
+    filtered_commits = []
 
-    for cid, cdata in reversed(commits.items()):
-        message = cdata['message']
-        date = cdata['date']
+    for cid, cdata in reversed(commits.items()):    
+        if filter_by_name:
+            if cdata['author'] == filter_by_name:
+                filtered_commits.append((cid, cdata))
+        elif filter_by_email:
+            if cdata['author_email'] == filter_by_email:
+                filtered_commits.append((cid, cdata))
+        else:
+            filtered_commits.append((cid, cdata))
+
+    for cid, cdata in filtered_commits:
+        author_email = cdata['author_email']
         files = len(cdata['objects'])
+        message = cdata['message']
         author = cdata['author']
-        author_email = cdata['author_email']
+        date = cdata['date']
+
         print(f'{files} file(s) in \033[34;4m{cid[:7]}\033[m by {author} <{author_email}> '
               f'({date}) \033[33m{repr(message)}\033[m')
 
 
 def _diff() -> None:
     tracked = tracker.get_tracked()
 
@@ -212,14 +224,17 @@
     parser.add_flag('-a', 'Select all files to tracking', action='store_true')
     parser.add_flag('-am', 'Commit all changed files add insert a message')
     parser.add_flag('-m', 'A short message to commit')
 
     parser.add_flag('--name', 'Set author name')
     parser.add_flag('--email', 'Set author email')
 
+    parser.add_flag('--filter-by-name', 'Filter log commit by author name')
+    parser.add_flag('--filter-by-email', 'Filter log commit by author email')
+
     args = parser.parse()
 
     if not args.init and not path.isdir(OBJECTS_PATH):
         print('\033[1;31mRepository not found\033[m')
         print('\033[33mCreate a repository with "init" command\033[m')
         sys.exit(1)
 
@@ -229,15 +244,15 @@
         if args.a:
             _add('*')
         else:
             _add(args.add)
     elif args.status:
         _status()
     elif args.log:
-        _log()
+        _log(args.filter_by_name, args.filter_by_email)
     elif args.commit is not None:
         if args.am:
             _commit('*', args.am)
         else:
             _commit(args.commit, args.m)
     elif args.diff:
         _diff()
```

### Comparing `box-vcs-0.1.0/box/_config.py` & `box-vcs-0.2.0/box/_config.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/box/commit.py` & `box-vcs-0.2.0/box/commit.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/box/exceptions.py` & `box-vcs-0.2.0/box/exceptions.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/box/ignore.py` & `box-vcs-0.2.0/box/ignore.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-from os import path as os_path, walk as os_walk
+import os
 
 
 def _filter_filelist(path: str) -> str:
-    if path.startswith('/'):
-        path = path[1:]
+    if not path.startswith('*'):
+        if path.startswith('/'):
+            path = path[1:]
 
-    return os_path.abspath(path)
+        return os.path.abspath(path)
+    else:
+        return path
 
 
 def _path_has_ignored(ignored: list, path: str) -> bool:
     for i in ignored:
-        if i in os_path.abspath(path):
+        if i in os.path.abspath(path):
             return True
 
 
 def _load_ignore() -> list:
     try:
         with open('.ignore', 'r') as ignore_file:
             filelist = ignore_file.readlines()
@@ -45,15 +48,19 @@
     return ignored
 
 
 def get_non_ignored() -> list:
     ignored = _load_ignore()
     non_ignored = []
 
-    for root, dirs, files in os_walk('.'):
+    for root, __, files in os.walk('.'):
         if not _path_has_ignored(ignored, root):
             for file in files:
-                filepath = os_path.join(root, file)
+                filepath = os.path.join(root, file)
                 if not _path_has_ignored(ignored, filepath):
                     non_ignored.append(filepath.replace('./', ''))
 
-    return non_ignored
+    ignore_with = [i.replace('*', '') for i in ignored if i.startswith('*')]
+    check_ignored = lambda f: not any([f.endswith(a) for a in ignore_with])
+    filtered_non_ignored = [f for f in non_ignored if check_ignored(f)]
+
+    return filtered_non_ignored
```

### Comparing `box-vcs-0.1.0/box/tracker.py` & `box-vcs-0.2.0/box/tracker.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/box/utils.py` & `box-vcs-0.2.0/box/utils.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/box_vcs.egg-info/PKG-INFO` & `box-vcs-0.2.0/box_vcs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-vcs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple and fast file versioning with Box
 Home-page: https://github.com/firlast/box
 Author: Firlast
 Author-email: firlastinc@gmail.com
 License: GNU GPLv2
 Keywords: version,control,versioning,vcs
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -22,15 +22,15 @@
 <p align="center">Fast and simple file versioning</p>
 
 <p align="center">
     <a href="https://github.com/firlast/box/releases">
         <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/firlast/box?include_prereleases">
     </a>
     <a href="https://github.com/firlast/box/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/box-vcs">
     </a>
 </p>
 
 Box is an open-source version control system **written in Python** that allows users to manage changes to their projects efficiently and collaboratively. With Box, you can control the history of **changes made to files**, track issues and bugs, and collaborate with other developers in a safe and secure environment. With an **intuitive interface** and customizable features, Box is a complete solution for development teams looking for an affordable and easy-to-use version control system. If you are looking for an efficient and organized way to manage your project versions, Box is a smart and affordable choice.
 
 ## Getting Started with Box
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: box-vcs Version: 0.1.0 Summary: Simple and fast
+Metadata-Version: 2.1 Name: box-vcs Version: 0.2.0 Summary: Simple and fast
 file versioning with Box Home-page: https://github.com/firlast/box Author:
 Firlast Author-email: firlastinc@gmail.com License: GNU GPLv2 Keywords:
 version,control,versioning,vcs Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
```

### Comparing `box-vcs-0.1.0/setup.py` & `box-vcs-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `box-vcs-0.1.0/tests/test_box.py` & `box-vcs-0.2.0/tests/test_box.py`

 * *Files identical despite different names*

