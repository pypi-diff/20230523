# Comparing `tmp/bytez-0.1.98.tar.gz` & `tmp/bytez-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytez-0.1.98.tar", last modified: Sat May 20 23:51:33 2023, max compression
+gzip compressed data, was "bytez-0.1.99.tar", last modified: Sat May 20 23:52:50 2023, max compression
```

## Comparing `bytez-0.1.98.tar` & `bytez-0.1.99.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:51:33.403843 bytez-0.1.98/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.98/README.md
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.98/bytez/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106246 2023-05-20 23:35:10.000000 bytez-0.1.98/bytez/exports.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1152 2023-05-17 01:52:53.000000 bytez-0.1.98/bytez/model.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.98/bytez/tasks/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/language_modelling/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.98/bytez/tasks/language_modelling/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/language_modelling/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.98/bytez/tasks/language_modelling/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1356 2023-05-20 01:55:06.000000 bytez-0.1.98/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:53:53.000000 bytez-0.1.98/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      357 2023-05-20 01:50:51.000000 bytez-0.1.98/bytez/tasks/language_modelling/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/style_transfer/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.98/bytez/tasks/style_transfer/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/style_transfer/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.98/bytez/tasks/style_transfer/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.98/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.98/bytez/tasks/style_transfer/_models/fast_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.98/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.98/bytez/tasks/style_transfer/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/super_resolution/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.98/bytez/tasks/super_resolution/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/super_resolution/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.98/bytez/tasks/super_resolution/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.98/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.98/bytez/tasks/super_resolution/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/text_summarization/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:10.000000 bytez-0.1.98/bytez/tasks/text_summarization/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez/tasks/text_summarization/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:10.000000 bytez-0.1.98/bytez/tasks/text_summarization/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.98/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.98/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2807 2023-05-20 23:51:27.000000 bytez-0.1.98/bytez/tasks/text_summarization/_models/hhousen_docsum.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      691 2023-05-20 23:40:28.000000 bytez-0.1.98/bytez/tasks/text_summarization/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:51:33.403843 bytez-0.1.98/bytez.egg-info/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:51:33.000000 bytez-0.1.98/bytez.egg-info/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1333 2023-05-20 23:51:33.000000 bytez-0.1.98/bytez.egg-info/SOURCES.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-20 23:51:33.000000 bytez-0.1.98/bytez.egg-info/dependency_links.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-20 23:51:33.000000 bytez-0.1.98/bytez.egg-info/requires.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-20 23:51:33.000000 bytez-0.1.98/bytez.egg-info/top_level.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-20 23:51:33.403843 bytez-0.1.98/setup.cfg
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-20 23:51:32.000000 bytez-0.1.98/setup.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:52:50.891219 bytez-0.1.99/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.99/README.md
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.99/bytez/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106246 2023-05-20 23:35:10.000000 bytez-0.1.99/bytez/exports.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1152 2023-05-17 01:52:53.000000 bytez-0.1.99/bytez/model.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.99/bytez/tasks/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/language_modelling/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.99/bytez/tasks/language_modelling/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/language_modelling/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.99/bytez/tasks/language_modelling/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1356 2023-05-20 01:55:06.000000 bytez-0.1.99/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:53:53.000000 bytez-0.1.99/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      357 2023-05-20 01:50:51.000000 bytez-0.1.99/bytez/tasks/language_modelling/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/style_transfer/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.99/bytez/tasks/style_transfer/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/style_transfer/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.99/bytez/tasks/style_transfer/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.99/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.99/bytez/tasks/style_transfer/_models/fast_style_transfer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.99/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.99/bytez/tasks/style_transfer/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/super_resolution/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.99/bytez/tasks/super_resolution/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/super_resolution/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.99/bytez/tasks/super_resolution/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.99/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.99/bytez/tasks/super_resolution/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/text_summarization/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:10.000000 bytez-0.1.99/bytez/tasks/text_summarization/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez/tasks/text_summarization/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:10.000000 bytez-0.1.99/bytez/tasks/text_summarization/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.99/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.99/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2774 2023-05-20 23:52:46.000000 bytez-0.1.99/bytez/tasks/text_summarization/_models/hhousen_docsum.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      691 2023-05-20 23:40:28.000000 bytez-0.1.99/bytez/tasks/text_summarization/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:52:50.891219 bytez-0.1.99/bytez.egg-info/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:52:50.000000 bytez-0.1.99/bytez.egg-info/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1333 2023-05-20 23:52:50.000000 bytez-0.1.99/bytez.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-20 23:52:50.000000 bytez-0.1.99/bytez.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-20 23:52:50.000000 bytez-0.1.99/bytez.egg-info/requires.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-20 23:52:50.000000 bytez-0.1.99/bytez.egg-info/top_level.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-20 23:52:50.891219 bytez-0.1.99/setup.cfg
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-20 23:52:50.000000 bytez-0.1.99/setup.py
```

### Comparing `bytez-0.1.98/bytez/exports.py` & `bytez-0.1.99/bytez/exports.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/model.py` & `bytez-0.1.99/bytez/model.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py` & `bytez-0.1.99/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/language_modelling/_models/hazyresearch_h3.py` & `bytez-0.1.99/bytez/tasks/language_modelling/_models/hazyresearch_h3.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/style_transfer/_models/cmd_style_transfer.py` & `bytez-0.1.99/bytez/tasks/style_transfer/_models/cmd_style_transfer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/style_transfer/_models/fast_style_transfer.py` & `bytez-0.1.99/bytez/tasks/style_transfer/_models/fast_style_transfer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py` & `bytez-0.1.99/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/style_transfer/models.py` & `bytez-0.1.99/bytez/tasks/style_transfer/models.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py` & `bytez-0.1.99/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py` & `bytez-0.1.99/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py` & `bytez-0.1.99/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez/tasks/text_summarization/_models/hhousen_docsum.py` & `bytez-0.1.99/bytez/tasks/text_summarization/_models/hhousen_docsum.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         Returns:
 
         - str: The output of the summarization. This is a dictionary of chapter and headings to summarized text.
         """
 
         request_params = {
             "input_pdf": input_pdf,
-            "preprocess": False,
             "model": model,
             "bart_checkpoint": bart_checkpoint,
             "bart_state_dict_key": bart_state_dict_key,
             "bart_fairseq": bart_fairseq,
             "chapter_heading_font": chapter_heading_font,
             "body_heading_font": body_heading_font,
             "body_font": body_font
```

### Comparing `bytez-0.1.98/bytez/tasks/text_summarization/models.py` & `bytez-0.1.99/bytez/tasks/text_summarization/models.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/bytez.egg-info/SOURCES.txt` & `bytez-0.1.99/bytez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytez-0.1.98/setup.py` & `bytez-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 packages = find_packages()
 
 
 setup(
     name='bytez',
-    version='0.1.98',
+    version='0.1.99',
     packages=packages,
     install_requires=[
         'charset-normalizer==3.1.0',
         'idna==3.4',
         'requests==2.28.2',
         'urllib3==1.26.15',
     ],
```

