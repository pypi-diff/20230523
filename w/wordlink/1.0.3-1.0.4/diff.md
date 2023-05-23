# Comparing `tmp/wordlink-1.0.3.tar.gz` & `tmp/wordlink-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordlink-1.0.3.tar", last modified: Mon May 22 21:55:49 2023, max compression
+gzip compressed data, was "wordlink-1.0.4.tar", last modified: Tue May 23 01:41:36 2023, max compression
```

## Comparing `wordlink-1.0.3.tar` & `wordlink-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 21:55:49.318490 wordlink-1.0.3/
--rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-22 21:55:49.318556 wordlink-1.0.3/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     3615 2023-05-22 21:54:44.000000 wordlink-1.0.3/readme.md
--rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-22 21:55:49.318804 wordlink-1.0.3/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-22 21:55:06.000000 wordlink-1.0.3/setup.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 21:55:49.317586 wordlink-1.0.3/wordlink/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-22 21:54:44.000000 wordlink-1.0.3/wordlink/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-22 21:54:44.000000 wordlink-1.0.3/wordlink/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 21:55:49.318406 wordlink-1.0.3/wordlink.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-22 21:55:49.000000 wordlink-1.0.3/wordlink.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      264 2023-05-22 21:55:49.000000 wordlink-1.0.3/wordlink.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-22 21:55:49.000000 wordlink-1.0.3/wordlink.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-22 21:55:49.000000 wordlink-1.0.3/wordlink.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-22 21:55:49.000000 wordlink-1.0.3/wordlink.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-22 21:55:49.000000 wordlink-1.0.3/wordlink.egg-info/top_level.txt
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-23 01:41:36.316065 wordlink-1.0.4/
+-rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-23 01:41:36.316230 wordlink-1.0.4/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     3615 2023-05-23 01:40:33.000000 wordlink-1.0.4/readme.md
+-rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-23 01:41:36.316517 wordlink-1.0.4/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-23 01:41:27.000000 wordlink-1.0.4/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-23 01:41:36.315030 wordlink-1.0.4/wordlink/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-22 21:54:44.000000 wordlink-1.0.4/wordlink/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-22 21:54:44.000000 wordlink-1.0.4/wordlink/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-23 01:41:36.315969 wordlink-1.0.4/wordlink.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      264 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-23 01:41:36.000000 wordlink-1.0.4/wordlink.egg-info/top_level.txt
```

### Comparing `wordlink-1.0.3/PKG-INFO` & `wordlink-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordlink
-Version: 1.0.3
+Version: 1.0.4
 Summary: Word Link Generator
 Home-page: https://github.com/psibir/wordlink
 Download-URL: https://github.com/psibir/wordlink/archive/v_01.tar.gz
 Author: Trevor Bloomfield
 Author-email: bloomfieldtm@gmail.com
 Keywords: word,link,html,console
 Classifier: Programming Language :: Python :: 3
@@ -76,15 +76,15 @@
 
 The tool includes a test suite to ensure its functionality. The `main_test.py` file contains the unit tests. Here's a description of what each test case in `main_test.py` is testing:
 
 - `test_find_word_locations`: This test verifies that the `find_word_locations` method correctly identifies the locations of the given search term within a test file.
 - `test_generate_links_output_file`: This test checks if the `generate_links` method generates the expected output file in HTML format when an output file name is provided.
 - `test_generate_links_console`: This test validates that the `generate_links` method produces the expected console output when no output file name is provided.
 
-To run the tests, navigate to the `/tests/` directpry and execute the following command:
+To run the tests, navigate to the `/tests/` directory and execute the following command:
 
 ```bash
 python3 main_test.py
 ```
 
 ## Limitations
```

### Comparing `wordlink-1.0.3/readme.md` & `wordlink-1.0.4/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 The tool includes a test suite to ensure its functionality. The `main_test.py` file contains the unit tests. Here's a description of what each test case in `main_test.py` is testing:
 
 - `test_find_word_locations`: This test verifies that the `find_word_locations` method correctly identifies the locations of the given search term within a test file.
 - `test_generate_links_output_file`: This test checks if the `generate_links` method generates the expected output file in HTML format when an output file name is provided.
 - `test_generate_links_console`: This test validates that the `generate_links` method produces the expected console output when no output file name is provided.
 
-To run the tests, navigate to the `/tests/` directpry and execute the following command:
+To run the tests, navigate to the `/tests/` directory and execute the following command:
 
 ```bash
 python3 main_test.py
 ```
 
 ## Limitations
```

### Comparing `wordlink-1.0.3/setup.cfg` & `wordlink-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.3/setup.py` & `wordlink-1.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wordlink',
-    version='1.0.3',
+    version='1.0.4',
     author='Trevor Bloomfield',
     author_email='bloomfieldtm@gmail.com',
     description='Word Link Generator',
     py_modules=['wordlink'],
     url = 'https://github.com/psibir/wordlink',   # Provide either the link to your github or to your website
     download_url = 'https://github.com/psibir/wordlink/archive/v_01.tar.gz',    # I explain this later on
     keywords = ['word', 'link', 'html', 'console'],   # Keywords that define your package best
```

### Comparing `wordlink-1.0.3/wordlink/__main__.py` & `wordlink-1.0.4/wordlink/__main__.py`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.3/wordlink.egg-info/PKG-INFO` & `wordlink-1.0.4/wordlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordlink
-Version: 1.0.3
+Version: 1.0.4
 Summary: Word Link Generator
 Home-page: https://github.com/psibir/wordlink
 Download-URL: https://github.com/psibir/wordlink/archive/v_01.tar.gz
 Author: Trevor Bloomfield
 Author-email: bloomfieldtm@gmail.com
 Keywords: word,link,html,console
 Classifier: Programming Language :: Python :: 3
@@ -76,15 +76,15 @@
 
 The tool includes a test suite to ensure its functionality. The `main_test.py` file contains the unit tests. Here's a description of what each test case in `main_test.py` is testing:
 
 - `test_find_word_locations`: This test verifies that the `find_word_locations` method correctly identifies the locations of the given search term within a test file.
 - `test_generate_links_output_file`: This test checks if the `generate_links` method generates the expected output file in HTML format when an output file name is provided.
 - `test_generate_links_console`: This test validates that the `generate_links` method produces the expected console output when no output file name is provided.
 
-To run the tests, navigate to the `/tests/` directpry and execute the following command:
+To run the tests, navigate to the `/tests/` directory and execute the following command:
 
 ```bash
 python3 main_test.py
 ```
 
 ## Limitations
```

