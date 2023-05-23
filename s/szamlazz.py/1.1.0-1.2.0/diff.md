# Comparing `tmp/szamlazz.py-1.1.0.tar.gz` & `tmp/szamlazz.py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szamlazz.py-1.1.0.tar", last modified: Sat Mar 11 13:08:14 2023, max compression
+gzip compressed data, was "szamlazz.py-1.2.0.tar", last modified: Tue May 23 18:12:51 2023, max compression
```

## Comparing `szamlazz.py-1.1.0.tar` & `szamlazz.py-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 13:08:14.569108 szamlazz.py-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-11 13:08:14.569108 szamlazz.py-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 13:08:14.565108 szamlazz.py-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/delete_pro_forma_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/generate_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/query_invoice_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/query_invoice_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/register_credit_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/examples/storno.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 13:08:14.569108 szamlazz.py-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 13:08:14.569108 szamlazz.py-1.1.0/szamlazz/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/szamlazz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20152 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/szamlazz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/szamlazz/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/szamlazz/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/szamlazz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    34736 2023-03-11 13:08:06.000000 szamlazz.py-1.1.0/szamlazz/xsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 13:08:14.569108 szamlazz.py-1.1.0/szamlazz.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-11 13:08:14.000000 szamlazz.py-1.1.0/szamlazz.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-11 13:08:14.000000 szamlazz.py-1.1.0/szamlazz.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 13:08:14.000000 szamlazz.py-1.1.0/szamlazz.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-11 13:08:14.000000 szamlazz.py-1.1.0/szamlazz.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-11 13:08:14.000000 szamlazz.py-1.1.0/szamlazz.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:12:51.460265 szamlazz.py-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-23 18:12:51.460265 szamlazz.py-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:12:51.460265 szamlazz.py-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/delete_pro_forma_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/generate_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/query_invoice_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/query_invoice_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/register_credit_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/examples/storno.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:12:51.460265 szamlazz.py-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:12:51.460265 szamlazz.py-1.2.0/szamlazz/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/szamlazz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/szamlazz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/szamlazz/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/szamlazz/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/szamlazz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34736 2023-05-23 18:12:40.000000 szamlazz.py-1.2.0/szamlazz/xsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:12:51.460265 szamlazz.py-1.2.0/szamlazz.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-23 18:12:51.000000 szamlazz.py-1.2.0/szamlazz.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-23 18:12:51.000000 szamlazz.py-1.2.0/szamlazz.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:12:51.000000 szamlazz.py-1.2.0/szamlazz.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 18:12:51.000000 szamlazz.py-1.2.0/szamlazz.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 18:12:51.000000 szamlazz.py-1.2.0/szamlazz.py.egg-info/top_level.txt
```

### Comparing `szamlazz.py-1.1.0/LICENSE` & `szamlazz.py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/PKG-INFO` & `szamlazz.py-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szamlazz.py
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python client for Szamlazz.hu :: Számla Agent
 Home-page: https://github.com/theriverman/szamlazz.py
 Author: Kristof Daja (theriverman)
 Author-email: kristof@daja.hu
 License: MIT License | Copyright (c) 2020 — 2023 Kristof Daja
 Project-URL: Bug Tracker, https://github.com/theriverman/szamlazz.py/issues
 Classifier: Environment :: Web Environment
```

### Comparing `szamlazz.py-1.1.0/README.md` & `szamlazz.py-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/examples/delete_pro_forma_invoice.py` & `szamlazz.py-1.2.0/examples/delete_pro_forma_invoice.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/examples/generate_invoice.py` & `szamlazz.py-1.2.0/examples/generate_invoice.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/examples/query_invoice_pdf.py` & `szamlazz.py-1.2.0/examples/query_invoice_pdf.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/examples/query_invoice_xml.py` & `szamlazz.py-1.2.0/examples/query_invoice_xml.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/examples/register_credit_entry.py` & `szamlazz.py-1.2.0/examples/register_credit_entry.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/examples/storno.py` & `szamlazz.py-1.2.0/examples/storno.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/setup.py` & `szamlazz.py-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_description_content_type="text/markdown",
     url='https://github.com/theriverman/szamlazz.py',
     project_urls={
         "Bug Tracker": "https://github.com/theriverman/szamlazz.py/issues",
     },
     install_requires=[
         'Jinja2~=3.1.2',
-        'requests~=2.28.2',
+        'requests>=2.31.0',
         'lxml~=4.9.2',
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `szamlazz.py-1.1.0/szamlazz/client.py` & `szamlazz.py-1.2.0/szamlazz/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,21 +445,20 @@
         :param template_data: (dict) Data injected into the Jinja2 compatible template XML template
         :param xsd_xml: [optional] The XSD Scheme for XSD scheme compliance check
         :param payload_extra_attachments: (dict) Extra data injected into the Jinja2 compatible template XML template
         :return: requests.models.Response
 
         Note: Use SzamlazzClient.get_basic_settings() as a skeleton while creating your own template_data. See `get_basic_settings` to learn what fields are available automatically
         """
-        logger.info(f"request_maker / action: {action}")
-        logger.info(f"request_maker / template: {template}")
-        logger.info(f"request_maker / template_data: {template_data}")
-        logger.info(f"request_maker / xsd_xml: {xsd_xml}")
-
-        template = Template(template)
-        output = template.render(template_data)
+        t = Template(template)
+        output = t.render(template_data)
+        logger.debug(f"request_maker / action: {action}")
+        logger.debug(f"request_maker / template: {template}")
+        logger.debug(f"request_maker / template_data: {template_data}")
+        logger.debug(f"request_maker / xsd_xml: {xsd_xml}")
         logger.debug(f"request_maker / Rendered Template Output: {output}")
 
         if xsd_xml != "":
             ok, err = xsd.validate(xml=output, xsd=xsd_xml)
             if not ok:
                 raise xsd.ValidationError(f"XML validation failed: " + err)
```

### Comparing `szamlazz.py-1.1.0/szamlazz/models.py` & `szamlazz.py-1.2.0/szamlazz/models.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/szamlazz/templates.py` & `szamlazz.py-1.2.0/szamlazz/templates.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/szamlazz/version.py` & `szamlazz.py-1.2.0/szamlazz/version.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/szamlazz/xsd.py` & `szamlazz.py-1.2.0/szamlazz/xsd.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.1.0/szamlazz.py.egg-info/PKG-INFO` & `szamlazz.py-1.2.0/szamlazz.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szamlazz.py
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python client for Szamlazz.hu :: Számla Agent
 Home-page: https://github.com/theriverman/szamlazz.py
 Author: Kristof Daja (theriverman)
 Author-email: kristof@daja.hu
 License: MIT License | Copyright (c) 2020 — 2023 Kristof Daja
 Project-URL: Bug Tracker, https://github.com/theriverman/szamlazz.py/issues
 Classifier: Environment :: Web Environment
```

### Comparing `szamlazz.py-1.1.0/szamlazz.py.egg-info/SOURCES.txt` & `szamlazz.py-1.2.0/szamlazz.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

