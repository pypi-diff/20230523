# Comparing `tmp/django-marion-howard-0.4.0.tar.gz` & `tmp/django-marion-howard-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-marion-howard-0.4.0.tar", last modified: Wed Dec 21 14:07:32 2022, max compression
+gzip compressed data, was "django-marion-howard-0.5.0.tar", last modified: Tue May 23 15:06:02 2023, max compression
```

## Comparing `django-marion-howard-0.4.0.tar` & `django-marion-howard-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      151 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1327 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      586 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.781249 django-marion-howard-0.4.0/django_marion_howard.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1327 2022-12-21 14:07:32.000000 django-marion-howard-0.4.0/django_marion_howard.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1007 2022-12-21 14:07:32.000000 django-marion-howard-0.4.0/django_marion_howard.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-12-21 14:07:32.000000 django-marion-howard-0.4.0/django_marion_howard.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2022-12-21 14:07:32.000000 django-marion-howard-0.4.0/django_marion_howard.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-12-21 14:07:32.000000 django-marion-howard-0.4.0/django_marion_howard.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-12-21 14:07:32.000000 django-marion-howard-0.4.0/django_marion_howard.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.781249 django-marion-howard-0.4.0/howard/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      539 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      577 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/defaults.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/howard/issuers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      223 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/issuers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1748 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/issuers/certificate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1928 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/issuers/invoice.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3568 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/issuers/realisation.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.781249 django-marion-howard-0.4.0/howard/locale/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.781249 django-marion-howard-0.4.0/howard/locale/fr_FR/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/howard/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1914 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2976 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.781249 django-marion-howard-0.4.0/howard/static/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/howard/static/howard/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4538 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/static/howard/logo-edx.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)    54828 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/static/howard/logo-fun.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25032 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/static/howard/logo-ministere-travail.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12105 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/static/howard/test-signature.png
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.781249 django-marion-howard-0.4.0/howard/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/howard/templates/howard/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2246 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templates/howard/certificate.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2488 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templates/howard/certificate.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4372 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templates/howard/invoice.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4968 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templates/howard/invoice.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2603 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templates/howard/realisation.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4341 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templates/howard/realisation.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/howard/templatetags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templatetags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      243 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/templatetags/howard_tags.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/howard/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2022-12-21 14:07:32.785249 django-marion-howard-0.4.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2022-12-21 14:07:31.000000 django-marion-howard-0.4.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.144068 django-marion-howard-0.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-05-23 15:06:02.144068 django-marion-howard-0.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/django_marion_howard.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-05-23 15:06:02.000000 django-marion-howard-0.5.0/django_marion_howard.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-23 15:06:02.000000 django-marion-howard-0.5.0/django_marion_howard.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 15:06:02.000000 django-marion-howard-0.5.0/django_marion_howard.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-23 15:06:02.000000 django-marion-howard-0.5.0/django_marion_howard.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-23 15:06:02.000000 django-marion-howard-0.5.0/django_marion_howard.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 15:06:02.000000 django-marion-howard-0.5.0/django_marion_howard.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      577 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/defaults.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/issuers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/issuers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/issuers/certificate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1928 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/issuers/invoice.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3568 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/issuers/realisation.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/locale/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/locale/fr_FR/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1914 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2976 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/static/howard/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4538 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/static/howard/logo-edx.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54828 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/static/howard/logo-fun.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25032 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/static/howard/logo-ministere-travail.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12105 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/static/howard/test-signature.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.140068 django-marion-howard-0.5.0/howard/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.144068 django-marion-howard-0.5.0/howard/templates/howard/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2246 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templates/howard/certificate.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2488 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templates/howard/certificate.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4372 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templates/howard/invoice.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templates/howard/invoice.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2603 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templates/howard/realisation.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4341 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templates/howard/realisation.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:02.144068 django-marion-howard-0.5.0/howard/templatetags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templatetags/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/templatetags/howard_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/howard/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-05-23 15:06:02.144068 django-marion-howard-0.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      149 2023-05-23 15:06:01.000000 django-marion-howard-0.5.0/setup.py
```

### Comparing `django-marion-howard-0.4.0/PKG-INFO` & `django-marion-howard-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: django-marion-howard
-Version: 0.4.0
+Version: 0.5.0
 Summary: FUN documents for Marion, the documents factory
 Home-page: https://github.com/openfun/marion
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
+Description: # Howard, FUN documents for Marion, The Documents Factory
+        
+        Howard is a collection of document issuers for
+        [Marion](https://openfun.github.io/marion).
+        
+        ## Contributing
+        
+        This project is intended to be community-driven, so please, do not hesitate to
+        get in touch if you have any questions related to our implementation or design
+        decisions.
+        
+        We try to raise our code quality standards and expect contributors to follow
+        the recommendations from our
+        [handbook](https://openfun.gitbooks.io/handbook/content).
+        
+        ## License
+        
+        This work is released under the MIT License (see [LICENSE](./LICENSE))
+        
 Keywords: Django,LMS,learning,PDF
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-
-# Howard, FUN documents for Marion, The Documents Factory
-
-Howard is a collection of document issuers for
-[Marion](https://openfun.github.io/marion).
-
-## Contributing
-
-This project is intended to be community-driven, so please, do not hesitate to
-get in touch if you have any questions related to our implementation or design
-decisions.
-
-We try to raise our code quality standards and expect contributors to follow
-the recommendations from our
-[handbook](https://openfun.gitbooks.io/handbook/content).
-
-## License
-
-This work is released under the MIT License (see [LICENSE](./LICENSE))
-
-
```

### Comparing `django-marion-howard-0.4.0/README.md` & `django-marion-howard-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/django_marion_howard.egg-info/PKG-INFO` & `django-marion-howard-0.5.0/django_marion_howard.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: django-marion-howard
-Version: 0.4.0
+Version: 0.5.0
 Summary: FUN documents for Marion, the documents factory
 Home-page: https://github.com/openfun/marion
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
+Description: # Howard, FUN documents for Marion, The Documents Factory
+        
+        Howard is a collection of document issuers for
+        [Marion](https://openfun.github.io/marion).
+        
+        ## Contributing
+        
+        This project is intended to be community-driven, so please, do not hesitate to
+        get in touch if you have any questions related to our implementation or design
+        decisions.
+        
+        We try to raise our code quality standards and expect contributors to follow
+        the recommendations from our
+        [handbook](https://openfun.gitbooks.io/handbook/content).
+        
+        ## License
+        
+        This work is released under the MIT License (see [LICENSE](./LICENSE))
+        
 Keywords: Django,LMS,learning,PDF
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-
-# Howard, FUN documents for Marion, The Documents Factory
-
-Howard is a collection of document issuers for
-[Marion](https://openfun.github.io/marion).
-
-## Contributing
-
-This project is intended to be community-driven, so please, do not hesitate to
-get in touch if you have any questions related to our implementation or design
-decisions.
-
-We try to raise our code quality standards and expect contributors to follow
-the recommendations from our
-[handbook](https://openfun.gitbooks.io/handbook/content).
-
-## License
-
-This work is released under the MIT License (see [LICENSE](./LICENSE))
-
-
```

### Comparing `django-marion-howard-0.4.0/django_marion_howard.egg-info/SOURCES.txt` & `django-marion-howard-0.5.0/django_marion_howard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/__init__.py` & `django-marion-howard-0.5.0/howard/__init__.py`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/defaults.py` & `django-marion-howard-0.5.0/howard/defaults.py`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/issuers/certificate.py` & `django-marion-howard-0.5.0/howard/issuers/certificate.py`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/issuers/invoice.py` & `django-marion-howard-0.5.0/howard/issuers/invoice.py`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/issuers/realisation.py` & `django-marion-howard-0.5.0/howard/issuers/realisation.py`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/locale/fr_FR/LC_MESSAGES/django.mo` & `django-marion-howard-0.5.0/howard/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/locale/fr_FR/LC_MESSAGES/django.po` & `django-marion-howard-0.5.0/howard/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/static/howard/logo-edx.svg` & `django-marion-howard-0.5.0/howard/static/howard/logo-edx.svg`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/static/howard/logo-fun.png` & `django-marion-howard-0.5.0/howard/static/howard/logo-fun.png`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/static/howard/logo-ministere-travail.svg` & `django-marion-howard-0.5.0/howard/static/howard/logo-ministere-travail.svg`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/static/howard/test-signature.png` & `django-marion-howard-0.5.0/howard/static/howard/test-signature.png`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/templates/howard/certificate.css` & `django-marion-howard-0.5.0/howard/templates/howard/certificate.css`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/templates/howard/certificate.html` & `django-marion-howard-0.5.0/howard/templates/howard/certificate.html`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/templates/howard/invoice.css` & `django-marion-howard-0.5.0/howard/templates/howard/invoice.css`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/templates/howard/invoice.html` & `django-marion-howard-0.5.0/howard/templates/howard/invoice.html`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/templates/howard/realisation.css` & `django-marion-howard-0.5.0/howard/templates/howard/realisation.css`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/howard/templates/howard/realisation.html` & `django-marion-howard-0.5.0/howard/templates/howard/realisation.html`

 * *Files identical despite different names*

### Comparing `django-marion-howard-0.4.0/setup.cfg` & `django-marion-howard-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-marion-howard
-version = 0.4.0
+version = 0.5.0
 description = FUN documents for Marion, the documents factory
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://github.com/openfun/marion
 license = MIT
@@ -19,15 +19,15 @@
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 
 [options]
 include_package_data = True
 install_requires = 
-	django-marion>=0.4.0
+	django-marion>=0.5.0
 packages = find:
 zip_safe = True
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
```

