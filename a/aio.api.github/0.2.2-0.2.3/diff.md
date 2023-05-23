# Comparing `tmp/aio.api.github-0.2.2.tar.gz` & `tmp/aio.api.github-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio.api.github-0.2.2.tar", last modified: Sun May 21 17:27:43 2023, max compression
+gzip compressed data, was "aio.api.github-0.2.3.tar", last modified: Tue May 23 17:56:59 2023, max compression
```

## Comparing `aio.api.github-0.2.2.tar` & `aio.api.github-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.692289 aio.api.github-0.2.2/aio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.692289 aio.api.github-0.2.2/aio/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio/api/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio/api/github/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio/api/github/abstract/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/issues/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/issues/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/abstract/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio/api/github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/aio.api.github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/aio.api.github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:27:43.696289 aio.api.github-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-21 17:27:43.000000 aio.api.github-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.372130 aio.api.github-0.2.3/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.372130 aio.api.github-0.2.3/aio/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/abstract/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio/api/github/abstract/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/issues/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/issues/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/abstract/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio/api/github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/aio.api.github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/aio.api.github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:56:59.376130 aio.api.github-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-23 17:56:59.000000 aio.api.github-0.2.3/setup.py
```

### Comparing `aio.api.github-0.2.2/aio/api/github/__init__.py` & `aio.api.github-0.2.3/aio/api/github/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,100 @@
 """aio.api.github."""
 
 from . import abstract
 from . import exceptions
 from . import interface
 from . import utils
 from .api import (
+    GithubActions,
     GithubAPI,
     GithubCommit,
     GithubIssue,
     GithubIssues,
     GithubIterator,
     GithubLabel,
     GithubRelease,
     GithubReleaseAssets,
     GithubRepo,
-    GithubTag)
+    GithubTag,
+    GithubWorkflows)
 from .abstract import (
+    AGithubActions,
     AGithubAPI,
     AGithubCommit,
     AGithubIssue,
     AGithubIssues,
     AGithubIssuesTracker,
     AGithubIterator,
     AGithubLabel,
     AGithubRelease,
     AGithubReleaseAssets,
     AGithubRepo,
     AGithubTag,
     AGithubTrackedIssue,
-    AGithubTrackedIssues)
+    AGithubTrackedIssues,
+    AGithubWorkflows)
 from .interface import (
+    IGithubActions,
     IGithubAPI,
     IGithubCommit,
     IGithubIssue,
     IGithubIssues,
     IGithubIssuesTracker,
     IGithubIterator,
     IGithubLabel,
     IGithubRelease,
     IGithubReleaseAssets,
     IGithubRepo,
     IGithubTag,
     IGithubTrackedIssue,
-    IGithubTrackedIssues)
+    IGithubTrackedIssues,
+    IGithubWorkflows)
 
 
 __all__ = (
     "abstract",
+    "AGithubActions",
     "AGithubAPI",
     "AGithubCommit",
     "AGithubIssue",
     "AGithubIssuesTracker",
     "AGithubIssues",
     "AGithubIterator",
     "AGithubLabel",
     "AGithubRelease",
     "AGithubReleaseAssets",
     "AGithubRepo",
     "AGithubTag",
     "AGithubTrackedIssue",
     "AGithubTrackedIssues",
+    "AGithubWorkflows",
     "exceptions",
+    "GithubActions",
     "GithubAPI",
     "GithubCommit",
     "GithubLabel",
     "GithubIssue",
     "GithubIssues",
     "GithubIterator",
     "GithubRelease",
     "GithubReleaseAssets",
     "GithubRepo",
     "GithubTag",
+    "GithubWorkflows",
+    "IGithubActions",
     "IGithubAPI",
     "IGithubCommit",
     "IGithubIssue",
     "IGithubIssues",
     "IGithubIssuesTracker",
     "IGithubIterator",
     "IGithubLabel",
     "IGithubRelease",
     "IGithubReleaseAssets",
     "IGithubRepo",
     "IGithubTag",
     "IGithubTrackedIssue",
     "IGithubTrackedIssues",
+    "IGithubWorkflows",
     "interface",
     "utils")
```

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/__init__.py` & `aio.api.github-0.2.3/aio/api/github/abstract/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from .actions import AGithubActions, AGithubWorkflows
 from .api import AGithubAPI
 from .commit import AGithubCommit
 from .issues import (
     AGithubIssue,
     AGithubIssues,
     AGithubIssuesTracker,
     AGithubTrackedIssue,
@@ -11,20 +12,22 @@
 from .label import AGithubLabel
 from .release import AGithubRelease, AGithubReleaseAssets
 from .repo import AGithubRepo
 from .tag import AGithubTag
 
 
 __all__ = (
+    "AGithubActions",
     "AGithubAPI",
     "AGithubCommit",
     "AGithubIssue",
     "AGithubIssues",
     "AGithubIssuesTracker",
     "AGithubIterator",
     "AGithubLabel",
     "AGithubRelease",
     "AGithubReleaseAssets",
     "AGithubRepo",
     "AGithubTag",
     "AGithubTrackedIssue",
-    "AGithubTrackedIssues")
+    "AGithubTrackedIssues",
+    "AGithubWorkflows")
```

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/api.py` & `aio.api.github-0.2.3/aio/api/github/abstract/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import abc
 from functools import cached_property
 from typing import Any, Type
 
 import aiohttp
 
 import gidgethub
+import gidgethub.abc
 import gidgethub.aiohttp
 
 import abstracts
 
 from aio.api.github import interface
 
 
@@ -31,14 +32,19 @@
         self.kwargs = kwargs
 
     def __getitem__(self, k) -> interface.IGithubRepo:
         # TODO: make this work with user and organization
         #  and validate `k`
         return self.repo_class(self, k)
 
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def actions_class(self) -> Type[interface.IGithubActions]:
+        raise NotImplementedError
+
     @cached_property
     def api(self) -> gidgethub.aiohttp.GitHubAPI:
         """Gidgethub API."""
         return self.api_class(
             self.session,
             *self.args,
             **self.kwargs)
@@ -94,14 +100,19 @@
         return self._session
 
     @property  # type:ignore
     @abstracts.interfacemethod
     def tag_class(self) -> Type[interface.IGithubTag]:
         raise NotImplementedError
 
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def workflows_class(self) -> Type[interface.IGithubWorkflows]:
+        raise NotImplementedError
+
     async def getitem(self, *args, **kwargs) -> Any:
         # print("GETITEM", args, kwargs)
         return await self.api.getitem(*args, **kwargs)
 
     def getiter(self, *args, **kwargs) -> interface.IGithubIterator:
         # print("GETITER", args, kwargs)
         return self.iterator_class(self.api, *args, **kwargs)
```

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/base.py` & `aio.api.github-0.2.3/aio/api/github/abstract/base.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/commit.py` & `aio.api.github-0.2.3/aio/api/github/abstract/commit.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/issues/issues.py` & `aio.api.github-0.2.3/aio/api/github/abstract/issues/issues.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/issues/tracker.py` & `aio.api.github-0.2.3/aio/api/github/abstract/issues/tracker.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/iterator.py` & `aio.api.github-0.2.3/aio/api/github/abstract/iterator.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/release.py` & `aio.api.github-0.2.3/aio/api/github/abstract/release.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/repo.py` & `aio.api.github-0.2.3/aio/api/github/abstract/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
         self._github = github
         self._name = name
 
     def __str__(self):
         return f"<{self.__class__.__name__} {self.name}>"
 
     @cached_property
+    def actions(self) -> "interface.IGithubActions":
+        return self.github.actions_class(repo=self)
+
+    @cached_property
     def github_path(self) -> pathlib.PurePosixPath:
         """Github API repos path."""
         return pathlib.PurePosixPath(f"/repos/{self.name}")
 
     @property
     def github(self) -> interface.IGithubAPI:
         return self._github
```

### Comparing `aio.api.github-0.2.2/aio/api/github/abstract/tag.py` & `aio.api.github-0.2.3/aio/api/github/abstract/tag.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/aio/api/github/api.py` & `aio.api.github-0.2.3/aio/api/github/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,39 @@
 from typing import Type
 
 import gidgethub.aiohttp
 
 import abstracts
 
 from .abstract import (
+    AGithubActions,
     AGithubAPI,
     AGithubCommit,
     AGithubIssue,
     AGithubIssues,
     AGithubIterator,
     AGithubLabel,
     AGithubRelease,
     AGithubReleaseAssets,
     AGithubRepo,
-    AGithubTag)
+    AGithubTag,
+    AGithubWorkflows)
 from . import interface
 
 
+@abstracts.implementer(AGithubActions)
+class GithubActions:
+    pass
+
+
+@abstracts.implementer(AGithubWorkflows)
+class GithubWorkflows:
+    pass
+
+
 @abstracts.implementer(AGithubCommit)
 class GithubCommit:
     pass
 
 
 @abstracts.implementer(AGithubIssue)
 class GithubIssue:
@@ -70,14 +82,18 @@
 @abstracts.implementer(AGithubAPI)
 class GithubAPI:
 
     def __init__(self, session, *args, **kwargs) -> None:
         AGithubAPI.__init__(self, session, *args, **kwargs)
 
     @property
+    def actions_class(self) -> Type[AGithubActions]:
+        return GithubActions
+
+    @property
     def api_class(self) -> Type[gidgethub.aiohttp.GitHubAPI]:
         return super().api_class
 
     @property
     def commit_class(self) -> Type[AGithubCommit]:
         return GithubCommit
 
@@ -104,7 +120,11 @@
     @property
     def repo_class(self) -> Type[AGithubRepo]:
         return GithubRepo
 
     @property
     def tag_class(self) -> Type[AGithubTag]:
         return GithubTag
+
+    @property
+    def workflows_class(self) -> Type[AGithubWorkflows]:
+        return GithubWorkflows
```

### Comparing `aio.api.github-0.2.2/aio/api/github/interface.py` & `aio.api.github-0.2.3/aio/api/github/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from datetime import datetime
 from typing import (
     Any, AsyncGenerator, Dict,
     Optional, Pattern, Tuple, Type)
 
 from packaging import version
 
+import gidgethub.abc
+
 import abstracts
 
 import aiohttp
 
 
 class IGithubCommit(metaclass=abstracts.Interface):
     pass
@@ -74,14 +76,26 @@
     @abstracts.interfacemethod
     def __getitem__(self, k: str) -> "IGithubRepo":
         """Return a `GithubRepository` for `k`"""
         raise NotImplementedError
 
     @property  # type:ignore
     @abstracts.interfacemethod
+    def api(self) -> Type[gidgethub.abc.GitHubAPI]:
+        """Github API."""
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def actions_class(self) -> Type["IGithubActions"]:
+        """Github actions class."""
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
     def commit_class(self) -> Type["IGithubCommit"]:
         """Github commit class."""
         raise NotImplementedError
 
     @property  # type:ignore
     @abstracts.interfacemethod
     def issue_class(self) -> Type["IGithubIssue"]:
@@ -138,14 +152,20 @@
         raise NotImplementedError
 
     @abstracts.interfacemethod
     async def post(self, *args, **kwargs) -> Any:
         """Call the `gidgethub.post` api."""
         raise NotImplementedError
 
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def workflows_class(self) -> Type["IGithubWorkflows"]:
+        """Github workflows class."""
+        raise NotImplementedError
+
 
 class IGithubRepo(metaclass=abstracts.Interface):
 
     @abstracts.interfacemethod
     def __init__(self, github: "IGithubAPI", name: str) -> None:
         raise NotImplementedError
 
@@ -253,14 +273,44 @@
 
     @abstracts.interfacemethod
     async def comment(self, comment: str) -> Any:
         """Add a comment to this issue."""
         raise NotImplementedError
 
 
+class IGithubActions(metaclass=abstracts.Interface):
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def github(self) -> IGithubAPI:
+        """Github API."""
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def repo(self) -> IGithubRepo:
+        """Github repo."""
+        raise NotImplementedError
+
+
+class IGithubWorkflows(metaclass=abstracts.Interface):
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def github(self) -> IGithubAPI:
+        """Github API."""
+        raise NotImplementedError
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def repo(self) -> IGithubRepo:
+        """Github repo."""
+        raise NotImplementedError
+
+
 class IGithubIssues(metaclass=abstracts.Interface):
 
     @abstracts.interfacemethod
     async def create(self, title: str, **kwargs) -> IGithubIssue:
         """Create an issue."""
         raise NotImplementedError
```

### Comparing `aio.api.github-0.2.2/aio.api.github.egg-info/SOURCES.txt` & `aio.api.github-0.2.3/aio.api.github.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,10 +19,12 @@
 aio/api/github/abstract/base.py
 aio/api/github/abstract/commit.py
 aio/api/github/abstract/iterator.py
 aio/api/github/abstract/label.py
 aio/api/github/abstract/release.py
 aio/api/github/abstract/repo.py
 aio/api/github/abstract/tag.py
+aio/api/github/abstract/actions/__init__.py
+aio/api/github/abstract/actions/actions.py
 aio/api/github/abstract/issues/__init__.py
 aio/api/github/abstract/issues/issues.py
 aio/api/github/abstract/issues/tracker.py
```

### Comparing `aio.api.github-0.2.2/backend_shim.py` & `aio.api.github-0.2.3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `aio.api.github-0.2.2/setup.py` & `aio.api.github-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,13 +31,14 @@
         'aio.api.github': (
             'py.typed',
         ),
     },
     'packages': (
         'aio.api.github',
         'aio.api.github.abstract',
+        'aio.api.github.abstract.actions',
         'aio.api.github.abstract.issues',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/toolshed/tree/main/aio.api.github',
-    'version': '0.2.2',
+    'version': '0.2.3',
 })
```

