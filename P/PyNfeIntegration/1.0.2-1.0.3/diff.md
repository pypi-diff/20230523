# Comparing `tmp/PyNfeIntegration-1.0.2.tar.gz` & `tmp/PyNfeIntegration-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNfeIntegration-1.0.2.tar", last modified: Tue May 23 21:28:21 2023, max compression
+gzip compressed data, was "PyNfeIntegration-1.0.3.tar", last modified: Tue May 23 21:35:47 2023, max compression
```

## Comparing `PyNfeIntegration-1.0.2.tar` & `PyNfeIntegration-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,44 @@
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/
--rw-rw-r--   0 cris      (1000) cris      (1000)     1078 2023-05-23 19:17:17.000000 PyNfeIntegration-1.0.2/LICENSE.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)      813 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/PKG-INFO
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/PyNfeIntegration.egg-info/
--rw-rw-r--   0 cris      (1000) cris      (1000)      813 2023-05-23 21:28:21.000000 PyNfeIntegration-1.0.2/PyNfeIntegration.egg-info/PKG-INFO
--rw-rw-r--   0 cris      (1000) cris      (1000)      382 2023-05-23 21:28:21.000000 PyNfeIntegration-1.0.2/PyNfeIntegration.egg-info/SOURCES.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)        1 2023-05-23 21:28:21.000000 PyNfeIntegration-1.0.2/PyNfeIntegration.egg-info/dependency_links.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)       17 2023-05-23 21:28:21.000000 PyNfeIntegration-1.0.2/PyNfeIntegration.egg-info/top_level.txt
--rw-rw-r--   0 cris      (1000) cris      (1000)      641 2023-05-23 18:22:56.000000 PyNfeIntegration-1.0.2/README.rst
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/pynfeintegration/
--rw-rw-r--   0 cris      (1000) cris      (1000)      120 2023-05-23 21:26:52.000000 PyNfeIntegration-1.0.2/pynfeintegration/__init__.py
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/pynfeintegration/certificates/
--rw-rw-r--   0 cris      (1000) cris      (1000)       44 2023-05-23 17:32:25.000000 PyNfeIntegration-1.0.2/pynfeintegration/certificates/__init__.py
--rw-rw-r--   0 cris      (1000) cris      (1000)     3517 2023-05-23 17:42:26.000000 PyNfeIntegration-1.0.2/pynfeintegration/certificates/pfx_certificate.py
-drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/pynfeintegration/nfe/
--rw-rw-r--   0 cris      (1000) cris      (1000)       68 2023-05-23 17:27:35.000000 PyNfeIntegration-1.0.2/pynfeintegration/nfe/__init__.py
--rw-rw-r--   0 cris      (1000) cris      (1000)     6019 2023-05-23 17:42:26.000000 PyNfeIntegration-1.0.2/pynfeintegration/nfe/nfe_requester.py
--rw-rw-r--   0 cris      (1000) cris      (1000)       38 2023-05-23 21:28:21.463559 PyNfeIntegration-1.0.2/setup.cfg
--rw-rw-r--   0 cris      (1000) cris      (1000)     1072 2023-05-23 21:28:18.000000 PyNfeIntegration-1.0.2/setup.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1078 2023-05-23 19:17:17.000000 PyNfeIntegration-1.0.3/LICENSE.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)      813 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/PKG-INFO
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/PyNfeIntegration.egg-info/
+-rw-rw-r--   0 cris      (1000) cris      (1000)      813 2023-05-23 21:35:47.000000 PyNfeIntegration-1.0.3/PyNfeIntegration.egg-info/PKG-INFO
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1299 2023-05-23 21:35:47.000000 PyNfeIntegration-1.0.3/PyNfeIntegration.egg-info/SOURCES.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)        1 2023-05-23 21:35:47.000000 PyNfeIntegration-1.0.3/PyNfeIntegration.egg-info/dependency_links.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)       17 2023-05-23 21:35:47.000000 PyNfeIntegration-1.0.3/PyNfeIntegration.egg-info/top_level.txt
+-rw-rw-r--   0 cris      (1000) cris      (1000)      641 2023-05-23 18:22:56.000000 PyNfeIntegration-1.0.3/README.rst
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/
+-rw-rw-r--   0 cris      (1000) cris      (1000)      120 2023-05-23 21:26:52.000000 PyNfeIntegration-1.0.3/pynfeintegration/__init__.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/base/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       23 2023-05-23 21:35:02.000000 PyNfeIntegration-1.0.3/pynfeintegration/base/__init__.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/base/classes/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       78 2023-05-23 17:34:25.000000 PyNfeIntegration-1.0.3/pynfeintegration/base/classes/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      129 2023-05-23 14:03:17.000000 PyNfeIntegration-1.0.3/pynfeintegration/base/classes/base_entity.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      583 2023-05-18 21:13:52.000000 PyNfeIntegration-1.0.3/pynfeintegration/base/classes/base_requester.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/certificates/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       44 2023-05-23 17:32:25.000000 PyNfeIntegration-1.0.3/pynfeintegration/certificates/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     3517 2023-05-23 17:42:26.000000 PyNfeIntegration-1.0.3/pynfeintegration/certificates/pfx_certificate.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/constantes/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       99 2023-05-23 17:36:08.000000 PyNfeIntegration-1.0.3/pynfeintegration/constantes/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      462 2023-05-18 21:17:07.000000 PyNfeIntegration-1.0.3/pynfeintegration/constantes/codes.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      222 2023-05-18 18:18:21.000000 PyNfeIntegration-1.0.3/pynfeintegration/constantes/contingency.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      358 2023-05-22 18:49:58.000000 PyNfeIntegration-1.0.3/pynfeintegration/constantes/name_spaces.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      111 2023-05-18 13:13:28.000000 PyNfeIntegration-1.0.3/pynfeintegration/constantes/versions.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/nfe/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       68 2023-05-23 17:27:35.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     6019 2023-05-23 17:42:26.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/nfe_requester.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/
+-rw-rw-r--   0 cris      (1000) cris      (1000)      277 2023-05-23 17:26:32.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      366 2023-05-23 15:13:18.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/nfe_xml_builder.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1128 2023-05-23 21:35:02.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/nfe_xml_builder_base.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1652 2023-05-23 17:42:26.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/nfe_xml_builder_distribution.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      614 2023-05-23 15:14:18.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/nfe_xml_builder_factory.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1004 2023-05-23 17:42:26.000000 PyNfeIntegration-1.0.3/pynfeintegration/nfe/xml_builders/nfe_xml_builder_status.py
+drwxrwxr-x   0 cris      (1000) cris      (1000)        0 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/pynfeintegration/webservices/
+-rw-rw-r--   0 cris      (1000) cris      (1000)       92 2023-05-23 17:38:26.000000 PyNfeIntegration-1.0.3/pynfeintegration/webservices/__init__.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)    11309 2023-05-23 17:20:43.000000 PyNfeIntegration-1.0.3/pynfeintegration/webservices/nfce.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     9741 2023-05-23 21:35:02.000000 PyNfeIntegration-1.0.3/pynfeintegration/webservices/nfe.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1027 2023-05-18 18:37:54.000000 PyNfeIntegration-1.0.3/pynfeintegration/webservices/nfse.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)      144 2023-05-18 21:44:10.000000 PyNfeIntegration-1.0.3/pynfeintegration/webservices/web_service_model.py
+-rw-rw-r--   0 cris      (1000) cris      (1000)       38 2023-05-23 21:35:47.757244 PyNfeIntegration-1.0.3/setup.cfg
+-rw-rw-r--   0 cris      (1000) cris      (1000)     1271 2023-05-23 21:35:38.000000 PyNfeIntegration-1.0.3/setup.py
```

### Comparing `PyNfeIntegration-1.0.2/LICENSE.txt` & `PyNfeIntegration-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyNfeIntegration-1.0.2/PKG-INFO` & `PyNfeIntegration-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNfeIntegration
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyNfeIntegration is a library that implement consults to invoices generate against some CNPJ
 Home-page: https://github.com/ADD01-TECH/py-nfe-integration
 Author: Cristiano dos Santos Lemos
 Author-email: cristianolemos@somma-it.com
 License: MIT
 Keywords: nfe,sped
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyNfeIntegration-1.0.2/PyNfeIntegration.egg-info/PKG-INFO` & `PyNfeIntegration-1.0.3/PyNfeIntegration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNfeIntegration
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyNfeIntegration is a library that implement consults to invoices generate against some CNPJ
 Home-page: https://github.com/ADD01-TECH/py-nfe-integration
 Author: Cristiano dos Santos Lemos
 Author-email: cristianolemos@somma-it.com
 License: MIT
 Keywords: nfe,sped
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyNfeIntegration-1.0.2/README.rst` & `PyNfeIntegration-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `PyNfeIntegration-1.0.2/pynfeintegration/certificates/pfx_certificate.py` & `PyNfeIntegration-1.0.3/pynfeintegration/certificates/pfx_certificate.py`

 * *Files identical despite different names*

### Comparing `PyNfeIntegration-1.0.2/pynfeintegration/nfe/nfe_requester.py` & `PyNfeIntegration-1.0.3/pynfeintegration/nfe/nfe_requester.py`

 * *Files identical despite different names*

### Comparing `PyNfeIntegration-1.0.2/setup.py` & `PyNfeIntegration-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="PyNfeIntegration",
-    version="1.0.2",
+    version="1.0.3",
     author="Cristiano dos Santos Lemos",
     author_email='cristianolemos@somma-it.com',
     keywords=['nfe', 'sped'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Intended Audience :: Developers',
@@ -15,15 +15,20 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     packages=[
         'pynfeintegration',
         'pynfeintegration.nfe',
-        'pynfeintegration.certificates'
+        'pynfeintegration.nfe.xml_builders',
+        'pynfeintegration.certificates',
+        'pynfeintegration.base',
+        'pynfeintegration.base.classes',
+        'pynfeintegration.constantes',
+        'pynfeintegration.webservices',
     ],
     url='https://github.com/ADD01-TECH/py-nfe-integration',
     license='MIT',
     description='PyNfeIntegration is a library that implement consults to invoices generate against some CNPJ',
     # long_description=open('README.rst').read(),
     requires=[
         'lxml(>=4.9.2)',
```

