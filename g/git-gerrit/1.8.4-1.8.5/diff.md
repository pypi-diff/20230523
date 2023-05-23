# Comparing `tmp/git_gerrit-1.8.4.tar.gz` & `tmp/git_gerrit-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_gerrit-1.8.4.tar", last modified: Wed Jun 22 19:56:05 2022, max compression
+gzip compressed data, was "git_gerrit-1.8.5.tar", last modified: Tue May 23 18:33:00 2023, max compression
```

## Comparing `git_gerrit-1.8.4.tar` & `git_gerrit-1.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2022-06-22 19:56:05.221786 git_gerrit-1.8.4/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1018 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/LICENSE.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       39 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/MANIFEST.in
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    17997 2022-06-22 19:56:05.221786 git_gerrit-1.8.4/PKG-INFO
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    14109 2022-06-22 19:54:26.000000 git_gerrit-1.8.4/README.rst
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2022-06-22 19:56:05.221786 git_gerrit-1.8.4/bin/
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      112 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-checkout
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      118 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-cherry-pick
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      106 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-fetch
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      104 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-help
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      122 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-install-hooks
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      102 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-log
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      106 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-query
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      108 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-review
--rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      112 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/bin/git-gerrit-unpicked
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2022-06-22 19:56:05.221786 git_gerrit-1.8.4/git_gerrit/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    17181 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/git_gerrit/__init__.py
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       23 2022-06-22 19:55:42.000000 git_gerrit-1.8.4/git_gerrit/_version.py
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    14324 2022-06-22 19:54:26.000000 git_gerrit-1.8.4/git_gerrit/cli.py
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     2544 2022-06-22 19:54:26.000000 git_gerrit-1.8.4/git_gerrit/config.py
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1536 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/git_gerrit/error.py
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     2554 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/git_gerrit/unicode.py
-drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2022-06-22 19:56:05.221786 git_gerrit-1.8.4/git_gerrit.egg-info/
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    17997 2022-06-22 19:56:05.000000 git_gerrit-1.8.4/git_gerrit.egg-info/PKG-INFO
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      546 2022-06-22 19:56:05.000000 git_gerrit-1.8.4/git_gerrit.egg-info/SOURCES.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        1 2022-06-22 19:56:05.000000 git_gerrit-1.8.4/git_gerrit.egg-info/dependency_links.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       13 2022-06-22 19:56:05.000000 git_gerrit-1.8.4/git_gerrit.egg-info/requires.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       11 2022-06-22 19:56:05.000000 git_gerrit-1.8.4/git_gerrit.egg-info/top_level.txt
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       38 2022-06-22 19:56:05.221786 git_gerrit-1.8.4/setup.cfg
--rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1282 2022-06-10 14:39:53.000000 git_gerrit-1.8.4/setup.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-05-23 18:33:00.072792 git_gerrit-1.8.5/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1018 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/LICENSE.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       39 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/MANIFEST.in
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    17997 2023-05-23 18:33:00.068791 git_gerrit-1.8.5/PKG-INFO
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    14109 2023-04-02 01:53:36.000000 git_gerrit-1.8.5/README.rst
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-05-23 18:33:00.068791 git_gerrit-1.8.5/bin/
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      112 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-checkout
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      118 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-cherry-pick
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      106 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-fetch
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      104 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-help
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      122 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-install-hooks
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      102 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-log
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      106 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-query
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      108 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-review
+-rwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)      112 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/bin/git-gerrit-unpicked
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-05-23 18:33:00.068791 git_gerrit-1.8.5/git_gerrit/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    17515 2023-05-23 13:48:47.000000 git_gerrit-1.8.5/git_gerrit/__init__.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       23 2023-05-23 13:00:02.000000 git_gerrit-1.8.5/git_gerrit/_version.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    14324 2023-05-23 13:11:10.000000 git_gerrit-1.8.5/git_gerrit/cli.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     2544 2023-04-02 01:53:36.000000 git_gerrit-1.8.5/git_gerrit/config.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1536 2022-06-10 14:39:53.000000 git_gerrit-1.8.5/git_gerrit/error.py
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     2554 2023-05-23 12:55:33.000000 git_gerrit-1.8.5/git_gerrit/unicode.py
+drwxrwxr-x   0 mmeffie   (1001) mmeffie   (1001)        0 2023-05-23 18:33:00.068791 git_gerrit-1.8.5/git_gerrit.egg-info/
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)    17997 2023-05-23 18:33:00.000000 git_gerrit-1.8.5/git_gerrit.egg-info/PKG-INFO
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)      546 2023-05-23 18:33:00.000000 git_gerrit-1.8.5/git_gerrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)        1 2023-05-23 18:33:00.000000 git_gerrit-1.8.5/git_gerrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       13 2023-05-23 18:33:00.000000 git_gerrit-1.8.5/git_gerrit.egg-info/requires.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       11 2023-05-23 18:33:00.000000 git_gerrit-1.8.5/git_gerrit.egg-info/top_level.txt
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)       38 2023-05-23 18:33:00.072792 git_gerrit-1.8.5/setup.cfg
+-rw-rw-r--   0 mmeffie   (1001) mmeffie   (1001)     1282 2023-01-02 20:34:32.000000 git_gerrit-1.8.5/setup.py
```

### Comparing `git_gerrit-1.8.4/LICENSE.txt` & `git_gerrit-1.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/PKG-INFO` & `git_gerrit-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: git_gerrit
-Version: 1.8.4
+Version: 1.8.5
 Summary: Gerrit review system command line tools.
 Home-page: https://github.com/meffie/git-gerrit
 Author: Michael Meffie
 Author-email: mmeffie@sinenomine.net
 License: BSD
 Description: git-gerrit
         ==========
```

### Comparing `git_gerrit-1.8.4/README.rst` & `git_gerrit-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/git_gerrit/__init__.py` & `git_gerrit-1.8.5/git_gerrit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -311,53 +311,61 @@
     args:
         number (int):     limit the log to these number of entries [optional]
         reverse (bool):   reverse log order
         shorthash (bool): short sha1
         revision (str):   git revision to log (default is HEAD)
         repodir (str):    local git repo directory (default: current)
     yields:
-        dictionary with keys: 'hash', 'subject', 'number'
+        dictionary with keys: 'hash', 'subject', 'number', 'author', 'email'
     """
     git = sh.Command('git').bake(_cwd=repodir, _tty_out=False)
 
     args = []
     if revision:
         args.append(revision)
 
     if shorthash:
         hashfmt = '%h'
     else:
         hashfmt = '%H'
     options = {}
-    options['pretty'] = 'hash:{0}%nsubject:%s%n%n%b%%%%'.format(hashfmt)
+    options['pretty'] = 'hash:{0}%nsubject:%s%nauthor:%an%nemail:%ae%n%b%%%%'.format(hashfmt)
     options['reverse'] = reverse
     if number:
         options['max-count'] = number
     options['_iter'] = True
 
-    fields = {'hash':'', 'subject':'', 'number':'-'}
+    fields = {'hash':'', 'subject':'', 'number':'-', 'author': '', 'email': ''}
     for line in git.log(*args, **options):
         line = cook(line)
         line = line.strip()
         m = re.match(r'^hash:(.*)', line)
         if m:
             fields['hash'] = m.group(1)
             continue
         m = re.match(r'^subject:(.*)', line)
         if m:
             fields['subject'] = m.group(1)
             continue
+        m = re.match(r'^author:(.*)', line)
+        if m:
+            fields['author'] = m.group(1)
+            continue
+        m = re.match(r'^email:(.*)', line)
+        if m:
+            fields['email'] = m.group(1)
+            continue
         m = re.match(r'^Reviewed-on: .*/([0-9]+)$', line)
         if m:
             fields['number'] = int(m.group(1)) # get last one
             continue
         m = re.match(r'^%%$', line)
         if m:
             yield fields
-            fields = {'hash':'', 'subject':'', 'number':'-'}
+            fields = {'hash':'', 'subject':'', 'number':'-', 'author': '', 'email': ''}
 
 def query(search, limit=None, details=False, repodir=None, **options):
     """Search gerrit for changes.
 
     args:
         search (str): one or more Gerrit search terms
         options (dict): zero or more Gerrit search options
```

### Comparing `git_gerrit-1.8.4/git_gerrit/cli.py` & `git_gerrit-1.8.5/git_gerrit/cli.py`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/git_gerrit/config.py` & `git_gerrit-1.8.5/git_gerrit/config.py`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/git_gerrit/error.py` & `git_gerrit-1.8.5/git_gerrit/error.py`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/git_gerrit/unicode.py` & `git_gerrit-1.8.5/git_gerrit/unicode.py`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/git_gerrit.egg-info/PKG-INFO` & `git_gerrit-1.8.5/git_gerrit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: git-gerrit
-Version: 1.8.4
+Version: 1.8.5
 Summary: Gerrit review system command line tools.
 Home-page: https://github.com/meffie/git-gerrit
 Author: Michael Meffie
 Author-email: mmeffie@sinenomine.net
 License: BSD
 Description: git-gerrit
         ==========
```

### Comparing `git_gerrit-1.8.4/git_gerrit.egg-info/SOURCES.txt` & `git_gerrit-1.8.5/git_gerrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git_gerrit-1.8.4/setup.py` & `git_gerrit-1.8.5/setup.py`

 * *Files identical despite different names*

