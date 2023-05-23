# Comparing `tmp/tvb-storage-2.7.3.tar.gz` & `tmp/tvb-storage-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-storage-2.7.3.tar", last modified: Thu Jan 26 10:59:36 2023, max compression
+gzip compressed data, was "tvb-storage-2.8.1.tar", last modified: Tue May 23 12:09:31 2023, max compression
```

## Comparing `tvb-storage-2.7.3.tar` & `tvb-storage-2.8.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.841456 tvb-storage-2.7.3/
--rw-r--r--   0 root         (0) root         (0)      249 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      838 2023-01-26 10:59:36.840456 tvb-storage-2.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      368 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 10:59:36.841456 tvb-storage-2.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2659 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.835456 tvb-storage-2.7.3/tvb/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.835456 tvb-storage-2.7.3/tvb/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.836455 tvb-storage-2.7.3/tvb/storage/h5/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.837456 tvb-storage-2.7.3/tvb/storage/h5/encryption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15487 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/encryption/data_encryption_handler.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/encryption/encryption_handler.py
--rw-r--r--   0 root         (0) root         (0)     7075 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/encryption/import_export_encryption_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.838456 tvb-storage-2.7.3/tvb/storage/h5/file/
--rw-r--r--   0 root         (0) root         (0)     1233 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/file/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15312 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/file/files_helper.py
--rw-r--r--   0 root         (0) root         (0)    27392 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/file/hdf5_storage_manager.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/file/xml_metadata_handlers.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/h5/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.838456 tvb-storage-2.7.3/tvb/storage/kube/
--rw-r--r--   0 root         (0) root         (0)     1236 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/kube/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3982 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/kube/kube_notifier.py
--rw-r--r--   0 root         (0) root         (0)    21924 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/storage/storage_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.834455 tvb-storage-2.7.3/tvb/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.839456 tvb-storage-2.7.3/tvb/tests/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.839456 tvb-storage-2.7.3/tvb/tests/storage/dummy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/dummy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/dummy/dummy_project.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/dummy/dummy_storage_data_h5.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/files_helper_test.py
--rw-r--r--   0 root         (0) root         (0)    21133 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/hdf5_storage_test.py
--rw-r--r--   0 root         (0) root         (0)     4405 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/storage_test.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/test_read.xml
--rw-r--r--   0 root         (0) root         (0)     3805 2023-01-20 05:55:06.000000 tvb-storage-2.7.3/tvb/tests/storage/xml_metadata_handlers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 10:59:36.840456 tvb-storage-2.7.3/tvb_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      838 2023-01-26 10:59:36.000000 tvb-storage-2.7.3/tvb_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1177 2023-01-26 10:59:36.000000 tvb-storage-2.7.3/tvb_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 10:59:36.000000 tvb-storage-2.7.3/tvb_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-01-26 10:59:36.000000 tvb-storage-2.7.3/tvb_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-26 10:59:36.000000 tvb-storage-2.7.3/tvb_storage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.804173 tvb-storage-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-23 12:09:31.804173 tvb-storage-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:31.804173 tvb-storage-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.796172 tvb-storage-2.8.1/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.797173 tvb-storage-2.8.1/tvb/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.797173 tvb-storage-2.8.1/tvb/storage/h5/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.798173 tvb-storage-2.8.1/tvb/storage/h5/encryption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15487 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/data_encryption_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/encryption_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7075 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/encryption/import_export_encryption_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.799173 tvb-storage-2.8.1/tvb/storage/h5/file/
+-rw-r--r--   0 root         (0) root         (0)     1233 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15312 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/files_helper.py
+-rw-r--r--   0 root         (0) root         (0)    27392 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/hdf5_storage_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/file/xml_metadata_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/h5/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.800173 tvb-storage-2.8.1/tvb/storage/kube/
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/kube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/kube/kube_notifier.py
+-rw-r--r--   0 root         (0) root         (0)    21924 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/storage/storage_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.794172 tvb-storage-2.8.1/tvb/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.802173 tvb-storage-2.8.1/tvb/tests/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.802173 tvb-storage-2.8.1/tvb/tests/storage/dummy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/dummy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_project.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_storage_data_h5.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/files_helper_test.py
+-rw-r--r--   0 root         (0) root         (0)    21133 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/hdf5_storage_test.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/storage_test.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/test_read.xml
+-rw-r--r--   0 root         (0) root         (0)     3805 2023-05-23 11:37:04.000000 tvb-storage-2.8.1/tvb/tests/storage/xml_metadata_handlers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:31.803173 tvb-storage-2.8.1/tvb_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:31.000000 tvb-storage-2.8.1/tvb_storage.egg-info/top_level.txt
```

### Comparing `tvb-storage-2.7.3/LICENSE` & `tvb-storage-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/PKG-INFO` & `tvb-storage-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-storage
-Version: 2.7.3
+Version: 2.8.1
 Summary: A package which handles the storage of TVB data
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain storage h5
```

### Comparing `tvb-storage-2.7.3/setup.py` & `tvb-storage-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     python setup.py install/develop
 """
 
 import os
 import shutil
 import setuptools
 
-STORAGE_VERSION = "2.7.3"
+STORAGE_VERSION = "2.8.1"
 
 STORAGE_TEAM = "Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze"
 
 STORAGE_REQUIRED_PACKAGES = ["cryptography", "h5py", "kubernetes", "numpy", "pyAesCrypt", "requests", 'tvb-library']
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as fd:
     DESCRIPTION = fd.read()
```

### Comparing `tvb-storage-2.7.3/tvb/__init__.py` & `tvb-storage-2.8.1/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/decorators.py` & `tvb-storage-2.8.1/tvb/storage/h5/decorators.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/encryption/data_encryption_handler.py` & `tvb-storage-2.8.1/tvb/storage/h5/encryption/data_encryption_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/encryption/encryption_handler.py` & `tvb-storage-2.8.1/tvb/storage/h5/encryption/encryption_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/encryption/import_export_encryption_handler.py` & `tvb-storage-2.8.1/tvb/storage/h5/encryption/import_export_encryption_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/file/__init__.py` & `tvb-storage-2.8.1/tvb/storage/h5/file/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/file/exceptions.py` & `tvb-storage-2.8.1/tvb/storage/h5/file/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/file/files_helper.py` & `tvb-storage-2.8.1/tvb/storage/h5/file/files_helper.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/file/hdf5_storage_manager.py` & `tvb-storage-2.8.1/tvb/storage/h5/file/hdf5_storage_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/file/xml_metadata_handlers.py` & `tvb-storage-2.8.1/tvb/storage/h5/file/xml_metadata_handlers.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/h5/utils.py` & `tvb-storage-2.8.1/tvb/storage/h5/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/kube/__init__.py` & `tvb-storage-2.8.1/tvb/storage/kube/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/kube/kube_notifier.py` & `tvb-storage-2.8.1/tvb/storage/kube/kube_notifier.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/storage/storage_interface.py` & `tvb-storage-2.8.1/tvb/storage/storage_interface.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/dummy/dummy_project.py` & `tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_project.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/dummy/dummy_storage_data_h5.py` & `tvb-storage-2.8.1/tvb/tests/storage/dummy/dummy_storage_data_h5.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/files_helper_test.py` & `tvb-storage-2.8.1/tvb/tests/storage/files_helper_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/hdf5_storage_test.py` & `tvb-storage-2.8.1/tvb/tests/storage/hdf5_storage_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/storage_test.py` & `tvb-storage-2.8.1/tvb/tests/storage/storage_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/test_read.xml` & `tvb-storage-2.8.1/tvb/tests/storage/test_read.xml`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb/tests/storage/xml_metadata_handlers_test.py` & `tvb-storage-2.8.1/tvb/tests/storage/xml_metadata_handlers_test.py`

 * *Files identical despite different names*

### Comparing `tvb-storage-2.7.3/tvb_storage.egg-info/PKG-INFO` & `tvb-storage-2.8.1/tvb_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-storage
-Version: 2.7.3
+Version: 2.8.1
 Summary: A package which handles the storage of TVB data
 Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Lia Domide, Paula Prodan, Bogdan Valean, Robert Vincze
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb brain storage h5
```

### Comparing `tvb-storage-2.7.3/tvb_storage.egg-info/SOURCES.txt` & `tvb-storage-2.8.1/tvb_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

