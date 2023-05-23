# Comparing `tmp/poetry_source_env-1.1.1.tar.gz` & `tmp/poetry_source_env-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_source_env-1.1.1.tar", max compression
+gzip compressed data, was "poetry_source_env-2.0.0.tar", max compression
```

## Comparing `poetry_source_env-1.1.1.tar` & `poetry_source_env-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/LICENSE.md
--rw-r--r--   0        0        0     4005 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/poetry_source_env/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/poetry_source_env/plugin.py
--rw-r--r--   0        0        0      737 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 poetry_source_env-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3950 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/poetry_source_env/__init__.py
+-rw-r--r--   0        0        0     2787 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/poetry_source_env/plugin.py
+-rw-r--r--   0        0        0      739 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4785 1970-01-01 00:00:00.000000 poetry_source_env-2.0.0/PKG-INFO
```

### Comparing `poetry_source_env-1.1.1/LICENSE.md` & `poetry_source_env-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `poetry_source_env-1.1.1/README.md` & `poetry_source_env-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,42 +23,39 @@
 
 Normally, you would define a package source in `pyproject.toml` like this:
 
 ```toml
 [[tool.poetry.source]]
 name = "foo"
 url = "https://foo.bar/simple"
-default = false
-secondary = false
+priority = "supplemental"
 
 ```
 
 With poetry-source-env, you can define this source via environment variables, similar to how you can already
 configure [publishable repositories](https://python-poetry.org/docs/repositories/#publishable-repositories:~:text=Alternatively%2C%20you%20can%20use%20environment%20variables%20to%20provide%20the%20credentials%3A):
 
 ```bash
 export POETRY_REPOSITORIES_FOO_URL=https://foo.bar/simple
-export POETRY_REPOSITORIES_FOO_DEFAULT=false
-export POETRY_REPOSITORIES_FOO_SECONDARY=false
+export POETRY_REPOSITORIES_FOO_PRIORITY=supplemental
 ```
 
 If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal its name or URL, in whole or
 in part, behind environment variables:
 
 ```bash
 export FOO_INDEX_NAME="foo"
 export FOO_INDEX_URL="https://foo.bar/simple"
 ```
 
 ```toml
 [[tool.poetry.source]]
 name = "${FOO_INDEX_NAME}"
 url = "${FOO_INDEX_URL}"
-default = false
-secondary = false
+priority = "supplemental"
 
 ```
 
 If your source requires authentication, Poetry already supports defining its credentials via environment variables:
 
 ```bash
 export POETRY_HTTP_BASIC_FOO_USERNAME=celsiusnarhwal
```

### Comparing `poetry_source_env-1.1.1/poetry_source_env/plugin.py` & `poetry_source_env-2.0.0/poetry_source_env/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import re
 from os.path import expandvars
 
 from cleo.io.io import IO
 from dict_deep import deep_get
-from poetry.core.toml.file import TOMLFile
 from poetry.plugins.plugin import Plugin
 from poetry.poetry import Poetry
 from poetry.repositories.legacy_repository import LegacyRepository
+from poetry.repositories.repository_pool import Priority
+from poetry.toml.file import TOMLFile
 from pydantic import BaseSettings, validate_arguments
 from typing_extensions import Self
 
 
 class PSPConfig(BaseSettings):
     prefix: str = "POETRY_REPOSITORIES_"
     env: bool = True
@@ -38,24 +39,29 @@
                     repositories[match.group("name").lower().replace("_", "-")] = {
                         "env_name": match.group("name"),
                         "url": os.environ[env_key],
                     }
 
             for name, repository in repositories.items():
                 repo = LegacyRepository(name, repository["url"])
-                default = (
-                    os.getenv(f"{config.prefix}{repository['env_name']}_DEFAULT")
-                    == "true"
-                )
-                secondary = (
-                    os.getenv(f"{config.prefix}{repository['env_name']}_SECONDARY")
-                    == "true"
+
+                priority_name = os.getenv(
+                    f"{config.prefix}{repository['env_name']}_PRIORITY", "primary"
                 )
 
-                poetry.pool.add_repository(repo, default, secondary)
+                priorities = {
+                    "default": Priority.DEFAULT,
+                    "primary": Priority.PRIMARY,
+                    "supplemental": Priority.SUPPLEMENTAL,
+                    "explicit": Priority.EXPLICIT,
+                }
+
+                priority = priorities.get(priority_name.casefold(), Priority.PRIMARY)
+
+                poetry.pool.add_repository(repo, priority=priority)
 
         if config.toml:
             for repository in poetry.pool.repositories:
                 definition = next(
                     (
                         source
                         for source in poetry.get_sources()
@@ -65,10 +71,8 @@
                 )
 
                 if definition:
                     poetry.pool.remove_repository(repository.name)
                     repo = LegacyRepository(
                         expandvars(definition.name), expandvars(definition.url)
                     )
-                    poetry.pool.add_repository(
-                        repo, definition.default, definition.secondary
-                    )
+                    poetry.pool.add_repository(repo, priority=definition.priority)
```

### Comparing `poetry_source_env-1.1.1/PKG-INFO` & `poetry_source_env-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: poetry-source-env
-Version: 1.1.1
+Version: 2.0.0
 Summary: Load Poetry package sources from environment variables
 Home-page: https://github.com/celsiusnarhwal/poetry-source-env
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
-Requires-Dist: poetry (>=1.2,<2.0)
+Requires-Dist: poetry (>=1.5.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Project-URL: Repository, https://github.com/celsiusnarhwal/poetry-source-env
 Description-Content-Type: text/markdown
 
 # poetry-source-env
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-source-env?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/poetry-source-env)
@@ -44,42 +44,39 @@
 
 Normally, you would define a package source in `pyproject.toml` like this:
 
 ```toml
 [[tool.poetry.source]]
 name = "foo"
 url = "https://foo.bar/simple"
-default = false
-secondary = false
+priority = "supplemental"
 
 ```
 
 With poetry-source-env, you can define this source via environment variables, similar to how you can already
 configure [publishable repositories](https://python-poetry.org/docs/repositories/#publishable-repositories:~:text=Alternatively%2C%20you%20can%20use%20environment%20variables%20to%20provide%20the%20credentials%3A):
 
 ```bash
 export POETRY_REPOSITORIES_FOO_URL=https://foo.bar/simple
-export POETRY_REPOSITORIES_FOO_DEFAULT=false
-export POETRY_REPOSITORIES_FOO_SECONDARY=false
+export POETRY_REPOSITORIES_FOO_PRIORITY=supplemental
 ```
 
 If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal its name or URL, in whole or
 in part, behind environment variables:
 
 ```bash
 export FOO_INDEX_NAME="foo"
 export FOO_INDEX_URL="https://foo.bar/simple"
 ```
 
 ```toml
 [[tool.poetry.source]]
 name = "${FOO_INDEX_NAME}"
 url = "${FOO_INDEX_URL}"
-default = false
-secondary = false
+priority = "supplemental"
 
 ```
 
 If your source requires authentication, Poetry already supports defining its credentials via environment variables:
 
 ```bash
 export POETRY_HTTP_BASIC_FOO_USERNAME=celsiusnarhwal
```

