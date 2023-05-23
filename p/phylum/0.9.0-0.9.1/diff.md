# Comparing `tmp/phylum-0.9.0.tar.gz` & `tmp/phylum-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylum-0.9.0.tar", max compression
+gzip compressed data, was "phylum-0.9.1.tar", max compression
```

## Comparing `phylum-0.9.0.tar` & `phylum-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2022-06-27 19:07:26.607847 phylum-0.9.0/LICENSE
--rw-r--r--   0        0        0     6978 2022-06-27 19:07:26.607847 phylum-0.9.0/README.md
--rw-r--r--   0        0        0     3439 2022-06-27 19:07:51.839946 phylum-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      585 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/__init__.py
--rw-r--r--   0        0        0      167 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/__init__.py
--rw-r--r--   0        0        0      141 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/__main__.py
--rw-r--r--   0        0        0    22783 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/ci_base.py
--rw-r--r--   0        0        0     8729 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/ci_github.py
--rw-r--r--   0        0        0     6438 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/ci_gitlab.py
--rw-r--r--   0        0        0     4947 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/ci_none.py
--rw-r--r--   0        0        0     3897 2022-06-27 19:07:26.607847 phylum-0.9.0/src/phylum/ci/ci_precommit.py
--rw-r--r--   0        0        0     9948 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/ci/cli.py
--rw-r--r--   0        0        0     1813 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/ci/common.py
--rw-r--r--   0        0        0     3254 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/ci/constants.py
--rw-r--r--   0        0        0     2391 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/constants.py
--rw-r--r--   0        0        0      169 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/init/__init__.py
--rw-r--r--   0        0        0      129 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/init/__main__.py
--rw-r--r--   0        0        0    12209 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/init/cli.py
--rw-r--r--   0        0        0     5641 2022-06-27 19:07:26.611847 phylum-0.9.0/src/phylum/init/sig.py
--rw-r--r--   0        0        0        0 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0      273 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/constants.py
--rw-r--r--   0        0        0        0 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/functional/__init__.py
--rw-r--r--   0        0        0     1676 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/functional/test_ci.py
--rw-r--r--   0        0        0     1684 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/functional/test_init.py
--rw-r--r--   0        0        0        0 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     2272 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/unit/test_package_metadata.py
--rw-r--r--   0        0        0     1403 2022-06-27 19:07:26.611847 phylum-0.9.0/tests/unit/test_sig.py
--rw-r--r--   0        0        0     8326 2022-06-27 19:08:48.169499 phylum-0.9.0/setup.py
--rw-r--r--   0        0        0     8423 2022-06-27 19:08:48.170078 phylum-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-07-01 19:52:40.493178 phylum-0.9.1/LICENSE
+-rw-r--r--   0        0        0     6978 2022-07-01 19:52:40.493178 phylum-0.9.1/README.md
+-rw-r--r--   0        0        0     3439 2022-07-01 19:53:00.201433 phylum-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      585 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/__init__.py
+-rw-r--r--   0        0        0      167 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/__init__.py
+-rw-r--r--   0        0        0      141 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/__main__.py
+-rw-r--r--   0        0        0    23002 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/ci_base.py
+-rw-r--r--   0        0        0     8837 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/ci_github.py
+-rw-r--r--   0        0        0     6438 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/ci_gitlab.py
+-rw-r--r--   0        0        0     4947 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/ci_none.py
+-rw-r--r--   0        0        0     3897 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/ci_precommit.py
+-rw-r--r--   0        0        0     9948 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/cli.py
+-rw-r--r--   0        0        0     1567 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/common.py
+-rw-r--r--   0        0        0     3254 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/ci/constants.py
+-rw-r--r--   0        0        0     2391 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/constants.py
+-rw-r--r--   0        0        0      169 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/init/__init__.py
+-rw-r--r--   0        0        0      129 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/init/__main__.py
+-rw-r--r--   0        0        0    12209 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/init/cli.py
+-rw-r--r--   0        0        0     5641 2022-07-01 19:52:40.493178 phylum-0.9.1/src/phylum/init/sig.py
+-rw-r--r--   0        0        0        0 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      273 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/constants.py
+-rw-r--r--   0        0        0        0 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/functional/__init__.py
+-rw-r--r--   0        0        0     1676 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/functional/test_ci.py
+-rw-r--r--   0        0        0     1684 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/functional/test_init.py
+-rw-r--r--   0        0        0        0 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2272 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/unit/test_package_metadata.py
+-rw-r--r--   0        0        0     1403 2022-07-01 19:52:40.493178 phylum-0.9.1/tests/unit/test_sig.py
+-rw-r--r--   0        0        0     8326 2022-07-01 19:54:04.226592 phylum-0.9.1/setup.py
+-rw-r--r--   0        0        0     8423 2022-07-01 19:54:04.227222 phylum-0.9.1/PKG-INFO
```

### Comparing `phylum-0.9.0/LICENSE` & `phylum-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/README.md` & `phylum-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/pyproject.toml` & `phylum-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "phylum"
-version = "0.9.0"
+version = "0.9.1"
 description = "Utilities for integrating Phylum into CI pipelines (and beyond)"
 license = "MIT"
 authors = ["Phylum, Inc. <engineering@phylum.io>"]
 homepage = "https://phylum.io/"
 repository = "https://github.com/phylum-dev/phylum-ci"
 documentation = "https://docs.phylum.io/"
 readme = "README.md"
```

### Comparing `phylum-0.9.0/src/phylum/__init__.py` & `phylum-0.9.1/src/phylum/__init__.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/ci/ci_base.py` & `phylum-0.9.1/src/phylum/ci/ci_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,18 +445,23 @@
         A default secure value will be used when neither of these sources are used to set the value.
         """
         threshold = getattr(self.args, threshold_type, None)
         req_src = "phylum-ci option"
         if threshold is None:
             risk_domain: RiskDomain = PROJECT_THRESHOLD_OPTIONS.get(threshold_type, RiskDomain("", "", ""))
             threshold = project_thresholds.get(risk_domain.project_name)
-            req_src = "project setting"
+            req_src = "project per-axis threshold"
             if threshold is None:
                 threshold = 1.0
                 req_src = "N/A (fail safe)"
+
+            total_threshold = project_thresholds.get("total", 0.0)
+            if threshold < total_threshold:
+                threshold = total_threshold
+                req_src = "project total threshold"
         else:
             # The project risk threshold values returned by the analysis are normalized to [0.0, 1.0].
             # They are converted internally like this because it is more natural to ask users for input
             # as an integer in the range of [0, 100].
             threshold /= 100
         pti = ProjectThresholdInfo(threshold=threshold, req_src=req_src)
         return pti
```

### Comparing `phylum-0.9.0/src/phylum/ci/ci_github.py` & `phylum-0.9.1/src/phylum/ci/ci_github.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,24 @@
 from phylum.constants import REQ_TIMEOUT
 
 
 class CIGitHub(CIBase):
     """Provide methods for a GitHub Actions environment."""
 
     def __init__(self, args: Namespace) -> None:
-        super().__init__(args)
-        self.ci_platform_name = "GitHub Actions"
-
         # This is the recommended workaround for container actions, to avoid the `unsafe repository` error.
+        # It is added before super().__init__(args) so that lockfile change detection will be set properly.
         # See https://github.com/actions/checkout/issues/766 (git CVE-2022-24765) for more detail.
         github_workspace = os.getenv("GITHUB_WORKSPACE", "/github/workspace")
         cmd = f"git config --global --add safe.directory {github_workspace}"
         subprocess.run(cmd.split(), check=True)
 
+        super().__init__(args)
+        self.ci_platform_name = "GitHub Actions"
+
     def _check_prerequisites(self) -> None:
         """Ensure the necessary pre-requisites are met and bail when they aren't.
 
         These are the current pre-requisites for operating within a GitHub Actions Environment:
           * The environment must actually be within GitHub Actions
           * A GitHub token providing `issues` API access is available
           * `pull_request` webhook event payload is available
```

### Comparing `phylum-0.9.0/src/phylum/ci/ci_gitlab.py` & `phylum-0.9.1/src/phylum/ci/ci_gitlab.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/ci/ci_none.py` & `phylum-0.9.1/src/phylum/ci/ci_none.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/ci/ci_precommit.py` & `phylum-0.9.1/src/phylum/ci/ci_precommit.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/ci/cli.py` & `phylum-0.9.1/src/phylum/ci/cli.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/ci/constants.py` & `phylum-0.9.1/src/phylum/ci/constants.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/constants.py` & `phylum-0.9.1/src/phylum/constants.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/init/cli.py` & `phylum-0.9.1/src/phylum/init/cli.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/src/phylum/init/sig.py` & `phylum-0.9.1/src/phylum/init/sig.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/tests/functional/test_ci.py` & `phylum-0.9.1/tests/functional/test_ci.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/tests/functional/test_init.py` & `phylum-0.9.1/tests/functional/test_init.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/tests/unit/test_package_metadata.py` & `phylum-0.9.1/tests/unit/test_package_metadata.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/tests/unit/test_sig.py` & `phylum-0.9.1/tests/unit/test_sig.py`

 * *Files identical despite different names*

### Comparing `phylum-0.9.0/setup.py` & `phylum-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 entry_points = \
 {'console_scripts': ['phylum-ci = phylum.ci.cli:script_main',
                      'phylum-init = phylum.init.cli:main']}
 
 setup_kwargs = {
     'name': 'phylum',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Utilities for integrating Phylum into CI pipelines (and beyond)',
     'long_description': '# phylum-ci\n[![PyPI](https://img.shields.io/pypi/v/phylum)](https://pypi.org/project/phylum/)\n![PyPI - Status](https://img.shields.io/pypi/status/phylum)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/phylum)](https://pypi.org/project/phylum/)\n[![GitHub](https://img.shields.io/github/license/phylum-dev/phylum-ci)][license]\n[![GitHub issues](https://img.shields.io/github/issues/phylum-dev/phylum-ci)][issues]\n![GitHub last commit](https://img.shields.io/github/last-commit/phylum-dev/phylum-ci)\n[![GitHub Workflow Status (branch)][workflow_shield]][workflow_test]\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)][CoC]\n\nUtilities for integrating Phylum into CI pipelines (and beyond)\n\n[license]: https://github.com/phylum-dev/phylum-ci/blob/main/LICENSE\n[issues]: https://github.com/phylum-dev/phylum-ci/issues\n[workflow_shield]: https://img.shields.io/github/workflow/status/phylum-dev/phylum-ci/Test/main?label=Test&logo=GitHub\n[workflow_test]: https://github.com/phylum-dev/phylum-ci/actions/workflows/test.yml\n[CoC]: https://github.com/phylum-dev/phylum-ci/blob/main/CODE_OF_CONDUCT.md\n[contributing]: https://github.com/phylum-dev/phylum-ci/blob/main/CONTRIBUTING.md\n[changelog]: https://github.com/phylum-dev/phylum-ci/blob/main/CHANGELOG.md\n[security]: https://github.com/phylum-dev/phylum-ci/blob/main/docs/security.md\n\n## Installation and usage\n\n### Installation\n\nThe `phylum` Python package is pip installable for the environment of your choice:\n\n```sh\npip install phylum\n```\n\nIt can also be installed in an isolated environment with the excellent [`pipx` tool](https://pypa.github.io/pipx/):\n\n```sh\n# Globally install the app(s) on your system in an isolated virtual environment for the package\npipx install phylum\n\n# Use the apps from the package in an ephemeral environment\npipx run --spec phylum phylum-init <options>\npipx run --spec phylum phylum-ci <options>\n```\n\nThese installation methods require Python 3.7+ to run. For a self contained environment, consider using the Docker\nimage as described below.\n\n### Usage\n\nThe `phylum` Python package exposes its functionality with a command line interface (CLI).\nTo view the options available from the CLI, print the help message from one of the scripts provided as entry points:\n\n```sh\nphylum-init -h\nphylum-ci -h\n```\n\nThe functionality can also be accessed by calling the module:\n\n```sh\npython -m phylum.init -h\npython -m phylum.ci -h\n```\n\nThe functionality is also exposed in the form of a Docker image:\n\n```sh\n# Get the `latest` tagged image\ndocker pull phylumio/phylum-ci\n\n# View the help\ndocker run --rm phylumio/phylum-ci phylum-ci --help\n\n# Export a Phylum token (e.g., from `phylum auth token`)\nexport PHYLUM_API_KEY=$(phylum auth token)\n\n# Run it from a git repo directory containing a `.phylum_project` and a lockfile\ndocker run -it --rm -e PHYLUM_API_KEY --mount type=bind,src=$(pwd),dst=/phylum -w /phylum phylumio/phylum-ci\n```\n\nThe Docker image contains `git` and the installed `phylum` Python package.\nIt also contains an installed version of the Phylum CLI.\nAn advantage of using the Docker image is that the complete environment is packaged and made available with components\nthat are known to work together.\n\nWhen using the `latest` tagged image, the version of the Phylum CLI is the `latest` available.\nThere are additional image tag options available to specify a specific release of the `phylum-ci` project and a specific\nversion of the Phylum CLI, in the form of `<phylum-ci version>-CLIv<Phylum CLI version>`. Here are image tag examples:\n\n```sh\n# Get the most current release of *both* `phylum-ci` and the Phylum CLI\ndocker pull phylumio/phylum-ci:latest\n\n# Get the image with `phylum-ci` version 0.8.0 and Phylum CLI version 3.5.0\ndocker pull phylumio/phylum-ci:0.8.0-CLIv3.5.0\n```\n\n#### `phylum-init` Script Entry Point\n\nThe `phylum-init` script can be used to fetch and install the Phylum CLI.\nIt will attempt to install the latest released version of the CLI but can be specified to fetch a specific version.\nIt will attempt to automatically determine the correct CLI release, based on the platform where the script is run, but\na specific release target can be specified.\nIt will accept a Phylum token from an environment variable or specified as an option, but will also function in the case\nthat no token is provided. This can be because there is already a token set that should continue to be used or because\nno token exists and one will need to be manually created or set, after the CLI is installed.\n\n#### `phylum-ci` Script Entry Point\n\nThe `phylum-ci` script is for analyzing lockfile changes.\nThe script can be used locally or from within a Continuous Integration (CI) environment.\nIt will attempt to detect the CI platform based on the environment from which it is run and act accordingly.\nThe current CI platforms/environments supported are:\n\n* GitLab CI\n  * See the [GitLab CI Integration documentation][gitlab_docs] for more info\n\n* GitHub Actions\n  * See the [GitHub Actions Integration documentation][github_docs] for more info\n\n* None (local use)\n  * This is the "fall-through" case used when no other environment is detected\n  * Can be useful to analyze lockfiles locally, prior to or after submitting a pull/merge request (PR/MR) to a CI system\n    * Establishing a successful submission prior to submitting a PR/MR to a CI system\n    * Troubleshooting after submitting a PR/MR to a CI system and getting unexpected results\n\n[gitlab_docs]: https://github.com/phylum-dev/phylum-ci/blob/main/docs/gitlab_ci.md\n[github_docs]: https://github.com/phylum-dev/phylum-ci/blob/main/docs/github_actions.md\n\n## License\n\nMIT - with complete text available in the [LICENSE][license] file.\n\n## Contributing\n\nSuggestions and help are welcome. Feel free to open an issue or otherwise contribute.\nMore information is available on the [contributing documentation][contributing] page.\n\n## Code of Conduct\n\nEveryone participating in the `phylum-ci` project, and in particular in the issue tracker and pull requests, is\nexpected to treat other people with respect and more generally to follow the guidelines articulated in the\n[Code of Conduct][CoC].\n\n## Security Disclosures\n\nFound a security issue in this repository? See the [security policy][security]\nfor details on coordinated disclosure.\n\n## Change log\n\nAll notable changes to this project are documented in the [CHANGELOG][changelog].\n\nThe format of the change log is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),\nand this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).\nThe entries in the changelog are primarily automatically generated through the use of\n[conventional commits](https://www.conventionalcommits.org) and the\n[Python Semantic Release](https://python-semantic-release.readthedocs.io/en/latest/index.html) tool.\nHowever, some entries may be manually edited, where it helps for clarity and understanding.\n',
     'author': 'Phylum, Inc.',
     'author_email': 'engineering@phylum.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://phylum.io/',
```

### Comparing `phylum-0.9.0/PKG-INFO` & `phylum-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylum
-Version: 0.9.0
+Version: 0.9.1
 Summary: Utilities for integrating Phylum into CI pipelines (and beyond)
 Home-page: https://phylum.io/
 License: MIT
 Keywords: dependency,security,CI,integration
 Author: Phylum, Inc.
 Author-email: engineering@phylum.io
 Requires-Python: >=3.7,<4.0
```

