# Comparing `tmp/mobio-dedupe-sdk-test-1.0.8.tar.gz` & `tmp/mobio-dedupe-sdk-test-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-dedupe-sdk-test-1.0.8.tar", last modified: Tue May 23 09:17:07 2023, max compression
+gzip compressed data, was "mobio-dedupe-sdk-test-1.0.9.tar", last modified: Tue May 23 09:27:23 2023, max compression
```

## Comparing `mobio-dedupe-sdk-test-1.0.8.tar` & `mobio-dedupe-sdk-test-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:17:07.671445 mobio-dedupe-sdk-test-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 09:17:07.670445 mobio-dedupe-sdk-test-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:17:07.631444 mobio-dedupe-sdk-test-1.0.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:17:07.636444 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:17:07.654445 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/__init__.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/_init.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/_typing.py
--rw-r--r--   0 root         (0) root         (0)    55436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/api.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/backport.py
--rw-r--r--   0 root         (0) root         (0)    11058 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/blocking.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/canonical.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/canopy_index.py
--rw-r--r--   0 root         (0) root         (0)    12932 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/clustering.py
--rw-r--r--   0 root         (0) root         (0)    11718 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/convenience.py
--rw-r--r--   0 root         (0) root         (0)     9307 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/core.py
--rw-r--r--   0 root         (0) root         (0)     8410 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/datamodel.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/index.py
--rw-r--r--   0 root         (0) root         (0)    15883 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/labeler.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/levenshtein.py
--rw-r--r--   0 root         (0) root         (0)     6898 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/predicate_functions.py
--rw-r--r--   0 root         (0) root         (0)    11150 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/predicates.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/tfidf.py
--rw-r--r--   0 root         (0) root         (0)    14462 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:17:07.662445 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/base.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/categorical_type.py
--rw-r--r--   0 root         (0) root         (0)      390 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/exact.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/exists.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/interaction.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/latlong.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/price.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/set.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.8/mobio/sdks/dedupe/variables/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:17:07.669445 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 09:17:07.000000 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1334 2023-05-23 09:17:07.000000 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 09:17:07.000000 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 09:17:07.000000 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-23 09:17:07.000000 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 09:17:07.000000 mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 09:17:07.671445 mobio-dedupe-sdk-test-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10446 2023-05-23 09:17:06.000000 mobio-dedupe-sdk-test-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:27:23.433773 mobio-dedupe-sdk-test-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 09:27:23.432773 mobio-dedupe-sdk-test-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:27:23.419772 mobio-dedupe-sdk-test-1.0.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:27:23.419772 mobio-dedupe-sdk-test-1.0.9/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:27:23.427773 mobio-dedupe-sdk-test-1.0.9/mobio/sdks/dedupe/
+-rw-r--r--   0 root         (0) root         (0)   149524 2023-05-23 07:38:53.000000 mobio-dedupe-sdk-test-1.0.9/mobio/sdks/dedupe/cpredicates.c
+-rwxr-xr-x   0 root         (0) root         (0)   187160 2023-05-23 07:38:53.000000 mobio-dedupe-sdk-test-1.0.9/mobio/sdks/dedupe/cpredicates.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.9/mobio/sdks/dedupe/cpredicates.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:27:23.431773 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 09:27:23.000000 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-23 09:27:23.000000 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 09:27:23.000000 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 09:27:23.000000 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-23 09:27:23.000000 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 09:27:23.000000 mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 09:27:23.433773 mobio-dedupe-sdk-test-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    10335 2023-05-23 09:27:22.000000 mobio-dedupe-sdk-test-1.0.9/setup.py
```

### Comparing `mobio-dedupe-sdk-test-1.0.8/PKG-INFO` & `mobio-dedupe-sdk-test-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-dedupe-sdk-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio dedupe SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/PKG-INFO` & `mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-dedupe-sdk-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio dedupe SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-dedupe-sdk-test-1.0.8/mobio_dedupe_sdk_test.egg-info/requires.txt` & `mobio-dedupe-sdk-test-1.0.9/mobio_dedupe_sdk_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.8/setup.py` & `mobio-dedupe-sdk-test-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                         'pycodestyle==2.9.1', 'pycparser==2.21', 'pyflakes==2.5.0', 'pyhacrf-datamade==0.2.6',
                         'PyLBFGS==0.2.0.14', 'python-dateutil==2.8.2', 'scikit-learn==1.2.2', 'scipy==1.10.1',
                         'simplecosine==1.2', 'six==1.16.0', 'threadpoolctl==3.1.0', 'toml==0.10.2',
                         'typing_extensions==4.5.0', 'zope.index==6.0', 'zope.interface==6.0']
         return requirements
 
 
-version_dev='1.0.8'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_dev='1.0.9'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 version_prod='1.0.0'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -57,15 +57,15 @@
     name="mobio-dedupe-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.8',  # Required, Phần này cũng không được format file.
+    version='1.0.9',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio dedupe SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -136,18 +136,18 @@
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    packages=find_namespace_packages(include=["mobio.*"]),  # Required
-    package_data={"mobio": ['mobio/sdks/dedupe/cpredicates.c',
-                            "mobio/sdks/dedupe/cpredicates.cpython-38-x86_64-linux-gnu.so",
-                            "mobio/sdks/dedupe/cpredicates.pyx"]},  # Required
+    packages=["mobio"],  # Required
+    package_data={"mobio": ['sdks/dedupe/*.c',
+                            "sdks/dedupe/*.so",
+                            "sdks/dedupe/*.pyx"]},  # Required
     namespace_packages=["mobio"],  # Optional
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires=">=3",
     # This field lists other packages that your project depends on to run.
```

