# Comparing `tmp/vedro-allure-reporter-1.6.0.tar.gz` & `tmp/vedro-allure-reporter-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-allure-reporter-1.6.0.tar", last modified: Sun Sep  4 13:41:18 2022, max compression
+gzip compressed data, was "vedro-allure-reporter-1.7.0.tar", last modified: Tue May 23 08:53:51 2023, max compression
```

## Comparing `vedro-allure-reporter-1.6.0.tar` & `vedro-allure-reporter-1.7.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 13:41:18.218202 vedro-allure-reporter-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-09-04 13:41:18.218202 vedro-allure-reporter-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-09-04 13:41:18.218202 vedro-allure-reporter-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 13:41:18.214202 vedro-allure-reporter-1.6.0/vedro_allure_reporter/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter/_allure_labels.py
--rw-r--r--   0 runner    (1001) docker     (121)    10295 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter/_allure_reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-04 13:41:09.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 13:41:18.218202 vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-09-04 13:41:18.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-09-04 13:41:18.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 13:41:18.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-04 13:41:18.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-04 13:41:18.000000 vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/tests/test_allure_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/tests/test_allure_reporter_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/vedro_allure_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:41.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:53:51.394274 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 08:53:51.000000 vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/top_level.txt
```

### Comparing `vedro-allure-reporter-1.6.0/LICENSE` & `vedro-allure-reporter-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.6.0/PKG-INFO` & `vedro-allure-reporter-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: vedro-allure-reporter
-Version: 1.6.0
+Version: 1.7.0
 Summary: Allure reporter for Vedro framework
-Home-page: https://github.com/nikitanovosibirsk/vedro-allure-reporter
+Home-page: https://github.com/vedro-universe/vedro-allure-reporter
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Allure Reporter
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-allure-reporter)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-allure-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-allure-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 
-[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://github.com/nikitanovosibirsk/vedro) framework
+[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) framework
 
 ## Installation
 
 ### 1. Install package
 
 ```shell
 $ pip3 install vedro-allure-reporter
@@ -76,14 +77,16 @@
 
 Docs — https://docs.qameta.io/allure-testops/quickstart/qa-auto/
 
 ## Documentation
 
 ### Custom Global Labels
 
+Global labels will be added to each scenario
+
 ```python
 # ./vedro.cfg.py
 import vedro
 import vedro_allure_reporter as allure_reporter
 from vedro_allure_reporter import AllureLabel
 
 class Config(vedro.Config):
@@ -96,14 +99,16 @@
             labels = [
                 AllureLabel("custom", "value")
             ]
 ```
 
 ### Custom Scenario Labels
 
+Scenario labels will be added to specific scenario
+
 ```python
 # ./scenarios/sign_up_user.py
 import vedro
 from vedro_allure_reporter import allure_labels, Story, AllureLabel
 
 @allure_labels(Story("Sign Up"), AllureLabel("custom", "value"))
 class Scenario(vedro.Scenario):
```

### Comparing `vedro-allure-reporter-1.6.0/README.md` & `vedro-allure-reporter-1.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Vedro Allure Reporter
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-allure-reporter)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-allure-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-allure-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 
-[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://github.com/nikitanovosibirsk/vedro) framework
+[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) framework
 
 ## Installation
 
 ### 1. Install package
 
 ```shell
 $ pip3 install vedro-allure-reporter
@@ -58,14 +58,16 @@
 
 Docs — https://docs.qameta.io/allure-testops/quickstart/qa-auto/
 
 ## Documentation
 
 ### Custom Global Labels
 
+Global labels will be added to each scenario
+
 ```python
 # ./vedro.cfg.py
 import vedro
 import vedro_allure_reporter as allure_reporter
 from vedro_allure_reporter import AllureLabel
 
 class Config(vedro.Config):
@@ -78,14 +80,16 @@
             labels = [
                 AllureLabel("custom", "value")
             ]
 ```
 
 ### Custom Scenario Labels
 
+Scenario labels will be added to specific scenario
+
 ```python
 # ./scenarios/sign_up_user.py
 import vedro
 from vedro_allure_reporter import allure_labels, Story, AllureLabel
 
 @allure_labels(Story("Sign Up"), AllureLabel("custom", "value"))
 class Scenario(vedro.Scenario):
```

### Comparing `vedro-allure-reporter-1.6.0/setup.cfg` & `vedro-allure-reporter-1.7.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.6.0
+current_version = 1.7.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-allure-reporter-1.6.0/setup.py` & `vedro-allure-reporter-1.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-allure-reporter",
-    version="1.6.0",
+    version="1.7.0",
     description="Allure reporter for Vedro framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
-    url="https://github.com/nikitanovosibirsk/vedro-allure-reporter",
+    url="https://github.com/vedro-universe/vedro-allure-reporter",
     license="Apache-2.0",
     packages=find_packages(exclude=("tests",)),
     package_data={"vedro_allure_reporter": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

### Comparing `vedro-allure-reporter-1.6.0/vedro_allure_reporter/_allure_labels.py` & `vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_labels.py`

 * *Files identical despite different names*

### Comparing `vedro-allure-reporter-1.6.0/vedro_allure_reporter/_allure_reporter.py` & `vedro-allure-reporter-1.7.0/vedro_allure_reporter/_allure_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,19 @@
         return labels
 
     def _get_scenario_tags(self, scenario: VirtualScenario) -> Tuple[str, ...]:
         return getattr(scenario._orig_scenario, "tags", ())
 
     def _get_scenario_labels(self, scenario: VirtualScenario) -> Tuple[Label, ...]:
         template = getattr(scenario._orig_scenario, "__vedro__template__", None)
-        return getattr(template or scenario._orig_scenario, "__vedro__allure_labels__", ())
+
+        labels = getattr(template, "__vedro__allure_labels__", ())
+        labels += getattr(scenario._orig_scenario, "__vedro__allure_labels__", ())
+
+        return labels
 
     def _create_attachment(self, name: str, mime_type: str, ext: str) -> AllureAttachment:
         file_name = ATTACHMENT_PATTERN.format(prefix=utils.uuid4(), ext=ext)
         return AllureAttachment(name=name, source=file_name, type=mime_type)
 
     def _add_memory_attachment(self, artifact: MemoryArtifact) -> AllureAttachment:
         guessed = guess_extension(artifact.mime_type)
@@ -230,9 +234,9 @@
 
     # Attach tags to Allure report
     attach_tags: bool = True
 
     # Attach artifacts to Allure report
     attach_artifacts: bool = True
 
-    # Add custom labels
+    # Add custom labels to each scenario
     labels: List[Label] = []
```

### Comparing `vedro-allure-reporter-1.6.0/vedro_allure_reporter.egg-info/PKG-INFO` & `vedro-allure-reporter-1.7.0/vedro_allure_reporter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: vedro-allure-reporter
-Version: 1.6.0
+Version: 1.7.0
 Summary: Allure reporter for Vedro framework
-Home-page: https://github.com/nikitanovosibirsk/vedro-allure-reporter
+Home-page: https://github.com/vedro-universe/vedro-allure-reporter
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Allure Reporter
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-allure-reporter)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-allure-reporter/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-allure-reporter)
 [![PyPI](https://img.shields.io/pypi/v/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-allure-reporter?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-allure-reporter.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-allure-reporter/)
 
-[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://github.com/nikitanovosibirsk/vedro) framework
+[Allure](https://docs.qameta.io/allure/) reporter for [Vedro](https://vedro.io/) framework
 
 ## Installation
 
 ### 1. Install package
 
 ```shell
 $ pip3 install vedro-allure-reporter
@@ -76,14 +77,16 @@
 
 Docs — https://docs.qameta.io/allure-testops/quickstart/qa-auto/
 
 ## Documentation
 
 ### Custom Global Labels
 
+Global labels will be added to each scenario
+
 ```python
 # ./vedro.cfg.py
 import vedro
 import vedro_allure_reporter as allure_reporter
 from vedro_allure_reporter import AllureLabel
 
 class Config(vedro.Config):
@@ -96,14 +99,16 @@
             labels = [
                 AllureLabel("custom", "value")
             ]
 ```
 
 ### Custom Scenario Labels
 
+Scenario labels will be added to specific scenario
+
 ```python
 # ./scenarios/sign_up_user.py
 import vedro
 from vedro_allure_reporter import allure_labels, Story, AllureLabel
 
 @allure_labels(Story("Sign Up"), AllureLabel("custom", "value"))
 class Scenario(vedro.Scenario):
```

