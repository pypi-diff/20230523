# Comparing `tmp/schatsi-0.1.8.tar.gz` & `tmp/schatsi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schatsi-0.1.8.tar", max compression
+gzip compressed data, was "schatsi-0.1.9.tar", max compression
```

## Comparing `schatsi-0.1.8.tar` & `schatsi-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      708 2022-12-06 21:56:15.686066 schatsi-0.1.8/README.md
--rw-r--r--   0        0        0      982 2022-12-06 21:57:52.826130 schatsi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/__init__.py
--rw-r--r--   0        0        0      971 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/cli.py
--rw-r--r--   0        0        0      141 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/jobs/__init__.py
--rw-r--r--   0        0        0     3560 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/jobs/base_job.py
--rw-r--r--   0        0        0     2219 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/jobs/parallel_job.py
--rw-r--r--   0        0        0     1730 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/jobs/single_job.py
--rw-r--r--   0        0        0       93 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/models/___init__.py
--rw-r--r--   0        0        0      724 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/models/document.py
--rw-r--r--   0        0        0      311 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/models/ranking.py
--rw-r--r--   0        0        0      892 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/processor/document_processor.py
--rw-r--r--   0        0        0      795 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/processor/ngram_processor.py
--rw-r--r--   0        0        0     2050 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/processor/ranker.py
--rw-r--r--   0        0        0     1040 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/processor/text_cleaner.py
--rw-r--r--   0        0        0        0 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/reader/__init__.py
--rw-r--r--   0        0        0      978 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/reader/base_reader.py
--rw-r--r--   0        0        0     1331 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/reader/pdf_reader.py
--rw-r--r--   0        0        0     1627 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/reader/reader_facade.py
--rw-r--r--   0        0        0      133 2022-12-06 21:56:15.894066 schatsi-0.1.8/src/schatsi/reader/reader_type.py
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 schatsi-0.1.8/setup.py
--rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 schatsi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      708 2022-12-06 22:01:18.662761 schatsi-0.1.9/README.md
+-rw-r--r--   0        0        0      982 2022-12-06 22:01:49.767090 schatsi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/__init__.py
+-rw-r--r--   0        0        0      971 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/cli.py
+-rw-r--r--   0        0        0      141 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/jobs/__init__.py
+-rw-r--r--   0        0        0     3560 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/jobs/base_job.py
+-rw-r--r--   0        0        0     2219 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/jobs/parallel_job.py
+-rw-r--r--   0        0        0     1730 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/jobs/single_job.py
+-rw-r--r--   0        0        0       93 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/models/___init__.py
+-rw-r--r--   0        0        0      724 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/models/document.py
+-rw-r--r--   0        0        0      311 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/models/ranking.py
+-rw-r--r--   0        0        0      892 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/processor/document_processor.py
+-rw-r--r--   0        0        0      795 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/processor/ngram_processor.py
+-rw-r--r--   0        0        0     2050 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/processor/ranker.py
+-rw-r--r--   0        0        0     1040 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/processor/text_cleaner.py
+-rw-r--r--   0        0        0        0 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/reader/__init__.py
+-rw-r--r--   0        0        0      978 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/reader/base_reader.py
+-rw-r--r--   0        0        0     1331 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/reader/pdf_reader.py
+-rw-r--r--   0        0        0     1627 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/reader/reader_facade.py
+-rw-r--r--   0        0        0      133 2022-12-06 22:01:18.858763 schatsi-0.1.9/src/schatsi/reader/reader_type.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 schatsi-0.1.9/setup.py
+-rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 schatsi-0.1.9/PKG-INFO
```

### Comparing `schatsi-0.1.8/README.md` & `schatsi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/pyproject.toml` & `schatsi-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schatsi"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["robnoflop <info@robertkasseck.de>"]
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/robnoflop/Schatsi"
 
 [tool.poetry.dependencies]
```

### Comparing `schatsi-0.1.8/src/schatsi/cli.py` & `schatsi-0.1.9/src/schatsi/cli.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/jobs/base_job.py` & `schatsi-0.1.9/src/schatsi/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/jobs/parallel_job.py` & `schatsi-0.1.9/src/schatsi/jobs/parallel_job.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/jobs/single_job.py` & `schatsi-0.1.9/src/schatsi/jobs/single_job.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/models/document.py` & `schatsi-0.1.9/src/schatsi/models/document.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/processor/document_processor.py` & `schatsi-0.1.9/src/schatsi/processor/document_processor.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/processor/ngram_processor.py` & `schatsi-0.1.9/src/schatsi/processor/ngram_processor.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/processor/ranker.py` & `schatsi-0.1.9/src/schatsi/processor/ranker.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/processor/text_cleaner.py` & `schatsi-0.1.9/src/schatsi/processor/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/reader/base_reader.py` & `schatsi-0.1.9/src/schatsi/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/reader/pdf_reader.py` & `schatsi-0.1.9/src/schatsi/reader/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/src/schatsi/reader/reader_facade.py` & `schatsi-0.1.9/src/schatsi/reader/reader_facade.py`

 * *Files identical despite different names*

### Comparing `schatsi-0.1.8/setup.py` & `schatsi-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'tqdm>=4.64.1,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['schatsi = schatsi.cli:cli']}
 
 setup_kwargs = {
     'name': 'schatsi',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# (f)SCHA.T.S.I\n\n(f)SCHA.T.S.I - An abbreviation for \'**f**aster **SCH**eduling *A*lgorithm for **T**ext **S**each **I**ntelligence\'.\n\n\n## Getting Started\nhttps://python-poetry.org/\npip install poetry  \npoetry install  \n\nGenerate documentation\n----------------------\n\nTheme documentation: https://sphinx-rtd-theme.readthedocs.io/en/stable/index.html\napidoc documentation: https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html\n\n\nos.environ["SPHINX_APIDOC_OPTIONS"]="members,show-inheritance"\n\nWindows\n\n```shell\ncd docs\nsphinx-apidoc -lfM -d 0 -o drg_analytic/ ../src/drg_analytic\n.\\make.bat html\n```\n\nMac/Linux\n\n```shell\ncd docs\nsphinx-apidoc -lfM -d 0 -o drg_analytic/ ../src/drg_analytic\nmake html\n```',
     'author': 'robnoflop',
     'author_email': 'info@robertkasseck.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/robnoflop/Schatsi',
```

### Comparing `schatsi-0.1.8/PKG-INFO` & `schatsi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schatsi
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/robnoflop/Schatsi
 Author: robnoflop
 Author-email: info@robertkasseck.de
 Requires-Python: >=3.9.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

