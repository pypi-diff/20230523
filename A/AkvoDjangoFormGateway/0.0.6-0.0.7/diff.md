# Comparing `tmp/AkvoDjangoFormGateway-0.0.6.tar.gz` & `tmp/AkvoDjangoFormGateway-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoDjangoFormGateway-0.0.6.tar", last modified: Mon May 22 16:17:20 2023, max compression
+gzip compressed data, was "AkvoDjangoFormGateway-0.0.7.tar", last modified: Tue May 23 14:48:33 2023, max compression
```

## Comparing `AkvoDjangoFormGateway-0.0.6.tar` & `AkvoDjangoFormGateway-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.513941 AkvoDjangoFormGateway-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-23 14:48:33.513941 AkvoDjangoFormGateway-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-23 14:48:33.513941 AkvoDjangoFormGateway-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.509941 AkvoDjangoFormGateway-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.509941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.509941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.509941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.509941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.513941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.513941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-23 14:48:14.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:48:33.509941 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-23 14:48:33.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-23 14:48:33.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:48:33.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:48:33.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-23 14:48:33.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 14:48:33.000000 AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/top_level.txt
```

### Comparing `AkvoDjangoFormGateway-0.0.6/LICENSE` & `AkvoDjangoFormGateway-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/PKG-INFO` & `AkvoDjangoFormGateway-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.6/README.md` & `AkvoDjangoFormGateway-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/setup.py` & `AkvoDjangoFormGateway-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/feed.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 class Feed:
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
 
     def __init__(self):
         self.welcome = ["hi", "hello", "info"]
 
-    def get_init_survey_session(self, text: str, form: Forms = None):
+    def get_init_survey_session(self, text: str):
         init = False
-        form_id = form.id if form else None
-        if "#" in text and not form:
+        form_id = None
+        if "#" in text:
             info = str(text).split("#")
             form_id = info[1]
             init = len(info) == 2 and str(info[0]).lower() == "ready"
         return init, form_id
 
     def get_form(self, form_id: int = None, data: FormData = None) -> Forms:
         survey = None
```

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/0001_initial.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/models.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     created = models.DateTimeField(auto_now_add=True)
     updated = models.DateTimeField(default=None, null=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
+        ordering = ["id"]
         db_table = "ag_data"
 
 
 class AkvoGatewayAnswer(models.Model):
     data = models.ForeignKey(
         to=AkvoGatewayData,
         on_delete=models.CASCADE,
```

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/serializers.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/serializers.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_init.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_init.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.test import TestCase, Client
 from django.core.management import call_command
 from AkvoDjangoFormGateway.feed import Feed
 from AkvoDjangoFormGateway.models import (
     AkvoGatewayQuestion as Questions,
     AkvoGatewayAnswer as Answers,
 )
+from AkvoDjangoFormGateway.serializers import TwilioSerializer
 
 client = Client()
 feed = Feed()
 # Tests
 # consider that 8 digit phone number will
 # skip to send twillio message
 phone_number = "12345678"
@@ -45,16 +46,17 @@
         init, form_id = feed.get_init_survey_session(text=reply_text)
         json_form = {"Body": reply_text, "From": f"whatsapp:+{phone_number}"}
         response = client.post("/api/gateway/twilio/", json_form)
         self.assertEqual(response.status_code, 200)
 
         datapoint = feed.get_draft_datapoint(phone=phone_number)
         survey = feed.get_form(form_id=form_id, data=datapoint)
-        # First question
         question = feed.get_question(form=survey)
+        # First question shown when survey session started
+        # This response related to line code: 47
         self.assertEqual(response.json(), f"{question.order}. {question.text}")
 
         # datapoint is exist
         self.assertEqual(datapoint.phone, phone_number)
         # Form id equal with datapoint
         self.assertEqual(survey.id, datapoint.form.id)
 
@@ -73,23 +75,43 @@
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "MediaUrl0": image,
         }
         response = client.post("/api/gateway/twilio/", json_form)
         self.assertEqual(response.status_code, 400)
+        serializer = TwilioSerializer(data=json_form)
+        self.assertFalse(serializer.is_valid())
+        self.assertEqual(
+            response.json(),
+            {
+                "non_field_errors": [
+                    "MediaContentType0 is required when MediaUrl0 is present."
+                ]
+            },
+        )
 
         image_type = "image/png"
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "MediaContentType0": image_type,
         }
         response = client.post("/api/gateway/twilio/", json_form)
         self.assertEqual(response.status_code, 400)
+        serializer = TwilioSerializer(data=json_form)
+        self.assertFalse(serializer.is_valid())
+        self.assertEqual(
+            response.json(),
+            {
+                "non_field_errors": [
+                    "MediaUrl0 is required when MediaContentType0 is present."
+                ]
+            },
+        )
 
         # Answer right photo question
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "MediaContentType0": image_type,
             "MediaUrl0": image,
@@ -122,28 +144,48 @@
         text = feed.get_answer_text(
             body=None,
             image_url=None,
             lat=lat,
         )
         response = client.post("/api/gateway/twilio/", json_form)
         self.assertEqual(response.status_code, 400)
+        serializer = TwilioSerializer(data=json_form)
+        self.assertFalse(serializer.is_valid())
+        self.assertEqual(
+            response.json(),
+            {
+                "non_field_errors": [
+                    "Longitude is required when Latitude is present."
+                ]
+            },
+        )
 
         lng = "10.11"
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "Longitude": lng,
         }
         text = feed.get_answer_text(
             body=None,
             image_url=None,
             lng=lng,
         )
         response = client.post("/api/gateway/twilio/", json_form)
         self.assertEqual(response.status_code, 400)
+        serializer = TwilioSerializer(data=json_form)
+        self.assertFalse(serializer.is_valid())
+        self.assertEqual(
+            response.json(),
+            {
+                "non_field_errors": [
+                    "Latitude is required when Longitude is present."
+                ]
+            },
+        )
 
         # Answer GPS question
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "Latitude": lat,
             "Longitude": lng,
@@ -244,14 +286,15 @@
             ),
             True,
         )
         answer = Answers.objects.filter(
             data=datapoint, question=question
         ).first()
         self.assertEqual(answer.name, reply_text)
+        self.assertEqual(response.json(), "Thank you!")
 
     def test_show_options(self):
         opt_question = Questions.objects.get(pk=5)
         opt_question_output = "\n- option 1\n- option 2\n"
         self.assertEqual(
             feed.show_options(question=opt_question), opt_question_output
         )
@@ -274,29 +317,7 @@
         test3 = "1"
         init, form_id = feed.get_init_survey_session(text=test1)
         self.assertEqual(init, True)
         init, form_id = feed.get_init_survey_session(text=test2)
         self.assertEqual(init, False)
         init, form_id = feed.get_init_survey_session(text=test3)
         self.assertEqual(init, False)
-
-    def test_instance_request(self):
-        form_id = 1
-
-        json_form = {}
-        response = client.post(
-            f"/api/gateway/twilio/{form_id}?format=json", json_form
-        )
-        self.assertEqual(response.status_code, 200)
-        # first question shown
-        fq = Questions.objects.filter(form=form_id).order_by("order").first()
-
-        reply_text = "answer first question"
-        json_form = {"Body": reply_text, "From": f"whatsapp:+{phone_number}"}
-
-        response = client.post(f"/api/gateway/twilio/{form_id}", json_form)
-        datapoint = feed.get_draft_datapoint(phone=phone_number)
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(
-            feed.validate_answer(text=reply_text, question=fq, data=datapoint),
-            True,
-        )
```

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_validation.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/tests/tests_validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/urls.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/urls.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/functions.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/utils/functions.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/validation.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/utils/validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/views.py` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,34 +54,32 @@
         lng = serializer.validated_data.get("Longitude")
         text = feed.get_answer_text(
             body=body,
             image_url=image_url,
             lat=lat,
             lng=lng,
         )
-        init, form_id = feed.get_init_survey_session(
-            text=text, form=form_instance
-        )
+        init, form_id = feed.get_init_survey_session(text=text)
         datapoint = feed.get_draft_datapoint(phone=phone)
         survey = (
             form_instance
             if form_instance
             else feed.get_form(form_id=form_id, data=datapoint)
         )
         lq = feed.get_question(form=survey, data=datapoint)
         message = None
-        if text in feed.welcome and not datapoint:
+        if text in feed.welcome and not datapoint and not form_instance:
             message = feed.get_list_form()
 
-        if init and not datapoint:
-            dp_name = f"{survey.id}-{phone}"
+        new_datapoint = not datapoint and phone and len(str(phone).strip())
+        init_session = form_instance or init
+        if new_datapoint and init_session:
             # create new survey session by creating new datapoint
             FormData.objects.create(
                 form=survey,
-                name=dp_name,
                 phone=phone,
                 status=StatusTypes.draft,
             )
             message = f"{lq.order}. {lq.text}"
 
         if datapoint and lq:
             valid_answer = feed.validate_answer(
```

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/PKG-INFO` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt` & `AkvoDjangoFormGateway-0.0.7/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,11 +30,12 @@
 src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
 src/AkvoDjangoFormGateway/tests/tests_env.py
 src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
 src/AkvoDjangoFormGateway/tests/tests_init.py
 src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
 src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
 src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py
 src/AkvoDjangoFormGateway/tests/tests_validation.py
 src/AkvoDjangoFormGateway/utils/__init__.py
 src/AkvoDjangoFormGateway/utils/functions.py
 src/AkvoDjangoFormGateway/utils/validation.py
```

