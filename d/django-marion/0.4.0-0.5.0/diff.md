# Comparing `tmp/django-marion-0.4.0.tar.gz` & `tmp/django-marion-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-marion-0.4.0.tar", last modified: Fri Aug  5 08:42:22 2022, max compression
+gzip compressed data, was "django-marion-0.5.0.tar", last modified: Tue May 23 15:06:34 2023, max compression
```

## Comparing `django-marion-0.4.0.tar` & `django-marion-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      151 2022-08-05 08:42:22.000000 django-marion-0.4.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1771 2022-08-05 08:42:22.929458 django-marion-0.4.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1000 2022-08-05 08:42:22.000000 django-marion-0.4.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.925459 django-marion-0.4.0/django_marion.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1771 2022-08-05 08:42:22.000000 django-marion-0.4.0/django_marion.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1070 2022-08-05 08:42:22.000000 django-marion-0.4.0/django_marion.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-05 08:42:22.000000 django-marion-0.4.0/django_marion.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2022-08-05 08:42:22.000000 django-marion-0.4.0/django_marion.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-08-05 08:42:22.000000 django-marion-0.4.0/django_marion.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-05 08:42:22.000000 django-marion-0.4.0/django_marion.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.925459 django-marion-0.4.0/marion/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      539 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/admin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/apps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1127 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/defaults.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1324 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      262 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/fields.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/issuers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       98 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/issuers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11540 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/issuers/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1290 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/issuers/dummy.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/migrations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2956 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/migrations/0001_initial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/migrations/0002_alter_documentrequest_issuer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/migrations/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8716 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/serializers.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.925459 django-marion-0.4.0/marion/static/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/static/marion/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/static/marion/noun_Check_3612574.svg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.925459 django-marion-0.4.0/marion/templates/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/templates/marion/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/templates/marion/dummy.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/templates/marion/dummy.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/tests/issuers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/issuers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16007 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/issuers/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1081 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/test_defaults.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      956 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/test_fields.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7800 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/test_models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/test_serializers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3205 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/test_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9623 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/tests/test_views.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-05 08:42:22.929458 django-marion-0.4.0/marion/urls/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/urls/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/urls/debug.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1599 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2242 2022-08-05 08:42:22.000000 django-marion-0.4.0/marion/views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1824 2022-08-05 08:42:22.929458 django-marion-0.4.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2022-08-05 08:42:22.000000 django-marion-0.4.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.081427 django-marion-0.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-05-23 15:06:33.000000 django-marion-0.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1998 2023-05-23 15:06:34.081427 django-marion-0.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1000 2023-05-23 15:06:33.000000 django-marion-0.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/django_marion.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1998 2023-05-23 15:06:34.000000 django-marion-0.5.0/django_marion.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-05-23 15:06:34.000000 django-marion-0.5.0/django_marion.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 15:06:34.000000 django-marion-0.5.0/django_marion.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-05-23 15:06:34.000000 django-marion-0.5.0/django_marion.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-23 15:06:34.000000 django-marion-0.5.0/django_marion.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-23 15:06:34.000000 django-marion-0.5.0/django_marion.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/marion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      249 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/defaults.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1324 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      262 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/factories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/fields.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/marion/issuers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/issuers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12625 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/issuers/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/issuers/dummy.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/marion/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/migrations/0002_alter_documentrequest_issuer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/migrations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8716 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/serializers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/marion/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/marion/static/marion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/static/marion/noun_Check_3612574.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.077427 django-marion-0.5.0/marion/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.081427 django-marion-0.5.0/marion/templates/marion/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2126 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/templates/marion/dummy.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1637 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/templates/marion/dummy.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.081427 django-marion-0.5.0/marion/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.081427 django-marion-0.5.0/marion/tests/issuers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/issuers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18984 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/issuers/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/test_defaults.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/test_fields.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7800 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/test_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/test_serializers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3205 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9623 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/tests/test_views.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-23 15:06:34.081427 django-marion-0.5.0/marion/urls/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/urls/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/urls/debug.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1564 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-23 15:06:33.000000 django-marion-0.5.0/marion/views.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1825 2023-05-23 15:06:34.081427 django-marion-0.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      149 2023-05-23 15:06:33.000000 django-marion-0.5.0/setup.py
```

### Comparing `django-marion-0.4.0/PKG-INFO` & `django-marion-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,43 @@
 Metadata-Version: 2.1
 Name: django-marion
-Version: 0.4.0
+Version: 0.5.0
 Summary: The documents factory
 Home-page: https://openfun.github.io/marion/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
+Description: # Marion, The Documents Factory
+        
+        Marion is a styled documents factory using HTML/CSS Django templates and a
+        headless browser that render them as PDF files. It can be used as a library or
+        an application in your Django project.
+        
+        ## Documentation
+        
+        We try our best to maintain an up-to-date reference documentation for this
+        project. If you intend to install, test or contribute to Marion or Howard, we
+        invite you to read this [documentation](https://openfun.github.io/marion) and
+        give us feedback if some parts are unclear or your use case is not (or poorly)
+        covered.
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
@@ -17,37 +45,7 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: sandbox
 Provides-Extra: ci
-
-# Marion, The Documents Factory
-
-Marion is a styled documents factory using HTML/CSS Django templates and a
-headless browser that render them as PDF files. It can be used as a library or
-an application in your Django project.
-
-## Documentation
-
-We try our best to maintain an up-to-date reference documentation for this
-project. If you intend to install, test or contribute to Marion or Howard, we
-invite you to read this [documentation](https://openfun.github.io/marion) and
-give us feedback if some parts are unclear or your use case is not (or poorly)
-covered.
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

### Comparing `django-marion-0.4.0/README.md` & `django-marion-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/django_marion.egg-info/PKG-INFO` & `django-marion-0.5.0/django_marion.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,43 @@
 Metadata-Version: 2.1
 Name: django-marion
-Version: 0.4.0
+Version: 0.5.0
 Summary: The documents factory
 Home-page: https://openfun.github.io/marion/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
+Description: # Marion, The Documents Factory
+        
+        Marion is a styled documents factory using HTML/CSS Django templates and a
+        headless browser that render them as PDF files. It can be used as a library or
+        an application in your Django project.
+        
+        ## Documentation
+        
+        We try our best to maintain an up-to-date reference documentation for this
+        project. If you intend to install, test or contribute to Marion or Howard, we
+        invite you to read this [documentation](https://openfun.github.io/marion) and
+        give us feedback if some parts are unclear or your use case is not (or poorly)
+        covered.
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
@@ -17,37 +45,7 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: sandbox
 Provides-Extra: ci
-
-# Marion, The Documents Factory
-
-Marion is a styled documents factory using HTML/CSS Django templates and a
-headless browser that render them as PDF files. It can be used as a library or
-an application in your Django project.
-
-## Documentation
-
-We try our best to maintain an up-to-date reference documentation for this
-project. If you intend to install, test or contribute to Marion or Howard, we
-invite you to read this [documentation](https://openfun.github.io/marion) and
-give us feedback if some parts are unclear or your use case is not (or poorly)
-covered.
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

### Comparing `django-marion-0.4.0/django_marion.egg-info/SOURCES.txt` & `django-marion-0.5.0/django_marion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/__init__.py` & `django-marion-0.5.0/marion/__init__.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/defaults.py` & `django-marion-0.5.0/marion/defaults.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/exceptions.py` & `django-marion-0.5.0/marion/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/fields.py` & `django-marion-0.5.0/marion/fields.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/issuers/base.py` & `django-marion-0.5.0/marion/issuers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.text import re_camel_case
 from django.utils.translation import gettext_lazy as _
 
 from pydantic import BaseModel
 from pydantic.error_wrappers import ValidationError
-from weasyprint import CSS, HTML
+from weasyprint import CSS, DEFAULT_OPTIONS, HTML
 from weasyprint.document import DocumentMetadata
 from weasyprint.text.fonts import FontConfiguration
 
 from marion import __version__ as marion_version
 
 from .. import defaults
 from ..exceptions import (
@@ -37,15 +37,14 @@
     authors = None
     description = None
     generator = f"Marion, version {marion_version}"
     keywords = None
     title = None
 
     def __init__(self):
-
         self._created = None
         self._metadata = None
         self._modified = None
 
     @property
     def metadata(self):
         """Get document PDF file metadata.
@@ -123,15 +122,14 @@
     # Models
     context_model: BaseModel = None
     context_query_model: BaseModel = None
 
     def __init__(
         self, identifier: uuid.UUID = None, context_query: Union[str, dict] = None
     ):
-
         # Document
         self.identifier = self.generate_identifier(identifier)
         self.document_path = self.get_document_path()
 
         # Data
         self.context = None
         self.context_query = (
@@ -321,15 +319,24 @@
         """Validate and set context passed as a dictionary instance"""
         self.context = self.validate_context(context)
 
     def get_django_context(self) -> Context:
         """Get the Django Context instance from the context model instance."""
         return Context(self.context.dict())
 
-    def create(self, persist=True):
+    @staticmethod
+    def _clean_pdf_options(options: dict) -> dict:
+        """Clean pdf options.
+
+        Remove any pdf options that is not in the DEFAULT_OPTIONS list.
+
+        """
+        return {key: value for key, value in options.items() if key in DEFAULT_OPTIONS}
+
+    def create(self, persist=True, pdf_options: DEFAULT_OPTIONS = None):
         """Create document.
 
         Given an HTML template, a CSS template and the required context to
         compile them, we render the document HTML that will be used by
         Weasyprint's headless web browser to generate the document as a PDF
         file.
 
@@ -340,14 +347,20 @@
             By default persist is True. In this way file is created and
             persisted into the document_path finally the path of the document is
             returned as a pathlib.Path instance.
 
             When persist is False, document is created without persisting. In
             this case create returns the PDF document as bytes.
 
+        - pdf_options<dict>
+
+            Additional options to pass to Weasyprint's write_pdf method.
+            Check to see all available options:
+            https://doc.courtbouillon.org/weasyprint/stable/api_reference.html#weasyprint.DEFAULT_OPTIONS
+
         """
 
         if self.context is None:
             self.set_context(self.fetch_context())
 
         django_context = self.get_django_context()
         html_str = self.get_html().render(django_context)
@@ -356,14 +369,26 @@
         font_config = FontConfiguration()
         html = HTML(string=html_str, url_fetcher=static_file_fetcher)
         css = CSS(string=css_str, font_config=font_config)
 
         document = html.render(stylesheets=[css], font_config=font_config)
         document.metadata = self.metadata
 
+        common_options = {"zoom": 1}
+        cleaned_pdf_options = (
+            self._clean_pdf_options(pdf_options) if pdf_options else {}
+        )
+
+        if "uncompressed_pdf" not in cleaned_pdf_options:
+            # MARK: Disable PDF compression by default until this issue is fixed:
+            # https://github.com/Kozea/WeasyPrint/issues/1885
+            cleaned_pdf_options["uncompressed_pdf"] = True
+
         if persist is False:
-            return document.write_pdf(zoom=1)
+            return document.write_pdf(**common_options, **cleaned_pdf_options)
 
         document_path = self.get_document_path()
-        document.write_pdf(target=document_path, zoom=1)
+        document.write_pdf(
+            target=document_path, **common_options, **cleaned_pdf_options
+        )
 
         return document_path
```

### Comparing `django-marion-0.4.0/marion/issuers/dummy.py` & `django-marion-0.5.0/marion/issuers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/migrations/0001_initial.py` & `django-marion-0.5.0/marion/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from django.db import migrations, models
 
 import marion.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="DocumentRequest",
```

### Comparing `django-marion-0.4.0/marion/migrations/0002_alter_documentrequest_issuer.py` & `django-marion-0.5.0/marion/migrations/0002_alter_documentrequest_issuer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import marion.fields
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("marion", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="documentrequest",
```

### Comparing `django-marion-0.4.0/marion/models.py` & `django-marion-0.5.0/marion/models.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/serializers.py` & `django-marion-0.5.0/marion/serializers.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/static/marion/noun_Check_3612574.svg` & `django-marion-0.5.0/marion/static/marion/noun_Check_3612574.svg`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/templates/marion/dummy.css` & `django-marion-0.5.0/marion/templates/marion/dummy.css`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/templates/marion/dummy.html` & `django-marion-0.5.0/marion/templates/marion/dummy.html`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/tests/issuers/test_base.py` & `django-marion-0.5.0/marion/tests/issuers/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from django.template import Context, Template, engines
 from django.template.engine import Engine
 
 import pytest
 from pdfminer.high_level import extract_text as pdf_extract_text
 from pydantic import BaseModel
-from weasyprint.document import DocumentMetadata
+from weasyprint.document import Document, DocumentMetadata
 
 from marion.defaults import DOCUMENTS_ROOT
 from marion.exceptions import (
     DocumentIssuerContextQueryValidationError,
     DocumentIssuerContextValidationError,
     DocumentIssuerMissingContext,
     DocumentIssuerMissingContextQuery,
@@ -272,15 +272,14 @@
 
     class ContextModel(BaseModel):
         fullname: str
         friends: int
 
     # pylint: disable=missing-class-docstring
     class TestDocument(AbstractDocument):
-
         context_model = ContextModel
 
         def fetch_context(self, **context_query):
             pass
 
     with pytest.raises(
         DocumentIssuerContextValidationError, match="value is not a valid integer"
@@ -314,15 +313,14 @@
     # pylint: disable=missing-class-docstring
     class ContextQueryModel(BaseModel):
         fullname: str
         friends: int
 
     # pylint: disable=missing-class-docstring
     class TestDocument(AbstractDocument):
-
         context_query_model = ContextQueryModel
 
         def fetch_context(self, **context_query):
             pass
 
     with pytest.raises(
         DocumentIssuerContextQueryValidationError,
@@ -346,15 +344,14 @@
     # pylint: disable=missing-class-docstring
     class ContextModel(BaseModel):
         fullname: str
         friends: int
 
     # pylint: disable=missing-class-docstring
     class TestDocument(AbstractDocument):
-
         context_model = ContextModel
 
         def fetch_context(self, **context_query):
             pass
 
     test_document = TestDocument()
 
@@ -468,14 +465,117 @@
 
     assert (
         pdf_extract_text(BytesIO(test_document_file)).strip()
         == "My name is Richie Cunningham (user id: rcunningham)"
     )
 
 
+def test_abstract_document_create_with_pdf_options():
+    """Test AbstractDocument create method with pdf_options"""
+
+    # pylint: disable=missing-class-docstring
+    class ContextModel(BaseModel):
+        pass
+
+    # pylint: disable=missing-class-docstring
+    class ContextQueryModel(BaseModel):
+        pass
+
+    class TestDocument(AbstractDocument):
+        context_model = ContextModel
+        context_query_model = ContextQueryModel
+
+        def get_html(self):
+            return Template("<body>An empty document</body>")
+
+        def get_css(self):
+            return Template("")
+
+        def fetch_context(self):
+            return {}
+
+    test_document = TestDocument()
+
+    with patch.object(Document, "write_pdf") as mocked_write_pdf:
+        test_document.create(
+            pdf_options={
+                "presentational_hints": True,
+                "pdf_version": "1.5",
+                "jpeg_quality": 50,
+                "optimize_images": True,
+            }
+        )
+
+    mocked_write_pdf.assert_called_once()
+    kwargs = mocked_write_pdf.call_args[1]
+
+    # PDF compression should be disabled by default
+    assert kwargs["uncompressed_pdf"] is True
+
+    assert kwargs["presentational_hints"] is True
+    assert kwargs["optimize_images"] is True
+    assert kwargs["pdf_version"] == "1.5"
+    assert kwargs["jpeg_quality"] == 50
+
+
+def test_abstract_document_clean_pdf_options():
+    """
+    When pdf_options are passed to the create method, they should be cleaned.
+    """
+
+    # pylint: disable=missing-class-docstring
+    class ContextModel(BaseModel):
+        pass
+
+    # pylint: disable=missing-class-docstring
+    class ContextQueryModel(BaseModel):
+        pass
+
+    class TestDocument(AbstractDocument):
+        context_model = ContextModel
+        context_query_model = ContextQueryModel
+
+        def get_html(self):
+            return Template("<body>An empty document</body>")
+
+        def get_css(self):
+            return Template("")
+
+        def fetch_context(self):
+            return {}
+
+    test_document = TestDocument()
+
+    with patch.object(Document, "write_pdf") as mocked_write_pdf:
+        test_document_file_path = test_document.create(
+            pdf_options={
+                "target": "unknown.pdf",
+                "zoom": 2,
+                "unknown_option": "unknown",
+                "jpeg_quality": 50,
+                "presentational_hints": True,
+                "uncompressed_pdf": False,
+            }
+        )
+
+    mocked_write_pdf.assert_called_once()
+    kwargs = mocked_write_pdf.call_args[1]
+
+    # Valid options should have been kept
+    assert kwargs["presentational_hints"] is True
+    assert kwargs["uncompressed_pdf"] is False
+    assert kwargs["jpeg_quality"] == 50
+
+    # Invalid options should have been removed
+    assert kwargs.get("unknown_option") is None
+    assert kwargs["zoom"] == 1
+    assert kwargs["target"] != "unknown.pdf"
+    assert kwargs["target"] == test_document_file_path
+
+
 def test_abstract_document_jinja_template_engine(settings):
     """Test document rendering with jinja templates"""
 
     settings.TEMPLATES = [
         {"BACKEND": "django.template.backends.django.DjangoTemplates", "DIRS": []},
         {"BACKEND": "django.template.backends.jinja2.Jinja2", "DIRS": []},
     ]
```

### Comparing `django-marion-0.4.0/marion/tests/test_defaults.py` & `django-marion-0.5.0/marion/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/tests/test_fields.py` & `django-marion-0.5.0/marion/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/tests/test_models.py` & `django-marion-0.5.0/marion/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/tests/test_serializers.py` & `django-marion-0.5.0/marion/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/tests/test_utils.py` & `django-marion-0.5.0/marion/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/tests/test_views.py` & `django-marion-0.5.0/marion/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/marion/utils.py` & `django-marion-0.5.0/marion/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Documents generation utilities."""
 
 import mimetypes
 from pathlib import Path
 from urllib.parse import urlparse
 
 from django.conf import settings
-from django.contrib.staticfiles.storage import get_storage_class
+from django.contrib.staticfiles.storage import storages
 from django.core.exceptions import SuspiciousFileOperation
 
 import weasyprint
 
-static_storage = get_storage_class(settings.STATICFILES_STORAGE)()
+static_storage = storages["staticfiles"]
 
 
 def static_file_fetcher(url, *args, **kwargs):
     """Weasyprint static files fetcher.
 
     If the file URL starts with 'file://', it will be fetched from the configured
     storage.
```

### Comparing `django-marion-0.4.0/marion/views.py` & `django-marion-0.5.0/marion/views.py`

 * *Files identical despite different names*

### Comparing `django-marion-0.4.0/setup.cfg` & `django-marion-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-marion
-version = 0.4.0
+version = 0.5.0
 description = The documents factory
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://openfun.github.io/marion/
 license = MIT
@@ -22,43 +22,43 @@
 
 [options]
 include_package_data = True
 install_requires = 
 	arrow>=1.0.0
 	djangorestframework>=3.12.0
 	pydantic>=1.8.0
-	WeasyPrint>=53.0
+	WeasyPrint>=59.0
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 dev = 
-	bandit==1.7.4
-	black==22.6.0
+	bandit==1.7.5
+	black==23.3.0
 	factory_boy==3.2.1
-	flake8==5.0.1
-	hypothesis[django]==6.53.0
-	isort==5.10.1
+	flake8==6.0.0
+	hypothesis[django]==6.75.3
+	isort==5.12.0
 	Jinja2==3.1.2
-	mkdocs==1.3.1
-	mkdocs-material==8.3.9
-	mkdocstrings==0.19.0
-	pdfminer.six==20220524
-	pyfakefs==4.6.3
-	pylint==2.14.5
+	mkdocs==1.4.3
+	mkdocs-material==9.1.12
+	mkdocstrings==0.21.2
+	pdfminer.six==20221105
+	pyfakefs==5.2.2
+	pylint==2.17.4
 	pylint-django==2.5.3
-	pytest==7.1.2
-	pytest-cov==3.0.0
+	pytest==7.3.1
+	pytest-cov==4.0.0
 	pytest-django==4.5.2
 sandbox = 
-	Django==4.0.6
-	django-configurations==2.3.2
-	psycopg2-binary==2.9.3
+	Django==4.2.1
+	django-configurations==2.4.1
+	psycopg2-binary==2.9.6
 ci = 
-	twine==4.0.1
+	twine==4.0.2
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 max-line-length = 88
 exclude =
```

