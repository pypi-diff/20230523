# Comparing `tmp/gh_env_manager-0.4.0.tar.gz` & `tmp/gh_env_manager-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_env_manager-0.4.0.tar", max compression
+gzip compressed data, was "gh_env_manager-0.4.1.tar", max compression
```

## Comparing `gh_env_manager-0.4.0.tar` & `gh_env_manager-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-02-17 08:10:45.047583 gh_env_manager-0.4.0/LICENSE
--rw-r--r--   0        0        0     6095 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/gh_env_manager/__init__.py
--rw-r--r--   0        0        0    10260 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/gh_env_manager/github_api_class.py
--rw-r--r--   0        0        0     1372 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/gh_env_manager/github_api_implementations.py
--rw-r--r--   0        0        0     8173 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/gh_env_manager/main.py
--rw-r--r--   0        0        0     1496 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/gh_env_manager/secret_variable_entity_class.py
--rw-r--r--   0        0        0     8149 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/gh_env_manager/yaml_env_class.py
--rw-r--r--   0        0        0      602 2023-02-17 08:10:45.051583 gh_env_manager-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 gh_env_manager-0.4.0/setup.py
--rw-r--r--   0        0        0     6809 1970-01-01 00:00:00.000000 gh_env_manager-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6095 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/gh_env_manager/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/gh_env_manager/github_api_class.py
+-rw-r--r--   0        0        0     1372 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/gh_env_manager/github_api_implementations.py
+-rw-r--r--   0        0        0     8173 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/gh_env_manager/main.py
+-rw-r--r--   0        0        0     1496 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/gh_env_manager/secret_variable_entity_class.py
+-rw-r--r--   0        0        0     8149 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/gh_env_manager/yaml_env_class.py
+-rw-r--r--   0        0        0      607 2023-05-23 00:57:15.019029 gh_env_manager-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6806 1970-01-01 00:00:00.000000 gh_env_manager-0.4.1/PKG-INFO
```

### Comparing `gh_env_manager-0.4.0/LICENSE` & `gh_env_manager-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/README.md` & `gh_env_manager-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/gh_env_manager/github_api_class.py` & `gh_env_manager-0.4.1/gh_env_manager/github_api_class.py`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/gh_env_manager/github_api_implementations.py` & `gh_env_manager-0.4.1/gh_env_manager/github_api_implementations.py`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/gh_env_manager/main.py` & `gh_env_manager-0.4.1/gh_env_manager/main.py`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/gh_env_manager/secret_variable_entity_class.py` & `gh_env_manager-0.4.1/gh_env_manager/secret_variable_entity_class.py`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/gh_env_manager/yaml_env_class.py` & `gh_env_manager-0.4.1/gh_env_manager/yaml_env_class.py`

 * *Files identical despite different names*

### Comparing `gh_env_manager-0.4.0/pyproject.toml` & `gh_env_manager-0.4.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "gh-env-manager"
-version = "0.4.0"
+version = "0.4.1"
 description = "A CLI tool to update GitHub Actions secrets and variables from a YAML file"
 authors = ["Antti Viitala <tied02beaches@icloud.com>"]
 readme = "README.md"
 packages = [{include = "gh_env_manager"}]
 
 [tool.poetry.scripts]
 gh-env-manager = "gh_env_manager.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = {extras = ["all"], version = ">=0.7,<0.10"}
 requests = "^2.28.2"
 pyyaml = "^6.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pynacl = "^1.5.0"
 
 [build-system]
```

### Comparing `gh_env_manager-0.4.0/setup.py` & `gh_env_manager-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gh-env-manager
+Version: 0.4.1
+Summary: A CLI tool to update GitHub Actions secrets and variables from a YAML file
+Author: Antti Viitala
+Author-email: tied02beaches@icloud.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pynacl (>=1.5.0,<2.0.0)
+Requires-Dist: pytest (>=7.2.1,<8.0.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: typer[all] (>=0.7,<0.10)
+Description-Content-Type: text/markdown
+
+# GitHub Environment Manager - `gh_env_manager`
+
+This tool is in early development - use with care and expect to find bugs, When you do, please raise issues to help guide development 😊
+
+[![PyPI version](https://badge.fury.io/py/gh-env-manager.svg)](https://badge.fury.io/py/gh-env-manager)
+![Pytest coverage](./.github/badges/coverage.svg)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=Antvirf_gh-environment-manager&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=Antvirf_gh-environment-manager)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=Antvirf_gh-environment-manager&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=Antvirf_gh-environment-manager)
+![Python](https://img.shields.io/badge/python-3.9%20-blue)
+
+GitHub Environment Manager helps you maintain GitHub Actions [Secrets](https://docs.github.com/en/rest/actions/secrets?apiVersion=2022-11-28) and [Variables](https://docs.github.com/en/rest/actions/variables?apiVersion=2022-11-28) across your repositories, and [environments](https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment) within them. You provide your target state in the form of a `YAML` file - the desired Secrets and Variables that your repositories and their environments should contain - and the tool does the rest.
+
+## Installation
+
+```bash
+pip install gh-env-manager
+```
+
+---
+
+## Quick start to update entities in your repositories
+
+`gh-env-manager` requires as an input a `YAML` file that describes the target state of your GitHub repository (or repositories) and its (their) Secrets and Variables. It does **not** create any repositories or environments for you - so every repository, and every environment within your repositories, that you add to the configuration must exist already. The tool maintains the entities - Secrets and Variables - within.
+
+1. Install this tool with `pip install gh-env-manager`
+1. Create a GitHub personal access token following [this guide from GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
+1. Create a `YAML` file that describes your target state, following the format below. You can also check the [example used for tests](./tests/test.yml).
+
+    ```yaml
+    GH_SECRET_SYNC_KEY: <your GitHub personal access token>
+    
+    repositories:
+      username/repositoryname: # e.g. Antvirf/gh-environment-manager 
+        secrets:
+          - YOUR_SECRET: "something"
+        variables:
+          - YOUR_VARIABLE: "something" 
+        environments:
+          dev: # assuming 'dev' environment exists in your repository
+            secrets:
+              - YOUR_DEV_SECRET: "something"
+            variables:
+              - YOUR_DEV_VARIABLE: "something"
+
+      # you can add as many repositories as desired
+      username/repositoryname: #...
+        secrets:
+          ...
+        variables:
+          ...
+    ```
+
+1. Run `gh-env-manager fetch ./path_to_your_yaml_file` to get current state of your repositories
+1. Run `gh-env-manager update ./path_to_your_yaml_file` to push the contents of the `YAML` file to your repositories
+    * By default, nothing is overwritten - if an entity exists already, it is **NOT** updated. Use the `--overwrite` flag to enable that behaviour.
+    * By default, nothing is deleted - if your repository has an entity that is not in the `YAML` file, it is ignored. Use the `--delete-nonexisting` or `--delete-nonexisting-without-prompt` to delete any secret or variable from your repository that was missing from your input `YAML` file.
+
+## Usage
+
+`PATH_TO_FILE` is always required for each command.
+
+```bash
+$ gh_env_manager [COMMANDS] PATH_TO_FILE [OPTIONS]
+
+# examples
+$ gh_env_manager read .env.yaml
+$ gh_env_manager fetch .env.yaml
+$ gh_env_manager update .env.yaml
+
+# to overwrite existing entries
+$ gh_env_manager update .env.yaml --overwrite 
+
+# to delete any secret/variable missing from your YAML
+$ gh_env_manager update .env.yaml --delete-nonexisting
+
+# fully sync your repository with the contents of the yaml by updating all values, and deleting any that are not present
+$ gh_env_manager update .env.yaml --overwrite --delete-nonexisting-without-prompt 
+```
+
+### Commands
+
+* `read`:    Read given YAML file and output the interpreted contents.
+* `fetch`:   Fetch all secrets and all variables from the specific GitHub repositories provided in your environment YAML file.
+* `update`:  Update secrets and variables of the GitHub repositories using data from the provided YAML file. By default, existing secrets or variables are NOT overwritten. Try `gh-env-manager update --help` to view the available options.
+
+### Options for `update`
+
+* `-o, --overwrite`: If enabled, overwrite existing secrets and values in GitHub to match the provided YAML file.  [default: False]
+* `-d, --delete-nonexisting`: If enabled, delete secrets and variables that are not found in the provided YAML file.  [default: False]
+* `--delete-nonexisting-without-prompt`: Applies the same commands as `delete_nonexisting`, but without prompting the user for confirmation. [default: False]
+<!-- 
+* `--install-completion`: Install completion for the current shell.
+* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
+* `--help`: Show this message and exit. -->
+
+## FAQ
 
-packages = \
-['gh_env_manager']
+1. Why do secrets sometimes state their value as `None`?
+    1. GitHub Secrets API does **NOT** support fetching the *value* of a secret, and hence they are shown as `None` when data coming *from* GitHub is output.
 
-package_data = \
-{'': ['*']}
+## Known missing features & potential roadmap items
 
-install_requires = \
-['pynacl>=1.5.0,<2.0.0',
- 'pytest-cov>=4.0.0,<5.0.0',
- 'pytest>=7.2.1,<8.0.0',
- 'pyyaml>=6.0,<7.0',
- 'requests>=2.28.2,<3.0.0',
- 'typer[all]>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['gh-env-manager = gh_env_manager.main:app']}
-
-setup_kwargs = {
-    'name': 'gh-env-manager',
-    'version': '0.4.0',
-    'description': 'A CLI tool to update GitHub Actions secrets and variables from a YAML file',
-    'long_description': '# GitHub Environment Manager - `gh_env_manager`\n\nThis tool is in early development - use with care and expect to find bugs, When you do, please raise issues to help guide development 😊\n\n[![PyPI version](https://badge.fury.io/py/gh-env-manager.svg)](https://badge.fury.io/py/gh-env-manager)\n![Pytest coverage](./.github/badges/coverage.svg)\n[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=Antvirf_gh-environment-manager&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=Antvirf_gh-environment-manager)\n[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=Antvirf_gh-environment-manager&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=Antvirf_gh-environment-manager)\n![Python](https://img.shields.io/badge/python-3.9%20-blue)\n\nGitHub Environment Manager helps you maintain GitHub Actions [Secrets](https://docs.github.com/en/rest/actions/secrets?apiVersion=2022-11-28) and [Variables](https://docs.github.com/en/rest/actions/variables?apiVersion=2022-11-28) across your repositories, and [environments](https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment) within them. You provide your target state in the form of a `YAML` file - the desired Secrets and Variables that your repositories and their environments should contain - and the tool does the rest.\n\n## Installation\n\n```bash\npip install gh-env-manager\n```\n\n---\n\n## Quick start to update entities in your repositories\n\n`gh-env-manager` requires as an input a `YAML` file that describes the target state of your GitHub repository (or repositories) and its (their) Secrets and Variables. It does **not** create any repositories or environments for you - so every repository, and every environment within your repositories, that you add to the configuration must exist already. The tool maintains the entities - Secrets and Variables - within.\n\n1. Install this tool with `pip install gh-env-manager`\n1. Create a GitHub personal access token following [this guide from GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)\n1. Create a `YAML` file that describes your target state, following the format below. You can also check the [example used for tests](./tests/test.yml).\n\n    ```yaml\n    GH_SECRET_SYNC_KEY: <your GitHub personal access token>\n    \n    repositories:\n      username/repositoryname: # e.g. Antvirf/gh-environment-manager \n        secrets:\n          - YOUR_SECRET: "something"\n        variables:\n          - YOUR_VARIABLE: "something" \n        environments:\n          dev: # assuming \'dev\' environment exists in your repository\n            secrets:\n              - YOUR_DEV_SECRET: "something"\n            variables:\n              - YOUR_DEV_VARIABLE: "something"\n\n      # you can add as many repositories as desired\n      username/repositoryname: #...\n        secrets:\n          ...\n        variables:\n          ...\n    ```\n\n1. Run `gh-env-manager fetch ./path_to_your_yaml_file` to get current state of your repositories\n1. Run `gh-env-manager update ./path_to_your_yaml_file` to push the contents of the `YAML` file to your repositories\n    * By default, nothing is overwritten - if an entity exists already, it is **NOT** updated. Use the `--overwrite` flag to enable that behaviour.\n    * By default, nothing is deleted - if your repository has an entity that is not in the `YAML` file, it is ignored. Use the `--delete-nonexisting` or `--delete-nonexisting-without-prompt` to delete any secret or variable from your repository that was missing from your input `YAML` file.\n\n## Usage\n\n`PATH_TO_FILE` is always required for each command.\n\n```bash\n$ gh_env_manager [COMMANDS] PATH_TO_FILE [OPTIONS]\n\n# examples\n$ gh_env_manager read .env.yaml\n$ gh_env_manager fetch .env.yaml\n$ gh_env_manager update .env.yaml\n\n# to overwrite existing entries\n$ gh_env_manager update .env.yaml --overwrite \n\n# to delete any secret/variable missing from your YAML\n$ gh_env_manager update .env.yaml --delete-nonexisting\n\n# fully sync your repository with the contents of the yaml by updating all values, and deleting any that are not present\n$ gh_env_manager update .env.yaml --overwrite --delete-nonexisting-without-prompt \n```\n\n### Commands\n\n* `read`:    Read given YAML file and output the interpreted contents.\n* `fetch`:   Fetch all secrets and all variables from the specific GitHub repositories provided in your environment YAML file.\n* `update`:  Update secrets and variables of the GitHub repositories using data from the provided YAML file. By default, existing secrets or variables are NOT overwritten. Try `gh-env-manager update --help` to view the available options.\n\n### Options for `update`\n\n* `-o, --overwrite`: If enabled, overwrite existing secrets and values in GitHub to match the provided YAML file.  [default: False]\n* `-d, --delete-nonexisting`: If enabled, delete secrets and variables that are not found in the provided YAML file.  [default: False]\n* `--delete-nonexisting-without-prompt`: Applies the same commands as `delete_nonexisting`, but without prompting the user for confirmation. [default: False]\n<!-- \n* `--install-completion`: Install completion for the current shell.\n* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n* `--help`: Show this message and exit. -->\n\n## FAQ\n\n1. Why do secrets sometimes state their value as `None`?\n    1. GitHub Secrets API does **NOT** support fetching the *value* of a secret, and hence they are shown as `None` when data coming *from* GitHub is output.\n\n## Known missing features & potential roadmap items\n\n* Support for GitHub Organizations (see API ref for [org Variables](https://docs.github.com/en/rest/actions/variables?apiVersion=2022-11-28#list-organization-variables), [org Secrets](https://docs.github.com/en/rest/actions/secrets?apiVersion=2022-11-28#list-organization-secrets))\n  * Potentially support for scoped secrets and variables (ability to set visibility at repo level)\n',
-    'author': 'Antti Viitala',
-    'author_email': 'tied02beaches@icloud.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+* Support for GitHub Organizations (see API ref for [org Variables](https://docs.github.com/en/rest/actions/variables?apiVersion=2022-11-28#list-organization-variables), [org Secrets](https://docs.github.com/en/rest/actions/secrets?apiVersion=2022-11-28#list-organization-secrets))
+  * Potentially support for scoped secrets and variables (ability to set visibility at repo level)
 
-
-setup(**setup_kwargs)
```

